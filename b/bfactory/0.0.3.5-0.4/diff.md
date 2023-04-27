# Comparing `tmp/bfactory-0.0.3.5.tar.gz` & `tmp/bfactory-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfactory-0.0.3.5.tar", last modified: Thu Oct  6 04:48:19 2022, max compression
+gzip compressed data, was "bfactory-0.4.tar", last modified: Thu Apr 27 02:45:23 2023, max compression
```

## Comparing `bfactory-0.0.3.5.tar` & `bfactory-0.4.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1063 2022-10-03 05:31:24.000000 bfactory-0.0.3.5/LICENSE
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      545 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/PKG-INFO
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1604 2022-10-03 05:40:11.000000 bfactory-0.0.3.5/README.md
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)       87 2022-10-03 05:07:00.000000 bfactory-0.0.3.5/pyproject.toml
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      856 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/setup.cfg
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/__init__.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/config/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        0 2022-10-03 01:33:49.000000 bfactory-0.0.3.5/src/bfactory/config/__init__.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1255 2022-10-06 04:47:34.000000 bfactory-0.0.3.5/src/bfactory/config/settings.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/core/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/__init__.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     3514 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/engine.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     2126 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/tasks.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/core/templates/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)       85 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/READ.ME
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      570 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/admin.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/core/templates/helpers/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      535 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/helpers/field.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      566 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/helpers/field_serializer.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      594 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/models.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     2759 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/myconf.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      428 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/selectors.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1452 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/services.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      493 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/urls.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1640 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/core/templates/views.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/inputs/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/inputs/__init__.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1504 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/inputs/arguments.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     2570 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/inputs/manifest.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      887 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/inputs/parse_manifest.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1363 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/inputs/validators.py
--rwxr-xr-x   0 blackbox  (1000) blackbox  (1000)     1066 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/main.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/startproject/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        0 2022-08-20 18:51:43.000000 bfactory-0.0.3.5/src/bfactory/startproject/__init__.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      620 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/startproject/startproject.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/tests/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        0 2022-08-20 18:51:43.000000 bfactory-0.0.3.5/src/bfactory/tests/__init__.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      764 2022-10-06 04:46:29.000000 bfactory-0.0.3.5/src/bfactory/tests/engine_tests.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1019 2022-09-19 04:56:43.000000 bfactory-0.0.3.5/src/bfactory/tests/manifest_test.json
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      675 2022-10-06 04:46:34.000000 bfactory-0.0.3.5/src/bfactory/tests/manifest_test.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      932 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/tests/run_tests.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory/utils/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      900 2022-08-20 18:51:43.000000 bfactory-0.0.3.5/src/bfactory/utils/crypto.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     2442 2022-10-06 04:46:22.000000 bfactory-0.0.3.5/src/bfactory/utils/paths.py
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      450 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory/utils/render.py
-drwxr-xr-x   0 blackbox  (1000) blackbox  (1000)        0 2022-10-06 04:48:19.278190 bfactory-0.0.3.5/src/bfactory.egg-info/
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)      545 2022-10-06 04:48:19.000000 bfactory-0.0.3.5/src/bfactory.egg-info/PKG-INFO
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)     1382 2022-10-06 04:48:19.000000 bfactory-0.0.3.5/src/bfactory.egg-info/SOURCES.txt
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        1 2022-10-06 04:48:19.000000 bfactory-0.0.3.5/src/bfactory.egg-info/dependency_links.txt
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)       48 2022-10-06 04:48:19.000000 bfactory-0.0.3.5/src/bfactory.egg-info/entry_points.txt
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)       91 2022-10-06 04:48:19.000000 bfactory-0.0.3.5/src/bfactory.egg-info/requires.txt
--rw-r--r--   0 blackbox  (1000) blackbox  (1000)        9 2022-10-06 04:48:19.000000 bfactory-0.0.3.5/src/bfactory.egg-info/top_level.txt
--rwxr-xr-x   0 blackbox  (1000) blackbox  (1000)      196 2022-10-06 04:01:04.000000 bfactory-0.0.3.5/src/bfactory.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4/LICENSE
+-rw-r--r--   0 blackbox  (1000) users      (985)      541 2023-04-27 02:45:23.808709 bfactory-0.4/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1604 2022-10-03 23:46:43.000000 bfactory-0.4/README.md
+-rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4/pyproject.toml
+-rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-04-27 02:45:23.812043 bfactory-0.4/setup.cfg
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4/src/bfactory/__init__.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/config/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/config/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1251 2023-04-27 02:45:10.000000 bfactory-0.4/src/bfactory/config/settings.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/core/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/core/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     3515 2022-11-10 04:08:56.000000 bfactory-0.4/src/bfactory/core/engine.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2130 2022-11-05 23:27:19.000000 bfactory-0.4/src/bfactory/core/tasks.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/core/templates/
+-rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/core/templates/READ.ME
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-10-04 00:02:46.000000 bfactory-0.4/src/bfactory/core/templates/admin.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/core/templates/helpers/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1179 2022-11-10 03:35:21.000000 bfactory-0.4/src/bfactory/core/templates/helpers/field.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      982 2022-11-10 03:37:52.000000 bfactory-0.4/src/bfactory/core/templates/helpers/field_serializer.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      341 2022-11-06 19:43:09.000000 bfactory-0.4/src/bfactory/core/templates/helpers/field_type_linting.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      624 2022-11-06 04:00:22.000000 bfactory-0.4/src/bfactory/core/templates/models.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4/src/bfactory/core/templates/myconf.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      599 2022-11-06 04:00:13.000000 bfactory-0.4/src/bfactory/core/templates/selectors.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1621 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory/core/templates/services.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4/src/bfactory/core/templates/urls.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     4388 2022-11-10 03:54:52.000000 bfactory-0.4/src/bfactory/core/templates/views.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/inputs/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/inputs/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1550 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory/inputs/arguments.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4/src/bfactory/inputs/manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2698 2022-10-30 07:02:48.000000 bfactory-0.4/src/bfactory/inputs/manifest.schema.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/inputs/parse_manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1363 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/inputs/validators.py
+-rwxr-xr-x   0 blackbox  (1000) users      (985)     1066 2022-10-04 00:33:18.000000 bfactory-0.4/src/bfactory/main.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/startproject/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/startproject/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      620 2022-10-04 00:19:42.000000 bfactory-0.4/src/bfactory/startproject/startproject.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/tests/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/tests/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      743 2022-11-10 04:08:38.000000 bfactory-0.4/src/bfactory/tests/engine_tests.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1022 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory/tests/manifest_test.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      675 2022-10-07 02:36:35.000000 bfactory-0.4/src/bfactory/tests/manifest_test.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      932 2022-10-04 00:31:46.000000 bfactory-0.4/src/bfactory/tests/run_tests.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory/utils/
+-rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4/src/bfactory/utils/crypto.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2442 2022-10-07 02:36:35.000000 bfactory-0.4/src/bfactory/utils/paths.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4/src/bfactory/utils/render.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-27 02:45:23.808709 bfactory-0.4/src/bfactory.egg-info/
+-rw-r--r--   0 blackbox  (1000) users      (985)      541 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1481 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/entry_points.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/requires.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-04-27 02:45:23.000000 bfactory-0.4/src/bfactory.egg-info/top_level.txt
+-rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4/src/bfactory.py
```

### Comparing `bfactory-0.0.3.5/LICENSE` & `bfactory-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/PKG-INFO` & `bfactory-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.0.3.5
+Version: 0.4
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.0.3.5/README.md` & `bfactory-0.4/README.md`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/setup.cfg` & `bfactory-0.4/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 	Documentation = https://github.com/forkear/bfactory/blob/main/README.md
 	Source = https://github.com/forkear/bfactory
 	Tracker = https://github.com/forkear/bfactory/issues
 
 [options]
 python_requires = >=3.8
 install_requires = 
-	Django==4.1
-	djangorestframework==3.13.1
-	djangorestframework-simplejwt==5.2.0
+	Django==4.2
+	djangorestframework==3.14.0
+	djangorestframework-simplejwt==5.2.2
 	Jinja2==3.1.2
 
 [options.entry_points]
 console_scripts = 
 	bfactory = bfactory.main:main
 
 [options.package_data]
```

### Comparing `bfactory-0.0.3.5/src/bfactory/config/settings.py` & `bfactory-0.4/src/bfactory/config/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.0.3.5'
+__version__ = '0.4'
 
 TITLE_BANNER='''\
 
 ██████╗ ███████╗ █████╗  ██████╗████████╗ ██████╗ ██████╗ ██╗   ██╗
 ██╔══██╗██╔════╝██╔══██╗██╔════╝╚══██╔══╝██╔═══██╗██╔══██╗╚██╗ ██╔╝
 ██████╔╝█████╗  ███████║██║        ██║   ██║   ██║██████╔╝ ╚████╔╝ 
 ██╔══██╗██╔══╝  ██╔══██║██║        ██║   ██║   ██║██╔══██╗  ╚██╔╝
```

### Comparing `bfactory-0.0.3.5/src/bfactory/core/engine.py` & `bfactory-0.4/src/bfactory/core/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         path_models = fpaths.path_file_from_app_api('views.py')
 
         render_to_file(template='views.py', file_name=path_models, values=values)
 
 
 
     def _create_urls(self) -> None:
+
         values = {
             'models':self.manifest.get_models(),
         } 
 
         path_models = fpaths.path_file_from_app_api('urls.py')
 
         render_to_file(template='urls.py', file_name=path_models, values=values)
```

### Comparing `bfactory-0.0.3.5/src/bfactory/core/tasks.py` & `bfactory-0.4/src/bfactory/core/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,33 +21,33 @@
         Se encarga de descargar el archivo zip de un proyecto
         base creado en django para nuestra futura api. 
         Luego de descargar el zip lo descomprime en el path dado
         y a continuacion se renombran los directorios y los imports
         para que sea igual que el slug de nuestra api autogenerada
     """
 
-    print("> geting main.zip")
+    print("> descargando main.zip")
     if not path:
         path = fpaths.base_path
 
     resp = urlopen(URL_BASE_BACKEND)
 
     base_path_name = os.path.join(path, slug)
 
-    print("> main.zip in memory ")
+    print("> main.zip en memoria")
 
     zipfile = ZipFile(BytesIO(resp.read()))
 
     zipfile.extractall(path=path)
 
     # eliminamos codigo viejo
     shutil.rmtree(base_path_name, ignore_errors=True)
 
     # renombramos directorios base
-    print("> renombramos directorios ")
+    print("> renombramos directorios")
 
     os.rename('forkear-backend-main/forkear-backend',
               f'forkear-backend-main/{slug}')
     os.rename('forkear-backend-main', f'{slug}')
 
     print("> refactorizamos el codigo base ")
```

### Comparing `bfactory-0.0.3.5/src/bfactory/core/templates/admin.py` & `bfactory-0.4/src/bfactory/core/templates/admin.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/core/templates/models.py` & `bfactory-0.4/src/bfactory/core/templates/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 from django.db import models
 from django.contrib.auth.models import User
+from datetime import datetime
 
 {% for model in models %}
 class {{model.name}}(models.Model):
 
 {% for field in model.fields -%}
 {{ '    ' }}{{field.name}} = {% include "helpers/field.py" %}
 {%- endfor %}
```

### Comparing `bfactory-0.0.3.5/src/bfactory/core/templates/myconf.py` & `bfactory-0.4/src/bfactory/core/templates/myconf.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/core/templates/services.py` & `bfactory-0.4/src/bfactory/core/templates/services.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 
-from  django.db import models
+from django.db import models
 from django.contrib.auth.models import User
 from django.db import transaction
+from datetime import datetime
 
 {% for model in models %}from .models import {{model.name}}
 {% endfor %}
 
 {% for model in models %}
 class {{model.name}}Service:
     
     def __init__(self, user: User = None):
         self._user = user
     
     @transaction.atomic
     def create(
-        self,{% for field in model.fields %}
-        {{field.name}}: {{field.type}},{%endfor%}
+        self,{%- for field in model.fields if field.editable  %}
+        {{field.name}}: {%- include "helpers/field_type_linting.py" -%},{%endfor -%}
     ) -> {{model.name}}:
 
-        {{model.name|lower}} = {{model.name}}({% for field in model.fields %}
+        {{model.name|lower}} = {{model.name}}({% for field in model.fields if field.editable %}
                 {{field.name}}={{field.name}},
                 {%- endfor%}
         )
 
         {{model.name|lower}}.full_clean()
         {{model.name|lower}}.save()
 
         return {{model.name|lower}}
 
     @transaction.atomic
     def update(
         self,
-        {{model.name|lower}}: {{model.name}}, {% for field in model.fields %}
-        {{field.name}}: {{field.type}},{%endfor%}
+        {{model.name|lower}}: {{model.name}}, {% for field in model.fields if field.editable %}
+        {{field.name}}: {% include "helpers/field_type_linting.py" %},{%endfor%}
     ) -> {{model.name}}:
-        {% for field in model.fields %}
+        {% for field in model.fields if field.editable %}
         {{model.name|lower}}.{{field.name}}={{field.name}}{%endfor%}
         
         {{model.name|lower}}.full_clean()
         {{model.name|lower}}.save()
         return {{model.name|lower}}
```

### Comparing `bfactory-0.0.3.5/src/bfactory/inputs/arguments.py` & `bfactory-0.4/src/bfactory/inputs/arguments.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             exit(1)
         setattr(namespace, self.dest, values)
 
 
 parser = argparse.ArgumentParser(
     prog='bfactory',
     formatter_class=argparse.RawDescriptionHelpFormatter,
-    description=textwrap.dedent(TITLE_BANNER),
-    epilog='Gracias a Django',
+    #description=textwrap.dedent(TITLE_BANNER),
+    epilog='thx to:\n\tPython\n\tDjango\n\tJinja\n\tDjango REST framework',
 )
 
 
 parser.add_argument(
     'test',
     nargs='?',
     help='Ejecutar test de unidad',
```

### Comparing `bfactory-0.0.3.5/src/bfactory/inputs/manifest.py` & `bfactory-0.4/src/bfactory/inputs/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 class Field():
 
     def __init__(self, obj:Dict):
 
         self.name = obj['name']
         self.type = obj['type']
-        self.req = obj['req']
-        if 'default' in obj:
-            self.default = obj['default']
-        if 'fk' in obj:
-            self.fk = obj['fk']
-        else:
-            self.default = None
+        self.req  = obj['req']
+        self.default = obj.get('default',None)
+        self.fk = obj.get('fk', None)
+        self.editable = obj.get('editable', True)
+
     
     def __str__(self) -> str:
         return f"{self.name} - {self.type}"  
 
 
 
 class Model():
```

### Comparing `bfactory-0.0.3.5/src/bfactory/inputs/parse_manifest.py` & `bfactory-0.4/src/bfactory/inputs/parse_manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/inputs/validators.py` & `bfactory-0.4/src/bfactory/inputs/validators.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/main.py` & `bfactory-0.4/src/bfactory/main.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/startproject/startproject.py` & `bfactory-0.4/src/bfactory/startproject/startproject.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/tests/manifest_test.json` & `bfactory-0.4/src/bfactory/tests/manifest_test.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'schema'": "{0: {'attrs': {2: {'name': 'usuario', 'type': 'owner'}}}}"}*

```diff
@@ -22,17 +22,17 @@
                     "default": false,
                     "name": "realizada",
                     "req": false,
                     "type": "bool"
                 },
                 {
                     "default": "",
-                    "name": "owner",
+                    "name": "usuario",
                     "req": true,
-                    "type": "User"
+                    "type": "owner"
                 }
             ],
             "name": "Tarea",
             "perm": "700"
         }
     ],
     "version": "1"
```

### Comparing `bfactory-0.0.3.5/src/bfactory/tests/manifest_test.py` & `bfactory-0.4/src/bfactory/tests/manifest_test.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/tests/run_tests.py` & `bfactory-0.4/src/bfactory/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/utils/crypto.py` & `bfactory-0.4/src/bfactory/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory/utils/paths.py` & `bfactory-0.4/src/bfactory/utils/paths.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.0.3.5/src/bfactory.egg-info/PKG-INFO` & `bfactory-0.4/src/bfactory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.0.3.5
+Version: 0.4
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.0.3.5/src/bfactory.egg-info/SOURCES.txt` & `bfactory-0.4/src/bfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 src/bfactory/core/templates/myconf.py
 src/bfactory/core/templates/selectors.py
 src/bfactory/core/templates/services.py
 src/bfactory/core/templates/urls.py
 src/bfactory/core/templates/views.py
 src/bfactory/core/templates/helpers/field.py
 src/bfactory/core/templates/helpers/field_serializer.py
+src/bfactory/core/templates/helpers/field_type_linting.py
 src/bfactory/inputs/__init__.py
 src/bfactory/inputs/arguments.py
 src/bfactory/inputs/manifest.py
+src/bfactory/inputs/manifest.schema.json
 src/bfactory/inputs/parse_manifest.py
 src/bfactory/inputs/validators.py
 src/bfactory/startproject/__init__.py
 src/bfactory/startproject/startproject.py
 src/bfactory/tests/__init__.py
 src/bfactory/tests/engine_tests.py
 src/bfactory/tests/manifest_test.json
```

