# Comparing `tmp/pyatlan-0.0.22.tar.gz` & `tmp/pyatlan-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.22.tar", last modified: Wed Apr 12 16:58:44 2023, max compression
+gzip compressed data, was "pyatlan-0.0.23.tar", last modified: Thu Apr 27 16:51:06 2023, max compression
```

## Comparing `pyatlan-0.0.22.tar` & `pyatlan-0.0.23.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.774000 pyatlan-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-12 16:58:34.000000 pyatlan-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:58:34.000000 pyatlan-0.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 16:58:34.000000 pyatlan-0.0.22/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 16:58:44.774000 pyatlan-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 16:58:34.000000 pyatlan-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.766000 pyatlan-0.0.22/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   748743 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:58:34.000000 pyatlan-0.0.22/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.766000 pyatlan-0.0.22/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 16:58:44.000000 pyatlan-0.0.22/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:58:44.774000 pyatlan-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-12 16:58:34.000000 pyatlan-0.0.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.770000 pyatlan-0.0.22/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.774000 pyatlan-0.0.22/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:58:44.774000 pyatlan-0.0.22/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    48559 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 16:58:34.000000 pyatlan-0.0.22/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.412176 pyatlan-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-27 16:50:54.000000 pyatlan-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 16:50:54.000000 pyatlan-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 16:50:54.000000 pyatlan-0.0.23/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-27 16:51:06.412176 pyatlan-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-27 16:50:54.000000 pyatlan-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.404176 pyatlan-0.0.23/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.404176 pyatlan-0.0.23/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.408176 pyatlan-0.0.23/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.408176 pyatlan-0.0.23/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.408176 pyatlan-0.0.23/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.408176 pyatlan-0.0.23/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   756677 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 16:50:54.000000 pyatlan-0.0.23/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.404176 pyatlan-0.0.23/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-27 16:51:06.000000 pyatlan-0.0.23/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-27 16:51:06.000000 pyatlan-0.0.23/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:51:06.000000 pyatlan-0.0.23/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:51:06.000000 pyatlan-0.0.23/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 16:51:06.000000 pyatlan-0.0.23/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 16:51:06.000000 pyatlan-0.0.23/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:51:06.412176 pyatlan-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-27 16:50:54.000000 pyatlan-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.408176 pyatlan-0.0.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.408176 pyatlan-0.0.23/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:51:06.412176 pyatlan-0.0.23/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48518 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-27 16:50:54.000000 pyatlan-0.0.23/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.22/LICENSE` & `pyatlan-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/PKG-INFO` & `pyatlan-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.22
+Version: 0.0.23
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.22/README.md` & `pyatlan-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.23/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.23/pyatlan/cache/custom_metadata_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import json
-from typing import Optional
+from typing import Any, Optional
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.error import LogicError, NotFoundError
+from pyatlan.model.core import CustomMetadata
 from pyatlan.model.enums import AtlanTypeCategory
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef
 
 
 class Synonym:
     def __init__(self, storage_name):
         self.storage_name = storage_name
@@ -31,15 +32,15 @@
     map_attr_id_to_name: dict[str, dict[str, str]] = dict()
     map_attr_name_to_id: dict[str, dict[str, str]] = dict()
     archived_attr_ids: dict[str, str] = dict()
     types_by_asset: dict[str, set[type]] = dict()
 
     @classmethod
     def _refresh_cache(cls) -> None:
-        from pyatlan.model.core import BusinessAttributes, to_snake_case
+        from pyatlan.model.core import CustomMetadata, to_snake_case
 
         client = AtlanClient.get_default_client()
         if client is None:
             client = AtlanClient()
         response = client.get_typedefs(type_category=AtlanTypeCategory.CUSTOM_METADATA)
         if response is not None:
             cls.map_id_to_name = {}
@@ -54,15 +55,15 @@
                 cls.cache_by_id[type_id] = cm
                 cls.map_id_to_name[type_id] = type_name
                 cls.map_name_to_id[type_name] = type_id
                 cls.map_attr_id_to_name[type_id] = {}
                 cls.map_attr_name_to_id[type_id] = {}
                 meta_name = cm.display_name.replace(" ", "")
                 attribute_class_name = f"Attributes_{meta_name}"
-                attrib_type = type(attribute_class_name, (BusinessAttributes,), {})
+                attrib_type = type(attribute_class_name, (CustomMetadata,), {})
                 attrib_type._meta_data_type_id = type_id  # type: ignore
                 attrib_type._meta_data_type_name = type_name  # type: ignore
                 cls.map_id_to_type[type_id] = attrib_type
                 applicable_types: set[str] = set()
                 if cm.attribute_defs:
                     for attr in cm.attribute_defs:
                         if attr.options.custom_applicable_entity_types:
@@ -198,7 +199,34 @@
         """
         if set_id := cls.get_id_for_name(set_name):
             if dot_names := cls._get_attributes_for_search_results(set_id):
                 return dot_names
             cls._refresh_cache()
             return cls._get_attributes_for_search_results(set_id)
         return None
+
+    @classmethod
+    def get_custom_metadata(
+        cls,
+        name: str,
+        asset_type: type,
+        business_attributes: Optional[dict[str, Any]] = None,
+    ) -> CustomMetadata:
+        type_name = asset_type.__name__
+        ba_id = cls.get_id_for_name(name)
+        if ba_id is None:
+            raise ValueError(f"No custom metadata with the name: {name} exist")
+        for a_type in CustomMetadataCache.types_by_asset[type_name]:
+            if (
+                hasattr(a_type, "_meta_data_type_name")
+                and a_type._meta_data_type_name == name
+            ):
+                break
+        else:
+            raise ValueError(f"Custom metadata {name} is not applicable to {type_name}")
+        if ba_type := CustomMetadataCache.get_type_for_id(ba_id):
+            return (
+                ba_type(business_attributes[ba_id])
+                if business_attributes and ba_id in business_attributes
+                else ba_type()
+            )
+        raise ValueError(f"Custom metadata {name} is not applicable to {type_name}")
```

### Comparing `pyatlan-0.0.22/pyatlan/cache/role_cache.py` & `pyatlan-0.0.23/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/client/atlan.py` & `pyatlan-0.0.23/pyatlan/client/atlan.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     parse_obj_as,
     validate_arguments,
 )
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from pyatlan.client.constants import (
+    ADD_BUSINESS_ATTRIBUTE_BY_ID,
     BULK_UPDATE,
     CREATE_TYPE_DEFS,
     DELETE_ENTITY_BY_ATTRIBUTE,
     DELETE_ENTITY_BY_GUID,
     DELETE_TYPE_DEF_BY_NAME,
     GET_ALL_TYPE_DEFS,
     GET_ENTITY_BY_GUID,
@@ -53,14 +54,16 @@
     AssetRequest,
     AssetResponse,
     AtlanObject,
     BulkRequest,
     Classification,
     ClassificationName,
     Classifications,
+    CustomMetadata,
+    CustomMetadataReqest,
 )
 from pyatlan.model.enums import AtlanDeleteType, AtlanTypeCategory, CertificateStatus
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
 from pyatlan.model.search import IndexSearchRequest
 from pyatlan.model.typedef import (
     ClassificationDef,
@@ -373,19 +376,20 @@
         )
 
     def upsert(
         self,
         entity: Union[Asset, list[Asset]],
         replace_classifications: bool = False,
         replace_custom_metadata: bool = False,
+        overwrite_custom_metadata: bool = False,
     ) -> AssetMutationResponse:
         query_params = {
             "replaceClassifications": replace_classifications,
             "replaceBusinessAttributes": replace_custom_metadata,
-            "overwriteBusinessAttribute": replace_custom_metadata,
+            "overwriteBusinessAttributes": overwrite_custom_metadata,
         }
         entities: list[Asset] = []
         if isinstance(entity, list):
             entities.extend(entity)
         else:
             entities.append(entity)
         for asset in entities:
@@ -583,7 +587,18 @@
         self, asset_type: Type[A], qualified_name: str, name: str
     ) -> Optional[A]:
         asset = asset_type()
         asset.qualified_name = qualified_name
         asset.name = name
         asset.remove_announcement()
         return self._update_asset_by_attribute(asset, asset_type, qualified_name)
+
+    def replace_custom_metadata(self, guid: str, custom_metadata: CustomMetadata):
+        # TODO: This endpoint is not currently functioning correctly on the server
+        custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
+        self._call_api(
+            ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
+                {"entity_guid": guid, "bm_id": custom_metadata._meta_data_type_id}
+            ),
+            None,
+            custom_metadata_request,
+        )
```

### Comparing `pyatlan-0.0.22/pyatlan/client/constants.py` & `pyatlan-0.0.23/pyatlan/client/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,20 @@
     HTTPMethod.DELETE,
     HTTPStatus.NO_CONTENT,
 )
 GET_BULK_HEADERS = API(ENTITY_API + BULK_HEADERS, HTTPMethod.GET, HTTPStatus.OK)
 
 # Business Attributes APIs
 ADD_BUSINESS_ATTRIBUTE = API(
-    ENTITY_API + "guid/{entity_guid}/businessmetadata",
+    ENTITY_API + "guid/{entity_guid}/businessmetadata/",
+    HTTPMethod.POST,
+    HTTPStatus.NO_CONTENT,
+)
+ADD_BUSINESS_ATTRIBUTE_BY_ID = API(
+    ENTITY_API + "guid/{entity_guid}/businessmetadata/{bm_id}",
     HTTPMethod.POST,
     HTTPStatus.NO_CONTENT,
 )
 ADD_BUSINESS_ATTRIBUTE_BY_NAME = API(
     ENTITY_API + "guid/{entity_guid}/businessmetadata/{bm_name}",
     HTTPMethod.POST,
     HTTPStatus.NO_CONTENT,
```

### Comparing `pyatlan-0.0.22/pyatlan/error.py` & `pyatlan-0.0.23/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/exceptions.py` & `pyatlan-0.0.23/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.23/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/model/assets.py` & `pyatlan-0.0.23/pyatlan/model/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Any, ClassVar, Dict, List, Optional, TypeVar
 
 from pydantic import Field, StrictStr, root_validator, validator
 
 from pyatlan.model.core import (
     Announcement,
     AtlanObject,
-    BusinessAttributes,
     Classification,
+    CustomMetadata,
     Meaning,
 )
 from pyatlan.model.enums import (
     ADLSAccessTier,
     ADLSAccountStatus,
     ADLSEncryptionTypes,
     ADLSLeaseState,
@@ -242,59 +242,59 @@
 
     unique_attributes: Optional[dict[str, Any]] = Field(None)
 
     def validate_required(self):
         if not self.create_time or self.created_by:
             self.attributes.validate_required()
 
-    def get_business_attributes(self, name: str) -> BusinessAttributes:
+    def get_custom_metadata(self, name: str) -> CustomMetadata:
         from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
         ba_id = CustomMetadataCache.get_id_for_name(name)
         if ba_id is None:
-            raise ValueError(f"No business attributes with the name: {name} exist")
+            raise ValueError(f"No custom metadata with the name: {name} exist")
         for a_type in CustomMetadataCache.types_by_asset[self.type_name]:
             if (
                 hasattr(a_type, "_meta_data_type_name")
                 and a_type._meta_data_type_name == name
             ):
                 break
         else:
             raise ValueError(
-                f"Business attributes {name} are not applicable to {self.type_name}"
+                f"Custom metadata attributes {name} are not applicable to {self.type_name}"
             )
         if ba_type := CustomMetadataCache.get_type_for_id(ba_id):
             return (
                 ba_type(self.business_attributes[ba_id])
                 if self.business_attributes and ba_id in self.business_attributes
                 else ba_type()
             )
         else:
             raise ValueError(
-                f"Business attributes {name} are not applicable to {self.type_name}"
+                f"Custom metadata attributes {name} are not applicable to {self.type_name}"
             )
 
-    def set_business_attribute(self, business_attributes: BusinessAttributes) -> None:
+    def set_custom_metadata(self, custom_metadata: CustomMetadata) -> None:
         from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
-        if not isinstance(business_attributes, BusinessAttributes):
+        if not isinstance(custom_metadata, CustomMetadata):
             raise ValueError(
-                "business_attributes must be an instance of BusinessAttributes"
+                "business_attributes must be an instance of CustomMetadata"
             )
         if (
-            type(business_attributes)
+            type(custom_metadata)
             not in CustomMetadataCache.types_by_asset[self.type_name]
         ):
             raise ValueError(
-                f"Business attributes {business_attributes._meta_data_type_name} are not applicable to {self.type_name}"
+                f"Business attributes {custom_metadata._meta_data_type_name} are not applicable to {self.type_name}"
             )
-        ba_dict = dict(business_attributes)
+        ba_dict = dict(custom_metadata)
         if not self.business_attributes:
             self.business_attributes = {}
-        self.business_attributes[business_attributes._meta_data_type_id] = ba_dict
+        self.business_attributes[custom_metadata._meta_data_type_id] = ba_dict
 
 
 class Asset(Referenceable):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Asset._convience_properties:
@@ -394,14 +394,15 @@
         "asset_dbt_job_next_run_humanized",
         "asset_dbt_environment_name",
         "asset_dbt_environment_dbt_version",
         "asset_dbt_tags",
         "asset_dbt_semantic_layer_proxy_url",
         "asset_dbt_source_freshness_criteria",
         "sample_data_url",
+        "asset_tags",
     ]
 
     @property
     def name(self) -> str:
         return self.attributes.name
 
     @name.setter
@@ -1489,14 +1490,24 @@
 
     @sample_data_url.setter
     def sample_data_url(self, sample_data_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sample_data_url = sample_data_url
 
+    @property
+    def asset_tags(self) -> Optional[set[str]]:
+        return self.attributes.asset_tags
+
+    @asset_tags.setter
+    def asset_tags(self, asset_tags: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_tags = asset_tags
+
     _subtypes_: dict[str, type] = dict()
 
     def __init_subclass__(cls, type_name=None):
         cls._subtypes_[type_name or cls.__name__.lower()] = cls
 
     @classmethod
     def create_for_modification(
@@ -1821,14 +1832,15 @@
         )
         asset_dbt_source_freshness_criteria: Optional[str] = Field(
             None, description="", alias="assetDbtSourceFreshnessCriteria"
         )
         sample_data_url: Optional[str] = Field(
             None, description="", alias="sampleDataUrl"
         )
+        asset_tags: Optional[set[str]] = Field(None, description="", alias="assetTags")
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6145,14 +6157,88 @@
     attributes: "QuickSight.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Thoughtspot(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Thoughtspot._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "thoughtspot_chart_type",
+        "thoughtspot_question_text",
+    ]
+
+    @property
+    def thoughtspot_chart_type(self) -> Optional[str]:
+        return self.attributes.thoughtspot_chart_type
+
+    @thoughtspot_chart_type.setter
+    def thoughtspot_chart_type(self, thoughtspot_chart_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_chart_type = thoughtspot_chart_type
+
+    @property
+    def thoughtspot_question_text(self) -> Optional[str]:
+        return self.attributes.thoughtspot_question_text
+
+    @thoughtspot_question_text.setter
+    def thoughtspot_question_text(self, thoughtspot_question_text: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_question_text = thoughtspot_question_text
+
+    type_name: str = Field("Thoughtspot", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Thoughtspot":
+            raise ValueError("must be Thoughtspot")
+        return v
+
+    class Attributes(BI.Attributes):
+        thoughtspot_chart_type: Optional[str] = Field(
+            None, description="", alias="thoughtspotChartType"
+        )
+        thoughtspot_question_text: Optional[str] = Field(
+            None, description="", alias="thoughtspotQuestionText"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Thoughtspot.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class PowerBI(BI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PowerBI._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -9983,17 +10069,23 @@
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
         sql_dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="sqlDbtModels"
         )  # relationship
+        foreign_key_to: Optional[list[Column]] = Field(
+            None, description="", alias="foreignKeyTo"
+        )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
+        foreign_key_from: Optional[Column] = Field(
+            None, description="", alias="foreignKeyFrom"
+        )  # relationship
         dbt_metrics: Optional[list[DbtMetric]] = Field(
             None, description="", alias="dbtMetrics"
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
         view: Optional[View] = Field(None, description="", alias="view")  # relationship
@@ -13672,14 +13764,133 @@
     attributes: "QuickSightDataset.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class ThoughtspotLiveboard(Thoughtspot):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ThoughtspotLiveboard._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotLiveboard":
+            raise ValueError("must be ThoughtspotLiveboard")
+        return v
+
+
+class ThoughtspotDashlet(Thoughtspot):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ThoughtspotDashlet._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "thoughtspot_liveboard_name",
+        "thoughtspot_liveboard_qualified_name",
+    ]
+
+    @property
+    def thoughtspot_liveboard_name(self) -> Optional[str]:
+        return self.attributes.thoughtspot_liveboard_name
+
+    @thoughtspot_liveboard_name.setter
+    def thoughtspot_liveboard_name(self, thoughtspot_liveboard_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_liveboard_name = thoughtspot_liveboard_name
+
+    @property
+    def thoughtspot_liveboard_qualified_name(self) -> Optional[str]:
+        return self.attributes.thoughtspot_liveboard_qualified_name
+
+    @thoughtspot_liveboard_qualified_name.setter
+    def thoughtspot_liveboard_qualified_name(
+        self, thoughtspot_liveboard_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_liveboard_qualified_name = (
+            thoughtspot_liveboard_qualified_name
+        )
+
+    type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotDashlet":
+            raise ValueError("must be ThoughtspotDashlet")
+        return v
+
+    class Attributes(Thoughtspot.Attributes):
+        thoughtspot_liveboard_name: Optional[str] = Field(
+            None, description="", alias="thoughtspotLiveboardName"
+        )
+        thoughtspot_liveboard_qualified_name: Optional[str] = Field(
+            None, description="", alias="thoughtspotLiveboardQualifiedName"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        thoughtspot_liveboard: Optional[ThoughtspotLiveboard] = Field(
+            None, description="", alias="thoughtspotLiveboard"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "ThoughtspotDashlet.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ThoughtspotAnswer(Thoughtspot):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ThoughtspotAnswer._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("ThoughtspotAnswer", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotAnswer":
+            raise ValueError("must be ThoughtspotAnswer")
+        return v
+
+
 class PowerBIReport(PowerBI):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PowerBIReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -20003,14 +20214,16 @@
 
 Metric.Attributes.update_forward_refs()
 
 Metabase.Attributes.update_forward_refs()
 
 QuickSight.Attributes.update_forward_refs()
 
+Thoughtspot.Attributes.update_forward_refs()
+
 PowerBI.Attributes.update_forward_refs()
 
 Preset.Attributes.update_forward_refs()
 
 Mode.Attributes.update_forward_refs()
 
 Sigma.Attributes.update_forward_refs()
@@ -20099,14 +20312,20 @@
 
 QuickSightAnalysis.Attributes.update_forward_refs()
 
 QuickSightDashboard.Attributes.update_forward_refs()
 
 QuickSightDataset.Attributes.update_forward_refs()
 
+ThoughtspotLiveboard.Attributes.update_forward_refs()
+
+ThoughtspotDashlet.Attributes.update_forward_refs()
+
+ThoughtspotAnswer.Attributes.update_forward_refs()
+
 PowerBIReport.Attributes.update_forward_refs()
 
 PowerBIMeasure.Attributes.update_forward_refs()
 
 PowerBIColumn.Attributes.update_forward_refs()
 
 PowerBITable.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.0.22/pyatlan/model/core.py` & `pyatlan-0.0.23/pyatlan/model/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,19 @@
     entity: T
 
 
 class BulkRequest(AtlanObject, GenericModel, Generic[T]):
     entities: list[T]
 
 
-class BusinessAttributes(dict):
+class CustomMetadata(dict):
     _meta_data_type_name = ""
     _meta_data_type_id = ""
 
     def __setattr__(self, key, value):
         if not hasattr(self, key):
             raise AttributeError(f"Attribute {key} does not exist")
         super().__setattr__(key, value)
+
+
+class CustomMetadataReqest(AtlanObject):
+    __root__: CustomMetadata
```

### Comparing `pyatlan-0.0.22/pyatlan/model/enums.py` & `pyatlan-0.0.23/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/model/response.py` & `pyatlan-0.0.23/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/model/role.py` & `pyatlan-0.0.23/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/model/search.py` & `pyatlan-0.0.23/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/model/structs.py` & `pyatlan-0.0.23/pyatlan/model/structs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,36 +25,36 @@
             None, description="", alias="awsCloudWatchMetricName"
         )
         aws_cloud_watch_metric_scope: str = Field(
             None, description="", alias="awsCloudWatchMetricScope"
         )
 
 
+class Histogram(AtlanObject):
+    """Description"""
+
+    class Attributes(AtlanObject):
+        boundaries: set[float] = Field(None, description="", alias="boundaries")
+        frequencies: set[float] = Field(None, description="", alias="frequencies")
+
+
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
     class Attributes(AtlanObject):
         topic_name: Optional[str] = Field(None, description="", alias="topicName")
         topic_partition: Optional[str] = Field(
             None, description="", alias="topicPartition"
         )
         topic_lag: Optional[int] = Field(None, description="", alias="topicLag")
         topic_current_offset: Optional[int] = Field(
             None, description="", alias="topicCurrentOffset"
         )
 
 
-class Histogram(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        boundaries: set[float] = Field(None, description="", alias="boundaries")
-        frequencies: set[float] = Field(None, description="", alias="frequencies")
-
-
 class DbtMetricFilter(AtlanObject):
     """Description"""
 
     class Attributes(AtlanObject):
         dbt_metric_filter_column_qualified_name: Optional[str] = Field(
             None, description="", alias="dbtMetricFilterColumnQualifiedName"
         )
```

### Comparing `pyatlan-0.0.22/pyatlan/model/typedef.py` & `pyatlan-0.0.23/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan/utils.py` & `pyatlan-0.0.23/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.23/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.22
+Version: 0.0.23
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.22/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.23/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/setup.py` & `pyatlan-0.0.23/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/integration/classification_test.py` & `pyatlan-0.0.23/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.23/tests/integration/custom_metadata_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     cm_id = CustomMetadataCache.get_id_for_name(CM_NAME)
     assert cm_id
     client.purge_typedef(cm_id)
 
 
 def test_custom_metadata_has_human_readable_properties(client: AtlanClient):
     table = client.get_asset_by_guid("5f47cfb9-1313-4f03-9213-9913fff3c878", Table)
-    anomalo = table.get_business_attributes("Anomalo")
+    anomalo = table.get_custom_metadata("Anomalo")
     assert hasattr(anomalo, "data_volume")
     assert anomalo.data_volume is None
     assert hasattr(anomalo, "data_volume_details")
     assert anomalo.data_volume_details is None
     assert hasattr(anomalo, "data_freshness")
     assert anomalo.data_freshness is None
     assert hasattr(anomalo, "data_freshness_details")
@@ -110,9 +110,23 @@
     assert anomalo.key_metrics is None
     assert hasattr(anomalo, "key_metrics_details")
     assert anomalo.key_metrics_details is None
     assert hasattr(anomalo, "validation_rules")
     assert anomalo.validation_rules is None
     assert hasattr(anomalo, "validation_rules_details")
     assert anomalo.validation_rules_details is None
-    monte_carlo = table.get_business_attributes("Monte Carlo")
+    monte_carlo = table.get_custom_metadata("Monte Carlo")
     assert monte_carlo is not None
+
+
+def test_get_custom_metadata():
+    custom_metadata = CustomMetadataCache.get_custom_metadata(
+        name="RACI", asset_type=Table
+    )
+    assert custom_metadata is not None
+
+
+def test_get_custom_metadata_when_name_is_invalid_then_raises_value_error():
+    with pytest.raises(
+        ValueError, match="No custom metadata with the name: Bogs exist"
+    ):
+        CustomMetadataCache.get_custom_metadata(name="Bogs", asset_type=Table)
```

### Comparing `pyatlan-0.0.22/tests/integration/role_test.py` & `pyatlan-0.0.23/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/integration/test_entity_model.py` & `pyatlan-0.0.23/tests/integration/test_entity_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/integration/test_index_search.py` & `pyatlan-0.0.23/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/unit/test_classification_name.py` & `pyatlan-0.0.23/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/unit/test_glossary_term.py` & `pyatlan-0.0.23/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/unit/test_model.py` & `pyatlan-0.0.23/tests/unit/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1027,38 +1027,38 @@
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_get_business_attributes_when_name_not_valid_raises_value_error(
     mock_client, table, type_def_response
 ):
     mock_client.return_value.get_typedefs.return_value = type_def_response
     with pytest.raises(
-        ValueError, match="No business attributes with the name: Zoro exist"
+        ValueError, match="No custom metadata with the name: Zoro exist"
     ):
-        table.get_business_attributes("Zoro")
+        table.get_custom_metadata("Zoro")
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_get_business_attributes_when_name_not_appropriate_for_asset_raises_value_error(
     mock_client, table, type_def_response
 ):
     mock_client.get_default_client.return_value = mock_client
     mock_client.get_typedefs.return_value = type_def_response
     with pytest.raises(
-        ValueError, match="Business attributes Moon are not applicable to Table"
+        ValueError, match="Custom metadata attributes Moon are not applicable to Table"
     ):
-        table.get_business_attributes("Moon")
+        table.get_custom_metadata("Moon")
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_get_business_attributes_with_valid_name_returns_empty_attribute_when_table_does_not_have_attribute(
     mock_client, table, type_def_response
 ):
     mock_client.return_value.get_typedefs.return_value = type_def_response
 
-    monte_carlo = table.get_business_attributes("Monte Carlo")
+    monte_carlo = table.get_custom_metadata("Monte Carlo")
 
     assert monte_carlo is not None
     assert monte_carlo.freshness is None
     assert monte_carlo.freshness_date is None
     assert monte_carlo.table_url is None
 
 
@@ -1070,54 +1070,54 @@
     table.business_attributes = {
         MONTE_CARLO: {
             FRESHNESS: "pass",
             TABLE_URL: "https://getmontecarlo.com/catalog/",
         }
     }
 
-    monte_carlo = table.get_business_attributes("Monte Carlo")
+    monte_carlo = table.get_custom_metadata("Monte Carlo")
 
     assert monte_carlo is not None
     assert monte_carlo.freshness == "pass"
     assert monte_carlo.table_url == "https://getmontecarlo.com/catalog/"
 
 
 def test_set_busines_attributes_with_non_business_attributes_object_raises_value_error(
     table,
 ):
     with pytest.raises(
         ValueError,
-        match="business_attributes must be an instance of BusinessAttributes",
+        match="business_attributes must be an instance of CustomMetadata",
     ):
-        table.set_business_attribute({})
+        table.set_custom_metadata({})
 
 
 def test_set_business_attributes_with_non_appropriate_meta_data_type_name_raises_value_error(
     table,
 ):
 
     with pytest.raises(
         ValueError,
-        match="business_attributes must be an instance of BusinessAttributes",
+        match="business_attributes must be an instance of CustomMetadata",
     ):
-        table.set_business_attribute({})
+        table.set_custom_metadata({})
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_assigning_to_invalid_business_attribute_raises_attribute_error(
     mock_client, table, type_def_response
 ):
     mock_client.return_value.get_typedefs.return_value = type_def_response
     table.business_attributes = {
         MONTE_CARLO: {
             FRESHNESS: "pass",
             TABLE_URL: "https://getmontecarlo.com/catalog/",
         }
     }
-    business_attributes = table.get_business_attributes("Monte Carlo")
+    business_attributes = table.get_custom_metadata("Monte Carlo")
     with pytest.raises(AttributeError, match="Attribute bogus does not exist"):
         business_attributes.bogus = "123"
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_set_business_attributes_with_business_attribute_not_appropriate_to_asset_raises_value_error(
     mock_client, table, type_def_response
@@ -1126,34 +1126,34 @@
 
     moon = CustomMetadataCache.get_type_for_id(MOON)()
 
     with pytest.raises(
         ValueError,
         match="Business attributes Moon are not applicable to Table",
     ):
-        table.set_business_attribute(moon)
+        table.set_custom_metadata(moon)
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_set_business_attributes_with_appropriate_business_attribute_updates_dictionary(
     mock_client, table, type_def_response
 ):
     mock_client.return_value.get_typedefs.return_value = type_def_response
 
     table.business_attributes = {
         MONTE_CARLO: {
             FRESHNESS: "pass",
             TABLE_URL: "https://getmontecarlo.com/catalog/",
         }
     }
-    monte_carlo = table.get_business_attributes("Monte Carlo")
+    monte_carlo = table.get_custom_metadata("Monte Carlo")
 
     monte_carlo.freshness = "fail"
     monte_carlo.table_url = "http://anywhere.com"
-    table.set_business_attribute(monte_carlo)
+    table.set_custom_metadata(monte_carlo)
 
     monte_carlo_dict = table.business_attributes[MONTE_CARLO]
     assert monte_carlo_dict[FRESHNESS] == monte_carlo.freshness
     assert monte_carlo_dict[TABLE_URL] == monte_carlo.table_url
 
 
 @pytest.mark.parametrize(
```

### Comparing `pyatlan-0.0.22/tests/unit/test_search_model.py` & `pyatlan-0.0.23/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.22/tests/unit/test_typedef_model.py` & `pyatlan-0.0.23/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

