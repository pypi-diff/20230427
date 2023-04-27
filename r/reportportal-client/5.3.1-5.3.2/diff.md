# Comparing `tmp/reportportal-client-5.3.1.tar.gz` & `tmp/reportportal-client-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportportal-client-5.3.1.tar", last modified: Tue Apr 18 12:53:00 2023, max compression
+gzip compressed data, was "reportportal-client-5.3.2.tar", last modified: Thu Apr 27 13:40:30 2023, max compression
```

## Comparing `reportportal-client-5.3.1.tar` & `reportportal-client-5.3.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.983669 reportportal-client-5.3.1/reportportal_client/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.983669 reportportal-client-5.3.1/reportportal_client/_local/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/rp_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/item_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_base_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/items/rp_log_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_log_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_log_items/rp_log_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_base_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_child_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_root_test_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/logs/log_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/services/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/services/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.987669 reportportal-client-5.3.1/reportportal_client/static/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/static/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/reportportal_client/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/reportportal_client/steps/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.983669 reportportal-client-5.3.1/reportportal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 12:53:00.000000 reportportal-client-5.3.1/reportportal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:53:00.991669 reportportal-client-5.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-18 12:52:54.000000 reportportal-client-5.3.1/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.850358 reportportal-client-5.3.2/reportportal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.854358 reportportal-client-5.3.2/reportportal_client/_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/client.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.854358 reportportal-client-5.3.2/reportportal_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/rp_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/item_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_base_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/items/rp_log_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_log_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_log_items/rp_log_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_base_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_child_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_root_test_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/logs/log_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/services/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/static/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/reportportal_client/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/reportportal_client/steps/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.854358 reportportal-client-5.3.2/reportportal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 13:40:30.000000 reportportal-client-5.3.2/reportportal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:40:30.858358 reportportal-client-5.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-27 13:40:26.000000 reportportal-client-5.3.2/tests/test_statistics.py
```

### Comparing `reportportal-client-5.3.1/CONTRIBUTING.rst` & `reportportal-client-5.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/LICENSE.md` & `reportportal-client-5.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/PKG-INFO` & `reportportal-client-5.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.1
+Version: 5.3.2
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.1
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.2
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reportportal-client-5.3.1/README.md` & `reportportal-client-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/__init__.py` & `reportportal-client-5.3.2/reportportal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/_local/__init__.py` & `reportportal-client-5.3.2/reportportal_client/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/client.py` & `reportportal-client-5.3.2/reportportal_client/client.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/client.pyi` & `reportportal-client-5.3.2/reportportal_client/client.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/__init__.py` & `reportportal-client-5.3.2/reportportal_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/rp_file.py` & `reportportal-client-5.3.2/reportportal_client/core/rp_file.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/rp_issues.py` & `reportportal-client-5.3.2/reportportal_client/core/rp_issues.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/rp_requests.py` & `reportportal-client-5.3.2/reportportal_client/core/rp_requests.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/rp_responses.py` & `reportportal-client-5.3.2/reportportal_client/core/rp_responses.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/test_manager.py` & `reportportal-client-5.3.2/reportportal_client/core/test_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/core/worker.py` & `reportportal-client-5.3.2/reportportal_client/core/worker.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/errors.py` & `reportportal-client-5.3.2/reportportal_client/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/helpers.py` & `reportportal-client-5.3.2/reportportal_client/helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/helpers.pyi` & `reportportal-client-5.3.2/reportportal_client/helpers.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/__init__.py` & `reportportal-client-5.3.2/reportportal_client/items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/item_weight.py` & `reportportal-client-5.3.2/reportportal_client/items/item_weight.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_base_item.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_base_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_log_items/__init__.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_log_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_log_items/rp_log_item.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_log_items/rp_log_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/__init__.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_base_test_item.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_base_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_child_test_item.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_child_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/items/rp_test_items/rp_root_test_item.py` & `reportportal-client-5.3.2/reportportal_client/items/rp_test_items/rp_root_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/logs/__init__.py` & `reportportal-client-5.3.2/reportportal_client/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/logs/log_manager.py` & `reportportal-client-5.3.2/reportportal_client/logs/log_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/services/__init__.py` & `reportportal-client-5.3.2/reportportal_client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/services/client_id.py` & `reportportal-client-5.3.2/reportportal_client/services/client_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 import configparser
 import io
+import logging
 import os
 from uuid import uuid4
 
 import six
 
 from .constants import CLIENT_ID_PROPERTY, RP_FOLDER_PATH, \
     RP_PROPERTIES_FILE_PATH
 
 
+logger = logging.getLogger(__name__)
+logger.addHandler(logging.NullHandler())
+
+
 class __NoSectionConfigParser(configparser.ConfigParser):
     DEFAULT_SECTION = 'DEFAULT'
 
     def __preprocess_file(self, fp):
         content = u'[' + self.DEFAULT_SECTION + ']\n' + fp.read()
         return io.StringIO(content)
 
@@ -73,9 +78,13 @@
 
 
 def get_client_id():
     """Return unique client ID of the instance, generate new if not exists."""
     client_id = _read_client_id()
     if not client_id:
         client_id = str(uuid4())
-        _store_client_id(client_id)
+        try:
+            _store_client_id(client_id)
+        except (PermissionError, IOError) as error:
+            logger.exception('[%s] Unknown exception has occurred. '
+                             'Skipping client ID saving.', error)
     return client_id
```

### Comparing `reportportal-client-5.3.1/reportportal_client/services/constants.py` & `reportportal-client-5.3.2/reportportal_client/services/constants.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/services/statistics.py` & `reportportal-client-5.3.2/reportportal_client/services/statistics.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/static/__init__.py` & `reportportal-client-5.3.2/reportportal_client/static/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/static/abstract.py` & `reportportal-client-5.3.2/reportportal_client/static/abstract.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/static/defines.py` & `reportportal-client-5.3.2/reportportal_client/static/defines.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/static/errors.py` & `reportportal-client-5.3.2/reportportal_client/static/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/steps/__init__.py` & `reportportal-client-5.3.2/reportportal_client/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client/steps/__init__.pyi` & `reportportal-client-5.3.2/reportportal_client/steps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/reportportal_client.egg-info/PKG-INFO` & `reportportal-client-5.3.2/reportportal_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.1
+Version: 5.3.2
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.1
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.2
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reportportal-client-5.3.1/reportportal_client.egg-info/SOURCES.txt` & `reportportal-client-5.3.2/reportportal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/setup.py` & `reportportal-client-5.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config for setup package client Python."""
 
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '5.3.1'
+__version__ = '5.3.2'
 
 TYPE_STUBS = ['*.pyi']
 
 
 def read_file(fname):
     """Read the given file.
```

### Comparing `reportportal-client-5.3.1/tests/test_client.py` & `reportportal-client-5.3.2/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,23 +119,23 @@
     rp_client.session.get.side_effect = get_call
 
     assert rp_client.get_launch_ui_url() == expected_url
 
 
 @mock.patch('reportportal_client.client.getenv')
 @mock.patch('reportportal_client.client.send_event')
-def test_skip_analytics(send_event, getenv):
+def test_skip_statistics(send_event, getenv):
     getenv.return_value = '1'
     client = RPClient('http://endpoint', 'project', 'token')
     client.session = mock.Mock()
     client.start_launch('Test Launch', timestamp())
     assert mock.call('start_launch', None, None) not in send_event.mock_calls
 
 
 @mock.patch('reportportal_client.client.getenv')
 @mock.patch('reportportal_client.client.send_event')
-def test_analytics(send_event, getenv):
+def test_statistics(send_event, getenv):
     getenv.return_value = ''
     client = RPClient('http://endpoint', 'project', 'token')
     client.session = mock.Mock()
     client.start_launch('Test Launch', timestamp())
     assert mock.call('start_launch', None, None) in send_event.mock_calls
```

### Comparing `reportportal-client-5.3.1/tests/test_client_id.py` & `reportportal-client-5.3.2/tests/test_client_id.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/tests/test_helpers.py` & `reportportal-client-5.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.1/tests/test_statistics.py` & `reportportal-client-5.3.2/tests/test_statistics.py`

 * *Files identical despite different names*

