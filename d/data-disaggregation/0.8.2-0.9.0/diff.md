# Comparing `tmp/data-disaggregation-0.8.2.tar.gz` & `tmp/data-disaggregation-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-disaggregation-0.8.2.tar", last modified: Tue Apr 25 06:18:03 2023, max compression
+gzip compressed data, was "data-disaggregation-0.9.0.tar", last modified: Thu Apr 27 06:20:49 2023, max compression
```

## Comparing `data-disaggregation-0.8.2.tar` & `data-disaggregation-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/data_disaggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/data_disaggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/data_disaggregation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/data_disaggregation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/data_disaggregation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 06:18:03.000000 data-disaggregation-0.8.2/data_disaggregation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:18:03.196411 data-disaggregation-0.8.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-04-25 06:17:54.000000 data-disaggregation-0.8.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:20:49.106236 data-disaggregation-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 06:20:49.106236 data-disaggregation-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:20:49.102236 data-disaggregation-0.9.0/data_disaggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/data_disaggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/data_disaggregation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/data_disaggregation/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/data_disaggregation/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/data_disaggregation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:20:49.106236 data-disaggregation-0.9.0/data_disaggregation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 06:20:49.000000 data-disaggregation-0.9.0/data_disaggregation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 06:20:49.000000 data-disaggregation-0.9.0/data_disaggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:20:49.000000 data-disaggregation-0.9.0/data_disaggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 06:20:49.000000 data-disaggregation-0.9.0/data_disaggregation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 06:20:49.000000 data-disaggregation-0.9.0/data_disaggregation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:20:49.106236 data-disaggregation-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:20:49.106236 data-disaggregation-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-27 06:20:36.000000 data-disaggregation-0.9.0/test/test.py
```

### Comparing `data-disaggregation-0.8.2/LICENSE` & `data-disaggregation-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.8.2/setup.py` & `data-disaggregation-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         packages=["data_disaggregation"],
         name="data-disaggregation",
         install_requires=["pandas"],
         keywords=[],
         description="",
         long_description="",
         long_description_content_type="text/markdown",
-        version="0.8.2",
+        version="0.9.0",
         author="Christian Winger",
         platforms=["any"],
         license="MIT",
         project_urls={
             "Documentation": "https://data-disaggregation.readthedocs.io",
         },
         classifiers=[
```

