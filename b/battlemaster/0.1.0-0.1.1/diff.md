# Comparing `tmp/battlemaster-0.1.0.tar.gz` & `tmp/battlemaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battlemaster-0.1.0.tar", last modified: Thu Apr 27 00:46:36 2023, max compression
+gzip compressed data, was "battlemaster-0.1.1.tar", last modified: Thu Apr 27 01:55:07 2023, max compression
```

## Comparing `battlemaster-0.1.0.tar` & `battlemaster-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:36.854452 battlemaster-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-27 00:46:18.000000 battlemaster-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 00:46:36.854452 battlemaster-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 00:46:18.000000 battlemaster-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:36.854452 battlemaster-0.1.0/battlemaster/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 00:46:18.000000 battlemaster-0.1.0/battlemaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:36.854452 battlemaster-0.1.0/battlemaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 00:46:36.000000 battlemaster-0.1.0/battlemaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 00:46:36.000000 battlemaster-0.1.0/battlemaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:46:36.000000 battlemaster-0.1.0/battlemaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 00:46:36.000000 battlemaster-0.1.0/battlemaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:46:36.854452 battlemaster-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-27 00:46:18.000000 battlemaster-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:36.854452 battlemaster-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 00:46:18.000000 battlemaster-0.1.0/test/test_battlemaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:55:07.250473 battlemaster-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-27 01:54:52.000000 battlemaster-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 01:55:07.250473 battlemaster-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 01:54:52.000000 battlemaster-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:55:07.250473 battlemaster-0.1.1/battlemaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 01:54:52.000000 battlemaster-0.1.1/battlemaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:55:07.250473 battlemaster-0.1.1/battlemaster/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 01:54:52.000000 battlemaster-0.1.1/battlemaster/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:55:07.250473 battlemaster-0.1.1/battlemaster/rules/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 01:54:52.000000 battlemaster-0.1.1/battlemaster/rules/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-27 01:54:52.000000 battlemaster-0.1.1/battlemaster/rules/tables/hex_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 01:54:52.000000 battlemaster-0.1.1/battlemaster/rules/tables/turn_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:55:07.250473 battlemaster-0.1.1/battlemaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 01:55:07.000000 battlemaster-0.1.1/battlemaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 01:55:07.000000 battlemaster-0.1.1/battlemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:55:07.000000 battlemaster-0.1.1/battlemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 01:55:07.000000 battlemaster-0.1.1/battlemaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 01:55:07.250473 battlemaster-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-27 01:54:52.000000 battlemaster-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:55:07.250473 battlemaster-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 01:54:52.000000 battlemaster-0.1.1/test/test_battlemaster.py
```

### Comparing `battlemaster-0.1.0/LICENSE.txt` & `battlemaster-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `battlemaster-0.1.0/setup.py` & `battlemaster-0.1.1/setup.py`

 * *Files identical despite different names*

