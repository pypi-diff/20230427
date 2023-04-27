# Comparing `tmp/base_system-0.1.3.tar.gz` & `tmp/base_system-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.1.3.tar", last modified: Thu Apr 27 03:40:58 2023, max compression
+gzip compressed data, was "base_system-0.1.4.tar", last modified: Thu Apr 27 07:41:10 2023, max compression
```

## Comparing `base_system-0.1.3.tar` & `base_system-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.449387 base_system-0.1.3/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.3/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.3/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.433326 base_system-0.1.3/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.3/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.3/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11870 2023-04-27 02:20:00.000000 base_system-0.1.3/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.1.3/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.3/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.3/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.3/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.3/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1192 2023-04-27 03:40:58.449387 base_system-0.1.3/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.1.3/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.445372 base_system-0.1.3/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.1.3/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.449387 base_system-0.1.3/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.1.3/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.1.3/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.1.3/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19403 2023-04-27 03:37:46.000000 base_system-0.1.3/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.1.3/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.1.3/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.1.3/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    32530 2023-04-27 02:23:46.000000 base_system-0.1.3/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11937 2023-04-27 02:23:47.000000 base_system-0.1.3/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.1.3/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.1.3/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.1.3/base_system/auth.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.449387 base_system-0.1.3/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    38650 2023-04-27 03:38:07.000000 base_system-0.1.3/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.1.3/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.449387 base_system-0.1.3/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.1.3/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25401 2023-04-27 03:37:37.000000 base_system-0.1.3/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.1.3/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.1.3/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.1.3/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    71863 2023-04-27 02:23:42.000000 base_system-0.1.3/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14977 2023-04-25 05:48:42.000000 base_system-0.1.3/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 03:40:58.445372 base_system-0.1.3/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1192 2023-04-27 03:40:58.000000 base_system-0.1.3/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1243 2023-04-27 03:40:58.000000 base_system-0.1.3/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:40:58.000000 base_system-0.1.3/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:06:19.000000 base_system-0.1.3/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       82 2023-04-27 03:40:58.000000 base_system-0.1.3/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-04-27 03:40:58.000000 base_system-0.1.3/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.3/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.1.3/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.3/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.1.3/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-04-27 03:40:58.449387 base_system-0.1.3/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2629 2023-04-27 03:40:36.000000 base_system-0.1.3/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.442585 base_system-0.1.4/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.4/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.4/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.402424 base_system-0.1.4/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.4/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.4/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11870 2023-04-27 02:20:00.000000 base_system-0.1.4/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.1.4/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.4/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.4/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.4/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.4/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-04-27 07:41:10.438569 base_system-0.1.4/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.1.4/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.418489 base_system-0.1.4/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.1.4/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.434553 base_system-0.1.4/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.1.4/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.1.4/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.1.4/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19403 2023-04-27 03:37:46.000000 base_system-0.1.4/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.1.4/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.1.4/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.1.4/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    32530 2023-04-27 02:23:46.000000 base_system-0.1.4/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11937 2023-04-27 02:23:47.000000 base_system-0.1.4/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.1.4/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.1.4/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.1.4/base_system/auth.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.434553 base_system-0.1.4/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39508 2023-04-27 07:36:54.000000 base_system-0.1.4/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.1.4/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.434553 base_system-0.1.4/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.1.4/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25401 2023-04-27 03:37:37.000000 base_system-0.1.4/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.1.4/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.1.4/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.1.4/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    71863 2023-04-27 02:23:42.000000 base_system-0.1.4/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14977 2023-04-25 05:48:42.000000 base_system-0.1.4/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 07:41:10.426521 base_system-0.1.4/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-04-27 07:41:10.000000 base_system-0.1.4/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1243 2023-04-27 07:41:10.000000 base_system-0.1.4/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 07:41:10.000000 base_system-0.1.4/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:06:19.000000 base_system-0.1.4/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       82 2023-04-27 07:41:10.000000 base_system-0.1.4/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-04-27 07:41:10.000000 base_system-0.1.4/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.4/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.1.4/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.4/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.1.4/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-04-27 07:41:10.442585 base_system-0.1.4/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2602 2023-04-27 07:39:38.000000 base_system-0.1.4/setup.py
```

### Comparing `base_system-0.1.3/.gitignore` & `base_system-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/BaseFunctionModule/settings.py` & `base_system-0.1.4/BaseFunctionModule/settings.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/BaseFunctionModule/urls.py` & `base_system-0.1.4/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/LICENCE` & `base_system-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/PKG-INFO` & `base_system-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.1.3
+Version: 0.1.4
 Summary: Basic feature component
-Home-page: https://devcloud.huaweicloud.com/
+Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `base_system-0.1.3/README.rst` & `base_system-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.1.4/base_system/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.1.4/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.1.4/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.1.4/base_system/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.1.4/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/auth.py` & `base_system-0.1.4/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/migrations/0001_initial.py` & `base_system-0.1.4/base_system/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -485,14 +485,19 @@
             options={
                 'verbose_name': '用户信息',
             },
             managers=[
                 ('objects', django.contrib.auth.models.UserManager()),
             ],
         ),
+        migrations.RunSQL(
+            """
+            INSERT INTO "base_system_user"("id", "username", "first_name", "last_name", "email", "is_staff", "is_active", "date_joined", "name", "password", "last_login", "is_superuser", "phone", "birthday", "gender", "idcardnum", "order_by", "avatar_url", "default_group_id", "allow_office", "note", "created_by", "created_time", "updated_time", "hospital_id", "office_id", "user_rank_id", "updated_by", "doctor_id") VALUES (1, 'admin', '', '', 'admin@admin.com', 't', 't', '2023-02-13 10:22:39+08', '管理员', 'pbkdf2_sha256$260000$eR3ouH02QKSmOTLN0Y2vsL$rx5zmoAR0PgQ2fB6l5gKLCvLPxkw2NtBsTDXQO7iIT8=', '2022-09-08', 't', NULL, NULL, NULL, NULL, 1, 'user_avatar', NULL, NULL, NULL, NULL, '2022-09-08 16:32:24.192312+08', '2023-03-23 09:54:21.211661+08', NULL, NULL, NULL, NULL, NULL);
+            """
+        ),
         migrations.CreateModel(
             name='ExpenseStandard',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_time', models.DateTimeField(auto_now_add=True, null=True, verbose_name='创建时间')),
                 ('updated_time', models.DateTimeField(auto_now=True, null=True, verbose_name='更新时间')),
                 ('is_active', models.BooleanField(default=True, verbose_name='是否启用')),
```

### Comparing `base_system-0.1.3/base_system/models.py` & `base_system-0.1.4/base_system/models.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/serializers.py` & `base_system-0.1.4/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/urls.py` & `base_system-0.1.4/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/views.py` & `base_system-0.1.4/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system/viewsets.py` & `base_system-0.1.4/base_system/viewsets.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/base_system.egg-info/PKG-INFO` & `base_system-0.1.4/base_system.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.1.3
+Version: 0.1.4
 Summary: Basic feature component
-Home-page: https://devcloud.huaweicloud.com/
+Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `base_system-0.1.3/base_system.egg-info/SOURCES.txt` & `base_system-0.1.4/base_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/init_data.json` & `base_system-0.1.4/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/manage.py` & `base_system-0.1.4/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/requirements.txt` & `base_system-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/runtests.py` & `base_system-0.1.4/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.3/setup.py` & `base_system-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.1.3',
+    version='0.1.4',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
-    url="https://devcloud.huaweicloud.com/",
+    url="https://github.com/zcjwin",
     include_package_data=True,
-    packages=find_packages(include=('base_system', 'work_scheduling',)),
+    packages=find_packages(include=('base_system',)),
     zip_safe=False,
     install_requires=[
         'Django>=2.0',
         'djangorestframework>=3.7.0',
         'xlrd2>=1.3.4',
         'pyDes>=2.0.1',
         'drf-excel>=2.1.0',
```

