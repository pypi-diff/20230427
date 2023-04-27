# Comparing `tmp/datasette-1.0a1.tar.gz` & `tmp/datasette-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-1.0a1.tar", last modified: Thu Dec  1 21:52:30 2022, max compression
+gzip compressed data, was "datasette-1.0a2.tar", last modified: Thu Dec 15 02:14:46 2022, max compression
```

## Comparing `datasette-1.0a1.tar` & `datasette-1.0a2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.347755 datasette-1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-01 21:52:16.000000 datasette-1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-01 21:52:16.000000 datasette-1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2022-12-01 21:52:30.347755 datasette-1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2022-12-01 21:52:16.000000 datasette-1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.343755 datasette-1.0a1/datasette/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/actor_auth_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)    62421 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/blob_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/default_magic_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/default_menu_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/default_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/forbidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/handle_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.343755 datasette-1.0a1/datasette/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/publish/cloudrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/publish/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/publish/heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/sql_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.343755 datasette-1.0a1/datasette/static/
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   367207 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/cm-editor-6.0.1.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/cm-editor-6.0.1.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/json-format-highlight-1.0.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    41376 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/sql-formatter-2.3.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/static/table.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.347755 datasette-1.0a1/datasette/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_close_open_menus.html
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_codemirror.html
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_codemirror_foot.html
--rw-r--r--   0 runner    (1001) docker     (123)      422 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_crumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_description_source_license.html
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_facet_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_suggested_facets.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/allow_debug.html
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/api_explorer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/create_token.html
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/database.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/messages_debug.html
--rw-r--r--   0 runner    (1001) docker     (123)    24496 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/patterns.html
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/permissions_debug.html
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/query.html
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/row.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/show_json.html
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/url_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.347755 datasette-1.0a1/datasette/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    36493 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/baseconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/internal_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/shutil_backport.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.347755 datasette-1.0a1/datasette/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20813 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31053 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/row.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/special.py
--rw-r--r--   0 runner    (1001) docker     (123)    48240 2022-12-01 21:52:16.000000 datasette-1.0a1/datasette/views/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 21:52:30.343755 datasette-1.0a1/datasette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2022-12-01 21:52:30.000000 datasette-1.0a1/datasette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-01 21:52:30.000000 datasette-1.0a1/datasette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 21:52:30.000000 datasette-1.0a1/datasette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-01 21:52:30.000000 datasette-1.0a1/datasette.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      510 2022-12-01 21:52:30.000000 datasette-1.0a1/datasette.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-01 21:52:30.000000 datasette-1.0a1/datasette.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-01 21:52:30.351755 datasette-1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2022-12-01 21:52:16.000000 datasette-1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.815858 datasette-1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-15 02:14:38.000000 datasette-1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-15 02:14:38.000000 datasette-1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2022-12-15 02:14:46.819858 datasette-1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2022-12-15 02:14:38.000000 datasette-1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.811858 datasette-1.0a2/datasette/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/actor_auth_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65319 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/blob_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23179 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/default_magic_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/default_menu_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/default_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/handle_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.811858 datasette-1.0a2/datasette/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/publish/cloudrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/publish/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/publish/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/sql_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.815858 datasette-1.0a2/datasette/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    16205 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   367207 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/cm-editor-6.0.1.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/cm-editor-6.0.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/json-format-highlight-1.0.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41376 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/sql-formatter-2.3.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/static/table.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.815858 datasette-1.0a2/datasette/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_close_open_menus.html
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_codemirror.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_codemirror_foot.html
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_crumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_description_source_license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_facet_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_suggested_facets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/allow_debug.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/api_explorer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/create_token.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/database.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/messages_debug.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24496 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/patterns.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/permissions_debug.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/show_json.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/url_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.815858 datasette-1.0a2/datasette/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    36493 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13587 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/baseconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/internal_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/shutil_backport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.815858 datasette-1.0a2/datasette/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20813 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28816 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51252 2022-12-15 02:14:38.000000 datasette-1.0a2/datasette/views/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 02:14:46.811858 datasette-1.0a2/datasette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2022-12-15 02:14:46.000000 datasette-1.0a2/datasette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-15 02:14:46.000000 datasette-1.0a2/datasette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 02:14:46.000000 datasette-1.0a2/datasette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-15 02:14:46.000000 datasette-1.0a2/datasette.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2022-12-15 02:14:46.000000 datasette-1.0a2/datasette.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-15 02:14:46.000000 datasette-1.0a2/datasette.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-15 02:14:46.819858 datasette-1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2022-12-15 02:14:38.000000 datasette-1.0a2/setup.py
```

### Comparing `datasette-1.0a1/LICENSE` & `datasette-1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/PKG-INFO` & `datasette-1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette
-Version: 1.0a1
+Version: 1.0a2
 Summary: An open source multi-tool for exploring and publishing data
 Home-page: https://datasette.io/
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.datasette.io/en/stable/
 Project-URL: Changelog, https://docs.datasette.io/en/stable/changelog.html
 Project-URL: Live demo, https://latest.datasette.io/
```

### Comparing `datasette-1.0a1/README.md` & `datasette-1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/actor_auth_cookie.py` & `datasette-1.0a2/datasette/actor_auth_cookie.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/app.py` & `datasette-1.0a2/datasette/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Sequence, Union, Tuple, Optional
+from typing import Sequence, Union, Tuple, Optional, Dict, Iterable
 import asgi_csrf
 import collections
 import datetime
 import functools
 import glob
 import hashlib
 import httpx
@@ -12,14 +12,15 @@
 import json
 import os
 import pkg_resources
 import re
 import secrets
 import sys
 import threading
+import time
 import urllib.parse
 from concurrent import futures
 from pathlib import Path
 
 from markupsafe import Markup, escape
 from itsdangerous import URLSafeSerializer
 from jinja2 import ChoiceLoader, Environment, FileSystemLoader, PrefixLoader
@@ -36,15 +37,15 @@
     ApiExplorerView,
     CreateTokenView,
     LogoutView,
     AllowDebugView,
     PermissionsDebugView,
     MessagesDebugView,
 )
-from .views.table import TableView, TableInsertView, TableDropView
+from .views.table import TableView, TableInsertView, TableUpsertView, TableDropView
 from .views.row import RowView, RowDeleteView, RowUpdateView
 from .renderer import json_renderer
 from .url_builder import Urls
 from .database import Database, QueryInterrupted
 
 from .utils import (
     PrefixedUrlString,
@@ -190,14 +191,16 @@
     "hash_urls": _HASH_URLS_REMOVED,
     "default_cache_ttl_hashed": _HASH_URLS_REMOVED,
 }
 DEFAULT_SETTINGS = {option.name: option.default for option in SETTINGS}
 
 FAVICON_PATH = app_root / "datasette" / "static" / "favicon.png"
 
+DEFAULT_NOT_SET = object()
+
 
 async def favicon(request, send):
     await asgi_send_file(
         send,
         str(FAVICON_PATH),
         content_type="image/png",
         headers={"Cache-Control": "max-age=3600, immutable, public"},
@@ -260,14 +263,15 @@
                 immutable_filenames = [i["file"] for i in inspect_data.values()]
                 immutables = [
                     f for f in self.files if Path(f).name in immutable_filenames
                 ]
         self.inspect_data = inspect_data
         self.immutables = set(immutables or [])
         self.databases = collections.OrderedDict()
+        self.permissions = {}  # .invoke_startup() will populate this
         try:
             self._refresh_schemas_lock = asyncio.Lock()
         except RuntimeError as rex:
             # Workaround for intermittent test failure, see:
             # https://github.com/simonw/datasette/issues/1802
             if "There is no current event loop in thread" in str(rex):
                 loop = asyncio.new_event_loop()
@@ -426,28 +430,85 @@
     def urls(self):
         return Urls(self)
 
     async def invoke_startup(self):
         # This must be called for Datasette to be in a usable state
         if self._startup_invoked:
             return
+        # Register permissions, but watch out for duplicate name/abbr
+        names = {}
+        abbrs = {}
+        for hook in pm.hook.register_permissions(datasette=self):
+            if hook:
+                for p in hook:
+                    if p.name in names and p != names[p.name]:
+                        raise StartupError(
+                            "Duplicate permission name: {}".format(p.name)
+                        )
+                    if p.abbr and p.abbr in abbrs and p != abbrs[p.abbr]:
+                        raise StartupError(
+                            "Duplicate permission abbr: {}".format(p.abbr)
+                        )
+                    names[p.name] = p
+                    if p.abbr:
+                        abbrs[p.abbr] = p
+                    self.permissions[p.name] = p
         for hook in pm.hook.prepare_jinja2_environment(
             env=self.jinja_env, datasette=self
         ):
             await await_me_maybe(hook)
         for hook in pm.hook.startup(datasette=self):
             await await_me_maybe(hook)
         self._startup_invoked = True
 
     def sign(self, value, namespace="default"):
         return URLSafeSerializer(self._secret, namespace).dumps(value)
 
     def unsign(self, signed, namespace="default"):
         return URLSafeSerializer(self._secret, namespace).loads(signed)
 
+    def create_token(
+        self,
+        actor_id: str,
+        *,
+        expires_after: Optional[int] = None,
+        restrict_all: Optional[Iterable[str]] = None,
+        restrict_database: Optional[Dict[str, Iterable[str]]] = None,
+        restrict_resource: Optional[Dict[str, Dict[str, Iterable[str]]]] = None,
+    ):
+        token = {"a": actor_id, "t": int(time.time())}
+        if expires_after:
+            token["d"] = expires_after
+
+        def abbreviate_action(action):
+            # rename to abbr if possible
+            permission = self.permissions.get(action)
+            if not permission:
+                return action
+            return permission.abbr or action
+
+        if expires_after:
+            token["d"] = expires_after
+        if restrict_all or restrict_database or restrict_resource:
+            token["_r"] = {}
+            if restrict_all:
+                token["_r"]["a"] = [abbreviate_action(a) for a in restrict_all]
+            if restrict_database:
+                token["_r"]["d"] = {}
+                for database, actions in restrict_database.items():
+                    token["_r"]["d"][database] = [abbreviate_action(a) for a in actions]
+            if restrict_resource:
+                token["_r"]["r"] = {}
+                for database, resources in restrict_resource.items():
+                    for resource, actions in resources.items():
+                        token["_r"]["r"].setdefault(database, {})[resource] = [
+                            abbreviate_action(a) for a in actions
+                        ]
+        return "dstok_{}".format(self.sign(token, namespace="token"))
+
     def get_database(self, name=None, route=None):
         if route is not None:
             matches = [db for db in self.databases.values() if db.route == route]
             if not matches:
                 raise KeyError
             return matches[0]
         if name is None:
@@ -664,52 +725,53 @@
 
     async def _crumb_items(self, request, table=None, database=None):
         crumbs = []
         actor = None
         if request:
             actor = request.actor
         # Top-level link
-        if await self.permission_allowed(
-            actor=actor, action="view-instance", default=True
-        ):
+        if await self.permission_allowed(actor=actor, action="view-instance"):
             crumbs.append({"href": self.urls.instance(), "label": "home"})
         # Database link
         if database:
             if await self.permission_allowed(
                 actor=actor,
                 action="view-database",
                 resource=database,
-                default=True,
             ):
                 crumbs.append(
                     {
                         "href": self.urls.database(database),
                         "label": database,
                     }
                 )
         # Table link
         if table:
             assert database, "table= requires database="
             if await self.permission_allowed(
                 actor=actor,
                 action="view-table",
                 resource=(database, table),
-                default=True,
             ):
                 crumbs.append(
                     {
                         "href": self.urls.table(database, table),
                         "label": table,
                     }
                 )
         return crumbs
 
-    async def permission_allowed(self, actor, action, resource=None, default=False):
+    async def permission_allowed(
+        self, actor, action, resource=None, default=DEFAULT_NOT_SET
+    ):
         """Check permissions using the permissions_allowed plugin hook"""
         result = None
+        # Use default from registered permission, if available
+        if default is DEFAULT_NOT_SET and action in self.permissions:
+            default = self.permissions[action].default
         for check in pm.hook.permission_allowed(
             datasette=self,
             actor=actor,
             action=action,
             resource=resource,
         ):
             check = await await_me_maybe(check)
@@ -1236,15 +1298,17 @@
             r"/-/threads(\.(?P<format>json))?$",
         )
         add_route(
             JsonDataView.as_view(self, "databases.json", self._connected_databases),
             r"/-/databases(\.(?P<format>json))?$",
         )
         add_route(
-            JsonDataView.as_view(self, "actor.json", self._actor, needs_request=True),
+            JsonDataView.as_view(
+                self, "actor.json", self._actor, needs_request=True, permission=None
+            ),
             r"/-/actor(\.(?P<format>json))?$",
         )
         add_route(
             AuthTokenView.as_view(self),
             r"/-/auth-token$",
         )
         add_route(
@@ -1289,14 +1353,18 @@
             r"/(?P<database>[^\/\.]+)/(?P<table>[^/]+?)/(?P<pks>[^/]+?)(\.(?P<format>\w+))?$",
         )
         add_route(
             TableInsertView.as_view(self),
             r"/(?P<database>[^\/\.]+)/(?P<table>[^\/\.]+)/-/insert$",
         )
         add_route(
+            TableUpsertView.as_view(self),
+            r"/(?P<database>[^\/\.]+)/(?P<table>[^\/\.]+)/-/upsert$",
+        )
+        add_route(
             TableDropView.as_view(self),
             r"/(?P<database>[^\/\.]+)/(?P<table>[^\/\.]+)/-/drop$",
         )
         add_route(
             RowDeleteView.as_view(self),
             r"/(?P<database>[^\/\.]+)/(?P<table>[^/]+?)/(?P<pks>[^/]+?)/-/delete$",
         )
```

### Comparing `datasette-1.0a1/datasette/blob_renderer.py` & `datasette-1.0a2/datasette/blob_renderer.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/cli.py` & `datasette-1.0a2/datasette/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import click
 from click import formatting
 from click.types import CompositeParamType
 from click_default_group import DefaultGroup
 import json
 import os
 import pathlib
+from runpy import run_module
 import shutil
 from subprocess import call
 import sys
-from runpy import run_module
 import webbrowser
 from .app import (
     OBSOLETE_SETTINGS,
     Datasette,
     DEFAULT_SETTINGS,
     SETTINGS,
     SQLITE_LIMIT_ATTACHED,
@@ -430,14 +430,18 @@
     help="Output URL that sets a cookie authenticating the root user",
     is_flag=True,
 )
 @click.option(
     "--get",
     help="Run an HTTP GET request against this path, print results and exit",
 )
+@click.option(
+    "--token",
+    help="API token to send with --get requests",
+)
 @click.option("--version-note", help="Additional note to show on /-/versions")
 @click.option("--help-settings", is_flag=True, help="Show available settings")
 @click.option("--pdb", is_flag=True, help="Launch debugger on any errors")
 @click.option(
     "-o",
     "--open",
     "open_browser",
@@ -483,14 +487,15 @@
     static,
     memory,
     config,
     settings,
     secret,
     root,
     get,
+    token,
     version_note,
     help_settings,
     pdb,
     open_browser,
     create,
     crossdb,
     nolock,
@@ -589,17 +594,23 @@
 
     # Run the "startup" plugin hooks
     asyncio.get_event_loop().run_until_complete(ds.invoke_startup())
 
     # Run async soundness checks - but only if we're not under pytest
     asyncio.get_event_loop().run_until_complete(check_databases(ds))
 
+    if token and not get:
+        raise click.ClickException("--token can only be used with --get")
+
     if get:
         client = TestClient(ds)
-        response = client.get(get)
+        headers = {}
+        if token:
+            headers["Authorization"] = "Bearer {}".format(token)
+        response = client.get(get, headers=headers)
         click.echo(response.text)
         exit_code = 0 if response.status == 200 else 1
         sys.exit(exit_code)
         return
 
     # Start the server
     url = None
@@ -624,14 +635,140 @@
     if ssl_keyfile:
         uvicorn_kwargs["ssl_keyfile"] = ssl_keyfile
     if ssl_certfile:
         uvicorn_kwargs["ssl_certfile"] = ssl_certfile
     uvicorn.run(ds.app(), **uvicorn_kwargs)
 
 
+@cli.command()
+@click.argument("id")
+@click.option(
+    "--secret",
+    help="Secret used for signing the API tokens",
+    envvar="DATASETTE_SECRET",
+    required=True,
+)
+@click.option(
+    "-e",
+    "--expires-after",
+    help="Token should expire after this many seconds",
+    type=int,
+)
+@click.option(
+    "alls",
+    "-a",
+    "--all",
+    type=str,
+    metavar="ACTION",
+    multiple=True,
+    help="Restrict token to this action",
+)
+@click.option(
+    "databases",
+    "-d",
+    "--database",
+    type=(str, str),
+    metavar="DB ACTION",
+    multiple=True,
+    help="Restrict token to this action on this database",
+)
+@click.option(
+    "resources",
+    "-r",
+    "--resource",
+    type=(str, str, str),
+    metavar="DB RESOURCE ACTION",
+    multiple=True,
+    help="Restrict token to this action on this database resource (a table, SQL view or named query)",
+)
+@click.option(
+    "--debug",
+    help="Show decoded token",
+    is_flag=True,
+)
+@click.option(
+    "--plugins-dir",
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
+    help="Path to directory containing custom plugins",
+)
+def create_token(
+    id, secret, expires_after, alls, databases, resources, debug, plugins_dir
+):
+    """
+    Create a signed API token for the specified actor ID
+
+    Example:
+
+        datasette create-token root --secret mysecret
+
+    To allow only "view-database-download" for all databases:
+
+    \b
+        datasette create-token root --secret mysecret \\
+            --all view-database-download
+
+    To allow "create-table" against a specific database:
+
+    \b
+        datasette create-token root --secret mysecret \\
+            --database mydb create-table
+
+    To allow "insert-row" against a specific table:
+
+    \b
+        datasette create-token root --secret myscret \\
+            --resource mydb mytable insert-row
+
+    Restricted actions can be specified multiple times using
+    multiple --all, --database, and --resource options.
+
+    Add --debug to see a decoded version of the token.
+    """
+    ds = Datasette(secret=secret, plugins_dir=plugins_dir)
+
+    # Run ds.invoke_startup() in an event loop
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(ds.invoke_startup())
+
+    # Warn about any unknown actions
+    actions = []
+    actions.extend(alls)
+    actions.extend([p[1] for p in databases])
+    actions.extend([p[2] for p in resources])
+    for action in actions:
+        if not ds.permissions.get(action):
+            click.secho(
+                f"  Unknown permission: {action} ",
+                fg="red",
+                err=True,
+            )
+
+    restrict_database = {}
+    for database, action in databases:
+        restrict_database.setdefault(database, []).append(action)
+    restrict_resource = {}
+    for database, resource, action in resources:
+        restrict_resource.setdefault(database, {}).setdefault(resource, []).append(
+            action
+        )
+
+    token = ds.create_token(
+        id,
+        expires_after=expires_after,
+        restrict_all=alls,
+        restrict_database=restrict_database,
+        restrict_resource=restrict_resource,
+    )
+    click.echo(token)
+    if debug:
+        encoded = token[len("dstok_") :]
+        click.echo("\nDecoded:\n")
+        click.echo(json.dumps(ds.unsign(encoded, namespace="token"), indent=2))
+
+
 pm.hook.register_commands(cli=cli)
 
 
 async def check_databases(ds):
     # Run check_connection against every connected database
     # to confirm they are all usable
     for database in list(ds.databases.values()):
```

### Comparing `datasette-1.0a1/datasette/database.py` & `datasette-1.0a2/datasette/database.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/default_magic_parameters.py` & `datasette-1.0a2/datasette/default_magic_parameters.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/default_menu_links.py` & `datasette-1.0a2/datasette/default_menu_links.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/facets.py` & `datasette-1.0a2/datasette/facets.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/filters.py` & `datasette-1.0a2/datasette/filters.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/handle_exception.py` & `datasette-1.0a2/datasette/handle_exception.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/hookspecs.py` & `datasette-1.0a2/datasette/hookspecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 
 @hookspec
 def register_facet_classes():
     """Register Facet subclasses"""
 
 
 @hookspec
+def register_permissions(datasette):
+    """Register permissions: returns a list of datasette.permission.Permission named tuples"""
+
+
+@hookspec
 def register_routes(datasette):
     """Register URL routes: return a list of (regex, view_function) pairs"""
 
 
 @hookspec
 def register_commands(cli):
     """Register additional CLI commands, e.g. 'datasette mycommand ...'"""
```

### Comparing `datasette-1.0a1/datasette/inspect.py` & `datasette-1.0a2/datasette/inspect.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/plugins.py` & `datasette-1.0a2/datasette/plugins.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/publish/cloudrun.py` & `datasette-1.0a2/datasette/publish/cloudrun.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/publish/common.py` & `datasette-1.0a2/datasette/publish/common.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/publish/heroku.py` & `datasette-1.0a2/datasette/publish/heroku.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/renderer.py` & `datasette-1.0a2/datasette/renderer.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/static/app.css` & `datasette-1.0a2/datasette/static/app.css`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/static/cm-editor-6.0.1.bundle.js` & `datasette-1.0a2/datasette/static/cm-editor-6.0.1.bundle.js`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/static/cm-editor-6.0.1.js` & `datasette-1.0a2/datasette/static/cm-editor-6.0.1.js`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/static/json-format-highlight-1.0.1.js` & `datasette-1.0a2/datasette/static/json-format-highlight-1.0.1.js`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/static/sql-formatter-2.3.3.min.js` & `datasette-1.0a2/datasette/static/sql-formatter-2.3.3.min.js`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/static/table.js` & `datasette-1.0a2/datasette/static/table.js`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_close_open_menus.html` & `datasette-1.0a2/datasette/templates/_close_open_menus.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_codemirror.html` & `datasette-1.0a2/datasette/templates/_codemirror.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_codemirror_foot.html` & `datasette-1.0a2/datasette/templates/_codemirror_foot.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_description_source_license.html` & `datasette-1.0a2/datasette/templates/_description_source_license.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_facet_results.html` & `datasette-1.0a2/datasette/templates/_facet_results.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_footer.html` & `datasette-1.0a2/datasette/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/_table.html` & `datasette-1.0a2/datasette/templates/_table.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/allow_debug.html` & `datasette-1.0a2/datasette/templates/allow_debug.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/api_explorer.html` & `datasette-1.0a2/datasette/templates/api_explorer.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/base.html` & `datasette-1.0a2/datasette/templates/base.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/database.html` & `datasette-1.0a2/datasette/templates/database.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/index.html` & `datasette-1.0a2/datasette/templates/index.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/messages_debug.html` & `datasette-1.0a2/datasette/templates/messages_debug.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/patterns.html` & `datasette-1.0a2/datasette/templates/patterns.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/permissions_debug.html` & `datasette-1.0a2/datasette/templates/permissions_debug.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/query.html` & `datasette-1.0a2/datasette/templates/query.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/row.html` & `datasette-1.0a2/datasette/templates/row.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/templates/table.html` & `datasette-1.0a2/datasette/templates/table.html`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/tracer.py` & `datasette-1.0a2/datasette/tracer.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/url_builder.py` & `datasette-1.0a2/datasette/url_builder.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/__init__.py` & `datasette-1.0a2/datasette/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/asgi.py` & `datasette-1.0a2/datasette/utils/asgi.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/baseconv.py` & `datasette-1.0a2/datasette/utils/baseconv.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/internal_db.py` & `datasette-1.0a2/datasette/utils/internal_db.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/shutil_backport.py` & `datasette-1.0a2/datasette/utils/shutil_backport.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/sqlite.py` & `datasette-1.0a2/datasette/utils/sqlite.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/utils/testing.py` & `datasette-1.0a2/datasette/utils/testing.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/views/base.py` & `datasette-1.0a2/datasette/views/base.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/views/database.py` & `datasette-1.0a2/datasette/views/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 if extra_links:
                     links.extend(extra_links)
             return links
 
         attached_databases = [d.name for d in await db.attached_databases()]
 
         allow_execute_sql = await self.ds.permission_allowed(
-            request.actor, "execute-sql", database, default=True
+            request.actor, "execute-sql", database
         )
         return (
             {
                 "database": database,
                 "private": private,
                 "path": self.ds.urls.database(database),
                 "size": db.size,
@@ -371,15 +371,15 @@
                 columns = [r[0] for r in results.description]
             except sqlite3.DatabaseError as e:
                 query_error = e
                 results = None
                 columns = []
 
         allow_execute_sql = await self.ds.permission_allowed(
-            request.actor, "execute-sql", database, default=True
+            request.actor, "execute-sql", database
         )
 
         async def extra_template():
             display_rows = []
             truncate_cells = self.ds.setting("truncate_cells_html")
             for row in results.rows if results else []:
                 display_row = []
@@ -556,15 +556,15 @@
         else:
             return super().__getitem__(key)
 
 
 class TableCreateView(BaseView):
     name = "table-create"
 
-    _valid_keys = {"table", "rows", "row", "columns", "pk"}
+    _valid_keys = {"table", "rows", "row", "columns", "pk", "pks", "ignore", "replace"}
     _supported_column_types = {
         "text",
         "integer",
         "float",
         "blob",
     }
     # Any string that does not contain a newline or start with sqlite_
@@ -592,155 +592,62 @@
         if not isinstance(data, dict):
             return _error(["JSON must be an object"])
 
         invalid_keys = set(data.keys()) - self._valid_keys
         if invalid_keys:
             return _error(["Invalid keys: {}".format(", ".join(invalid_keys))])
 
-        table_name = data.get("table")
-        if not table_name:
-            return _error(["Table is required"])
-
-        if not self._table_name_re.match(table_name):
-            return _error(["Invalid table name"])
-
-        columns = data.get("columns")
-        rows = data.get("rows")
-        row = data.get("row")
-        if not columns and not rows and not row:
-            return _error(["columns, rows or row is required"])
-
-        if rows and row:
-            return _error(["Cannot specify both rows and row"])
-
-        if columns:
-            if rows or row:
-                return _error(["Cannot specify columns with rows or row"])
-            if not isinstance(columns, list):
-                return _error(["columns must be a list"])
-            for column in columns:
-                if not isinstance(column, dict):
-                    return _error(["columns must be a list of objects"])
-                if not column.get("name") or not isinstance(column.get("name"), str):
-                    return _error(["Column name is required"])
-                if not column.get("type"):
-                    column["type"] = "text"
-                if column["type"] not in self._supported_column_types:
-                    return _error(
-                        ["Unsupported column type: {}".format(column["type"])]
-                    )
-            # No duplicate column names
-            dupes = {c["name"] for c in columns if columns.count(c) > 1}
-            if dupes:
-                return _error(["Duplicate column name: {}".format(", ".join(dupes))])
-
-        if row:
-            rows = [row]
-
-        if rows:
-            if not isinstance(rows, list):
-                return _error(["rows must be a list"])
-            for row in rows:
-                if not isinstance(row, dict):
-                    return _error(["rows must be a list of objects"])
-
-        pk = data.get("pk")
-        if pk:
-            if not isinstance(pk, str):
-                return _error(["pk must be a string"])
-
-        def create_table(conn):
-            table = sqlite_utils.Database(conn)[table_name]
-            if rows:
-                table.insert_all(rows, pk=pk)
-            else:
-                table.create(
-                    {c["name"]: c["type"] for c in columns},
-                    pk=pk,
-                )
-            return table.schema
-
-        try:
-            schema = await db.execute_write_fn(create_table)
-        except Exception as e:
-            return _error([str(e)])
-        table_url = self.ds.absolute_url(
-            request, self.ds.urls.table(db.name, table_name)
-        )
-        table_api_url = self.ds.absolute_url(
-            request, self.ds.urls.table(db.name, table_name, format="json")
-        )
-        details = {
-            "ok": True,
-            "database": db.name,
-            "table": table_name,
-            "table_url": table_url,
-            "table_api_url": table_api_url,
-            "schema": schema,
-        }
-        if rows:
-            details["row_count"] = len(rows)
-        return Response.json(details, status=201)
-
-
-class TableCreateView(BaseView):
-    name = "table-create"
-
-    _valid_keys = {"table", "rows", "row", "columns", "pk", "pks"}
-    _supported_column_types = {
-        "text",
-        "integer",
-        "float",
-        "blob",
-    }
-    # Any string that does not contain a newline or start with sqlite_
-    _table_name_re = re.compile(r"^(?!sqlite_)[^\n]+$")
-
-    def __init__(self, datasette):
-        self.ds = datasette
-
-    async def post(self, request):
-        db = await self.ds.resolve_database(request)
-        database_name = db.name
-
-        # Must have create-table permission
-        if not await self.ds.permission_allowed(
-            request.actor, "create-table", resource=database_name
-        ):
-            return _error(["Permission denied"], 403)
-
-        body = await request.post_body()
-        try:
-            data = json.loads(body)
-        except json.JSONDecodeError as e:
-            return _error(["Invalid JSON: {}".format(e)])
-
-        if not isinstance(data, dict):
-            return _error(["JSON must be an object"])
-
-        invalid_keys = set(data.keys()) - self._valid_keys
-        if invalid_keys:
-            return _error(["Invalid keys: {}".format(", ".join(invalid_keys))])
+        # ignore and replace are mutually exclusive
+        if data.get("ignore") and data.get("replace"):
+            return _error(["ignore and replace are mutually exclusive"])
+
+        # ignore and replace only allowed with row or rows
+        if "ignore" in data or "replace" in data:
+            if not data.get("row") and not data.get("rows"):
+                return _error(["ignore and replace require row or rows"])
+
+        # ignore and replace require pk or pks
+        if "ignore" in data or "replace" in data:
+            if not data.get("pk") and not data.get("pks"):
+                return _error(["ignore and replace require pk or pks"])
+
+        ignore = data.get("ignore")
+        replace = data.get("replace")
+
+        if replace:
+            # Must have update-row permission
+            if not await self.ds.permission_allowed(
+                request.actor, "update-row", resource=database_name
+            ):
+                return _error(["Permission denied - need update-row"], 403)
 
         table_name = data.get("table")
         if not table_name:
             return _error(["Table is required"])
 
         if not self._table_name_re.match(table_name):
             return _error(["Invalid table name"])
 
+        table_exists = await db.table_exists(data["table"])
         columns = data.get("columns")
         rows = data.get("rows")
         row = data.get("row")
         if not columns and not rows and not row:
             return _error(["columns, rows or row is required"])
 
         if rows and row:
             return _error(["Cannot specify both rows and row"])
 
+        if rows or row:
+            # Must have insert-row permission
+            if not await self.ds.permission_allowed(
+                request.actor, "insert-row", resource=database_name
+            ):
+                return _error(["Permission denied - need insert-row"], 403)
+
         if columns:
             if rows or row:
                 return _error(["Cannot specify columns with rows or row"])
             if not isinstance(columns, list):
                 return _error(["columns must be a list"])
             for column in columns:
                 if not isinstance(column, dict):
@@ -779,18 +686,35 @@
         if pks:
             if not isinstance(pks, list):
                 return _error(["pks must be a list"])
             for pk in pks:
                 if not isinstance(pk, str):
                     return _error(["pks must be a list of strings"])
 
+        # If table exists already, read pks from that instead
+        if table_exists:
+            actual_pks = await db.primary_keys(table_name)
+            # if pk passed and table already exists check it does not change
+            bad_pks = False
+            if len(actual_pks) == 1 and data.get("pk") and data["pk"] != actual_pks[0]:
+                bad_pks = True
+            elif (
+                len(actual_pks) > 1
+                and data.get("pks")
+                and set(data["pks"]) != set(actual_pks)
+            ):
+                bad_pks = True
+            if bad_pks:
+                return _error(["pk cannot be changed for existing table"])
+            pks = actual_pks
+
         def create_table(conn):
             table = sqlite_utils.Database(conn)[table_name]
             if rows:
-                table.insert_all(rows, pk=pks or pk)
+                table.insert_all(rows, pk=pks or pk, ignore=ignore, replace=replace)
             else:
                 table.create(
                     {c["name"]: c["type"] for c in columns},
                     pk=pks or pk,
                 )
             return table.schema
```

### Comparing `datasette-1.0a1/datasette/views/index.py` & `datasette-1.0a2/datasette/views/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,11 +138,11 @@
                 ["index.html"],
                 request=request,
                 context={
                     "databases": databases,
                     "metadata": self.ds.metadata(),
                     "datasette_version": __version__,
                     "private": not await self.ds.permission_allowed(
-                        None, "view-instance", default=True
+                        None, "view-instance"
                     ),
                 },
             )
```

### Comparing `datasette-1.0a1/datasette/views/row.py` & `datasette-1.0a2/datasette/views/row.py`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/datasette/views/special.py` & `datasette-1.0a2/datasette/views/special.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 import json
-from datasette.permissions import PERMISSIONS
 from datasette.utils.asgi import Response, Forbidden
-from datasette.utils import actor_matches_allow, add_cors_headers
-from datasette.permissions import PERMISSIONS
+from datasette.utils import (
+    actor_matches_allow,
+    add_cors_headers,
+    tilde_encode,
+    tilde_decode,
+)
 from .base import BaseView
 import secrets
-import time
 import urllib
 
 
 class JsonDataView(BaseView):
     name = "json_data"
 
-    def __init__(self, datasette, filename, data_callback, needs_request=False):
+    def __init__(
+        self,
+        datasette,
+        filename,
+        data_callback,
+        needs_request=False,
+        permission="view-instance",
+    ):
         self.ds = datasette
         self.filename = filename
         self.data_callback = data_callback
         self.needs_request = needs_request
+        self.permission = permission
 
     async def get(self, request):
         as_format = request.url_vars["format"]
-        await self.ds.ensure_permissions(request.actor, ["view-instance"])
+        if self.permission:
+            await self.ds.ensure_permissions(request.actor, [self.permission])
         if self.needs_request:
             data = self.data_callback(request)
         else:
             data = self.data_callback()
         if as_format:
             headers = {}
             if self.ds.cors:
@@ -104,15 +115,15 @@
             raise Forbidden("Permission denied")
         return await self.render(
             ["permissions_debug.html"],
             request,
             # list() avoids error if check is performed during template render:
             {
                 "permission_checks": list(reversed(self.ds._permission_checks)),
-                "permissions": PERMISSIONS,
+                "permissions": list(self.ds.permissions.values()),
             },
         )
 
     async def post(self, request):
         await self.ds.ensure_permissions(request.actor, ["view-instance"])
         if not await self.ds.permission_allowed(request.actor, "permissions-debug"):
             raise Forbidden("Permission denied")
@@ -215,65 +226,123 @@
                 "You must be logged in as an actor with an ID to create a token"
             )
         if request.actor.get("token"):
             raise Forbidden(
                 "Token authentication cannot be used to create additional tokens"
             )
 
+    async def shared(self, request):
+        self.check_permission(request)
+        # Build list of databases and tables the user has permission to view
+        database_with_tables = []
+        for database in self.ds.databases.values():
+            if database.name in ("_internal", "_memory"):
+                continue
+            if not await self.ds.permission_allowed(
+                request.actor, "view-database", database.name
+            ):
+                continue
+            hidden_tables = await database.hidden_table_names()
+            tables = []
+            for table in await database.table_names():
+                if table in hidden_tables:
+                    continue
+                if not await self.ds.permission_allowed(
+                    request.actor,
+                    "view-table",
+                    resource=(database.name, table),
+                ):
+                    continue
+                tables.append({"name": table, "encoded": tilde_encode(table)})
+            database_with_tables.append(
+                {
+                    "name": database.name,
+                    "encoded": tilde_encode(database.name),
+                    "tables": tables,
+                }
+            )
+        return {
+            "actor": request.actor,
+            "all_permissions": self.ds.permissions.keys(),
+            "database_permissions": [
+                key
+                for key, value in self.ds.permissions.items()
+                if value.takes_database
+            ],
+            "resource_permissions": [
+                key
+                for key, value in self.ds.permissions.items()
+                if value.takes_resource
+            ],
+            "database_with_tables": database_with_tables,
+        }
+
     async def get(self, request):
         self.check_permission(request)
         return await self.render(
-            ["create_token.html"],
-            request,
-            {"actor": request.actor},
+            ["create_token.html"], request, await self.shared(request)
         )
 
     async def post(self, request):
         self.check_permission(request)
         post = await request.post_vars()
         errors = []
-        duration = None
+        expires_after = None
         if post.get("expire_type"):
             duration_string = post.get("expire_duration")
             if (
                 not duration_string
                 or not duration_string.isdigit()
                 or not int(duration_string) > 0
             ):
                 errors.append("Invalid expire duration")
             else:
                 unit = post["expire_type"]
                 if unit == "minutes":
-                    duration = int(duration_string) * 60
+                    expires_after = int(duration_string) * 60
                 elif unit == "hours":
-                    duration = int(duration_string) * 60 * 60
+                    expires_after = int(duration_string) * 60 * 60
                 elif unit == "days":
-                    duration = int(duration_string) * 60 * 60 * 24
+                    expires_after = int(duration_string) * 60 * 60 * 24
                 else:
                     errors.append("Invalid expire duration unit")
-        token_bits = None
-        token = None
-        if not errors:
-            token_bits = {
-                "a": request.actor["id"],
-                "t": int(time.time()),
-            }
-            if duration:
-                token_bits["d"] = duration
-            token = "dstok_{}".format(self.ds.sign(token_bits, "token"))
-        return await self.render(
-            ["create_token.html"],
-            request,
-            {
-                "actor": request.actor,
-                "errors": errors,
-                "token": token,
-                "token_bits": token_bits,
-            },
+
+        # Are there any restrictions?
+        restrict_all = []
+        restrict_database = {}
+        restrict_resource = {}
+
+        for key in post:
+            if key.startswith("all:") and key.count(":") == 1:
+                restrict_all.append(key.split(":")[1])
+            elif key.startswith("database:") and key.count(":") == 2:
+                bits = key.split(":")
+                database = tilde_decode(bits[1])
+                action = bits[2]
+                restrict_database.setdefault(database, []).append(action)
+            elif key.startswith("resource:") and key.count(":") == 3:
+                bits = key.split(":")
+                database = tilde_decode(bits[1])
+                resource = tilde_decode(bits[2])
+                action = bits[3]
+                restrict_resource.setdefault(database, {}).setdefault(
+                    resource, []
+                ).append(action)
+
+        token = self.ds.create_token(
+            request.actor["id"],
+            expires_after=expires_after,
+            restrict_all=restrict_all,
+            restrict_database=restrict_database,
+            restrict_resource=restrict_resource,
         )
+        token_bits = self.ds.unsign(token[len("dstok_") :], namespace="token")
+        context = await self.shared(request)
+        context.update({"errors": errors, "token": token, "token_bits": token_bits})
+        return await self.render(["create_token.html"], request, context)
 
 
 class ApiExplorerView(BaseView):
     name = "api_explorer"
     has_json_alternate = False
 
     async def example_links(self, request):
@@ -312,29 +381,45 @@
                 if not db.is_mutable:
                     continue
 
                 if await self.ds.permission_allowed(
                     request.actor, "insert-row", (name, table)
                 ):
                     pks = await db.primary_keys(table)
-                    table_links.append(
-                        {
-                            "path": self.ds.urls.table(name, table) + "/-/insert",
-                            "method": "POST",
-                            "label": "Insert rows into {}".format(table),
-                            "json": {
-                                "rows": [
-                                    {
-                                        column: None
-                                        for column in await db.table_columns(table)
-                                        if column not in pks
-                                    }
-                                ]
+                    table_links.extend(
+                        [
+                            {
+                                "path": self.ds.urls.table(name, table) + "/-/insert",
+                                "method": "POST",
+                                "label": "Insert rows into {}".format(table),
+                                "json": {
+                                    "rows": [
+                                        {
+                                            column: None
+                                            for column in await db.table_columns(table)
+                                            if column not in pks
+                                        }
+                                    ]
+                                },
+                            },
+                            {
+                                "path": self.ds.urls.table(name, table) + "/-/upsert",
+                                "method": "POST",
+                                "label": "Upsert rows into {}".format(table),
+                                "json": {
+                                    "rows": [
+                                        {
+                                            column: None
+                                            for column in await db.table_columns(table)
+                                            if column not in pks
+                                        }
+                                    ]
+                                },
                             },
-                        }
+                        ]
                     )
                 if await self.ds.permission_allowed(
                     request.actor, "drop-table", (name, table)
                 ):
                     table_links.append(
                         {
                             "path": self.ds.urls.table(name, table) + "/-/drop",
```

### Comparing `datasette-1.0a1/datasette/views/table.py` & `datasette-1.0a2/datasette/views/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -383,25 +383,27 @@
         sort_desc = request.args.get("_sort_desc")
 
         if not sort and not sort_desc:
             sort = table_metadata.get("sort")
             sort_desc = table_metadata.get("sort_desc")
 
         if sort and sort_desc:
-            raise DatasetteError("Cannot use _sort and _sort_desc at the same time")
+            raise DatasetteError(
+                "Cannot use _sort and _sort_desc at the same time", status=400
+            )
 
         if sort:
             if sort not in sortable_columns:
-                raise DatasetteError(f"Cannot sort table by {sort}")
+                raise DatasetteError(f"Cannot sort table by {sort}", status=400)
 
             order_by = escape_sqlite(sort)
 
         if sort_desc:
             if sort_desc not in sortable_columns:
-                raise DatasetteError(f"Cannot sort table by {sort_desc}")
+                raise DatasetteError(f"Cannot sort table by {sort_desc}", status=400)
 
             order_by = f"{escape_sqlite(sort_desc)} desc"
 
         from_sql = "from {table_name} {where}".format(
             table_name=escape_sqlite(table_name),
             where=("where {} ".format(" and ".join(where_clauses)))
             if where_clauses
@@ -860,15 +862,15 @@
                 "query": {"sql": sql, "params": params},
                 "facet_results": facet_results,
                 "suggested_facets": suggested_facets,
                 "next": next_value and str(next_value) or None,
                 "next_url": next_url,
                 "private": private,
                 "allow_execute_sql": await self.ds.permission_allowed(
-                    request.actor, "execute-sql", database_name, default=True
+                    request.actor, "execute-sql", database_name
                 ),
             },
             extra_template,
             (
                 f"table-{to_css_class(database_name)}-{to_css_class(table_name)}.html",
                 "table.html",
             ),
@@ -1070,17 +1072,26 @@
 
 class TableInsertView(BaseView):
     name = "table-insert"
 
     def __init__(self, datasette):
         self.ds = datasette
 
-    async def _validate_data(self, request, db, table_name):
+    async def _validate_data(self, request, db, table_name, pks, upsert):
         errors = []
 
+        pks_list = []
+        if isinstance(pks, str):
+            pks_list = [pks]
+        else:
+            pks_list = list(pks)
+
+        if not pks_list:
+            pks_list = ["rowid"]
+
         def _errors(errors):
             return None, errors, {}
 
         if request.headers.get("content-type") != "application/json":
             # TODO: handle form-encoded data
             return _errors(["Invalid content-type, must be application/json"])
         body = await request.post_body()
@@ -1130,78 +1141,150 @@
                 ['Invalid parameter: "{}"'.format('", "'.join(sorted(invalid_extras)))]
             )
         if extras.get("ignore") and extras.get("replace"):
             return _errors(['Cannot use "ignore" and "replace" at the same time'])
 
         # Validate columns of each row
         columns = set(await db.table_columns(table_name))
+        columns.update(pks_list)
+
         for i, row in enumerate(rows):
+            if upsert:
+                # It MUST have the primary key
+                missing_pks = [pk for pk in pks_list if pk not in row]
+                if missing_pks:
+                    errors.append(
+                        'Row {} is missing primary key column(s): "{}"'.format(
+                            i, '", "'.join(missing_pks)
+                        )
+                    )
             invalid_columns = set(row.keys()) - columns
             if invalid_columns:
                 errors.append(
                     "Row {} has invalid columns: {}".format(
                         i, ", ".join(sorted(invalid_columns))
                     )
                 )
         if errors:
             return _errors(errors)
         return rows, errors, extras
 
-    async def post(self, request):
+    async def post(self, request, upsert=False):
         try:
             resolved = await self.ds.resolve_table(request)
         except NotFound as e:
             return _error([e.args[0]], 404)
         db = resolved.db
         database_name = db.name
         table_name = resolved.table
 
         # Table must exist (may handle table creation in the future)
         db = self.ds.get_database(database_name)
         if not await db.table_exists(table_name):
             return _error(["Table not found: {}".format(table_name)], 404)
-        # Must have insert-row permission
-        if not await self.ds.permission_allowed(
-            request.actor, "insert-row", resource=(database_name, table_name)
-        ):
-            return _error(["Permission denied"], 403)
-        rows, errors, extras = await self._validate_data(request, db, table_name)
+
+        if upsert:
+            # Must have insert-row AND upsert-row permissions
+            if not (
+                await self.ds.permission_allowed(
+                    request.actor, "insert-row", database_name, table_name
+                )
+                and await self.ds.permission_allowed(
+                    request.actor, "update-row", database_name, table_name
+                )
+            ):
+                return _error(
+                    ["Permission denied: need both insert-row and update-row"], 403
+                )
+        else:
+            # Must have insert-row permission
+            if not await self.ds.permission_allowed(
+                request.actor, "insert-row", resource=(database_name, table_name)
+            ):
+                return _error(["Permission denied"], 403)
+
+        if not db.is_mutable:
+            return _error(["Database is immutable"], 403)
+
+        pks = await db.primary_keys(table_name)
+
+        rows, errors, extras = await self._validate_data(
+            request, db, table_name, pks, upsert
+        )
         if errors:
             return _error(errors, 400)
 
+        # No that we've passed pks to _validate_data it's safe to
+        # fix the rowids case:
+        if not pks:
+            pks = ["rowid"]
+
         ignore = extras.get("ignore")
         replace = extras.get("replace")
 
+        if upsert and (ignore or replace):
+            return _error(["Upsert does not support ignore or replace"], 400)
+
         should_return = bool(extras.get("return", False))
-        # Insert rows
-        def insert_rows(conn):
+        row_pk_values_for_later = []
+        if should_return and upsert:
+            row_pk_values_for_later = [tuple(row[pk] for pk in pks) for row in rows]
+
+        def insert_or_upsert_rows(conn):
             table = sqlite_utils.Database(conn)[table_name]
-            if should_return:
+            kwargs = {}
+            if upsert:
+                kwargs["pk"] = pks[0] if len(pks) == 1 else pks
+            else:
+                kwargs = {"ignore": ignore, "replace": replace}
+            if should_return and not upsert:
                 rowids = []
+                method = table.upsert if upsert else table.insert
                 for row in rows:
-                    rowids.append(
-                        table.insert(row, ignore=ignore, replace=replace).last_rowid
-                    )
+                    rowids.append(method(row, **kwargs).last_rowid)
                 return list(
                     table.rows_where(
                         "rowid in ({})".format(",".join("?" for _ in rowids)),
                         rowids,
                     )
                 )
             else:
-                table.insert_all(rows, ignore=ignore, replace=replace)
+                method_all = table.upsert_all if upsert else table.insert_all
+                method_all(rows, **kwargs)
 
         try:
-            rows = await db.execute_write_fn(insert_rows)
+            rows = await db.execute_write_fn(insert_or_upsert_rows)
         except Exception as e:
             return _error([str(e)])
         result = {"ok": True}
         if should_return:
-            result["rows"] = rows
-        return Response.json(result, status=201)
+            if upsert:
+                # Fetch based on initial input IDs
+                where_clause = " OR ".join(
+                    ["({})".format(" AND ".join("{} = ?".format(pk) for pk in pks))]
+                    * len(row_pk_values_for_later)
+                )
+                args = list(itertools.chain.from_iterable(row_pk_values_for_later))
+                fetched_rows = await db.execute(
+                    "select {}* from [{}] where {}".format(
+                        "rowid, " if pks == ["rowid"] else "", table_name, where_clause
+                    ),
+                    args,
+                )
+                result["rows"] = [dict(r) for r in fetched_rows.rows]
+            else:
+                result["rows"] = rows
+        return Response.json(result, status=200 if upsert else 201)
+
+
+class TableUpsertView(TableInsertView):
+    name = "table-upsert"
+
+    async def post(self, request):
+        return await super().post(request, upsert=True)
 
 
 class TableDropView(BaseView):
     name = "table-drop"
 
     def __init__(self, datasette):
         self.ds = datasette
```

### Comparing `datasette-1.0a1/datasette.egg-info/PKG-INFO` & `datasette-1.0a2/datasette.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette
-Version: 1.0a1
+Version: 1.0a2
 Summary: An open source multi-tool for exploring and publishing data
 Home-page: https://datasette.io/
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.datasette.io/en/stable/
 Project-URL: Changelog, https://docs.datasette.io/en/stable/changelog.html
 Project-URL: Live demo, https://latest.datasette.io/
```

### Comparing `datasette-1.0a1/datasette.egg-info/SOURCES.txt` & `datasette-1.0a2/datasette.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-1.0a1/setup.py` & `datasette-1.0a2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,26 +62,26 @@
     entry_points="""
         [console_scripts]
         datasette=datasette.cli:cli
     """,
     setup_requires=["pytest-runner"],
     extras_require={
         "docs": [
-            "furo==2022.9.29",
+            "furo==2022.12.7",
             "sphinx-autobuild",
             "codespell",
             "blacken-docs",
             "sphinx-copybutton",
         ],
         "test": [
             "pytest>=5.2.2",
             "pytest-xdist>=2.2.1",
             "pytest-asyncio>=0.17",
             "beautifulsoup4>=4.8.1",
-            "black==22.10.0",
+            "black==22.12.0",
             "blacken-docs==1.12.1",
             "pytest-timeout>=1.4.2",
             "trustme>=0.7",
             "cogapp>=3.3.0",
         ],
         "rich": ["rich"],
     },
```

