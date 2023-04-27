# Comparing `tmp/django-datadog-logger-0.5.6.tar.gz` & `tmp/django-datadog-logger-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-datadog-logger-0.5.6.tar", last modified: Tue Jan 17 14:36:16 2023, max compression
+gzip compressed data, was "django-datadog-logger-0.6.1.tar", last modified: Thu Apr 27 15:00:21 2023, max compression
```

## Comparing `django-datadog-logger-0.5.6.tar` & `django-datadog-logger-0.6.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.812156 django-datadog-logger-0.5.6/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      155 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/AUTHORS.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     3699 2020-11-27 12:01:54.000000 django-datadog-logger-0.5.6/CONTRIBUTING.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1662 2023-01-16 20:40:29.000000 django-datadog-logger-0.5.6/HISTORY.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1070 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/LICENSE
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      287 2020-11-27 12:01:54.000000 django-datadog-logger-0.5.6/MANIFEST.in
--rw-rw-r--   0 lenno     (1000) lenno     (1000)    10770 2023-01-17 14:36:16.812156 django-datadog-logger-0.5.6/PKG-INFO
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     8345 2021-08-27 08:13:56.000000 django-datadog-logger-0.5.6/README.rst
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.804156 django-datadog-logger-0.5.6/django_datadog_logger/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-01-17 14:36:08.000000 django-datadog-logger-0.5.6/django_datadog_logger/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      964 2021-10-20 08:11:50.000000 django-datadog-logger-0.5.6/django_datadog_logger/celery.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      258 2019-12-16 08:08:58.000000 django-datadog-logger-0.5.6/django_datadog_logger/encoders.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.808156 django-datadog-logger-0.5.6/django_datadog_logger/formatters/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.5.6/django_datadog_logger/formatters/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     8459 2023-01-17 14:34:58.000000 django-datadog-logger-0.5.6/django_datadog_logger/formatters/datadog.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1608 2021-06-14 11:05:07.000000 django-datadog-logger-0.5.6/django_datadog_logger/local.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.808156 django-datadog-logger-0.5.6/django_datadog_logger/middleware/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.5.6/django_datadog_logger/middleware/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      412 2019-12-16 08:08:58.000000 django-datadog-logger-0.5.6/django_datadog_logger/middleware/error_log.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      879 2020-11-04 07:40:11.000000 django-datadog-logger-0.5.6/django_datadog_logger/middleware/request_id.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1861 2020-11-04 07:42:19.000000 django-datadog-logger-0.5.6/django_datadog_logger/middleware/request_log.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      481 2021-06-14 11:41:52.000000 django-datadog-logger-0.5.6/django_datadog_logger/recursion.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.808156 django-datadog-logger-0.5.6/django_datadog_logger/rest_framework/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.5.6/django_datadog_logger/rest_framework/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     2395 2022-08-09 10:34:11.000000 django-datadog-logger-0.5.6/django_datadog_logger/rest_framework/mixins.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      224 2021-06-14 11:05:07.000000 django-datadog-logger-0.5.6/django_datadog_logger/wsgi.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.808156 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)    10770 2023-01-17 14:36:16.000000 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/PKG-INFO
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1176 2023-01-17 14:36:16.000000 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2023-01-17 14:36:16.000000 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2020-02-17 12:25:46.000000 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/not-zip-safe
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       58 2023-01-17 14:36:16.000000 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/requires.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-01-17 14:36:16.000000 django-datadog-logger-0.5.6/django_datadog_logger.egg-info/top_level.txt
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.812156 django-datadog-logger-0.5.6/docs/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      622 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/Makefile
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/authors.rst
--rwxrwxr-x   0 lenno     (1000) lenno     (1000)     4957 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/conf.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       33 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/contributing.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/history.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      318 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/index.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1242 2020-02-17 11:49:32.000000 django-datadog-logger-0.5.6/docs/installation.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      783 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/make.bat
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       27 2020-11-27 12:01:54.000000 django-datadog-logger-0.5.6/docs/readme.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       97 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/docs/usage.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      139 2020-02-17 12:15:03.000000 django-datadog-logger-0.5.6/pyproject.toml
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       58 2020-04-15 06:33:05.000000 django-datadog-logger-0.5.6/requirements.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      404 2023-01-17 14:36:16.812156 django-datadog-logger-0.5.6/setup.cfg
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1731 2023-01-17 14:36:08.000000 django-datadog-logger-0.5.6/setup.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-01-17 14:36:16.812156 django-datadog-logger-0.5.6/tests/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       51 2020-02-17 11:36:11.000000 django-datadog-logger-0.5.6/tests/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      437 2020-02-17 11:54:33.000000 django-datadog-logger-0.5.6/tests/test_django_datadog_logger.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      155 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/AUTHORS.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     3699 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.1/CONTRIBUTING.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1965 2023-04-27 14:59:53.000000 django-datadog-logger-0.6.1/HISTORY.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1070 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/LICENSE
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      287 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.1/MANIFEST.in
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)    11053 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/PKG-INFO
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     8345 2021-08-27 08:13:56.000000 django-datadog-logger-0.6.1/README.rst
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-04-27 15:00:05.000000 django-datadog-logger-0.6.1/django_datadog_logger/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1001 2023-04-27 14:57:10.000000 django-datadog-logger-0.6.1/django_datadog_logger/celery.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      258 2019-12-16 08:08:58.000000 django-datadog-logger-0.6.1/django_datadog_logger/encoders.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/formatters/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.1/django_datadog_logger/formatters/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     7874 2023-04-27 14:22:11.000000 django-datadog-logger-0.6.1/django_datadog_logger/formatters/datadog.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1608 2021-06-14 11:05:07.000000 django-datadog-logger-0.6.1/django_datadog_logger/local.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/middleware/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      412 2019-12-16 08:08:58.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/error_log.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      879 2020-11-04 07:40:11.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_id.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1861 2020-11-04 07:42:19.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_log.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      481 2021-06-14 11:41:52.000000 django-datadog-logger-0.6.1/django_datadog_logger/recursion.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     2395 2022-08-09 10:34:11.000000 django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/mixins.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      224 2021-06-14 11:05:07.000000 django-datadog-logger-0.6.1/django_datadog_logger/wsgi.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)    11053 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1176 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2020-02-17 12:25:46.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/not-zip-safe
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       46 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/requires.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/top_level.txt
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/docs/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      622 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/Makefile
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/authors.rst
+-rwxrwxr-x   0 lenno     (1000) lenno     (1000)     4964 2023-04-27 14:32:31.000000 django-datadog-logger-0.6.1/docs/conf.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       33 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/contributing.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/history.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      318 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/index.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1242 2020-02-17 11:49:32.000000 django-datadog-logger-0.6.1/docs/installation.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      783 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/make.bat
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       27 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.1/docs/readme.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       97 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/usage.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      139 2020-02-17 12:15:03.000000 django-datadog-logger-0.6.1/pyproject.toml
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       46 2023-04-27 12:59:29.000000 django-datadog-logger-0.6.1/requirements.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      404 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/setup.cfg
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1731 2023-04-27 15:00:05.000000 django-datadog-logger-0.6.1/setup.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/tests/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       51 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/tests/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      437 2020-02-17 11:54:33.000000 django-datadog-logger-0.6.1/tests/test_django_datadog_logger.py
```

### Comparing `django-datadog-logger-0.5.6/CONTRIBUTING.rst` & `django-datadog-logger-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/HISTORY.rst` & `django-datadog-logger-0.6.1/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 =======
 History
 =======
 
+0.6.1 (2023-04-27)
+------------------
+
+* Removed dependency on Celery package, fixed import error
+
+0.6.0 (2023-04-27)
+------------------
+
+* Removed dependency on Celery package
+
+0.5.6 (2023-01-17)
+------------------
+
+* Datadog formatter: avoid recursion loop when accessing WSGI request auth attribute
+
 0.5.5 (2023-01-16)
 ------------------
 
 * Improved support for request version reporting in `http.request_version`
 * Add support for `http.url_details.view_name`
 
 0.5.4 (2023-01-16)
```

### Comparing `django-datadog-logger-0.5.6/LICENSE` & `django-datadog-logger-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/PKG-INFO` & `django-datadog-logger-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-datadog-logger
-Version: 0.5.6
+Version: 0.6.1
 Summary: Django DataDog Logger integration package.
 Home-page: https://github.com/namespace-ee/django-datadog-logger
 Author: Lenno Nagel
 Author-email: lenno@namespace.ee
 License: MIT license
 Keywords: django_datadog_logger
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -234,14 +233,29 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.6.1 (2023-04-27)
+------------------
+
+* Removed dependency on Celery package, fixed import error
+
+0.6.0 (2023-04-27)
+------------------
+
+* Removed dependency on Celery package
+
+0.5.6 (2023-01-17)
+------------------
+
+* Datadog formatter: avoid recursion loop when accessing WSGI request auth attribute
+
 0.5.5 (2023-01-16)
 ------------------
 
 * Improved support for request version reporting in `http.request_version`
 * Add support for `http.url_details.view_name`
 
 0.5.4 (2023-01-16)
@@ -312,9 +326,7 @@
 
 * Added Celery request local.
 
 0.1.0 (2020-02-17)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `django-datadog-logger-0.5.6/README.rst` & `django-datadog-logger-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger/celery.py` & `django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_id.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-from functools import wraps
-
-from celery import Task
-
-from django_datadog_logger.local import Local, release_local  # NOQA
-
-local = Local()
-
-
-def get_celery_request():
-    try:
-        return local.request
-    except AttributeError:
-        return None
-
-
-def get_task_name(request):
-    if hasattr(request, "task"):
-        if isinstance(request.task, str):
-            return request.task
-        elif hasattr(request.task, "name"):
-            return request.task.name
-    return None
-
-
-def store_celery_request(func):
-    @wraps(func)
-    def function_wrapper(*args, **kwargs):
-        try:
-            if args and isinstance(args[0], Task) and hasattr(args[0], "request"):
-                local.request = {"id": args[0].request.id, "name": get_task_name(args[0].request)}
-            return func(*args, **kwargs)
-        finally:
-            release_local(local)
-
-    return function_wrapper
-
-
-__all__ = ["local", "get_celery_request", "store_celery_request"]
+import re
+import time
+import uuid
+
+from django_datadog_logger.wsgi import local
+from django_datadog_logger.local import release_local
+
+
+def generate_request_id():
+    return str(uuid.uuid4())
+
+
+def get_or_create_request_id(request):
+    request_id = request.META.get("HTTP_X_REQUEST_ID")
+    if request_id and re.match("^[a-zA-Z0-9+/=\-]{20,200}$", request_id):
+        return request_id
+    else:
+        return generate_request_id()
+
+
+class RequestIdMiddleware:
+    def __init__(self, get_response=None):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        request.request_id = get_or_create_request_id(request)
+        request.request_start_time = time.time()
+        local.request = request
+        response = self.get_response(request)
+        response["X-Request-ID"] = request.request_id
+        release_local(local)
+        return response
```

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger/formatters/datadog.py` & `django-datadog-logger-0.6.1/django_datadog_logger/formatters/datadog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import datetime
 import re
 import traceback
 
 import pytz
 import json_log_formatter
-from celery.worker.request import Request
 from django.conf import settings
 from django.core.exceptions import DisallowedHost
 from django.http.request import split_domain_port
 from django.urls import resolve, NoReverseMatch, Resolver404
 from rest_framework.compat import unicode_http_header
-from rest_framework.utils.mediatypes import _MediaType
 
 from django_datadog_logger.encoders import SafeJsonEncoder
-from django_datadog_logger.celery import get_task_name
+from django_datadog_logger.celery import get_task_name, get_celery_request
 import django_datadog_logger.celery
 import django_datadog_logger.wsgi
 
 # those fields are excluded from extra dict
 # and remains acceptable in record
 from django_datadog_logger.recursion import not_recursive, RecursionDetected
 
@@ -65,33 +63,27 @@
     if getattr(wsgi_request, "user", None) is not None:
         if getattr(wsgi_request.user, "is_authenticated", False):
             return wsgi_request.user
 
 
 class DataDogJSONFormatter(json_log_formatter.JSONFormatter):
     def json_record(self, message, extra, record):
-
         log_entry_dict = {
             "message": message,
             "logger.name": record.name,
             "logger.thread_name": record.threadName,
             "logger.method_name": record.funcName,
             "syslog.timestamp": pytz.utc.localize(datetime.datetime.utcfromtimestamp(record.created)).isoformat(),
             "syslog.severity": record.levelname,
         }
 
         # Add special `dd.` log record attributes added by `ddtrace` library
         # For example: dd.trace_id, dd.span_id, dd.service, dd.env, dd.version, etc
         log_entry_dict.update(self.get_datadog_attributes(record))
 
-        celery_request = self.get_celery_request(record)
-        if celery_request is not None:
-            log_entry_dict["celery.request_id"] = celery_request["id"]
-            log_entry_dict["celery.task_name"] = celery_request["name"]
-
         wsgi_request = self.get_wsgi_request()
         if wsgi_request is not None:
             log_entry_dict["network.client.ip"] = get_client_ip(wsgi_request)
 
             try:
                 domain, port = split_domain_port(wsgi_request.get_host())
             except DisallowedHost:
@@ -157,37 +149,32 @@
 
         if hasattr(record, "duration"):
             log_entry_dict["duration"] = record.duration
 
         if hasattr(record, "sql"):
             log_entry_dict["db.statement"] = record.sql
 
-        if record.name == "celery.app.trace":
-            if "data" in extra:
-                if "id" in extra["data"]:
-                    log_entry_dict["celery.request_id"] = extra["data"]["id"]
-                if "name" in extra["data"]:
-                    log_entry_dict["celery.task_name"] = extra["data"]["name"]
-                if "runtime" in extra["data"]:
-                    log_entry_dict["duration"] = extra["data"]["runtime"] * 1000000000
+        celery_request = get_celery_request()
+        if celery_request is not None:
+            log_entry_dict["celery.request_id"] = celery_request.id
+            log_entry_dict["celery.task_name"] = get_task_name(celery_request)
+        elif record.name in {"celery.app.trace", "celery.worker.strategy"} and "data" in extra:
+            if "id" in extra["data"]:
+                log_entry_dict["celery.request_id"] = extra["data"]["id"]
+            if "name" in extra["data"]:
+                log_entry_dict["celery.task_name"] = extra["data"]["name"]
+            if "runtime" in extra["data"]:
+                log_entry_dict["duration"] = extra["data"]["runtime"] * 1000000000
 
         if hasattr(settings, "DJANGO_DATADOG_LOGGER_EXTRA_INCLUDE"):
             if re.match(getattr(settings, "DJANGO_DATADOG_LOGGER_EXTRA_INCLUDE"), record.name):
                 log_entry_dict.update(extra)
 
         return log_entry_dict
 
-    def get_celery_request(self, record):
-        if record.name == "celery.worker.strategy" and record.args:
-            if isinstance(record.args, (list, tuple)) and isinstance(record.args[0], Request):
-                return {"id": record.args[0].id, "name": get_task_name(record.args[0])}
-            elif isinstance(record.args, dict):
-                return {"id": record.data.get("id"), "name": record.data.get("name")}
-        return django_datadog_logger.celery.get_celery_request()
-
     def get_datadog_attributes(self, record):
         """Helper to extract dd.* attributes from the log record."""
         return {attr_name: record.__dict__[attr_name] for attr_name in record.__dict__ if attr_name.startswith("dd.")}
 
     def get_wsgi_request(self):
         return django_datadog_logger.wsgi.get_wsgi_request()
```

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger/local.py` & `django-datadog-logger-0.6.1/django_datadog_logger/local.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger/middleware/request_log.py` & `django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_log.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger/rest_framework/mixins.py` & `django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger.egg-info/PKG-INFO` & `django-datadog-logger-0.6.1/django_datadog_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-datadog-logger
-Version: 0.5.6
+Version: 0.6.1
 Summary: Django DataDog Logger integration package.
 Home-page: https://github.com/namespace-ee/django-datadog-logger
 Author: Lenno Nagel
 Author-email: lenno@namespace.ee
 License: MIT license
 Keywords: django_datadog_logger
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -234,14 +233,29 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.6.1 (2023-04-27)
+------------------
+
+* Removed dependency on Celery package, fixed import error
+
+0.6.0 (2023-04-27)
+------------------
+
+* Removed dependency on Celery package
+
+0.5.6 (2023-01-17)
+------------------
+
+* Datadog formatter: avoid recursion loop when accessing WSGI request auth attribute
+
 0.5.5 (2023-01-16)
 ------------------
 
 * Improved support for request version reporting in `http.request_version`
 * Add support for `http.url_details.view_name`
 
 0.5.4 (2023-01-16)
@@ -312,9 +326,7 @@
 
 * Added Celery request local.
 
 0.1.0 (2020-02-17)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `django-datadog-logger-0.5.6/django_datadog_logger.egg-info/SOURCES.txt` & `django-datadog-logger-0.6.1/django_datadog_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/docs/Makefile` & `django-datadog-logger-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/docs/conf.py` & `django-datadog-logger-0.6.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,42 +15,43 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import django_datadog_logger
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'Django DataDog Logger'
+project = "Django DataDog Logger"
 copyright = "2020, Lenno Nagel"
 author = "Lenno Nagel"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -65,98 +66,89 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'django_datadog_loggerdoc'
+htmlhelp_basename = "django_datadog_loggerdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'django_datadog_logger.tex',
-     'Django DataDog Logger Documentation',
-     'Lenno Nagel', 'manual'),
+    (master_doc, "django_datadog_logger.tex", "Django DataDog Logger Documentation", "Lenno Nagel", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'django_datadog_logger',
-     'Django DataDog Logger Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "django_datadog_logger", "Django DataDog Logger Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'django_datadog_logger',
-     'Django DataDog Logger Documentation',
-     author,
-     'django_datadog_logger',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "django_datadog_logger",
+        "Django DataDog Logger Documentation",
+        author,
+        "django_datadog_logger",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
-
-
-
```

### Comparing `django-datadog-logger-0.5.6/docs/installation.rst` & `django-datadog-logger-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/docs/make.bat` & `django-datadog-logger-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.5.6/setup.py` & `django-datadog-logger-0.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="django_datadog_logger",
     name="django-datadog-logger",
     packages=find_packages(include=["django_datadog_logger", "django_datadog_logger.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/namespace-ee/django-datadog-logger",
-    version="0.5.6",
+    version="0.6.1",
     zip_safe=False,
 )
```

