# Comparing `tmp/grblogtools-2.0.0.tar.gz` & `tmp/grblogtools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grblogtools-2.0.0.tar", last modified: Mon Apr  4 08:38:13 2022, max compression
+gzip compressed data, was "grblogtools-2.1.0.tar", last modified: Thu Apr 27 13:20:29 2023, max compression
```

## Comparing `grblogtools-2.0.0.tar` & `grblogtools-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.950788 grblogtools-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10976 2022-04-04 08:37:57.000000 grblogtools-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-04 08:38:13.950788 grblogtools-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-04 08:37:57.000000 grblogtools-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-04 08:37:57.000000 grblogtools-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-04-04 08:38:13.950788 grblogtools-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.942788 grblogtools-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.946788 grblogtools-2.0.0/src/grblogtools/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6557 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.946788 grblogtools-2.0.0/src/grblogtools/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.946788 grblogtools-2.0.0/src/grblogtools/parameters/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/800.json
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/801.json
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/810.json
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/811.json
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/900.json
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/901.json
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/902.json
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/903.json
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/910.json
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/911.json
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/912.json
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/950.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/data/descriptions.json
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parameters/pretty.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.950788 grblogtools-2.0.0/src/grblogtools/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/barrier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/continuous.py
--rw-r--r--   0 runner    (1001) docker     (121)     3193 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/header.py
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/nodelog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/norel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/presolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/simplex.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/single_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/termination.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/parsers/util.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3198 2022-04-04 08:37:57.000000 grblogtools-2.0.0/src/grblogtools/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 08:38:13.946788 grblogtools-2.0.0/src/grblogtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-04 08:38:13.000000 grblogtools-2.0.0/src/grblogtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-04-04 08:38:13.000000 grblogtools-2.0.0/src/grblogtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 08:38:13.000000 grblogtools-2.0.0/src/grblogtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-04 08:38:13.000000 grblogtools-2.0.0/src/grblogtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-04 08:38:13.000000 grblogtools-2.0.0/src/grblogtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.922702 grblogtools-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-27 13:20:15.000000 grblogtools-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-27 13:20:29.922702 grblogtools-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-27 13:20:15.000000 grblogtools-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 13:20:15.000000 grblogtools-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-27 13:20:29.922702 grblogtools-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.910702 grblogtools-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.914702 grblogtools-2.1.0/src/grblogtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.914702 grblogtools-2.1.0/src/grblogtools/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.918702 grblogtools-2.1.0/src/grblogtools/parameters/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/1000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/1001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/800.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/801.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/810.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/811.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/900.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/901.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/902.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/903.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/910.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/911.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/912.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/950.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/951.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/952.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/data/descriptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parameters/pretty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.918702 grblogtools-2.1.0/src/grblogtools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/nodelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/norel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/presolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/simplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/single_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/parsers/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3198 2023-04-27 13:20:15.000000 grblogtools-2.1.0/src/grblogtools/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.914702 grblogtools-2.1.0/src/grblogtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-27 13:20:29.000000 grblogtools-2.1.0/src/grblogtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-27 13:20:29.000000 grblogtools-2.1.0/src/grblogtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:20:29.000000 grblogtools-2.1.0/src/grblogtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 13:20:29.000000 grblogtools-2.1.0/src/grblogtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:20:29.000000 grblogtools-2.1.0/src/grblogtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:20:29.922702 grblogtools-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-27 13:20:15.000000 grblogtools-2.1.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-27 13:20:15.000000 grblogtools-2.1.0/tests/test_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-27 13:20:15.000000 grblogtools-2.1.0/tests/test_fill_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 13:20:15.000000 grblogtools-2.1.0/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 13:20:15.000000 grblogtools-2.1.0/tests/test_plotting.py
```

### Comparing `grblogtools-2.0.0/LICENSE` & `grblogtools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/PKG-INFO` & `grblogtools-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grblogtools
-Version: 2.0.0
+Version: 2.1.0
 Summary: Gurobi log file tools for parsing and exploring data
 Home-page: https://github.com/Gurobi/grblogtools
 Author: Gurobi Optimization, LLC
 Author-email: support@gurobi.com
 License: Apache-2.0
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
@@ -73,15 +73,15 @@
     - progress charts for the individual runs:
     ```Python
     glt.plot(nodelog_progress, y="Gap", color="Log", type="line")
     ```
 
     - progress of the norel heuristic (note, the time recorded here is since the start of norel, and does not include presolve + read time):
     ```Python
-    glt.plot(result.progress("norel"), x="Time", y="Incumbent", color="Log", type="line")
+    glt.plot(results.progress("norel"), x="Time", y="Incumbent", color="Log", type="line")
     ```
 
     These are just examples using the [Plotly Python library](https://plotly.com/python/) - of course, any other plotting library of your choice can be used to work with these DataFrames.
 
 ## Excel
 Convert your log files to Excel worksheets right on the command-line:
 
@@ -90,9 +90,7 @@
 ```
 
 List all available options and how to use the command-line tool:
 
 ```
 python -m grblogtools --help
 ```
-
-
```

### Comparing `grblogtools-2.0.0/README.md` & `grblogtools-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     - progress charts for the individual runs:
     ```Python
     glt.plot(nodelog_progress, y="Gap", color="Log", type="line")
     ```
 
     - progress of the norel heuristic (note, the time recorded here is since the start of norel, and does not include presolve + read time):
     ```Python
-    glt.plot(result.progress("norel"), x="Time", y="Incumbent", color="Log", type="line")
+    glt.plot(results.progress("norel"), x="Time", y="Incumbent", color="Log", type="line")
     ```
 
     These are just examples using the [Plotly Python library](https://plotly.com/python/) - of course, any other plotting library of your choice can be used to work with these DataFrames.
 
 ## Excel
 Convert your log files to Excel worksheets right on the command-line:
```

### Comparing `grblogtools-2.0.0/setup.cfg` & `grblogtools-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/api.py` & `grblogtools-2.1.0/src/grblogtools/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
         Returns:
             pd.DataFrame: A data frame representing the progress of the given section
                 in the log.
         """
         progress = []
         for logfile, lognumber, parser in self.parsers:
-
             if section == "nodelog":
                 log = parser.nodelog_parser.get_progress()
             elif section == "rootlp":
                 log = parser.continuous_parser.get_progress()
             elif section == "norel":
                 log = parser.norel_parser.get_progress()
             else:
```

### Comparing `grblogtools-2.0.0/src/grblogtools/cli.py` & `grblogtools-2.1.0/src/grblogtools/cli.py`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/helpers.py` & `grblogtools-2.1.0/src/grblogtools/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """Fill NaN parameter values with the actual default value."""
     parameter_columns = [
         column
         for column, series in summary.items()
         if re_parameter_column.match(column) and series.isnull().any()
     ]
     # TODO test cases where there are different versions involved
-    return summary.groupby("Version").apply(
+    return summary.groupby("Version", group_keys=False).apply(
         partial(fill_for_version, parameter_columns=parameter_columns)
     )
 
 
 def fill_for_version_nosuffix(group):
     parameter_defaults = load_defaults(
         version=group["Version"].iloc[0].replace(".", "")
@@ -40,15 +40,17 @@
         if default is not None:
             group[parameter] = group[parameter].fillna(default).astype(type(default))
     return group
 
 
 def fill_default_parameters_nosuffix(parameters):
     """Fill defaults for Version and parameter cols with no (Parameter) suffix."""
-    return parameters.groupby("Version").apply(fill_for_version_nosuffix)
+    return parameters.groupby("Version", group_keys=False).apply(
+        fill_for_version_nosuffix
+    )
 
 
 def add_categorical_descriptions(summary):
     """Replace some columns with categorical descriptions if available.
 
     It modifies the summary dict in place.
     """
```

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/800.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/800.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/801.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/801.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/810.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/810.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/811.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/811.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/900.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/900.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/901.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/901.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/902.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/902.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/903.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/903.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/910.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/910.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/911.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/911.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/912.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/912.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/950.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/950.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parameters/data/descriptions.json` & `grblogtools-2.1.0/src/grblogtools/parameters/data/descriptions.json`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/barrier.py` & `grblogtools-2.1.0/src/grblogtools/parsers/barrier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from grblogtools.parsers.util import typeconvert_groupdict
+from grblogtools.parsers.util import float_pattern, typeconvert_groupdict
 
 
 class BarrierParser:
     # The pattern indicating the initialization of the parser
     barrier_start_pattern = re.compile(
         r"Iter(\s+)Primal(\s+)Dual(\s+)Primal(\s+)Dual(\s+)Compl(\s+)Time"
     )
@@ -20,14 +20,24 @@
     barrier_crossover_pattern = re.compile(
         r"\s*Push phase complete: Pinf (?P<PushPhasePInf>[^\s]+), Dinf (?P<PushPhaseDInf>[^\s]+)\s+(?P<PushPhaseEndTime>\d+)s"
     )
 
     # The pattern indicating the termination of the barrier algorithm
     barrier_termination_patterns = [
         re.compile(
+            r"Barrier solved model in (?P<BarIterCount>[^\s]+) iterations and (?P<Runtime>{0}) seconds \((?P<Work>{0}) work units\)".format(
+                float_pattern
+            )
+        ),
+        re.compile(
+            r"Barrier performed (?P<BarIterCount>\d+) iterations in (?P<Runtime>{0}) seconds \((?P<Work>{0}) work units\)".format(
+                float_pattern
+            )
+        ),
+        re.compile(
             r"Barrier solved model in (?P<BarIterCount>[^\s]+) iterations and (?P<Runtime>[^\s]+) seconds"
         ),
         re.compile(
             r"Barrier performed (?P<BarIterCount>\d+) iterations in (?P<Runtime>[^\s]+) seconds"
         ),
     ]
```

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/continuous.py` & `grblogtools-2.1.0/src/grblogtools/parsers/continuous.py`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/header.py` & `grblogtools-2.1.0/src/grblogtools/parsers/header.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         re.compile(r"Compute Server job ID: (?P<JobID>.*)$"),
         re.compile(r"Gurobi Optimizer version (?P<Version>\d{1,2}\.[^\s]+)"),
         re.compile(
             r"Gurobi Compute Server Worker version (?P<Version>\d{1,2}\.[^\s]+) build (.*) \((?P<Platform>[^\)]+)\)$"
         ),
         re.compile(r"Compute Server job ID: (?P<JobID>.*)$"),
         re.compile(r"Gurobi Optimizer version (?P<Version>\d{1,2}\.[^\s]+)"),
+        re.compile(r"Solving model (?P<ModelName>.*)$"),
     ]
 
     header_other_patterns = [
         re.compile(r"Read (MPS|LP) format model from file (?P<ModelFilePath>.*)$"),
         re.compile(r"Reading time = (?P<ReadingTime>[\d\.]+) seconds"),
         re.compile(
             r"Thread count: (?P<PhysicalCores>\d+) physical cores, (?P<LogicalProcessors>\d+) logical processors, using up to (?P<Threads>\d+) threads"
@@ -82,7 +83,11 @@
     def get_summary(self) -> dict:
         """Return the current parsed summary."""
         return self._summary
 
     def get_parameters(self) -> dict:
         """Return all changed parameters detected in the header."""
         return self._parameters
+
+    def changed_params(self) -> int:
+        omit_params = {"Seed", "LogFile"}
+        return {k: v for k, v in self._parameters.items() if k not in omit_params}
```

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/nodelog.py` & `grblogtools-2.1.0/src/grblogtools/parsers/nodelog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import re
 
-from grblogtools.parsers.util import convert_data_types, typeconvert_groupdict
-
-float_pattern = r"[-+]?((\d*\.\d+)|(\d+\.?))([Ee][+-]?\d+)?"
+from grblogtools.parsers.util import (
+    convert_data_types,
+    float_pattern,
+    typeconvert_groupdict,
+)
 
 
 class NodeLogParser:
     tree_search_start = re.compile(r" Expl Unexpl(.*)It/Node Time$")
 
     tree_search_final_stats = [
         re.compile(
+            r"Explored (?P<NodeCount>\d+) nodes \((?P<IterCount>\d+) simplex iterations\) in (?P<Runtime>{0}) seconds \((?P<Work>{0}) work units\)".format(
+                float_pattern
+            )
+        ),
+        re.compile(
             r"Explored (?P<NodeCount>\d+) nodes \((?P<IterCount>\d+) simplex iterations\) in (?P<Runtime>[^\s]+) seconds"
         ),
         re.compile(
             r"Best objective (?P<ObjVal>[^,]+), best bound (?P<ObjBound>[^,]+), gap (?P<MIPGap>.*)$"
         ),
     ]
```

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/norel.py` & `grblogtools-2.1.0/src/grblogtools/parsers/norel.py`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/presolve.py` & `grblogtools-2.1.0/src/grblogtools/parsers/presolve.py`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/simplex.py` & `grblogtools-2.1.0/src/grblogtools/parsers/simplex.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import re
 
-from grblogtools.parsers.util import typeconvert_groupdict
+from grblogtools.parsers.util import float_pattern, typeconvert_groupdict
 
 
 class SimplexParser:
     # The pattern indicating the initialization of the parser
     simplex_start_pattern = re.compile(
         r"Iteration(\s+)Objective(\s+)Primal Inf.(\s+)Dual Inf.(\s+)Time"
     )
 
     # The pattern indicating the simplex progress
     simplex_progress_pattern = re.compile(
         r"\s*(?P<Iteration>\d+)\s+(?P<Objective>[^\s]+)\s+(?P<PInf>[^\s]+)\s+(?P<DInf>[^\s]+)\s+(?P<Time>\d+)s"
     )
 
     # The pattern indicating the termination of the simplex method
-    simplex_termination_pattern = re.compile(
-        r"(Solved|Stopped) in (?P<IterCount>[^\s]+) iterations and (?P<Runtime>[^\s]+) seconds"
-    )
+    simplex_termination_patterns = [
+        re.compile(
+            r"(Solved|Stopped) in (?P<IterCount>[^\s]+) iterations and (?P<Runtime>{0}) seconds \((?P<Work>{0}) work units\)".format(
+                float_pattern
+            )
+        ),
+        re.compile(
+            r"(Solved|Stopped) in (?P<IterCount>[^\s]+) iterations and (?P<Runtime>[^\s]+) seconds"
+        ),
+    ]
 
     def __init__(self):
         """Initialize the Simplex parser."""
         self._summary = {}
         self._progress = []
         self._started = False
 
@@ -32,18 +39,21 @@
             line (str): A line in the log file.
 
         Returns:
             bool: Return True if the given line is matched by some pattern.
         """
         # Check this first since the termination line might appear
         # without any progress log in the concurrent case.
-        match = SimplexParser.simplex_termination_pattern.match(line)
-        if match:
-            self._summary.update(typeconvert_groupdict(match))
-            return True
+
+        for regex in self.simplex_termination_patterns:
+            match = regex.match(line)
+            if match:
+                entry = typeconvert_groupdict(match)
+                self._summary.update(entry)
+                return True
 
         if not self._started:
             match = SimplexParser.simplex_start_pattern.match(line)
             if match:
                 self._started = True
                 return True
             return False
```

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/single_log.py` & `grblogtools-2.1.0/src/grblogtools/parsers/single_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             discrete_vars=summary.get("PresolvedNumBinVars", 0)
             + summary.get("PresolvedNumIntVars", 0)
             + summary.get("PresolvedNumSemiContVars", 0)
             + summary.get("PresolvedNumSemiIntVars", 0),
             quad_nonzeros=summary.get("NumQNZs", 0),
             quad_constrs=summary.get("NumQConstrs", 0),
         )
+        summary["ChangedParams"] = self.header_parser.changed_params()
         return summary
 
     def parse(self, line: str) -> bool:
         """Parse the given log line to populate the component parsers in sequence.
 
         Args:
             line (str): A line in the log file.
```

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/termination.py` & `grblogtools-2.1.0/src/grblogtools/parsers/termination.py`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools/parsers/util.py` & `grblogtools-2.1.0/src/grblogtools/parsers/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 import re
 from typing import Iterable
 
+float_pattern = r"[-+]?((\d*\.\d+)|(\d+\.?))([Ee][+-]?\d+)?"
+
 int_regex = re.compile(r"[-+]?\d+$")
 float_regex = re.compile(r"[-+]?((\d*\.\d+)|(\d+\.?))([Ee][+-]?\d+)?$")
 percentage_regex = re.compile(r"[-+]?((\d*\.\d+)|(\d+\.?))([Ee][+-]?\d+)?%$")
 date_time_regex = re.compile(r"\D+\s\D+\s\d+\s\d+:\d+:\d+\s\d{4}")
 
 
 def convert_data_types(value):
```

### Comparing `grblogtools-2.0.0/src/grblogtools/plotting.py` & `grblogtools-2.1.0/src/grblogtools/plotting.py`

 * *Files identical despite different names*

### Comparing `grblogtools-2.0.0/src/grblogtools.egg-info/PKG-INFO` & `grblogtools-2.1.0/src/grblogtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grblogtools
-Version: 2.0.0
+Version: 2.1.0
 Summary: Gurobi log file tools for parsing and exploring data
 Home-page: https://github.com/Gurobi/grblogtools
 Author: Gurobi Optimization, LLC
 Author-email: support@gurobi.com
 License: Apache-2.0
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
@@ -73,15 +73,15 @@
     - progress charts for the individual runs:
     ```Python
     glt.plot(nodelog_progress, y="Gap", color="Log", type="line")
     ```
 
     - progress of the norel heuristic (note, the time recorded here is since the start of norel, and does not include presolve + read time):
     ```Python
-    glt.plot(result.progress("norel"), x="Time", y="Incumbent", color="Log", type="line")
+    glt.plot(results.progress("norel"), x="Time", y="Incumbent", color="Log", type="line")
     ```
 
     These are just examples using the [Plotly Python library](https://plotly.com/python/) - of course, any other plotting library of your choice can be used to work with these DataFrames.
 
 ## Excel
 Convert your log files to Excel worksheets right on the command-line:
 
@@ -90,9 +90,7 @@
 ```
 
 List all available options and how to use the command-line tool:
 
 ```
 python -m grblogtools --help
 ```
-
-
```

### Comparing `grblogtools-2.0.0/src/grblogtools.egg-info/SOURCES.txt` & `grblogtools-2.1.0/src/grblogtools.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,32 +12,41 @@
 src/grblogtools.egg-info/SOURCES.txt
 src/grblogtools.egg-info/dependency_links.txt
 src/grblogtools.egg-info/requires.txt
 src/grblogtools.egg-info/top_level.txt
 src/grblogtools/parameters/__init__.py
 src/grblogtools/parameters/defaults.py
 src/grblogtools/parameters/pretty.py
+src/grblogtools/parameters/data/1000.json
+src/grblogtools/parameters/data/1001.json
 src/grblogtools/parameters/data/800.json
 src/grblogtools/parameters/data/801.json
 src/grblogtools/parameters/data/810.json
 src/grblogtools/parameters/data/811.json
 src/grblogtools/parameters/data/900.json
 src/grblogtools/parameters/data/901.json
 src/grblogtools/parameters/data/902.json
 src/grblogtools/parameters/data/903.json
 src/grblogtools/parameters/data/910.json
 src/grblogtools/parameters/data/911.json
 src/grblogtools/parameters/data/912.json
 src/grblogtools/parameters/data/950.json
+src/grblogtools/parameters/data/951.json
+src/grblogtools/parameters/data/952.json
 src/grblogtools/parameters/data/__init__.py
 src/grblogtools/parameters/data/descriptions.json
 src/grblogtools/parsers/__init__.py
 src/grblogtools/parsers/barrier.py
 src/grblogtools/parsers/continuous.py
 src/grblogtools/parsers/header.py
 src/grblogtools/parsers/nodelog.py
 src/grblogtools/parsers/norel.py
 src/grblogtools/parsers/presolve.py
 src/grblogtools/parsers/simplex.py
 src/grblogtools/parsers/single_log.py
 src/grblogtools/parsers/termination.py
-src/grblogtools/parsers/util.py
+src/grblogtools/parsers/util.py
+tests/test_api.py
+tests/test_cuts.py
+tests/test_fill_defaults.py
+tests/test_load.py
+tests/test_plotting.py
```

