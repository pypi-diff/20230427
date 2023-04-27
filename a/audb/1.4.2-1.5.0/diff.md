# Comparing `tmp/audb-1.4.2.tar.gz` & `tmp/audb-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audb-1.4.2.tar", last modified: Mon Feb 13 13:00:57 2023, max compression
+gzip compressed data, was "audb-1.5.0.tar", last modified: Thu Apr 27 13:01:57 2023, max compression
```

## Comparing `audb-1.4.2.tar` & `audb-1.5.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.431140 audb-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-02-13 13:00:46.000000 audb-1.4.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-13 13:00:46.000000 audb-1.4.2/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-02-13 13:00:46.000000 audb-1.4.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-13 13:00:46.000000 audb-1.4.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-13 13:00:46.000000 audb-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-13 13:00:46.000000 audb-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-02-13 13:00:46.000000 audb-1.4.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-02-13 13:00:46.000000 audb-1.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-13 13:00:46.000000 audb-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-02-13 13:00:57.431140 audb-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-13 13:00:46.000000 audb-1.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/audb/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-13 13:00:46.000000 audb-1.4.2/audb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/audb/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/define.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/audb/core/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/etc/audb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/flavor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    39719 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/load_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-13 13:00:46.000000 audb-1.4.2/audb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/audb/info/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-13 13:00:46.000000 audb-1.4.2/audb/info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/audb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-02-13 13:00:57.000000 audb-1.4.2/audb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-02-13 13:00:57.000000 audb-1.4.2/audb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 13:00:57.000000 audb-1.4.2/audb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-13 13:00:57.000000 audb-1.4.2/audb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-13 13:00:57.000000 audb-1.4.2/audb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.431140 audb-1.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.427140 audb-1.4.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.431140 audb-1.4.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-13 13:00:46.000000 audb-1.4.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-02-13 13:00:46.000000 audb-1.4.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-13 13:00:46.000000 audb-1.4.2/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.431140 audb-1.4.2/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-13 13:00:46.000000 audb-1.4.2/docs/api-src/audb.info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-13 13:00:46.000000 audb-1.4.2/docs/api-src/audb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-13 13:00:46.000000 audb-1.4.2/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-02-13 13:00:46.000000 audb-1.4.2/docs/caching.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-13 13:00:46.000000 audb-1.4.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-02-13 13:00:46.000000 audb-1.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-13 13:00:46.000000 audb-1.4.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-13 13:00:46.000000 audb-1.4.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-02-13 13:00:46.000000 audb-1.4.2/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-13 13:00:46.000000 audb-1.4.2/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-13 13:00:46.000000 audb-1.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-13 13:00:46.000000 audb-1.4.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-02-13 13:00:46.000000 audb-1.4.2/docs/load.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-02-13 13:00:46.000000 audb-1.4.2/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.431140 audb-1.4.2/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-13 13:00:46.000000 audb-1.4.2/docs/pics/load.dot
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-13 13:00:46.000000 audb-1.4.2/docs/pics/publish.dot
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-02-13 13:00:46.000000 audb-1.4.2/docs/publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-13 13:00:46.000000 audb-1.4.2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-13 13:00:46.000000 audb-1.4.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-13 13:00:46.000000 audb-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-13 13:00:57.435140 audb-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-13 13:00:46.000000 audb-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 13:00:57.431140 audb-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-13 13:00:46.000000 audb-1.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-13 13:00:46.000000 audb-1.4.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_flavor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_load_on_demand.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_lock_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    19413 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-02-13 13:00:46.000000 audb-1.4.2/tests/test_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.085238 audb-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.073238 audb-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.077238 audb-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 13:01:43.000000 audb-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 13:01:43.000000 audb-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-27 13:01:43.000000 audb-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-27 13:01:43.000000 audb-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 13:01:43.000000 audb-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-04-27 13:01:57.085238 audb-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-27 13:01:43.000000 audb-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.077238 audb-1.5.0/audb/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 13:01:43.000000 audb-1.5.0/audb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/audb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/audb/core/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/etc/audb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49096 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/load_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/audb/info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-27 13:01:43.000000 audb-1.5.0/audb/info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.077238 audb-1.5.0/audb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-27 13:01:57.000000 audb-1.5.0/audb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.073238 audb-1.5.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 13:01:43.000000 audb-1.5.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 13:01:43.000000 audb-1.5.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 13:01:43.000000 audb-1.5.0/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 13:01:43.000000 audb-1.5.0/docs/api-src/audb.info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-27 13:01:43.000000 audb-1.5.0/docs/api-src/audb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-27 13:01:43.000000 audb-1.5.0/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-27 13:01:43.000000 audb-1.5.0/docs/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 13:01:43.000000 audb-1.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-27 13:01:43.000000 audb-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 13:01:43.000000 audb-1.5.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 13:01:43.000000 audb-1.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-27 13:01:43.000000 audb-1.5.0/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:01:43.000000 audb-1.5.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-27 13:01:43.000000 audb-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-27 13:01:43.000000 audb-1.5.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-27 13:01:43.000000 audb-1.5.0/docs/load.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-27 13:01:43.000000 audb-1.5.0/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 13:01:43.000000 audb-1.5.0/docs/pics/load.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 13:01:43.000000 audb-1.5.0/docs/pics/publish.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-27 13:01:43.000000 audb-1.5.0/docs/publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-27 13:01:43.000000 audb-1.5.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 13:01:43.000000 audb-1.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 13:01:43.000000 audb-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-27 13:01:57.085238 audb-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 13:01:43.000000 audb-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.085238 audb-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-27 13:01:43.000000 audb-1.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:01:43.000000 audb-1.5.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_load_on_demand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_lock_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40591 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_utils.py
```

### Comparing `audb-1.4.2/.github/workflows/doc.yml` & `audb-1.5.0/.github/workflows/doc.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Documentation
 
 on:
   push:
-    branches: [ main ]
+    branches: [ main, dev ]
   pull_request:
-    branches: [ main ]
+    branches: [ main, dev ]
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
@@ -18,15 +18,15 @@
     steps:
     - uses: actions/checkout@v3
 
     - name: Cache emodb
       uses: actions/cache@v3
       with:
         path: ~/audb
-        key: emodb-1.2.0
+        key: emodb-1.4.1
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Ubuntu - install libsndfile
```

### Comparing `audb-1.4.2/.github/workflows/publish.yml` & `audb-1.5.0/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -73,9 +73,9 @@
     - name: Create release on Github
       id: create_release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
-        release_name: Release ${{ github.ref_name }}
+        name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audb-1.4.2/.github/workflows/test.yml` & `audb-1.5.0/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Test
 
 on:
   push:
-    branches: [ main ]
+    branches: [ main, dev ]
   pull_request:
-    branches: [ main ]
+    branches: [ main, dev ]
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
@@ -25,15 +25,15 @@
     steps:
     - uses: actions/checkout@v3
 
     - name: Cache emodb
       uses: actions/cache@v3
       with:
         path: ~/audb
-        key: emodb-1.2.0
+        key: emodb-1.4.1
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Ubuntu - install libsndfile
```

### Comparing `audb-1.4.2/CHANGELOG.rst` & `audb-1.5.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,45 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.5.0 (2023-04-27)
+--------------------------
+
+* Added: support loading and publishing
+  of database attachments
+  (``audformat.Attachment``)
+* Added: ``audb.load_attachment()``
+  to load a single attachment of a database
+* Added: ``audb.info.attachments()``
+  to return the attachments entry
+  of a database header
+* Added: ``attachments`` argument to ``audb.load()``
+  to load only specific
+  attachments of a database
+* Changed: raise ``RuntimeError`` in ``audb.publish()``
+  if the file extension of a media file
+  contains uppercase letters
+* Changed: raise ``RuntimeError`` in ``audb.publish()``
+  if a table ID or attachment ID
+  contains a character not in ``[A-Za-z0-9._-]``
+* Changed: raise ``ValueError`` in ``audb.publish()``
+  if ``version`` or ``previous_version``
+  are not conform to ``audeer.StrictVersion``
+* Changed: use emodb v1.4.1 for documentation examples
+* Changed: require ``audbackend<1.0.0``
+  as ``audbackend`` will introduce breaking changes
+* Fixed: speed up ``audb.load_to()``
+  when loading databases with large tables
+  using ``only_metadata=True``
+
+
 Version 1.4.2 (2023-02-13)
 --------------------------
 
 * Added: support for Python 3.10
 * Added: document optional needed overwrite permissions
   for ``audb.publish()``
   when continuing a canceled publishing command
```

### Comparing `audb-1.4.2/CONTRIBUTING.rst` & `audb-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/LICENSE` & `audb-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/PKG-INFO` & `audb-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audb
-Version: 1.4.2
+Version: 1.5.0
 Summary: Load and publish databases in audformat
 Home-page: https://audeering.github.io/audb/
 Author: Johannes Wagner, Hagen Wierstorf
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audb/
 Description: ====
@@ -37,15 +37,15 @@
         .. _quickstart: https://audeering.github.io/audb/quickstart.html
         
         
         .. badges images and links:
         .. |tests| image:: https://github.com/audeering/audb/workflows/Test/badge.svg
             :target: https://github.com/audeering/audb/actions?query=workflow%3ATest
             :alt: Test status
-        .. |coverage| image:: https://codecov.io/gh/audeering/audb/branch/master/graph/badge.svg?token=drrULW8vEG
+        .. |coverage| image:: https://codecov.io/gh/audeering/audb/branch/main/graph/badge.svg?token=drrULW8vEG
             :target: https://codecov.io/gh/audeering/audb/
             :alt: code coverage
         .. |docs| image:: https://img.shields.io/pypi/v/audb?label=docs
             :target: https://audeering.github.io/audb/
             :alt: audb's documentation
         .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
             :target: https://github.com/audeering/audb/blob/master/LICENSE
@@ -59,14 +59,45 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.5.0 (2023-04-27)
+        --------------------------
+        
+        * Added: support loading and publishing
+          of database attachments
+          (``audformat.Attachment``)
+        * Added: ``audb.load_attachment()``
+          to load a single attachment of a database
+        * Added: ``audb.info.attachments()``
+          to return the attachments entry
+          of a database header
+        * Added: ``attachments`` argument to ``audb.load()``
+          to load only specific
+          attachments of a database
+        * Changed: raise ``RuntimeError`` in ``audb.publish()``
+          if the file extension of a media file
+          contains uppercase letters
+        * Changed: raise ``RuntimeError`` in ``audb.publish()``
+          if a table ID or attachment ID
+          contains a character not in ``[A-Za-z0-9._-]``
+        * Changed: raise ``ValueError`` in ``audb.publish()``
+          if ``version`` or ``previous_version``
+          are not conform to ``audeer.StrictVersion``
+        * Changed: use emodb v1.4.1 for documentation examples
+        * Changed: require ``audbackend<1.0.0``
+          as ``audbackend`` will introduce breaking changes
+        * Fixed: speed up ``audb.load_to()``
+          when loading databases with large tables
+          using ``only_metadata=True``
+        
+        
         Version 1.4.2 (2023-02-13)
         --------------------------
         
         * Added: support for Python 3.10
         * Added: document optional needed overwrite permissions
           for ``audb.publish()``
           when continuing a canceled publishing command
```

### Comparing `audb-1.4.2/README.rst` & `audb-1.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 .. _quickstart: https://audeering.github.io/audb/quickstart.html
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/audb/workflows/Test/badge.svg
     :target: https://github.com/audeering/audb/actions?query=workflow%3ATest
     :alt: Test status
-.. |coverage| image:: https://codecov.io/gh/audeering/audb/branch/master/graph/badge.svg?token=drrULW8vEG
+.. |coverage| image:: https://codecov.io/gh/audeering/audb/branch/main/graph/badge.svg?token=drrULW8vEG
     :target: https://codecov.io/gh/audeering/audb/
     :alt: code coverage
 .. |docs| image:: https://img.shields.io/pypi/v/audb?label=docs
     :target: https://audeering.github.io/audb/
     :alt: audb's documentation
 .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
     :target: https://github.com/audeering/audb/blob/master/LICENSE
```

### Comparing `audb-1.4.2/audb/__init__.py` & `audb-1.5.0/audb/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from audb.core.cache import default_cache_root
 from audb.core.config import config
 from audb.core.dependencies import Dependencies
 from audb.core.flavor import Flavor
 from audb.core.load import (
     load,
+    load_attachment,
     load_media,
     load_table,
 )
 from audb.core.load_to import load_to
 from audb.core.publish import publish
 from audb.core.repository import Repository
```

### Comparing `audb-1.4.2/audb/core/api.py` & `audb-1.5.0/audb/core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         table with database name as index,
         and backend, host, repository, version as columns
 
     Examples:
         >>> audb.available(only_latest=True)
                    backend                                    host   repository version
         name
-        emodb  artifactory  https://audeering.jfrog.io/artifactory  data-public   1.3.0
+        emodb  artifactory  https://audeering.jfrog.io/artifactory  data-public   1.4.1
 
     """  # noqa: E501
     databases = []
     for repository in config.REPOSITORIES:
         backend = audbackend.create(
             repository.backend,
             repository.host,
@@ -121,24 +121,24 @@
         mixdown,
         sampling_rate
         as columns
 
     Examples:
         >>> db = audb.load(
         ...     'emodb',
-        ...     version='1.3.0',
+        ...     version='1.4.1',
         ...     only_metadata=True,
         ...     full_path=False,
         ...     verbose=False,
         ... )
         >>> df = cached()
         >>> print(df.iloc[0].to_string())
         name                emodb
         flavor_id        d3b62a9b
-        version             1.3.0
+        version             1.4.1
         complete            False
         bit_depth            None
         channels             None
         format               None
         mixdown             False
         sampling_rate        None
 
@@ -240,15 +240,15 @@
             If not set :meth:`audb.default_cache_root` is used
         verbose: show debug messages
 
     Returns:
         dependency object
 
     Examples:
-        >>> deps = dependencies('emodb', version='1.3.0')
+        >>> deps = dependencies('emodb', version='1.4.1')
         >>> deps.version('db.emotion.csv')
         '1.1.0'
 
     """
     if version is None:
         version = latest_version(name)
 
@@ -319,21 +319,21 @@
 
     Returns:
         ``True`` if database flavor exists
 
     Examples:
         >>> db = audb.load(
         ...     'emodb',
-        ...     version='1.3.0',
+        ...     version='1.4.1',
         ...     only_metadata=True,
         ...     verbose=False,
         ... )
-        >>> audb.exists('emodb', version='1.3.0')
+        >>> audb.exists('emodb', version='1.4.1')
         True
-        >>> audb.exists('emodb', version='1.3.0', format='wav')
+        >>> audb.exists('emodb', version='1.4.1', format='wav')
         False
 
     """
     if version is None:
         version = latest_version(name)
 
     relative_flavor_path = flavor_path(
@@ -401,16 +401,16 @@
     Raises:
         ValueError: if a non-supported ``bit_depth``,
             ``format``,
             or ``sampling_rate``
             is requested
 
     Examples:
-        >>> flavor_path('emodb', version='1.3.0').split(os.path.sep)
-        ['emodb', '1.3.0', 'd3b62a9b']
+        >>> flavor_path('emodb', version='1.4.1').split(os.path.sep)
+        ['emodb', '1.4.1', 'd3b62a9b']
 
     """
     flavor = Flavor(
         channels=channels,
         format=format,
         mixdown=mixdown,
         bit_depth=bit_depth,
@@ -432,15 +432,15 @@
         version string
 
     Raises:
         RuntimeError: if no version exists for the requested database
 
     Examples:
         >>> latest_version('emodb')
-        '1.3.0'
+        '1.4.1'
 
     """
     vs = versions(name)
     if not vs:
         raise RuntimeError(
             f"Cannot find a version for database '{name}'.",
         )
@@ -559,15 +559,15 @@
     Returns:
         repository that contains the database
 
     Raises:
         RuntimeError: if database is not found
 
     Examples:
-        >>> audb.repository('emodb', '1.3.0')
+        >>> audb.repository('emodb', '1.4.1')
         Repository('data-public', 'https://audeering.jfrog.io/artifactory', 'artifactory')
 
     """  # noqa: E501
     return _lookup(name, version)[0]
 
 
 def versions(
@@ -579,15 +579,15 @@
         name: name of database
 
     Returns:
         list of versions
 
     Examples:
         >>> versions('emodb')
-        ['1.1.0', '1.1.1', '1.2.0', '1.3.0']
+        ['1.1.0', '1.1.1', '1.2.0', '1.3.0', '1.4.0', '1.4.1']
 
     """
     vs = []
     for repository in config.REPOSITORIES:
         backend = audbackend.create(
             repository.backend,
             repository.host,
```

### Comparing `audb-1.4.2/audb/core/cache.py` & `audb-1.5.0/audb/core/cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/audb/core/config.py` & `audb-1.5.0/audb/core/config.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/audb/core/define.py` & `audb-1.5.0/audb/core/define.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,19 +60,21 @@
 }
 
 
 class DependType:
     r"""Dependency file types."""
     META = 0
     MEDIA = 1
+    ATTACHMENT = 2
 
 
 DEPEND_TYPE_NAMES = {
     DependType.META: 'meta',
     DependType.MEDIA: 'media',
+    DependType.ATTACHMENT: 'attachment',
 }
 
 
 # Flavors
 class Format:
     r"""Media formats.
```

### Comparing `audb-1.4.2/audb/core/dependencies.py` & `audb-1.5.0/audb/core/dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 from audb.core import define
 
 
 class Dependencies:
     r"""Dependencies of a database.
 
-    :class:`audb.Dependencies` gathers all database files
+    :class:`audb.Dependencies` gathers
+    all database media, table, and attachment files
     and metadata about them
     in a single object.
     The metadata contains information
     about the single files
     like duration,
     but also what version of the file is required.
 
@@ -26,16 +27,16 @@
 
     Examples:
         >>> deps = Dependencies()
         >>> deps()
         Empty DataFrame
         Columns: [archive, bit_depth, channels, checksum, duration, format, removed, sampling_rate, type, version]
         Index: []
-        >>> # Request dependencies for emodb 1.3.0
-        >>> deps = audb.dependencies('emodb', version='1.3.0')
+        >>> # Request dependencies for emodb 1.4.1
+        >>> deps = audb.dependencies('emodb', version='1.4.1')
         >>> # List all files or archives
         >>> deps.files[:3]
         ['db.emotion.csv', 'db.files.csv', 'wav/03a01Fa.wav']
         >>> deps.archives[:2]
         ['005d2b91-5317-0c80-d602-6d55f0323f8c', '014f82d8-3491-fd00-7397-c3b2ac3b2875']
         >>> # Access properties for a given file
         >>> deps.archive('wav/03a01Fa.wav')
@@ -96,26 +97,54 @@
         return len(self._df)
 
     def __str__(self) -> str:
         return self._df.to_string()
 
     @property
     def archives(self) -> typing.List[str]:
-        r"""All archives (table and media).
+        r"""All media, table, attachment archives.
 
         Return:
             list of archives
 
         """
         archives = self._df.archive.to_list()
         return sorted(list(set(archives)))
 
     @property
+    def attachments(self) -> typing.List[str]:
+        r"""Attachment paths (can be a file or a folder).
+
+        Returns:
+            list of attachments
+
+        """
+        return list(
+            self._df[
+                self._df['type'] == define.DependType.ATTACHMENT
+            ].index
+        )
+
+    @property
+    def attachment_ids(self) -> typing.List[str]:
+        r"""Attachment IDs.
+
+        Returns:
+            list of attachment IDs
+
+        """
+        return list(
+            self._df[
+                self._df['type'] == define.DependType.ATTACHMENT
+            ].archive
+        )
+
+    @property
     def files(self) -> typing.List[str]:
-        r"""All files (table and media).
+        r"""All media, table, attachments.
 
         Returns:
             list of files
 
         """
         return list(self._df.index)
 
@@ -357,14 +386,45 @@
 
         Returns:
             version string
 
         """
         return self._df.version[file]
 
+    def _add_attachment(
+            self,
+            file: str,
+            version: str,
+            archive: str,
+            checksum: str,
+    ):
+        r"""Add or update attachment.
+
+        Args:
+            file: relative path of attachment
+            version: version string
+            archive: archive name without extension
+            checksum: checksum of file
+
+        """
+        format = audeer.file_extension(file).lower()
+
+        self._df.loc[file] = [
+            archive,                       # archive
+            0,                             # bit_depth
+            0,                             # channels
+            checksum,                      # checksum
+            0.0,                           # duration
+            format,                        # format
+            0,                             # removed
+            0,                             # sampling_rate
+            define.DependType.ATTACHMENT,  # type
+            version,                       # version
+        ]
+
     def _add_media(
             self,
             values: typing.Sequence[
                 typing.Tuple[
                     str,    # file
                     str,    # archive
                     int,    # bit_depth
@@ -487,32 +547,40 @@
 
         """
         field = define.DEPEND_FIELD_NAMES[define.DependField.VERSION]
         self._df.loc[files, field] = version
 
 
 def error_message_missing_object(
-        object_name: str,
+        object_type: str,
         missing_object_id: typing.Union[str, typing.Sequence],
         database_name: str = None,
         database_version: str = None,
 ) -> str:
     r"""Error message for missing objects.
 
     Args:
-        object_name: object that is supposed to contain ``missing_object_id``,
-            should be ``'table'`` or ``'media file'``
+        object_type: object that is supposed to contain ``missing_object_id``,
+            should be
+            ``'media'``,
+            ``'table'``
+            or ``'attachment'``
         missing_object_id: ID of missing object
         database_name: name of affected database
         database_version: name of affected database
 
     Returns:
         error message
 
     """
+    if object_type == 'media':
+        object_name = f'{object_type} file'
+    else:
+        object_name = object_type
+
     if isinstance(missing_object_id, str):
         msg = (
             f"Could not find a {object_name} "
             f"matching '{missing_object_id}'"
         )
     else:
         msg = (
@@ -520,117 +588,65 @@
             f"'{missing_object_id[0]}'"
         )
     if database_name is not None and database_version is not None:
         msg += f' in {database_name} v{database_version}'
     return msg
 
 
-def filter_media(
-        requested_media: typing.Optional[
-            typing.Union[str, typing.Sequence[str]]
-        ],
-        available_media: typing.Sequence[str],
-        database_name: str = None,
-        database_version: str = None,
-) -> typing.Sequence[str]:
-    r"""Filter media files by requested media.
-
-    Args:
-        requested_media: requested media files
-        available_media: sequence of media files
-        database_name: name of affected database
-        database_version: name of affected database
-
-    Returns:
-        list of media files inside the dependency object
-            matching ``requested_media``
-
-    """
-    if requested_media is None:
-        return available_media
-    elif len(requested_media) == 0:
-        return []
-
-    if isinstance(requested_media, str):
-        request = requested_media
-        pattern = re.compile(request)
-        requested_media = []
-        for m in available_media:
-            if pattern.search(m):
-                requested_media.append(m)
-        if len(requested_media) == 0:
-            msg = error_message_missing_object(
-                'media file',
-                request,
-                database_name,
-                database_version,
-            )
-            raise ValueError(msg)
-    else:
-        for media_file in requested_media:
-            if media_file not in available_media:
-                msg = error_message_missing_object(
-                    'media file',
-                    [media_file],
-                    database_name,
-                    database_version,
-                )
-                raise ValueError(msg)
-
-    return requested_media
-
-
-def filter_tables(
-        requested_tables: typing.Optional[
+def filter_deps(
+        requested_deps: typing.Optional[
             typing.Union[str, typing.Sequence[str]]
         ],
-        available_tables: typing.Sequence[str],
+        available_deps: typing.Sequence[str],
+        deps_type: str,
         database_name: str = None,
         database_version: str = None,
 ) -> typing.Sequence[str]:
-    r"""Filter dependency tables by requested tables.
+    r"""Filter dependency files by requested files.
 
     Args:
-        requested_tables: include only tables
+        requested_deps: include only media, tables
             matching the regular expression
             or provided in the list
-        available_tables: sequence of available table IDs
+        available_deps: sequence of available media files or tables
+        deps_type: ``'attachment'``, ``'media'`` or ``'table'``
         database_name: name of affected database
         database_version: name of affected database
 
     Returns:
-        list of table IDs inside the dependency object
-            matching ``requested_tables``
+        list of attachments, media or tables
+            inside the dependency object
+            matching ``requested_deps``
 
     """
-    if requested_tables is None:
-        return available_tables
-    elif len(requested_tables) == 0:
+    if requested_deps is None:
+        return available_deps
+    elif len(requested_deps) == 0:
         return []
 
-    if isinstance(requested_tables, str):
-        request = requested_tables
+    if isinstance(requested_deps, str):
+        request = requested_deps
         pattern = re.compile(request)
-        requested_tables = []
-        for table in available_tables:
-            if pattern.search(table):
-                requested_tables.append(table)
-        if len(requested_tables) == 0:
+        requested_deps = []
+        for dep in available_deps:
+            if pattern.search(dep):
+                requested_deps.append(dep)
+        if len(requested_deps) == 0:
             msg = error_message_missing_object(
-                'table',
+                deps_type,
                 request,
                 database_name,
                 database_version,
             )
             raise ValueError(msg)
     else:
-        for table in requested_tables:
-            if table not in available_tables:
+        for dep in requested_deps:
+            if dep not in available_deps:
                 msg = error_message_missing_object(
-                    'table',
-                    [table],
+                    deps_type,
+                    [dep],
                     database_name,
                     database_version,
                 )
                 raise ValueError(msg)
 
-    return requested_tables
+    return requested_deps
```

### Comparing `audb-1.4.2/audb/core/flavor.py` & `audb-1.5.0/audb/core/flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/audb/core/info.py` & `audb-1.5.0/audb/core/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,45 @@
 from audb.core.load import (
     filtered_dependencies,
     load_header,
     load_table,
 )
 
 
+def attachments(
+        name: str,
+        *,
+        version: str = None,
+        cache_root: str = None,
+) -> typing.Dict[str, audformat.Attachment]:
+    """Attachment(s) of database.
+
+    Args:
+        name: name of database
+        version: version of database
+        cache_root: cache folder where databases are stored.
+            If not set :meth:`audb.default_cache_root` is used
+
+    Returns:
+        attachments of database
+
+    Examples:
+        >>> list(attachments('emodb', version='1.4.1'))
+        ['bibtex']
+
+    """
+    db = header(
+        name,
+        version=version,
+        load_tables=False,
+        cache_root=cache_root,
+    )
+    return db.attachments
+
+
 def author(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
 ) -> str:
     """Author(s) of database.
@@ -27,15 +58,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         author(s) of database
 
     Examples:
-        >>> author('emodb', version='1.3.0')
+        >>> author('emodb', version='1.4.1')
         'Felix Burkhardt, Astrid Paeschke, Miriam Rolfes, Walter Sendlmeier, Benjamin Weiss'
 
     """  # noqa: E501
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -68,15 +99,15 @@
         bit depths
 
     Raises:
         ValueError: if table or media is requested
             that is not part of the database
 
     Examples:
-        >>> bit_depths('emodb', version='1.3.0')
+        >>> bit_depths('emodb', version='1.4.1')
         {16}
 
     """
     df = filtered_dependencies(name, version, media, tables, cache_root)
     return set(df[df.type == define.DependType.MEDIA].bit_depth)
 
 
@@ -104,15 +135,15 @@
         channel numbers
 
     Raises:
         ValueError: if table or media is requested
             that is not part of the database
 
     Examples:
-        >>> channels('emodb', version='1.3.0')
+        >>> channels('emodb', version='1.4.1')
         {1}
 
     """
     df = filtered_dependencies(name, version, media, tables, cache_root)
     return set(df[df.type == define.DependType.MEDIA].channels)
 
 
@@ -130,15 +161,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         description of database
 
     Examples:
-        >>> desc = description('emodb', version='1.3.0')
+        >>> desc = description('emodb', version='1.4.1')
         >>> desc.split('.')[0]  # show first sentence
         'Berlin Database of Emotional Speech'
 
     """
     db = header(
         name,
         version=version,
@@ -172,17 +203,17 @@
         duration
 
     Raises:
         ValueError: if table or media is requested
             that is not part of the database
 
     Examples:
-        >>> duration('emodb', version='1.3.0')
+        >>> duration('emodb', version='1.4.1')
         Timedelta('0 days 00:24:47.092187500')
-        >>> duration('emodb', version='1.3.0', media=['wav/03a01Fa.wav'])
+        >>> duration('emodb', version='1.4.1', media=['wav/03a01Fa.wav'])
         Timedelta('0 days 00:00:01.898250')
 
     """
     df = filtered_dependencies(name, version, media, tables, cache_root)
     return pd.to_timedelta(
         df[df.type == define.DependType.MEDIA].duration.sum(),
         unit='s',
@@ -203,15 +234,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         media files
 
     Examples:
-        >>> files('emodb', version='1.3.0')[:2]
+        >>> files('emodb', version='1.4.1')[:2]
         ['wav/03a01Fa.wav', 'wav/03a01Nc.wav']
 
     """
     deps = dependencies(name, version=version, cache_root=cache_root)
     return deps.media
 
 
@@ -239,15 +270,15 @@
         formats
 
     Raises:
         ValueError: if table or media is requested
             that is not part of the database
 
     Examples:
-        >>> formats('emodb', version='1.3.0')
+        >>> formats('emodb', version='1.4.1')
         {'wav'}
 
     """
     df = filtered_dependencies(name, version, media, tables, cache_root)
     return set(df[df.type == define.DependType.MEDIA].format)
 
 
@@ -269,15 +300,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         database object without table data
 
     Examples:
-        >>> db = header('emodb', version='1.3.0')
+        >>> db = header('emodb', version='1.4.1')
         >>> db.name
         'emodb'
 
     """
     db = load_header(name, version=version, cache_root=cache_root)
     if load_tables:
         for scheme in db.schemes.values():
@@ -307,15 +338,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         languages of database
 
     Examples:
-        >>> languages('emodb', version='1.3.0')
+        >>> languages('emodb', version='1.4.1')
         ['deu']
 
     """
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -338,15 +369,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         license of database
 
     Examples:
-        >>> license('emodb', version='1.3.0')
+        >>> license('emodb', version='1.4.1')
         'CC0-1.0'
 
     """
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -369,15 +400,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         license URL of database
 
     Examples:
-        >>> license_url('emodb', version='1.3.0')
+        >>> license_url('emodb', version='1.4.1')
         'https://creativecommons.org/publicdomain/zero/1.0/'
 
     """
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -387,28 +418,28 @@
 
 
 def media(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
-) -> typing.Dict:
+) -> typing.Dict[str, audformat.Media]:
     """Audio and video media of database.
 
     Args:
         name: name of database
         version: version of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         media of database
 
     Examples:
-        >>> media('emodb', version='1.3.0')
+        >>> media('emodb', version='1.4.1')
         microphone:
             {type: other, format: wav, channels: 1, sampling_rate: 16000}
 
     """
     db = header(
         name,
         version=version,
@@ -432,15 +463,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         meta information of database
 
     Examples:
-        >>> meta('emodb', version='1.3.0')
+        >>> meta('emodb', version='1.4.1')
         pdf:
           http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.130.8506&rep=rep1&type=pdf
 
     """
     db = header(
         name,
         version=version,
@@ -451,28 +482,28 @@
 
 
 def misc_tables(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
-) -> typing.Dict:
+) -> typing.Dict[str, audformat.MiscTable]:
     """Miscellaneous tables of database.
 
     Args:
         name: name of database
         version: version of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         miscellaneous tables of database
 
     Examples:
-        >>> list(misc_tables('emodb', version='1.3.0'))
+        >>> list(misc_tables('emodb', version='1.4.1'))
         ['speaker']
 
     """  # noqa: E501
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -495,15 +526,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         organization responsible for database
 
     Examples:
-        >>> organization('emodb', version='1.3.0')
+        >>> organization('emodb', version='1.4.1')
         'audEERING'
 
     """
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -513,28 +544,28 @@
 
 
 def raters(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
-) -> typing.Dict:
+) -> typing.Dict[str, audformat.Rater]:
     """Raters contributed to database.
 
     Args:
         name: name of database
         version: version of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         raters of database
 
     Examples:
-        >>> raters('emodb', version='1.3.0')
+        >>> raters('emodb', version='1.4.1')
         gold:
             {type: human}
 
     """
     db = header(
         name,
         version=version,
@@ -568,29 +599,29 @@
         sampling rates
 
     Raises:
         ValueError: if table or media is requested
             that is not part of the database
 
     Examples:
-        >>> sampling_rates('emodb', version='1.3.0')
+        >>> sampling_rates('emodb', version='1.4.1')
         {16000}
 
     """
     df = filtered_dependencies(name, version, media, tables, cache_root)
     return set(df[df.type == define.DependType.MEDIA].sampling_rate)
 
 
 def schemes(
         name: str,
         *,
         version: str = None,
         load_tables: bool = True,
         cache_root: str = None,
-) -> typing.Dict:
+) -> typing.Dict[str, audformat.Scheme]:
     """Schemes of database.
 
     Args:
         name: name of database
         version: version of database
         load_tables: if ``True``
             downloads misc tables
@@ -598,15 +629,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         schemes of database
 
     Examples:
-        >>> list(schemes('emodb', version='1.3.0'))
+        >>> list(schemes('emodb', version='1.4.1'))
         ['age', 'confidence', 'duration', 'emotion', 'gender', 'language', 'speaker', 'transcription']
 
     """  # noqa: E501
     db = header(
         name,
         version=version,
         load_tables=load_tables,
@@ -629,15 +660,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         source of database
 
     Examples:
-        >>> source('emodb', version='1.3.0')
+        >>> source('emodb', version='1.4.1')
         'http://emodb.bilderbar.info/download/download.zip'
 
     """
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -647,28 +678,28 @@
 
 
 def splits(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
-) -> typing.Dict:
+) -> typing.Dict[str, audformat.Split]:
     """Splits of database.
 
     Args:
         name: name of database
         version: version of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         splits of database
 
     Examples:
-        >>> splits('emodb', version='1.3.0')
+        >>> splits('emodb', version='1.4.1')
         test:
           {description: Unofficial speaker-independent test split, type: test}
         train:
           {description: Unofficial speaker-independent train split, type: train}
 
     """  # noqa: E501
     db = header(
@@ -681,28 +712,28 @@
 
 
 def tables(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
-) -> typing.Dict:
+) -> typing.Dict[str, audformat.Table]:
     """Tables of database.
 
     Args:
         name: name of database
         version: version of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         tables of database
 
     Examples:
-        >>> list(tables('emodb', version='1.3.0'))
+        >>> list(tables('emodb', version='1.4.1'))
         ['emotion', 'emotion.categories.test.gold_standard', 'emotion.categories.train.gold_standard', 'files']
 
     """  # noqa: E501
     db = header(
         name,
         version=version,
         load_tables=False,
@@ -725,15 +756,15 @@
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
 
     Returns:
         usage of database
 
     Examples:
-        >>> usage('emodb', version='1.3.0')
+        >>> usage('emodb', version='1.4.1')
         'unrestricted'
 
     """
     db = header(
         name,
         version=version,
         load_tables=False,
```

### Comparing `audb-1.4.2/audb/core/load.py` & `audb-1.5.0/audb/core/load.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,24 +20,23 @@
     database_cache_root,
     database_tmp_root,
     default_cache_root,
 )
 from audb.core.dependencies import (
     Dependencies,
     error_message_missing_object,
-    filter_media,
-    filter_tables,
+    filter_deps,
 )
 from audb.core.flavor import Flavor
 from audb.core.lock import FolderLock
 from audb.core.utils import lookup_backend
 
 
 CachedVersions = typing.Sequence[
-    typing.Tuple[audeer.LooseVersion, str, Dependencies],
+    typing.Tuple[audeer.StrictVersion, str, Dependencies],
 ]
 
 
 def _cached_versions(
         name: str,
         version: str,
         flavor: Flavor,
@@ -63,15 +62,15 @@
                 cache_root=cache_root,
             )
             # as it is more likely we find files
             # in newer versions, push them to front
             cached_versions.insert(
                 0,
                 (
-                    audeer.LooseVersion(row['version']),
+                    audeer.StrictVersion(row['version']),
                     str(flavor_root),
                     deps,
                 ),
             )
 
     return cached_versions
 
@@ -90,15 +89,15 @@
 
     for file in audeer.progress_bar(
             files,
             desc='Cached files',
             disable=not verbose,
     ):
         found = False
-        file_version = audeer.LooseVersion(deps.version(file))
+        file_version = audeer.StrictVersion(deps.version(file))
         for cache_version, cache_root, cache_deps in cached_versions:
             if cache_version >= file_version:
                 if file in cache_deps:
                     if deps.checksum(file) == cache_deps.checksum(file):
                         path = os.path.join(cache_root, file)
                         if flavor and flavor.format is not None:
                             path = audeer.replace_file_extension(
@@ -117,38 +116,44 @@
             cached_files.append((cache_root, file))
         else:
             missing_files.append(file)
 
     return cached_files, missing_files
 
 
-def _copy_file(
-        file: str,
+def _copy_path(
+        path: str,
         root_src: str,
         root_tmp: str,
         root_dst: str,
 ):
     r"""Copy file."""
-    src_path = os.path.join(root_src, file)
-    tmp_path = os.path.join(root_tmp, file)
-    dst_path = os.path.join(root_dst, file)
-    audeer.mkdir(os.path.dirname(tmp_path))
+    src_path = os.path.join(root_src, path)
+    tmp_path = os.path.join(root_tmp, path)
+    dst_path = os.path.join(root_dst, path)
+    if os.path.isdir(src_path):
+        shutil.copytree(src_path, tmp_path)
+    else:
+        audeer.mkdir(os.path.dirname(tmp_path))
+        shutil.copy(src_path, tmp_path)
     audeer.mkdir(os.path.dirname(dst_path))
-    shutil.copy(src_path, tmp_path)
     audeer.move_file(tmp_path, dst_path)
 
 
 def _database_check_complete(
         db: audformat.Database,
         db_root: str,
         flavor: Flavor,
         deps: Dependencies,
 ):
     def check() -> bool:
         complete = True
+        for attachment in deps.attachments:
+            if not os.path.exists(os.path.join(db_root, attachment)):
+                return False
         for table in deps.tables:
             if not os.path.exists(os.path.join(db_root, table)):
                 return False
         for media in deps.media:
             if not deps.removed(media):
                 path = os.path.join(db_root, media)
                 path = flavor.destination(path)
@@ -198,14 +203,218 @@
             durs.index,
             os.path.normpath,
         )
     durs.index = audformat.utils.expand_file_path(durs.index, db.root)
     db._files_duration = durs.to_dict()
 
 
+def _get_attachments_from_cache(
+        attachments: typing.Sequence[str],
+        db_root: str,
+        db: audformat.Database,
+        deps: Dependencies,
+        cached_versions: CachedVersions,
+        flavor: Flavor,
+        num_workers: int,
+        verbose: bool,
+) -> typing.Sequence[str]:
+    r"""Copy files from cache.
+
+    This function copies all files
+    associated with the requested attachments
+    from other cached versions
+    to the new database folder.
+
+    Args:
+        attachments: sequence of attachment IDs
+        db_root: database root
+        db: database object
+        deps: dependency object
+        cached_versions: object containing information
+            on existing cached versions of the database
+        flavor: database flavor object
+        num_workers: number of workers to use
+        verbose: if ``True`` show progress bar
+
+    Returns:
+        list of attachment IDs that couldn't be found in cache
+
+    """
+    db_root_cached = [x[1] for x in cached_versions]
+
+    paths = [db.attachments[attachment].path for attachment in attachments]
+
+    with FolderLock(
+            db_root_cached,
+            timeout=define.CACHED_VERSIONS_TIMEOUT,
+    ):
+
+        cached_paths, missing_paths = _cached_files(
+            paths,
+            deps,
+            cached_versions,
+            flavor,
+            verbose,
+        )
+        missing_attachments = [
+            deps.archive(path) for path in missing_paths
+        ]
+        db_root_tmp = database_tmp_root(db_root)
+
+        def job(cache_root: str, file: str):
+            _copy_path(file, cache_root, db_root_tmp, db_root)
+
+        audeer.run_tasks(
+            job,
+            params=[([root, path], {}) for root, path in cached_paths],
+            num_workers=num_workers,
+            progress_bar=verbose,
+            task_description='Copy attachments',
+        )
+
+        audeer.rmdir(db_root_tmp)
+
+    return missing_attachments
+
+
+def _get_files_from_cache(
+        files: typing.Sequence[str],
+        files_type: str,
+        db_root: str,
+        deps: Dependencies,
+        cached_versions: CachedVersions,
+        flavor: Flavor,
+        num_workers: int,
+        verbose: bool,
+) -> typing.Sequence[str]:
+    r"""Copy files from cache.
+
+    This function copies requested media files
+    or table files
+    from other cached versions
+    to the new database folder.
+
+    Args:
+        files: sequence of media files,
+            attachment IDs,
+            or table IDs
+        files_type: ``'media'``,
+            ``'table'``,
+        db_root: database root
+        deps: dependency object
+        cached_versions: object containing information
+            on existing cached versions of the database
+        flavor: database flavor object
+        num_workers: number of workers to use
+        verbose: if ``True`` show progress bar
+
+    Returns:
+        list of files that couldn't be found in cache
+
+    """
+    db_root_cached = [x[1] for x in cached_versions]
+
+    try:
+        with FolderLock(
+                db_root_cached,
+                timeout=define.CACHED_VERSIONS_TIMEOUT,
+        ):
+
+            cached_files, missing_files = _cached_files(
+                files,
+                deps,
+                cached_versions,
+                flavor,
+                verbose,
+            )
+            db_root_tmp = database_tmp_root(db_root)
+
+            # Tables are also cached as PKL files
+            if files_type == 'table':
+
+                def job(cache_root: str, file: str):
+                    file_pkl = audeer.replace_file_extension(
+                        file,
+                        audformat.define.TableStorageFormat.PICKLE,
+                    )
+                    _copy_path(file, cache_root, db_root_tmp, db_root)
+                    _copy_path(file_pkl, cache_root, db_root_tmp, db_root)
+
+            else:
+
+                def job(cache_root: str, file: str):
+                    _copy_path(file, cache_root, db_root_tmp, db_root)
+
+            audeer.run_tasks(
+                job,
+                params=[([root, file], {}) for root, file in cached_files],
+                num_workers=num_workers,
+                progress_bar=verbose,
+                task_description=f'Copy {files_type}',
+            )
+
+            audeer.rmdir(db_root_tmp)
+
+    except filelock.Timeout:
+        missing_files = files
+
+    return missing_files
+
+
+def _get_attachments_from_backend(
+        db: audformat.Database,
+        attachments: typing.Sequence[str],
+        db_root: str,
+        deps: Dependencies,
+        backend: audbackend.Backend,
+        num_workers: typing.Optional[int],
+        verbose: bool,
+):
+    r"""Load attachments from backend."""
+    db_root_tmp = database_tmp_root(db_root)
+
+    paths = [db.attachments[attachment].path for attachment in attachments]
+
+    # create folder tree to avoid race condition
+    # in os.makedirs when files are unpacked
+    utils.mkdir_tree(paths, db_root_tmp)
+
+    def job(path: str):
+        archive = deps.archive(path)
+        version = deps.version(path)
+        archive = backend.join(
+            db.name,
+            define.DEPEND_TYPE_NAMES[define.DependType.ATTACHMENT],
+            archive,
+        )
+        backend.get_archive(
+            archive,
+            db_root_tmp,
+            version,
+            tmp_root=db_root_tmp,
+        )
+        src_path = audeer.path(db_root_tmp, path)
+        dst_path = audeer.path(db_root, path)
+        audeer.mkdir(os.path.dirname(dst_path))
+        audeer.move_file(
+            src_path,
+            dst_path,
+        )
+
+    audeer.run_tasks(
+        job,
+        params=[([path], {}) for path in paths],
+        num_workers=num_workers,
+        progress_bar=verbose,
+        task_description='Load attachments',
+    )
+
+    audeer.rmdir(db_root_tmp)
+
+
 def _get_media_from_backend(
         name: str,
         media: typing.Sequence[str],
         db_root: str,
         flavor: typing.Optional[Flavor],
         deps: Dependencies,
         backend: audbackend.Backend,
@@ -283,61 +492,14 @@
         progress_bar=verbose,
         task_description='Load media',
     )
 
     audeer.rmdir(db_root_tmp)
 
 
-def _get_media_from_cache(
-        media: typing.Sequence[str],
-        db_root: str,
-        deps: Dependencies,
-        cached_versions: CachedVersions,
-        flavor: Flavor,
-        num_workers: int,
-        verbose: bool,
-) -> typing.Sequence[str]:
-    r"""Copy media from cache."""
-
-    db_root_cached = [x[1] for x in cached_versions]
-
-    try:
-        with FolderLock(
-                db_root_cached,
-                timeout=define.CACHED_VERSIONS_TIMEOUT,
-        ):
-
-            cached_media, missing_media = _cached_files(
-                media,
-                deps,
-                cached_versions,
-                flavor,
-                verbose,
-            )
-            db_root_tmp = database_tmp_root(db_root)
-
-            def job(cache_root: str, file: str):
-                _copy_file(file, cache_root, db_root_tmp, db_root)
-
-            audeer.run_tasks(
-                job,
-                params=[([root, file], {}) for root, file in cached_media],
-                num_workers=num_workers,
-                progress_bar=verbose,
-                task_description='Copy media',
-            )
-
-            audeer.rmdir(db_root_tmp)
-
-    except filelock.Timeout:
-        missing_media = media
-
-    return missing_media
-
-
 def _get_tables_from_backend(
         db: audformat.Database,
         tables: typing.Sequence[str],
         db_root: str,
         deps: Dependencies,
         backend: audbackend.Backend,
         num_workers: typing.Optional[int],
@@ -382,182 +544,191 @@
         progress_bar=verbose,
         task_description='Load tables',
     )
 
     audeer.rmdir(db_root_tmp)
 
 
-def _get_tables_from_cache(
-        tables: typing.Sequence[str],
-        db_root: str,
-        deps: Dependencies,
-        cached_versions: CachedVersions,
-        num_workers: int,
-        verbose: bool,
-) -> typing.Sequence[str]:
-    r"""Copy tables from cache."""
-
-    db_root_cached = [x[1] for x in cached_versions]
-
-    try:
-        with FolderLock(
-                db_root_cached,
-                timeout=define.CACHED_VERSIONS_TIMEOUT,
-        ):
-
-            cached_tables, missing_tables = _cached_files(
-                tables,
-                deps,
-                cached_versions,
-                None,
-                verbose,
-            )
-            db_root_tmp = database_tmp_root(db_root)
-
-            def job(cache_root: str, file: str):
-                file_pkl = audeer.replace_file_extension(
-                    file,
-                    audformat.define.TableStorageFormat.PICKLE,
-                )
-                _copy_file(file, cache_root, db_root_tmp, db_root)
-                _copy_file(file_pkl, cache_root, db_root_tmp, db_root)
-
-            audeer.run_tasks(
-                job,
-                params=[([root, file], {}) for root, file in cached_tables],
-                num_workers=num_workers,
-                progress_bar=verbose,
-                task_description='Copy tables',
-            )
-
-            audeer.rmdir(db_root_tmp)
-
-    except filelock.Timeout:
-        missing_tables = tables
-
-    return missing_tables
-
-
-def _load_media(
-        media: typing.Sequence[str],
+def _load_attachments(
+        attachments: typing.Sequence[str],
         backend: audbackend.Backend,
         db_root: str,
-        name: str,
+        db: audformat.Database,
         version: str,
         cached_versions: typing.Optional[CachedVersions],
         deps: Dependencies,
         flavor: Flavor,
         cache_root: str,
         num_workers: int,
         verbose: bool,
 ) -> typing.Optional[CachedVersions]:
-    r"""Load media files to cache.
+    r"""Load attachments to cache.
 
-    All media files not existing in cache yet
-    are copied from the corresponding flavor cache
-    folder of other versions of the database
-    or are downloaded from the backend.
+    Args:
+        attachments: list of attachment IDs
+        backend: backend object
+        db_root: database root
+        db: database object
+        version: database version
+        cached_versions: object representing cached versions
+            of the database
+        deps: database dependency object
+        flavor: database flavor object
+        cache_root: root path of cache
+        num_workers: number of workers to use
+        verbose: if ``True`` show progress bars
+            for each step
+
+    Returns:
+        cached versions object
+            if other versions of the database are found in cache
 
     """
-    missing_media = _missing_media(
-        db_root,
-        media,
-        flavor,
-        verbose,
-    )
-    if missing_media:
+    missing_attachments = []
+    for attachment in attachments:
+        path = db.attachments[attachment].path
+        path = audeer.path(db_root, path)
+        if not os.path.exists(path):
+            missing_attachments.append(attachment)
+
+    if missing_attachments:
         if cached_versions is None:
             cached_versions = _cached_versions(
-                name,
+                db.name,
                 version,
                 flavor,
                 cache_root,
             )
         if cached_versions:
-            missing_media = _get_media_from_cache(
-                missing_media,
+            missing_attachments = _get_attachments_from_cache(
+                missing_attachments,
                 db_root,
+                db,
                 deps,
                 cached_versions,
                 flavor,
                 num_workers,
                 verbose,
             )
-        if missing_media:
+        if missing_attachments:
             if backend is None:
-                backend = lookup_backend(name, version)
-            _get_media_from_backend(
-                name,
-                missing_media,
+                backend = lookup_backend(db.name, version)
+            _get_attachments_from_backend(
+                db,
+                missing_attachments,
                 db_root,
-                flavor,
                 deps,
                 backend,
                 num_workers,
                 verbose,
             )
 
     return cached_versions
 
 
-def _load_tables(
-        tables: typing.Sequence[str],
+def _load_files(
+        files: typing.Sequence[str],
+        files_type: str,
         backend: audbackend.Backend,
         db_root: str,
         db: audformat.Database,
         version: str,
         cached_versions: typing.Optional[CachedVersions],
         deps: Dependencies,
         flavor: Flavor,
         cache_root: str,
         num_workers: int,
         verbose: bool,
 ) -> typing.Optional[CachedVersions]:
-    r"""Load table files to cache.
+    r"""Load files to cache.
+
+    Loads media files,
+    attachment files,
+    or table files to database root folder.
 
-    All table files not existing in cache yet
+    All files not existing in cache yet
     are copied from the corresponding flavor cache
     folder of other versions of the database
     or are downloaded from the backend.
 
+    Args:
+        files: list of media files,
+            attachment files,
+            or table IDs
+        files_type: ``'media'``,
+            ``'table'``,
+            or ``'attachment'``
+        backend: backend object
+        db_root: database root
+        db: database object
+        version: database version
+        cached_versions: object representing cached versions
+            of the database
+        deps: database dependency object
+        flavor: database flavor object
+        cache_root: root path of cache
+        num_workers: number of workers to use
+        verbose: if ``True`` show progress bars
+            for each step
+
+    Returns:
+        cached versions object
+            if other versions of the database are found in cache
+
     """
-    missing_tables = _missing_tables(
+    missing_files = _missing_files(
+        files,
+        files_type,
         db_root,
-        tables,
+        flavor,
         verbose,
     )
-    if missing_tables:
+    if missing_files:
         if cached_versions is None:
             cached_versions = _cached_versions(
                 db.name,
                 version,
                 flavor,
                 cache_root,
             )
         if cached_versions:
-            missing_tables = _get_tables_from_cache(
-                missing_tables,
+            missing_files = _get_files_from_cache(
+                missing_files,
+                files_type,
                 db_root,
                 deps,
                 cached_versions,
+                flavor,
                 num_workers,
                 verbose,
             )
-        if missing_tables:
+        if missing_files:
             if backend is None:
                 backend = lookup_backend(db.name, version)
-            _get_tables_from_backend(
-                db,
-                missing_tables,
-                db_root,
-                deps,
-                backend,
-                num_workers,
-                verbose,
-            )
+            if files_type == 'media':
+                _get_media_from_backend(
+                    db.name,
+                    missing_files,
+                    db_root,
+                    flavor,
+                    deps,
+                    backend,
+                    num_workers,
+                    verbose,
+                )
+            elif files_type == 'table':
+                _get_tables_from_backend(
+                    db,
+                    missing_files,
+                    db_root,
+                    deps,
+                    backend,
+                    num_workers,
+                    verbose,
+                )
 
     return cached_versions
 
 
 def _misc_tables_used_in_scheme(
         db: audformat.Database,
 ) -> typing.List[str]:
@@ -566,50 +737,58 @@
     for scheme in db.schemes.values():
         if scheme.uses_table:
             misc_tables_used_in_scheme.append(scheme.labels)
 
     return list(set(misc_tables_used_in_scheme))
 
 
-def _missing_media(
+def _missing_files(
+        files: typing.Sequence[str],
+        files_type: str,
         db_root: str,
-        media: typing.Sequence[str],
         flavor: Flavor,
         verbose: bool,
 ) -> typing.Sequence[str]:
-    missing_media = []
-    for file in audeer.progress_bar(
-            media,
-            desc='Missing media',
-            disable=not verbose
-    ):
-        path = os.path.join(db_root, file)
-        if flavor.format is not None:
-            path = audeer.replace_file_extension(path, flavor.format)
-        if not os.path.exists(path):
-            missing_media.append(file)
-    return missing_media
+    r"""List missing files.
 
+    Checks for media files,
+    attachment files,
+    or table files
+    if they exist already in database root.
 
-def _missing_tables(
-        db_root: str,
-        tables: typing.Sequence[str],
-        verbose: bool,
-) -> typing.Sequence[str]:
-    missing_tables = []
-    for table in audeer.progress_bar(
-            tables,
-            desc='Missing tables',
+    Args:
+        db_root: database root
+        files: list of media files,
+            attachment files,
+            or table IDs
+        files_type: ``'media'``,
+            ``'table'``,
+            or ``'attachment'``
+        flavor: requested database flavor
+        verbose: if ``True`` show progress bar
+
+    Returns:
+        list of missing files
+
+    """
+    missing_files = []
+
+    if files_type == 'table':
+        files = [f'db.{file}.csv' for file in files]
+
+    for file in audeer.progress_bar(
+            files,
+            desc=f'Missing {files_type}',
             disable=not verbose,
     ):
-        file = f'db.{table}.csv'
         path = os.path.join(db_root, file)
         if not os.path.exists(path):
-            missing_tables.append(file)
-    return missing_tables
+            missing_files.append(file)
+
+    return missing_files
 
 
 def _remove_media(
         db: audformat.Database,
         deps: Dependencies,
         num_workers: int,
         verbose: bool,
@@ -701,15 +880,15 @@
     """
     deps = dependencies(name, version=version, cache_root=cache_root)
     if tables is None and media is None:
         df = deps()
     else:
         # Load header to get list of tables
         db = load_header(name, version=version, cache_root=cache_root)
-        tables = filter_tables(tables, list(db))
+        tables = filter_deps(tables, list(db), 'table')
         tables = [t for t in tables if t not in list(db.misc_tables)]
         # Gather media files from tables
         available_media = []
         for table in tables:
             df = load_table(
                 name,
                 table,
@@ -718,15 +897,15 @@
                 verbose=False,
             )
             available_media += list(
                 df.index.get_level_values('file').unique()
             )
 
         if len(available_media) > 0:
-            media = filter_media(media, deps.media, name, version)
+            media = filter_deps(media, deps.media, 'media', name, version)
             available_media = [
                 m for m in media
                 if m in list(set(available_media))
             ]
         df = deps().loc[available_media]
 
     return df
@@ -738,14 +917,15 @@
         version: str = None,
         only_metadata: bool = False,
         bit_depth: int = None,
         channels: typing.Union[int, typing.Sequence[int]] = None,
         format: str = None,
         mixdown: bool = False,
         sampling_rate: int = None,
+        attachments: typing.Union[str, typing.Sequence[str]] = None,
         tables: typing.Union[str, typing.Sequence[str]] = None,
         media: typing.Union[str, typing.Sequence[str]] = None,
         removed_media: bool = False,
         full_path: bool = True,
         cache_root: str = None,
         num_workers: typing.Optional[int] = 1,
         timeout: float = -1,
@@ -772,31 +952,51 @@
     I.e. filtering meta files, may also remove media files.
     Likewise, references to missing media files will be removed, too.
     I.e. filtering media files, may also remove entries from the meta files.
 
     Args:
         name: name of database
         version: version string, latest if ``None``
-        only_metadata: load only metadata
+        only_metadata: load only header and tables of database
         bit_depth: bit depth, one of ``16``, ``24``, ``32``
         channels: channel selection, see :func:`audresample.remix`.
             Note that media files with too few channels
             will be first upsampled by repeating the existing channels.
             E.g. ``channels=[0, 1]`` upsamples all mono files to stereo,
             and ``channels=[1]`` returns the second channel
             of all multi-channel files
             and all mono files
         format: file format, one of ``'flac'``, ``'wav'``
         mixdown: apply mono mix-down
         sampling_rate: sampling rate in Hz, one of
             ``8000``, ``16000``, ``22500``, ``44100``, ``48000``
-        tables: include only tables matching the regular expression or
-            provided in the list
-        media: include only media matching the regular expression or
-            provided in the list
+        attachments: load only attachment files
+            for the attachments
+            matching the regular expression
+            or provided in the list.
+            If set to ``[]`` no attachments are loaded
+        tables: load only tables and misc tables
+            matching the regular expression
+            or provided in the list.
+            Media files not referenced
+            in the selected tables
+            are automatically excluded, too.
+            If set to ``[]``
+            no tables and media files are loaded.
+            Misc tables used in schemes are always loaded
+        media: load only media files
+            matching the regular expression
+            or provided in the list.
+            Excluded media files are
+            automatically removed from the tables, too.
+            This may result in empty tables.
+            If set to ``[]``
+            no media files are loaded
+            and all tables except
+            misc tables will be empty
         removed_media: keep rows that reference removed media
         full_path: replace relative with absolute file paths
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
         num_workers: number of parallel jobs or 1 for sequential
             processing. If ``None`` will be set to the number of
             processors on the machine multiplied by 5
@@ -806,25 +1006,25 @@
             database can be accessed
         verbose: show debug messages
 
     Returns:
         database object
 
     Raises:
-        ValueError: if table or media is requested
+        ValueError: if attachment, table or media is requested
             that is not part of the database
         ValueError: if a non-supported ``bit_depth``,
             ``format``,
             or ``sampling_rate``
             is requested
 
     Examples:
         >>> db = audb.load(
         ...     'emodb',
-        ...     version='1.3.0',
+        ...     version='1.4.1',
         ...     tables=['emotion', 'files'],
         ...     only_metadata=True,
         ...     full_path=False,
         ...     verbose=False,
         ... )
         >>> list(db.tables)
         ['emotion', 'files']
@@ -865,16 +1065,40 @@
                 version,
                 flavor=flavor,
                 add_audb_meta=True,
             )
 
             db_is_complete = _database_is_complete(db)
 
+            # load attachments
+            if not db_is_complete and not only_metadata:
+
+                # filter attachments
+                requested_attachments = filter_deps(
+                    attachments,
+                    db.attachments,
+                    'attachment',
+                )
+
+                cached_versions = _load_attachments(
+                    requested_attachments,
+                    backend,
+                    db_root,
+                    db,
+                    version,
+                    cached_versions,
+                    deps,
+                    flavor,
+                    cache_root,
+                    num_workers,
+                    verbose,
+                )
+
             # filter tables (convert regexp pattern to list of tables)
-            requested_tables = filter_tables(tables, list(db))
+            requested_tables = filter_deps(tables, list(db), 'table')
 
             # add/split into misc tables used in a scheme
             # and all other (misc) tables
             requested_misc_tables = _misc_tables_used_in_scheme(db)
             requested_tables = [
                 table for table in requested_tables
                 if table not in requested_misc_tables
@@ -884,16 +1108,17 @@
             if not db_is_complete:
                 for _tables in [
                         requested_misc_tables,
                         requested_tables,
                 ]:
                     # need to load misc tables used in a scheme first
                     # as loading is done in parallel
-                    cached_versions = _load_tables(
+                    cached_versions = _load_files(
                         _tables,
+                        'table',
                         backend,
                         db_root,
                         db,
                         version,
                         cached_versions,
                         deps,
                         flavor,
@@ -908,23 +1133,30 @@
                 db.pick_tables(requested_tables)
 
             # load tables
             for table in requested_tables:
                 db[table].load(os.path.join(db_root, f'db.{table}'))
 
             # filter media
-            requested_media = filter_media(media, db.files, name, version)
+            requested_media = filter_deps(
+                media,
+                db.files,
+                'media',
+                name,
+                version,
+            )
 
             # load missing media
             if not db_is_complete and not only_metadata:
-                cached_versions = _load_media(
+                cached_versions = _load_files(
                     requested_media,
+                    'media',
                     backend,
                     db_root,
-                    name,
+                    db,
                     version,
                     cached_versions,
                     deps,
                     flavor,
                     cache_root,
                     num_workers,
                     verbose,
@@ -966,14 +1198,105 @@
 
     except filelock.Timeout:
         utils.timeout_warning()
 
     return db
 
 
+def load_attachment(
+        name: str,
+        attachment: str,
+        *,
+        version: str = None,
+        cache_root: str = None,
+        verbose: bool = True,
+) -> typing.List[str]:
+    r"""Load attachment(s) of database.
+
+    Args:
+        name: name of database
+        attachment: attachment ID to load
+        version: version of database
+        cache_root: cache folder where databases are stored.
+            If not set :meth:`audb.default_cache_root` is used
+        verbose: show debug messages
+
+    Returns:
+        list of file paths belonging to attachment
+
+    Raises:
+        ValueError: if an attachment ID is requested
+            that is not part of the database
+
+    Examples:
+        >>> paths = load_attachment(
+        ...     'emodb',
+        ...     'bibtex',
+        ...     version='1.4.1',
+        ...     verbose=False,
+        ... )
+        >>> os.path.basename(paths[0])
+        'burkhardt2005emodb.bib'
+
+    """
+    if version is None:
+        version = latest_version(name)
+
+    db_root = database_cache_root(name, version, cache_root)
+
+    if verbose:  # pragma: no cover
+        print(f'Get:   {name} v{version}')
+        print(f'Cache: {db_root}')
+
+    deps = dependencies(
+        name,
+        version=version,
+        cache_root=cache_root,
+        verbose=verbose,
+    )
+
+    if attachment not in deps.archives:
+        msg = error_message_missing_object(
+            'attachment',
+            [attachment],
+            name,
+            version,
+        )
+        raise ValueError(msg)
+
+    with FolderLock(db_root):
+
+        # Start with database header
+        db, backend = load_header_to(
+            db_root,
+            name,
+            version,
+        )
+
+        # Load attachment
+        _load_attachments(
+            [attachment],
+            backend,
+            db_root,
+            db,
+            version,
+            None,
+            deps,
+            Flavor(),
+            cache_root,
+            1,
+            verbose,
+        )
+
+    attachment_files = db.attachments[attachment].files
+    attachment_files = [audeer.path(db_root, a) for a in attachment_files]
+
+    return attachment_files
+
+
 def load_header(
         name: str,
         *,
         version: str = None,
         cache_root: str = None,
 ) -> audformat.Database:
     r"""Load header of database.
@@ -1120,20 +1443,20 @@
             or ``sampling_rate``
             is requested
 
     Examples:
         >>> paths = load_media(
         ...     'emodb',
         ...     ['wav/03a01Fa.wav'],
-        ...     version='1.3.0',
+        ...     version='1.4.1',
         ...     format='flac',
         ...     verbose=False,
         ... )
         >>> paths[0].split(os.path.sep)[-5:]
-        ['emodb', '1.3.0', '40bb2241', 'wav', '03a01Fa.flac']
+        ['emodb', '1.4.1', '40bb2241', 'wav', '03a01Fa.flac']
 
     """
     media = audeer.to_list(media)
     if len(media) == 0:
         return []
 
     if version is None:
@@ -1160,15 +1483,15 @@
         verbose=verbose,
     )
 
     available_files = deps.media
     for media_file in media:
         if media_file not in available_files:
             msg = error_message_missing_object(
-                'media file',
+                'media',
                 [media_file],
                 name,
                 version,
             )
             raise ValueError(msg)
 
     try:
@@ -1183,19 +1506,20 @@
                 add_audb_meta=True,
             )
 
             db_is_complete = _database_is_complete(db)
 
             # load missing media
             if not db_is_complete:
-                _load_media(
+                _load_files(
                     media,
+                    'media',
                     backend,
                     db_root,
-                    name,
+                    db,
                     version,
                     None,
                     deps,
                     flavor,
                     cache_root,
                     num_workers,
                     verbose,
@@ -1233,14 +1557,15 @@
     This will not download any media files
     to your disk,
     but share the cache with :func:`audb.load`.
 
     Args:
         name: name of database
         table: load table from database
+        version: version of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used
         num_workers: number of parallel jobs or 1 for sequential
             processing. If ``None`` will be set to the number of
             processors on the machine multiplied by 5
         verbose: show debug messages
 
@@ -1251,15 +1576,15 @@
         ValueError: if a table is requested
             that is not part of the database
 
     Examples:
         >>> df = load_table(
         ...     'emodb',
         ...     'emotion',
-        ...     version='1.3.0',
+        ...     version='1.4.1',
         ...     verbose=False,
         ... )
         >>> df[:3]
                            emotion  emotion.confidence
         file
         wav/03a01Fa.wav  happiness                0.90
         wav/03a01Nc.wav    neutral                1.00
@@ -1304,16 +1629,17 @@
         tables = _misc_tables_used_in_scheme(db) + [table]
         for table in tables:
             table_file = os.path.join(db_root, f'db.{table}')
             if not (
                     os.path.exists(f'{table_file}.csv')
                     or os.path.exists(f'{table_file}.pkl')
             ):
-                _load_tables(
+                _load_files(
                     [table],
+                    'table',
                     backend,
                     db_root,
                     db,
                     version,
                     None,
                     deps,
                     Flavor(),
```

### Comparing `audb-1.4.2/audb/core/load_to.py` & `audb-1.5.0/audb/core/load_to.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import glob
 import os
 import typing
 
 import audbackend
 import audeer
 import audformat
 
@@ -15,22 +14,47 @@
 from audb.core.dependencies import Dependencies
 from audb.core.load import (
     database_tmp_root,
     load_header_to,
 )
 
 
+def _find_attachments(
+        db_root: str,
+        deps: Dependencies,
+) -> typing.List[str]:
+    r"""Find missing attachments."""
+
+    attachments = []
+
+    for file in deps.attachments:
+        full_file = os.path.join(db_root, file)
+        if not os.path.exists(full_file):
+            attachments.append(file)
+
+    return attachments
+
+
 def _find_media(
         db: audformat.Database,
         db_root: str,
         deps: Dependencies,
         num_workers: typing.Optional[int],
         verbose: bool,
 ) -> typing.List[str]:
-    r"""Find altered and new media."""
+    r"""Find missing media.
+
+    Collects all media files present in ``db.files``,
+    but not in ``db_root``.
+    This will find missing files,
+    but also altered files
+    as those have been deleted
+    in a previous step.
+
+    """
 
     media = []
 
     def job(file: str):
         if not deps.removed(file):
             full_file = os.path.join(db_root, file)
             if not os.path.exists(full_file):
@@ -50,41 +74,92 @@
 def _find_tables(
         db_header: audformat.Database,
         db_root: str,
         deps: Dependencies,
         num_workers: typing.Optional[int],
         verbose: bool,
 ) -> typing.List[str]:
+    r"""Find missing tables.
+
+    Collects all tables and misc tables
+    present in ``db_header``,
+    but not in ``db_root``.
+    This will find missing tables,
+    but also altered tables
+    as those have been deleted
+    in a previous step.
+
+    """
 
     tables = []
 
     def job(table: str):
         file = f'db.{table}.csv'
         full_file = os.path.join(db_root, file)
         if not os.path.exists(full_file):
             tables.append(file)
-        else:
-            checksum = audbackend.md5(full_file)
-            # if the table already exists
-            # we have to compare checksum
-            # in case it was altered by flavor
-            if checksum != deps.checksum(file):  # pragma: no cover
-                tables.append(file)
 
     audeer.run_tasks(
         job,
         params=[([table], {}) for table in list(db_header)],
         num_workers=num_workers,
         progress_bar=verbose,
         task_description='Find tables',
     )
 
     return tables
 
 
+def _get_attachments(
+        paths: typing.Sequence[str],
+        db_root: str,
+        db_root_tmp: str,
+        db_name: str,
+        deps: Dependencies,
+        backend: audbackend.Backend,
+        num_workers: typing.Optional[int],
+        verbose: bool,
+):
+    r"""Load attachments from backend."""
+
+    # create folder tree to avoid race condition
+    # in os.makedirs when files are unpacked
+    utils.mkdir_tree(paths, db_root)
+    utils.mkdir_tree(paths, db_root_tmp)
+
+    def job(path: str):
+        archive = deps.archive(path)
+        version = deps.version(path)
+        archive = backend.join(
+            db_name,
+            define.DEPEND_TYPE_NAMES[define.DependType.ATTACHMENT],
+            archive,
+        )
+        backend.get_archive(
+            archive,
+            db_root_tmp,
+            version,
+            tmp_root=db_root_tmp,
+        )
+        src_path = audeer.path(db_root_tmp, path)
+        dst_path = audeer.path(db_root, path)
+        audeer.move_file(
+            src_path,
+            dst_path,
+        )
+
+    audeer.run_tasks(
+        job,
+        params=[([path], {}) for path in paths],
+        num_workers=num_workers,
+        progress_bar=verbose,
+        task_description='Load attachments',
+    )
+
+
 def _get_media(
         media: typing.List[str],
         db_root: str,
         db_root_tmp: str,
         db_name: str,
         deps: Dependencies,
         backend: audbackend.Backend,
@@ -142,15 +217,15 @@
         verbose: bool,
 ):
 
     def job(table: str):
         # If a pickled version of the table exists,
         # we have to remove it to make sure that
         # later on the new CSV tables are loaded.
-        # This can happen if we upgrading an existing
+        # This can happen if we upgrade an existing
         # database to a different version.
         path_pkl = os.path.join(
             db_root, table
         )[:-3] + audformat.define.TableStorageFormat.PICKLE
         if os.path.exists(path_pkl):
             os.remove(path_pkl)
         archive = backend.join(
@@ -187,47 +262,14 @@
             full_file = os.path.join(root, file)
             if os.path.isdir(full_file):
                 _remove_empty_dirs(full_file)
 
     os.rmdir(root)
 
 
-def _save_database(
-        db: audformat.Database,
-        db_root: str,
-        db_root_tmp: str,
-        num_workers: typing.Optional[int],
-        verbose: bool,
-):
-
-    for storage_format in [
-        audformat.define.TableStorageFormat.CSV,
-        audformat.define.TableStorageFormat.PICKLE,
-    ]:
-        db.save(
-            db_root_tmp,
-            storage_format=storage_format,
-            update_other_formats=False,
-            num_workers=num_workers,
-            verbose=verbose,
-        )
-        audeer.move_file(
-            os.path.join(db_root_tmp, define.HEADER_FILE),
-            os.path.join(db_root, define.HEADER_FILE),
-        )
-        for path in glob.glob(
-                os.path.join(db_root_tmp, f'*.{storage_format}')
-        ):
-            file = os.path.relpath(path, db_root_tmp)
-            audeer.move_file(
-                os.path.join(db_root_tmp, file),
-                os.path.join(db_root, file),
-            )
-
-
 def load_to(
         root: str,
         name: str,
         *,
         version: str = None,
         only_metadata: bool = False,
         cache_root: str = None,
@@ -244,15 +286,15 @@
     it will upgrade to the requested version.
     Unchanged files will be skipped.
 
     Args:
         root: target directory
         name: name of database
         version: version string, latest if ``None``
-        only_metadata: load only metadata
+        only_metadata: load only header and tables of database
         cache_root: cache folder where databases are stored.
             If not set :meth:`audb.default_cache_root` is used.
             Only used to read the dependencies of the requested version
         num_workers: number of parallel jobs or 1 for sequential
             processing. If ``None`` will be set to the number of
             processors on the machine multiplied by 5
         verbose: show debug messages
@@ -274,34 +316,58 @@
     deps = dependencies(
         name,
         version=version,
         cache_root=cache_root,
         verbose=verbose,
     )
     if update:
-        files = deps.tables if only_metadata else deps.files
+        if only_metadata:
+            files = deps.tables
+        else:
+            files = deps.attachments + deps.files
         for file in files:
             full_file = os.path.join(db_root, file)
             if os.path.exists(full_file):
-                checksum = audbackend.md5(full_file)
+                checksum = utils.md5(full_file)
                 if checksum != deps.checksum(file):
-                    os.remove(full_file)
+                    if os.path.isdir(full_file):
+                        audeer.rmdir(full_file)
+                    else:
+                        os.remove(full_file)
 
     # load database header without tables from backend
 
     db_header, backend = load_header_to(
         db_root_tmp,
         name,
         version,
         overwrite=True,
     )
+    db_header.save(db_root_tmp, header_only=True)
+
+    # get altered and new attachments
+
+    if not only_metadata:
+        attachments = _find_attachments(
+            db_root,
+            deps,
+        )
+        _get_attachments(
+            attachments,
+            db_root,
+            db_root_tmp,
+            name,
+            deps,
+            backend,
+            num_workers,
+            verbose,
+        )
 
     # get altered and new tables
 
-    db_header.save(db_root_tmp, header_only=True)
     tables = _find_tables(db_header, db_root, deps, num_workers, verbose)
     _get_tables(tables, db_root, db_root_tmp, name, deps, backend,
                 num_workers, verbose)
 
     # load database
 
     # move header to root and load database ...
@@ -315,14 +381,15 @@
             num_workers=num_workers,
             verbose=verbose,
         )
     except (KeyboardInterrupt, Exception):  # pragma: no cover
         # make sure to remove header if user interrupts
         os.remove(os.path.join(db_root, define.HEADER_FILE))
         raise
+
     # afterwards remove header to avoid the database
     # can be loaded before download is complete
     os.remove(os.path.join(db_root, define.HEADER_FILE))
 
     # get altered and new media files
 
     if not only_metadata:
@@ -335,24 +402,29 @@
     dep_path_tmp = os.path.join(db_root_tmp, define.DEPENDENCIES_FILE)
     deps.save(dep_path_tmp)
     audeer.move_file(
         dep_path_tmp,
         os.path.join(db_root, define.DEPENDENCIES_FILE),
     )
 
-    # save database and remove the temporal directory
-    # to signal all files were correctly loaded
+    # save database and PKL tables
+
+    db.save(
+        db_root,
+        storage_format=audformat.define.TableStorageFormat.PICKLE,
+        update_other_formats=False,
+        num_workers=num_workers,
+        verbose=verbose,
+    )
 
-    _save_database(db, db_root, db_root_tmp, num_workers, verbose)
+    # remove the temporal directory
+    # to signal all files were correctly loaded
     try:
         _remove_empty_dirs(db_root_tmp)
     except OSError:  # pragma: no cover
         raise RuntimeError(
             'Could not remove temporary directory, '
             'probably there are some leftover files. '
             'This should not happen.'
         )
 
-    # Force root to not point to tmp folder
-    db._root = db_root
-
     return db
```

### Comparing `audb-1.4.2/audb/core/lock.py` & `audb-1.5.0/audb/core/lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/audb/core/publish.py` & `audb-1.5.0/audb/core/publish.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import collections
 import os
+import re
 import shutil
 import tempfile
 import typing
 
 import audbackend
 import audeer
 import audformat
 import audiofile
 
 from audb.core import define
+from audb.core import utils
 from audb.core.api import dependencies
 from audb.core.dependencies import Dependencies
 from audb.core.repository import Repository
 
 
 def _check_for_duplicates(
         db: audformat.Database,
@@ -64,42 +66,102 @@
             error_msg += "."
         else:
             error_msg = error_msg[:-1]
             error_msg += ", ...]."
         raise RuntimeError(error_msg)
 
 
-def _find_tables(
+def _find_attachments(
         db: audformat.Database,
         db_root: str,
         version: str,
         deps: Dependencies,
         verbose: bool,
 ) -> typing.List[str]:
-    r"""Find altered, new or removed tables and update 'deps'."""
+    r"""Find altered, new or removed attachments and update 'deps'."""
 
-    # release dependencies to removed tables
+    for attachment_id in deps.attachment_ids:
+        if attachment_id not in db.attachments:
+            path = deps._df.index[deps._df.archive == attachment_id][0]
+            deps._drop(path)
+
+    # check attachments are valid
+    db_files = list(db.files) + [f'db.{t}.csv' for t in db.tables]
+    for attachment_id in db.attachments:
+
+        path = db.attachments[attachment_id].path
+        for file in db_files:
+            if file.startswith(path):
+                raise RuntimeError(
+                    "An attachment must not "
+                    "overlap with media or tables. "
+                    f"But attachment '{attachment_id}' "
+                    f"contains '{file}'."
+                )
 
-    db_tables = [f'db.{table}.csv' for table in list(db)]
-    for file in set(deps.tables) - set(db_tables):
-        deps._drop(file)
+        path = audeer.path(db.root, db.attachments[attachment_id].path)
+        if os.path.exists(path):
+            if os.path.isdir(path):
+                folders = audeer.list_dir_names(
+                    path,
+                    recursive=True,
+                    hidden=True,
+                    basenames=True,
+                )
+                for folder in folders:
+                    if not os.listdir(audeer.path(path, folder)):
+                        raise RuntimeError(
+                            "An attachment must not "
+                            "contain empty sub-folders. "
+                            f"But attachment '{attachment_id}' "
+                            f"contains the empty sub-folder '{folder}'."
+                        )
 
-    tables = []
-    for table in audeer.progress_bar(
-            list(db),
-            desc='Find tables',
+            files = db.attachments[attachment_id].files
+            if len(files) == 0:
+                raise RuntimeError(
+                    "An attached folder must "
+                    "contain at least one file. "
+                    f"But attachment '{attachment_id}' "
+                    "points to an empty folder."
+                )
+
+    # add dependencies to new or updated attachments
+    attachment_ids = []
+    for attachment_id in audeer.progress_bar(
+            list(db.attachments),
+            desc='Find attachments',
             disable=not verbose,
     ):
-        file = f'db.{table}.csv'
-        checksum = audbackend.md5(os.path.join(db_root, file))
-        if file not in deps or checksum != deps.checksum(file):
-            deps._add_meta(file, version, table, checksum)
-            tables.append(table)
+        # use one archive per attachment ID
+        path = db.attachments[attachment_id].path
+        if not os.path.exists(audeer.path(db_root, path)):
+            if path not in deps:
+                # Raise FileNotFoundError
+                #
+                # Attachment is not in deps,
+                # but its path does not exist on disk either.
+                # We call its `files` property
+                # which raises a FileNotFoundError in this case
+                db.attachments[attachment_id].files
+        else:
+            checksum = utils.md5(audeer.path(db_root, path))
+            if (
+                    path not in deps
+                    or checksum != deps.checksum(path)
+            ):
+                deps._add_attachment(
+                    file=path,
+                    version=version,
+                    archive=attachment_id,
+                    checksum=checksum,
+                )
+                attachment_ids.append(attachment_id)
 
-    return tables
+    return list(attachment_ids)
 
 
 def _find_media(
         db: audformat.Database,
         db_root: str,
         db_root_files: typing.Set[str],
         version: str,
@@ -123,14 +185,21 @@
     db_media_in_root = db_media.intersection(db_root_files)
 
     # update version of altered media and insert new ones
 
     def job(file):
         path = os.path.join(db_root, file)
         if file not in deps:
+            # assert lowercase file extensions
+            ext = audeer.file_extension(file)
+            if ext.lower() != ext:
+                raise RuntimeError(
+                    "The file extension of a media file must be lowercase, "
+                    f"but '{file}' includes at least one uppercase letter."
+                )
             checksum = audbackend.md5(path)
             if file in archives:
                 archive = archives[file]
             else:
                 archive = audeer.uid(from_string=file.replace('\\', '/'))
             values = _media_values(
                 db_root,
@@ -171,14 +240,44 @@
     for file in deps.media:
         if not deps.removed(file) and deps.version(file) == version:
             media_archives.add(deps.archive(file))
 
     return media_archives
 
 
+def _find_tables(
+        db: audformat.Database,
+        db_root: str,
+        version: str,
+        deps: Dependencies,
+        verbose: bool,
+) -> typing.List[str]:
+    r"""Find altered, new or removed tables and update 'deps'."""
+
+    # release dependencies to removed tables
+
+    db_tables = [f'db.{table}.csv' for table in list(db)]
+    for file in set(deps.tables) - set(db_tables):
+        deps._drop(file)
+
+    tables = []
+    for table in audeer.progress_bar(
+            list(db),
+            desc='Find tables',
+            disable=not verbose,
+    ):
+        file = f'db.{table}.csv'
+        checksum = audbackend.md5(os.path.join(db_root, file))
+        if file not in deps or checksum != deps.checksum(file):
+            deps._add_meta(file, version, table, checksum)
+            tables.append(table)
+
+    return tables
+
+
 def _get_root_files(
         db_root: str,
 ) -> typing.Set[str]:
     r"""Return list of files in root directory."""
 
     db_root_files = audeer.list_file_names(
         db_root,
@@ -230,14 +329,41 @@
         0,  # removed
         sampling_rate,
         define.DependType.MEDIA,
         version,
     )
 
 
+def _put_attachments(
+        attachments: typing.List[str],
+        db_root: str,
+        db: audformat.Database,
+        version: str,
+        backend: audbackend.Backend,
+        num_workers: typing.Optional[int],
+        verbose: bool,
+):
+    def job(attachment_id: str):
+        archive_file = backend.join(
+            db.name,
+            define.DEPEND_TYPE_NAMES[define.DependType.ATTACHMENT],
+            attachment_id,
+        )
+        files = db.attachments[attachment_id].files
+        backend.put_archive(db_root, files, archive_file, version)
+
+    audeer.run_tasks(
+        job,
+        params=[([attachment_id], {}) for attachment_id in attachments],
+        num_workers=num_workers,
+        progress_bar=verbose,
+        task_description='Put attachments',
+    )
+
+
 def _put_media(
         media_archives: typing.Set[str],
         db_root: str,
         db_name: str,
         version: str,
         previous_version: typing.Optional[str],
         deps: Dependencies,
@@ -380,14 +506,21 @@
 
     Setting ``previous_version=None`` allows you
     to start from scratch and upload all files
     even if an older versions exist.
     In this case you don't call :func:`audb.load_to`
     before running :func:`audb.publish`.
 
+    Handling of audio formats
+    is based on the file extension
+    in :mod:`audb`.
+    This means the file extension must be lowercase
+    and should match the audio format of the file,
+    e.g. ``.wav``.
+
     When canceling :func:`audb.publish`
     during publication
     you can restart it afterwards.
     It will continue from the current state,
     but you might need overwrite permissions
     in addition to write permissions
     on the backend.
@@ -420,29 +553,45 @@
 
     Returns:
         dependency object
 
     Raises:
         RuntimeError: if version already exists
         RuntimeError: if database tables reference non-existing files
+        RuntimeError: if database attachment path does not exist,
+            is a symlink,
+            is empty,
+            or contains an empty sub-folder
         RuntimeError: if database in ``db_root`` depends on other version
             as indicated by ``previous_version``
         RuntimeError: if database is not portable,
             see :meth:`audformat.Database.is_portable`
         RuntimeError: if non-standard formats like MP3 and MP4 are published,
             but sox and/or mediafile is not installed
+        RuntimeError: if the type of a database file changes,
+            e.g. from media to attachment
+        RuntimeError: if a new media file
+            has an uppercase letter in its file extension
+        RuntimeError: if database contains tables,
+            misc tables, or attachemnts
+            that are stored under an ID
+            using a char not in ``'[A-Za-z0-9._-]'``
+        ValueError: if ``version`` or ``previous_version``
+            cannot be parsed by :class:`audeer.StrictVersion`
         ValueError: if ``previous_version`` >= ``version``
 
     """
+    # Enforce error if version cannot be converted to audeer.StrictVersion
+    audeer.StrictVersion(version)
     if (
             previous_version is not None
             and previous_version != 'latest'
             and (
-                audeer.LooseVersion(version)
-                <= audeer.LooseVersion(previous_version)
+                audeer.StrictVersion(version)
+                <= audeer.StrictVersion(previous_version)
             )
     ):
         raise ValueError(
             "'previous_version' needs to be smaller than 'version', "
             f"but yours is {previous_version} >= {version}."
         )
 
@@ -535,14 +684,36 @@
     db = audformat.Database.load(
         db_root,
         load_data=True,
         num_workers=num_workers,
         verbose=verbose,
     )
 
+    # ensure table and attachment IDs
+    # contain only chars allowed by the backend
+    # as the IDs are included in the filenames of the archives
+    # uploaded to the backend
+    allowed_chars = audbackend.core.utils.BACKEND_ALLOWED_CHARS
+    allowed_chars = allowed_chars.replace('/', '')
+    allowed_chars_compiled = re.compile(allowed_chars)
+    for table_id in list(db):
+        if allowed_chars_compiled.fullmatch(table_id) is None:
+            raise RuntimeError(
+                "Table IDs must only contain chars from "
+                f"{allowed_chars[:-1]}, "
+                f"which is not the case for table '{table_id}'."
+            )
+    for attachment_id in list(db.attachments):
+        if allowed_chars_compiled.fullmatch(attachment_id) is None:
+            raise RuntimeError(
+                "Attachment IDs must only contain chars from "
+                f"{allowed_chars[:-1]}, "
+                f"which is not the case for attachment '{attachment_id}'."
+            )
+
     # check all tables are conform with audformat
     if not db.is_portable:
         raise RuntimeError(
             "Some files in the tables have absolute paths "
             "or use '\\', '.', '..' in its path. "
             "Please replace those paths by relative paths, "
             "use folder names instead of dots, "
@@ -562,14 +733,19 @@
         table_ext = audformat.define.TableStorageFormat.CSV
         if not os.path.exists(table_path + f'.{table_ext}'):
             table.save(table_path, storage_format=table_ext)
 
     # check archives
     archives = archives or {}
 
+    # publish attachments
+    attachments = _find_attachments(db, db_root, version, deps, verbose)
+    _put_attachments(attachments, db_root, db, version, backend, num_workers,
+                     verbose)
+
     # publish tables
     tables = _find_tables(db, db_root, version, deps, verbose)
     _put_tables(tables, db_root, db.name, version, backend, num_workers,
                 verbose)
 
     # publish media
     media_archives = _find_media(db, db_root, db_root_files, version, deps,
```

### Comparing `audb-1.4.2/audb/info/__init__.py` & `audb-1.5.0/audb/info/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 .. jupyter-execute::
     :stderr:
     :hide-code:
     :hide-output:
 
     audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         only_metadata=True,
         verbose=False,
     )
 
 Instead of caching the header (:file:`db.yaml`)
 of a database first locally to inspect it,
 the functions under :mod:`audb.info`
@@ -35,31 +35,32 @@
 
 So instead of running:
 
 .. jupyter-execute::
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         only_metadata=True,
         verbose=False,
     )
     db.tables
 
 You can run:
 
 .. jupyter-execute::
 
     audb.info.tables(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
     )
 
 """
 from audb.core.info import (
+    attachments,
     author,
     bit_depths,
     channels,
     description,
     duration,
     files,
     formats,
```

### Comparing `audb-1.4.2/audb.egg-info/PKG-INFO` & `audb-1.5.0/audb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audb
-Version: 1.4.2
+Version: 1.5.0
 Summary: Load and publish databases in audformat
 Home-page: https://audeering.github.io/audb/
 Author: Johannes Wagner, Hagen Wierstorf
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audb/
 Description: ====
@@ -37,15 +37,15 @@
         .. _quickstart: https://audeering.github.io/audb/quickstart.html
         
         
         .. badges images and links:
         .. |tests| image:: https://github.com/audeering/audb/workflows/Test/badge.svg
             :target: https://github.com/audeering/audb/actions?query=workflow%3ATest
             :alt: Test status
-        .. |coverage| image:: https://codecov.io/gh/audeering/audb/branch/master/graph/badge.svg?token=drrULW8vEG
+        .. |coverage| image:: https://codecov.io/gh/audeering/audb/branch/main/graph/badge.svg?token=drrULW8vEG
             :target: https://codecov.io/gh/audeering/audb/
             :alt: code coverage
         .. |docs| image:: https://img.shields.io/pypi/v/audb?label=docs
             :target: https://audeering.github.io/audb/
             :alt: audb's documentation
         .. |license| image:: https://img.shields.io/badge/license-MIT-green.svg
             :target: https://github.com/audeering/audb/blob/master/LICENSE
@@ -59,14 +59,45 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.5.0 (2023-04-27)
+        --------------------------
+        
+        * Added: support loading and publishing
+          of database attachments
+          (``audformat.Attachment``)
+        * Added: ``audb.load_attachment()``
+          to load a single attachment of a database
+        * Added: ``audb.info.attachments()``
+          to return the attachments entry
+          of a database header
+        * Added: ``attachments`` argument to ``audb.load()``
+          to load only specific
+          attachments of a database
+        * Changed: raise ``RuntimeError`` in ``audb.publish()``
+          if the file extension of a media file
+          contains uppercase letters
+        * Changed: raise ``RuntimeError`` in ``audb.publish()``
+          if a table ID or attachment ID
+          contains a character not in ``[A-Za-z0-9._-]``
+        * Changed: raise ``ValueError`` in ``audb.publish()``
+          if ``version`` or ``previous_version``
+          are not conform to ``audeer.StrictVersion``
+        * Changed: use emodb v1.4.1 for documentation examples
+        * Changed: require ``audbackend<1.0.0``
+          as ``audbackend`` will introduce breaking changes
+        * Fixed: speed up ``audb.load_to()``
+          when loading databases with large tables
+          using ``only_metadata=True``
+        
+        
         Version 1.4.2 (2023-02-13)
         --------------------------
         
         * Added: support for Python 3.10
         * Added: document optional needed overwrite permissions
           for ``audb.publish()``
           when continuing a canceled publishing command
```

### Comparing `audb-1.4.2/audb.egg-info/SOURCES.txt` & `audb-1.5.0/audb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,8 +67,9 @@
 tests/test_flavor.py
 tests/test_info.py
 tests/test_load.py
 tests/test_load_on_demand.py
 tests/test_lock.py
 tests/test_lock_db.py
 tests/test_publish.py
-tests/test_remove.py
+tests/test_remove.py
+tests/test_utils.py
```

### Comparing `audb-1.4.2/docs/_templates/autosummary/class.rst` & `audb-1.5.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/authentication.rst` & `audb-1.5.0/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/caching.rst` & `audb-1.5.0/docs/caching.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/conf.py` & `audb-1.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     audb.Repository(
         name='data-public',
         host='https://audeering.jfrog.io/artifactory',
         backend='artifactory',
     )
 ]
 database_name = 'emodb'
-database_version = '1.3.0'
+database_version = '1.4.1'
 if not audb.exists(database_name, version=database_version):
     print(f'Pre-caching {database_name} v{database_version}')
     audb.load(
         database_name,
         version=database_version,
         num_workers=5,
         only_metadata=True,
```

### Comparing `audb-1.4.2/docs/configuration.rst` & `audb-1.5.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/dependencies.rst` & `audb-1.5.0/docs/dependencies.rst`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 for every version of a database.
 
 You request a :class:`audb.Dependencies` object with
 :func:`audb.dependencies`.
 
 .. jupyter-execute::
 
-    deps = audb.dependencies('emodb', version='1.3.0')
+    deps = audb.dependencies('emodb', version='1.4.1')
 
 You can see all entries by calling the returned object.
 
 .. jupyter-execute::
 
     df = deps()
     df.head()
@@ -68,38 +68,38 @@
 
 If your database contains only WAV or FLAC files,
 we store the duration in seconds of every file
 in the database dependency table.
 
 .. jupyter-execute::
 
-    deps = audb.dependencies('emodb', version='1.3.0')
+    deps = audb.dependencies('emodb', version='1.4.1')
     df = deps()
     df.duration[:10]
 
 For those databases
 you can get their overall duration with:
 
 .. jupyter-execute::
 
-    audb.info.duration('emodb', version='1.3.0')
+    audb.info.duration('emodb', version='1.4.1')
 
 The duration of parts of a database
 can be calculated
 by first loading the dependency table
 and filter for the selected media files.
 The following calculates the duration
 of the first ten files in the *emotion* table
 of the emodb database.
 
 .. jupyter-execute::
 
     import numpy as np
 
-    df = audb.load_table('emodb', 'emotion', version='1.3.0', verbose=False)
+    df = audb.load_table('emodb', 'emotion', version='1.4.1', verbose=False)
     files = df.index[:10]
     duration_in_sec = np.sum([deps.duration(f) for f in files])
     pd.to_timedelta(duration_in_sec, unit='s')
 
 If your table is a segmented table,
 and you would like to get the duration
 of its segments
```

### Comparing `audb-1.4.2/docs/index.rst` & `audb-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/install.rst` & `audb-1.5.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/load.rst` & `audb-1.5.0/docs/load.rst`

 * *Files 4% similar despite different names*

```diff
@@ -52,24 +52,24 @@
 
 .. Prefetch data with only_metadata=True
 .. jupyter-execute::
     :hide-code:
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         only_metadata=True,
         verbose=False,
     )
 
 .. code-block:: python
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         verbose=False,
     )
 
 :func:`audb.load` will download the data,
 store them in a cache folder,
 and return the database as an :class:`audformat.Database` object.
 The most important content of that object
@@ -150,26 +150,26 @@
 
 .. Prefetch data with only_metadata=True
 .. jupyter-execute::
     :hide-code:
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         format='flac',
         sampling_rate=44100,
         only_metadata=True,
         verbose=False,
     )
 
 .. code-block:: python
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         format='flac',
         sampling_rate=44100,
         verbose=False,
     )
 
 The flavor information of a database is stored
 inside the ``db.meta['audb']`` dictionary.
@@ -200,15 +200,15 @@
 In that case media files are not loaded,
 but all the tables and the header.
 
 .. jupyter-execute::
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         only_metadata=True,
         verbose=False,
     )
 
 For databases with many annotations,
 this can still take some time.
 If you are only interested in header information,
@@ -218,24 +218,24 @@
 have a look at the :mod:`audb.info` module.
 It can list all table definitions.
 
 .. jupyter-execute::
 
     audb.info.tables(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
     )
 
 Or get the total duration of all media files.
 
 .. jupyter-execute::
 
     audb.info.duration(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
     )
 
 See :mod:`audb.info` for a list of all available options.
 
 
 .. _filter:
 
@@ -257,15 +257,15 @@
 First, we download the table with information
 about the speakers (here ``db['files']``):
 
 .. jupyter-execute::
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         tables=['files'],
         only_metadata=True,
         full_path=False,
         verbose=False,
     )
     db.tables
 
@@ -297,26 +297,26 @@
 
 .. Prefetch data with only_metadata=True
 .. jupyter-execute::
     :hide-code:
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         media=media,
         full_path=False,
         only_metadata=True,
         verbose=False,
     )
 
 .. code-block:: python
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         media=media,
         full_path=False,
         verbose=False,
     )
 
 This will also remove
 entries of other speakers
```

### Comparing `audb-1.4.2/docs/overview.rst` & `audb-1.5.0/docs/overview.rst`

 * *Files 4% similar despite different names*

```diff
@@ -92,10 +92,10 @@
 6. inspect and :ref:`convert <media-conversion-and-flavors>`
    the audio files (optional)
 7. store the data in a :ref:`cache <caching>` folder
 
 .. graphviz:: pics/load.dot
 
 
-.. _Generic repository: https://www.jfrog.com/confluence/display/JFROG/Repository+Management#RepositoryManagement-GenericRepositories
+.. _Generic repository: https://jfrog.com/help/r/jfrog-artifactory-documentation/repository-management
 .. _Artifactory server: https://jfrog.com/artifactory/
 .. _implements the required functions: https://github.com/audeering/audbackend/blob/edd23462799ae9052a43cdd045698f78e19dbcaf/audbackend/core/backend.py#L559-L659
```

### Comparing `audb-1.4.2/docs/pics/load.dot` & `audb-1.5.0/docs/pics/load.dot`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/pics/publish.dot` & `audb-1.5.0/docs/pics/publish.dot`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/publish.rst` & `audb-1.5.0/docs/publish.rst`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/docs/quickstart.rst` & `audb-1.5.0/docs/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 
 .. Load with only_metadata=True in the background
 .. jupyter-execute::
     :hide-code:
 
     db = audb.load(
         'emodb',
-        version='1.3.0',
+        version='1.4.1',
         only_metadata=True,
         verbose=False,
     )
 
 .. code-block:: python
 
-    db = audb.load('emodb', version='1.3.0', verbose=False)
+    db = audb.load('emodb', version='1.4.1', verbose=False)
 
 This downloads the database header,
 all the media files,
 and tables with annotations
 to a caching folder on your machine.
 The database is then returned
 as an :class:`audformat.Database` object.
```

### Comparing `audb-1.4.2/setup.cfg` & `audb-1.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 install_requires = 
-	audbackend >=0.3.17
+	audbackend >=0.3.17, <1.0.0
 	audeer >=1.18.0
-	audformat >=0.15.2,<2.0.0
+	audformat >=0.16.1
 	audiofile >=1.0.0
 	audobject >=0.5.0
 	audresample >=0.1.6
 	filelock
 	oyaml
 python_requires = >=3.8
 setup_requires =
```

### Comparing `audb-1.4.2/tests/test_api.py` & `audb-1.5.0/tests/test_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import os
 
-import pytest
-
 import audb
 import audeer
 
 
-def test_available():
+def test_available(repository):
+
+    # Broken database in repo
+    name = 'non-existing-database'
+    path = os.path.join(
+        repository.host,
+        repository.name,
+        name,
+    )
+    path = audeer.mkdir(path)
+    df = audb.available()
+    os.rmdir(path)
+    assert len(df) == 0
 
     # Non existing repo
     name = 'non-existing-repo'
     audb.config.REPOSITORIES = [
         audb.Repository(
             name=name,
-            host=pytest.FILE_SYSTEM_HOST,
-            backend=pytest.BACKEND,
+            host=repository.host,
+            backend=repository.backend,
         )
     ]
     df = audb.available()
     assert len(df) == 0
-
-    # Borken database in repo
-    name = 'non-existing-database'
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
-    path = os.path.join(
-        audb.config.REPOSITORIES[0].host,
-        audb.config.REPOSITORIES[0].name,
-        name,
-    )
-    path = audeer.mkdir(path)
-    audb.available()
-    os.rmdir(path)
-    assert len(df) == 0
```

### Comparing `audb-1.4.2/tests/test_config.py` & `audb-1.5.0/tests/test_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import os
-
 import pytest
 
 import audb
 import audeer
 
 
-def test_config_file():
+def test_config_file(tmpdir):
 
-    audeer.mkdir(pytest.ROOT)
+    root = audeer.mkdir(tmpdir)
 
-    config_file = os.path.join(pytest.ROOT, '.audb.yaml')
+    config_file = audeer.path(root, '.audb.yaml')
 
     # Try loading non-existing file
     config = audb.core.config.load_configuration_file(config_file)
     assert config == {}
 
     # Add a custom cache entry
     # and check if combining with global config works
@@ -25,15 +23,15 @@
     assert config == {'cache_root': '~/user'}
 
     global_config = audb.core.config.load_configuration_file(
         audb.core.config.global_config_file
     )
     global_config.update(config)
     assert global_config['cache_root'] == '~/user'
-    assert global_config['shared_cache_root'] == audb.config.SHARED_CACHE_ROOT
+    assert global_config['shared_cache_root'] == '/data/audb'
 
     # Fail for wrong repositories entries
     with open(config_file, 'w') as cf:
         cf.write('repositories:\n')
     error_msg = (
         "You cannot specify an empty 'repositories:' section "
         f"in the configuration file '{audb.core.define.USER_CONFIG_FILE}'."
```

### Comparing `audb-1.4.2/tests/test_convert.py` & `audb-1.5.0/tests/test_convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,109 @@
 import os
-import shutil
-
 import numpy as np
 import pytest
 
 import audformat.testing
 import audeer
 import audiofile
 
 import audb
 
 
-os.environ['AUDB_CACHE_ROOT'] = pytest.CACHE_ROOT
-os.environ['AUDB_SHARED_CACHE_ROOT'] = pytest.SHARED_CACHE_ROOT
+DB_NAME = 'test_convert'
 
 
 @pytest.fixture(
-    scope='session',
+    scope='module',
     autouse=True,
 )
-def fixture_set_repositories():
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
-
-
-DB_NAME = f'test_convert-{pytest.ID}'
-DB_ROOT = os.path.join(pytest.ROOT, 'db')
+def db_root(tmpdir_factory, persistent_repository):
+    r"""Publish single database.
 
-DB_FILES = {
-    'audio/file1.wav': {
-        'bit_depth': 16,
-        'channels': 1,
-        'format': 'wav',
-        'sampling_rate': 8000,
-    },
-    'audio/file2.wav': {
-        'bit_depth': 24,
-        'channels': 2,
-        'format': 'wav',
-        'sampling_rate': 16000,
-    },
-    'audio/file3.flac': {
-        'bit_depth': 8,
-        'channels': 3,
-        'format': 'flac',
-        'sampling_rate': 44100,
-    },
-}
-
-
-def clear_root(root: str):
-    root = audeer.path(root)
-    if os.path.exists(root):
-        shutil.rmtree(root)
+    Returns:
+        path to original database root
 
+    """
 
-@pytest.fixture(
-    scope='module',
-    autouse=True,
-)
-def fixture_publish_db():
-
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
+    version = '1.0.0'
+    db_root = tmpdir_factory.mktemp(version)
+
+    # define audio files and metadata
+
+    db_files = {
+        'audio/file1.wav': {
+            'bit_depth': 16,
+            'channels': 1,
+            'format': 'wav',
+            'sampling_rate': 8000,
+        },
+        'audio/file2.wav': {
+            'bit_depth': 24,
+            'channels': 2,
+            'format': 'wav',
+            'sampling_rate': 16000,
+        },
+        'audio/file3.flac': {
+            'bit_depth': 8,
+            'channels': 3,
+            'format': 'flac',
+            'sampling_rate': 44100,
+        },
+    }
 
     # create db
 
     db = audformat.testing.create_db(minimal=True)
     db.name = DB_NAME
-    db['files'] = audformat.Table(audformat.filewise_index(list(DB_FILES)))
+
+    db['files'] = audformat.Table(audformat.filewise_index(list(db_files)))
     db['files']['original'] = audformat.Column()
-    db['files']['original'].set(list(DB_FILES))
-    for file in DB_FILES:
+    db['files']['original'].set(list(db_files))
+    for file in db_files:
         signal = np.zeros(
             (
-                DB_FILES[file]['channels'],
-                DB_FILES[file]['sampling_rate'],
+                db_files[file]['channels'],
+                db_files[file]['sampling_rate'],
             ),
             dtype=np.float32,
         )
-        path = os.path.join(DB_ROOT, file)
+        path = os.path.join(db_root, file)
         audeer.mkdir(os.path.dirname(path))
         audiofile.write(
-            path, signal, DB_FILES[file]['sampling_rate'],
-            bit_depth=DB_FILES[file]['bit_depth']
+            path, signal, db_files[file]['sampling_rate'],
+            bit_depth=db_files[file]['bit_depth']
         )
     db['segments'] = audformat.Table(
         audformat.segmented_index(
-            [list(DB_FILES)[0]] * 3,
+            [list(db_files)[0]] * 3,
             starts=['0s', '1s', '2s'],
             ends=['1s', '2s', '3s'],
         )
     )
-    db.save(DB_ROOT)
+    db.save(db_root)
 
     # publish db
 
     audb.publish(
-        DB_ROOT,
-        '1.0.0',
-        pytest.PUBLISH_REPOSITORY,
+        db_root,
+        version,
+        persistent_repository,
         verbose=False,
     )
 
-    yield
-
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
-
-
-@pytest.fixture(
-    scope='function',
-    autouse=True,
-)
-def fixture_clear_cache():
-    clear_root(pytest.CACHE_ROOT)
-    yield
-    clear_root(pytest.CACHE_ROOT)
+    return db_root
 
 
 @pytest.mark.parametrize(
     'bit_depth',
     [
         None, 16,
     ],
 )
-def test_bit_depth(bit_depth):
+def test_bit_depth(db_root, bit_depth):
 
     db = audb.load(
         DB_NAME,
         bit_depth=bit_depth,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
@@ -137,30 +112,30 @@
 
     df = audb.cached()
     assert df['bit_depth'].values[0] == bit_depth
 
     for converted_file, original_file in zip(db.files, original_files):
 
         converted_file = os.path.join(db.meta['audb']['root'], converted_file)
-        original_file = os.path.join(DB_ROOT, original_file)
+        original_file = os.path.join(db_root, original_file)
 
         if bit_depth is None:
             assert audiofile.bit_depth(converted_file) == \
                 audiofile.bit_depth(original_file)
         else:
             assert audiofile.bit_depth(converted_file) == bit_depth
 
 
 @pytest.mark.parametrize(
     'channels',
     [
         None, 1, [0, -1], range(5),
     ],
 )
-def test_channels(channels):
+def test_channels(db_root, channels):
 
     db = audb.load(
         DB_NAME,
         channels=channels,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
@@ -168,15 +143,15 @@
     original_files = db['files']['original'].get()
 
     df = audb.cached()
 
     for converted_file, original_file in zip(db.files, original_files):
 
         converted_file = os.path.join(db.meta['audb']['root'], converted_file)
-        original_file = os.path.join(DB_ROOT, original_file)
+        original_file = os.path.join(db_root, original_file)
 
         if channels is None:
             assert audiofile.channels(converted_file) == \
                 audiofile.channels(original_file)
             assert df['channels'].values[0] == channels
         elif isinstance(channels, int):
             assert audiofile.channels(converted_file) == 1
@@ -189,15 +164,15 @@
     'format',
     [
         None,
         audb.core.define.Format.WAV,
         audb.core.define.Format.FLAC,
     ],
 )
-def test_format(format):
+def test_format(db_root, format):
 
     db = audb.load(
         DB_NAME,
         format=format,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
@@ -206,29 +181,29 @@
 
     df = audb.cached()
     assert df['format'].values[0] == format
 
     for converted_file, original_file in zip(db.files, original_files):
 
         converted_file = os.path.join(db.meta['audb']['root'], converted_file)
-        original_file = os.path.join(DB_ROOT, original_file)
+        original_file = os.path.join(db_root, original_file)
 
         if format is None:
             assert converted_file[-4:] == original_file[-4:]
         else:
             assert converted_file.endswith(format)
 
 
 @pytest.mark.parametrize(
     'mixdown',
     [
         False, True
     ],
 )
-def test_mixdown(mixdown):
+def test_mixdown(db_root, mixdown):
 
     db = audb.load(
         DB_NAME,
         mixdown=mixdown,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
@@ -237,30 +212,30 @@
 
     df = audb.cached()
     assert df['mixdown'].values[0] == mixdown
 
     for converted_file, original_file in zip(db.files, original_files):
 
         converted_file = os.path.join(db.meta['audb']['root'], converted_file)
-        original_file = os.path.join(DB_ROOT, original_file)
+        original_file = os.path.join(db_root, original_file)
 
         if mixdown:
             assert audiofile.channels(converted_file) == 1
         else:
             assert audiofile.channels(converted_file) == \
                 audiofile.channels(original_file)
 
 
 @pytest.mark.parametrize(
     'sampling_rate',
     [
         None, 16000
     ],
 )
-def test_sampling_rate(sampling_rate):
+def test_sampling_rate(db_root, sampling_rate):
 
     db = audb.load(
         DB_NAME,
         sampling_rate=sampling_rate,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
@@ -269,44 +244,43 @@
 
     df = audb.cached()
     assert df['sampling_rate'].values[0] == sampling_rate
 
     for converted_file, original_file in zip(db.files, original_files):
 
         converted_file = os.path.join(db.meta['audb']['root'], converted_file)
-        original_file = os.path.join(DB_ROOT, original_file)
+        original_file = os.path.join(db_root, original_file)
 
         if sampling_rate is None:
             assert audiofile.sampling_rate(converted_file) == \
                 audiofile.sampling_rate(original_file)
         else:
             assert audiofile.sampling_rate(converted_file) == sampling_rate
 
 
-def test_mixed_cache():
+def test_mixed_cache(cache, shared_cache):
     # Avoid failing searching for other versions
     # if databases a stored accross private and shared cache
     # and the private one is empty, see
     # https://github.com/audeering/audb/issues/101
 
     # First load to shared cache
     audb.load(
         DB_NAME,
         sampling_rate=8000,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
         only_metadata=True,
         tables='files',
-        cache_root=pytest.SHARED_CACHE_ROOT,
+        cache_root=shared_cache,
     )
     # Now try to load same version to private cache
     # to force audb.cached() to return empty dataframe
-    clear_root(pytest.CACHE_ROOT)
-    audeer.mkdir(pytest.CACHE_ROOT)
+    audeer.rmdir(cache)
     audb.load(
         DB_NAME,
         sampling_rate=8000,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
         only_metadata=True,
```

### Comparing `audb-1.4.2/tests/test_dependencies.py` & `audb-1.5.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/tests/test_filter.py` & `audb-1.5.0/tests/test_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,27 @@
-import os
-import shutil
-
 import pandas as pd
 import pytest
 
 import audformat.testing
-import audeer
 
 import audb
 
 
-os.environ['AUDB_CACHE_ROOT'] = pytest.CACHE_ROOT
-os.environ['AUDB_SHARED_CACHE_ROOT'] = pytest.SHARED_CACHE_ROOT
-
-
-@pytest.fixture(
-    scope='session',
-    autouse=True,
-)
-def fixture_set_repositories():
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
-
-
-DB_NAME = f'test_filter-{pytest.ID}'
-DB_ROOT = os.path.join(pytest.ROOT, 'db')
-
-
-def clear_root(root: str):
-    root = audeer.path(root)
-    if os.path.exists(root):
-        shutil.rmtree(root)
+DB_NAME = 'test_filter'
 
 
 @pytest.fixture(
     scope='module',
     autouse=True,
 )
-def fixture_publish_db():
+def db(tmpdir_factory, persistent_repository):
+    r"""Publish a single database."""
 
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
+    version = '1.0.0'
+    db_root = tmpdir_factory.mktemp(version)
 
     # create db
 
     db = audformat.testing.create_db(minimal=True)
     db.name = DB_NAME
     db.schemes['scheme'] = audformat.Scheme(
         labels=['some', 'test', 'labels']
@@ -95,49 +73,34 @@
     starts = db['train'].df.index.get_level_values('start')
     ends = db['train'].df.index.get_level_values('end')
     db['train'].df.index = audformat.segmented_index(
         files=[mapping[f] for f in files],
         starts=starts,
         ends=ends,
     )
-    db.save(DB_ROOT)
+    db.save(db_root)
     audformat.testing.create_audio_files(db)
 
     # publish db
 
     archives = {}
     for table in db.tables:
         archives.update(
             {
                 file: table for file in db[table].files
             }
         )
     audb.publish(
-        DB_ROOT,
-        '1.0.0',
-        pytest.PUBLISH_REPOSITORY,
+        db_root,
+        version,
+        persistent_repository,
         archives=archives,
         verbose=False,
     )
 
-    yield
-
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
-
-
-@pytest.fixture(
-    scope='function',
-    autouse=True,
-)
-def fixture_clear_cache():
-    clear_root(pytest.CACHE_ROOT)
-    yield
-    clear_root(pytest.CACHE_ROOT)
-
 
 @pytest.mark.parametrize(
     'media, format, expected_files',
     [
         (
             None,
             None,
@@ -268,11 +231,9 @@
         DB_NAME,
         tables=tables,
         format=format,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
     )
-    print(list(db))
-    print(expected_tables)
     assert list(db) == expected_tables
     assert list(db.files) == expected_files
```

### Comparing `audb-1.4.2/tests/test_flavor.py` & `audb-1.5.0/tests/test_flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/tests/test_info.py` & `audb-1.5.0/tests/test_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,153 +1,132 @@
 import os
-import shutil
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import audformat.testing
 import audeer
 import audiofile
 
 import audb
 
 
-os.environ['AUDB_CACHE_ROOT'] = pytest.CACHE_ROOT
-os.environ['AUDB_SHARED_CACHE_ROOT'] = pytest.SHARED_CACHE_ROOT
+DB_NAME = 'test_info'
+DB_VERSION = '1.0.0'
 
 
 @pytest.fixture(
-    scope='session',
+    scope='module',
     autouse=True,
 )
-def fixture_set_repositories():
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
-
-
-DB_NAME = f'test_info-{pytest.ID}'
-DB_VERSION = '1.0.0'
-DB = audformat.Database(
-    DB_NAME,
-    source='https://audeering.github.io/audb/',
-    usage=audformat.define.Usage.UNRESTRICTED,
-    languages=['de', 'English'],
-    description='audb.info unit test database',
-    meta={'foo': 'bar'}
-)
-DB.media['media'] = audformat.Media()
-DB.schemes['scheme1'] = audformat.Scheme()
-DB.splits['split'] = audformat.Split()
-DB.raters['rater'] = audformat.Rater()
-DB['table1'] = audformat.Table(
-    audformat.filewise_index(
-        ['f11.wav', 'f12.wav', 'f13.wav'],
-    ),
-    media_id='media',
-    split_id='split',
-)
-DB['table1']['column'] = audformat.Column(
-    scheme_id='scheme1',
-    rater_id='rater',
-)
-DB['table2'] = audformat.Table(
-    audformat.segmented_index(
-        ['f21.wav', 'f22.wav', 'f22.wav'],
-        [0, 0, .5],
-        [1, .5, 1],
-    ),
-    media_id='media',
-    split_id='split',
-)
-DB['table2']['column'] = audformat.Column(
-    scheme_id='scheme1',
-    rater_id='rater',
-)
-DB['misc-in-scheme'] = audformat.MiscTable(
-    pd.Index([0, 1], name='idx')
-)
-DB['misc-not-in-scheme'] = audformat.MiscTable(
-    pd.Index([0, 1], name='idx')
-)
-DB.schemes['scheme2'] = audformat.Scheme(
-    'int',
-    labels='misc-in-scheme',
-)
-
-DB_ROOT = os.path.join(pytest.ROOT, 'db')
+def db(tmpdir_factory, persistent_repository):
+    r"""Publish a single database.
 
+    Returns:
+        database object
 
-def clear_root(root: str):
-    root = audeer.path(root)
-    if os.path.exists(root):
-        shutil.rmtree(root)
+    """
 
+    # creat db
 
-@pytest.fixture(
-    scope='module',
-    autouse=True,
-)
-def fixture_publish_db():
-
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
+    db = audformat.Database(
+        DB_NAME,
+        source='https://audeering.github.io/audb/',
+        usage=audformat.define.Usage.UNRESTRICTED,
+        languages=['de', 'English'],
+        description='audb.info unit test database',
+        meta={'foo': 'bar'}
+    )
+    db.media['media'] = audformat.Media()
+    db.schemes['scheme1'] = audformat.Scheme()
+    db.splits['split'] = audformat.Split()
+    db.raters['rater'] = audformat.Rater()
+    db.attachments['attachment'] = audformat.Attachment('file.txt')
+    db['table1'] = audformat.Table(
+        audformat.filewise_index(
+            ['f11.wav', 'f12.wav', 'f13.wav'],
+        ),
+        media_id='media',
+        split_id='split',
+    )
+    db['table1']['column'] = audformat.Column(
+        scheme_id='scheme1',
+        rater_id='rater',
+    )
+    db['table2'] = audformat.Table(
+        audformat.segmented_index(
+            ['f21.wav', 'f22.wav', 'f22.wav'],
+            [0, 0, .5],
+            [1, .5, 1],
+        ),
+        media_id='media',
+        split_id='split',
+    )
+    db['table2']['column'] = audformat.Column(
+        scheme_id='scheme1',
+        rater_id='rater',
+    )
+    db['misc-in-scheme'] = audformat.MiscTable(
+        pd.Index([0, 1], name='idx')
+    )
+    db['misc-not-in-scheme'] = audformat.MiscTable(
+        pd.Index([0, 1], name='idx')
+    )
+    db.schemes['scheme2'] = audformat.Scheme(
+        'int',
+        labels='misc-in-scheme',
+    )
 
     # create db + audio files
+
+    db_root = tmpdir_factory.mktemp(DB_VERSION)
     sampling_rate = 8000
-    audeer.mkdir(DB_ROOT)
-    for table in list(DB.tables):
-        for file in DB[table].files:
+    audeer.touch(audeer.path(db_root, db.attachments['attachment'].path))
+    for table in list(db.tables):
+        for file in db[table].files:
             audiofile.write(
-                os.path.join(DB_ROOT, file),
+                os.path.join(db_root, file),
                 np.zeros((1, sampling_rate)),
                 sampling_rate,
             )
 
-    DB.save(DB_ROOT)
+    db.save(db_root)
 
     # publish db
 
     audb.publish(
-        DB_ROOT,
+        db_root,
         DB_VERSION,
-        pytest.PUBLISH_REPOSITORY,
+        persistent_repository,
         verbose=False,
     )
 
-    yield
+    return db
 
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
 
-
-@pytest.fixture(
-    scope='function',
-    autouse=True,
-)
-def fixture_clear_cache():
-    clear_root(pytest.CACHE_ROOT)
-    yield
-    clear_root(pytest.CACHE_ROOT)
+def test_attachemnts(db):
+    assert str(audb.info.attachments(DB_NAME)) == str(db.attachments)
 
 
-def test_author():
-    assert audb.info.author(DB_NAME) == DB.author
+def test_author(db):
+    assert audb.info.author(DB_NAME) == db.author
 
 
-def test_header():
+def test_header(db):
     # Load header without loading misc tables
-    db = audb.info.header(DB_NAME, load_tables=False)
-    assert str(db) == str(DB)
+    header = audb.info.header(DB_NAME, load_tables=False)
+    assert str(header) == str(db)
     error_msg = 'No file found for table with path'
     with pytest.raises(RuntimeError, match=error_msg):
-        assert 0 in db.schemes['scheme2']
+        assert 0 in header.schemes['scheme2']
     # Load header with tables
-    db = audb.info.header(DB_NAME)
-    assert str(db) == str(DB)
-    assert 0 in db.schemes['scheme2']
+    header = audb.info.header(DB_NAME)
+    assert str(header) == str(db)
+    assert 0 in header.schemes['scheme2']
 
 
 def test_bit_depths():
     deps = audb.dependencies(DB_NAME, version=DB_VERSION)
     assert audb.info.bit_depths(DB_NAME) == set(
         [
             deps.bit_depth(file) for file in deps.media
@@ -162,16 +141,16 @@
         [
             deps.channels(file) for file in deps.media
             if deps.channels(file)
         ]
     )
 
 
-def test_description():
-    assert audb.info.description(DB_NAME) == DB.description
+def test_description(db):
+    assert audb.info.description(DB_NAME) == db.description
 
 
 @pytest.mark.parametrize(
     'tables, media',
     [
         (None, None),
         ([], None),
@@ -217,76 +196,76 @@
     assert audb.info.formats(DB_NAME) == set(
         [
             deps.format(file) for file in deps.media
         ]
     )
 
 
-def test_languages():
-    assert audb.info.languages(DB_NAME) == DB.languages
+def test_languages(db):
+    assert audb.info.languages(DB_NAME) == db.languages
 
 
-def test_license():
-    assert audb.info.license(DB_NAME) == DB.license
+def test_license(db):
+    assert audb.info.license(DB_NAME) == db.license
 
 
-def test_license_url():
-    assert audb.info.license_url(DB_NAME) == DB.license_url
+def test_license_url(db):
+    assert audb.info.license_url(DB_NAME) == db.license_url
 
 
-def test_media():
-    assert str(audb.info.media(DB_NAME)) == str(DB.media)
+def test_media(db):
+    assert str(audb.info.media(DB_NAME)) == str(db.media)
 
 
-def test_meta():
-    assert audb.info.meta(DB_NAME) == DB.meta
+def test_meta(db):
+    assert audb.info.meta(DB_NAME) == db.meta
 
 
-def test_misc_tables():
-    assert str(audb.info.misc_tables(DB_NAME)) == str(DB.misc_tables)
+def test_misc_tables(db):
+    assert str(audb.info.misc_tables(DB_NAME)) == str(db.misc_tables)
 
 
-def test_organization():
-    assert audb.info.organization(DB_NAME) == DB.organization
+def test_organization(db):
+    assert audb.info.organization(DB_NAME) == db.organization
 
 
-def test_raters():
-    assert str(audb.info.raters(DB_NAME)) == str(DB.raters)
+def test_raters(db):
+    assert str(audb.info.raters(DB_NAME)) == str(db.raters)
 
 
 def test_sampling_rates():
     deps = audb.dependencies(DB_NAME, version=DB_VERSION)
     assert audb.info.sampling_rates(DB_NAME) == set(
         [
             deps.sampling_rate(file) for file in deps.media
             if deps.sampling_rate(file)
         ]
     )
 
 
-def test_schemes():
+def test_schemes(db):
     # Load schemes without loading misc tables
     schemes = audb.info.schemes(DB_NAME, load_tables=False)
-    assert str(schemes) == str(DB.schemes)
+    assert str(schemes) == str(db.schemes)
     error_msg = 'No file found for table with path'
     with pytest.raises(RuntimeError, match=error_msg):
         assert 0 in schemes['scheme2']
     # Load header with tables
     schemes = audb.info.schemes(DB_NAME)
-    str(schemes) == str(DB.schemes)
+    str(schemes) == str(db.schemes)
     assert 0 in schemes['scheme2']
 
 
-def test_splits():
-    assert str(audb.info.splits(DB_NAME)) == str(DB.splits)
+def test_splits(db):
+    assert str(audb.info.splits(DB_NAME)) == str(db.splits)
 
 
-def test_source():
-    assert audb.info.source(DB_NAME) == DB.source
+def test_source(db):
+    assert audb.info.source(DB_NAME) == db.source
 
 
-def test_tables():
-    assert str(audb.info.tables(DB_NAME)) == str(DB.tables)
+def test_tables(db):
+    assert str(audb.info.tables(DB_NAME)) == str(db.tables)
 
 
-def test_usage():
-    assert audb.info.usage(DB_NAME) == DB.usage
+def test_usage(db):
+    assert audb.info.usage(DB_NAME) == db.usage
```

### Comparing `audb-1.4.2/tests/test_lock.py` & `audb-1.5.0/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.4.2/tests/test_lock_db.py` & `audb-1.5.0/tests/test_lock_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import audbackend
 import audeer
 import audformat.testing
 
 import audb
 
 
+DB_NAME = 'test_lock'
+
+
 class SlowFileSystem(audbackend.FileSystem):
     r"""Emulate a slow file system.
 
     Introduces a short delay when getting a file from the backend.
     This ensures that timeouts are reached in the tests.
 
     """
@@ -33,156 +36,158 @@
 class CrashFileSystem(audbackend.FileSystem):
     r"""Emulate a file system that crashes.
 
     Raises an exception when getting a file from the backend.
 
     """
     def _get_file(self, *args):
-        assert any([os.path.exists(path) for path in DB_LOCK_PATHS])
         raise RuntimeError()
 
 
 audbackend.register(
     'crash-file-system',
     CrashFileSystem,
 )
 
 
-os.environ['AUDB_CACHE_ROOT'] = pytest.CACHE_ROOT
-os.environ['AUDB_SHARED_CACHE_ROOT'] = pytest.SHARED_CACHE_ROOT
+def lock_paths(cache):
+    r"""Return list of lock file locations."""
+    paths = []
+    for version in audb.versions(DB_NAME):
+        paths.append(
+            audeer.path(
+                cache,
+                DB_NAME,
+                version,
+                '.lock',
+            )
+        )
+        paths.append(
+            audeer.path(
+                cache,
+                DB_NAME,
+                version,
+                audb.Flavor().short_id,
+                '.lock',
+            )
+        )
+    return paths
 
 
 @pytest.fixture(
     scope='function',
     autouse=True,
 )
-def fixture_ensure_lock_file_deleted():
-    assert not any([os.path.exists(path) for path in DB_LOCK_PATHS])
+def assert_lock_file_is_deleted():
+    r"""Tests if all lock files are deleted."""
+    assert not any(
+        [
+            os.path.exists(path)
+            for path in lock_paths(audb.default_cache_root())
+        ]
+    )
     yield
-    assert not any([os.path.exists(path) for path in DB_LOCK_PATHS])
+    assert not any(
+        [
+            os.path.exists(path)
+            for path in lock_paths(audb.default_cache_root())
+        ]
+    )
 
 
 @pytest.fixture(
     scope='function',
     autouse=True,
 )
-def fixture_set_repositories(request):
+def set_repositories(persistent_repository, request):
+    r"""Access module wide repository with custom backends."""
     audb.config.REPOSITORIES = [
         audb.Repository(
-            name=pytest.REPOSITORY_NAME,
-            host=pytest.FILE_SYSTEM_HOST,
+            name=persistent_repository.name,
+            host=persistent_repository.host,
             backend=request.param,
         ),
     ]
 
 
-DB_NAME = f'test_lock-{pytest.ID}'
-DB_ROOT = os.path.join(pytest.ROOT, 'db')
-DB_VERSIONS = ['1.0.0', '2.0.0']
-
-DB_LOCK_PATHS = []
-for version in DB_VERSIONS:
-    DB_LOCK_PATHS.append(
-        audeer.path(
-            pytest.CACHE_ROOT,
-            DB_NAME,
-            version,
-            '.lock',
-        )
-    )
-    DB_LOCK_PATHS.append(
-        audeer.path(
-            pytest.CACHE_ROOT,
-            DB_NAME,
-            version,
-            audb.Flavor().short_id,
-            '.lock',
-        )
-    )
-
-
-def clear_root(root: str):
-    audeer.rmdir(root)
-
-
-@pytest.fixture(
-    scope='function',
-    autouse=True,
-)
-def fixture_remove_db_from_cache():
-    root = audeer.path(pytest.CACHE_ROOT, DB_NAME)
-    clear_root(root)
-
-
 @pytest.fixture(
     scope='module',
     autouse=True,
 )
-def fixture_publish_db():
+def dbs(tmpdir_factory, persistent_repository):
+    r"""Publish databases.
 
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
+    This publishes a database with the name ``DB_NAME``
+    and the versions 1.0.0 and 2.0.0
+    to a module wide repository.
 
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
+    """
+    db_root = tmpdir_factory.mktemp('db')
 
     # create db
 
     db = audformat.testing.create_db(minimal=True)
     db.name = DB_NAME
     db.schemes['scheme'] = audformat.Scheme()
     audformat.testing.add_table(
         db,
         'table',
         'filewise',
         num_files=[0, 1, 2],
     )
-    db.save(DB_ROOT)
+    db.attachments['file'] = audformat.Attachment('extra/file.txt')
+    db.attachments['folder'] = audformat.Attachment('extra/folder')
+    audeer.mkdir(audeer.path(db_root, 'extra/folder/sub-folder'))
+    for file in [
+            'extra/file.txt',
+            'extra/folder/file1.txt',
+            'extra/folder/file2.txt',
+            'extra/folder/sub-folder/file3.txt',
+    ]:
+        with open(audeer.path(db_root, file), 'w') as fp:
+            fp.write('Some text')
+    db.save(db_root)
     audformat.testing.create_audio_files(db)
 
     # publish 1.0.0
 
     audb.publish(
-        DB_ROOT,
-        DB_VERSIONS[0],
-        pytest.PUBLISH_REPOSITORY,
+        db_root,
+        '1.0.0',
+        persistent_repository,
         verbose=False,
     )
 
     # publish 2.0.0
 
     audformat.testing.add_table(
         db,
         'empty',
         'filewise',
         num_files=0,
     )
-    db.save(DB_ROOT)
+    db.save(db_root)
     audb.publish(
-        DB_ROOT,
-        DB_VERSIONS[1],
-        pytest.PUBLISH_REPOSITORY,
-        previous_version=DB_VERSIONS[0],
+        db_root,
+        '2.0.0',
+        persistent_repository,
+        previous_version='1.0.0',
         verbose=False,
     )
 
-    yield
-
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
-
 
 def load_deps():
     return audb.dependencies(
         DB_NAME,
-        version=DB_VERSIONS[0],
+        version='1.0.0',
     )
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['slow-file-system'],
     indirect=True,
 )
 @pytest.mark.parametrize(
     'multiprocessing',
     [
         False,
@@ -191,16 +196,19 @@
 )
 @pytest.mark.parametrize(
     'num_workers',
     [
         10,
     ]
 )
-def test_lock_dependencies(fixture_set_repositories, multiprocessing,
-                           num_workers):
+def test_lock_dependencies(
+        set_repositories,
+        multiprocessing,
+        num_workers,
+):
 
     # avoid
     # AttributeError: module pytest has no attribute CACHE_ROOT
     # when multiprocessing=True on Windows and macOS
     if multiprocessing and sys.platform in ['win32', 'darwin']:
         return
 
@@ -213,20 +221,20 @@
 
     assert len(result) == num_workers
 
 
 def load_header():
     return audb.info.header(
         DB_NAME,
-        version=DB_VERSIONS[0],
+        version='1.0.0',
     )
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['slow-file-system'],
     indirect=True,
 )
 @pytest.mark.parametrize(
     'multiprocessing',
     [
         False,
@@ -235,15 +243,15 @@
 )
 @pytest.mark.parametrize(
     'num_workers',
     [
         10,
     ]
 )
-def test_lock_header(fixture_set_repositories, multiprocessing, num_workers):
+def test_lock_header(set_repositories, multiprocessing, num_workers):
 
     # avoid
     # AttributeError: module pytest has no attribute CACHE_ROOT
     # when multiprocessing=True on Windows and macOS
     if multiprocessing and sys.platform in ['win32', 'darwin']:
         return
 
@@ -256,22 +264,22 @@
 
     assert len(result) == num_workers
 
 
 def load_db(timeout):
     return audb.load(
         DB_NAME,
-        version=DB_VERSIONS[0],
+        version='1.0.0',
         timeout=timeout,
         verbose=False,
     )
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['slow-file-system'],
     indirect=True,
 )
 @pytest.mark.parametrize(
     'multiprocessing',
     [
         False,
@@ -282,16 +290,21 @@
     'num_workers, timeout, expected',
     [
         (2, -1, 2),
         (2, 9999, 2),
         (2, 0, 1),
     ]
 )
-def test_lock_load(fixture_set_repositories, multiprocessing, num_workers,
-                   timeout, expected):
+def test_lock_load(
+        set_repositories,
+        multiprocessing,
+        num_workers,
+        timeout,
+        expected,
+):
 
     # avoid
     # AttributeError: module pytest has no attribute CACHE_ROOT
     # when multiprocessing=True on Windows and macOS
     if multiprocessing and sys.platform in ['win32', 'darwin']:
         return
 
@@ -308,56 +321,59 @@
         )
     result = [x for x in result if x is not None]
 
     assert len(result) == expected
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['crash-file-system'],
     indirect=True,
 )
-def test_lock_load_crash(fixture_set_repositories):
+def test_lock_load_crash(set_repositories):
 
     with pytest.raises(RuntimeError):
         load_db(-1)
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['file-system'],
     indirect=True,
 )
-def test_lock_load_from_cached_versions(fixture_set_repositories):
+def test_lock_load_from_cached_versions(
+        persistent_repository,
+        set_repositories,
+):
 
     # ensure immediate timeout if cache folder is locked
     cached_version_timeout = audb.core.define.CACHED_VERSIONS_TIMEOUT
     audb.core.define.CACHED_VERSIONS_TIMEOUT = 0
 
     # load version 1.0.0
     db_v1 = audb.load(
         DB_NAME,
-        version=DB_VERSIONS[0],
+        version='1.0.0',
         verbose=False,
     )
 
     # load new files added in version 2.0.0
     audb.load(
         DB_NAME,
-        version=DB_VERSIONS[1],
+        version='2.0.0',
         tables='empty',
         verbose=False,
     )
 
     # switch to crash backend to ensure remaining files
     # must be copied from version 1.0.0
     audb.config.REPOSITORIES = [
         audb.Repository(
-            name=pytest.REPOSITORY_NAME,
-            host=pytest.FILE_SYSTEM_HOST,
+            name=persistent_repository.name,
+            host=persistent_repository.host,
             backend='crash-file-system',
         ),
     ]
 
     # lock cache folder of version 1.0.0
     def lock_v1():
         with audb.core.lock.FolderLock(db_v1.root):
@@ -367,73 +383,122 @@
     thread = threading.Thread(target=lock_v1)
     thread.start()
 
     # -> loading missing table from cache fails
     with pytest.raises(RuntimeError):
         audb.load(
             DB_NAME,
-            version=DB_VERSIONS[1],
+            version='2.0.0',
             tables='table',
             only_metadata=True,
             verbose=False,
         )
 
     # release cache folder of version 1.0.0
     event.set()
     thread.join()
 
     # -> loading missing table from cache succeeds
     audb.load(
         DB_NAME,
-        version=DB_VERSIONS[1],
+        version='2.0.0',
         tables='table',
         only_metadata=True,
         verbose=False,
     )
 
     # lock cache folder of version 1.0.0
     event.clear()
     thread = threading.Thread(target=lock_v1)
     thread.start()
 
     # -> loading missing media from cache fails
     with pytest.raises(RuntimeError):
         audb.load(
             DB_NAME,
-            version=DB_VERSIONS[1],
+            version='2.0.0',
             verbose=False,
         )
 
     # release cache folder of version 1.0.0
     event.set()
     thread.join()
 
     # -> loading missing media from cache succeeds
     audb.load(
         DB_NAME,
-        version=DB_VERSIONS[1],
+        version='2.0.0',
         verbose=False,
     )
 
     # reset timeout
     audb.core.define.CACHED_VERSIONS_TIMEOUT = cached_version_timeout
 
 
+def load_attachment():
+    return audb.load_attachment(
+        DB_NAME,
+        'folder',
+        version='1.0.0',
+        verbose=False,
+    )
+
+
+@pytest.mark.parametrize(
+    'set_repositories',
+    ['slow-file-system'],
+    indirect=True,
+)
+@pytest.mark.parametrize(
+    'multiprocessing',
+    [
+        False,
+        True,
+    ]
+)
+@pytest.mark.parametrize(
+    'num_workers',
+    [
+        4,
+    ]
+)
+def test_lock_load_attachment(
+        set_repositories,
+        multiprocessing,
+        num_workers,
+):
+
+    # Avoid
+    # AttributeError: module pytest has no attribute CACHE_ROOT
+    # when multiprocessing=True on Windows and macOS
+    if multiprocessing and sys.platform in ['win32', 'darwin']:
+        return
+
+    result = audeer.run_tasks(
+        load_attachment,
+        [([], {})] * num_workers,
+        num_workers=num_workers,
+        multiprocessing=multiprocessing,
+    )
+
+    assert len(result) == num_workers
+
+
 def load_media(timeout):
     return audb.load_media(
         DB_NAME,
         'audio/001.wav',
-        version=DB_VERSIONS[0],
+        version='1.0.0',
         timeout=timeout,
         verbose=False,
     )
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['slow-file-system'],
     indirect=True,
 )
 @pytest.mark.parametrize(
     'multiprocessing',
     [
         False,
@@ -444,16 +509,21 @@
     'num_workers, timeout, expected',
     [
         (2, -1, 2),
         (2, 9999, 2),
         (2, 0, 1),
     ]
 )
-def test_lock_load_media(fixture_set_repositories, multiprocessing,
-                         num_workers, timeout, expected):
+def test_lock_load_media(
+        set_repositories,
+        multiprocessing,
+        num_workers,
+        timeout,
+        expected,
+):
 
     # avoid
     # AttributeError: module pytest has no attribute CACHE_ROOT
     # when multiprocessing=True on Windows and macOS
     if multiprocessing and sys.platform in ['win32', 'darwin']:
         return
 
@@ -473,21 +543,21 @@
     assert len(result) == expected
 
 
 def load_table():
     return audb.load_table(
         DB_NAME,
         'table',
-        version=DB_VERSIONS[0],
+        version='1.0.0',
         verbose=False,
     )
 
 
 @pytest.mark.parametrize(
-    'fixture_set_repositories',
+    'set_repositories',
     ['slow-file-system'],
     indirect=True,
 )
 @pytest.mark.parametrize(
     'multiprocessing',
     [
         False,
@@ -496,16 +566,15 @@
 )
 @pytest.mark.parametrize(
     'num_workers',
     [
         10,
     ]
 )
-def test_lock_load_table(fixture_set_repositories, multiprocessing,
-                         num_workers):
+def test_lock_load_table(set_repositories, multiprocessing, num_workers):
 
     # avoid
     # AttributeError: module pytest has no attribute CACHE_ROOT
     # when multiprocessing=True on Windows and macOS
     if multiprocessing and sys.platform in ['win32', 'darwin']:
         return
```

### Comparing `audb-1.4.2/tests/test_publish.py` & `audb-1.5.0/tests/test_load.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-import filecmp
 import os
-import re
 import shutil
 
-import numpy as np
 import pandas as pd
 import pytest
 
-import audbackend
-import audeer
-import audformat.testing
 import audiofile
 
+import audformat.testing
+import audeer
+
 import audb
 
 
-os.environ['AUDB_CACHE_ROOT'] = pytest.CACHE_ROOT
-os.environ['AUDB_SHARED_CACHE_ROOT'] = pytest.SHARED_CACHE_ROOT
+DB_NAME = 'test_load'
 
 
 @pytest.fixture(
-    scope='session',
+    scope='function',
     autouse=True,
 )
-def fixture_set_repositories():
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
+def assert_database_tmp_folder_is_deleted():
+    """Fixture to test that the ~ tmp folder gets deleted.
 
+    audb.load() first loads files to a folder
+    named after the database
+    and appended by ``'~'``.
+    This folder should be deleted in the end.
 
-DB_NAME = f'test_publish-{pytest.ID}'
-DB_ROOT = os.path.join(pytest.ROOT, 'db')
-DB_ROOT_VERSION = {
-    version: os.path.join(DB_ROOT, version) for version in
-    ['0.1.0', '1.0.0', '2.0.0', '2.1.0', '3.0.0', '4.0.0', '5.0.0', '6.0.0']
-}
-LONG_PATH = '/'.join(['audio'] * 50) + '/new.wav'
-
-
-def clear_root(root: str):
-    root = audeer.path(root)
-    if os.path.exists(root):
-        shutil.rmtree(root)
+    """
+    yield
+
+    dirs = audeer.list_dir_names(audb.default_cache_root(), recursive=True)
+    assert len([d for d in dirs if d.endswith('~')]) == 0
 
 
 @pytest.fixture(
     scope='module',
     autouse=True,
 )
-def fixture_publish_db():
+def dbs(tmpdir_factory, persistent_repository):
+    r"""Publish different versions of the same database.
+
+    Returns:
+        dictionary containing root folder for each version
 
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
+    """
+
+    # Collect single database paths
+    # and return them in the end
+    paths = {}
 
     # create db
 
     db = audformat.testing.create_db(minimal=True)
     db.name = DB_NAME
     db.schemes['scheme'] = audformat.Scheme(
         labels=['positive', 'neutral', 'negative']
@@ -67,612 +66,773 @@
     )
     audformat.testing.add_misc_table(
         db,
         'misc-in-scheme',
         pd.Index([0, 1, 2], dtype='Int64', name='idx'),
         columns={'emotion': ('scheme', None)}
     )
-    audformat.testing.add_misc_table(
-        db,
-        'misc-not-in-scheme',
-        pd.Index([0, 1, 2], dtype='Int64', name='idx'),
-        columns={'emotion': ('scheme', None)}
-    )
     db.schemes['speaker'] = audformat.Scheme(
-        labels=['adam', '11']
+        labels=['adam', 'eve']
     )
     db.schemes['misc'] = audformat.Scheme(
         'int',
         labels='misc-in-scheme',
     )
     db['files'] = audformat.Table(db.files)
     db['files']['speaker'] = audformat.Column(scheme_id='speaker')
     db['files']['speaker'].set(
-        ['adam', 'adam', 'adam', '11'],
+        ['adam', 'adam', 'eve', 'eve'],
         index=audformat.filewise_index(db.files[:4]),
     )
     db['files']['misc'] = audformat.Column(scheme_id='misc')
     db['files']['misc'].set(
         [0, 1, 1, 2],
         index=audformat.filewise_index(db.files[:4]),
     )
-    db.save(
-        DB_ROOT_VERSION['1.0.0'],
-        storage_format=audformat.define.TableStorageFormat.PICKLE,
-    )
-    audformat.testing.create_audio_files(db)
+    db.attachments['file'] = audformat.Attachment('extra/file.txt')
+    db.attachments['folder'] = audformat.Attachment('extra/folder')
 
-    # Extend version 2.0.0 by a new file with a path >260 characters
-    db['files'].extend_index(audformat.filewise_index(LONG_PATH), inplace=True)
-    db.save(DB_ROOT_VERSION['2.0.0'])
-    audformat.testing.create_audio_files(db)
+    # publish 1.0.0
 
-    # Remove one file in version 3.0.0
-    remove_file = 'audio/001.wav'
-    db.drop_files(remove_file)
-    db.save(DB_ROOT_VERSION['3.0.0'])
+    version = '1.0.0'
+    db_root = tmpdir_factory.mktemp(version)
+    paths[version] = str(db_root)
+
+    audeer.mkdir(audeer.path(db_root, 'extra/folder/sub-folder'))
+    audeer.touch(audeer.path(db_root, 'extra/file.txt'))
+    audeer.touch(audeer.path(db_root, 'extra/folder/file1.txt'))
+    audeer.touch(audeer.path(db_root, 'extra/folder/file2.txt'))
+    audeer.touch(audeer.path(db_root, 'extra/folder/sub-folder/file3.txt'))
+    db.save(db_root)
     audformat.testing.create_audio_files(db)
+    archives = db['files']['speaker'].get().dropna().to_dict()
+    audb.publish(
+        db_root,
+        version,
+        persistent_repository,
+        archives=archives,
+        verbose=False,
+    )
 
-    # Store without audio files in version 4.0.0
-    db.save(DB_ROOT_VERSION['4.0.0'])
+    # publish 1.1.0, add table, remove attachment file
+
+    previous_db_root = db_root
+    version = '1.1.0'
+    db_root = tmpdir_factory.mktemp(version)
+    paths[version] = str(db_root)
 
-    # Extend database to >20 files and store without audio in version 5.0.0
-    db['files'] = db['files'].extend_index(
-        audformat.filewise_index([f'file{n}.wav' for n in range(20)])
+    audformat.testing.add_table(
+        db, 'train', audformat.define.IndexType.SEGMENTED,
+        columns={'label': ('scheme', None)}
+    )
+    shutil.copytree(
+        audeer.path(previous_db_root, 'extra'),
+        audeer.path(db_root, 'extra'),
     )
-    assert len(db.files) > 20
-    db.save(DB_ROOT_VERSION['5.0.0'])
+    os.remove(audeer.path(db_root, 'extra/folder/file2.txt'))
 
-    # Make database non-portable in version 6.0.0
-    db = audformat.testing.create_db(minimal=True)
-    db.name = DB_NAME
-    db.schemes['scheme'] = audformat.Scheme(
-        labels=['positive', 'neutral', 'negative']
+    db.save(db_root)
+    audformat.testing.create_audio_files(db)
+    shutil.copy(
+        audeer.path(previous_db_root, 'db.csv'),
+        audeer.path(db_root, 'db.csv'),
     )
-    audformat.testing.add_table(
-        db,
-        'emotion',
-        audformat.define.IndexType.SEGMENTED,
-        num_files=5,
-        columns={'emotion': ('scheme', None)}
+    audb.publish(
+        db_root,
+        version,
+        persistent_repository,
+        verbose=False,
     )
-    audformat.testing.add_misc_table(
-        db,
-        'misc-in-scheme',
-        pd.Index([0, 1, 2], dtype='Int64', name='idx'),
-        columns={'emotion': ('scheme', None)}
+
+    # publish 1.1.1, change label
+
+    previous_db_root = db_root
+    version = '1.1.1'
+    db_root = tmpdir_factory.mktemp(version)
+    paths[version] = str(db_root)
+
+    db['train'].df['label'][0] = None
+    shutil.copytree(
+        audeer.path(previous_db_root, 'extra'),
+        audeer.path(db_root, 'extra'),
     )
-    audformat.testing.add_misc_table(
-        db,
-        'misc-not-in-scheme',
-        pd.Index([0, 1, 2], dtype='Int64', name='idx'),
-        columns={'emotion': ('scheme', None)}
+
+    db.save(db_root)
+    audformat.testing.create_audio_files(db)
+    shutil.copy(
+        audeer.path(previous_db_root, 'db.csv'),
+        audeer.path(db_root, 'db.csv'),
     )
-    db.schemes['speaker'] = audformat.Scheme(
-        labels=['adam', '11']
+    audb.publish(
+        db_root,
+        version,
+        persistent_repository,
+        verbose=False,
     )
-    db.schemes['misc'] = audformat.Scheme(
-        'int',
-        labels='misc-in-scheme',
+
+    # publish 2.0.0, alter and remove media, remove attachment
+
+    previous_db_root = db_root
+    version = '2.0.0'
+    db_root = tmpdir_factory.mktemp(version)
+    paths[version] = str(db_root)
+
+    shutil.copytree(
+        audeer.path(previous_db_root, 'extra'),
+        audeer.path(db_root, 'extra'),
     )
-    db['files'] = audformat.Table(db.files)
-    db['files']['speaker'] = audformat.Column(scheme_id='speaker')
-    db['files']['speaker'].set(
-        ['adam', 'adam', 'adam', '11'],
-        index=audformat.filewise_index(db.files[:4]),
+    del db.attachments['file']
+    os.remove(audeer.path(db_root, 'extra/file.txt'))
+
+    db.save(db_root)
+    audformat.testing.create_audio_files(db)
+    file = os.path.join(db_root, db.files[0])
+    y, sr = audiofile.read(file)
+    y[0] = 1
+    audiofile.write(file, y, sr)
+    file = db.files[-1]
+    db.pick_files(lambda x: x != file)
+    os.remove(audeer.path(db_root, file))
+    db.save(db_root)
+
+    shutil.copy(
+        os.path.join(previous_db_root, 'db.csv'),
+        os.path.join(db_root, 'db.csv'),
     )
-    db['files']['misc'] = audformat.Column(scheme_id='misc')
-    db['files']['misc'].set(
-        [0, 1, 1, 2],
-        index=audformat.filewise_index(db.files[:4]),
+    audb.publish(
+        db_root,
+        version,
+        persistent_repository,
+        verbose=False,
     )
-    db.save(DB_ROOT_VERSION['6.0.0'])
+
+    # publish 3.0.0, remove table, alter attachment file
+
+    previous_db_root = db_root
+    version = '3.0.0'
+    db_root = tmpdir_factory.mktemp(version)
+    paths[version] = str(db_root)
+
+    shutil.copytree(
+        audeer.path(previous_db_root, 'extra'),
+        audeer.path(db_root, 'extra'),
+    )
+    with open(audeer.path(db_root, 'extra/folder/file1.txt'), 'a') as fp:
+        fp.write('text')
+
+    db.drop_tables('train')
+    db.save(db_root)
     audformat.testing.create_audio_files(db)
-    db.map_files(lambda x: os.path.join(db.root, x))  # make paths absolute
-    db.save(DB_ROOT_VERSION['6.0.0'])
+    shutil.copy(
+        os.path.join(previous_db_root, 'db.csv'),
+        os.path.join(db_root, 'db.csv'),
+    )
+    audb.publish(
+        db_root,
+        version,
+        persistent_repository,
+        verbose=False,
+    )
 
-    yield
+    return paths
 
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
 
+def test_database_cache_folder(cache):
+    cache_root = os.path.join(cache, 'cache')
+    version = '1.0.0'
+    db_root = audb.core.load.database_cache_root(
+        DB_NAME,
+        version,
+        cache_root,
+    )
+    expected_db_root = os.path.join(
+        cache_root,
+        DB_NAME,
+        version,
+    )
+    assert db_root == expected_db_root
 
-@pytest.mark.parametrize(
-    'name',
-    ['?', '!', ','],
-)
-def test_invalid_archives(name):
 
-    archives = {
-        'audio/001.wav': name
-    }
-    with pytest.raises(ValueError):
-        audb.publish(
-            DB_ROOT_VERSION['1.0.0'],
-            '1.0.1',
-            pytest.PUBLISH_REPOSITORY,
-            archives=archives,
-            num_workers=pytest.NUM_WORKERS,
-            verbose=False,
-        )
+def test_load_wrong_argument():
+    with pytest.raises(TypeError):
+        audb.load(DB_NAME, typo='1.0.0')
 
 
+@pytest.mark.parametrize('only_metadata', [True, False])
+@pytest.mark.parametrize(
+    'format',
+    [
+        None,
+        'wav',
+        'flac',
+    ]
+)
 @pytest.mark.parametrize(
     'version',
     [
+        None,  # 3.0.0
         '1.0.0',
-        pytest.param(
-            '1.0.0',
-            marks=pytest.mark.xfail(raises=RuntimeError),
-        ),
+        '1.1.0',
+        '1.1.1',
         '2.0.0',
-        '3.0.0',
         pytest.param(
             '4.0.0',
-            marks=pytest.mark.xfail(
-                raises=RuntimeError,
-                reason='Files missing (fewer than 20)',
-            ),
-        ),
-        pytest.param(
-            '5.0.0',
-            marks=pytest.mark.xfail(
-                raises=RuntimeError,
-                reason='Files missing (more than 20)',
-            ),
-        ),
-        pytest.param(
-            '6.0.0',
-            marks=pytest.mark.xfail(
-                raises=RuntimeError,
-                reason='Database not portable',
-            ),
+            marks=pytest.mark.xfail(raises=RuntimeError),
         ),
     ]
 )
-def test_publish(version):
+def test_load(dbs, format, version, only_metadata):
 
-    db = audformat.Database.load(DB_ROOT_VERSION[version])
+    # When loading the first time (only_metadata=True)
+    # the database should not exists in cache
+    if only_metadata:
+        assert not audb.exists(
+            DB_NAME,
+            version=version,
+            format=format,
+        )
 
-    if not audb.versions(DB_NAME):
-        with pytest.raises(RuntimeError):
-            audb.latest_version(DB_NAME)
+    # === Load from REPOSITORY with full_path=False ===
 
-    archives = db['files']['speaker'].get().dropna().to_dict()
-    deps = audb.publish(
-        DB_ROOT_VERSION[version],
-        version,
-        pytest.PUBLISH_REPOSITORY,
-        archives=archives,
-        previous_version=None,
+    db = audb.load(
+        DB_NAME,
+        version=version,
+        format=format,
+        only_metadata=only_metadata,
+        full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
     )
-    backend = audb.core.utils.lookup_backend(DB_NAME, version)
-    number_of_files = len(set(archives.keys()))
-    number_of_archives = len(set(archives.values()))
-    assert len(deps.files) - len(deps.archives) == (
-        number_of_files - number_of_archives
+    db_root = db.meta['audb']['root']
+
+    # Load original database from folder (expected database)
+    resolved_version = version or audb.latest_version(DB_NAME)
+    db_original = audformat.Database.load(dbs[resolved_version])
+    if format is not None:
+        db_original.map_files(
+            lambda x: audeer.replace_file_extension(x, format)
+        )
+
+    # Assert database exists in cache
+    assert audb.exists(DB_NAME, version=version, format=format)
+    df = audb.cached()
+    assert df.loc[db_root]['version'] == resolved_version
+
+    # Assert files duration are stored as hidden attribute
+    if not only_metadata:
+        files_duration = {
+            os.path.join(db_root, os.path.normpath(file)): pd.to_timedelta(
+                audiofile.duration(os.path.join(db_root, file)), unit='s')
+            for file in db.files
+        }
+        assert db._files_duration == files_duration
+
+    # Assert media files are identical and (not) exist
+    pd.testing.assert_index_equal(db.files, db_original.files)
+    for file in db.files:
+        if only_metadata:
+            assert not os.path.exists(os.path.join(db_root, file))
+        else:
+            assert os.path.exists(os.path.join(db_root, file))
+
+    # Assert tables are identical and exist as CSV files
+    for table in db:
+        assert os.path.exists(os.path.join(db_root, f'db.{table}.csv'))
+        pd.testing.assert_frame_equal(
+            db_original[table].df,
+            db[table].df,
+        )
+
+    # Assert attachments are identical and files do (not) exist
+    assert db.attachments == db_original.attachments
+    for attachment in db.attachments:
+        path = audeer.path(db.root, db.attachments[attachment].path)
+        if only_metadata:
+            assert not os.path.exists(path)
+        else:
+            assert os.path.exists(path)
+            for attachment_file in db.attachments[attachment].files:
+                assert os.path.exists(audeer.path(db.root, attachment_file))
+
+    # Assert all files are listed in dependency table
+    deps = audb.dependencies(DB_NAME, version=version)
+    assert str(deps().to_string()) == str(deps)
+    assert len(deps) == (
+        len(db.files)
+        + len(db.tables)
+        + len(db.misc_tables)
+        + len(db.attachments)
     )
-    for archive in set(archives.values()):
-        assert archive in deps.archives
+
+    # === Load from CACHE with full_path=True ===
 
     db = audb.load(
         DB_NAME,
         version=version,
+        full_path=True,
+        format=format,
+        only_metadata=only_metadata,
+        num_workers=pytest.NUM_WORKERS,
+        verbose=False,
+    )
+
+    # Assert files duration are stored as hidden attribute
+    if not only_metadata:
+        files_duration = {
+            os.path.normpath(file):
+            pd.to_timedelta(audiofile.duration(file), unit='s')
+            for file in db.files
+        }
+        assert db._files_duration == files_duration
+
+    # Assert media files do (not) exist
+    for file in db.files:
+        if only_metadata:
+            assert not os.path.exists(file)
+        else:
+            assert os.path.exists(file)
+
+    # Assert table CSV files exist
+    for table in db:
+        assert os.path.exists(os.path.join(db_root, f'db.{table}.csv'))
+
+    # Assert attachments files do (not) exist
+    for attachment in db.attachments:
+        path = audeer.path(db.root, db.attachments[attachment].path)
+        if only_metadata:
+            assert not os.path.exists(path)
+        else:
+            assert os.path.exists(path)
+            for attachment_file in db.attachments[attachment].files:
+                assert os.path.exists(audeer.path(db.root, attachment_file))
+
+
+def test_load_from_cache(dbs):
+
+    # Load a database with flavor to cache
+    # and reload afterwards from cache
+    format = 'flac'
+    version = '1.0.0'
+    db = audb.load(
+        DB_NAME,
+        version='1.0.0',
+        format='flac',
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
     )
-    assert db.name == DB_NAME
+    db_root = db.meta['audb']['root']
 
-    versions = audb.versions(DB_NAME)
-    latest_version = audb.latest_version(DB_NAME)
+    # Load original database from folder (expected database)
+    db_original = audformat.Database.load(dbs[version])
+    db_original.map_files(
+        lambda x: audeer.replace_file_extension(x, format)
+    )
 
-    assert version in versions
-    assert latest_version == versions[-1]
+    # Assert database exists in cache
+    assert audb.exists(DB_NAME, version=version, format=format)
+    df = audb.cached()
+    assert df.loc[db_root]['version'] == version
 
-    df = audb.available(only_latest=False)
-    assert DB_NAME in df.index
-    assert set(df[df.index == DB_NAME]['version']) == set(versions)
+    # Assert media files are identical and exist
+    pd.testing.assert_index_equal(db.files, db_original.files)
+    for file in db.files:
+        assert os.path.exists(os.path.join(db_root, file))
 
-    df = audb.available(only_latest=True)
-    assert DB_NAME in df.index
-    assert df[df.index == DB_NAME]['version'][0] == latest_version
+    version = '2.0.0'
+    db = audb.load(
+        DB_NAME,
+        version='2.0.0',
+        format='flac',
+        full_path=False,
+        num_workers=pytest.NUM_WORKERS,
+        verbose=False,
+    )
+    db_root = db.meta['audb']['root']
+
+    # Load original database from folder (expected database)
+    db_original = audformat.Database.load(dbs[version])
+    db_original.map_files(
+        lambda x: audeer.replace_file_extension(x, format)
+    )
+
+    # Assert database exists in cache
+    assert audb.exists(DB_NAME, version=version, format=format)
+    df = audb.cached()
+    assert df.loc[db_root]['version'] == version
 
+    # Assert media files are identical and exist
+    pd.testing.assert_index_equal(db.files, db_original.files)
     for file in db.files:
-        name = archives[file] if file in archives else file
-        file_path = backend.join(db.name, 'media', name)
-        backend.exists(file_path, version)
-        path = os.path.join(DB_ROOT_VERSION[version], file)
-        assert deps.checksum(file) == audbackend.md5(path)
-        if deps.format(file) in [
-            audb.core.define.Format.WAV,
-            audb.core.define.Format.FLAC,
-        ]:
-            assert deps.bit_depth(file) == audiofile.bit_depth(path)
-            assert deps.channels(file) == audiofile.channels(path)
-            assert deps.duration(file) == audiofile.duration(path)
-            assert deps.sampling_rate(file) == audiofile.sampling_rate(path)
+        assert os.path.exists(os.path.join(db_root, file))
 
 
 @pytest.mark.parametrize(
-    'version1, version2, media_difference',
+    'version, attachment_id',
     [
         (
             '1.0.0',
-            '1.0.0',
-            [],
-        ),
-        (
-            '1.0.0',
-            '2.0.0',
-            [],
+            'file',
         ),
         (
-            '2.0.0',
             '1.0.0',
-            [LONG_PATH],
-        ),
-        (
-            '2.0.0',
-            '3.0.0',
-            ['audio/001.wav'],
+            'folder',
         ),
         (
-            '3.0.0',
-            '2.0.0',
-            [],
+            None,
+            'folder',
         ),
+    ]
+)
+def test_load_attachment(cache, version, attachment_id):
+
+    db = audb.load(
+        DB_NAME,
+        version=version,
+        verbose=False,
+    )
+
+    paths = audb.load_attachment(
+        DB_NAME,
+        attachment_id,
+        version=version,
+        verbose=False,
+    )
+
+    if version is None:
+        version = audb.latest_version(DB_NAME)
+
+    expected_paths = [
+        os.path.join(
+            cache,
+            DB_NAME,
+            version,
+            os.path.normpath(file),
+        )
+        for file in db.attachments[attachment_id].files
+    ]
+    assert paths == expected_paths
+
+    # Clear cache to force loading from other cache
+    cache_root = audb.core.load.database_cache_root(
+        DB_NAME,
+        version,
+        cache,
+        audb.Flavor(),
+    )
+    shutil.rmtree(cache_root)
+    paths2 = audb.load_attachment(
+        DB_NAME,
+        attachment_id,
+        version=version,
+        verbose=False,
+    )
+    assert paths2 == expected_paths
+
+
+@pytest.mark.parametrize(
+    'version, attachment_id, error, error_msg',
+    [
         (
             '1.0.0',
-            '3.0.0',
-            ['audio/001.wav'],
+            '',
+            ValueError,
+            "Could not find the attachment ''"
         ),
         (
-            '3.0.0',
             '1.0.0',
-            [LONG_PATH],
+            'non-existent',
+            ValueError,
+            "Could not find the attachment 'non-existent'"
         ),
     ]
 )
-def test_publish_changed_db(version1, version2, media_difference):
-
-    depend1 = audb.dependencies(DB_NAME, version=version1)
-    depend2 = audb.dependencies(DB_NAME, version=version2)
-
-    media1 = set(sorted(depend1.media))
-    media2 = set(sorted(depend2.media))
+def test_load_attachment_errors(version, attachment_id, error, error_msg):
 
-    assert media1 - media2 == set(media_difference)
+    with pytest.raises(error, match=error_msg):
+        audb.load_attachment(
+            DB_NAME,
+            attachment_id,
+            version=version,
+            verbose=False,
+        )
 
 
 @pytest.mark.parametrize(
-    'version, previous_version, error_type, error_msg',
+    'version, media, format',
     [
         (
             '1.0.0',
+            [],
             None,
-            RuntimeError,
-            (
-                "A version '1.0.0' already exists for database "
-                f"'{DB_NAME}'."
-            ),
-        ),
-        (
-            '4.0.0',
-            None,
-            RuntimeError,
-            (
-                "The following 5 files are referenced in tables "
-                "that cannot be found on disk "
-                "and are not yet part of the database: "
-                "['audio/002.wav', 'audio/003.wav', "
-                "'audio/004.wav', 'audio/005.wav', "
-                f"'{LONG_PATH}']."
-            ),
         ),
         (
-            '5.0.0',
-            None,
-            RuntimeError,
-            (
-                "The following 25 files are referenced in tables "
-                "that cannot be found on disk "
-                "and are not yet part of the database: "
-                "['audio/002.wav', 'audio/003.wav', "
-                "'audio/004.wav', 'audio/005.wav', "
-                f"'{LONG_PATH}', "
-                "'file0.wav', 'file1.wav', 'file10.wav', 'file11.wav', "
-                "'file12.wav', 'file13.wav', 'file14.wav', 'file15.wav', "
-                "'file16.wav', 'file17.wav', 'file18.wav', 'file19.wav', "
-                "'file2.wav', 'file3.wav', 'file4.wav', ...]."
-            ),
+            '1.0.0',
+            'audio/001.wav',
+            'wav',
         ),
-        (
-            '5.0.0',
+        pytest.param(
             '1.0.0',
-            RuntimeError,
-            (
-                "The following 21 files are referenced in tables "
-                "that cannot be found on disk "
-                "and are not yet part of the database: "
-                f"['{LONG_PATH}', "
-                "'file0.wav', 'file1.wav', 'file10.wav', 'file11.wav', "
-                "'file12.wav', 'file13.wav', 'file14.wav', 'file15.wav', "
-                "'file16.wav', 'file17.wav', 'file18.wav', 'file19.wav', "
-                "'file2.wav', 'file3.wav', 'file4.wav', 'file5.wav', "
-                "'file6.wav', 'file7.wav', 'file8.wav', ...]."
-            ),
+            ['audio/001.flac', 'audio/002.flac'],
+            'flac',
+            marks=pytest.mark.xfail(raises=ValueError),
         ),
         (
-            '0.1.0',
             '1.0.0',
-            ValueError,
-            (
-                "'previous_version' needs to be smaller than 'version', "
-                "but yours is 1.0.0 >= 0.1.0."
-            ),
+            ['audio/001.wav', 'audio/002.wav'],
+            'flac',
         ),
         (
-            '0.1.0',
-            '0.1.0',
-            ValueError,
-            (
-                "'previous_version' needs to be smaller than 'version', "
-                "but yours is 0.1.0 >= 0.1.0."
-            ),
+            None,
+            ['audio/001.wav'],
+            None,
         ),
     ]
 )
-def test_publish_error_messages(
-        version,
-        previous_version,
-        error_type,
-        error_msg,
-):
-    with pytest.raises(error_type, match=re.escape(error_msg)):
-        if (
-                previous_version
-                and (
-                    audeer.LooseVersion(previous_version)
-                    < audeer.LooseVersion(version)
-                )
-        ):
-            deps = audb.dependencies(
-                DB_NAME,
-                version=previous_version,
-            )
-            path = os.path.join(
-                DB_ROOT_VERSION[version],
-                audb.core.define.DEPENDENCIES_FILE,
-            )
-            deps.save(path)
-        audb.publish(
-            DB_ROOT_VERSION[version],
-            version,
-            pytest.PUBLISH_REPOSITORY,
-            previous_version=previous_version,
-            num_workers=pytest.NUM_WORKERS,
-            verbose=False,
-        )
+def test_load_media(cache, version, media, format):
 
-
-def test_update_database():
-
-    version = '2.1.0'
-    start_version = '2.0.0'
-
-    audb.load_to(
-        DB_ROOT_VERSION[version],
+    paths = audb.load_media(
         DB_NAME,
-        version=start_version,
-        num_workers=pytest.NUM_WORKERS,
+        media,
+        version=version,
+        format=format,
         verbose=False,
     )
-
-    # == Fail with missing dependency file
-    previous_version = start_version
-    dep_file = os.path.join(
-        DB_ROOT_VERSION[version],
-        audb.core.define.DEPENDENCIES_FILE,
-    )
-    os.remove(dep_file)
-    error_msg = (
-        f"You want to depend on '{previous_version}' "
-        f"of {DB_NAME}, "
-        f"but you don't have a '{audb.core.define.DEPENDENCIES_FILE}' "
-        f"file present "
-        f"in {DB_ROOT_VERSION[version]}. "
-        f"Did you forgot to call "
-        f"'audb.load_to({DB_ROOT_VERSION[version]}, {DB_NAME}, "
-        f"version={previous_version}?"
-    )
-    with pytest.raises(RuntimeError, match=re.escape(error_msg)):
-        audb.publish(
-            DB_ROOT_VERSION[version],
-            version,
-            pytest.PUBLISH_REPOSITORY,
-            previous_version=previous_version,
-            num_workers=pytest.NUM_WORKERS,
-            verbose=False,
-        )
-
-    # Reload data to restore dependency file
-    shutil.rmtree(DB_ROOT_VERSION[version])
-    db = audb.load_to(
-        DB_ROOT_VERSION[version],
+    expected_paths = [
+        os.path.join(cache, p)
+        for p in paths
+    ]
+    if format is not None:
+        expected_paths = [
+            audeer.replace_file_extension(p, format)
+            for p in expected_paths
+        ]
+    assert paths == expected_paths
+
+    # Clear cache to force loading from other cache
+    if version is None:
+        version = audb.latest_version(DB_NAME)
+    cache_root = audb.core.load.database_cache_root(
         DB_NAME,
-        version=start_version,
-        num_workers=pytest.NUM_WORKERS,
-        verbose=False,
-    )
-    # Remove one file as in version 3.0.0
-    remove_file = 'audio/001.wav'
-    remove_path = os.path.join(DB_ROOT_VERSION[version], remove_file)
-    os.remove(remove_path)
-    db.drop_files(remove_file)
-    db.save(DB_ROOT_VERSION[version])
-
-    # == Fail as 2.0.0 is not the latest version
-    previous_version = 'latest'
-    error_msg = (
-        f"You want to depend on '{audb.latest_version(DB_NAME)}' "
-        f"of {DB_NAME}, "
-        f"but the MD5 sum of your "
-        f"'{audb.core.define.DEPENDENCIES_FILE}' file "
-        f"in {DB_ROOT_VERSION[version]} "
-        f"does not match the MD5 sum of the corresponding file "
-        f"for the requested version in the repository. "
-        f"Did you forgot to call "
-        f"'audb.load_to({DB_ROOT_VERSION[version]}, {DB_NAME}, "
-        f"version='{audb.latest_version(DB_NAME)}') "
-        f"or modified the file manually?"
-    )
-    with pytest.raises(RuntimeError, match=re.escape(error_msg)):
-        audb.publish(
-            DB_ROOT_VERSION[version],
-            version,
-            pytest.PUBLISH_REPOSITORY,
-            previous_version=previous_version,
-            num_workers=pytest.NUM_WORKERS,
-            verbose=False,
-        )
-
-    # == Fail as we require a previous version
-    previous_version = None
-    error_msg = (
-        f"You did not set a dependency to a previous version, "
-        f"but you have a '{audb.core.define.DEPENDENCIES_FILE}' file present "
-        f"in {DB_ROOT_VERSION[version]}."
-    )
-    with pytest.raises(RuntimeError, match=re.escape(error_msg)):
-        audb.publish(
-            DB_ROOT_VERSION[version],
-            version,
-            pytest.PUBLISH_REPOSITORY,
-            previous_version=previous_version,
-            num_workers=pytest.NUM_WORKERS,
-            verbose=False,
-        )
-
-    previous_version = start_version
-    deps = audb.publish(
-        DB_ROOT_VERSION[version],
         version,
-        pytest.PUBLISH_REPOSITORY,
-        previous_version=previous_version,
-        num_workers=pytest.NUM_WORKERS,
-        verbose=False,
+        cache,
+        audb.Flavor(format=format),
     )
-
-    # Check that dependencies include previous and actual version only
-    versions = audeer.sort_versions([deps.version(f) for f in deps.files])
-    assert versions[-1] == version
-    assert versions[0] == previous_version
-
-    # Check that there is no difference in the database
-    # if published from scratch or from previous version
-    db1 = audb.load(
+    shutil.rmtree(cache_root)
+    paths2 = audb.load_media(
         DB_NAME,
+        media,
         version=version,
-        full_path=False,
-        num_workers=pytest.NUM_WORKERS,
+        format=format,
         verbose=False,
     )
-    db2 = audb.load(
+    assert paths2 == paths
+
+
+@pytest.mark.parametrize(
+    'version, table',
+    [
+        (
+            '1.0.0',
+            'emotion',
+        ),
+        pytest.param(
+            '1.0.0',
+            'non-existing-table',
+            marks=pytest.mark.xfail(raises=ValueError),
+        ),
+        (
+            None,
+            'emotion',
+        ),
+    ]
+)
+def test_load_table(version, table):
+
+    df = audb.load_table(
         DB_NAME,
-        version='3.0.0',
-        full_path=False,
-        num_workers=pytest.NUM_WORKERS,
+        table,
+        version=version,
         verbose=False,
     )
-    db1.meta['audb'] = {}
-    db2.meta['audb'] = {}
-    assert db1 == db2
+    if version is None:
+        expected_files = [
+            'audio/001.wav',
+            'audio/002.wav',
+            'audio/003.wav',
+            'audio/004.wav',
+        ]
+    elif version == '1.0.0':
+        expected_files = [
+            'audio/001.wav',
+            'audio/002.wav',
+            'audio/003.wav',
+            'audio/004.wav',
+            'audio/005.wav',
+        ]
+    files = sorted(list(set(df.index.get_level_values('file'))))
+    assert files == expected_files
 
 
-def test_update_database_without_media(tmpdir):
-
-    build_root = tmpdir
-    previous_version = '1.0.0'
-    version = '1.1.0'
-
-    new_table = 'new'
-    new_files = [
-        'new/001.wav',
-        'new/002.wav',
-    ]
-    alter_files = [
-        'audio/001.wav',  # same archive as 'audio/00[2,3].wav'
-        'audio/005.wav',
-    ]
-    rem_files = [
-        'new/003.wav',  # same archive as 'audio/00[1,2].wav'
+@pytest.mark.parametrize(
+    'version',
+    [
+        None,
+        '1.0.0',
+        '1.1.0',
+        '1.1.1',
+        '2.0.0',
+        '3.0.0',
+        pytest.param(
+            '4.0.0',
+            marks=pytest.mark.xfail(raises=RuntimeError),
+        ),
     ]
+)
+@pytest.mark.parametrize('only_metadata', [True, False])
+def test_load_to(tmpdir, dbs, version, only_metadata):
+
+    db_root = audeer.path(tmpdir, 'raw')
 
-    # load without media
     db = audb.load_to(
-        build_root,
+        db_root,
         DB_NAME,
-        only_metadata=True,
-        version=previous_version,
+        version=version,
+        only_metadata=only_metadata,
         num_workers=pytest.NUM_WORKERS,
         verbose=False,
     )
-    for file in db.files:
-        assert not os.path.exists(audeer.path(build_root, file))
+    assert db.root == db_root
 
-    # update and save database
+    # Load original database from folder (expected database)
+    resolved_version = version or audb.latest_version(DB_NAME)
+    db_original = audformat.Database.load(dbs[resolved_version])
 
-    # remove files
-    for file in rem_files:
-        db.drop_files(file)
-
-    # create and alter files
-    sampling_rate = 16000
-    signal = np.ones((1, sampling_rate), np.float32)
-    for file in new_files + alter_files:
-        path = audeer.path(build_root, file)
-        audeer.mkdir(os.path.dirname(path))
-        audiofile.write(path, signal, sampling_rate)
+    # Assert media files are identical and do (not) exist
+    pd.testing.assert_index_equal(db.files, db_original.files)
+    for file in db.files:
+        if only_metadata:
+            assert not os.path.exists(os.path.join(db_root, file))
+        else:
+            assert os.path.exists(os.path.join(db_root, file))
+
+    # Assert tables are identical and exist as CSV files
+    for table in db:
+        assert os.path.exists(os.path.join(db_root, f'db.{table}.csv'))
+        pd.testing.assert_frame_equal(
+            db_original[table].df,
+            db[table].df,
+        )
 
-    # add new table
-    db[new_table] = audformat.Table(audformat.filewise_index(new_files))
+    # Assert attachments are identical and files exist
+    assert db.attachments == db_original.attachments
+    for attachment in db.attachments:
+        path = audeer.path(db.root, db.attachments[attachment].path)
+        if only_metadata:
+            assert not os.path.exists(path)
+        else:
+            assert os.path.exists(path)
+            for attachment_file in db.attachments[attachment].files:
+                assert os.path.exists(audeer.path(db.root, attachment_file))
+
+
+@pytest.mark.parametrize('only_metadata', [True, False])
+def test_load_to_update(tmpdir, dbs, only_metadata):
+
+    # Use version 1.0.0 as this contains two attachments,
+    # one file and one folder
+    # which is needed to reach full code coverage
+    version = '1.0.0'
 
-    db.save(build_root)
+    db_root = audeer.path(tmpdir, 'raw')
 
-    # publish database
-    audb.publish(
-        build_root,
-        version,
-        pytest.PUBLISH_REPOSITORY,
-        previous_version=previous_version,
+    db = audb.load_to(
+        db_root,
+        DB_NAME,
+        version=version,
+        only_metadata=only_metadata,
+        num_workers=pytest.NUM_WORKERS,
         verbose=False,
     )
+    assert db.root == db_root
 
-    # check if missing archive files were downloaded during publish
-    assert os.path.exists(audeer.path(build_root, 'audio/002.wav'))
+    # Remove some files
+    if not only_metadata:
+        media = audeer.path(db_root, db.files[0])
+        os.remove(media)
+    table = audeer.path(db_root, f'db.{list(db)[0]}.csv')
+    os.remove(table)
+
+    # Change some files
+    if not only_metadata:
+        for attachment_id in list(db.attachments):
+            attachment = audeer.path(
+                db_root,
+                db.attachments[attachment_id].path,
+            )
+            if os.path.isdir(attachment):
+                audeer.touch(audeer.path(attachment, 'other-file.txt'))
+            else:
+                with open(attachment, 'a') as fp:
+                    fp.write('next')
 
-    # load new version and check media
-    db_load = audb.load(
+    # Load again to force restoring to original state
+    db = audb.load_to(
+        db_root,
         DB_NAME,
         version=version,
+        only_metadata=only_metadata,
+        num_workers=pytest.NUM_WORKERS,
+        verbose=False,
     )
+    assert db.root == db_root
+
+    # Load original database from folder (expected database)
+    resolved_version = version or audb.latest_version(DB_NAME)
+    db_original = audformat.Database.load(dbs[resolved_version])
+
+    # Assert media files are identical and do (not) exist
+    pd.testing.assert_index_equal(db.files, db_original.files)
     for file in db.files:
-        assert os.path.exists(audeer.path(db_load.root, file))
-    for file in rem_files:
-        assert not os.path.exists(audeer.path(db_load.root, file))
-    for file in new_files + alter_files:
-        assert filecmp.cmp(
-            audeer.path(build_root, file),
-            audeer.path(db_load.root, file),
+        if only_metadata:
+            assert not os.path.exists(os.path.join(db_root, file))
+        else:
+            assert os.path.exists(os.path.join(db_root, file))
+
+    # Assert tables are identical and exist as CSV files
+    for table in db:
+        assert os.path.exists(os.path.join(db_root, f'db.{table}.csv'))
+        pd.testing.assert_frame_equal(
+            db_original[table].df,
+            db[table].df,
         )
 
+    # Assert attachments are identical and files exist
+    assert db.attachments == db_original.attachments
+    for attachment in db.attachments:
+        path = audeer.path(db.root, db.attachments[attachment].path)
+        if only_metadata:
+            assert not os.path.exists(path)
+        else:
+            assert os.path.exists(path)
+            for attachment_file in db.attachments[attachment].files:
+                assert os.path.exists(audeer.path(db.root, attachment_file))
 
-def test_cached():
-    # Check first that we have different database names available
-    df = audb.cached()
-    names = list(set(df.name))
-    assert len(names) > 1
-    df = audb.cached(name=names[0])
-    assert set(df.name) == set([names[0]])
+
+@pytest.mark.parametrize(
+    'name, version',
+    [
+        (DB_NAME, None),
+        (DB_NAME, '1.0.0'),
+        pytest.param(  # database does not exist
+            'does-not-exist', None,
+            marks=pytest.mark.xfail(raises=RuntimeError),
+        ),
+        pytest.param(  # version does not exist
+            DB_NAME, 'does-not-exist',
+            marks=pytest.mark.xfail(raises=RuntimeError),
+        )
+    ]
+)
+def test_repository(persistent_repository, name, version):
+    repository = audb.repository(name, version)
+    assert repository == persistent_repository
```

### Comparing `audb-1.4.2/tests/test_remove.py` & `audb-1.5.0/tests/test_remove.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,101 @@
 import os
-import shutil
 
 import pytest
 
 import audformat.testing
 import audeer
 
 import audb
 
 
-os.environ['AUDB_CACHE_ROOT'] = pytest.CACHE_ROOT
-os.environ['AUDB_SHARED_CACHE_ROOT'] = pytest.SHARED_CACHE_ROOT
-
-
-@pytest.fixture(
-    scope='session',
-    autouse=True,
-)
-def fixture_set_repositories():
-    audb.config.REPOSITORIES = pytest.REPOSITORIES
-
-
-DB_NAME = f'test_remove-{pytest.ID}'
-DB_ROOT = os.path.join(pytest.ROOT, 'db')
+DB_NAME = 'test_remove'
 DB_FILES = {
     '1.0.0': [
         'audio/bundle1.wav',
         'audio/bundle2.wav',
         'audio/single.wav',
     ],
     '2.0.0': [
         'audio/new.wav',
     ],
 }
 
 
-def clear_root(root: str):
-    root = audeer.path(root)
-    if os.path.exists(root):
-        shutil.rmtree(root)
-
+@pytest.fixture(
+    scope='module',
+    autouse=True,
+)
+def dbs(tmpdir_factory, persistent_repository):
+    r"""Publish databases.
 
-@pytest.fixture
-def publish_db():
+    This publishes a database with the name ``DB_NAME``
+    and the versions 1.0.0 and 2.0.0
+    to a module wide repository.
 
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
+    """
+    db_root = tmpdir_factory.mktemp('db')
 
     # create db
 
     db = audformat.testing.create_db(minimal=True)
     db.name = DB_NAME
     db['files'] = audformat.Table(audformat.filewise_index(DB_FILES['1.0.0']))
 
     # publish 1.0.0
 
-    db.save(DB_ROOT)
+    db.save(db_root)
     audformat.testing.create_audio_files(db)
     archives = {
         db.files[0]: 'bundle',
         db.files[1]: 'bundle',
     }
     audb.publish(
-        DB_ROOT,
+        db_root,
         '1.0.0',
-        pytest.PUBLISH_REPOSITORY,
+        persistent_repository,
         archives=archives,
         verbose=False,
     )
 
     # publish 2.0.0
 
     db['files'].extend_index(
         audformat.filewise_index(DB_FILES['2.0.0']),
         inplace=True,
     )
-    db.save(DB_ROOT)
+    db.save(db_root)
     audformat.testing.create_audio_files(db)
     audb.publish(
-        DB_ROOT,
+        db_root,
         '2.0.0',
-        pytest.PUBLISH_REPOSITORY,
+        persistent_repository,
         verbose=False,
     )
 
-    yield
-
-    clear_root(DB_ROOT)
-    clear_root(pytest.FILE_SYSTEM_HOST)
-
 
 @pytest.mark.parametrize(
     'format',
     [
         None,
         'wav',
         'flac',
     ]
 )
-def test_remove(publish_db, format):
+def test_remove(cache, format):
 
     for remove in (
             DB_FILES['1.0.0'][0],  # bundle1
             DB_FILES['1.0.0'][1],  # bundle2
             DB_FILES['1.0.0'][2],  # single
             DB_FILES['2.0.0'][0],  # new
     ):
 
         # remove db cache to ensure we always get a fresh copy
-        shutil.rmtree(pytest.CACHE_ROOT)
+        audeer.rmdir(cache)
 
         audb.remove_media(DB_NAME, remove)
 
         for removed_media in [False, True]:
 
             for version in audb.versions(DB_NAME):
```

