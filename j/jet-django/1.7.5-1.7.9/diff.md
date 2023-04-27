# Comparing `tmp/jet-django-1.7.5.tar.gz` & `tmp/jet-django-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jet-django-1.7.5.tar", last modified: Thu Feb 23 16:24:18 2023, max compression
+gzip compressed data, was "dist/jet-django-1.7.9.tar", last modified: Thu Mar 16 07:39:33 2023, max compression
```

## Comparing `jet-django-1.7.5.tar` & `jet-django-1.7.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:24:18.000000 jet-django-1.7.5/
--rw-r--r--   0 f1nal      (501) staff       (20)     3925 2023-02-23 16:24:18.000000 jet-django-1.7.5/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-django-1.7.5/LICENSE
--rw-r--r--   0 f1nal      (501) staff       (20)       66 2021-08-25 15:07:30.000000 jet-django-1.7.5/MANIFEST.in
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:24:18.000000 jet-django-1.7.5/jet_django.egg-info/
--rw-r--r--   0 f1nal      (501) staff       (20)     3925 2023-02-23 16:24:17.000000 jet-django-1.7.5/jet_django.egg-info/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:49:12.000000 jet-django-1.7.5/jet_django.egg-info/not-zip-safe
--rw-r--r--   0 f1nal      (501) staff       (20)     1219 2023-02-23 16:24:17.000000 jet-django-1.7.5/jet_django.egg-info/SOURCES.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       39 2023-02-23 16:24:17.000000 jet-django-1.7.5/jet_django.egg-info/requires.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-02-23 16:24:17.000000 jet-django-1.7.5/jet_django.egg-info/top_level.txt
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-02-23 16:24:17.000000 jet-django-1.7.5/jet_django.egg-info/dependency_links.txt
--rw-r--r--   0 f1nal      (501) staff       (20)      973 2023-02-23 13:44:39.000000 jet-django-1.7.5/setup.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-02-23 16:24:18.000000 jet-django-1.7.5/setup.cfg
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:24:18.000000 jet-django-1.7.5/jet_django/
--rw-r--r--   0 f1nal      (501) staff       (20)    13442 2023-02-14 16:01:58.000000 jet-django-1.7.5/jet_django/configuration.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:24:18.000000 jet-django-1.7.5/jet_django/migrations/
--rw-r--r--   0 f1nal      (501) staff       (20)      761 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/0002_auto_20181014_2002.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:24:18.000000 jet-django-1.7.5/jet_django/migrations/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     2338 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      789 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1432 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1218 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/0003_auto_20191007_2005.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5152 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/migrations/0001_initial.py
--rw-r--r--   0 f1nal      (501) staff       (20)       73 2023-02-23 13:44:39.000000 jet-django-1.7.5/jet_django/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-02-23 16:24:18.000000 jet-django-1.7.5/jet_django/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     5807 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/__pycache__/route_view.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2359 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2941 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    13595 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/__pycache__/configuration.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      244 2023-02-23 16:24:17.000000 jet-django-1.7.5/jet_django/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3329 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/__pycache__/router.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1080 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      254 2022-11-13 04:37:35.000000 jet-django-1.7.5/jet_django/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 04:35:29.000000 jet-django-1.7.5/jet_django/apps.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3480 2023-02-14 16:01:58.000000 jet-django-1.7.5/jet_django/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4989 2023-02-14 16:01:58.000000 jet-django-1.7.5/jet_django/route_view.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3446 2023-02-14 16:01:58.000000 jet-django-1.7.5/jet_django/router.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4845 2023-02-14 16:01:58.000000 jet-django-1.7.5/jet_django/urls.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3689 2021-08-25 15:07:30.000000 jet-django-1.7.5/README.rst
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3925 2023-03-16 07:39:33.000000 jet-django-1.7.9/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-django-1.7.9/LICENSE
+-rw-r--r--   0 f1nal      (501) staff       (20)       66 2021-08-25 15:07:30.000000 jet-django-1.7.9/MANIFEST.in
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3925 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:49:12.000000 jet-django-1.7.9/jet_django.egg-info/not-zip-safe
+-rw-r--r--   0 f1nal      (501) staff       (20)     1219 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/SOURCES.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       39 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/requires.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/top_level.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/dependency_links.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)      973 2023-03-16 02:56:11.000000 jet-django-1.7.9/setup.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-03-16 07:39:33.000000 jet-django-1.7.9/setup.cfg
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/
+-rw-r--r--   0 f1nal      (501) staff       (20)    13442 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/configuration.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/migrations/
+-rw-r--r--   0 f1nal      (501) staff       (20)      761 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/0002_auto_20181014_2002.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     2338 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      789 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1432 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1218 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/0003_auto_20191007_2005.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     5152 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/0001_initial.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       73 2023-03-16 02:56:11.000000 jet-django-1.7.9/jet_django/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     5807 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/route_view.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2359 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2941 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    13595 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/configuration.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      244 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3329 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/router.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1080 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      254 2022-11-13 04:37:35.000000 jet-django-1.7.9/jet_django/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/apps.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3480 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4989 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/route_view.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3446 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/router.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4845 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/urls.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3689 2021-08-25 15:07:30.000000 jet-django-1.7.9/README.rst
```

### Comparing `jet-django-1.7.5/PKG-INFO` & `jet-django-1.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-django
-Version: 1.7.5
+Version: 1.7.9
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-django
 Author: Denis Kildishev
 Author-email: hello@geex-arts.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `jet-django-1.7.5/jet_django.egg-info/PKG-INFO` & `jet-django-1.7.9/jet_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-django
-Version: 1.7.5
+Version: 1.7.9
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-django
 Author: Denis Kildishev
 Author-email: hello@geex-arts.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `jet-django-1.7.5/jet_django.egg-info/SOURCES.txt` & `jet-django-1.7.9/jet_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/setup.py` & `jet-django-1.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return file.read()
 
 
 def get_install_requires():
     install_requires = [
         'Django',
         'requests',
-        'jet-bridge-base==1.7.5',
+        'jet-bridge-base==1.7.9',
     ]
 
     try:
         from collections import OrderedDict
     except ImportError:
         install_requires.append('ordereddict')
```

### Comparing `jet-django-1.7.5/jet_django/configuration.py` & `jet-django-1.7.9/jet_django/configuration.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/migrations/0002_auto_20181014_2002.py` & `jet-django-1.7.9/jet_django/migrations/0002_auto_20181014_2002.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc` & `jet-django-1.7.9/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc` & `jet-django-1.7.9/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc` & `jet-django-1.7.9/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/migrations/0003_auto_20191007_2005.py` & `jet-django-1.7.9/jet_django/migrations/0003_auto_20191007_2005.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/migrations/0001_initial.py` & `jet-django-1.7.9/jet_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/__pycache__/route_view.cpython-310.pyc` & `jet-django-1.7.9/jet_django/__pycache__/route_view.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/__pycache__/settings.cpython-310.pyc` & `jet-django-1.7.9/jet_django/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/__pycache__/urls.cpython-310.pyc` & `jet-django-1.7.9/jet_django/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/__pycache__/configuration.cpython-310.pyc` & `jet-django-1.7.9/jet_django/__pycache__/configuration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/__pycache__/router.cpython-310.pyc` & `jet-django-1.7.9/jet_django/__pycache__/router.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/__pycache__/apps.cpython-310.pyc` & `jet-django-1.7.9/jet_django/__pycache__/apps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/apps.py` & `jet-django-1.7.9/jet_django/apps.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/settings.py` & `jet-django-1.7.9/jet_django/settings.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/route_view.py` & `jet-django-1.7.9/jet_django/route_view.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/router.py` & `jet-django-1.7.9/jet_django/router.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/jet_django/urls.py` & `jet-django-1.7.9/jet_django/urls.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.5/README.rst` & `jet-django-1.7.9/README.rst`

 * *Files identical despite different names*

