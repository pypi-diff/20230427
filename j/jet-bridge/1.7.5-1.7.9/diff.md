# Comparing `tmp/jet-bridge-1.7.5.tar.gz` & `tmp/jet-bridge-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jet-bridge-1.7.5.tar", last modified: Thu Feb 23 16:23:53 2023, max compression
+gzip compressed data, was "dist/jet-bridge-1.7.9.tar", last modified: Thu Mar 16 07:39:18 2023, max compression
```

## Comparing `jet-bridge-1.7.5.tar` & `jet-bridge-1.7.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/
--rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)     1099 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/LICENSE
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/
--rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:48:56.000000 jet-bridge-1.7.5/jet_bridge.egg-info/not-zip-safe
--rw-r--r--   0 f1nal      (501) staff       (20)     1431 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       57 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/entry_points.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       68 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/requires.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/top_level.txt
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge.egg-info/dependency_links.txt
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/
--rw-r--r--   0 f1nal      (501) staff       (20)     5863 2023-02-14 16:01:58.000000 jet-bridge-1.7.5/jet_bridge/configuration.py
--rw-r--r--   0 f1nal      (501) staff       (20)       28 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/media.py
--rw-r--r--   0 f1nal      (501) staff       (20)       18 2023-02-23 13:44:39.000000 jet-bridge-1.7.5/jet_bridge/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)   229376 2022-11-24 06:42:37.000000 jet-bridge-1.7.5/jet_bridge/jet_bridge_store.db
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/utils/
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/utils/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/utils/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     1593 2021-08-31 19:06:46.000000 jet-bridge-1.7.5/jet_bridge/utils/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6817 2021-11-08 16:38:24.000000 jet-bridge-1.7.5/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      174 2021-08-31 19:06:46.000000 jet-bridge-1.7.5/jet_bridge/utils/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1948 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/utils/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)    13378 2023-02-14 16:01:58.000000 jet-bridge-1.7.5/jet_bridge/utils/create_config.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     3595 2023-02-16 15:32:25.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/app.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-31 19:06:46.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/media.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3205 2022-06-08 13:55:47.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/router.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5121 2023-02-16 15:32:23.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5369 2023-02-16 15:32:23.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/configuration.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      185 2023-02-23 13:44:39.000000 jet-bridge-1.7.5/jet_bridge/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     6365 2023-02-14 16:01:58.000000 jet-bridge-1.7.5/jet_bridge/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3874 2023-02-14 16:01:58.000000 jet-bridge-1.7.5/jet_bridge/app.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/commands/
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/commands/__init__.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2896 2022-06-08 13:55:45.000000 jet-bridge-1.7.5/jet_bridge/router.py
--rw-r--r--   0 f1nal      (501) staff       (20)     2299 2023-02-14 16:01:58.000000 jet-bridge-1.7.5/jet_bridge/__main__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/handlers/
--rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/handlers/temporary_redirect.py
--rw-r--r--   0 f1nal      (501) staff       (20)      224 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/handlers/not_found.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/jet_bridge/handlers/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)      611 2021-08-31 19:07:59.000000 jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     5704 2023-02-16 15:32:26.000000 jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/view.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      613 2021-08-31 19:08:00.000000 jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      177 2021-08-31 19:07:59.000000 jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     4644 2023-02-14 16:01:58.000000 jet-bridge-1.7.5/jet_bridge/handlers/view.py
--rw-r--r--   0 f1nal      (501) staff       (20)   106496 2023-02-22 06:44:49.000000 jet-bridge-1.7.5/jet_bridge/jet_bridge_store.sqlite3
--rw-r--r--   0 f1nal      (501) staff       (20)       65 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/MANIFEST.in
--rw-r--r--   0 f1nal      (501) staff       (20)    10270 2021-08-25 15:07:30.000000 jet-bridge-1.7.5/README.md
--rw-r--r--   0 f1nal      (501) staff       (20)     1069 2023-02-23 13:44:39.000000 jet-bridge-1.7.5/setup.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-02-23 16:23:53.000000 jet-bridge-1.7.5/setup.cfg
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/
+-rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)     1099 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/LICENSE
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/
+-rw-r--r--   0 f1nal      (501) staff       (20)    10546 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:48:56.000000 jet-bridge-1.7.9/jet_bridge.egg-info/not-zip-safe
+-rw-r--r--   0 f1nal      (501) staff       (20)     1431 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       57 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       68 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/requires.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/top_level.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge.egg-info/dependency_links.txt
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/
+-rw-r--r--   0 f1nal      (501) staff       (20)     5863 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/configuration.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       28 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/media.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       18 2023-03-16 02:56:11.000000 jet-bridge-1.7.9/jet_bridge/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)   229376 2022-11-24 06:42:37.000000 jet-bridge-1.7.9/jet_bridge/jet_bridge_store.db
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/utils/
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/utils/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     1593 2021-08-31 19:06:46.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6817 2021-11-08 16:38:24.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      174 2021-08-31 19:06:46.000000 jet-bridge-1.7.9/jet_bridge/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1948 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/utils/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)    13378 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/utils/create_config.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3595 2023-02-16 15:32:25.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/app.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-31 19:06:46.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/media.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3205 2022-06-08 13:55:47.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/router.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5121 2023-02-16 15:32:23.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5369 2023-02-16 15:32:23.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/configuration.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      185 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     6365 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3874 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/app.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/commands/
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/commands/__init__.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2896 2022-06-08 13:55:45.000000 jet-bridge-1.7.9/jet_bridge/router.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     2299 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/__main__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/handlers/
+-rw-r--r--   0 f1nal      (501) staff       (20)      192 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/handlers/temporary_redirect.py
+-rw-r--r--   0 f1nal      (501) staff       (20)      224 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/handlers/not_found.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/jet_bridge/handlers/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)      611 2021-08-31 19:07:59.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     5704 2023-02-16 15:32:26.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/view.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      613 2021-08-31 19:08:00.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      177 2021-08-31 19:07:59.000000 jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     4644 2023-02-14 16:01:58.000000 jet-bridge-1.7.9/jet_bridge/handlers/view.py
+-rw-r--r--   0 f1nal      (501) staff       (20)   106496 2023-02-22 06:44:49.000000 jet-bridge-1.7.9/jet_bridge/jet_bridge_store.sqlite3
+-rw-r--r--   0 f1nal      (501) staff       (20)       65 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/MANIFEST.in
+-rw-r--r--   0 f1nal      (501) staff       (20)    10270 2021-08-25 15:07:30.000000 jet-bridge-1.7.9/README.md
+-rw-r--r--   0 f1nal      (501) staff       (20)     1069 2023-03-16 02:56:11.000000 jet-bridge-1.7.9/setup.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-03-16 07:39:18.000000 jet-bridge-1.7.9/setup.cfg
```

### Comparing `jet-bridge-1.7.5/PKG-INFO` & `jet-bridge-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-bridge
-Version: 1.7.5
+Version: 1.7.9
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-bridge
 Author: Denis Kildishev
 Author-email: support@jetadmin.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jet-bridge-1.7.5/LICENSE` & `jet-bridge-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge.egg-info/PKG-INFO` & `jet-bridge-1.7.9/jet_bridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-bridge
-Version: 1.7.5
+Version: 1.7.9
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-bridge
 Author: Denis Kildishev
 Author-email: support@jetadmin.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jet-bridge-1.7.5/jet_bridge.egg-info/SOURCES.txt` & `jet-bridge-1.7.9/jet_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/configuration.py` & `jet-bridge-1.7.9/jet_bridge/configuration.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/jet_bridge_store.db` & `jet-bridge-1.7.9/jet_bridge/jet_bridge_store.db`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/utils/__pycache__/settings.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/utils/__pycache__/settings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/utils/__pycache__/create_config.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/utils/settings.py` & `jet-bridge-1.7.9/jet_bridge/utils/settings.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/utils/create_config.py` & `jet-bridge-1.7.9/jet_bridge/utils/create_config.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/__pycache__/app.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/__pycache__/app.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/__pycache__/router.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/__pycache__/router.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/__pycache__/settings.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/__pycache__/settings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/__pycache__/configuration.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/__pycache__/configuration.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/settings.py` & `jet-bridge-1.7.9/jet_bridge/settings.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/app.py` & `jet-bridge-1.7.9/jet_bridge/app.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/router.py` & `jet-bridge-1.7.9/jet_bridge/router.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/__main__.py` & `jet-bridge-1.7.9/jet_bridge/__main__.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/temporary_redirect.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/view.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/view.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc` & `jet-bridge-1.7.9/jet_bridge/handlers/__pycache__/not_found.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/handlers/view.py` & `jet-bridge-1.7.9/jet_bridge/handlers/view.py`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/jet_bridge/jet_bridge_store.sqlite3` & `jet-bridge-1.7.9/jet_bridge/jet_bridge_store.sqlite3`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/README.md` & `jet-bridge-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `jet-bridge-1.7.5/setup.py` & `jet-bridge-1.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return file.read()
 
 
 def get_install_requires():
     install_requires = [
         'tornado==5.1.1',
         'six',
-        'jet-bridge-base==1.7.5',
+        'jet-bridge-base==1.7.9',
         'paramiko==2.8.1',
         'sshtunnel',
     ]
 
     return install_requires
 
 setup(
```

