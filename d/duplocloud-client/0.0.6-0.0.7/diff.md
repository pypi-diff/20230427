# Comparing `tmp/duplocloud-client-0.0.6.tar.gz` & `tmp/duplocloud-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplocloud-client-0.0.6.tar", last modified: Mon Apr 17 18:36:26 2023, max compression
+gzip compressed data, was "duplocloud-client-0.0.7.tar", last modified: Wed Apr 26 23:16:31 2023, max compression
```

## Comparing `duplocloud-client-0.0.6.tar` & `duplocloud-client-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/src/duplo_resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplo_resource/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.411969 duplocloud-client-0.0.6/src/duplocloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-17 18:35:51.000000 duplocloud-client-0.0.6/src/duplocloud/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:36:26.415969 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 18:36:26.000000 duplocloud-client-0.0.6/src/duplocloud_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/src/duplo_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplo_resource/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.747641 duplocloud-client-0.0.7/src/duplocloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 23:15:43.000000 duplocloud-client-0.0.7/src/duplocloud/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:16:31.751641 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 23:16:31.000000 duplocloud-client-0.0.7/src/duplocloud_client.egg-info/top_level.txt
```

### Comparing `duplocloud-client-0.0.6/.github/workflows/publish.yaml` & `duplocloud-client-0.0.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/.github/workflows/test.yml` & `duplocloud-client-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/CONTRIBUTING.md` & `duplocloud-client-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/PKG-INFO` & `duplocloud-client-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.6/setup.cfg` & `duplocloud-client-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/src/duplo_resource/service.py` & `duplocloud-client-0.0.7/src/duplo_resource/service.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/src/duplo_resource/user.py` & `duplocloud-client-0.0.7/src/duplo_resource/user.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/src/duplocloud/cli.py` & `duplocloud-client-0.0.7/src/duplocloud/cli.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/src/duplocloud/client.py` & `duplocloud-client-0.0.7/src/duplocloud/client.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/src/duplocloud/resource.py` & `duplocloud-client-0.0.7/src/duplocloud/resource.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.6/src/duplocloud_client.egg-info/PKG-INFO` & `duplocloud-client-0.0.7/src/duplocloud_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.6/src/duplocloud_client.egg-info/SOURCES.txt` & `duplocloud-client-0.0.7/src/duplocloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

