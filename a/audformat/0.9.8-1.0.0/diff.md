# Comparing `tmp/audformat-0.9.8.tar.gz` & `tmp/audformat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audformat-0.9.8.tar", last modified: Tue Feb 23 07:04:32 2021, max compression
+gzip compressed data, was "audformat-1.0.0.tar", last modified: Thu Apr 27 13:00:24 2023, max compression
```

## Comparing `audformat-0.9.8.tar` & `audformat-1.0.0.tar`

### file list

```diff
@@ -1,85 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.517134 audformat-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.517134 audformat-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2021-02-23 07:04:22.000000 audformat-0.9.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1889 2021-02-23 07:04:22.000000 audformat-0.9.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)      111 2021-02-23 07:04:22.000000 audformat-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     2695 2021-02-23 07:04:22.000000 audformat-0.9.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2089 2021-02-23 07:04:22.000000 audformat-0.9.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1143 2021-02-23 07:04:22.000000 audformat-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     6708 2021-02-23 07:04:32.525134 audformat-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1924 2021-02-23 07:04:22.000000 audformat-0.9.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.517134 audformat-0.9.8/audformat/
--rw-r--r--   0 runner    (1001) docker     (116)      780 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/audformat/core/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7075 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/column.py
--rw-r--r--   0 runner    (1001) docker     (116)     7031 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/common.py
--rw-r--r--   0 runner    (1001) docker     (116)    19552 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/database.py
--rw-r--r--   0 runner    (1001) docker     (116)     2223 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/define.py
--rw-r--r--   0 runner    (1001) docker     (116)     1558 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     7152 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/index.py
--rw-r--r--   0 runner    (1001) docker     (116)     2434 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/media.py
--rw-r--r--   0 runner    (1001) docker     (116)      780 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/rater.py
--rw-r--r--   0 runner    (1001) docker     (116)     7947 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/scheme.py
--rw-r--r--   0 runner    (1001) docker     (116)      864 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/split.py
--rw-r--r--   0 runner    (1001) docker     (116)    28221 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/table.py
--rw-r--r--   0 runner    (1001) docker     (116)     9137 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (116)      476 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (116)    18627 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/audformat/define/
--rw-r--r--   0 runner    (1001) docker     (116)      188 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/define/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/audformat/errors/
--rw-r--r--   0 runner    (1001) docker     (116)       91 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/audformat/testing/
--rw-r--r--   0 runner    (1001) docker     (116)       93 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/audformat/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      154 2021-02-23 07:04:22.000000 audformat-0.9.8/audformat/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.517134 audformat-0.9.8/audformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6708 2021-02-23 07:04:32.000000 audformat-0.9.8/audformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2021-02-23 07:04:32.000000 audformat-0.9.8/audformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-23 07:04:32.000000 audformat-0.9.8/audformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       73 2021-02-23 07:04:32.000000 audformat-0.9.8/audformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-02-23 07:04:32.000000 audformat-0.9.8/audformat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     1238 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/accessing-data.rst
--rw-r--r--   0 runner    (1001) docker     (116)      880 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/api-define.rst
--rw-r--r--   0 runner    (1001) docker     (116)      276 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/api-errors.rst
--rw-r--r--   0 runner    (1001) docker     (116)      529 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/api-testing.rst
--rw-r--r--   0 runner    (1001) docker     (116)      454 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/api-utils.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1078 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       30 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1905 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/combine-tables.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2637 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3157 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/create-database.rst
--rw-r--r--   0 runner    (1001) docker     (116)     8407 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/data-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (116)      492 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/data-example.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1673 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/data-format.rst
--rw-r--r--   0 runner    (1001) docker     (116)    10327 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/data-header.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/data-introduction.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4293 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/data-tables.rst
--rw-r--r--   0 runner    (1001) docker     (116)    11007 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/emodb-example.rst
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (116)      826 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      284 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/map-scheme.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (116)      467 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/pics/audformat.dot
--rw-r--r--   0 runner    (1001) docker     (116)      903 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/pics/tables.dot
--rw-r--r--   0 runner    (1001) docker     (116)      699 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/pics/workflow.dot
--rw-r--r--   0 runner    (1001) docker     (116)      117 2021-02-23 07:04:22.000000 audformat-0.9.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2021-02-23 07:04:22.000000 audformat-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1420 2021-02-23 07:04:32.525134 audformat-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       59 2021-02-23 07:04:22.000000 audformat-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 07:04:32.521134 audformat-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)      131 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     8222 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (116)     8028 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     2256 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (116)     1616 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     5774 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_scheme.py
--rw-r--r--   0 runner    (1001) docker     (116)    17942 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (116)    27570 2021-02-23 07:04:22.000000 audformat-0.9.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.785670 audformat-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.773670 audformat-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-27 13:00:09.000000 audformat-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-27 13:00:09.000000 audformat-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 13:00:09.000000 audformat-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-04-27 13:00:09.000000 audformat-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-27 13:00:09.000000 audformat-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 13:00:09.000000 audformat-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21353 2023-04-27 13:00:24.785670 audformat-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-27 13:00:09.000000 audformat-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/audformat/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/audformat/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41048 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/rater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50292 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59756 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/define/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/define/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/audformat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 13:00:09.000000 audformat-1.0.0/audformat/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/audformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21353 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 13:00:24.000000 audformat-1.0.0/audformat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-27 13:00:09.000000 audformat-1.0.0/benchmarks/benchmark_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.777670 audformat-1.0.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/accessing-data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api/audformat.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.define.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/api-src/audformat.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/combine-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/create-database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-misc-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/data-tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/emodb-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/map-scheme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.781670 audformat-1.0.0/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/pics/audformat-database.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/pics/audformat-misc-table.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/pics/audformat-table.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-27 13:00:09.000000 audformat-1.0.0/docs/update-database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 13:00:09.000000 audformat-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-27 13:00:24.785670 audformat-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 13:00:09.000000 audformat-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:00:24.785670 audformat-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46124 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_misc_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55836 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85100 2023-04-27 13:00:09.000000 audformat-1.0.0/tests/test_utils.py
```

### Comparing `audformat-0.9.8/.github/workflows/publish.yml` & `audformat-1.0.0/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 2
 
     - name: Cache emodb
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
         path: emodb-src
         key: emodb-ubuntu
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.x'
+        python-version: '3.8'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
 
     # PyPI package
@@ -71,14 +71,14 @@
         CHANGELOG="${CHANGELOG//$'\n'/'%0A'}"
         CHANGELOG="${CHANGELOG//$'\r'/'%0D'}"
         echo "Got changelog: $CHANGELOG"
         echo "::set-output name=body::$CHANGELOG"
 
     - name: Create release on Github
       id: create_release
-      uses: actions/create-release@v1
+      uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
-        release_name: Release ${{ github.ref }}
+        name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audformat-0.9.8/.github/workflows/test.yml` & `audformat-1.0.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,62 @@
 name: Test
 
 on:
   push:
-    branches: [ master ]
+    branches: [ main ]
   pull_request:
-    branches: [ master ]
+    branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ ubuntu-18.04, windows-latest, macOS-latest ]
-        python-version: [3.6]
+        os: [ ubuntu-20.04, windows-latest, macOS-latest ]
+        python-version: [ '3.8' ]
         include:
           - os: ubuntu-latest
-            python-version: 3.7
+            python-version: '3.9'
           - os: ubuntu-latest
-            python-version: 3.8
+            python-version: '3.10'
+          - os: ubuntu-latest
+            python-version: '3.11'
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Cache emodb
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
         path: emodb-src
         key: emodb-ubuntu
-      if: matrix.os == 'ubuntu-18.04'
+      if: matrix.os == 'ubuntu-20.04'
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Prepare Ubuntu
       run: |
         sudo apt-get update
-        sudo apt-get install --no-install-recommends --yes graphviz libsndfile1 sox
-      if: matrix.os == 'ubuntu-latest' || matrix.os == 'ubuntu-18.04'
-
-    - name: Prepare Windows
-      run: choco install sox.portable
-      if: matrix.os == 'windows-latest'
-
-    - name: Prepare OSX
-      run: brew install sox
-      if: matrix.os == 'macOS-latest'
+        sudo apt-get install --no-install-recommends --yes libsndfile1
+      if: matrix.os == 'ubuntu-latest' || matrix.os == 'ubuntu-20.04'
 
     - name: Install dependencies
       run: |
         python -V
         python -m pip install --upgrade pip
         pip install -r requirements.txt
-        pip install -r docs/requirements.txt
         pip install -r tests/requirements.txt
 
     - name: Test with pytest
       run: |
         python -m pytest
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
-      if: matrix.os == 'ubuntu-18.04'
-
-    - name: Test building documentation
-      run: |
-        python -m sphinx docs/ docs/_build/ -b html -W
-        python -m sphinx docs/ build/sphinx/html -b linkcheck
-      if: matrix.os == 'ubuntu-18.04'
+      if: matrix.os == 'ubuntu-20.04'
```

### Comparing `audformat-0.9.8/CONTRIBUTING.rst` & `audformat-1.0.0/CONTRIBUTING.rst`

 * *Files 20% similar despite different names*

```diff
@@ -17,23 +17,56 @@
 you should get the newest development version from Github_::
 
     git clone https://github.com/audeering/audformat/
     cd audformat
     # Create virutal environment for this project
     # e.g.
     # virtualenv --python="python3"  $HOME/.envs/audformat
-    # source $HOME/.envs/audeer/bin/activate
+    # source $HOME/.envs/audformat/bin/activate
     pip install -r requirements.txt
 
 .. _Github: https://github.com/audeering/audformat
 
 This way, your installation always stays up-to-date,
 even if you pull new changes from the Github repository.
 
 
+Coding Convention
+-----------------
+
+We follow the PEP8_ convention for Python code
+and check for correct syntax with flake8_.
+Exceptions are defined under the ``[flake8]`` section
+in :file:`setup.cfg`.
+
+The checks are executed in the CI using `pre-commit`_.
+You can enable those checks locally by executing::
+
+    pip install pre-commit  # consider system wide installation
+    pre-commit install
+    pre-commit run --all-files
+
+Afterwards flake8_ is executed
+every time you create a commit.
+
+You can also install flake8_
+and call it directly::
+
+    pip install flake8  # consider system wide installation
+    flake8
+
+It can be restricted to specific folders::
+
+    flake8 audfoo/ tests/
+
+.. _PEP8: http://www.python.org/dev/peps/pep-0008/
+.. _flake8: https://flake8.pycqa.org/en/latest/index.html
+.. _pre-commit: https://pre-commit.com
+
+
 Building the Documentation
 --------------------------
 
 If you make changes to the documentation,
 you can re-create the HTML pages using Sphinx_.
 You can install it and a few other necessary packages with::
```

### Comparing `audformat-0.9.8/LICENSE` & `audformat-1.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MIT License
 
-Copyright (c) 2018-2020 audEERING GmbH and Contributors
+Copyright (c) 2018-present audEERING GmbH and Contributors
 
 Authors:
     Johannes Wagner
     Hagen Wierstorf
+    Baha Eddine Abrougui
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `audformat-0.9.8/README.rst` & `audformat-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `audformat-0.9.8/audformat/__init__.py` & `audformat-1.0.0/audformat/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from audformat import define
 from audformat import errors
 from audformat import utils
+from audformat.core.attachment import Attachment
+from audformat.core.column import Column
 from audformat.core.database import Database
 from audformat.core.index import (
     assert_index,
+    assert_no_duplicates,
     filewise_index,
-    segmented_index,
     index_type,
+    is_filewise_index,
+    is_segmented_index,
+    segmented_index,
 )
 from audformat.core.media import Media
 from audformat.core.rater import Rater
 from audformat.core.scheme import Scheme
 from audformat.core.split import Split
 from audformat.core.table import (
-    Column,
+    MiscTable,
     Table,
 )
 
 
 # Discourage from audformat import *
 __all__ = []
```

### Comparing `audformat-0.9.8/audformat/core/column.py` & `audformat-1.0.0/audformat/core/column.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,72 @@
+from __future__ import annotations  # allow typing without string
+
+import typing
+import warnings
+
 import numpy as np
 import pandas as pd
 
 from audformat.core import define
 from audformat.core.common import HeaderBase
 from audformat.core.index import (
     index_type,
     is_scalar,
     to_array,
 )
-from audformat.core.scheme import Scheme
+from audformat.core.rater import Rater
 from audformat.core.typing import Values
 
+if typing.TYPE_CHECKING:
+    # Fix to make mypy work without circular imports,
+    # compare
+    # https://adamj.eu/tech/2021/05/13/python-type-hints-how-to-fix-circular-imports/
+    from audformat.core.scheme import Scheme  # pragma: nocover
+
 
 def assert_values(
         values: Values,
         scheme: Scheme,
 ):
     r"""Raise error if values do not match scheme."""
-    ok = True
+    bad_values = []
 
-    if scheme.labels is not None or \
-            scheme.minimum is not None or \
-            scheme.maximum is not None:
+    if (
+            scheme.labels is not None
+            or scheme.minimum is not None
+            or scheme.maximum is not None
+    ):
 
         if is_scalar(values):
-            ok = values in scheme
-        else:
-            if isinstance(values, pd.Series):
-                values = values.values
-            if isinstance(values, np.ndarray):
-                if scheme.is_numeric:
-                    values = [
-                        np.min(values),
-                        np.max(values),
-                    ]
-                else:
-                    values = np.unique(values)
-            else:
-                values = set(values)
-            ok = all([value in scheme for value in values])
-
-    if not ok:
+            values = [values]
+        elif isinstance(values, pd.Series):
+            values = values.values
+        elif isinstance(values, np.ndarray):
+            if scheme.is_numeric:
+                # Support type object with None entries,
+                # which need to be converted to NaN
+                # to support min/max
+                values = values.astype(float)
+                values = [
+                    np.nanmin(values),
+                    np.nanmax(values),
+                ]
+        # Get unique values and preserve order
+        values = list(dict.fromkeys(values))
+        bad_values = [value for value in values if value not in scheme]
+
+    if len(bad_values) > 0:
+        max_display = 10
+        values = str(bad_values[:max_display])[1:-1]
+        if len(bad_values) > max_display:
+            values += ', ...'
         raise ValueError(
-            f'Some value(s) do not match scheme:\n{scheme}.'
+            f"Some value(s) do not match scheme\n{scheme}\n"
+            f"with scheme ID '{scheme._id}':\n"
+            f'{values}'
         )
 
 
 class Column(HeaderBase):
     r"""Table column.
 
     Represents a table column (see :class:`audformat.Table`) and
@@ -55,15 +75,15 @@
 
     Args:
         scheme_id: scheme identifier (must exist)
         rater_id: rater identifier (must exist)
         description: table description
         meta: additional meta fields
 
-    Example:
+    Examples:
         >>> Column(scheme_id='emotion')
         {scheme_id: emotion}
 
     """
     def __init__(
             self,
             *,
@@ -77,119 +97,214 @@
         self.scheme_id = scheme_id
         r"""Scheme identifier"""
         self.rater_id = rater_id
         r"""Rater identifier"""
         self._table = None
         self._id = None
 
+    @property
+    def rater(self) -> typing.Optional[Rater]:
+        r"""Rater object.
+
+        Returns:
+            rater object or ``None`` if not available
+
+        """
+        if (
+                self.rater_id is not None
+        ) and (
+                self.table is not None
+        ) and (
+                self.table.db is not None
+        ):
+            return self.table.db.raters[self.rater_id]
+
+    @property
+    def scheme(self) -> typing.Optional[Scheme]:
+        r"""Scheme object.
+
+        Returns:
+            scheme object or ``None`` if not available
+
+        """
+        if (
+                self.scheme_id is not None
+        ) and (
+                self.table is not None
+        ) and (
+                self.table.db is not None
+        ):
+            return self.table.db.schemes[self.scheme_id]
+
+    @property
+    def table(self):
+        r"""Table object.
+
+        Returns:
+            table object or ``None`` if not assigned yet
+
+        """
+        return self._table
+
     def get(
             self,
             index: pd.Index = None,
             *,
             map: str = None,
             copy: bool = True,
+            as_segmented: bool = False,
+            allow_nat: bool = True,
+            root: str = None,
+            num_workers: typing.Optional[int] = 1,
+            verbose: bool = False,
     ) -> pd.Series:
         r"""Get labels.
 
-        By default all labels of the column are returned,
+        By default, all labels of the column are returned,
         use ``index`` to get a subset.
 
         Examples are provided with the
         :ref:`table specifications <data-tables:Tables>`.
 
         Args:
             index: index conform to
                 :ref:`table specifications <data-tables:Tables>`
             copy: return a copy of the labels
-            map: map scheme or scheme field to column values.
+            map: :ref:`map scheme or scheme field to column values
+                <map-scheme-labels>`.
                 For example if your column holds speaker IDs and is
                 assigned to a scheme that contains a dict mapping
                 speaker IDs to age entries, ``map='age'``
                 will replace the ID values with the age of the speaker
+            as_segmented: if set to ``True``
+                and column has a filewise index,
+                the index of the returned column
+                will be converted to a segmented index.
+                ``start`` will be set to ``0`` and
+                ``end`` to ``NaT`` or to the file duration
+                if ``allow_nat`` is set to ``False``.
+                If column belongs to a miscellaneous table,
+                this and the following arguments have no effect
+            allow_nat: if set to ``False``,
+                ``end=NaT`` is replaced with file duration
+            root: root directory under which the files are stored.
+                Provide if file names are relative and
+                database was not saved or loaded from disk.
+                If ``None`` :attr:`audformat.Database.root` is used.
+                Only relevant if ``allow_nat`` is set to ``False``
+            num_workers: number of parallel jobs.
+                If ``None`` will be set to the number of processors
+                on the machine multiplied by 5
+            verbose: show progress bar
 
         Returns:
             labels
 
         Raises:
+            FileNotFoundError: if file is not found
             RuntimeError: if column is not assigned to a table
-            ValueError: if trying to map without a scheme
-            ValueError: if trying to map from a scheme that has no labels
-            ValueError: if trying to map to a non-existing field
+            ValueError: if trying to map without a scheme,
+                or from a scheme that has no labels,
+                or from a scheme that has only a list of labels,
+                or to a non-existing field
 
         """
         if self._table is None:
             raise RuntimeError(
                 'Column is not assigned to a table.'
             )
 
-        result = self._table.get(index, copy=False)
+        if hasattr(self._table, 'type'):
+            result = self._table.get(
+                index,
+                copy=False,
+                as_segmented=as_segmented,
+                allow_nat=allow_nat,
+                root=root,
+                num_workers=num_workers,
+                verbose=verbose,
+            )
+        else:
+            result = self._table.get(
+                index,
+                copy=False,
+            )
         result = result[self._id]
 
         if map is not None:
 
             copy = False  # to avoid another copy
 
             if self.scheme_id is None:
                 raise ValueError(
                     f"Column '{self._id}' is not assigned to a scheme."
                 )
 
-            labels = self._table._db.schemes[self.scheme_id].labels
+            scheme = self._table._db.schemes[self.scheme_id]
+            labels = scheme._labels_to_dict()
 
             if labels is None:
                 raise ValueError(
                     f"Scheme '{self.scheme_id}' has no labels."
                 )
 
+            if not any(labels.values()):
+                raise ValueError(
+                    f"Scheme '{self.scheme_id}' provides no mapping "
+                    "for its labels."
+                )
+
             mapping = {}
             for key, value in labels.items():
                 if isinstance(value, dict):
                     if map in value:
                         value = value[map]
                     else:
                         raise ValueError(
                             f"Cannot map "
-                            f"'{mapping}' "
+                            f"'{self._id}' "
                             f"to "
-                            f"'{self._id}'. "
+                            f"'{map}'. "
                             f"Expected one of "
                             f"{list(value)}."
                         )
                 mapping[key] = value
-            result = result.map(mapping)
+            result = result.map(mapping).astype('category')
             result.name = map
 
         return result.copy() if copy else result
 
     def set(
             self,
             values: Values,
             *,
             index: pd.Index = None,
     ):
         r"""Set labels.
 
-        By default all labels of the column are replaced,
+        By default, all labels of the column are replaced,
         use ``index`` to set a subset.
         If columns is assigned to a :class:`Scheme`
-        values have to match its ``dtype``.
+        values will be automatically converted
+        to match its dtype.
 
         Examples are provided with the
         :ref:`table specifications <data-tables:Tables>`.
 
         Args:
             values: list of values
             index: index conform to
                 :ref:`table specifications <data-tables:Tables>`
 
         Raises:
             RuntimeError: if column is not assign to a table
             ValueError: if trying to set values of a filewise column
                 using a segmented index
-            ValueError: if values do not match scheme
+            ValueError: if values cannot be converted
+                to match the schemes dtype
 
         """
         if self._table is None:
             raise RuntimeError(
                 'Column is not assigned to a table.'
             )
 
@@ -198,34 +313,57 @@
 
         if index is None:
             index = df.index
 
         if self.scheme_id is not None:
             scheme = self._table._db.schemes[self.scheme_id]
             assert_values(values, scheme)
-
-        if index_type(df.index) == index_type(index):
-            if is_scalar(values):
-                values = [values] * len(index)
-            values = to_array(values)
-            df.loc[index, column_id] = pd.Series(
-                values,
-                index=index,
-                dtype=df[column_id].dtype,
-            )
+            dtype = scheme.to_pandas_dtype()
         else:
+            dtype = df[column_id].dtype
+
+        if hasattr(self._table, 'type') and \
+                self._table.type != index_type(index):
+            # special case where a filewise / segmented table
+            # is requested with an index of the other type
             if not self._table.is_filewise:
                 files = index.get_level_values(define.IndexField.FILE)
                 index = df.loc[files].index
                 return self.set(values, index=index)
             else:
                 raise ValueError(
                     'Cannot set values of a filewise column '
                     'using a segmented index.'
                 )
+        else:
+            if is_scalar(values):
+                values = [values] * len(index)
+            values = to_array(values)
+            if dtype == 'datetime64[ns]':
+                # Ensure all date values are timezone unaware,
+                # see https://github.com/audeering/audformat/issues/364
+                values = [
+                    pd.to_datetime(value).tz_localize(None)
+                    if value is not None else value
+                    for value in values
+                ]
+            with warnings.catch_warnings():
+                # Avoid FutureWarning and DeprecationWarning
+                # for pandas 1.5.0 to 1.5.3
+                # for setting values in place
+                # as introduced at
+                # https://pandas.pydata.org/docs/dev/whatsnew/v1.5.0.html#inplace-operation-when-setting-values-with-loc-and-iloc
+                # For pandas >=2.0.0 values are always set in place
+                for warning in [FutureWarning, DeprecationWarning]:
+                    warnings.simplefilter(action='ignore', category=warning)
+                df.loc[index, column_id] = pd.Series(
+                    values,
+                    index=index,
+                    dtype=dtype,
+                )
 
     def __eq__(
             self,
             other: 'Column',
     ) -> bool:
         if self.dump() != other.dump():
             return False
```

### Comparing `audformat-0.9.8/audformat/core/common.py` & `audformat-1.0.0/audformat/core/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import inspect
+import os
 import oyaml as yaml
-from typing import Sequence, Callable
+import typing
 import textwrap
 from collections import OrderedDict
 
 import pandas as pd
 
-from audformat.core.errors import BadTypeError, BadValueError
+from audformat import define
+from audformat.core.errors import (
+    BadKeyError,
+    BadTypeError,
+    BadValueError,
+)
 
 
 class HeaderDict(OrderedDict):
     r"""Custom implementation of a dictionary.
 
     * by default ``items()`` returns a sorted iterator (see ``sorted_iter``)
     * prints the dictionary in a prettified way:
@@ -20,88 +26,138 @@
           key-1:
             value-1
           key-2:
             value-2
 
     Args:
         *args: default arguments
-        sorted_iter: if set, ``items()`` returns a sorted iterator
+        sort_by_key: if ``True`` maintain a sorted order,
+            otherwise order by assignment
         value_type: only accept values of this type
         get_callback: call this function when an item is requested
         set_callback: call this function when an item is added
         **kwargs: default keyword arguments
 
     Raises:
         BadTypeError: if a value of an invalid type is added
 
-    Example:
+    Examples:
         >>> HeaderDict()
 
+        >>> d = HeaderDict()
+        >>> d['b'] = 1
+        >>> d['a'] = 0
+        >>> d
+        a:
+          0
+        b:
+          1
+        >>> d = HeaderDict(sort_by_key=False)
+        >>> d['b'] = 1
+        >>> d['a'] = 0
+        >>> d
+        b:
+          1
+        a:
+          0
         >>> HeaderDict(
         ...     get_callback=lambda key, value: value + value,
         ...     set_callback=lambda key, value: value.upper(),
         ...     foo='bar',
         ... )
         foo:
           BARBAR
 
     """
     def __init__(
             self,
             *args,
-            sorted_iter: bool = True,
+            sort_by_key: bool = True,
             value_type: type = None,
-            get_callback: Callable = None,
-            set_callback: Callable = None,
+            get_callback: typing.Callable = None,
+            set_callback: typing.Callable = None,
             **kwargs,
     ):
-        self.sorted_iter = sorted_iter
-        r"""Use sorted iterator"""
+        self.sort_by_key = sort_by_key
+        r"""Sort items by key"""
         self.value_type = value_type
         r"""Only accept values of this type"""
         self.get_callback = get_callback
         r"""Callback function when item is requested"""
         self.set_callback = set_callback
         r"""Callback function when item is added"""
-        super().__init__(*args, **kwargs)
 
-    def __setitem__(self, key, value):
-        if self.set_callback is not None:
-            value = self.set_callback(key, value)
-        if self.value_type is not None:
-            if not isinstance(value, self.value_type):
-                raise BadTypeError(value, self.value_type)
-        super().__setitem__(key, value)
+        super().__init__(*args, **kwargs)
 
     def __getitem__(self, key):
+        if key not in self:
+            raise BadKeyError(key, list(self))
         value = super().__getitem__(key)
         if self.get_callback is not None:
             value = self.get_callback(key, value)
         return value
 
-    def items(self):
-        if self.sorted_iter:
-            return iter(sorted(super().items()))
+    def __iter__(self):
+        if self.sort_by_key:
+            return sorted(super().keys()).__iter__()
         else:
-            return super().items()
+            return super().__iter__()
+
+    def __repr__(self) -> str:
+        return self.dump()
+
+    def __reversed__(self):
+        if self.sort_by_key:
+            return sorted(super().keys()).__reversed__()
+        else:
+            return super().__reversed__()
+
+    def __setitem__(self, key, value):
+        if self.set_callback is not None:
+            value = self.set_callback(key, value)
+        if self.value_type is not None:
+            if not isinstance(value, self.value_type):
+                raise BadTypeError(value, self.value_type)
+        super().__setitem__(key, value)
 
     def dump(self) -> str:
         if not self:
             return ''
         else:
             return '\n'.join(
                 [
                     '{}:\n{}'.format(
                         key, textwrap.indent(str(self[key]), '  '))
                     for key in self
                 ]
             )
 
-    def __repr__(self) -> str:
-        return self.dump()
+    def items(self):
+        if self.sort_by_key:
+            return iter(sorted(super().items()))
+        else:
+            return super().items()
+
+    def keys(self):
+        return iter([key for key, _ in self.items()])
+
+    def popitem(self, last: bool = True):
+        if len(self) > 0 and self.sort_by_key:
+            keys = list(self)
+            if last:
+                key = keys[-1]
+            else:
+                key = keys[0]
+            value = super().pop(key)
+            return key, value
+        else:
+            return super().popitem(last)
+
+    def values(self):
+        return iter([value for _, value in self.items()])
 
 
 class HeaderBase:
     r"""Base class for header objects.
 
     Args:
         description: description string
@@ -163,27 +219,27 @@
             for key, value in self.meta.items():
                 d[key] = HeaderBase._value(value)
         return d
 
     def from_dict(
             self,
             d: dict,
-            ignore_keys: Sequence[str] = None,
+            ignore_keys: typing.Sequence[str] = None,
     ):
         r"""Deserialize object from dictionary.
 
         Args:
             d: dictionary of class variables to assign
             ignore_keys: variables listed here will be ignored
 
         """
         for key, value in d.items():
             if ignore_keys and key in ignore_keys:
                 continue
-            if key in self.__dict__:
+            if key in self.__dict__ and key != 'meta':
                 if self.__dict__[key] is not None:
                     assert isinstance(value, type(self.__dict__[key]))
                 self.__dict__[key] = value
             else:
                 self.meta[key] = value
 
     def dump(
@@ -222,37 +278,89 @@
     def __str__(self):
         return repr(self)
 
 
 class DefineBase:
 
     @classmethod
-    def assert_has_attribute_value(cls, value):
-        valid_values = cls.attribute_values()
+    def _assert_has_attribute_value(cls, value):
+        valid_values = cls._attribute_values()
         if value not in valid_values:
             raise BadValueError(value, valid_values)
 
     @classmethod
-    def attribute_values(cls):
+    def _attribute_values(cls):
         attributes = inspect.getmembers(
             cls, lambda x: not inspect.isroutine(x)
         )
         return sorted(
             [
                 a[1] for a in attributes
-                if not(a[0].startswith('__') and a[0].endswith('__'))
+                if not (a[0].startswith('__') and a[0].endswith('__'))
             ]
         )
 
 
 def format_series_as_html():  # pragma: no cover (only used in documentation)
     setattr(pd.Series, '_repr_html_', series_to_html)
     setattr(pd.Index, '_repr_html_', index_to_html)
 
 
 def index_to_html(self):  # pragma: no cover
-    return self.to_frame(index=False)._repr_html_()
+    df = self.to_frame()
+    df = df.drop(columns=df.columns)
+    return df.to_html()
+
+
+def is_relative_path(path):
+    return not (
+        os.path.isabs(path)
+        or '\\' in path
+        or path.startswith('./')
+        or '/./' in path
+        or path.startswith('../')
+        or '/../' in path
+    )
 
 
 def series_to_html(self):  # pragma: no cover
     df = self.to_frame()
-    return df._repr_html_()
+    return df.to_html()
+
+
+def to_audformat_dtype(dtype: typing.Union[str, typing.Type]) -> str:
+    r"""Convert pandas to audformat dtype."""
+    if pd.api.types.is_bool_dtype(dtype):
+        return define.DataType.BOOL
+    elif pd.api.types.is_datetime64_dtype(dtype):
+        return define.DataType.DATE
+    elif pd.api.types.is_float_dtype(dtype):
+        return define.DataType.FLOAT
+    elif pd.api.types.is_integer_dtype(dtype):
+        return define.DataType.INTEGER
+    elif pd.api.types.is_timedelta64_dtype(dtype):
+        return define.DataType.TIME
+    # We cannot use pd.api.types.is_string_dtype()
+    # as it returns `True` for list, object, etc.
+    elif dtype in [str, 'str', 'string']:
+        return define.DataType.STRING
+    else:
+        # default to object
+        return define.DataType.OBJECT
+
+
+def to_pandas_dtype(dtype: str) -> str:
+    r"""Convert audformat to pandas dtype."""
+    if dtype == define.DataType.BOOL:
+        return 'boolean'
+    elif dtype == define.DataType.DATE:
+        return 'datetime64[ns]'
+    elif dtype == define.DataType.FLOAT:
+        return 'float'
+    elif dtype == define.DataType.INTEGER:
+        return 'Int64'
+    elif dtype == define.DataType.OBJECT:
+        return 'object'
+    elif dtype == define.DataType.STRING:
+        return 'string'
+    elif dtype == define.DataType.TIME:
+        return 'timedelta64[ns]'
```

### Comparing `audformat-0.9.8/audformat/core/database.py` & `audformat-1.0.0/tests/test_scheme.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,610 +1,721 @@
-import datetime
-import os
-import typing
+import re
 
-import oyaml as yaml
+import numpy as np
 import pandas as pd
+import pytest
 
-import audeer
+import audformat
+import audformat.testing
 
-from audformat.core import define
-from audformat.core import utils
-from audformat.core.index import segmented_index
-from audformat.core.column import Column
-from audformat.core.common import HeaderBase, HeaderDict
-from audformat.core.errors import BadIdError
-from audformat.core.media import Media
-from audformat.core.rater import Rater
-from audformat.core.scheme import Scheme
-from audformat.core.split import Split
-from audformat.core.table import Table
-
-
-class Database(HeaderBase):
-    r"""Database object.
-
-    A database consists of a header holding raters,
-    schemes, splits, and other meta information.
-    In addition it links to a number of tables
-    listing files and labels.
-
-    Args:
-        name: name of database
-        source: data source (e.g. link to website)
-        usage: permission of usage, see :class:`audformat.define.Usage`.
-            Set to ``OTHER`` if none of the other fields fit.
-        expires: expiry date
-        languages: list of languages
-        description: database description
-        author: database author(s)
-        license: database license.
-            You can use a custom license
-            or pick one from :attr:`audformat.define.License`.
-            In the later case,
-            ``license_url`` will be automatically set
-            if it is not given
-        license_url: URL of database license
-        meta: additional meta fields
-
-    Raises:
-        BadValueError: if an invalid ``usage`` value is passed
-        ValueError: if language is unknown
-
-    Example:
-        >>> db = Database(
-        ...     'mydb',
-        ...     'https://www.audeering.com/',
-        ...     define.Usage.COMMERCIAL,
-        ...     languages=['English', 'de'],
-        ... )
-        >>> db
-        name: mydb
-        source: https://www.audeering.com/
-        usage: commercial
-        languages: [eng, deu]
-        >>> labels = ['positive', 'neutral', 'negative']
-        >>> db.schemes['emotion'] = Scheme(
-        ...     labels=labels,
-        ... )
-        >>> db.raters['rater'] = Rater()
-        >>> db.media['audio'] = Media(
-        ...     define.MediaType.AUDIO,
-        ...     format='wav',
-        ...     sampling_rate=16000,
-        ... )
-        >>> db['table'] = Table(
-        ...     media_id='audio',
-        ... )
-        >>> db['table']['column'] = Column(
-        ...     scheme_id='emotion',
-        ...     rater_id='rater',
-        ... )
-        >>> db
-        name: mydb
-        source: https://www.audeering.com/
-        usage: commercial
-        languages: [eng, deu]
-        media:
-          audio: {type: audio, format: wav, sampling_rate: 16000}
-        raters:
-          rater: {type: human}
-        schemes:
-          emotion:
-            dtype: str
-            labels: [positive, neutral, negative]
-        tables:
-          table:
-            type: filewise
-            media_id: audio
-            columns:
-              column: {scheme_id: emotion, rater_id: rater}
-
-    """
-    def __init__(
-            self,
-            name: str,
-            source: str = '',
-            usage: define.Usage = define.Usage.UNRESTRICTED,
-            *,
-            expires: datetime.date = None,
-            languages: typing.Union[str, typing.Sequence[str]] = None,
-            description: str = None,
-            author: str = None,
-            organization: str = None,
-            license: typing.Union[str, define.License] = None,
-            license_url: str = None,
-            meta: dict = None,
-    ):
-        define.Usage.assert_has_attribute_value(usage)
-        if (
-                license_url is None
-                and license in define.License.attribute_values()
-        ):
-            license_url = define.LICENSE_URLS[license]
-
-        languages = [] if languages is None else audeer.to_list(languages)
-        for idx in range(len(languages)):
-            languages[idx] = utils.map_language(languages[idx])
-
-        self.name = name
-        r"""Name of database"""
-        super().__init__(description=description, meta=meta)
-        self.source = source
-        r"""Database source"""
-        self.usage = usage
-        r"""Usage permission"""
-        self.expires = expires
-        r"""Expiry date"""
-        self.languages = languages
-        r"""List of included languages"""
-        self.author = author
-        r"""Author(s) of database"""
-        self.organization = organization
-        r"""Organization that created the database"""
-        self.license = license
-        r"""License of database"""
-        self.license_url = license_url
-        r"""URL of database license"""
-        self.media = HeaderDict(value_type=Media)
-        r"""Dictionary of media information"""
-        self.raters = HeaderDict(value_type=Rater)
-        r"""Dictionary of raters"""
-        self.schemes = HeaderDict(value_type=Scheme)
-        r"""Dictionary of schemes"""
-        self.splits = HeaderDict(value_type=Split)
-        r"""Dictionary of splits"""
-        self.tables = HeaderDict(
-            value_type=Table, set_callback=self._set_table,
-        )
-        r"""Dictionary of tables"""
 
-    @property
-    def files(self) -> pd.Index:
-        r"""Files referenced in the database.
-
-        Includes files from filewise and segmented tables.
-
-        Returns:
-            files
-
-        """
-        index = pd.Index([], name=define.IndexField.FILE)
-        for table in self.tables.values():
-            index = index.union(table.files.drop_duplicates())
-        return index.drop_duplicates()
-
-    @property
-    def segments(self) -> pd.MultiIndex:
-        r"""Segments referenced in the database.
-
-        Returns:
-            segments
-
-        """
-        index = segmented_index()
-        for table in self.tables.values():
-            if table.is_segmented:
-                index = index.union(table.df.index)
-        assert isinstance(index, pd.MultiIndex)
-        return index.drop_duplicates()
-
-    def drop_files(
-            self,
-            files: typing.Union[
-                str,
-                typing.Sequence[str],
-                typing.Callable[[str], bool],
-            ],
-            num_workers: typing.Optional[int] = 1,
-            verbose: bool = False,
-    ):
-        r"""Drop files from tables.
-
-        Iterate through all tables and remove rows with a reference to
-        listed or matching files.
-
-        Args:
-            files: list of files or condition function
-            num_workers: number of parallel jobs.
-                If ``None`` will be set to the number of processors
-                on the machine multiplied by 5
-            verbose: show progress bar
-
-        """
-        audeer.run_tasks(
-            lambda x: x.drop_files(files, inplace=True),
-            params=[([table], {}) for table in self.tables.values()],
-            num_workers=num_workers,
-            progress_bar=verbose,
-            task_description='Drop files',
+def test_scheme_assign_values():
+
+    db = audformat.testing.create_db(minimal=True)
+    speakers = ['spk1', 'spk2', 'spk3']
+    ages = [33, 44, 55]
+    index = pd.Index(speakers, name='speaker', dtype='string')
+    db.schemes['age'] = audformat.Scheme('int', minimum=0)
+    db['misc'] = audformat.MiscTable(index)
+    db['misc']['age'] = audformat.Column(scheme_id='age')
+    db['misc']['age'].set(ages)
+    db.schemes['scheme'] = audformat.Scheme(labels='misc', dtype='str')
+    db['table'] = audformat.Table(audformat.filewise_index(['f1', 'f2', 'f3']))
+    db['table']['speaker'] = audformat.Column(scheme_id='scheme')
+    db['table']['speaker'].set(speakers)
+
+    assert list(db['table']['speaker'].get()) == speakers
+    assert list(db['table']['speaker'].get(map='age')) == ages
+    assert list(db['table'].get(map={'speaker': 'age'})['age']) == ages
+
+    # Set values not matching scheme
+    bad_values = ['spk4', 'spk5', 'spk6']
+    error_msg = re.escape(
+        "Some value(s) do not match scheme\n"
+        f"{db.schemes['scheme']}\n"
+        "with scheme ID 'scheme':\n"
+        "'spk4', 'spk5', 'spk6'"
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        db['table']['speaker'].set(bad_values)
+    bad_values = list(range(-11, 0))
+    error_msg = re.escape(
+        "Some value(s) do not match scheme\n"
+        f"{db.schemes['age']}\n"
+        "with scheme ID 'age':\n"
+        f"-11, -10, -9, -8, -7, -6, -5, -4, -3, -2, ..."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        db['misc'].extend_index(
+            pd.Index(
+                [f'spk{n}' for n in range(4, 52)],
+                name='speaker',
+                dtype='string',
+            ),
+            inplace=True,
         )
+        db['misc']['age'].set(bad_values)
+
 
-    def drop_tables(
-            self,
-            table_ids: typing.Union[str, typing.Sequence[str]],
-    ):
-        r"""Drop tables by ID.
-
-        Args:
-            table_ids: table IDs to drop
-
-        """
-        if isinstance(table_ids, str):
-            table_ids = [table_ids]
-        for table_id in table_ids:
-            self.tables.pop(table_id)
-
-    def map_files(
-            self,
-            func: typing.Callable[[str], str],
-            num_workers: typing.Optional[int] = 1,
-            verbose: bool = False,
-    ):
-        r"""Apply function to file names in all tables.
-
-        Relies on :meth:`pandas.Index.map`,
-        which can be slow.
-        If speed is crucial,
-        consider to change the index directly.
-        In the following example we prefix every file with a folder:
-
-        .. code-block:: python
-
-            root = '/root/'
-            for table in db.tables.values():
-                if table.is_filewise:
-                    table.df.index = root + table.df.index
-                    table.df.index.name = audformat.define.IndexField.FILE
-                elif len(table.df.index) > 0:
-                    table.df.index.set_levels(
-                        root + table.df.index.levels[0],
-                        audformat.define.IndexField.FILE,
-                        inplace=True,
-                    )
-
-        Args:
-            func: map function
-            num_workers: number of parallel jobs.
-                If ``None`` will be set to the number of processors
-                on the machine multiplied by 5
-            verbose: show progress bar
-
-        """
-        def job(table):
-            if table.is_segmented:
-                table.df.index = table.df.index.map(
-                    lambda x: (func(x[0]), x[1], x[2])
-                )
-            else:
-                table.df.index = table.df.index.map(lambda x: func(x))
-
-        audeer.run_tasks(
-            job,
-            params=[([table], {}) for table in self.tables.values()],
-            num_workers=num_workers,
-            progress_bar=verbose,
-            task_description='Map files',
+@pytest.mark.parametrize(
+    'scheme, values',
+    [
+        (
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+            ),
+            [1.0, 2.0],
+        ),
+        (
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            [1.0, 2.0],
+        ),
+        pytest.param(  # minimum too low
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            [0.0, 2.0],
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # maximum too high
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            [1.0, 3.0],
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        # Finding minimum and maximum in array
+        # should nopt be affected by NaN, see
+        # https://github.com/audeering/audformat/issues/305
+        pytest.param(  # minimum too low
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            np.array([0.0, np.NaN, 2.0]),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # maximum too high
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            np.array([1.0, np.NaN, 3.0]),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        # Make sure we convert None to float
+        # before checking minimum/maximum, see
+        # https://github.com/audeering/audformat/issues/307
+        (
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            np.array([1.0, None, 2.0]),
+        ),
+        pytest.param(  # minimum too low
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            np.array([0.0, None, 2.0]),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # maximum too high
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=1.0,
+                maximum=2.0,
+            ),
+            np.array([1.0, None, 3.0]),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        # Using 0.0 failed before, see
+        # https://github.com/audeering/audformat/issues/304
+        pytest.param(  # minimum too low
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=0.0,
+                maximum=2.0,
+            ),
+            np.array([-1.0, 2.0]),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # maximum too high
+            audformat.Scheme(
+                audformat.define.DataType.FLOAT,
+                minimum=-1.0,
+                maximum=0.0,
+            ),
+            np.array([1.0, 2.0]),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+    ]
+)
+def test_scheme_minimum_maximum(scheme, values):
+
+    db = audformat.testing.create_db(minimal=True)
+    audformat.testing.add_table(
+        db,
+        'table',
+        audformat.define.IndexType.FILEWISE,
+        num_files=len(values),
+    )
+    db.schemes['scheme'] = scheme
+    db['table']['column'] = audformat.Column(scheme_id='scheme')
+
+    table = db['table']
+    column = db['table']['column']
+    column_id = 'column'
+
+    expected_series = pd.Series(
+        values,
+        audformat.filewise_index(table.files),
+        name=column_id,
+        dtype='float64',
+    )
+    column.set(values)
+    pd.testing.assert_series_equal(column.get(), expected_series)
+
+
+def test_scheme_contains():
+
+    db = pytest.DB
+
+    assert 'tests' in db.schemes['string']
+    assert 0.0 in db.schemes['float']
+    assert 1.0 in db.schemes['float']
+    assert -1.0 in db.schemes['float']
+    assert 2.0 not in db.schemes['float']
+    assert -2.0 not in db.schemes['float']
+    assert pd.Timedelta(0.5, unit='s') in db.schemes['time']
+    assert 'label1' in db.schemes['label']
+    assert 'label1' in db.schemes['label_map_str']
+    assert 1 in db.schemes['label_map_int']
+
+    # Misc table
+    # assigned scheme
+    assert 'label1' in db.schemes['label_map_misc']
+    # remove table
+    # db.drop_tables(['misc'])
+    db.misc_tables.pop('misc')
+    assert 'label1' not in db.schemes['label_map_misc']
+    # unassigned scheme
+    scheme = audformat.Scheme(labels='misc', dtype='str')
+    assert 'label1' not in scheme
+
+
+@pytest.mark.parametrize(
+    'dtype, values',
+    [
+        pytest.param(  # bool not supported
+            audformat.define.DataType.BOOL,
+            [True, False],
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        (
+            audformat.define.DataType.DATE,
+            pd.to_datetime(['3/11/2000', '3/12/2000', '3/13/2000']),
+        ),
+        (
+            audformat.define.DataType.INTEGER,
+            [1, 2, 3],
+        ),
+        (
+            audformat.define.DataType.FLOAT,
+            [1.0, 2.0, 3.0],
+        ),
+        (
+            audformat.define.DataType.STRING,
+            ['a', 'b', 'c'],
+        ),
+        (
+            audformat.define.DataType.TIME,
+            pd.to_timedelta(['1s', '2s', '3s']),
+        ),
+    ]
+)
+def test_scheme_dtypes(dtype, values):
+    db = audformat.Database('test')
+    pandas_dtype = audformat.core.common.to_pandas_dtype(dtype)
+    index = pd.Index(values, name='labels', dtype=pandas_dtype)
+    db['misc'] = audformat.MiscTable(index)
+    index = audformat.filewise_index([f'f{idx}' for idx in range(len(values))])
+    db.schemes['scheme'] = audformat.Scheme(dtype=dtype, labels='misc')
+    db['table'] = audformat.Table(index)
+    db['table']['labels'] = audformat.Column(scheme_id='scheme')
+    db['table']['labels'].set(values)
+
+    assert set(db['table']['labels'].get()) == set(values)
+
+
+def test_scheme_errors():
+
+    db = audformat.Database('test')
+
+    # dtype mismatch
+    error_msg = (
+        "Data type is set to 'str', "
+        "but data type of labels is 'int'."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        audformat.Scheme(
+            audformat.define.DataType.STRING,
+            labels=[1, 2, 3],
         )
 
-    def pick_files(
-            self,
-            files: typing.Union[
-                str,
-                typing.Sequence[str],
-                typing.Callable[[str], bool],
+    # unknown type
+    error_msg = (
+        "Bad value 'bad', "
+        "expected one of "
+        "\\['bool', 'date', 'float', 'int', 'object', 'str', 'time'\\]"
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        audformat.Scheme('bad')
+
+    # labels not list or dictionary
+    error_msg = (
+        'Labels must be passed '
+        'as a dictionary, list or ID of a misc table.'
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        audformat.Scheme(labels=set([1, 2, 3]))
+
+    # labels do not have the same type
+    error_msg = (
+        'All labels must be of the same data type.'
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        audformat.Scheme(labels=[1, '2', 3])
+
+    # update labels when scheme has no label
+    error_msg = (
+        'Cannot replace labels when '
+        'scheme does not define labels.'
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        scheme = audformat.Scheme(audformat.define.DataType.INTEGER)
+        scheme.replace_labels(['a', 'b'])
+
+    # misc table needs to define data type
+    error_msg = (
+        "'dtype' has to be provided "
+        "when using a misc table as labels."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        audformat.Scheme(labels='misc')
+
+    # misc table not assigned to a database
+    error_msg = (
+        "The misc table 'misc' used as scheme labels "
+        "needs to be assigned to the database"
+    )
+    scheme = audformat.Scheme(labels='misc', dtype='str')
+    with pytest.raises(ValueError, match=error_msg):
+        db.schemes['misc'] = scheme
+
+    # filewise table used instead of misc table
+    error_msg = (
+        "The table 'table' used as scheme labels "
+        "needs to be a misc table."
+    )
+    db['table'] = audformat.Table(audformat.filewise_index(['f1']))
+    scheme = audformat.Scheme(labels='table', dtype='str')
+    with pytest.raises(ValueError, match=error_msg):
+        db.schemes['misc'] = scheme
+
+    # misc table has different dtype
+    error_msg = (
+        "Data type is set to 'str', "
+        "but data type of labels in misc table is 'int'."
+    )
+    db['misc'] = audformat.MiscTable(pd.Index([0], name='misc'))
+    scheme = audformat.Scheme(labels='misc', dtype='str')
+    with pytest.raises(ValueError, match=error_msg):
+        db.schemes['misc'] = scheme
+
+    # misc table should only contain a one-dimensional index
+    error_msg = (
+        "Index of misc table 'misc' used as scheme labels "
+        "is only allowed to have a single level."
+    )
+    db['misc'] = audformat.MiscTable(
+        pd.MultiIndex.from_arrays(
+            [
+                [1, 2],
+                ['a', 'b'],
             ],
-            num_workers: typing.Optional[int] = 1,
-            verbose: bool = False,
-    ):
-        r"""Pick files from tables.
-
-        Iterate through all tables and keep only rows with a reference
-        to listed files or matching files.
-
-        Args:
-            files: list of files or condition function
-            num_workers: number of parallel jobs.
-                If ``None`` will be set to the number of processors
-                on the machine multiplied by 5
-            verbose: show progress bar
-
-        """
-        audeer.run_tasks(
-            lambda x: x.pick_files(files, inplace=True),
-            params=[([table], {}) for table in self.tables.values()],
-            num_workers=num_workers,
-            progress_bar=verbose,
-            task_description='Pick files',
+            names=['misc-1', 'misc-2'],
         )
+    )
+    scheme = audformat.Scheme(labels='misc', dtype='str')
+    with pytest.raises(ValueError, match=error_msg):
+        db.schemes['misc'] = scheme
+
+    # misc table should not contain duplicates
+    error_msg = (
+        "Index of misc table 'misc' used as scheme labels "
+        "is not allowed to contain duplicates."
+    )
+    db['misc'] = audformat.MiscTable(pd.Index([0, 0], name='misc'))
+    scheme = audformat.Scheme(labels='misc', dtype='int')
+    with pytest.raises(ValueError, match=error_msg):
+        db.schemes['misc'] = scheme
+
+    # cannot assign misc table scheme to itself
+    db['misc'] = audformat.MiscTable(pd.Index([], name='misc'))
+    db.schemes['scheme'] = audformat.Scheme(labels='misc', dtype='object')
+    error_msg = (
+        "Scheme 'scheme' uses misc table 'misc' as labels "
+        "and cannot be used with columns of the same table."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        db['misc']['column'] = audformat.Column(scheme_id='scheme')
+
+    # cannot assign column of a misc table used in a scheme
+    # to a scheme that already uses a misc table
+    db['misc2'] = audformat.MiscTable(pd.Index([], name='misc2'))
+    db.schemes['scheme2'] = audformat.Scheme(labels='misc2', dtype='object')
+    error_msg = (
+        "Since the misc table 'misc2' "
+        "is used as labels in scheme 'scheme2' "
+        "its columns cannot be used with a scheme "
+        "that also uses labels from a misc table."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        db['misc2']['column'] = audformat.Column(scheme_id='scheme')
+
+    # Cannot assign misc table as scheme if one of its column
+    # is linked to a scheme that already uses a misc table
+    db['misc3'] = audformat.MiscTable(pd.Index([], name='misc3'))
+    db['misc3']['column'] = audformat.Column(scheme_id='scheme')
+    scheme = audformat.Scheme(labels='misc3', dtype='object')
+    error_msg = (
+        "The misc table 'misc3' cannot be used as scheme labels "
+        "when one of its columns is assigned to a scheme "
+        "that uses labels from a misc table."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        db.schemes['scheme3'] = scheme
+
+
+def test_scheme_labels():
+
+    # No labels
+    s = audformat.Scheme('str')
+    assert s.labels is None
+    assert s.labels_as_list == []
+
+    # List of labels
+    labels = ['a', 'b']
+    s = audformat.Scheme('str', labels=labels)
+    assert s.labels == labels
+    assert s.labels_as_list == labels
+
+    # Dict of labels
+    labels = {'a': 0, 'b': 1}
+    s = audformat.Scheme('str', labels=labels)
+    assert s.labels == labels
+    assert s.labels_as_list == list(labels)
+
+    # Misc table as labels
+    labels = ['a', 'b']
+    db = audformat.Database('db')
+    index = pd.Index(labels, name='labels', dtype='string')
+    db['labels'] = audformat.MiscTable(index)
+    db.schemes['s'] = audformat.Scheme('str', labels='labels')
+    assert db.schemes['s'].labels == 'labels'
+    assert db.schemes['s'].labels_as_list == labels
+
+
+@pytest.mark.parametrize(
+    'values, labels, new_labels, expected',
+    [
+        (
+            pd.Series(
+                index=audformat.filewise_index(),
+                dtype=pd.CategoricalDtype(),
+            ),
+            [],
+            [],
+            pd.Series(
+                index=audformat.filewise_index(),
+                dtype=pd.CategoricalDtype(),
+            ),
+        ),
+        (
+            pd.Series(
+                index=audformat.filewise_index(),
+                dtype=pd.CategoricalDtype(['a', 'b']),
+            ),
+            ['a', 'b'],
+            ['b', 'c', 'd'],
+            pd.Series(
+                index=audformat.filewise_index(),
+                dtype=pd.CategoricalDtype(['b', 'c', 'd']),
+            ),
+        ),
+        (
+            pd.Series(
+                ['a', 'b'],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['a', 'b']),
+            ),
+            ['a', 'b'],
+            ['a'],
+            pd.Series(
+                ['a', None],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['a']),
+            ),
+        ),
+        (
+            pd.Series(
+                ['a', 'b'],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['a', 'b']),
+            ),
+            ['a', 'b'],
+            ['a', 'b', 'c'],
+            pd.Series(
+                ['a', 'b'],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['a', 'b', 'c']),
+            ),
+        ),
+        (
+            pd.Series(
+                ['a', 'b'],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['a', 'b']),
+            ),
+            ['a', 'b'],
+            ['c'],
+            pd.Series(
+                [None, None],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['c']),
+            ),
+        ),
+        (
+            pd.Series(
+                ['a', 'b'],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype(['a', 'b']),
+            ),
+            ['a', 'b'],
+            [],
+            pd.Series(
+                [None, None],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype([]),
+            ),
+        ),
+        (
+            pd.Series(
+                [0, 1],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype([0, 1]),
+            ),
+            {0: 'a', 1: 'b'},
+            {1: {'b': 'B'}, 2: {'c': 'C'}},
+            pd.Series(
+                [None, 1],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype([1, 2]),
+            ),
+        ),
+        (
+            pd.Series(
+                [0, 1],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype([0, 1]),
+            ),
+            {0: 'a', 1: 'b'},
+            [1, 2],
+            pd.Series(
+                [None, 1],
+                index=audformat.filewise_index(['f1', 'f2']),
+                dtype=pd.CategoricalDtype([1, 2]),
+            ),
+        ),
+        # error: dtype of labels does not match
+        pytest.param(
+            pd.Series(
+                index=audformat.filewise_index(),
+                dtype=pd.CategoricalDtype(),
+            ),
+            ['a', 'b'],
+            [0, 1],
+            pd.Series(
+                index=audformat.filewise_index(),
+                dtype=pd.CategoricalDtype(),
+            ),
+            marks=pytest.mark.xfail(raises=ValueError),
+        )
+    ]
+)
+def test_replace_labels(values, labels, new_labels, expected):
+
+    db = audformat.testing.create_db(minimal=True)
+    db.schemes['scheme'] = audformat.Scheme(labels=labels)
+    db['table'] = audformat.Table(index=values.index)
+    db['table']['columns'] = audformat.Column(scheme_id='scheme')
+    db['table']['columns'].set(values)
+    db.schemes['scheme'].replace_labels(new_labels)
+    pd.testing.assert_series_equal(
+        db['table']['columns'].get(),
+        expected,
+        check_names=False,
+    )
+
+
+def test_replace_labels_misc_table():
+
+    db = audformat.testing.create_db(minimal=True)
+    db['labels'] = audformat.MiscTable(
+        pd.Index(
+            ['a', 'b', 'c', 'd'],
+            dtype='string',
+            name='idx',
+        )
+    )
 
-    def pick_tables(
-            self,
-            table_ids: typing.Union[str, typing.Sequence[str]],
-    ):
-        r"""Pick tables by ID.
-
-        Args:
-            table_ids: table IDs to pick
-
-        """
-        if isinstance(table_ids, str):
-            table_ids = [table_ids]
-        drop_ids = []
-        for table_id in list(self.tables):
-            if table_id not in table_ids:
-                drop_ids.append(table_id)
-        self.drop_tables(drop_ids)
-
-    def save(
-            self,
-            root: str,
-            *,
-            name: str = 'db',
-            indent: int = 2,
-            storage_format: define.TableStorageFormat = (
-                define.TableStorageFormat.CSV
-            ),
-            update_other_formats: bool = True,
-            header_only: bool = False,
-            num_workers: typing.Optional[int] = 1,
-            verbose: bool = False,
-    ):
-        r"""Save database to disk.
-
-        Creates a header ``<root>/<name>.yaml``
-        and for every table a file ``<root>/<name>.<table-id>.[csv,pkl]``.
-
-        Existing files will be overwritten.
-        If ``update_other_formats`` is provided,
-        it will overwrite all existing files in others formats as well.
-
-        Args:
-            root: root directory (possibly created)
-            name: base name of files
-            indent: indent size
-            storage_format: storage format of tables.
-                See :class:`audformat.define.TableStorageFormat`
-                for available formats
-            update_other_formats: if ``True`` it will not only save
-                to the given ``storage_format``,
-                but update all files stored in other storage formats as well
-            header_only: store header only
-            num_workers: number of parallel jobs.
-                If ``None`` will be set to the number of processors
-                on the machine multiplied by 5
-            verbose: show progress bar
-
-        """
-        root = audeer.mkdir(root)
-
-        ext = '.yaml'
-        header_path = os.path.join(root, name + ext)
-        with open(header_path, 'w') as fp:
-            self.dump(fp, indent=indent)
-
-        if not header_only:
-
-            def job(table_id, table):
-                table_path = os.path.join(root, name + '.' + table_id)
-                table.save(
-                    table_path,
-                    storage_format=storage_format,
-                    update_other_formats=update_other_formats,
-                )
-
-            audeer.run_tasks(
-                job,
-                params=[
-                    ([table_id, table], {})
-                    for table_id, table in self.tables.items()
-                ],
-                num_workers=num_workers,
-                progress_bar=verbose,
-                task_description='Save tables',
-            )
-
-    def __contains__(
-            self,
-            table_id: str,
-    ) -> bool:
-        r"""Check if table exists.
-
-        Args:
-            table_id: table identifier
-
-        """
-        return table_id in self.tables
-
-    def __getitem__(
-            self,
-            table_id: str,
-    ) -> Table:
-        r"""Get table from database.
-
-        Args:
-            table_id: table identifier
-
-        """
-        return self.tables[table_id]
-
-    def __eq__(
-            self,
-            other: 'Database',
-    ) -> bool:
-        if self.dump() != other.dump():
-            return False
-        for table_id in self.tables:
-            if self[table_id] != other[table_id]:
-                return False
-        return True
-
-    def __setitem__(
-            self,
-            table_id: str,
-            table: Table,
-    ) -> Table:
-        r"""Add table to database.
-
-        Args:
-            table_id: table identifier
-            table: the table
-
-        Raises:
-            BadIdError: if table has a ``split_id`` or ``media_id``,
-                which is not specified in the underlying database
-
-        """
-        self.tables[table_id] = table
-        return table
-
-    @staticmethod
-    def load(
-            root: str,
-            *,
-            name: str = 'db',
-            load_data: bool = True,
-            num_workers: typing.Optional[int] = 1,
-            verbose: bool = False,
-    ) -> 'Database':
-        r"""Load database from disk.
-
-        Expects a header ``<root>/<name>.yaml``
-        and for every table a file ``<root>/<name>.<table-id>.[csv|pkl]``
-        Media files should be located under ``root``.
-
-        Args:
-            root: root directory
-            name: base name of header and table files
-            load_data: if ``False`` :class:`audformat.Table`
-                will contain empty tables
-            num_workers: number of parallel jobs.
-                If ``None`` will be set to the number of processors
-                on the machine multiplied by 5
-            verbose: show progress bar
-
-        Returns:
-            database object
-
-        """
-        ext = '.yaml'
-        root = audeer.safe_path(root)
-        path = os.path.join(root, name + ext)
-
-        if not os.path.exists(path):
-            raise FileNotFoundError(path)
-
-        with open(path, 'r') as fp:
-
-            header = yaml.load(fp, Loader=yaml.Loader)
-            db = Database.load_header_from_yaml(header)
-
-            if 'tables' in header and header['tables'] and load_data:
-
-                def job(table_id):
-                    table = db[table_id]
-                    path = os.path.join(root, name + '.' + table_id)
-                    table.load(path)
-
-                audeer.run_tasks(
-                    job,
-                    params=[
-                        ([table_id], {}) for table_id in header['tables']
-                    ],
-                    num_workers=num_workers,
-                    progress_bar=verbose,
-                    task_description='Load tables',
-                )
-
-        return db
-
-    @staticmethod
-    def load_header_from_yaml(header: dict) -> 'Database':
-        r"""Load database header from YAML.
-
-        Args:
-            header: YAML header definition
-
-        Returns:
-            database object
-
-        """
-        # for backward compatibility
-        if len(header) == 1:  # pragma: no cover
-            id = next(iter(header))
-            header = header[id]
-            header['name'] = id
-
-        db = Database(
-            name=header['name'],
-            source=header['source'],
-            usage=header['usage'])
-        db.from_dict(header, ignore_keys=['media', 'raters', 'schemes',
-                                          'tables', 'splits'])
-
-        if 'media' in header and header['media']:
-            for media_id, media_d in header['media'].items():
-                media = Media()
-                media.from_dict(media_d)
-                db.media[media_id] = media
-
-        if 'raters' in header and header['raters']:
-            for rater_id, rater_d in header['raters'].items():
-                rater = Rater()
-                rater.from_dict(rater_d)
-                db.raters[rater_id] = rater
-
-        if 'schemes' in header and header['schemes']:
-            for scheme_id, scheme_d in header['schemes'].items():
-                scheme = Scheme()
-                scheme.from_dict(scheme_d)
-                db.schemes[scheme_id] = scheme
-
-        if 'splits' in header and header['splits']:
-            for split_id, split_d in header['splits'].items():
-                split = Split()
-                split.from_dict(split_d)
-                db.splits[split_id] = split
-
-        if 'tables' in header and header['tables']:
-            for table_id, table_d in header['tables'].items():
-                table = Table()
-                table.from_dict(table_d, ignore_keys=['is_segmented',
-                                                      'columns'])
-                if 'columns' in table_d and table_d['columns']:
-                    tmp_callback = table.columns.set_callback
-                    table.columns.set_callback = None
-                    for column_id, column_d in \
-                            table_d['columns'].items():
-                        column = Column()
-                        column.from_dict(
-                            column_d, ignore_keys=['has_confidence']
-                        )
-                        column._id = column_id
-                        column._table = table
-                        table.columns[column_id] = column
-
-                        # for backward compatibility we insert
-                        # confidences as a regular column
-                        if 'has_confidence' in column_d:  # pragma: no cover
-                            column = Column()
-                            column._id = '@' + column_id
-                            column._table = table
-                            table.columns['@' + column_id] = column
-
-                    table.columns.set_callback = tmp_callback
-                db[table_id] = table
-
-        return db
-
-    def _set_table(
-            self,
-            table_id: str,
-            table: Table,
-    ) -> Table:
-        if table.split_id is not None and table.split_id not in self.splits:
-            raise BadIdError('split', table.split_id, self.splits)
-        if table.media_id is not None and table.media_id not in self.media:
-            raise BadIdError('media', table.media_id, self.media)
-        table._db = self
-        table._id = table_id
-        return table
+    # non-assigned scheme
+    scheme = audformat.Scheme(
+        audformat.define.DataType.STRING,
+        labels='labels',
+    )
+    assert scheme.labels == 'labels'
+    assert scheme._labels_to_dict() == {}
+
+    # replace with non-existing misc table scheme
+    # and back again
+    scheme.replace_labels('misc-non-existing')
+    scheme.replace_labels('labels')
+
+    # assigned scheme
+    db.schemes['scheme'] = scheme
+    assert scheme.labels == 'labels'
+    assert scheme._labels_to_dict() == {'a': {}, 'b': {}, 'c': {}, 'd': {}}
+
+    # use scheme in (miscellaneous) table
+    db['table'] = audformat.Table(
+        index=audformat.filewise_index(['f1', 'f2', 'f3', 'f4']),
+    )
+    db['table']['column'] = audformat.Column(scheme_id='scheme')
+    db['table']['column'].set(['a', 'b', 'c', 'd'])
+    db['misc'] = audformat.MiscTable(
+        index=pd.Index(
+            [0, 1, 2, 3],
+            name='idx',
+        ),
+    )
+    db['misc']['column'] = audformat.Column(scheme_id='scheme')
+    db['misc']['column'].set(['a', 'b', 'c', 'd'])
+
+    # replace with new misc table scheme
+    db['labels-new'] = audformat.MiscTable(
+        pd.Index(
+            ['b', 'c', 'd', 'e'],
+            dtype='string',
+            name='idx',
+        )
+    )
+    scheme.replace_labels('labels-new')
+    assert scheme.labels == 'labels-new'
+    assert scheme._labels_to_dict() == {'b': {}, 'c': {}, 'd': {}, 'e': {}}
+    expected = [np.NaN, 'b', 'c', 'd']
+    assert list(db['table']['column'].get().values) == expected
+    assert list(db['misc']['column'].get().values) == expected
+
+    # extend labels
+    db['labels-new'].extend_index(
+        pd.Index(
+            ['f'],
+            dtype='string',
+            name='idx',
+        ),
+        inplace=True,
+    )
+    expected = {'b': {}, 'c': {}, 'd': {}, 'e': {}, 'f': {}}
+    assert scheme._labels_to_dict() == expected
+    assert 'f' in db['table']['column'].get().dtype.categories
+    assert 'f' in db['misc']['column'].get().dtype.categories
+
+    # pick labels
+    db['labels-new'].pick_index(
+        pd.Index(
+            ['c', 'd', 'e'],
+            dtype='string',
+            name='idx',
+        ),
+        inplace=True,
+    )
+    assert scheme._labels_to_dict() == {'c': {}, 'd': {}, 'e': {}}
+    expected = [np.NaN, np.NaN, 'c', 'd']
+    assert list(db['table']['column'].get().values) == expected
+    assert list(db['misc']['column'].get().values) == expected
+
+    # drop labels
+    db['labels-new'].drop_index(
+        pd.Index(
+            ['c'],
+            dtype='string',
+            name='idx',
+        ),
+        inplace=True,
+    )
+    assert scheme._labels_to_dict() == {'d': {}, 'e': {}}
+    expected = [np.NaN, np.NaN, np.NaN, 'd']
+    assert list(db['table']['column'].get().values) == expected
+    assert list(db['misc']['column'].get().values) == expected
+
+    # replace with dictionary
+    scheme.replace_labels({'e': {}})
+    assert scheme.labels == {'e': {}}
+    assert scheme._labels_to_dict() == {'e': {}}
+    expected = [np.NaN, np.NaN, np.NaN, np.NaN]
+    assert list(db['table']['column'].get().values) == expected
+    assert list(db['misc']['column'].get().values) == expected
+
+    # replace again with misc table
+    scheme.replace_labels('labels')
+    assert scheme.labels == 'labels'
+    assert scheme._labels_to_dict() == {'a': {}, 'b': {}, 'c': {}, 'd': {}}
+
+    # replace with list
+    scheme.replace_labels(['a', 'b'])
+    assert scheme.labels == ['a', 'b']
+    assert scheme._labels_to_dict() == {'a': {}, 'b': {}}
+
+    # replace with non-existing misc table scheme
+    error_msg = (
+        "The misc table 'misc-non-existing' used as scheme labels "
+        "needs to be assigned to the database."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        scheme.replace_labels('misc-non-existing')
+
+    # replace labels with a misc table that
+    # has a column that already links a misc table
+    scheme.replace_labels('labels')
+    db['labels-new']['column'] = audformat.Column(scheme_id='scheme')
+    error_msg = (
+        "The misc table 'labels-new' cannot be used as scheme labels "
+        "when one of its columns is assigned to a scheme "
+        "that uses labels from a misc table."
+    )
+    with pytest.raises(ValueError, match=error_msg):
+        scheme.replace_labels('labels-new')
```

### Comparing `audformat-0.9.8/audformat/core/errors.py` & `audformat-1.0.0/audformat/core/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 import typing
 
 
-class BadValueError(ValueError):
-    """Raised when a value is not in a list of pre-defined strings.
+class BadIdError(ValueError):
+    r"""Raised when a field identifier is unknown.
 
     Args:
-        invalid_value: value causing the error
-        valid_values: list of valid strings
+        name: name of the field
+        invalid_id: identifier causing the error
+        dictionary: dictionary with valid identifiers
 
     """
-    def __init__(self, invalid_value: str, valid_values: typing.Sequence[str]):
+    def __init__(self, name: str, invalid_id: str, dictionary: dict):
+        if not dictionary:
+            message = (
+                f"Bad {name} ID '{invalid_id}', "
+                f"no {name} objects defined yet"
+            )
+        else:
+            message = (
+                f"Bad {name} ID '{invalid_id}', "
+                f"expected one of {list(dictionary)}"
+            )
+        super().__init__(message)
+
+
+class BadKeyError(KeyError):
+    """Raised when a key is not found.
+
+    Args:
+        invalid_key: value causing the error
+        valid_keys: list of valid strings
+
+    """
+    def __init__(self, invalid_key: str, valid_keys: typing.Sequence[str]):
         message = (
-            f"Bad value '{invalid_value}', "
-            f"expected one of {list(valid_values)}"
+            f"Bad key '{invalid_key}', "
+            f"expected one of {list(valid_keys)}"
         )
         super().__init__(message)
 
 
-class BadTypeError(ValueError):
+class BadTypeError(TypeError):
     r"""Raised when a value has an unexpected type.
 
     Args:
         invalid_value: value causing the error
         expected_type: expected value type
 
     """
@@ -29,28 +52,38 @@
         message = (
             f"Bad type '{type(invalid_value)}', "
             f"expected '{expected_type}'"
         )
         super().__init__(message)
 
 
-class BadIdError(ValueError):
-    r"""Raised when a field identifier is unknown.
+class BadValueError(ValueError):
+    """Raised when a value is not in a list of pre-defined strings.
 
     Args:
-         name: name of the field
-         invalid_id: identifier causing the error
-         dictionary: dictionary with valid identifiers
+        invalid_value: value causing the error
+        valid_values: list of valid strings
 
     """
-    def __init__(self, name: str, invalid_id: str, dictionary: dict):
-        if not dictionary:
-            message = (
-                f"Bad {name} ID '{invalid_id}', "
-                f"no {name} objects defined yet"
-            )
-        else:
-            message = (
-                f"Bad {name} ID '{invalid_id}', "
-                f"expected one of {list(dictionary)}"
-            )
+    def __init__(self, invalid_value: str, valid_values: typing.Sequence[str]):
+        message = (
+            f"Bad value '{invalid_value}', "
+            f"expected one of {list(valid_values)}"
+        )
         super().__init__(message)
+
+
+class TableExistsError(KeyError):
+    r"""If a table of another type with same ID exists already.
+
+    Args:
+        table_type: table type
+        table_id: table identifier
+
+    """
+    def __init__(self, table_type: str, table_id: str):
+        KeyError(
+            f"There is already a "
+            f"{table_type} "
+            f"table with ID "
+            f"'{table_id}'."
+        )
```

### Comparing `audformat-0.9.8/audformat/core/index.py` & `audformat-1.0.0/audformat/core/index.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 
 import numpy as np
 import pandas as pd
 
 from audformat.core import define
+from audformat.core import utils
 from audformat.core.typing import (
     Files,
     Timestamps,
 )
 
 
 def is_scalar(value: typing.Any) -> bool:
@@ -31,30 +32,113 @@
     try:
         return pd.to_timedelta(times, unit='s')
     except ValueError:  # catches values like '1s'
         return pd.to_timedelta(times)
 
 
 def assert_index(
-    obj: typing.Union[pd.Index, pd.Series, pd.DataFrame]
+    obj: typing.Union[pd.Index, pd.Series, pd.DataFrame],
 ):
     r"""Assert object is conform to :ref:`table specifications
     <data-tables:Tables>`.
 
+    This does not check for duplicates in the index.
+    If you need that check
+    use :func:`audformat.assert_no_duplicates` in addition.
+
     Args:
         obj: object
 
     Raises:
         ValueError: if not conform to
             :ref:`table specifications <data-tables:Tables>`
 
     """
     if isinstance(obj, (pd.Series, pd.DataFrame)):
         obj = obj.index
 
+    num = len(obj.names)
+
+    if num != 1 and num != 3:
+        raise ValueError(
+            'Index not conform to audformat. '
+            f'Found '
+            f'{num} '
+            f'levels, but expected 1 or 3 levels.'
+        )
+
+    if num == 1:
+        if obj.names[0] != define.IndexField.FILE:
+            raise ValueError(
+                'Index not conform to audformat. '
+                'Found single level with name '
+                f'{obj.names[0]}, '
+                f'but expected name '
+                f"'{define.IndexField.FILE}'."
+            )
+        if not pd.api.types.is_string_dtype(obj.dtype):
+            raise ValueError(
+                "Index not conform to audformat. "
+                "Level 'file' must contain values of type 'string'."
+            )
+    elif num == 3:
+        if not (
+                obj.names[0] == define.IndexField.FILE
+                and obj.names[1] == define.IndexField.START
+                and obj.names[2] == define.IndexField.END
+        ):
+            expected_names = [
+                define.IndexField.FILE,
+                define.IndexField.START,
+                define.IndexField.END,
+            ]
+            raise ValueError(
+                'Index not conform to audformat. '
+                'Found three levels with names '
+                f'{obj.names}, '
+                f'but expected names '
+                f'{expected_names}.'
+            )
+        if not pd.api.types.is_string_dtype(obj.levels[0].dtype):
+            raise ValueError(
+                "Index not conform to audformat. "
+                "Level 'file' must contain values of type 'string'."
+            )
+        if not pd.api.types.is_timedelta64_dtype(obj.levels[1].dtype):
+            raise ValueError(
+                "Index not conform to audformat. "
+                "Level 'start' must contain values of type 'timedelta64[ns]'."
+            )
+        if not pd.api.types.is_timedelta64_dtype(obj.levels[2].dtype):
+            raise ValueError(
+                "Index not conform to audformat. "
+                "Level 'end' must contain values of type 'timedelta64[ns]'."
+            )
+
+
+def assert_no_duplicates(
+    obj: typing.Union[pd.Index, pd.Series, pd.DataFrame],
+):
+    r"""Assert object contains no duplicates in its index.
+
+    The :ref:`table specifications <data-tables:Tables>`
+    allow no duplicated index entries.
+    To save time we do not test for this
+    in :func:`audformat.assert_index`.
+
+    Args:
+        obj: object
+
+    Raises:
+        ValueError: if duplicates are found
+
+    """
+    if isinstance(obj, (pd.Series, pd.DataFrame)):
+        obj = obj.index
+
     if obj.has_duplicates:
         max_display = 10
         duplicates = obj[obj.duplicated()]
         msg_tail = '\n...' if len(duplicates) > max_display else ''
         msg_duplicates = '\n'.join(
             [
                 str(duplicate) for duplicate
@@ -63,52 +147,14 @@
         )
         raise ValueError(
             'Index not conform to audformat. '
             'Found duplicates:\n'
             f'{msg_duplicates}{msg_tail}'
         )
 
-    num = len(obj.names)
-
-    if num != 1 and num != 3:
-        raise ValueError(
-            'Index not conform to audformat. '
-            f'Found '
-            f'{num} '
-            f'levels, but expected 1 or 3 levels.'
-        )
-
-    if num == 1 and not (
-            obj.names[0] == define.IndexField.FILE
-    ):
-        raise ValueError(
-            'Index not conform to audformat. '
-            'Found single level with name '
-            f'{obj.names[0]}, '
-            f'but expected name '
-            f"'{define.IndexField.FILE}'."
-        )
-    elif num == 3 and not (
-            obj.names[0] == define.IndexField.FILE
-            and obj.names[1] == define.IndexField.START
-            and obj.names[2] == define.IndexField.END
-    ):
-        expected_names = [
-            define.IndexField.FILE,
-            define.IndexField.START,
-            define.IndexField.END,
-        ]
-        raise ValueError(
-            'Index not conform to audformat. '
-            'Found three levels with names '
-            f'{obj.names}, '
-            f'but expected names '
-            f'{expected_names}.'
-        )
-
 
 def filewise_index(
         files: Files = None,
 ) -> pd.Index:
     r"""Creates a filewise index.
 
     Index is conform to :ref:`table specifications <data-tables:Tables>`.
@@ -118,46 +164,53 @@
 
     Returns:
         filewise index
 
     Raises:
         ValueError: if created index contains duplicates
 
-    Example:
+    Examples:
         >>> filewise_index(['a.wav', 'b.wav'])
-        Index(['a.wav', 'b.wav'], dtype='object', name='file')
+        Index(['a.wav', 'b.wav'], dtype='string', name='file')
 
     """
     if files is None:
         files = []
 
     files = to_array(files)
-    index = pd.Index(files, name=define.IndexField.FILE)
+    index = pd.Index(
+        files,
+        name=define.IndexField.FILE,
+        dtype='string',
+    )
     assert_index(index)
 
     return index
 
 
 def index_type(
-        obj: typing.Union[pd.Index, pd.Series, pd.DataFrame]
+        obj: typing.Union[pd.Index, pd.Series, pd.DataFrame],
 ) -> define.IndexType:
     r"""Derive index type.
 
+    Possible return values are given by
+    :class:`audformat.define.IndexType`.
+
     Args:
         obj: object conform to
             :ref:`table specifications <data-tables:Tables>`
 
     Returns:
         table type
 
     Raises:
         ValueError: if not conform to
             :ref:`table specifications <data-tables:Tables>`
 
-    Example:
+    Examples:
         >>> index_type(filewise_index())
         'filewise'
         >>> index_type(segmented_index())
         'segmented'
 
     """
     if isinstance(obj, (pd.Series, pd.DataFrame)):
@@ -167,14 +220,73 @@
 
     if len(obj.names) == 1:
         return define.IndexType.FILEWISE
     else:
         return define.IndexType.SEGMENTED
 
 
+def is_filewise_index(
+        obj: typing.Union[pd.Index, pd.Series, pd.DataFrame],
+) -> bool:
+    r"""Check if object has a filewise index.
+
+    Returns ``True`` if index is a filewise index conform to
+    :ref:`table specifications <data-tables:Tables>`.
+
+    Args:
+        obj: object
+
+    Returns:
+        ``True`` if index is filewise, otherwise ``False``
+
+    Examples:
+        >>> is_filewise_index(filewise_index())
+        True
+        >>> is_filewise_index(pd.Index([]))
+        False
+
+    """
+    if not isinstance(obj, pd.Index):
+        obj = obj.index
+
+    return len(obj.names) == 1 and obj.names[0] == define.IndexField.FILE
+
+
+def is_segmented_index(
+        obj: typing.Union[pd.Index, pd.Series, pd.DataFrame],
+) -> bool:
+    r"""Check if object has a segmented index.
+
+    Returns ``True`` if index is a segmented index conform to
+    :ref:`table specifications <data-tables:Tables>`.
+
+    Args:
+        obj: object
+
+    Returns:
+        ``True`` if index is segmented, otherwise ``False``
+
+    Examples:
+        >>> is_segmented_index(segmented_index())
+        True
+        >>> is_segmented_index(pd.Index([]))
+        False
+
+    """
+    if not isinstance(obj, pd.Index):
+        obj = obj.index
+
+    return (
+        len(obj.names) == 3
+        and obj.names[0] == define.IndexField.FILE
+        and obj.names[1] == define.IndexField.START
+        and obj.names[2] == define.IndexField.END
+    )
+
+
 def segmented_index(
         files: Files = None,
         starts: Timestamps = None,
         ends: Timestamps = None,
 ) -> pd.Index:
     r"""Create segmented index.
 
@@ -197,15 +309,15 @@
 
     Raises:
         ValueError: if created index contains duplicates
 
     Raises:
         ValueError: if ``files``, ``start`` and ``ends`` differ in size
 
-    Example:
+    Examples:
         >>> segmented_index('a.wav', 0, 1.1)
         MultiIndex([('a.wav', '0 days', '0 days 00:00:01.100000')],
                    names=['file', 'start', 'end'])
         >>> segmented_index('a.wav', '0ms', '1ms')
         MultiIndex([('a.wav', '0 days', '0 days 00:00:00.001000')],
                    names=['file', 'start', 'end'])
         >>> segmented_index(['a.wav', 'b.wav'])
@@ -250,10 +362,11 @@
     index = pd.MultiIndex.from_arrays(
         [files, to_timedelta(starts), to_timedelta(ends)],
         names=[
             define.IndexField.FILE,
             define.IndexField.START,
             define.IndexField.END,
         ])
+    index = utils.set_index_dtypes(index, {define.IndexField.FILE: 'string'})
     assert_index(index)
 
     return index
```

### Comparing `audformat-0.9.8/audformat/core/media.py` & `audformat-1.0.0/audformat/core/media.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,56 +6,58 @@
 
 class Media(HeaderBase):
     r"""Media information.
 
     File ``format`` is always converted to lower case.
 
     Args:
-        type: media type
+        type: media type,
+            see :class:`audformat.define.MediaType`
+            for available media types
         format: file format (e.g. 'wav', 'flac', 'mp4')
         sampling_rate: audio sampling rate in Hz
         channels: number of audio channels
         bit_depth: audio bit depth
         video_fps: video rate in frames per seconds
         video_resolution: video resolution in pixels (e.g. ``[800, 600]``)
         video_channels: number of channels per pixel (e.g. 3 for RGB)
         video_depth: number of bits per video channel
         description: media description
         meta: additional meta fields
 
     Raises:
         BadValueError: if an invalid ``type`` is passed
 
-    Example:
+    Examples:
         >>> Media(
         ...     type=define.MediaType.AUDIO,
         ...     format='wav',
         ...     sampling_rate=16000,
         ...     channels=2,
         ... )
         {type: audio, format: wav, channels: 2, sampling_rate: 16000}
 
     """
     def __init__(
             self,
-            type: define.MediaType = define.MediaType.OTHER,
+            type: str = define.MediaType.OTHER,
             *,
             format: str = None,
             sampling_rate: int = None,
             channels: int = None,
             bit_depth: int = None,
             video_fps: int = None,
             video_resolution: typing.Sequence[int] = None,
             video_channels: int = None,
             video_depth: int = None,
             description: str = None,
             meta: dict = None,
     ):
         super().__init__(description=description, meta=meta)
-        define.MediaType.assert_has_attribute_value(type)
+        define.MediaType._assert_has_attribute_value(type)
 
         self.type = type
         r"""Media type"""
         self.format = None if format is None else str(format).lower()
         r"""File format"""
 
         self.channels = channels
```

### Comparing `audformat-0.9.8/audformat/core/rater.py` & `audformat-1.0.0/audformat/core/rater.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 from audformat.core.common import HeaderBase
 
 
 class Rater(HeaderBase):
     r"""A rater is the author of an annotation.
 
     Args:
-        type: rater type
+        type: rater type,
+            see :class:`audformat.define.RaterType`
+            for available rater types
         description: rater description
         meta: additional meta fields
 
     Raises:
         BadValueError: if an invalid ``type`` is passed
 
 
-    Example:
+    Examples:
         >>> Rater(define.RaterType.HUMAN)
         {type: human}
 
     """
     def __init__(
             self,
-            type: define.RaterType = define.RaterType.HUMAN,
+            type: str = define.RaterType.HUMAN,
             *,
             description: str = None,
             meta: dict = None,
     ):
         super().__init__(description=description, meta=meta)
-        define.RaterType.assert_has_attribute_value(type)
+        define.RaterType._assert_has_attribute_value(type)
         self.type = type
         r"""Rater type"""
```

### Comparing `audformat-0.9.8/audformat/core/split.py` & `audformat-1.0.0/audformat/core/split.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import typing
-
 from audformat.core import define
 from audformat.core.common import HeaderBase
 
 
 class Split(HeaderBase):
     r"""Database split.
 
     Defines if a subset of a database should be used for training,
     development or testing.
 
     Args:
-        type: split type
+        type: split type,
+            see :class:`audformat.define.SplitType`
+            for available split types
         description: split description
         meta: additional meta fields
 
     Raises:
         BadValueError: if an invalid ``type`` is passed
 
-    Example:
+    Examples:
         >>> Split(define.SplitType.TEST)
         {type: test}
 
     """
     def __init__(
             self,
-            type: define.SplitType = define.SplitType.OTHER,
+            type: str = define.SplitType.OTHER,
             *,
             description: str = None,
             meta: dict = None,
     ):
         super().__init__(description=description, meta=meta)
-        define.SplitType.assert_has_attribute_value(type)
+        define.SplitType._assert_has_attribute_value(type)
         self.type = type
         r"""Split type"""
```

### Comparing `audformat-0.9.8/audformat.egg-info/SOURCES.txt` & `audformat-1.0.0/audformat.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 .gitignore
+.pre-commit-config.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
+.github/workflows/doc.yml
+.github/workflows/flake8.yml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 audformat/__init__.py
 audformat.egg-info/PKG-INFO
 audformat.egg-info/SOURCES.txt
 audformat.egg-info/dependency_links.txt
 audformat.egg-info/requires.txt
 audformat.egg-info/top_level.txt
 audformat/core/__init__.py
+audformat/core/attachment.py
 audformat/core/column.py
 audformat/core/common.py
+audformat/core/conftest.py
 audformat/core/database.py
 audformat/core/define.py
 audformat/core/errors.py
 audformat/core/index.py
 audformat/core/media.py
 audformat/core/rater.py
 audformat/core/scheme.py
@@ -29,43 +34,57 @@
 audformat/core/testing.py
 audformat/core/typing.py
 audformat/core/utils.py
 audformat/define/__init__.py
 audformat/errors/__init__.py
 audformat/testing/__init__.py
 audformat/utils/__init__.py
+benchmarks/benchmark_union.py
 docs/accessing-data.rst
-docs/api-define.rst
-docs/api-errors.rst
-docs/api-testing.rst
-docs/api-utils.rst
-docs/api.rst
 docs/changelog.rst
 docs/combine-tables.rst
 docs/conf.py
 docs/contributing.rst
 docs/create-database.rst
 docs/data-conventions.rst
 docs/data-example.rst
 docs/data-format.rst
 docs/data-header.rst
 docs/data-introduction.rst
+docs/data-misc-tables.rst
 docs/data-tables.rst
 docs/emodb-example.rst
 docs/genindex.rst
 docs/index.rst
 docs/install.rst
 docs/map-scheme.rst
 docs/requirements.txt
-docs/pics/audformat.dot
-docs/pics/tables.dot
-docs/pics/workflow.dot
+docs/update-database.rst
+docs/_templates/autosummary/base.rst
+docs/_templates/autosummary/class.rst
+docs/_templates/autosummary/function.rst
+docs/api/audformat.define.rst
+docs/api/audformat.errors.rst
+docs/api/audformat.rst
+docs/api/audformat.testing.rst
+docs/api/audformat.utils.rst
+docs/api-src/audformat.define.rst
+docs/api-src/audformat.errors.rst
+docs/api-src/audformat.rst
+docs/api-src/audformat.testing.rst
+docs/api-src/audformat.utils.rst
+docs/pics/audformat-database.dot
+docs/pics/audformat-misc-table.dot
+docs/pics/audformat-table.dot
 tests/conftest.py
 tests/requirements.txt
+tests/test_attachment.py
 tests/test_column.py
+tests/test_common.py
 tests/test_database.py
 tests/test_eq.py
 tests/test_errors.py
 tests/test_index.py
+tests/test_misc_table.py
 tests/test_scheme.py
 tests/test_table.py
 tests/test_utils.py
```

### Comparing `audformat-0.9.8/docs/accessing-data.rst` & `audformat-1.0.0/docs/accessing-data.rst`

 * *Files identical despite different names*

### Comparing `audformat-0.9.8/docs/combine-tables.rst` & `audformat-1.0.0/docs/combine-tables.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _combine-tables:
+
 Combine tables
 ==============
 
 It can happen that labels in your database are stored
 in tables of different type as some labels belong to the whole file,
 others don't. The following examples highlights this with the labels
 for age and likability:
@@ -80,7 +82,51 @@
     df_age = db['age'].get(df_likability.index)
 
 Which results in the following :class:`pandas.DataFrame`:
 
 .. jupyter-execute::
 
     df_age
+
+So far we have combined tables using the ``+`` operator.
+The result is a table that is no longer attached to a database.
+That means that meta information about the media
+or referenced schemes is discarded.
+If you want to keep this information,
+you can use :meth:`audformat.Table.update`,
+which also works across databases,
+as we will demonstrate with the following example.
+
+First we create a second database
+and add a gender scheme:
+
+.. jupyter-execute::
+
+    db2 = audformat.testing.create_db(minimal=True)
+    db2.schemes['gender'] = audformat.Scheme(
+        labels=['female', 'male'],
+    )
+    db2.schemes
+
+Next, we add a table and fill in some gender information:
+
+.. jupyter-execute::
+
+    audformat.testing.add_table(
+        db2,
+        table_id='gender_and_age',
+        index_type=audformat.define.IndexType.FILEWISE,
+        columns='gender',
+        num_files=[2, 3, 4],
+    ).get()
+
+Now, we update the table with age values from the other database.
+
+.. jupyter-execute::
+
+    db2['gender_and_age'].update(db['age']).get()
+
+And also copies the according scheme to the database:
+
+.. jupyter-execute::
+
+    db2.schemes
```

### Comparing `audformat-0.9.8/docs/create-database.rst` & `audformat-1.0.0/docs/create-database.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _create-a-database:
+
 Create a database
 =================
 
 The following examples show you
 how to create a :class:`audformat.Database`
 and store it to the disk.
```

### Comparing `audformat-0.9.8/docs/data-conventions.rst` & `audformat-1.0.0/docs/data-conventions.rst`

 * *Files 24% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 =============================  =============================================
 Name                           Content
 =============================  =============================================
 emotion                        emotion categories
 arousal / valence / dominance  emotion dimensions
 speaker                        unique speaker id
 role                           the role a speaker has, e.g. agent vs. client
-duration                       file duration
 transcription                  transcriptions on word or phonetic level
                                accurate enough to be used for ASR
 text                           transcriptions that are not accurate enough
                                for ASR
 =============================  =============================================
 
 In case you have several schemes of the same type,
@@ -198,15 +197,15 @@
     db
 
 
 File and speaker information
 ----------------------------
 
 Meta information like speaker ID
-or file duration
+that is not included in another table
 should be collected in a table ``files``.
 If you have metadata
 belonging only to segments,
 collect it in a table ``segments``.
 
 Additional meta information,
 that is bound to another information
@@ -245,78 +244,39 @@
 for an extended documentation.
 
 .. jupyter-execute::
 
     db['files'].get(map={'speaker': 'gender'})
 
 
-File duration and temporal data
--------------------------------
+Temporal data
+-------------
 
-It is recommended to store file durations
-for every database
-in a table ``files``.
-This information is in principle redundant
-as you can calculate the duration always on the fly,
-but if you have thousands of files
-this might take some time.
-
-Every temporal data
-like file durations
-should be stored as :class:`pandas.Timedelta`
-or :class:`datetime.datetime`.
+Temporal duration data
+like response time of a rater
+should be stored as :class:`pd.Timedelta`.
+Temporal dates
+like time of rating
+should be stored as :class:`datetime.datetime`.
 
 .. jupyter-execute::
-    :hide-code:
-    :hide-output:
 
-    import audiofile as af
-    import numpy as np
-
-
-    signal = np.ones([0, 1000])
-
-
-.. jupyter-execute::
-
-    import audeer
-    import audiofile as af
-    import numpy as np
     import pandas as pd
 
 
-    # Create dummy WAV files
-    sampling_rate = 1000
-    af.write('a.wav', np.ones([1, 1000]), sampling_rate)
-    af.write('b.wav', np.ones([1, 500]), sampling_rate)
+    times = [2.1, 0.1]  # in seconds
 
     db = audformat.Database('mydata')
 
-    db.schemes['duration'] = audformat.Scheme(dtype=audformat.define.DataType.TIME)
+    db.schemes['time'] = audformat.Scheme(audformat.define.DataType.TIME)
+    db.raters['rater'] = audformat.Rater()
+
     db['files'] = audformat.Table(
         index=audformat.filewise_index(['a.wav', 'b.wav'])
     )
-    db['files']['duration'] = audformat.Column(scheme_id='duration')
-    durations = audeer.run_tasks(
-        task_func=lambda x: pd.to_timedelta(af.duration(x), unit='s'),
-        params=[([f], {}) for f in db.files],
-        num_workers=12,
-        progress_bar=False,
+    db['files']['time'] = audformat.Column(
+        scheme_id='time',
+        rater_id='rater',
     )
-    db['files']['duration'].set(durations)
-
-    db
-
-.. jupyter-execute::
+    db['files']['time'].set(pd.to_timedelta(times, unit='s'))
 
     db['files'].get()
-
-
-.. Clean up
-.. jupyter-execute::
-    :hide-code:
-    :hide-output:
-
-    import os
-
-    os.remove('a.wav')
-    os.remove('b.wav')
```

### Comparing `audformat-0.9.8/docs/data-format.rst` & `audformat-1.0.0/docs/data-format.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 Database
 ========
 
-audformat is implemented in the :class:`audformat.Database`.
-Written to hard disk it is converted to a YAML file (*Header*),
-which contains information about the raters,
-annotation schemes and meta information.
-Actual annotations are stored
-across (possibly) multiple CSV files (*Tables*).
+An audformat database consists of a **header**,
+several **tables**,
+and **media** files.
+On hard disk all of them are stored inside a single folder.
+The header is stored as a YAML file,
+the tables contain labels stored in (possibly) multiple CSV files,
+and the media files are usually stored in sub-folders.
 Each table column is linked to a scheme and/or to a rater.
 Each table row is linked to a media file,
 or a specific segment in a media file.
+If no links to media files are given,
+the table is called miscellaneous table,
+or short **misc table**.
+The database is implemented as :class:`audformat.Database`.
+
+.. table:: Parts of a database stored in audformat on the hard disk.
+
+    ==========================  ==========================================
+    File                        Content
+    ==========================  ==========================================
+    ``db.yaml``                 Meta information, schemes, list of raters
+    ``db.<table_id>.csv``       Table with files or file segments as index
+                                and columns holding annotations
+    ``db.<misc_table_id>.csv``  Misc table with unspecified index
+                                and columns holding annotations
+    ``<folder(s)/file(s)>``     Audio/Video files referenced in the tables
+    ==========================  ==========================================
 
-.. table:: Parts of a database stored in the audformat on the hard disk.
+The connection between the header, media files and a table
+is highlighted in the following sketch:
 
-    =======================  ==========================================
-    File                     Content
-    =======================  ==========================================
-    ``db.yaml``              Meta information, schemes, list of raters
-    ``db.<table_id>.csv``    Table with files or file segments as index
-                             and columns holding annotations,
-                             such as speaker id,
-                             emotion ratings, ...
-    ``<folder(s)/file(s)>``  Audio/Video files referenced in the tables
-    =======================  ==========================================
+.. graphviz:: pics/audformat-table.dot
+    :alt: audformat table
+    :align: center
+    :caption: Connection between header definitions and table entries.
 
-The connection between the header and the tables
+The connection between the header and a misc table
 is highlighted in the following sketch:
 
-.. figure:: pics/audformat.dot.svg
-    :alt: audformat
+.. graphviz:: pics/audformat-misc-table.dot
+    :alt: audformat misc table
     :align: center
-
-    Connection between header definitions and table entries.
+    :caption: Connection between header definitions and misc table entries.
 
 The annotations stored in the tables
 can be accessed as :class:`pandas.DataFrame`.
 The following sketch shows an example instance of a database:
 
-.. figure:: pics/tables.dot.svg
+.. graphviz:: pics/audformat-database.dot
     :alt: Header and Tables
     :align: center
-
-    Example content of tables and there connection to the header.
+    :caption: Example content of tables and there connection to the header.
```

### Comparing `audformat-0.9.8/docs/data-header.rst` & `audformat-1.0.0/docs/data-header.rst`

 * *Files 16% similar despite different names*

```diff
@@ -26,19 +26,25 @@
 ==============  =========  ====================================================
 Field           Mandatory  Description
 ==============  =========  ====================================================
 name            yes        Database name
 source          yes        Original source,
                            e.g. link to webpage where files are hosted
 usage           yes        What the database can be used for,
-                           see :class:`audformat.define.Usage`
+                           one of ``'commercial'``, ``'other'``,
+                           ``'research'``, ``'restricted'``, ``'unrestricted'``
+author                     Author(s) of the database
 description                Description of the database
 expires                    Until when we are allowed to use the data
 languages                  List of languages that appear in the media files
+license                    License of the database
+license_url                Link to license statement
+attachments                Dictionary of attachment objects (see below)
 media                      Dictionary of media objects (see below)
+organization               Organization that created the database
 raters                     Dictionary of rater objects (see below)
 schemes                    Dictionary of scheme objects (see below)
 splits                     Dictionary of rater objects (see below)
 tables                     Dictionary of tables (see below)
 *meta-key-1*               1st optional meta field
 ...                        ...
 *meta-key-N*               Nth optional meta field
@@ -61,29 +67,69 @@
     import audformat
 
 
     # Create Database
     db = audformat.Database(
         name='databasename',
         source='https://gitlab.audeering.com/data/databasename',
-        usage=audformat.define.Usage.COMMERCIAL,
+        usage='commercial',
     )
     db
 
 
+Attachment
+----------
+
+This part of the header is represented by :class:`audformat.Attachment`.
+
+==============  =========  ====================================================
+Field           Mandatory  Description
+==============  =========  ====================================================
+path            yes        Relative path to attached file/folder
+description                Description of rater
+*meta-key-1*               1st optional meta field
+...                        ...
+*meta-key-N*               Nth optional meta field
+==============  =========  ====================================================
+
+Minimal example
+^^^^^^^^^^^^^^^
+
+.. code-block:: yaml
+
+    attachments:
+        attachmentid:
+            path: docs/setup.pdf
+
+audformat implementation
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. jupyter-execute::
+
+    # Create minimal Attachment
+    attachment = audformat.Attachment('docs/setup.pdf')
+    # Add Attachment to Database
+    db.attachments['attachmentid'] = attachment
+    # Access path of Attachment
+    db.attachments['attachmentid'].path
+    # Access attachments
+    db.attachments
+
+
 Rater
 -----
 
 This part of the header is represented by :class:`audformat.Rater`.
 
 ==============  =========  ====================================================
 Field           Mandatory  Description
 ==============  =========  ====================================================
 id              yes        Unique identifier of rater
-type            yes        Rater type, see :class:`audformat.define.RaterType`
+type            yes        Rater type, one of ``'human'``, ``'machine'``,
+                           ``'other'``, ``'ground truth'``, ``'vote'``
 description                Description of rater
 *meta-key-1*               1st optional meta field
 ...                        ...
 *meta-key-N*               Nth optional meta field
 ==============  =========  ====================================================
 
 Minimal example
@@ -97,15 +143,15 @@
 
 audformat implementation
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. jupyter-execute::
 
     # Create minimal Rater
-    rater = audformat.Rater(audformat.define.RaterType.HUMAN)
+    rater = audformat.Rater('human')
     # Add Rater to Database
     db.raters['raterid'] = rater
     # Access type of Rater
     db.raters['raterid'].type
     # Access raters
     db.raters
 
@@ -114,15 +160,17 @@
 ------
 
 This part of the header is represented by :class:`audformat.Scheme`.
 
 ==============  =========  ====================================================
 Field           Mandatory  Description
 ==============  =========  ====================================================
-dtype           yes        Data type, see :class:`audformat.define.DataType`
+dtype           yes        Data type, one of ``'bool'``,
+                           ``'int'``, ``'float'``, ``'object'``,
+                           ``'str'``, ``'time'``, ``'date'``
 id              yes        Unique identifier of scheme
 description                Description of scheme
 labels                     Dictionary or list with labels
                            (elements or keys must fit ``dtype``)
 minimum                    Minimum label value (only applied if ``dtype`` is
                            numeric)
 maximum                    Maximum label value (only applied if ``dtype`` is
@@ -135,23 +183,23 @@
 Minimal example
 ^^^^^^^^^^^^^^^
 
 .. code-block:: yaml
 
     schemes:
         schemeid:
-            dtype: human
+            dtype: float
 
 audformat implementation
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. jupyter-execute::
 
     # Create minimal Scheme
-    scheme = audformat.Scheme(audformat.define.DataType.FLOAT)
+    scheme = audformat.Scheme('float')
     # Add Scheme to Database
     db.schemes['schemeid'] = scheme
     # Access dtype of Scheme
     db.schemes['schemeid'].dtype
     # Access schemes
     db.schemes
 
@@ -161,16 +209,16 @@
 
 This part of the header is represented by :class:`audformat.Split`.
 
 ==============  =========  ====================================================
 Field           Mandatory  Description
 ==============  =========  ====================================================
 id              yes        Unique identifier of split
-type            yes        Split type,
-                           typically one of :class:`audformat.define.SplitType`
+type            yes        Split type, one of ``'train'``, ``'dev'``,
+                           ``'other'``, ``'test'``
 description                Description of split
 *meta-key-1*               1st optional meta field
 ...                        ...
 *meta-key-N*               Nth optional meta field
 ==============  =========  ====================================================
 
 Minimal example
@@ -184,15 +232,15 @@
 
 audformat implementation
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. jupyter-execute::
 
     # Create minimal Split
-    split = audformat.Split(audformat.define.SplitType.TEST)
+    split = audformat.Split('test')
     # Add Split to Database
     db.splits['splitid'] = split
     # Access type of Split
     db.splits['splitid'].type
     # Access splits
     db.splits
 
@@ -204,15 +252,16 @@
 
 To store media information use:
 
 ================  =========  ====================================================
 Field             Mandatory  Description
 ================  =========  ====================================================
 id                yes        Unique identifier of media type
-type                         Media type, one of (``audio``, ``video``, ``other``)
+type                         Media type, one of ``'audio'``, ``'video'``,
+                             ``'other'``
 bit_depth                    Audio bit depth
 channels                     Number of audio channels
 description                  Description
 format                       Media file format (e.g. ``wav`` or ``mp4``)
 sampling_rate                Audio sampling rate in Hz
 video_fps                    Video rate in frames per seconds
 video_resolution             Video resolution in pixels (``width`` x ``height``)
@@ -234,15 +283,15 @@
 
 audformat implementation
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. jupyter-execute::
 
     # Create minimal media information
-    media = audformat.Media()
+    media = audformat.Media('audio')
     # Add media to Database
     db.media['mediaid'] = media
     # Access type of Media
     db.media['mediaid'].type
     # Access media
     db.media
 
@@ -252,15 +301,15 @@
 
 This part of the header is represented by :class:`audformat.Table`
 
 ==============  =========  ====================================================
 Field           Mandatory  Description
 ==============  =========  ====================================================
 id              yes        Unique identifier of table
-type            yes        Table type, see :class:`audformat.define.TableType`
+type            yes        Table type, one of ``'filewise'``, ``'segmented'``
 columns                    Dictionary of columns (see below)
 description                Description of table
 media_id                   Files in this table are of this media type
 split_id                   The split the table belongs to
 *meta-key-1*               1st optional meta field
 ...                        ...
 *meta-key-N*               Nth optional meta field
@@ -290,14 +339,61 @@
     db['tableid'] = table
     # Access type of Table (short notation)
     db['tableid'].type
     # Access tables
     db.tables
 
 
+Misc Table
+----------
+
+This part of the header is represented by :class:`audformat.MiscTable`.
+
+==============  =========  ====================================================
+Field           Mandatory  Description
+==============  =========  ====================================================
+id              yes        Unique identifier of misc table
+columns                    Dictionary of columns (see below)
+description                Description of table
+media_id                   Files in this table are of this media type
+split_id                   The split the table belongs to
+*meta-key-1*               1st optional meta field
+...                        ...
+*meta-key-N*               Nth optional meta field
+==============  =========  ====================================================
+
+Minimal example
+^^^^^^^^^^^^^^^
+
+.. code-block:: yaml
+
+    misc_tables:
+        misctableid:
+            levels: [idx]
+
+audformat implementation
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. jupyter-execute::
+
+    # Create minimal Misc Table
+    import pandas as pd
+    misc_table = audformat.MiscTable(pd.Index([], name='idx'))
+    # Add Misc Table to Database
+    db.misc_tables['misctableid'] = misc_table
+    # Access dataframe of Misc Table
+    db.misc_tables['misctableid'].df
+    # Add Misc Table to Database (short notation)
+    db['misctableid'] = misc_table
+    # Access dataframe of Misc Table (short notation)
+    db['misctableid'].df
+    # Access misc tables
+    db.misc_tables
+
+
 Column
 ------
 
 This part of the header is represented by :class:`audformat.Column`
 
 ==============  =========  ====================================================
 Field           Mandatory  Description
```

### Comparing `audformat-0.9.8/docs/data-introduction.rst` & `audformat-1.0.0/docs/data-introduction.rst`

 * *Files identical despite different names*

### Comparing `audformat-0.9.8/docs/data-tables.rst` & `audformat-1.0.0/docs/data-tables.rst`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     import audformat
 
 
     audformat.core.common.format_series_as_html()
 
 
 A table links labels to media files.
-It consists of one or more index columns
+It consists of one or three index columns
 followed by an arbitrary number of label columns.
 Labels can either refer to whole files or part of files.
 An empty label means that no label has been assigned (yet).
 
 There are two types of tables:
 
 * **Filewise**: labels refer to whole files
@@ -82,32 +82,29 @@
 
 Access labels as :class:`pandas.Series`
 
 .. jupyter-execute::
 
     db['filewise']['values'].get()
 
-Create a segmented index:
+Access labels and convert index to a segmented index:
 
 .. jupyter-execute::
 
-    import pandas as pd
+    db['filewise']['values'].get(as_segmented=True)
 
+Access labels from a filewise table with a segmented index:
+
+.. jupyter-execute::
 
     segmented_index = audformat.segmented_index(
         files=['f1', 'f1', 'f1', 'f2'],
         starts=['0s', '1s', '2s', '0s'],
-        ends=['1s', '2s', '3s', pd.NaT],
+        ends=['1s', '2s', '3s', None],
     )
-    segmented_index
-
-Access labels from a filewise table with a segmented index:
-
-.. jupyter-execute::
-
     db['filewise'].get(segmented_index)
 
 Access labels from a filewise column with a segmented index:
 
 .. jupyter-execute::
 
     db['filewise']['values'].get(segmented_index)
@@ -132,15 +129,15 @@
 Create a segmented index:
 
 .. jupyter-execute::
 
     segmented_index = audformat.segmented_index(
         files=['f1', 'f1', 'f1', 'f2', 'f3'],
         starts=['0s', '1s', '2s', '0s', '1m'],
-        ends=['1s', '2s', '3s', pd.NaT, '1h'],
+        ends=['1s', '2s', '3s', None, '1h'],
     )
     segmented_index
 
 Add table with a segmented index:
 
 .. jupyter-execute::
 
@@ -150,17 +147,15 @@
 
 Assign labels to the whole table:
 
 .. jupyter-execute::
 
     values_list = [1, 2, 3, 4, 5]
     values_dict = {'values': values_list}
-    db['segmented'].set(
-        values_dict,
-    )
+    db['segmented'].set(values_dict)
 
 Access all labels as :class:`pandas.DataFrame`:
 
 .. jupyter-execute::
 
     db['segmented'].get()
 
@@ -172,27 +167,21 @@
 
 Access labels from a column as :class:`pandas.Series`:
 
 .. jupyter-execute::
 
     db['segmented']['values'].get()
 
-Create a filewise index:
+Access labels from a segmented table with a filewise index:
 
 .. jupyter-execute::
 
     filewise_index = audformat.filewise_index(
         ['f1', 'f2'],
     )
-    filewise_index
-
-Access labels from a segmented table with a filewise index:
-
-.. jupyter-execute::
-
     db['segmented'].get(filewise_index)
 
 Access labels from a segmented column with a filewise index:
 
 .. jupyter-execute::
 
     db['segmented']['values'].get(filewise_index)
```

### Comparing `audformat-0.9.8/docs/emodb-example.rst` & `audformat-1.0.0/docs/emodb-example.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _emodb-example:
+
 Emodb example
 =============
 
 In this example we download the small emodb_ database,
 that contains sentences
 spoken with different emotions
 by different actors.
@@ -117,15 +119,14 @@
 We will read in this file
 and use the annotations to add a confidence column
 to the emotion table.
 
 .. jupyter-execute::
 
     import audformat
-    import audiofile as af
     import pandas as pd
 
     # Prepare functions for getting information from file names
     def parse_names(names, from_i, to_i, is_number=False, mapping=None):
         for name in names:
             key = name[from_i:to_i]
             if is_number:
@@ -167,36 +168,39 @@
         os.path.join(src_dir, 'erkennung.txt'),
         usecols=['Satz', 'erkannt'],
         index_col='Satz',
         delim_whitespace=True,
         encoding='Latin-1',
         decimal=',',
         converters={'Satz': lambda x: os.path.join('wav', x)},
-        squeeze=True,
-    )
+    ).squeeze('columns')
     y = y.loc[files]
     y = y.replace(to_replace=u'\xa0', value='', regex=True)
     y = y.replace(to_replace=',', value='.', regex=True)
     confidences = y.astype('float').values
 
     male = audformat.define.Gender.MALE
     female = audformat.define.Gender.FEMALE
-    language = audformat.utils.map_language('de')
-    speaker_mapping = {
-        3: {'gender': male, 'age': 31, 'language': language},
-        8: {'gender': female, 'age': 34, 'language': language},
-        9: {'gender': male, 'age': 21, 'language': language},
-        10: {'gender': female, 'age': 32, 'language': language},
-        11: {'gender': male, 'age': 26, 'language': language},
-        12: {'gender': female, 'age': 30, 'language': language},
-        13: {'gender': male, 'age': 32, 'language': language},
-        14: {'gender': female, 'age': 35, 'language': language},
-        15: {'gender': male, 'age': 25, 'language': language},
-        16: {'gender': female, 'age': 31, 'language': language},
-    }
+    de = audformat.utils.map_language('de')
+    df_speaker = pd.DataFrame(
+        index=pd.Index([3, 8, 9, 10, 11, 12, 13, 14, 15, 16], name='speaker'),
+        columns=['age', 'gender', 'language'],
+        data = [
+            [31, male, de],
+            [34, female, de],
+            [21, female, de],
+            [32, male, de],
+            [26, male, de],
+            [30, male, de],
+            [32, female, de],
+            [35, female, de],
+            [25, male, de],
+            [31, female, de],
+       ],
+    )
     speakers = list(parse_names(names, from_i=0, to_i=2, is_number=True))
 
     transcription_mapping = {
         'a01': 'Der Lappen liegt auf dem Eisschrank.',
         'a02': 'Das will sie am Mittwoch abgeben.',
         'a04': 'Heute abend könnte ich es ihm sagen.',
         'a05': 'Das schwarze Stück Papier befindet sich da oben neben dem '
@@ -210,37 +214,28 @@
                'gefahren und habe Agnes besucht.',
         'b09': 'Ich will das eben wegbringen und dann mit Karl was '
                'trinken gehen.',
         'b10': 'Die wird auf dem Platz sein, wo wir sie immer hinlegen.',
     }
     transcriptions = list(parse_names(names, from_i=2, to_i=5))
 
-    durations = audeer.run_tasks(
-        task_func=lambda x: pd.to_timedelta(
-            af.duration(os.path.join(src_dir, x)),
-            unit='s',
-        ),
-        params=[([f], {}) for f in files],
-        num_workers=12,
-    )
-
 
 Create audformat database
 -------------------------
 
 Now we create the database object
 and assign the information to it.
 
 .. jupyter-execute::
 
     db = audformat.Database(
         name='emodb',
         source=source,
         usage=audformat.define.Usage.UNRESTRICTED,
-        languages=[language],
+        languages=[de],
         description=description,
         meta={
             'pdf': (
                 'http://citeseerx.ist.psu.edu/viewdoc/'
                 'download?doi=10.1.1.130.8506&rep=rep1&type=pdf'
             ),
         },
@@ -258,41 +253,60 @@
 
     # Schemes
     db.schemes['emotion'] = audformat.Scheme(
         labels=[str(x) for x in emotion_mapping.values()],
         description='Six basic emotions and neutral.',
     )
     db.schemes['confidence'] = audformat.Scheme(
-        audformat.define.DataType.FLOAT,
+        'float',
         minimum=0,
         maximum=1,
         description='Confidence of emotion ratings.',
     )
+    db.schemes['age'] = audformat.Scheme(
+        'int',
+        minimum=0,
+        description='Age of speaker',
+    )
+    db.schemes['gender'] = audformat.Scheme(
+        labels=['female', 'male'],
+        description='Gender of speaker',
+    )
+    db.schemes['language'] = audformat.Scheme(
+        'str',
+        description='Language of speaker',
+    )
+    db.schemes['transcription'] = audformat.Scheme(
+        labels=transcription_mapping,
+        description='Sentence produced by actor.',
+    )
+
+    # MiscTable
+    db['speaker'] = audformat.MiscTable(df_speaker.index)
+    db['speaker']['age'] = audformat.Column(scheme_id='age')
+    db['speaker']['gender'] = audformat.Column(scheme_id='gender')
+    db['speaker']['language'] = audformat.Column(scheme_id='language')
+    db['speaker'].set(df_speaker.to_dict(orient='list'))
+
+    # MiscTable as Scheme
     db.schemes['speaker'] = audformat.Scheme(
-        labels=speaker_mapping,
+        labels='speaker',
+        dtype='int',
         description=(
             'The actors could produce each sentence as often as '
             'they liked and were asked to remember a real '
             'situation from their past when they had felt this '
             'emotion.'
         ),
     )
-    db.schemes['transcription'] = audformat.Scheme(
-        labels=transcription_mapping,
-        description='Sentence produced by actor.',
-    )
-    db.schemes['duration'] = audformat.Scheme(dtype=audformat.define.DataType.TIME)
 
     # Tables
     index = audformat.filewise_index(files)
     db['files'] = audformat.Table(index)
 
-    db['files']['duration'] = audformat.Column(scheme_id='duration')
-    db['files']['duration'].set(durations, index=index)
-
     db['files']['speaker'] = audformat.Column(scheme_id='speaker')
     db['files']['speaker'].set(speakers)
 
     db['files']['transcription'] = audformat.Column(scheme_id='transcription')
     db['files']['transcription'].set(transcriptions)
 
     db['emotion'] = audformat.Table(index)
@@ -322,27 +336,33 @@
 Inspect database tables
 -----------------------
 
 First check which tables are available.
 
 .. jupyter-execute::
 
-    list(db.tables)
+    list(db)
 
 Then list the first 10 entries of every table.
 
 .. jupyter-execute::
 
     db['files'].get()[:10]
 
 .. jupyter-execute::
 
     db['emotion'].get()[:10]
 
-You access additional header information in a table
+.. jupyter-execute::
+
+    db['speaker'].get()[:10]
+
+Columns might contain labels,
+that provide additional mappings.
+You can access this additional information
 with the ``map`` argument of :meth:`audformat.Table.get`,
 see :ref:`map-scheme-labels`
 for an extended documentation.
 
 .. jupyter-execute::
 
     db['files'].get(map={'speaker': ['speaker', 'age', 'gender']})[:10]
```

### Comparing `audformat-0.9.8/docs/index.rst` & `audformat-1.0.0/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -8,39 +8,41 @@
     :hidden:
 
     install
     create-database
     accessing-data
     combine-tables
     map-scheme
+    update-database
     emodb-example
 
 .. toctree::
     :caption: Format specification
     :hidden:
 
     data-introduction
     data-format
     data-conventions
     data-header
     data-tables
+    data-misc-tables
     data-example
 
 .. Warning: then usage of genindex is a hack to get a TOC entry, see
 .. https://stackoverflow.com/a/42310803. This might break the usage of sphinx if
 .. you want to create something different than HTML output.
 .. toctree::
     :caption: API Documentation
     :hidden:
 
-    api
-    api-define
-    api-errors
-    api-testing
-    api-utils
+    api/audformat
+    api/audformat.define
+    api/audformat.errors
+    api/audformat.testing
+    api/audformat.utils
     genindex
 
 .. toctree::
     :caption: Development
     :hidden:
 
     contributing
```

### Comparing `audformat-0.9.8/docs/map-scheme.rst` & `audformat-1.0.0/docs/map-scheme.rst`

 * *Files identical despite different names*

### Comparing `audformat-0.9.8/docs/pics/tables.dot` & `audformat-1.0.0/docs/pics/audformat-database.dot`

 * *Files 20% similar despite different names*

```diff
@@ -7,25 +7,25 @@
     label="{ Header | ... | <tbl1> Table#1 | <tbl2> Table#2 | ... }"
   ]
 
   tbl1 [
     label=<
       <table>
         <tr><td colspan='3'>Table#1</td></tr>
-        <tr><td>File</td><td>Name</td><td>Gender</td></tr>
+        <tr><td>file</td><td>name</td><td>gender</td></tr>
         <tr><td>alice.wav</td><td>Alice</td><td>female</td></tr>
         <tr><td>bob.wav</td><td>Bob</td><td>male</td></tr>
       </table>
     >]
 
   tbl2 [
     label=<
       <table>
         <tr><td colspan='4'>Table#2</td></tr>
-        <tr><td>File</td><td>Start</td><td>End</td><td>Text</td></tr>
+        <tr><td>file</td><td>start</td><td>end</td><td>text</td></tr>
         <tr><td>alice.wav</td><td>0.2</td><td>1.1</td><td>Hi, I'm Alice</td></tr>
         <tr><td>bob.wav</td><td>1.4</td><td>3.0</td><td>How are you doing?</td></tr>
         <tr><td>alice.wav</td><td>3.4</td><td>4.7</td><td>Thanks, I'm good!</td></tr>
       </table>
     >]
 
     header:tbl1 -> tbl1
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 digraph { node[shape=plaintext] header [ shape=record label="{ Header | ... |
 Table#1 |  Table#2 | ... }" ] tbl1 [ label=<
 Table#1
-File      Name  Gender
+file      name  gender
 alice.wav Alice female
 bob.wav   Bob   male
 >] tbl2 [ label=<
 Table#2
-File      Start End Text
+file      start end text
 alice.wav 0.2   1.1 Hi, I'm Alice
 bob.wav   1.4   3.0 How are you doing?
 alice.wav 3.4   4.7 Thanks, I'm good!
 >] header:tbl1 -> tbl1 header:tbl2 -> tbl2 }
```

### Comparing `audformat-0.9.8/setup.cfg` & `audformat-1.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 [metadata]
 name = audformat
-author = Johannes Wagner, Hagen Wierstorf
-author-email = jwagner@audeering.com, hwierstorf@audeering.com
+author = Johannes Wagner, Hagen Wierstorf, Baha Eddine Abrougui
+author_email = jwagner@audeering.com, hwierstorf@audeering.com, beddine@audeering.com
 url = https://github.com/audeering/audformat/
-project-urls = 
+project_urls = 
 	Documentation = https://audeering.github.io/audformat/
 description = Python implementation of audformat
-long-description = file: README.rst, CHANGELOG.rst
+long_description = file: README.rst, CHANGELOG.rst
 license = MIT
-license-file = LICENSE
+license_file = LICENSE
 keywords = audio, database, annotation
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 install_requires = 
-	audeer >=1.8.0,<2.0.0
-	audiofile >=0.4.0,<1.0.0
+	audeer >=1.19.0,<2.0.0
+	audiofile >=0.4.0
 	iso-639
+	iso3166
 	oyaml
-	pandas >=1.1.0
+	pyyaml >=5.4.1
+	pandas >=1.4.1
+python_requires = >=3.8
 setup_requires = 
 	setuptools_scm
 
 [tool:pytest]
 addopts = 
-	--flake8
 	--doctest-plus
 	--cov=audformat
 	--cov-fail-under=100
 	--cov-report xml
 	--cov-report term-missing
 xfail_strict = true
 
 [flake8]
-ignore = 
-	W503  # math, https://github.com/PyCQA/pycodestyle/issues/513
-	__init__.py F401 F403  # ignore unused and * imports
-	docs/examples/*.py F821  # ignore undefined variables
+exclude = 
+	.eggs,
+	build,
+extend-ignore = 
+	W503,
+per-file-ignores = 
+	__init__.py: F401, F403,
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `audformat-0.9.8/tests/test_eq.py` & `audformat-1.0.0/tests/test_eq.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,21 +23,40 @@
     assert str(db) == str(db2)  # same header
     assert db['files'] != db2['files']
     assert db['files']['string'] != db2['files']['string']
     assert db.schemes['string'] == db2.schemes['string']  # same schemes
 
     # compare with db that has same data
 
+    audformat.testing.create_attachment_files(db, tmpdir)
     db.save(tmpdir)
     db3 = audformat.Database.load(tmpdir)
 
     assert db == db3
     assert db['files'] == db3['files']
     assert db['files']['string'] == db3['files']['string']
 
+    # compare with db that has different table values
+
+    db.save(tmpdir)
+    db4 = audformat.Database.load(tmpdir)
+    db4['files'].df.at['string', 0] = 'Believe me, I am special!'
+
+    assert db != db4
+    assert db['files'] != db4['files']
+
+    # compare with db that has different table meta
+
+    db.save(tmpdir)
+    db5 = audformat.Database.load(tmpdir)
+    db5['files'].description = 'Believe me, I am special!'
+
+    assert db != db5
+    assert db['files'] != db5['files']
+
     # compare with column that has no data
 
     c_no_data = audformat.Column(
         scheme_id=db['files']['string'].scheme_id,
         rater_id=db['files']['string'].rater_id,
         description=db['files']['string'].description,
         meta=db['files']['string'].meta.copy()
```

### Comparing `audformat-0.9.8/tests/test_errors.py` & `audformat-1.0.0/tests/test_errors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pandas as pd
 import pytest
 
 import audformat
 from audformat import testing
 
 
 def test_errors():
@@ -45,7 +46,40 @@
         db.splits['split'] = audformat.Split('bad')
 
     with pytest.raises(audformat.errors.BadValueError):
         db.schemes['scheme'] = audformat.Scheme('bad')
 
     with pytest.raises(audformat.errors.BadValueError):
         audformat.Database('foo', 'internal', 'bad')
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db['bad']
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db.media['bad']
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db.misc_tables['bad']
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db.raters['bad']
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db.schemes['bad']
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db.splits['bad']
+
+    with pytest.raises(audformat.errors.BadKeyError):
+        db.tables['bad']
+
+    with pytest.raises(audformat.errors.TableExistsError):
+        # a miscellaneous table with same ID exists already
+        db['misc'] = audformat.Table()
+
+    with pytest.raises(audformat.errors.TableExistsError):
+        # a filewise table with same ID exists already
+        db['files'] = audformat.MiscTable(pd.Index([], name='idx'))
+
+    with pytest.raises(audformat.errors.TableExistsError):
+        # a segmented table with same ID exists already
+        db['segments'] = audformat.MiscTable(pd.Index([], name='idx'))
```

### Comparing `audformat-0.9.8/tests/test_index.py` & `audformat-1.0.0/tests/test_index.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @pytest.mark.parametrize(
     'obj',
     [
         audformat.filewise_index(),
         audformat.filewise_index(['f1', 'f2']),
         pd.Series(
             index=audformat.filewise_index(['f1', 'f2']),
+            dtype=float,
         ),
         pd.DataFrame(
             index=audformat.filewise_index(['f1', 'f2']),
         ),
         audformat.segmented_index(),
         audformat.segmented_index(['f1', 'f2']),
         pytest.param(  # missing names
@@ -56,32 +57,94 @@
                     [0, 0],
                     [0, 0],
                     [0, 0],
                 ]
             ),
             marks=pytest.mark.xfail(raises=ValueError),
         ),
+        pytest.param(  # invalid file type
+            pd.Index([1, 2], name='file'),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # invalid file type
+            pd.MultiIndex.from_arrays(
+                [
+                    [1, 2],
+                    pd.to_timedelta([0.0, 1.0], unit='s'),
+                    pd.to_timedelta([1.0, 2.0], unit='s'),
+                ],
+                names=['file', 'start', 'end'],
+            ),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # invalid start type
+            pd.MultiIndex.from_arrays(
+                [
+                    ['f1', 'f2'],
+                    [0.0, 1.0],
+                    pd.to_timedelta([1.0, 2.0], unit='s'),
+                ],
+                names=['file', 'start', 'end'],
+            ),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # invalid end type
+            pd.MultiIndex.from_arrays(
+                [
+                    ['f1', 'f2'],
+                    pd.to_timedelta([0.0, 1.0], unit='s'),
+                    [1.0, 2.0],
+                ],
+                names=['file', 'start', 'end'],
+            ),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
     ]
 )
 def test_assert_index(obj):
     audformat.assert_index(obj)
 
 
 @pytest.mark.parametrize(
+    'obj',
+    [
+        audformat.filewise_index(),
+        audformat.filewise_index(['f1', 'f2']),
+        pd.Series(
+            index=audformat.filewise_index(['f1', 'f2']),
+            dtype=float,
+        ),
+        pd.DataFrame(
+            index=audformat.filewise_index(['f1', 'f2']),
+        ),
+        audformat.segmented_index(),
+        audformat.segmented_index(['f1', 'f2']),
+        pytest.param(  # duplicates
+            audformat.filewise_index(['f1', 'f1']),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        pytest.param(  # duplicates
+            audformat.segmented_index(['f1', 'f1']),
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+    ]
+)
+def test_assert_no_duplicates(obj):
+    audformat.assert_no_duplicates(obj)
+
+
+@pytest.mark.parametrize(
     'files',
     [
         None,
         [],
         '1.wav',
         ['1.wav', '2.wav'],
         pytest.DB['files'].files,
-        pytest.param(  # duplicates
-            ['f1', 'f2', 'f2'],
-            marks=pytest.mark.xfail(raises=ValueError),
-        )
+        ['f1', 'f2', 'f2'],  # duplicates
     ]
 )
 def test_create_filewise_index(files):
 
     index = audformat.filewise_index(files)
 
     files = to_array(files)
@@ -163,31 +226,18 @@
         ),
         pytest.param(  # len files != len starts/ends
             ['1.wav'],
             [pd.Timedelta('0s'), pd.Timedelta('1s')],
             [pd.Timedelta('1s'), pd.Timedelta('2s')],
             marks=pytest.mark.xfail(raises=ValueError),
         ),
-        pytest.param(  # duplicates
+        (  # duplicates
             ['f1', 'f1'],
             None,
             None,
-            marks=pytest.mark.xfail(raises=ValueError),
-        ),
-        pytest.param(  # duplicates
-            ['f1', 'f1'],
-            [0, 0],
-            [1, 1],
-            marks=pytest.mark.xfail(raises=ValueError),
-        ),
-        pytest.param(  # duplicates
-            ['f1', 'f1'],
-            [0, 0],
-            None,
-            marks=pytest.mark.xfail(raises=ValueError),
         ),
     ]
 )
 def test_create_segmented_index(files, starts, ends):
 
     index = audformat.segmented_index(files, starts=starts, ends=ends)
```

