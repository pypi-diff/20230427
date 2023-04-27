# Comparing `tmp/here-search-demo-0.8.4.tar.gz` & `tmp/here-search-demo-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "here-search-demo-0.8.4.tar", last modified: Wed Apr 26 05:10:10 2023, max compression
+gzip compressed data, was "here-search-demo-0.8.5.tar", last modified: Thu Apr 27 15:17:25 2023, max compression
```

## Comparing `here-search-demo-0.8.4.tar` & `here-search-demo-0.8.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.755526 here-search-demo-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-26 05:10:10.755526 here-search-demo-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.743526 here-search-demo-0.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/docs/developers.md
--rw-r--r--   0 runner    (1001) docker     (123)   678996 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/docs/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.747526 here-search-demo-0.8.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/requirements/lite_run.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/requirements/util.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-26 05:10:10.755526 here-search-demo-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.743526 here-search-demo-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.739526 here-search-demo-0.8.4/src/here_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.747526 here-search-demo-0.8.4/src/here_search/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/api_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.751526 here-search-demo-0.8.4/src/here_search/demo/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/entity/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/entity/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/entity/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/entity/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/entity/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/lite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.751526 here-search-demo-0.8.4/src/here_search/demo/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/notebooks/obm_1_api.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/notebooks/obm_2_api.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/notebooks/obm_3_widget.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.751526 here-search-demo-0.8.4/src/here_search/demo/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/scripts/here-search-notebooks
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/scripts/lite-run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.751526 here-search-demo-0.8.4/src/here_search/demo/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/widgets/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/widgets/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/widgets/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/src/here_search/demo/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.755526 here-search-demo-0.8.4/src/here_search_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-26 05:10:10.000000 here-search-demo-0.8.4/src/here_search_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-26 05:10:10.000000 here-search-demo-0.8.4/src/here_search_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:10:10.000000 here-search-demo-0.8.4/src/here_search_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:10:10.000000 here-search-demo-0.8.4/src/here_search_demo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-26 05:10:10.000000 here-search-demo-0.8.4/src/here_search_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 05:10:10.000000 here-search-demo-0.8.4/src/here_search_demo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:10:10.755526 here-search-demo-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-26 05:09:50.000000 here-search-demo-0.8.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/docs/developers.md
+-rw-r--r--   0 runner    (1001) docker     (123)   678996 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/docs/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/lite_run.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/requirements/util.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:24.997240 here-search-demo-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:24.997240 here-search-demo-0.8.5/src/here_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/src/here_search/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/api_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.001240 here-search-demo-0.8.5/src/here_search/demo/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/entity/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/lite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search/demo/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_1_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_2_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_3_widget.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search/demo/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/scripts/here-search-notebooks
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/scripts/lite-run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search/demo/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/src/here_search/demo/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/src/here_search_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:17:24.000000 here-search-demo-0.8.5/src/here_search_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:17:25.005240 here-search-demo-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-27 15:17:02.000000 here-search-demo-0.8.5/tests/test_util.py
```

### Comparing `here-search-demo-0.8.4/LICENSE` & `here-search-demo-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/PKG-INFO` & `here-search-demo-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here-search-demo
-Version: 0.8.4
+Version: 0.8.5
 Summary: HERE Geocoding and Search demo and widgets
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
 Project-URL: Bug Tracker, https://github.com/heremaps/here-search-demo/issues
 Project-URL: Source, https://github.com/heremaps/here-search-demo
```

### Comparing `here-search-demo-0.8.4/README.md` & `here-search-demo-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/docs/developers.md` & `here-search-demo-0.8.5/docs/developers.md`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/docs/screenshot.png` & `here-search-demo-0.8.5/docs/screenshot.png`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/setup.cfg` & `here-search-demo-0.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/api.py` & `here-search-demo-0.8.5/src/here_search/demo/api.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/api_options.py` & `here-search-demo-0.8.5/src/here_search/demo/api_options.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/base.py` & `here-search-demo-0.8.5/src/here_search/demo/base.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/entity/endpoint.py` & `here-search-demo-0.8.5/src/here_search/demo/entity/endpoint.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/entity/intent.py` & `here-search-demo-0.8.5/src/here_search/demo/entity/intent.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/entity/place.py` & `here-search-demo-0.8.5/src/here_search/demo/entity/place.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/entity/request.py` & `here-search-demo-0.8.5/src/here_search/demo/entity/request.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/event.py` & `here-search-demo-0.8.5/src/here_search/demo/event.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/lite.py` & `here-search-demo-0.8.5/src/here_search/demo/lite.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/notebooks/demo.ipynb` & `here-search-demo-0.8.5/src/here_search/demo/notebooks/demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994047619047619%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.5-py3-none-any.whl"], '*

 * *            "keep_going=True)\\n')], delete: [2]}}}"}*

```diff
@@ -5,15 +5,15 @@
             "execution_count": null,
             "id": "717d9c13-684f-4ef9-8045-09624217caeb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.0-py3-none-any.whl\"], keep_going=True)\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
                 "    api_key = \"<YOUR API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `here-search-demo-0.8.4/src/here_search/demo/notebooks/obm_1_api.ipynb` & `here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_1_api.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998249299719888%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.5-py3-none-any.whl"], '*

 * *            "keep_going=True)\\n')], delete: [2]}}}"}*

```diff
@@ -5,15 +5,15 @@
             "execution_count": 1,
             "id": "e5c95683-6b47-40aa-8dba-1c815e1549c3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.0-py3-none-any.whl\"], keep_going=True)\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
                 "    api_key = \"<YOUR API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `here-search-demo-0.8.4/src/here_search/demo/notebooks/obm_2_api.ipynb` & `here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_2_api.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999702380952381%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.5-py3-none-any.whl"], '*

 * *            "keep_going=True)\\n')], delete: [2]}}}"}*

```diff
@@ -5,15 +5,15 @@
             "execution_count": 1,
             "id": "77ac7de0-8ebc-4686-87bf-a9e720cc79e4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.0-py3-none-any.whl\"], keep_going=True)\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
                 "    api_key = \"<YOUR API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `here-search-demo-0.8.4/src/here_search/demo/notebooks/obm_3_widget.ipynb` & `here-search-demo-0.8.5/src/here_search/demo/notebooks/obm_3_widget.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997519841269842%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, \'    await piplite.install(["ipywidgets==7.7.2", '*

 * *            '"ipyleaflet==0.17.1", "emfs:here_search_demo-0.8.5-py3-none-any.whl"], '*

 * *            "keep_going=True)\\n')], delete: [2]}}}"}*

```diff
@@ -5,15 +5,15 @@
             "execution_count": null,
             "id": "f4878c23-f9ec-4756-b085-bdccf7d726d8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import piplite\n",
-                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.0-py3-none-any.whl\"], keep_going=True)\n",
+                "    await piplite.install([\"ipywidgets==7.7.2\", \"ipyleaflet==0.17.1\", \"emfs:here_search_demo-0.8.5-py3-none-any.whl\"], keep_going=True)\n",
                 "    api_key = \"<YOUR API KEY>\"\n",
                 "except ImportError:\n",
                 "    api_key = None"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `here-search-demo-0.8.4/src/here_search/demo/scripts/lite-run.sh` & `here-search-demo-0.8.5/src/here_search/demo/scripts/lite-run.sh`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/user.py` & `here-search-demo-0.8.5/src/here_search/demo/user.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/util.py` & `here-search-demo-0.8.5/src/here_search/demo/util.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/widgets/app.py` & `here-search-demo-0.8.5/src/here_search/demo/widgets/app.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/widgets/input.py` & `here-search-demo-0.8.5/src/here_search/demo/widgets/input.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/widgets/output.py` & `here-search-demo-0.8.5/src/here_search/demo/widgets/output.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search/demo/widgets/util.py` & `here-search-demo-0.8.5/src/here_search/demo/widgets/util.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/src/here_search_demo.egg-info/PKG-INFO` & `here-search-demo-0.8.5/src/here_search_demo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here-search-demo
-Version: 0.8.4
+Version: 0.8.5
 Summary: HERE Geocoding and Search demo and widgets
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
 Project-URL: Bug Tracker, https://github.com/heremaps/here-search-demo/issues
 Project-URL: Source, https://github.com/heremaps/here-search-demo
```

### Comparing `here-search-demo-0.8.4/src/here_search_demo.egg-info/SOURCES.txt` & `here-search-demo-0.8.5/src/here_search_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/tests/test_api.py` & `here-search-demo-0.8.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/tests/test_base.py` & `here-search-demo-0.8.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/tests/test_entities.py` & `here-search-demo-0.8.5/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.4/tests/test_util.py` & `here-search-demo-0.8.5/tests/test_util.py`

 * *Files identical despite different names*

