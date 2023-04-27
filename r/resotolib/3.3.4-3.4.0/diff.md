# Comparing `tmp/resotolib-3.3.4.tar.gz` & `tmp/resotolib-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.3.4.tar", last modified: Wed Apr 26 16:51:02 2023, max compression
+gzip compressed data, was "resotolib-3.4.0.tar", last modified: Thu Apr 27 11:25:11 2023, max compression
```

## Comparing `resotolib-3.3.4.tar` & `resotolib-3.4.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.742747 resotolib-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 16:49:29.000000 resotolib-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-26 16:51:02.742747 resotolib-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-26 16:49:29.000000 resotolib-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 16:49:29.000000 resotolib-3.3.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-26 16:49:29.000000 resotolib-3.3.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.710747 resotolib-3.3.4/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.714747 resotolib-3.3.4/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/asynchronous/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.714747 resotolib-3.3.4/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.722747 resotolib-3.3.4/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.722747 resotolib-3.3.4/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    25794 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.722747 resotolib-3.3.4/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/log/logstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.722747 resotolib-3.3.4/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.730747 resotolib-3.3.4/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-04-26 16:49:29.000000 resotolib-3.3.4/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.714747 resotolib-3.3.4/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-26 16:51:02.000000 resotolib-3.3.4/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-26 16:51:02.000000 resotolib-3.3.4/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:02.000000 resotolib-3.3.4/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:02.000000 resotolib-3.3.4/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-26 16:51:02.000000 resotolib-3.3.4/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 16:51:02.000000 resotolib-3.3.4/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:51:02.742747 resotolib-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 16:49:29.000000 resotolib-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.738747 resotolib-3.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.738747 resotolib-3.3.4/test/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/asynchronous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.738747 resotolib-3.3.4/test/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/asynchronous/web/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:02.742747 resotolib-3.3.4/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/core/custom_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/core/model_check_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/core/model_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/core/progress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/core/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/durations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/json_bender_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/parse_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-26 16:49:29.000000 resotolib-3.3.4/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 11:22:59.000000 resotolib-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-27 11:25:11.410409 resotolib-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-27 11:22:59.000000 resotolib-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 11:22:59.000000 resotolib-3.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 11:22:59.000000 resotolib-3.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.370408 resotolib-3.4.0/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.374408 resotolib-3.4.0/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.378408 resotolib-3.4.0/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.382408 resotolib-3.4.0/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.386408 resotolib-3.4.0/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    25794 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.386408 resotolib-3.4.0/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/log/logstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.390408 resotolib-3.4.0/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.394408 resotolib-3.4.0/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-04-27 11:22:59.000000 resotolib-3.4.0/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.370408 resotolib-3.4.0/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 11:25:11.000000 resotolib-3.4.0/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:25:11.410409 resotolib-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-27 11:22:59.000000 resotolib-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/asynchronous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/asynchronous/web/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:25:11.406408 resotolib-3.4.0/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/custom_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/model_check_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/model_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/progress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/core/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/durations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/json_bender_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/parse_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-27 11:22:59.000000 resotolib-3.4.0/test/test_x509.py
```

### Comparing `resotolib-3.3.4/PKG-INFO` & `resotolib-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.3.4
+Version: 3.4.0
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.3.4/README.md` & `resotolib-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/args.py` & `resotolib-3.4.0/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/asynchronous/periodic.py` & `resotolib-3.4.0/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/asynchronous/web/auth.py` & `resotolib-3.4.0/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/asynchronous/web/runner.py` & `resotolib-3.4.0/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.4.0/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/baseplugin.py` & `resotolib-3.4.0/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/baseresources.py` & `resotolib-3.4.0/resotolib/baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/config.py` & `resotolib-3.4.0/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/__init__.py` & `resotolib-3.4.0/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/actions.py` & `resotolib-3.4.0/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/ca.py` & `resotolib-3.4.0/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/config.py` & `resotolib-3.4.0/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/custom_command.py` & `resotolib-3.4.0/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/events.py` & `resotolib-3.4.0/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/model_check.py` & `resotolib-3.4.0/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/model_export.py` & `resotolib-3.4.0/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/progress.py` & `resotolib-3.4.0/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/search.py` & `resotolib-3.4.0/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/core/tasks.py` & `resotolib-3.4.0/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/durations.py` & `resotolib-3.4.0/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/event.py` & `resotolib-3.4.0/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/graph/__init__.py` & `resotolib-3.4.0/resotolib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/graph/graph_extensions.py` & `resotolib-3.4.0/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/json.py` & `resotolib-3.4.0/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/json_bender.py` & `resotolib-3.4.0/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/jwt.py` & `resotolib-3.4.0/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/lock.py` & `resotolib-3.4.0/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/log/logstream.py` & `resotolib-3.4.0/resotolib/log/logstream.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/logger.py` & `resotolib-3.4.0/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/parse_util.py` & `resotolib-3.4.0/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/proc.py` & `resotolib-3.4.0/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/tree.py` & `resotolib-3.4.0/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/utils.py` & `resotolib-3.4.0/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/__init__.py` & `resotolib-3.4.0/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/metrics.py` & `resotolib-3.4.0/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.4.0/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.4.0/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.4.0/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/favicon-16x16.png` & `resotolib-3.4.0/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/favicon-32x32.png` & `resotolib-3.4.0/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/index.html` & `resotolib-3.4.0/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/mstile-150x150.png` & `resotolib-3.4.0/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/web/static/picnic.min.css` & `resotolib-3.4.0/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib/x509.py` & `resotolib-3.4.0/resotolib/x509.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/resotolib.egg-info/PKG-INFO` & `resotolib-3.4.0/resotolib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.3.4
+Version: 3.4.0
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.3.4/resotolib.egg-info/SOURCES.txt` & `resotolib-3.4.0/resotolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/setup.py` & `resotolib-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/asynchronous/web/test_auth.py` & `resotolib-3.4.0/test/asynchronous/web/test_auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/core/custom_command_test.py` & `resotolib-3.4.0/test/core/custom_command_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/core/model_check_test.py` & `resotolib-3.4.0/test/core/model_check_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/core/model_export_test.py` & `resotolib-3.4.0/test/core/model_export_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/core/progress_test.py` & `resotolib-3.4.0/test/core/progress_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/core/tasks_test.py` & `resotolib-3.4.0/test/core/tasks_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/durations_test.py` & `resotolib-3.4.0/test/durations_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/json_bender_test.py` & `resotolib-3.4.0/test/json_bender_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/parse_util_test.py` & `resotolib-3.4.0/test/parse_util_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_args.py` & `resotolib-3.4.0/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_baseresources.py` & `resotolib-3.4.0/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_config.py` & `resotolib-3.4.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_graph.py` & `resotolib-3.4.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_graph_extensions.py` & `resotolib-3.4.0/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_json.py` & `resotolib-3.4.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_jwt.py` & `resotolib-3.4.0/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_plugin.py` & `resotolib-3.4.0/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_tree.py` & `resotolib-3.4.0/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_utils.py` & `resotolib-3.4.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_web.py` & `resotolib-3.4.0/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.4/test/test_x509.py` & `resotolib-3.4.0/test/test_x509.py`

 * *Files identical despite different names*

