# Comparing `tmp/pyomicron-2.0.4.tar.gz` & `tmp/pyomicron-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyomicron-2.0.4.tar", last modified: Sun Oct 16 22:06:34 2022, max compression
+gzip compressed data, was "pyomicron-2.0.5.tar", last modified: Thu Apr 27 12:06:47 2023, max compression
```

## Comparing `pyomicron-2.0.4.tar` & `pyomicron-2.0.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.300503 pyomicron-2.0.4/
--rw-r--r--   0 areeda     (501) staff       (20)      183 2022-08-18 01:21:23.000000 pyomicron-2.0.4/.codecov.yml
--rw-r--r--   0 areeda     (501) staff       (20)       33 2022-05-22 22:48:23.000000 pyomicron-2.0.4/.gitattributes
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.259364 pyomicron-2.0.4/.github/
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.269150 pyomicron-2.0.4/.github/workflows/
--rw-r--r--   0 areeda     (501) staff       (20)     2683 2022-08-18 01:21:23.000000 pyomicron-2.0.4/.github/workflows/build.yml
--rw-r--r--   0 areeda     (501) staff       (20)     3512 2022-08-18 01:21:23.000000 pyomicron-2.0.4/.github/workflows/build.yml-codecov
--rw-r--r--   0 areeda     (501) staff       (20)     2683 2022-08-18 01:21:23.000000 pyomicron-2.0.4/.github/workflows/build.yml-nocodecov
--rw-r--r--   0 areeda     (501) staff       (20)      636 2022-05-22 22:48:23.000000 pyomicron-2.0.4/.github/workflows/lint.yml
--rw-r--r--   0 areeda     (501) staff       (20)      215 2022-05-22 22:48:23.000000 pyomicron-2.0.4/.gitignore
--rw-r--r--   0 areeda     (501) staff       (20)       72 2022-08-18 01:21:23.000000 pyomicron-2.0.4/.pep8speaks.yml
--rw-r--r--   0 areeda     (501) staff       (20)      386 2022-05-22 22:48:23.000000 pyomicron-2.0.4/.readthedocs.yml
--rw-r--r--   0 areeda     (501) staff       (20)    35147 2022-05-22 22:48:23.000000 pyomicron-2.0.4/LICENSE
--rw-r--r--   0 areeda     (501) staff       (20)       88 2022-05-22 22:48:23.000000 pyomicron-2.0.4/MANIFEST.in
--rw-r--r--   0 areeda     (501) staff       (20)     3244 2022-10-16 22:06:34.300694 pyomicron-2.0.4/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)     1800 2022-05-22 22:48:23.000000 pyomicron-2.0.4/README.md
--rw-r--r--   0 areeda     (501) staff       (20)      738 2022-08-18 01:21:23.000000 pyomicron-2.0.4/RELEASE.md
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.271336 pyomicron-2.0.4/docs/
--rw-r--r--   0 areeda     (501) staff       (20)      660 2022-08-18 01:21:23.000000 pyomicron-2.0.4/docs/Makefile
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.271601 pyomicron-2.0.4/docs/_static/
--rw-r--r--   0 areeda     (501) staff       (20)     1095 2022-08-18 01:21:23.000000 pyomicron-2.0.4/docs/_static/omicron-GW.dot
--rw-r--r--   0 areeda     (501) staff       (20)     9990 2022-08-18 01:21:23.000000 pyomicron-2.0.4/docs/conf.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.272556 pyomicron-2.0.4/docs/configuration/
--rw-r--r--   0 areeda     (501) staff       (20)     2819 2022-05-22 22:48:23.000000 pyomicron-2.0.4/docs/configuration/index.rst
--rw-r--r--   0 areeda     (501) staff       (20)      406 2022-05-22 22:48:23.000000 pyomicron-2.0.4/docs/environment.yml
--rw-r--r--   0 areeda     (501) staff       (20)     1405 2022-10-16 20:31:06.000000 pyomicron-2.0.4/docs/index.rst
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.275808 pyomicron-2.0.4/docs/utilities/
--rw-r--r--   0 areeda     (501) staff       (20)     3354 2022-08-18 01:21:23.000000 pyomicron-2.0.4/docs/utilities/merge.rst
--rw-r--r--   0 areeda     (501) staff       (20)     2019 2022-05-22 22:48:23.000000 pyomicron-2.0.4/docs/utilities/print.rst
--rw-r--r--   0 areeda     (501) staff       (20)      979 2022-08-18 01:21:23.000000 pyomicron-2.0.4/docs/utilities/status.rst
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.277763 pyomicron-2.0.4/docs/workflow/
--rw-r--r--   0 areeda     (501) staff       (20)     4970 2022-08-18 01:21:23.000000 pyomicron-2.0.4/docs/workflow/index.rst
--rw-r--r--   0 areeda     (501) staff       (20)     3799 2022-10-16 20:31:06.000000 pyomicron-2.0.4/docs/workflow/simulations.rst
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.285671 pyomicron-2.0.4/omicron/
--rw-r--r--   0 areeda     (501) staff       (20)      999 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)      176 2022-10-16 22:06:34.000000 pyomicron-2.0.4/omicron/_version.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.289366 pyomicron-2.0.4/omicron/cli/
--rw-r--r--   0 areeda     (501) staff       (20)      927 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/cli/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)     6928 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/cli/archive.py
--rw-r--r--   0 areeda     (501) staff       (20)     2044 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/cli/hdf5_merge.py
--rw-r--r--   0 areeda     (501) staff       (20)    11724 2022-10-16 20:31:06.000000 pyomicron-2.0.4/omicron/cli/merge_with_gaps.py
--rw-r--r--   0 areeda     (501) staff       (20)    52310 2022-10-16 20:31:06.000000 pyomicron-2.0.4/omicron/cli/process.py
--rw-r--r--   0 areeda     (501) staff       (20)     2297 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/cli/root_merge.py
--rw-r--r--   0 areeda     (501) staff       (20)     8100 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/cli/show.py
--rw-r--r--   0 areeda     (501) staff       (20)    29960 2022-10-16 20:31:06.000000 pyomicron-2.0.4/omicron/cli/status.py
--rw-r--r--   0 areeda     (501) staff       (20)    18602 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/condor.py
--rw-r--r--   0 areeda     (501) staff       (20)     2055 2022-10-16 20:31:06.000000 pyomicron-2.0.4/omicron/const.py
--rw-r--r--   0 areeda     (501) staff       (20)    10455 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/data.py
--rw-r--r--   0 areeda     (501) staff       (20)     9817 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/io.py
--rw-r--r--   0 areeda     (501) staff       (20)     4013 2022-10-16 20:31:06.000000 pyomicron-2.0.4/omicron/log.py
--rw-r--r--   0 areeda     (501) staff       (20)     6441 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/nagios.py
--rw-r--r--   0 areeda     (501) staff       (20)    16316 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/parameters.py
--rw-r--r--   0 areeda     (501) staff       (20)     9466 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/segments.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.296314 pyomicron-2.0.4/omicron/tests/
--rw-r--r--   0 areeda     (501) staff       (20)      810 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)      119 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/mock_classad.py
--rw-r--r--   0 areeda     (501) staff       (20)      763 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/mock_htcondor.py
--rw-r--r--   0 areeda     (501) staff       (20)     4158 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/test_condor.py
--rw-r--r--   0 areeda     (501) staff       (20)     1336 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/test_const.py
--rw-r--r--   0 areeda     (501) staff       (20)     1278 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/tests/test_io.py
--rw-r--r--   0 areeda     (501) staff       (20)     1436 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/tests/test_log.py
--rw-r--r--   0 areeda     (501) staff       (20)      969 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/test_nagios.py
--rw-r--r--   0 areeda     (501) staff       (20)     6582 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/tests/test_parameters.py
--rw-r--r--   0 areeda     (501) staff       (20)     2515 2022-08-18 01:21:23.000000 pyomicron-2.0.4/omicron/tests/test_segments.py
--rw-r--r--   0 areeda     (501) staff       (20)     2638 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/test_utils.py
--rw-r--r--   0 areeda     (501) staff       (20)     1101 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/tests/utils.py
--rw-r--r--   0 areeda     (501) staff       (20)     3357 2022-05-22 22:48:23.000000 pyomicron-2.0.4/omicron/utils.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.298958 pyomicron-2.0.4/pyomicron.egg-info/
--rw-r--r--   0 areeda     (501) staff       (20)     3244 2022-10-16 22:06:34.000000 pyomicron-2.0.4/pyomicron.egg-info/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)     1494 2022-10-16 22:06:34.000000 pyomicron-2.0.4/pyomicron.egg-info/SOURCES.txt
--rw-r--r--   0 areeda     (501) staff       (20)        1 2022-10-16 22:06:34.000000 pyomicron-2.0.4/pyomicron.egg-info/dependency_links.txt
--rw-r--r--   0 areeda     (501) staff       (20)      339 2022-10-16 22:06:34.000000 pyomicron-2.0.4/pyomicron.egg-info/entry_points.txt
--rw-r--r--   0 areeda     (501) staff       (20)      301 2022-10-16 22:06:34.000000 pyomicron-2.0.4/pyomicron.egg-info/requires.txt
--rw-r--r--   0 areeda     (501) staff       (20)        8 2022-10-16 22:06:34.000000 pyomicron-2.0.4/pyomicron.egg-info/top_level.txt
--rw-r--r--   0 areeda     (501) staff       (20)      238 2022-05-22 22:48:23.000000 pyomicron-2.0.4/pyproject.toml
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-10-16 22:06:34.300026 pyomicron-2.0.4/scripts/
--rwxr-xr-x   0 areeda     (501) staff       (20)      373 2022-08-18 01:21:23.000000 pyomicron-2.0.4/scripts/flist-check.sh
--rwxr-xr-x   0 areeda     (501) staff       (20)      161 2022-08-18 01:21:23.000000 pyomicron-2.0.4/scripts/xml-uint-fix.sh
--rw-r--r--   0 areeda     (501) staff       (20)     2398 2022-10-16 22:06:34.301502 pyomicron-2.0.4/setup.cfg
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.274414 pyomicron-2.0.5/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      183 2022-09-18 10:35:21.000000 pyomicron-2.0.5/.codecov.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       33 2020-08-05 08:24:16.000000 pyomicron-2.0.5/.gitattributes
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.194414 pyomicron-2.0.5/.github/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.254414 pyomicron-2.0.5/.github/workflows/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2683 2022-09-18 10:35:21.000000 pyomicron-2.0.5/.github/workflows/build.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3512 2022-09-18 10:35:21.000000 pyomicron-2.0.5/.github/workflows/build.yml-codecov
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2683 2022-09-18 10:35:21.000000 pyomicron-2.0.5/.github/workflows/build.yml-nocodecov
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      636 2022-02-01 18:30:32.000000 pyomicron-2.0.5/.github/workflows/lint.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      215 2022-09-18 10:35:21.000000 pyomicron-2.0.5/.gitignore
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       72 2022-09-18 10:35:21.000000 pyomicron-2.0.5/.pep8speaks.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      386 2022-02-01 18:30:32.000000 pyomicron-2.0.5/.readthedocs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2020-08-05 08:24:16.000000 pyomicron-2.0.5/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       88 2022-01-13 14:37:22.000000 pyomicron-2.0.5/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3244 2023-04-27 12:06:47.274414 pyomicron-2.0.5/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2022-09-18 10:35:21.000000 pyomicron-2.0.5/README.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      738 2022-09-18 10:35:21.000000 pyomicron-2.0.5/RELEASE.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.254414 pyomicron-2.0.5/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      660 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/Makefile
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.254414 pyomicron-2.0.5/docs/_static/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1095 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/_static/omicron-GW.dot
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9990 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/conf.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.254414 pyomicron-2.0.5/docs/configuration/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2819 2020-08-05 08:24:16.000000 pyomicron-2.0.5/docs/configuration/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      406 2022-02-01 18:30:32.000000 pyomicron-2.0.5/docs/environment.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1405 2023-04-10 13:36:49.000000 pyomicron-2.0.5/docs/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.254414 pyomicron-2.0.5/docs/utilities/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3354 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/utilities/merge.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2019 2020-08-05 08:24:16.000000 pyomicron-2.0.5/docs/utilities/print.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      979 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/utilities/status.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.254414 pyomicron-2.0.5/docs/workflow/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4970 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/workflow/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3799 2022-09-18 10:35:21.000000 pyomicron-2.0.5/docs/workflow/simulations.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.264414 pyomicron-2.0.5/omicron/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      999 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-27 12:06:47.000000 pyomicron-2.0.5/omicron/_version.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.264414 pyomicron-2.0.5/omicron/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      927 2022-01-13 14:37:22.000000 pyomicron-2.0.5/omicron/cli/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6934 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/cli/archive.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2039 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/cli/hdf5_merge.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12531 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/cli/merge_with_gaps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52715 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/cli/process.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2292 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/cli/root_merge.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8095 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/cli/show.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30331 2023-04-27 12:04:09.000000 pyomicron-2.0.5/omicron/cli/status.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18602 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/condor.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2055 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/const.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10575 2023-04-21 13:23:26.000000 pyomicron-2.0.5/omicron/data.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9817 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/io.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4013 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6441 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/nagios.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16316 2023-04-21 13:23:23.000000 pyomicron-2.0.5/omicron/parameters.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9466 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.274414 pyomicron-2.0.5/omicron/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      810 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      119 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/tests/mock_classad.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      763 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/tests/mock_htcondor.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4158 2022-01-13 14:37:22.000000 pyomicron-2.0.5/omicron/tests/test_condor.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1336 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/tests/test_const.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1278 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/tests/test_io.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1436 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/tests/test_log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      969 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/tests/test_nagios.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6582 2022-09-18 10:35:21.000000 pyomicron-2.0.5/omicron/tests/test_parameters.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2515 2022-09-18 10:35:18.000000 pyomicron-2.0.5/omicron/tests/test_segments.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2638 2022-01-13 14:37:22.000000 pyomicron-2.0.5/omicron/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1101 2020-08-05 08:24:16.000000 pyomicron-2.0.5/omicron/tests/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2023-04-10 13:36:49.000000 pyomicron-2.0.5/omicron/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.274414 pyomicron-2.0.5/pyomicron.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3244 2023-04-27 12:06:47.000000 pyomicron-2.0.5/pyomicron.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1494 2023-04-27 12:06:47.000000 pyomicron-2.0.5/pyomicron.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-27 12:06:47.000000 pyomicron-2.0.5/pyomicron.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      339 2023-04-27 12:06:47.000000 pyomicron-2.0.5/pyomicron.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      301 2023-04-27 12:06:47.000000 pyomicron-2.0.5/pyomicron.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        8 2023-04-27 12:06:47.000000 pyomicron-2.0.5/pyomicron.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      238 2022-09-18 10:35:21.000000 pyomicron-2.0.5/pyproject.toml
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-27 12:06:47.274414 pyomicron-2.0.5/scripts/
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      373 2022-09-18 10:35:21.000000 pyomicron-2.0.5/scripts/flist-check.sh
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      161 2022-09-18 10:35:21.000000 pyomicron-2.0.5/scripts/xml-uint-fix.sh
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2398 2023-04-27 12:06:47.274414 pyomicron-2.0.5/setup.cfg
```

### Comparing `pyomicron-2.0.4/.github/workflows/build.yml` & `pyomicron-2.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/.github/workflows/build.yml-codecov` & `pyomicron-2.0.5/.github/workflows/build.yml-codecov`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/.github/workflows/build.yml-nocodecov` & `pyomicron-2.0.5/.github/workflows/build.yml-nocodecov`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/.github/workflows/lint.yml` & `pyomicron-2.0.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/LICENSE` & `pyomicron-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/PKG-INFO` & `pyomicron-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyomicron
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python utilities and wrappers for GW Omicron
 Home-page: https://github.com/gwpy/pyomicron
 Download-URL: https://pypi.org/project/pyomicron/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 Maintainer: Joseph Areeda
 Maintainer-email: joseph.areeda@ligo.org
```

### Comparing `pyomicron-2.0.4/README.md` & `pyomicron-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/RELEASE.md` & `pyomicron-2.0.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/Makefile` & `pyomicron-2.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/_static/omicron-GW.dot` & `pyomicron-2.0.5/docs/_static/omicron-GW.dot`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/conf.py` & `pyomicron-2.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/configuration/index.rst` & `pyomicron-2.0.5/docs/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/index.rst` & `pyomicron-2.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/utilities/merge.rst` & `pyomicron-2.0.5/docs/utilities/merge.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/utilities/print.rst` & `pyomicron-2.0.5/docs/utilities/print.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/utilities/status.rst` & `pyomicron-2.0.5/docs/utilities/status.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/workflow/index.rst` & `pyomicron-2.0.5/docs/workflow/index.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/docs/workflow/simulations.rst` & `pyomicron-2.0.5/docs/workflow/simulations.rst`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/__init__.py` & `pyomicron-2.0.5/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/cli/__init__.py` & `pyomicron-2.0.5/omicron/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/cli/archive.py` & `pyomicron-2.0.5/omicron/cli/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,18 @@
 start_time = time.time()
 import argparse
 import glob
 import logging
 import os
 import re
 
+from .. import __version__
+
 __author__ = 'joseph areeda'
 __email__ = 'joseph.areeda@ligo.org'
-__version__ = '0.0.1'
 __process_name__ = 'archive'
 
 # example channel indir: L1:SUS-PR3_M1_DAMP_T_IN1_DQ
 chpat = re.compile(".*/?([A-Z][1-2]):(.+)$")
 # example trigger file: L1-SUS_PR3_M1_DAMP_T_IN1_DQ_OMICRON-1336799058-8064.h5
 tfpat = re.compile("([A-Z][0-9])-(.+)-(\\d+)-(\\d+)\\.(.*)$")
```

### Comparing `pyomicron-2.0.4/omicron/cli/hdf5_merge.py` & `pyomicron-2.0.5/omicron/cli/hdf5_merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 """Merge HDF5 files into one
 """
 
 import os.path
 import argparse
 
-from omicron import (io, __version__)
+from .. import (io, __version__)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 def create_parser():
     """Create a command-line parser for this entry point
     """
```

### Comparing `pyomicron-2.0.4/omicron/cli/merge_with_gaps.py` & `pyomicron-2.0.5/omicron/cli/merge_with_gaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 from logging.handlers import RotatingFileHandler
 
 from gwpy.table import EventTable
 
 prog_start_time = time.time()
 import argparse
 import glob
+import gzip
 import logging
+from .. import __version__
 from pathlib import Path
 import re
 import shutil
 import subprocess
 import sys
 
 __author__ = 'joseph areeda'
 __email__ = 'joseph.areeda@ligo.org'
-__version__ = '0.0.1'
 __process_name__ = 'omicron_merge_with_gaps'
 
 # global logger
-log_file_format = "%(asctime)s - %(levelname)s - %(funcName)s %(lineno)d: %(message)s"
+log_file_format = "%(asctime)s - %(levelname)s - %(funcName)s:%(lineno)d - %(message)s"
 log_file_date_format = '%m-%d %H:%M:%S'
 logging.basicConfig(format=log_file_format, datefmt=log_file_date_format)
 logger = logging.getLogger(__process_name__)
 logger.setLevel(logging.DEBUG)
 
 
 def get_merge_cmd(ext):
@@ -63,14 +64,30 @@
         raise AttributeError(f'Unknown trigger file typr {ext}')
     ret_path = shutil.which(ret)
     if not ret_path:
         raise AttributeError(f'{ext} files require {ret} which is not in out path')
     return ret_path
 
 
+def is_old_ligolw(path):
+    flag = "ilwd:char"
+    if 'gz' in path.name:
+        with gzip.open(str(path.absolute()), 'r') as gz:
+            for line in gz:
+                if flag in str(line):
+                    return True
+            return False
+    else:
+        with path.open('r') as fp:
+            for line in fp:
+                if flag in line:
+                    return True
+            return False
+
+
 def do_merge(opath, curfiles, chan, stime, etime, ext, skip_gzip):
     """
     Given the list of trigger files merge them all into a single file
     :param Path opath: output directory
     :param list curfiles: the pathes to files to merge
     :param str chan: channel name use in output filename
     :param int stime: Start GPS time for file list
@@ -90,14 +107,17 @@
                 logger.info(f'Copied singleton trigger file to {outfile_path}')
                 returncode = 0
         else:
             cmd = [get_merge_cmd(ext)]
             if 'xml' in ext:    # also accept xml.gz
                 outfile_path = Path(str(outfile_path.absolute()).replace('.xml.gz', '.xml'))
                 cmd.append(f'--output={outfile_path}')
+                if is_old_ligolw(curfiles[0]):
+                    cmd.append('--ilwdchar-compat')
+                    logger.debug('Working with old ligolw format')
             for cur in curfiles:
                 cmd.append(str(cur.absolute()))
             if 'xml' not in ext:
                 cmd.append(str(outfile_path.absolute()))
 
             logger.info(f'Merging {len(curfiles)} {ext} files into {outfile_path}')
             logger.debug(f'Merge command:\n {" ".join(cmd)}')
@@ -113,15 +133,15 @@
                 returncode = result.returncode
 
             if returncode == 0:
                 logger.debug(f'Merge of {ext} files succeeded')
             else:
                 logger.error(f'Return code:{returncode}, stderr:\n{result.stderr.decode("UTF-8")}')
 
-        if 'xml' in ext and returncode == 0 and not skip_gzip:
+        if 'xml' in ext and returncode == 0 and not skip_gzip and outfile_path.suffix != '.gz':
             logger.info(f'Compressing {outfile_path} with gzip')
             res2 = subprocess.run(['gzip', '-9', '--force', outfile_path], capture_output=True)
             if res2.returncode == 0:
                 ret = str(outfile_path.absolute()) + '.gz'
             else:
                 logger.error(f'gzip error on {outfile_path}:\n {res2.stderr.decode("UTF-8")}')
         else:
@@ -157,15 +177,15 @@
 
         ntrig = 0 if table is None else len(table)
         if table is None:
             logger.info(f'Invalid trigger file: {str(path.absolute())}')
             os.remove(path)
         else:
             ret = True
-        logger.debug(f'valid_file: {ret}  {path.name} ({ntrig}), {ret} took {time.time()-vf_strt:.2f}')
+        logger.debug(f'valid_file: {ret}  {path.name} ({ntrig}), took {time.time()-vf_strt:.2f}')
     return ret
 
 
 def main():
     global logger
 
     parser = argparse.ArgumentParser(description=__doc__,
@@ -204,14 +224,19 @@
         log_formatter = logging.Formatter(fmt=log_file_format,
                                           datefmt=log_file_date_format)
         log_file_handler = RotatingFileHandler(args.log_file, maxBytes=10 ** 7,
                                                backupCount=5)
         log_file_handler.setFormatter(log_formatter)
         logger.addHandler(log_file_handler)
 
+    # debugging?
+    logger.debug('{} called with arguments:'.format(__process_name__))
+    for k, v in args.__dict__.items():
+        logger.debug('    {} = {}'.format(k, v))
+
     fpat = '^(.+)-(\\d+)-(\\d+).(.+)$'
     fmatch = re.compile(fpat)
 
     infiles = list()
     for infile in args.infiles:
         files = glob.glob(infile)
         infiles.extend(files)
```

### Comparing `pyomicron-2.0.4/omicron/cli/process.py` & `pyomicron-2.0.5/omicron/cli/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,15 @@
 
 import gwpy.time
 from glue import pipeline
 
 from gwpy.io.cache import read_cache
 from gwpy.time import to_gps, tconvert
 
-from omicron import (const, segments, log, data, parameters, utils, condor, io,
-                     __version__)
+from .. import (const, segments, log, data, parameters, utils, condor, io, __version__)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 try:
     OMICRON_PATH = str(utils.find_omicron())
 except RuntimeError:
     OMICRON_PATH = None
@@ -461,15 +460,21 @@
     parser = create_parser()
     args = parser.parse_args(args=args)
 
     # apply verbosity to logger
     args.verbose = max(5 - args.verbose, 0)
     logger.setLevel(args.verbose * 10)
     if args.log_file:
-        logger.add_file_handler(args.log_file)
+        log_file = Path(args.log_file)
+    else:
+        # if not specified default to the output directory
+        log_file = Path(args.output_dir) / 'omicron-process.log'
+    log_file.parent.mkdir(mode=0o755, exist_ok=True, parents=True)
+    logger.add_file_handler(log_file)
+
     logger.debug("Command line args:")
     for arg in vars(args):
         logger.debug(f'{arg} = {str(getattr(args, arg))}')
 
     # validate command line arguments
     if args.ifo is None:
         parser.error("Cannot determine IFO prefix from sytem, "
@@ -846,15 +851,16 @@
         truncate = online and newdag and lastseg[1] == dataend
 
     # if final segment is shorter than two chunks, remove it entirely
     # so that it gets processed next time (when it will either a closed
     # segment, or long enough to process safely)
     if truncate and abs(lastseg) < chunkdur * 2:
         logger.info(
-            "The final segment is too short, but ends at the limit of "
+            "The final segment is too short, " f'Minimum length is {int(chunkdur*2)} '
+            "but ends at the limit of "
             "available data, presumably this is an active segment. It "
             "will be removed so that it can be processed properly later",
         )
         segs = type(segs)(segs[:-1])
         dataend = lastseg[0]
     # otherwise, we remove the final chunk (so that the next run has at
     # least that on which to operate), then truncate to an integer number
@@ -938,19 +944,16 @@
     segs = type(segs)(s for s in segs if abs(s) >= segdur)
 
     # if all of the data are available, but no analysable segments were found
     # (i.e. IFO not in right state for all times), record segments.txt
     if newdag and len(segs) == 0 and online and alldata:
         logger.info(
             "No analysable segments found, but up-to-date data are "
-            "available. A segments.txt file will be written so we don't "
-            "have to search these data again",
+            "available. "
         )
-        segments.write_segments(cachesegs, segfile)
-        logger.info("Segments written to\n%s" % segfile)
         clean_dirs(run_dir_list)
         clean_exit(0, tempfiles)
 
     # otherwise not all data are available, so
     elif len(segs) == 0 and online:
         logger.info("No analysable segments found, please try again later")
         clean_dirs(run_dir_list)
@@ -1009,33 +1012,39 @@
         args.universe,
         args.executable,
         subdir=condir,
         logdir=logdir,
         **condorcmds
     )
     # This allows us to start with a memory request that works maybe 80%, but bumps it if we go over
+    # we also limit individual jobs to a max runtime to cause them to be vacates to deal with NFS hanging
     reqmem = condorcmds.pop('request_memory', 1024)
     ojob.add_condor_cmd('+InitialRequestMemory', f'{reqmem}')
     ojob.add_condor_cmd('request_memory', f'ifthenelse(isUndefined(MemoryUsage), {reqmem}, int(3*MemoryUsage))')
-    ojob.add_condor_cmd('periodic_release', '(HoldReasonCode =?= 26 || HoldReasonCode =?= 34) && (JobStatus == 5)')
+    ojob.add_condor_cmd('periodic_release', '(HoldReasonCode =?= 26 || HoldReasonCode =?= 34 '
+                                            '|| HoldReasonCode =?= 46) && (JobStatus == 5)')
+    ojob.add_condor_cmd('allowed_job_duration', 3 * 3600)
     ojob.add_condor_cmd('periodic_remove', '(JobStatus == 1) && MemoryUsage >= 7G')
 
     ojob.add_condor_cmd('+OmicronProcess', f'"{group}"')
 
     # create post-processing jobs
     ppjob = condor.OmicronProcessJob(args.universe, find_executable('bash'),
                                      subdir=condir, logdir=logdir,
                                      tag='post-processing', **condorcmds)
     ppjob.add_condor_cmd('+OmicronPostProcess', f'"{group}"')
     ppmem = 1024
     ppjob.add_condor_cmd('+InitialRequestMemory', f'{ppmem}')
     ppjob.add_condor_cmd('request_memory',
                          f'ifthenelse(isUndefined(MemoryUsage), {ppmem}, int(3*MemoryUsage))')
+    ojob.add_condor_cmd('allowed_job_duration', 3 * 3600)
     ppjob.add_condor_cmd('periodic_release',
-                         '(HoldReasonCode =?= 26 || HoldReasonCode =?= 34) && (JobStatus == 5)')
+                         '(HoldReasonCode =?= 26 || HoldReasonCode =?= 34 '
+                         '|| HoldReasonCode =?= 46) && (JobStatus == 5)')
+
     ppjob.add_condor_cmd('periodic_remove', '(JobStatus == 1) && MemoryUsage >= 7G')
 
     ppjob.add_condor_cmd('environment', '"HDF5_USE_FILE_LOCKING=FALSE"')
     ppjob.add_short_opt('e', '')
     ppnodes = []
     prog_path = dict()
     prog_path['omicron-merge'] = find_executable('omicron-merge-with-gaps')
@@ -1155,15 +1164,15 @@
                         rmfiles.append(rootfiles)
 
                     # add HDF5 operations
                     if 'hdf5' in fileformats:
                         hdf5files = ' '.join(omicronfiles[c]['hdf5'])
                         for f in omicronfiles[c]['hdf5']:
                             ppnode.add_input_file(f)
-                        no_merge = '--no-merge' if args.skip_root_merge else ''
+                        no_merge = '--no-merge' if args.skip_hdf5_merge else ''
 
                         operations.append(
                             f'  {prog_path["omicron-merge"]} {no_merge}  '
                             f' --out-dir {mergepath} {hdf5files} ')
                         rmfiles.append(hdf5files)
 
                     # add LIGO_LW operations
```

### Comparing `pyomicron-2.0.4/omicron/cli/root_merge.py` & `pyomicron-2.0.5/omicron/cli/root_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 """Merge multiple Omicron ROOT files into one
 """
 
 import os.path
 import argparse
 
-from omicron import (io, __version__)
+from .. import (io, __version__)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 def create_parser():
     """Create a command-line parser for this entry point
     """
```

### Comparing `pyomicron-2.0.4/omicron/cli/show.py` & `pyomicron-2.0.5/omicron/cli/show.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from getpass import getuser
 
 from gwpy.table import EventTable
 from gwpy.table.filter import parse_column_filters
 from gwpy.table.filters import in_segmentlist
 from gwpy.time import to_gps
 
-from omicron import (io, const, __version__)
+from .. import (io, const, __version__)
 from omicron.data import write_cache
 from omicron.segments import (Segment, SegmentList, cache_segments)
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 BASEPATH = str(const.OMICRON_ARCHIVE).replace(getuser(), 'detchar')
```

### Comparing `pyomicron-2.0.4/omicron/cli/status.py` & `pyomicron-2.0.5/omicron/cli/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import logging
 import operator
 import sys
 import warnings
 from collections import OrderedDict
 from functools import reduce
 from getpass import getuser
+from os import linesep
 from pathlib import Path
+from textwrap import indent
 from time import sleep
 
 import htcondor
 
 import numpy
 
 from matplotlib import (rcParams, use)
@@ -47,16 +49,16 @@
 
 from gwpy.io.cache import sieve as sieve_cache
 from gwpy.time import to_gps
 from gwpy.segments import (Segment, SegmentList)
 from gwpy.plot import Plot
 from gwpy.plot.segments import SegmentRectangle
 
-from omicron import (condor, const, io, log, segments, __version__)
-from omicron.utils import get_omicron_version
+from .. import (condor, const, io, log, segments, __version__)
+from ..utils import get_omicron_version
 
 __author__ = "Duncan Macleod <duncan.macleod@ligo.org>"
 
 NOW = int(to_gps('now'))
 logger = None
 
 
@@ -709,15 +711,24 @@
     status = []
     for segset, tag in zip([gaps, overlap], ['gaps', 'overlap']):
         chans = [(c, segset[c]) for c in segset
                  if abs(reduce(operator.or_, segset[c].values()))]
         jsonfp = outdir / "nagios-{}-{}.json".format(tag, group)
         status.append((tag, jsonfp))
         if chans:
-            gapstr = '\n'.join('%s: %s' % c for c in chans)
+            # format the segments nicely for Icinga 2
+            lines = []
+            for chan, ftsegs in chans:
+                lines.append(f"{chan}:")
+                for ft, segs in ftsegs.items():
+                    lines.extend((
+                        f"  {ft}:",
+                        indent(str(segs), "    "),
+                    ))
+            gapstr = linesep.join(lines)
             code = 1
             message = ("%s found in Omicron files for group %r\n%s"
                        % (tag.title(), group, gapstr))
         else:
             code = 0
             message = (
                 "No %s found in Omicron files for group %r" % (tag, group)
```

### Comparing `pyomicron-2.0.4/omicron/condor.py` & `pyomicron-2.0.5/omicron/condor.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/const.py` & `pyomicron-2.0.5/omicron/const.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/data.py` & `pyomicron-2.0.5/omicron/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,34 +227,34 @@
             end,
             **kwargs
         ))
 
     return cache
 
 
-def find_ll_frames(ifo, frametype, start, end, root='/dev/shm', tmpdir=None):
+def find_ll_frames(ifo, frametype, start, end, root='/dev/shm/kafka', tmpdir=None):
     """Find all buffered low-latency frames in the given interval
 
     Parameters
     ----------
     ifo : `str`
         the IFO prefix, e.g. 'L1'
     frametype : `str`
         the frame type identifier, e.g. 'llhoft'
     start : `int`
         the GPS start time of this search
     end : `int`
         the GPS end time of this search
     root : `str`, optional
-        the base root for the buffer, defaults to `/dev/shm`
+        the base root for the buffer, defaults to `/dev/shm/kafka`
     on_gaps : `str`, optional
         what to do when the found frames don't cover the full span, one of
         'warn', 'raise', or 'ignore'
     tmpdir : `str`, optional
-        temporary directory into which to copy files from /dev/shm
+        temporary directory into which to copy files from /dev/shm/kafka
 
         ..note::
 
            Caller is reponsible for deleting the direcotyr and its
            contents when done with it.
 
     Returns
@@ -279,20 +279,23 @@
             new = os.path.join(tmpdir, os.path.basename(path))
             shutil.copyfile(path, new)
             out.append(new)
         return out
     return cache
 
 
-def _find_ll_frames(ifo, frametype, root='/dev/shm', ext='gwf'):
+def _find_ll_frames(ifo, frametype, root='/dev/shm/kafka', ext='gwf'):
     obs = ifo[0]
-    bits = frametype.rsplit('_', 1)
-    basedir = os.path.join(root, *bits[::-1])
-    globstr = os.path.join(basedir, '{obs}-{frametype}-*-*.{ext}'.format(
-        obs=obs, frametype=frametype, ext=ext))
+    root = root.rstrip(os.path.sep)
+    if root.endswith("kafka"):  # new shm system
+        subdirs = [ifo]
+    else:  # old 'lsmp' system
+        subdirs = frametype.rsplit('_', 1)[::-1]
+    basedir = os.path.join(root, *subdirs)
+    globstr = os.path.join(basedir, f"{obs}-{frametype}-*-*.{ext}")
     # don't return the last file, as it might not have been fully written yet
     return sorted(glob.glob(globstr)[:-1])
 
 
 # -- find latest file ---------------------------------------------------------
 
 def get_latest_data_gps(obs, frametype):
```

### Comparing `pyomicron-2.0.4/omicron/io.py` & `pyomicron-2.0.5/omicron/io.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/log.py` & `pyomicron-2.0.5/omicron/log.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/nagios.py` & `pyomicron-2.0.5/omicron/nagios.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/parameters.py` & `pyomicron-2.0.5/omicron/parameters.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/segments.py` & `pyomicron-2.0.5/omicron/segments.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/__init__.py` & `pyomicron-2.0.5/omicron/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/mock_htcondor.py` & `pyomicron-2.0.5/omicron/tests/mock_htcondor.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_condor.py` & `pyomicron-2.0.5/omicron/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_const.py` & `pyomicron-2.0.5/omicron/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_io.py` & `pyomicron-2.0.5/omicron/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_log.py` & `pyomicron-2.0.5/omicron/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_nagios.py` & `pyomicron-2.0.5/omicron/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_parameters.py` & `pyomicron-2.0.5/omicron/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_segments.py` & `pyomicron-2.0.5/omicron/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/test_utils.py` & `pyomicron-2.0.5/omicron/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/tests/utils.py` & `pyomicron-2.0.5/omicron/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/omicron/utils.py` & `pyomicron-2.0.5/omicron/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,16 @@
     try:
         return StrictVersion(
             subprocess.check_output([
                 executable,
                 "version",
             ]).decode("utf-8").rsplit(maxsplit=1)[-1],
         )
-    except subprocess.CalledProcessError:
-        raise RuntimeError(
-            "failed to determine omicron version from executable"
-        )
+    except subprocess.CalledProcessError as ex:
+        raise RuntimeError(f"failed to determine omicron version from executable: {str(ex)}")
 
 
 def astropy_config_path(parent, update_environ=True):
     """Create and return a directory for a temporary astropy config path
     """
     parent = Path(parent)
     astropath = parent / ".config" / "astropy"
```

### Comparing `pyomicron-2.0.4/pyomicron.egg-info/PKG-INFO` & `pyomicron-2.0.5/pyomicron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyomicron
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python utilities and wrappers for GW Omicron
 Home-page: https://github.com/gwpy/pyomicron
 Download-URL: https://pypi.org/project/pyomicron/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 Maintainer: Joseph Areeda
 Maintainer-email: joseph.areeda@ligo.org
```

### Comparing `pyomicron-2.0.4/pyomicron.egg-info/SOURCES.txt` & `pyomicron-2.0.5/pyomicron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyomicron-2.0.4/setup.cfg` & `pyomicron-2.0.5/setup.cfg`

 * *Files identical despite different names*

