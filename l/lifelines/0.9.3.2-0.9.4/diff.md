# Comparing `tmp/lifelines-0.9.3.2.tar.gz` & `tmp/lifelines-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lifelines-0.9.3.2.tar", last modified: Tue Nov  8 18:21:18 2016, max compression
+gzip compressed data, was "dist/lifelines-0.9.4.tar", last modified: Sun Jan  1 18:48:06 2017, max compression
```

## Comparing `lifelines-0.9.3.2.tar` & `lifelines-0.9.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1170 2014-02-12 03:26:48.000000 lifelines-0.9.3.2/LICENSE
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/lifelines/
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    12292 2015-01-03 00:46:11.000000 lifelines-0.9.3.2/lifelines/.DS_Store
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      444 2016-05-23 18:42:02.000000 lifelines-0.9.3.2/lifelines/__init__.py
--rwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)    32160 2014-05-31 18:23:45.000000 lifelines-0.9.3.2/lifelines/_statistics.so
--rwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)    32796 2014-12-13 14:04:01.000000 lifelines-0.9.3.2/lifelines/_utils.so
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/lifelines/datasets/
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/lifelines/datasets/.ipynb_checkpoints/
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   125625 2016-01-10 22:18:30.000000 lifelines-0.9.3.2/lifelines/datasets/.ipynb_checkpoints/Divorces Rates-checkpoint.ipynb
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    74057 2016-01-10 22:24:34.000000 lifelines-0.9.3.2/lifelines/datasets/.ipynb_checkpoints/The Gehan Survival Data-checkpoint.ipynb
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9983 2016-10-28 23:49:45.000000 lifelines-0.9.3.2/lifelines/datasets/__init__.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      580 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/anderson.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   163046 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/canadian_senators.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1996 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/CuZn-LeftCensoredDataset.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   267897 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/dd.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   198949 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/divorce.dat
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      580 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/g3.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      276 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/gehan.dat
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      180 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/holly_molly_polly.tsv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    13399 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/kidney_transplant.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1395 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/larynx.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9041 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/lung.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      306 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/panel_test.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      269 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/psychiatric_patients.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    24079 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/recur.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9746 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/regression.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     8693 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/rossi.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      100 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/static_test.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     2449 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/lifelines/datasets/waltons_dataset.csv
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      549 2016-05-23 18:42:02.000000 lifelines-0.9.3.2/lifelines/estimation.py
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/lifelines/fitters/
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     4076 2016-05-23 19:36:43.000000 lifelines-0.9.3.2/lifelines/fitters/__init__.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    19074 2016-05-23 19:36:43.000000 lifelines-0.9.3.2/lifelines/fitters/aalen_additive_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     3229 2016-05-23 18:42:04.000000 lifelines-0.9.3.2/lifelines/fitters/breslow_fleming_harrington_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    20136 2016-05-23 19:36:43.000000 lifelines-0.9.3.2/lifelines/fitters/coxph_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     5517 2016-05-23 19:36:43.000000 lifelines-0.9.3.2/lifelines/fitters/exponential_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     5211 2016-10-28 23:56:14.000000 lifelines-0.9.3.2/lifelines/fitters/kaplan_meier_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     7115 2016-05-23 18:42:05.000000 lifelines-0.9.3.2/lifelines/fitters/nelson_aalen_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9757 2016-05-23 19:36:43.000000 lifelines-0.9.3.2/lifelines/fitters/weibull_fitter.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9065 2016-05-23 19:36:43.000000 lifelines-0.9.3.2/lifelines/generate_datasets.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    13344 2016-11-08 18:04:54.000000 lifelines-0.9.3.2/lifelines/plotting.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    11965 2016-10-29 00:06:23.000000 lifelines-0.9.3.2/lifelines/statistics.py
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/lifelines/utils/
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    35215 2016-10-29 00:12:07.000000 lifelines-0.9.3.2/lifelines/utils/__init__.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     2313 2016-05-23 18:42:06.000000 lifelines-0.9.3.2/lifelines/utils/progress_bar.py
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       65 2016-11-08 18:04:54.000000 lifelines-0.9.3.2/lifelines/version.py
-drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/lifelines.egg-info/
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)        1 2016-11-08 18:21:17.000000 lifelines-0.9.3.2/lifelines.egg-info/dependency_links.txt
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       47 2016-11-08 14:14:26.000000 lifelines-0.9.3.2/lifelines.egg-info/pbr.json
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     4773 2016-11-08 18:21:17.000000 lifelines-0.9.3.2/lifelines.egg-info/PKG-INFO
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       25 2016-11-08 18:21:17.000000 lifelines-0.9.3.2/lifelines.egg-info/requires.txt
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1730 2016-11-08 18:21:17.000000 lifelines-0.9.3.2/lifelines.egg-info/SOURCES.txt
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       10 2016-11-08 18:21:17.000000 lifelines-0.9.3.2/lifelines.egg-info/top_level.txt
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      188 2014-02-12 03:26:48.000000 lifelines-0.9.3.2/MANIFEST.in
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     4773 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/PKG-INFO
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     3173 2016-05-22 19:02:21.000000 lifelines-0.9.3.2/README.md
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     3264 2016-02-15 03:03:34.000000 lifelines-0.9.3.2/README.txt
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      115 2016-11-08 18:21:18.000000 lifelines-0.9.3.2/setup.cfg
--rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1729 2016-08-05 02:59:31.000000 lifelines-0.9.3.2/setup.py
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1170 2014-02-12 03:26:48.000000 lifelines-0.9.4/LICENSE
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/lifelines/
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    12292 2015-01-03 00:46:11.000000 lifelines-0.9.4/lifelines/.DS_Store
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      444 2016-05-23 18:42:02.000000 lifelines-0.9.4/lifelines/__init__.py
+-rwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)    32160 2014-05-31 18:23:45.000000 lifelines-0.9.4/lifelines/_statistics.so
+-rwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)    32796 2014-12-13 14:04:01.000000 lifelines-0.9.4/lifelines/_utils.so
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/lifelines/datasets/
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/lifelines/datasets/.ipynb_checkpoints/
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   125625 2016-01-10 22:18:30.000000 lifelines-0.9.4/lifelines/datasets/.ipynb_checkpoints/Divorces Rates-checkpoint.ipynb
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    74057 2016-01-10 22:24:34.000000 lifelines-0.9.4/lifelines/datasets/.ipynb_checkpoints/The Gehan Survival Data-checkpoint.ipynb
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    10138 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/datasets/__init__.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      580 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/anderson.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   163046 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/canadian_senators.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1996 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/CuZn-LeftCensoredDataset.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   267897 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/dd.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   198949 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/divorce.dat
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      580 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/g3.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      276 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/gehan.dat
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      180 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/holly_molly_polly.tsv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    13399 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/kidney_transplant.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1395 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/larynx.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9041 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/lung.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      306 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/panel_test.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      269 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/psychiatric_patients.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    24079 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/recur.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9746 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/regression.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     8693 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/rossi.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      100 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/static_test.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     2449 2016-02-15 03:03:34.000000 lifelines-0.9.4/lifelines/datasets/waltons_dataset.csv
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      549 2016-05-23 18:42:02.000000 lifelines-0.9.4/lifelines/estimation.py
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/lifelines/fitters/
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     4076 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/fitters/__init__.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    19074 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/fitters/aalen_additive_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     3229 2016-05-23 18:42:04.000000 lifelines-0.9.4/lifelines/fitters/breslow_fleming_harrington_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    21330 2016-12-31 19:54:28.000000 lifelines-0.9.4/lifelines/fitters/coxph_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     5517 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/fitters/exponential_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     5302 2016-12-31 03:24:29.000000 lifelines-0.9.4/lifelines/fitters/kaplan_meier_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     7115 2016-05-23 18:42:05.000000 lifelines-0.9.4/lifelines/fitters/nelson_aalen_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9757 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/fitters/weibull_fitter.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     9065 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/generate_datasets.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    14649 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/plotting.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    11965 2016-12-28 22:51:56.000000 lifelines-0.9.4/lifelines/statistics.py
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/lifelines/utils/
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)    35214 2016-12-31 04:37:46.000000 lifelines-0.9.4/lifelines/utils/__init__.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     2313 2016-05-23 18:42:06.000000 lifelines-0.9.4/lifelines/utils/progress_bar.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       63 2017-01-01 18:32:41.000000 lifelines-0.9.4/lifelines/version.py
+drwxr-xr-x   0 camerondavidson-pilon   (501) staff       (20)        0 2017-01-01 18:48:06.000000 lifelines-0.9.4/lifelines.egg-info/
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)        1 2017-01-01 18:48:05.000000 lifelines-0.9.4/lifelines.egg-info/dependency_links.txt
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       47 2016-11-08 14:14:26.000000 lifelines-0.9.4/lifelines.egg-info/pbr.json
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     4771 2017-01-01 18:48:05.000000 lifelines-0.9.4/lifelines.egg-info/PKG-INFO
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       25 2017-01-01 18:48:05.000000 lifelines-0.9.4/lifelines.egg-info/requires.txt
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1765 2017-01-01 18:48:05.000000 lifelines-0.9.4/lifelines.egg-info/SOURCES.txt
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)       10 2017-01-01 18:48:05.000000 lifelines-0.9.4/lifelines.egg-info/top_level.txt
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      188 2014-02-12 03:26:48.000000 lifelines-0.9.4/MANIFEST.in
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     4771 2017-01-01 18:48:06.000000 lifelines-0.9.4/PKG-INFO
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     3173 2016-12-28 22:51:56.000000 lifelines-0.9.4/README.md
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     3264 2016-02-15 03:03:34.000000 lifelines-0.9.4/README.txt
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)      115 2017-01-01 18:48:06.000000 lifelines-0.9.4/setup.cfg
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)     1729 2016-12-28 22:51:56.000000 lifelines-0.9.4/setup.py
+-rw-r--r--   0 camerondavidson-pilon   (501) staff       (20)   198701 2016-12-10 02:44:29.000000 lifelines-0.9.4/test of the new loglogs plot.ipynb
```

### Comparing `lifelines-0.9.3.2/LICENSE` & `lifelines-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/.DS_Store` & `lifelines-0.9.4/lifelines/.DS_Store`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/_statistics.so` & `lifelines-0.9.4/lifelines/_statistics.so`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/_utils.so` & `lifelines-0.9.4/lifelines/_utils.so`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/.ipynb_checkpoints/Divorces Rates-checkpoint.ipynb` & `lifelines-0.9.4/lifelines/datasets/.ipynb_checkpoints/Divorces Rates-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/.ipynb_checkpoints/The Gehan Survival Data-checkpoint.ipynb` & `lifelines-0.9.4/lifelines/datasets/.ipynb_checkpoints/The Gehan Survival Data-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/__init__.py` & `lifelines-0.9.4/lifelines/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,20 @@
 
 
 def load_holly_molly_polly(**kwargs):
     """
     From https://stat.ethz.ch/education/semesters/ss2011/seminar/contents/presentation_10.pdf
     Used as a toy example for CoxPH in recurrent SA.
 
-     ID Status Stratum Start(days) Stop(days) tx T
-     M 1 1 0 100 1 100
-     M 1 2 100 105 1 5
-     H 1 1 0 30 0 30
-     H 1 2 30 50 0 20
-     P 1 1 0 20 0 20
-     P 1 2 20 60 0 40
-     P 1 3 60 85 0 25
+      ID  Status  Stratum  Start(days)  Stop(days)  tx    T
+    0  M       1        1            0         100   1  100
+    1  M       1        2          100         105   1    5
+    2  H       1        1            0          30   0   30
+    3  H       1        2           30          50   0   20
+    4  P       1        1            0          20   0   20
 
     """
     return load_dataset('holly_molly_polly.tsv', sep="\s", **kwargs)
 
 
 def load_leukemia(**kwargs):
     """
```

### Comparing `lifelines-0.9.3.2/lifelines/datasets/anderson.csv` & `lifelines-0.9.4/lifelines/datasets/anderson.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/canadian_senators.csv` & `lifelines-0.9.4/lifelines/datasets/canadian_senators.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/CuZn-LeftCensoredDataset.csv` & `lifelines-0.9.4/lifelines/datasets/CuZn-LeftCensoredDataset.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/dd.csv` & `lifelines-0.9.4/lifelines/datasets/dd.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/divorce.dat` & `lifelines-0.9.4/lifelines/datasets/divorce.dat`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/g3.csv` & `lifelines-0.9.4/lifelines/datasets/g3.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/kidney_transplant.csv` & `lifelines-0.9.4/lifelines/datasets/kidney_transplant.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/larynx.csv` & `lifelines-0.9.4/lifelines/datasets/larynx.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/lung.csv` & `lifelines-0.9.4/lifelines/datasets/lung.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/recur.csv` & `lifelines-0.9.4/lifelines/datasets/recur.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/regression.csv` & `lifelines-0.9.4/lifelines/datasets/regression.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/rossi.csv` & `lifelines-0.9.4/lifelines/datasets/rossi.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/datasets/waltons_dataset.csv` & `lifelines-0.9.4/lifelines/datasets/waltons_dataset.csv`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/estimation.py` & `lifelines-0.9.4/lifelines/estimation.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/fitters/__init__.py` & `lifelines-0.9.4/lifelines/fitters/__init__.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/fitters/aalen_additive_fitter.py` & `lifelines-0.9.4/lifelines/fitters/aalen_additive_fitter.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/fitters/breslow_fleming_harrington_fitter.py` & `lifelines-0.9.4/lifelines/fitters/breslow_fleming_harrington_fitter.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/fitters/coxph_fitter.py` & `lifelines-0.9.4/lifelines/fitters/coxph_fitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function
+import warnings
 import numpy as np
 import pandas as pd
 
 from numpy import dot, exp
 from numpy.linalg import solve, norm, inv
 from scipy.integrate import trapz
 import scipy.stats as stats
@@ -28,27 +29,27 @@
         in the input data before performing any fitting.
       penalizer: Attach a L2 penalizer to the size of the coeffcients during regression. This improves
         stability of the estimates and controls for high correlation between covariates.
         For example, this shrinks the absolute value of beta_i. Recommended, even if a small value.
         The penalty is 1/2 * penalizer * ||beta||^2.
     """
 
-    def __init__(self, alpha=0.95, tie_method='Efron', normalize=True, penalizer=0.0):
+    def __init__(self, alpha=0.95, tie_method='Efron', normalize=True, penalizer=0.0, strata=None):
         if not (0 < alpha <= 1.):
             raise ValueError('alpha parameter must be between 0 and 1.')
         if penalizer < 0:
             raise ValueError("penalizer parameter must be >= 0.")
         if tie_method != 'Efron':
             raise NotImplementedError("Only Efron is available atm.")
 
         self.alpha = alpha
         self.normalize = normalize
         self.tie_method = tie_method
         self.penalizer = penalizer
-        self.strata = None
+        self.strata = strata
 
     def _get_efron_values(self, X, beta, T, E, include_likelihood=False):
         """
         Calculates the first and second order vector differentials,
         with respect to beta. If 'include_likelihood' is True, then
         the log likelihood is also calculated. This is omitted by default
         to speed up the fit.
@@ -84,15 +85,15 @@
         # Iterate backwards to utilize recursive relationship
         for i, (ti, ei) in reversed(list(enumerate(zip(T, E)))):
             # Doing it like this to preserve shape
             xi = X[i:i + 1]
             # Calculate phi values
             phi_i = exp(dot(xi, beta))
             phi_x_i = dot(phi_i, xi)
-            phi_x_x_i = dot(xi.T, xi) * phi_i
+            phi_x_x_i = dot(xi.T, phi_i * xi)
 
             # Calculate sums of Risk set
             risk_phi += phi_i
             risk_phi_x += phi_x_i
             risk_phi_x_x += phi_x_x_i
             # Calculate sums of Ties, if this is an event
             if ei:
@@ -116,18 +117,14 @@
 
             for l in range(tie_count):
                 c = l / tie_count
 
                 denom = (risk_phi - c * tie_phi)
                 z = (risk_phi_x - c * tie_phi_x)
 
-                if denom == 0:
-                    # Can't divide by zero
-                    raise ValueError("Denominator was zero")
-
                 # Gradient
                 partial_gradient += z / denom
                 # Hessian
                 a1 = (risk_phi_x_x - c * tie_phi_x_x) / denom
                 # In case z and denom both are really small numbers,
                 # make sure to do division before multiplications
                 a2 = dot(z.T / denom, z / denom)
@@ -296,46 +293,48 @@
             E = pd.Series(np.ones(df.shape[0]), index=df.index)
         else:
             E = df[event_col]
             del df[event_col]
 
         # Store original non-normalized data
         self.data = df if self.strata is None else df.reset_index()
+        self._check_values(df)
 
         if self.normalize:
             # Need to normalize future inputs as well
             self._norm_mean = df.mean(0)
             self._norm_std = df.std(0)
             df = normalize(df)
 
         E = E.astype(bool)
-        self._check_values(df)
 
         hazards_ = self._newton_rhaphson(df, T, E, initial_beta=initial_beta,
                                          show_progress=show_progress,
                                          include_likelihood=include_likelihood)
 
         self.hazards_ = pd.DataFrame(hazards_.T, columns=df.columns,
                                      index=['coef'])
         self.confidence_intervals_ = self._compute_confidence_intervals()
 
         self.durations = T
         self.event_observed = E
 
-        self.baseline_hazard_ = self._compute_baseline_hazard()
+        self.baseline_hazard_ = self._compute_baseline_hazards(df, T, E)
         self.baseline_cumulative_hazard_ = self.baseline_hazard_.cumsum()
         self.baseline_survival_ = exp(-self.baseline_cumulative_hazard_)
         return self
 
     def _check_values(self, X):
         low_var = (X.var(0) < 10e-5)
         if low_var.any():
             cols = str(list(X.columns[low_var]))
-            print("Warning: column(s) %s have very low variance.\
- This may harm convergence." % cols)
+            warning_text = "Column(s) %s have very low variance.\
+ This may harm convergence. Try dropping this redundant column before fitting\
+ if convergence fails." % cols
+            warnings.warn(warning_text, RuntimeWarning)
 
     def _compute_confidence_intervals(self):
         alpha2 = inv_normal_cdf((1. + self.alpha) / 2.)
         se = self._compute_standard_errors()
         hazards = self.hazards_.values
         return pd.DataFrame(np.r_[hazards - alpha2 * se,
                                   hazards + alpha2 * se],
@@ -440,21 +439,29 @@
         return np.log(self.predict_partial_hazard(X) / self.predict_partial_hazard(mean_covariates).squeeze())
 
     def predict_cumulative_hazard(self, X):
         """
         X: a (n,d) covariate numpy array or DataFrame. If a DataFrame, columns
             can be in any order. If a numpy array, columns must be in the
             same order as the training data.
-
-        Returns the cumulative hazard for the individuals.
         """
-        v = self.predict_partial_hazard(X)
-        s_0 = self.baseline_survival_
-        col = _get_index(X)
-        return pd.DataFrame(-np.dot(np.log(s_0), v.T), index=self.baseline_survival_.index, columns=col)
+        if self.strata:
+            cumulative_hazard_ = pd.DataFrame()
+            for stratum, stratified_X in X.groupby(self.strata):
+                s_0 = self.baseline_survival_[[stratum]]
+                col = _get_index(stratified_X)
+                v = self.predict_partial_hazard(stratified_X)
+                cumulative_hazard_ = cumulative_hazard_.merge(pd.DataFrame(-np.dot(np.log(s_0), v.T), index=s_0.index, columns=col), how='outer', right_index=True, left_index=True)
+        else:
+            s_0 = self.baseline_survival_
+            col = _get_index(X)
+            v = self.predict_partial_hazard(X)
+            cumulative_hazard_ = pd.DataFrame(-np.dot(np.log(s_0), v.T), columns=col, index=s_0.index)
+
+        return cumulative_hazard_
 
     def predict_survival_function(self, X):
         """
         X: a (n,d) covariate numpy array or DataFrame. If a DataFrame, columns
             can be in any order. If a numpy array, columns must be in the
             same order as the training data.
 
@@ -492,27 +499,32 @@
 
         Compute the expected lifetime, E[T], using covarites X.
         """
         index = _get_index(X)
         v = self.predict_survival_function(X)[index]
         return pd.DataFrame(trapz(v.values.T, v.index), index=index)
 
-    def _compute_baseline_hazard(self):
+    def _compute_baseline_hazard(self, data, durations, event_observed, name):
         # http://courses.nus.edu.sg/course/stacar/internet/st3242/handouts/notes3.pdf
-        ind_hazards = self.predict_partial_hazard(self.data).values
-
-        event_table = survival_table_from_events(self.durations.values,
-                                                 self.event_observed.values)
+        ind_hazards = self.predict_partial_hazard(data)
+        ind_hazards['event_at'] = durations
+        ind_hazards_summed_over_durations = ind_hazards.groupby('event_at')[0].sum().sort_index(ascending=False).cumsum()
+        ind_hazards_summed_over_durations.name = 'hazards'
+
+        event_table = survival_table_from_events(durations, event_observed)
+        event_table = event_table.join(ind_hazards_summed_over_durations)
+        baseline_hazard = pd.DataFrame(event_table['observed'] / event_table['hazards'], columns=[name]).fillna(0)
+        return baseline_hazard
+
+    def _compute_baseline_hazards(self, df, T, E):
+        if self.strata:
+            baseline_hazards_ = pd.DataFrame(index=self.durations.unique())
+            for stratum in df.index.unique():
+                baseline_hazards_ = baseline_hazards_.merge(
+                                                 self._compute_baseline_hazard(data=df.ix[[stratum]], durations=T.ix[[stratum]], event_observed=E.ix[[stratum]], name=stratum),
+                                                 left_index=True,
+                                                 right_index=True,
+                                                 how='left')
+            return baseline_hazards_.fillna(0)
 
-        baseline_hazard_ = pd.DataFrame(np.zeros((event_table.shape[0], 1)),
-                                        index=event_table.index,
-                                        columns=['baseline hazard'])
-
-        for t, s in event_table.iterrows():
-            less = np.array(self.durations >= t)
-            if ind_hazards[less].sum() == 0:
-                v = 0
-            else:
-                v = (s['observed'] / ind_hazards[less].sum())
-            baseline_hazard_.ix[t] = v
-
-        return baseline_hazard_
+        else:
+            return self._compute_baseline_hazard(data=df, durations=T, event_observed=E, name='baseline hazard')
```

### Comparing `lifelines-0.9.3.2/lifelines/fitters/exponential_fitter.py` & `lifelines-0.9.4/lifelines/fitters/exponential_fitter.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/fitters/kaplan_meier_fitter.py` & `lifelines-0.9.4/lifelines/fitters/kaplan_meier_fitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import print_function
 import numpy as np
 import pandas as pd
 
 from lifelines.fitters import UnivariateFitter
 from lifelines.utils import _preprocess_inputs, _additive_estimate, StatError, inv_normal_cdf,\
     median_survival_times
+from lifelines.plotting import plot_loglogs
 
 
 class KaplanMeierFitter(UnivariateFitter):
 
     """
     Class for fitting the Kaplan-Meier estimate for the survival function.
 
@@ -72,14 +73,15 @@
         self.predict = self._predict(estimate_name, label)
         self.subtract = self._subtract(estimate_name)
         self.divide = self._divide(estimate_name)
 
         # plotting functions
         self.plot = self._plot_estimate(estimate_name)
         setattr(self, "plot_" + estimate_name, self.plot)
+        self.plot_loglogs = plot_loglogs(self)
         return self
 
     def _bounds(self, cumulative_sq_, alpha, ci_labels):
         # See http://courses.nus.edu.sg/course/stacar/internet/st3242/handouts/notes2.pdf
         alpha2 = inv_normal_cdf((1. + alpha) / 2.)
         df = pd.DataFrame(index=self.timeline)
         v = np.log(self.__estimate.values)
```

### Comparing `lifelines-0.9.3.2/lifelines/fitters/nelson_aalen_fitter.py` & `lifelines-0.9.4/lifelines/fitters/nelson_aalen_fitter.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/fitters/weibull_fitter.py` & `lifelines-0.9.4/lifelines/fitters/weibull_fitter.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/generate_datasets.py` & `lifelines-0.9.4/lifelines/generate_datasets.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/plotting.py` & `lifelines-0.9.4/lifelines/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     ax2.xaxis.set_label_coords(0, ax2_ypos)
     ax2.set_xlabel('At risk')
 
     plt.tight_layout()
     return ax
 
 
+
 def plot_lifetimes(lifetimes, event_observed=None, birthtimes=None,
                    order=False, block=True):
     """
     Parameters:
       lifetimes: an (n,) numpy array of lifetimes.
       event_observed: an (n,) numpy array of booleans: True if event observed, else False.
       birthtimes: an (n,) numpy array offsetting the births away from t=0.
@@ -238,23 +239,70 @@
     user_did_not_specify_certain_indexes = (iloc is None) and (ix is None)
     user_submitted_slice = slice(None) if user_did_not_specify_certain_indexes else coalesce(ix, iloc)
 
     get_method = "ix" if ix is not None else "iloc"
     return lambda df: getattr(df, get_method)[user_submitted_slice]
 
 
+def plot_loglogs(cls):
+    doc_string = """
+    Specifies a plot of the log(-log(SV)) versus log(time) where SV is the estimated survival function.
+    """
+
+    def _plot_loglogs(ix=None, iloc=None, show_censors=False, censor_styles=None, **kwargs):
+
+        loglog = lambda s: np.log(-np.log(s))
+
+        if (ix is not None) and (iloc is not None):
+            raise ValueError('Cannot set both ix and iloc in call to .plot().')
+
+        if censor_styles is None:
+            censor_styles = {}
+
+        set_kwargs_ax(kwargs)
+        set_kwargs_color(kwargs)
+        set_kwargs_drawstyle(kwargs)
+        kwargs['logx'] = True
+
+        dataframe_slicer = create_dataframe_slicer(iloc, ix)
+
+        # plot censors
+        ax = kwargs['ax']
+        colour = kwargs['color']
+
+        if show_censors and cls.event_table['censored'].sum() > 0:
+            cs = {
+                'marker': '+',
+                'ms': 12,
+                'mew': 1
+            }
+            cs.update(censor_styles)
+            times = dataframe_slicer(cls.event_table.ix[(cls.event_table['censored'] > 0)]).index.values.astype(float)
+            v = cls.predict(times)
+            # don't log times, as Pandas will take care of all log-scaling later.
+            ax.plot(times, loglog(v), linestyle='None',
+                    color=colour, **cs)
+
+        # plot estimate
+        dataframe_slicer(loglog(cls.survival_function_)).plot(**kwargs)
+        ax.set_xlabel('log(timeline)')
+        ax.set_ylabel('log(-log(survival_function_))')
+        return ax
+
+    _plot_loglogs.__doc__ = doc_string
+    return _plot_loglogs
+
+
 def plot_estimate(cls, estimate):
     doc_string = """"
         Plots a pretty version of the fitted %s.
 
         Matplotlib plot arguments can be passed in inside the kwargs, plus
 
         Parameters:
-          flat: an opiniated design style with stepped lines and no shading.
-                Similar to R's plotting. Default: False
           show_censors: place markers at censorship events. Default: False
           censor_styles: If show_censors, this dictionary will be passed into
                          the plot call.
           ci_alpha: the transparency level of the confidence interval.
                     Default: 0.3
           ci_force_lines: force the confidence intervals to be line plots
                           (versus default shaded areas). Default: False
@@ -272,36 +320,29 @@
           bandwidth: specify the bandwidth of the kernel smoother for the
                      smoothed-hazard rate. Only used when called 'plot_hazard'.
 
         Returns:
           ax: a pyplot axis object
         """ % estimate
 
-    def plot(ix=None, iloc=None, flat=False, show_censors=False,
+    def plot(ix=None, iloc=None, show_censors=False,
              censor_styles=None, ci_legend=False, ci_force_lines=False,
              ci_alpha=0.25, ci_show=True, at_risk_counts=False,
              bandwidth=None, **kwargs):
 
-        from matplotlib import pyplot as plt
-
         if censor_styles is None:
             censor_styles = {}
 
         if (ix is not None) and (iloc is not None):
             raise ValueError('Cannot set both ix and iloc in call to .plot().')
 
         set_kwargs_ax(kwargs)
         set_kwargs_color(kwargs)
         set_kwargs_drawstyle(kwargs)
 
-        # R-style graphics
-        if flat:
-            ci_force_lines = True
-            show_censors = True
-
         if estimate == "hazard_":
             if bandwidth is None:
                 raise ValueError('Must specify a bandwidth parameter in the call to plot_hazard.')
             estimate_ = cls.smoothed_hazard_(bandwidth)
             confidence_interval_ = \
                 cls.smoothed_hazard_confidence_intervals_(bandwidth, hazard_=estimate_.values[:, 0])
         else:
@@ -329,25 +370,26 @@
         # plot estimate
         dataframe_slicer(estimate_).plot(**kwargs)
 
         # plot confidence intervals
         if ci_show:
             if ci_force_lines:
                 dataframe_slicer(confidence_interval_).plot(linestyle="-", linewidth=1,
-                                                            color=[colour], legend=True,
+                                                            color=[colour], legend=ci_legend,
                                                             drawstyle=kwargs.get('drawstyle', 'default'),
                                                             ax=ax, alpha=0.6)
             else:
                 x = dataframe_slicer(confidence_interval_).index.values.astype(float)
                 lower = dataframe_slicer(confidence_interval_.filter(like='lower')).values[:, 0]
                 upper = dataframe_slicer(confidence_interval_.filter(like='upper')).values[:, 0]
                 fill_between_steps(x, lower, y2=upper, ax=ax,
                                    alpha=ci_alpha, color=colour,
                                    linewidth=1.0)
 
+
         if at_risk_counts:
             add_at_risk_counts(cls, ax=ax)
 
         return ax
 
     plot.__doc__ = doc_string
     return plot
```

### Comparing `lifelines-0.9.3.2/lifelines/statistics.py` & `lifelines-0.9.4/lifelines/statistics.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines/utils/__init__.py` & `lifelines-0.9.4/lifelines/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,14 @@
     death_table = df.groupby("event_at").sum()
     death_table[censored] = (death_table[removed] - death_table[observed]).astype(int)
 
     # deal with late births
     births = pd.DataFrame(birth_times, columns=['event_at'])
     births[entrance] = 1
     births_table = births.groupby('event_at').sum()
-
     event_table = death_table.join(births_table, how='outer', sort=True).fillna(0)  # http://wesmckinney.com/blog/?p=414
     event_table[at_risk] = event_table[entrance].cumsum() - event_table[removed].cumsum().shift(1).fillna(0)
     return event_table.astype(int)
 
 
 def survival_events_from_table(event_table, observed_deaths_col="observed", censored_col="censored"):
     """
```

### Comparing `lifelines-0.9.3.2/lifelines/utils/progress_bar.py` & `lifelines-0.9.4/lifelines/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/lifelines.egg-info/PKG-INFO` & `lifelines-0.9.4/lifelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lifelines
-Version: 0.9.3.2
+Version: 0.9.4
 Summary: Survival analysis in Python, including Kaplan Meier, Nelson Aalen and regression
 Home-page: https://github.com/CamDavidsonPilon/lifelines
 Author: Cameron Davidson-Pilon, Jonas Kalderstam
 Author-email: cam.davidson.pilon@gmail.com
 License: MIT
 Description: lifelines
         =========
```

### Comparing `lifelines-0.9.3.2/lifelines.egg-info/SOURCES.txt` & `lifelines-0.9.4/lifelines.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 README.txt
 setup.cfg
 setup.py
+test of the new loglogs plot.ipynb
 lifelines/.DS_Store
 lifelines/__init__.py
 lifelines/_statistics.so
 lifelines/_utils.so
 lifelines/estimation.py
 lifelines/generate_datasets.py
 lifelines/plotting.py
```

### Comparing `lifelines-0.9.3.2/PKG-INFO` & `lifelines-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lifelines
-Version: 0.9.3.2
+Version: 0.9.4
 Summary: Survival analysis in Python, including Kaplan Meier, Nelson Aalen and regression
 Home-page: https://github.com/CamDavidsonPilon/lifelines
 Author: Cameron Davidson-Pilon, Jonas Kalderstam
 Author-email: cam.davidson.pilon@gmail.com
 License: MIT
 Description: lifelines
         =========
```

### Comparing `lifelines-0.9.3.2/README.md` & `lifelines-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/README.txt` & `lifelines-0.9.4/README.txt`

 * *Files identical despite different names*

### Comparing `lifelines-0.9.3.2/setup.py` & `lifelines-0.9.4/setup.py`

 * *Files identical despite different names*

