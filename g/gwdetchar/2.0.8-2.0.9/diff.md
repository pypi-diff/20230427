# Comparing `tmp/gwdetchar-2.0.8.tar.gz` & `tmp/gwdetchar-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.0.8.tar", last modified: Tue Apr 25 23:12:37 2023, max compression
+gzip compressed data, was "gwdetchar-2.0.9.tar", last modified: Thu Apr 27 00:58:43 2023, max compression
```

## Comparing `gwdetchar-2.0.8.tar` & `gwdetchar-2.0.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.721923 gwdetchar-2.0.8/
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)      100 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-25 23:12:37.722127 gwdetchar-2.0.8/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.724659 gwdetchar-2.0.8/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1113 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-04-25 23:12:37.724775 gwdetchar-2.0.8/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4716 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.0.8/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3044 2023-04-25 15:49:41.000000 gwdetchar-2.0.8/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.691360 gwdetchar-2.0.8/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7367 2023-02-28 19:11:25.000000 gwdetchar-2.0.8/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41524 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.693427 gwdetchar-2.0.8/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24193 2023-04-25 22:58:28.000000 gwdetchar-2.0.8/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.696694 gwdetchar-2.0.8/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    35157 2022-10-03 17:36:21.000000 gwdetchar-2.0.8/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.0.8/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.699200 gwdetchar-2.0.8/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3965 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.700826 gwdetchar-2.0.8/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.701964 gwdetchar-2.0.8/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.705942 gwdetchar-2.0.8/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12666 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.710132 gwdetchar-2.0.8/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13619 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.711554 gwdetchar-2.0.8/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.712423 gwdetchar-2.0.8/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.714717 gwdetchar-2.0.8/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.716918 gwdetchar-2.0.8/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.721562 gwdetchar-2.0.8/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.0.8/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.689130 gwdetchar-2.0.8/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2419 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2022-12-02 22:06:25.000000 gwdetchar-2.0.8/gwdetchar.egg-info/not-zip-safe
--rw-r--r--   0 egoetz     (501) staff       (20)      292 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3000 2023-04-25 23:12:37.724103 gwdetchar-2.0.8/setup.cfg
--rw-r--r--   0 egoetz     (501) staff       (20)     1205 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/setup.py
--rw-r--r--   0 egoetz     (501) staff       (20)    65747 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/versioneer.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.224574 gwdetchar-2.0.9/
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)      100 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-27 00:58:43.224785 gwdetchar-2.0.9/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.226881 gwdetchar-2.0.9/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1113 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-04-27 00:58:43.227017 gwdetchar-2.0.9/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4716 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.0.9/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3044 2023-04-25 15:49:41.000000 gwdetchar-2.0.9/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.152453 gwdetchar-2.0.9/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7367 2023-02-28 19:11:25.000000 gwdetchar-2.0.9/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41524 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.156779 gwdetchar-2.0.9/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24193 2023-04-25 22:58:28.000000 gwdetchar-2.0.9/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.165821 gwdetchar-2.0.9/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    35157 2022-10-03 17:36:21.000000 gwdetchar-2.0.9/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.0.9/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.169632 gwdetchar-2.0.9/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.173014 gwdetchar-2.0.9/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.180972 gwdetchar-2.0.9/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.194792 gwdetchar-2.0.9/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12666 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.200650 gwdetchar-2.0.9/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13619 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.203482 gwdetchar-2.0.9/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.204832 gwdetchar-2.0.9/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.209764 gwdetchar-2.0.9/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.216016 gwdetchar-2.0.9/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.223958 gwdetchar-2.0.9/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.0.9/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.148599 gwdetchar-2.0.9/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2419 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2022-12-02 22:06:25.000000 gwdetchar-2.0.9/gwdetchar.egg-info/not-zip-safe
+-rw-r--r--   0 egoetz     (501) staff       (20)      292 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3000 2023-04-27 00:58:43.226296 gwdetchar-2.0.9/setup.cfg
+-rw-r--r--   0 egoetz     (501) staff       (20)     1205 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/setup.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    65747 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/versioneer.py
```

### Comparing `gwdetchar-2.0.8/LICENSE` & `gwdetchar-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/PKG-INFO` & `gwdetchar-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.0.8
+Version: 2.0.9
 Summary: A python package for gravitational-wave detector characterisation
 Home-page: https://github.com/gwdetchar/gwdetchar/
 Author: Alex Urban, Duncan Macleod
 Author-email: alexander.urban@ligo.org
 License: GPL-3.0-or-later
 Keywords: physics,astronomy,gravitational-waves,ligo
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gwdetchar-2.0.8/README.rst` & `gwdetchar-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/__init__.py` & `gwdetchar-2.0.9/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/cds.py` & `gwdetchar-2.0.9/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/cli.py` & `gwdetchar-2.0.9/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/condor.py` & `gwdetchar-2.0.9/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/conftest.py` & `gwdetchar-2.0.9/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/conlog.py` & `gwdetchar-2.0.9/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/const.py` & `gwdetchar-2.0.9/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/daq.py` & `gwdetchar-2.0.9/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/__init__.py` & `gwdetchar-2.0.9/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/datafind.py` & `gwdetchar-2.0.9/gwdetchar/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/html.py` & `gwdetchar-2.0.9/gwdetchar/io/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/ligolw.py` & `gwdetchar-2.0.9/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.0.9/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.0.9/gwdetchar/io/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.0.9/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/__init__.py` & `gwdetchar-2.0.9/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/__main__.py` & `gwdetchar-2.0.9/gwdetchar/lasso/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/core.py` & `gwdetchar-2.0.9/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/old.py` & `gwdetchar-2.0.9/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/plot.py` & `gwdetchar-2.0.9/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.0.9/gwdetchar/lasso/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     nptest.assert_almost_equal(model.dual_gap_, 0)
     nptest.assert_almost_equal(model.predict([[0], [1]]), [0, 1])
 
 
 def test_find_alpha():
     # find the optimal alpha parameter
     alpha = core.find_alpha(DATA, TARGET)
-    assert alpha == 0.1
+    nptest.assert_almost_equal(alpha, 0.1)
 
 
 def test_remove_flat():
     # remove flat TimeSeries
     tsdict = core.remove_flat(TSDICT)
     assert len(tsdict.keys()) == 2
     assert 'flat' not in tsdict.keys()
```

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.0.9/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.0.9/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/mct.py` & `gwdetchar-2.0.9/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/nagios/__init__.py` & `gwdetchar-2.0.9/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/nagios/__main__.py` & `gwdetchar-2.0.9/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/nagios/core.py` & `gwdetchar-2.0.9/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.0.9/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/__init__.py` & `gwdetchar-2.0.9/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/__main__.py` & `gwdetchar-2.0.9/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/batch.py` & `gwdetchar-2.0.9/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/config.py` & `gwdetchar-2.0.9/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/core.py` & `gwdetchar-2.0.9/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/html.py` & `gwdetchar-2.0.9/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/plot.py` & `gwdetchar-2.0.9/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.0.9/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/overflow.py` & `gwdetchar-2.0.9/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/plot.py` & `gwdetchar-2.0.9/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/saturation/__init__.py` & `gwdetchar-2.0.9/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/saturation/__main__.py` & `gwdetchar-2.0.9/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/saturation/core.py` & `gwdetchar-2.0.9/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.0.9/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/__init__.py` & `gwdetchar-2.0.9/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/__main__.py` & `gwdetchar-2.0.9/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/core.py` & `gwdetchar-2.0.9/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/plot.py` & `gwdetchar-2.0.9/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/simple.py` & `gwdetchar-2.0.9/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/__init__.py` & `gwdetchar-2.0.9/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_cds.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_cli.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_condor.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_const.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_daq.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_plot.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/tests/test_utils.py` & `gwdetchar-2.0.9/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar/utils.py` & `gwdetchar-2.0.9/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.0.9/gwdetchar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.0.8
+Version: 2.0.9
 Summary: A python package for gravitational-wave detector characterisation
 Home-page: https://github.com/gwdetchar/gwdetchar/
 Author: Alex Urban, Duncan Macleod
 Author-email: alexander.urban@ligo.org
 License: GPL-3.0-or-later
 Keywords: physics,astronomy,gravitational-waves,ligo
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gwdetchar-2.0.8/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.0.9/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.0.9/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/setup.cfg` & `gwdetchar-2.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/setup.py` & `gwdetchar-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.8/versioneer.py` & `gwdetchar-2.0.9/versioneer.py`

 * *Files identical despite different names*

