# Comparing `tmp/docts-0.1.0.tar.gz` & `tmp/docts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docts-0.1.0.tar", last modified: Sat Nov 27 15:01:46 2021, max compression
+gzip compressed data, was "docts-0.2.1.tar", last modified: Thu Apr 27 08:24:43 2023, max compression
```

## Comparing `docts-0.1.0.tar` & `docts-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:46.062020 docts-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-11-27 15:01:34.000000 docts-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13877 2021-11-27 15:01:46.062020 docts-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12820 2021-11-27 15:01:34.000000 docts-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:46.062020 docts-0.1.0/docts/
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2021-11-27 15:01:34.000000 docts-0.1.0/docts/Doc.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-11-27 15:01:38.000000 docts-0.1.0/docts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:46.062020 docts-0.1.0/docts/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-11-27 15:01:34.000000 docts-0.1.0/docts/filter/F1.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-27 15:01:34.000000 docts-0.1.0/docts/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:46.062020 docts-0.1.0/docts/map/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-11-27 15:01:34.000000 docts-0.1.0/docts/map/M1.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-27 15:01:34.000000 docts-0.1.0/docts/map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:46.062020 docts-0.1.0/docts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13877 2021-11-27 15:01:46.000000 docts-0.1.0/docts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-11-27 15:01:46.000000 docts-0.1.0/docts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-27 15:01:46.000000 docts-0.1.0/docts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-27 15:01:46.000000 docts-0.1.0/docts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-27 15:01:46.000000 docts-0.1.0/docts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-27 15:01:34.000000 docts-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-11-27 15:01:46.062020 docts-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:46.062020 docts-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-11-27 15:01:34.000000 docts-0.1.0/tests/InstallShield.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-27 15:01:34.000000 docts-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-11-27 15:01:34.000000 docts-0.1.0/tests/parse_xls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2021-11-27 15:01:34.000000 docts-0.1.0/tests/test_WordsFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-11-27 15:01:34.000000 docts-0.1.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-11-27 15:01:34.000000 docts-0.1.0/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-11-27 15:01:34.000000 docts-0.1.0/tests/test_parse_xlf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.626972 docts-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 08:24:33.000000 docts-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 08:24:33.000000 docts-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 08:24:43.626972 docts-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 08:24:33.000000 docts-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 08:24:33.000000 docts-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 08:24:33.000000 docts-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:24:43.626972 docts-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.622972 docts-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.626972 docts-0.2.1/src/docts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-27 08:24:42.000000 docts-0.2.1/src/docts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 08:24:33.000000 docts-0.2.1/src/docts/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:24:43.626972 docts-0.2.1/src/docts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 08:24:43.000000 docts-0.2.1/src/docts.egg-info/top_level.txt
```

### Comparing `docts-0.1.0/LICENSE` & `docts-0.2.1/LICENSE`

 * *Files identical despite different names*

