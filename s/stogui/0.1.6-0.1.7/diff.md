# Comparing `tmp/stogui-0.1.6.tar.gz` & `tmp/stogui-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stogui-0.1.6.tar", last modified: Tue Apr 25 23:38:30 2023, max compression
+gzip compressed data, was "stogui-0.1.7.tar", last modified: Thu Apr 27 02:31:16 2023, max compression
```

## Comparing `stogui-0.1.6.tar` & `stogui-0.1.7.tar`

### file list

```diff
@@ -1,52 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.745357 stogui-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 23:37:32.000000 stogui-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 23:37:32.000000 stogui-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 23:38:30.745357 stogui-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 23:37:32.000000 stogui-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 23:38:30.745357 stogui-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 23:37:32.000000 stogui-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.721356 stogui-0.1.6/stogui/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.725356 stogui-0.1.6/stogui/pipeline_maker/
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.721356 stogui-0.1.6/stogui/pipeline_maker/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.725356 stogui-0.1.6/stogui/pipeline_maker/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.721356 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.733357 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1718475 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  6244744 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    19537 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.733357 stogui-0.1.6/stogui/session_table/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.721356 stogui-0.1.6/stogui/session_table/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.737357 stogui-0.1.6/stogui/session_table/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/precache-manifest.c54c351d49044c01549cdc85c1442590.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.721356 stogui-0.1.6/stogui/session_table/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.745357 stogui-0.1.6/stogui/session_table/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1555139 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  5532059 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    68447 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-25 23:37:32.000000 stogui-0.1.6/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:38:30.725356 stogui-0.1.6/stogui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 23:38:30.000000 stogui-0.1.6/stogui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-25 23:38:30.000000 stogui-0.1.6/stogui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:38:30.000000 stogui-0.1.6/stogui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:38:30.000000 stogui-0.1.6/stogui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 23:38:30.000000 stogui-0.1.6/stogui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 23:38:30.000000 stogui-0.1.6/stogui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.032103 stogui-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 02:30:18.000000 stogui-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 02:30:18.000000 stogui-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 02:31:16.032103 stogui-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 02:30:18.000000 stogui-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 02:31:16.032103 stogui-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 02:30:18.000000 stogui-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/pipeline_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/pipeline_maker/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.008103 stogui-0.1.7/stogui/pipeline_maker/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.016102 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1718475 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-27 02:30:18.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  6244744 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19537 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.016102 stogui-0.1.7/stogui/session_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/session_table/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.016102 stogui-0.1.7/stogui/session_table/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/precache-manifest.c54c351d49044c01549cdc85c1442590.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/session_table/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.024103 stogui-0.1.7/stogui/session_table/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1555139 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  5532059 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    68447 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.024103 stogui-0.1.7/stogui/test_results_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/test_results_table/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.024103 stogui-0.1.7/stogui/test_results_table/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/precache-manifest.91a20b17e78199fc69d18c83d3df89a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui/test_results_table/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.032103 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1557976 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/2.6d15c91c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/2.6d15c91c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  5588155 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/2.6d15c91c.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/main.9a33623c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    70107 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/main.9a33623c.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-27 02:30:19.000000 stogui-0.1.7/stogui/test_results_table/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:31:16.004102 stogui-0.1.7/stogui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 02:31:15.000000 stogui-0.1.7/stogui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-27 02:31:15.000000 stogui-0.1.7/stogui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 02:31:15.000000 stogui-0.1.7/stogui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 02:31:15.000000 stogui-0.1.7/stogui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 02:31:15.000000 stogui-0.1.7/stogui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 02:31:15.000000 stogui-0.1.7/stogui.egg-info/top_level.txt
```

### Comparing `stogui-0.1.6/LICENSE` & `stogui-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/__init__.py` & `stogui-0.1.7/stogui/pipeline_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/asset-manifest.json` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/bootstrap.min.css` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/index.html` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/service-worker.js` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map` & `stogui-0.1.7/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/__init__.py` & `stogui-0.1.7/stogui/session_table/__init__.py`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/asset-manifest.json` & `stogui-0.1.7/stogui/session_table/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/bootstrap.min.css` & `stogui-0.1.7/stogui/session_table/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/index.html` & `stogui-0.1.7/stogui/session_table/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/precache-manifest.c54c351d49044c01549cdc85c1442590.js` & `stogui-0.1.7/stogui/session_table/frontend/build/precache-manifest.c54c351d49044c01549cdc85c1442590.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/service-worker.js` & `stogui-0.1.7/stogui/session_table/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.LICENSE.txt` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.map` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/2.268fd857.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js.map` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/main.7b870594.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.6/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map` & `stogui-0.1.7/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map`

 * *Files identical despite different names*

