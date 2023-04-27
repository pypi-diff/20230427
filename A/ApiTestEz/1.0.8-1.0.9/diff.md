# Comparing `tmp/ApiTestEz-1.0.8.tar.gz` & `tmp/ApiTestEz-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiTestEz-1.0.8.tar", last modified: Mon Jul  4 02:49:44 2022, max compression
+gzip compressed data, was "ApiTestEz-1.0.9.tar", last modified: Mon Jul  4 03:26:42 2022, max compression
```

## Comparing `ApiTestEz-1.0.8.tar` & `ApiTestEz-1.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.521192 ApiTestEz-1.0.8/
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.483736 ApiTestEz-1.0.8/ApiTestEz.egg-info/
--rw-rw-rw-   0        0        0      893 2022-07-04 02:49:43.000000 ApiTestEz-1.0.8/ApiTestEz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1393 2022-07-04 02:49:43.000000 ApiTestEz-1.0.8/ApiTestEz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-04 02:49:43.000000 ApiTestEz-1.0.8/ApiTestEz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-04 02:49:43.000000 ApiTestEz-1.0.8/ApiTestEz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      112 2022-07-04 02:49:43.000000 ApiTestEz-1.0.8/ApiTestEz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-07-04 02:49:43.000000 ApiTestEz-1.0.8/ApiTestEz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2022-06-18 09:48:06.000000 ApiTestEz-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      893 2022-07-04 02:49:44.520192 ApiTestEz-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    15916 2022-07-02 11:45:41.000000 ApiTestEz-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.524609 ApiTestEz-1.0.8/api_test_ez/
--rw-rw-rw-   0        0        0        5 2022-07-04 02:45:57.000000 ApiTestEz-1.0.8/api_test_ez/VERSION
--rw-rw-rw-   0        0        0       98 2022-06-16 11:13:26.000000 ApiTestEz-1.0.8/api_test_ez/__init__.py
--rw-rw-rw-   0        0        0       96 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/cmdline.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.657767 ApiTestEz-1.0.8/api_test_ez/core/
--rw-rw-rw-   0        0        0       98 2022-06-18 05:55:42.000000 ApiTestEz-1.0.8/api_test_ez/core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.734052 ApiTestEz-1.0.8/api_test_ez/core/case/
--rw-rw-rw-   0        0        0     5943 2022-06-28 03:08:53.000000 ApiTestEz-1.0.8/api_test_ez/core/case/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.841102 ApiTestEz-1.0.8/api_test_ez/core/case/frame/
--rw-rw-rw-   0        0        0       96 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/core/case/frame/__init__.py
--rw-rw-rw-   0        0        0      152 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/core/case/frame/frame_pytest.py
--rw-rw-rw-   0        0        0     3541 2022-06-15 11:43:12.000000 ApiTestEz-1.0.8/api_test_ez/core/case/frame/frame_unittest.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.924183 ApiTestEz-1.0.8/api_test_ez/core/case/http/
--rw-rw-rw-   0        0        0      198 2022-06-17 01:39:45.000000 ApiTestEz-1.0.8/api_test_ez/core/case/http/__init__.py
--rw-rw-rw-   0        0        0     4161 2022-06-20 12:08:51.000000 ApiTestEz-1.0.8/api_test_ez/core/case/http/request.py
--rw-rw-rw-   0        0        0     2007 2022-06-22 07:35:32.000000 ApiTestEz-1.0.8/api_test_ez/core/case/http/response.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:43.950872 ApiTestEz-1.0.8/api_test_ez/core/report/
--rw-rw-rw-   0        0        0     2933 2022-06-18 06:40:08.000000 ApiTestEz-1.0.8/api_test_ez/core/report/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.035053 ApiTestEz-1.0.8/api_test_ez/ez/
--rw-rw-rw-   0        0        0      227 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/ez/__init__.py
--rw-rw-rw-   0        0        0      284 2022-06-20 10:31:19.000000 ApiTestEz-1.0.8/api_test_ez/ez/config.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.192287 ApiTestEz-1.0.8/api_test_ez/ez/decorator/
--rw-rw-rw-   0        0        0      213 2022-06-16 06:13:16.000000 ApiTestEz-1.0.8/api_test_ez/ez/decorator/__init__.py
--rw-rw-rw-   0        0        0     1717 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/ez/decorator/jsonbean.py
--rw-rw-rw-   0        0        0      312 2022-06-17 07:38:13.000000 ApiTestEz-1.0.8/api_test_ez/ez/decorator/singleton.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.304184 ApiTestEz-1.0.8/api_test_ez/ez/http/
--rw-rw-rw-   0        0        0       98 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/ez/http/__init__.py
--rw-rw-rw-   0        0        0     7625 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/ez/http/http.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.341090 ApiTestEz-1.0.8/api_test_ez/ez/log/
--rw-rw-rw-   0        0        0       96 2022-06-13 06:19:30.000000 ApiTestEz-1.0.8/api_test_ez/ez/log/__init__.py
--rw-rw-rw-   0        0        0     4840 2022-06-22 08:46:01.000000 ApiTestEz-1.0.8/api_test_ez/ez/log/log.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.387016 ApiTestEz-1.0.8/api_test_ez/ez/mm/
--rw-rw-rw-   0        0        0      119 2022-06-20 07:45:17.000000 ApiTestEz-1.0.8/api_test_ez/ez/mm/__init__.py
--rw-rw-rw-   0        0        0      483 2022-06-20 09:10:55.000000 ApiTestEz-1.0.8/api_test_ez/ez/mm/schema.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.438690 ApiTestEz-1.0.8/api_test_ez/ez/serialize/
--rw-rw-rw-   0        0        0       98 2022-06-13 07:05:28.000000 ApiTestEz-1.0.8/api_test_ez/ez/serialize/__init__.py
--rw-rw-rw-   0        0        0     2881 2022-06-14 10:06:56.000000 ApiTestEz-1.0.8/api_test_ez/ez/serialize/errors.py
--rw-rw-rw-   0        0        0    16776 2022-06-21 12:19:34.000000 ApiTestEz-1.0.8/api_test_ez/ez/serialize/fields.py
--rw-rw-rw-   0        0        0     2930 2022-07-02 08:39:29.000000 ApiTestEz-1.0.8/api_test_ez/ez/serialize/models.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.466417 ApiTestEz-1.0.8/api_test_ez/libs/
--rw-rw-rw-   0        0        0    30452 2020-08-11 08:56:05.000000 ApiTestEz-1.0.8/api_test_ez/libs/HTMLTestRunner.py
--rw-rw-rw-   0        0        0       98 2022-06-17 11:11:03.000000 ApiTestEz-1.0.8/api_test_ez/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.472391 ApiTestEz-1.0.8/api_test_ez/project/
--rw-rw-rw-   0        0        0     5110 2022-06-22 09:14:29.000000 ApiTestEz-1.0.8/api_test_ez/project/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.500310 ApiTestEz-1.0.8/api_test_ez/project/configs/
--rw-rw-rw-   0        0        0     4979 2022-06-20 10:57:04.000000 ApiTestEz-1.0.8/api_test_ez/project/configs/__init__.py
--rw-rw-rw-   0        0        0      172 2022-06-20 12:00:27.000000 ApiTestEz-1.0.8/api_test_ez/project/configs/default_configs.cfg
-drwxrwxrwx   0        0        0        0 2022-07-04 02:49:44.516040 ApiTestEz-1.0.8/api_test_ez/project/settings/
--rw-rw-rw-   0        0        0     2045 2022-06-22 05:49:45.000000 ApiTestEz-1.0.8/api_test_ez/project/settings/__init__.py
--rw-rw-rw-   0        0        0      718 2022-06-18 04:50:05.000000 ApiTestEz-1.0.8/api_test_ez/project/settings/default_settings.py
--rw-rw-rw-   0        0        0       42 2022-07-04 02:49:44.521192 ApiTestEz-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1497 2022-07-04 02:45:50.000000 ApiTestEz-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.556580 ApiTestEz-1.0.9/
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.276701 ApiTestEz-1.0.9/ApiTestEz.egg-info/
+-rw-rw-rw-   0        0        0      995 2022-07-04 03:26:40.000000 ApiTestEz-1.0.9/ApiTestEz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1393 2022-07-04 03:26:41.000000 ApiTestEz-1.0.9/ApiTestEz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-04 03:26:40.000000 ApiTestEz-1.0.9/ApiTestEz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-04 03:26:40.000000 ApiTestEz-1.0.9/ApiTestEz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      112 2022-07-04 03:26:41.000000 ApiTestEz-1.0.9/ApiTestEz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-07-04 03:26:41.000000 ApiTestEz-1.0.9/ApiTestEz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2022-06-18 09:48:06.000000 ApiTestEz-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      995 2022-07-04 03:26:42.555584 ApiTestEz-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16517 2022-07-04 03:18:17.000000 ApiTestEz-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.317320 ApiTestEz-1.0.9/api_test_ez/
+-rw-rw-rw-   0        0        0        5 2022-07-04 03:26:32.000000 ApiTestEz-1.0.9/api_test_ez/VERSION
+-rw-rw-rw-   0        0        0       98 2022-06-16 11:13:26.000000 ApiTestEz-1.0.9/api_test_ez/__init__.py
+-rw-rw-rw-   0        0        0       96 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/cmdline.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.350596 ApiTestEz-1.0.9/api_test_ez/core/
+-rw-rw-rw-   0        0        0       98 2022-06-18 05:55:42.000000 ApiTestEz-1.0.9/api_test_ez/core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.361127 ApiTestEz-1.0.9/api_test_ez/core/case/
+-rw-rw-rw-   0        0        0     5943 2022-06-28 03:08:53.000000 ApiTestEz-1.0.9/api_test_ez/core/case/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.426046 ApiTestEz-1.0.9/api_test_ez/core/case/frame/
+-rw-rw-rw-   0        0        0       96 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/core/case/frame/__init__.py
+-rw-rw-rw-   0        0        0      152 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/core/case/frame/frame_pytest.py
+-rw-rw-rw-   0        0        0     3541 2022-06-15 11:43:12.000000 ApiTestEz-1.0.9/api_test_ez/core/case/frame/frame_unittest.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.469539 ApiTestEz-1.0.9/api_test_ez/core/case/http/
+-rw-rw-rw-   0        0        0      198 2022-06-17 01:39:45.000000 ApiTestEz-1.0.9/api_test_ez/core/case/http/__init__.py
+-rw-rw-rw-   0        0        0     4161 2022-06-20 12:08:51.000000 ApiTestEz-1.0.9/api_test_ez/core/case/http/request.py
+-rw-rw-rw-   0        0        0     2007 2022-06-22 07:35:32.000000 ApiTestEz-1.0.9/api_test_ez/core/case/http/response.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.491262 ApiTestEz-1.0.9/api_test_ez/core/report/
+-rw-rw-rw-   0        0        0     3106 2022-07-04 03:18:32.000000 ApiTestEz-1.0.9/api_test_ez/core/report/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.842742 ApiTestEz-1.0.9/api_test_ez/ez/
+-rw-rw-rw-   0        0        0      227 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/ez/__init__.py
+-rw-rw-rw-   0        0        0      284 2022-06-20 10:31:19.000000 ApiTestEz-1.0.9/api_test_ez/ez/config.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.913556 ApiTestEz-1.0.9/api_test_ez/ez/decorator/
+-rw-rw-rw-   0        0        0      213 2022-06-16 06:13:16.000000 ApiTestEz-1.0.9/api_test_ez/ez/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1717 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/ez/decorator/jsonbean.py
+-rw-rw-rw-   0        0        0      312 2022-06-17 07:38:13.000000 ApiTestEz-1.0.9/api_test_ez/ez/decorator/singleton.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.943239 ApiTestEz-1.0.9/api_test_ez/ez/http/
+-rw-rw-rw-   0        0        0       98 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/ez/http/__init__.py
+-rw-rw-rw-   0        0        0     7625 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/ez/http/http.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:41.989583 ApiTestEz-1.0.9/api_test_ez/ez/log/
+-rw-rw-rw-   0        0        0       96 2022-06-13 06:19:30.000000 ApiTestEz-1.0.9/api_test_ez/ez/log/__init__.py
+-rw-rw-rw-   0        0        0     4840 2022-06-22 08:46:01.000000 ApiTestEz-1.0.9/api_test_ez/ez/log/log.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.067190 ApiTestEz-1.0.9/api_test_ez/ez/mm/
+-rw-rw-rw-   0        0        0      119 2022-06-20 07:45:17.000000 ApiTestEz-1.0.9/api_test_ez/ez/mm/__init__.py
+-rw-rw-rw-   0        0        0      483 2022-06-20 09:10:55.000000 ApiTestEz-1.0.9/api_test_ez/ez/mm/schema.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.155794 ApiTestEz-1.0.9/api_test_ez/ez/serialize/
+-rw-rw-rw-   0        0        0       98 2022-06-13 07:05:28.000000 ApiTestEz-1.0.9/api_test_ez/ez/serialize/__init__.py
+-rw-rw-rw-   0        0        0     2881 2022-06-14 10:06:56.000000 ApiTestEz-1.0.9/api_test_ez/ez/serialize/errors.py
+-rw-rw-rw-   0        0        0    16776 2022-06-21 12:19:34.000000 ApiTestEz-1.0.9/api_test_ez/ez/serialize/fields.py
+-rw-rw-rw-   0        0        0     2930 2022-07-02 08:39:29.000000 ApiTestEz-1.0.9/api_test_ez/ez/serialize/models.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.219898 ApiTestEz-1.0.9/api_test_ez/libs/
+-rw-rw-rw-   0        0        0    30452 2020-08-11 08:56:05.000000 ApiTestEz-1.0.9/api_test_ez/libs/HTMLTestRunner.py
+-rw-rw-rw-   0        0        0       98 2022-06-17 11:11:03.000000 ApiTestEz-1.0.9/api_test_ez/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.272132 ApiTestEz-1.0.9/api_test_ez/project/
+-rw-rw-rw-   0        0        0     5110 2022-06-22 09:14:29.000000 ApiTestEz-1.0.9/api_test_ez/project/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.392468 ApiTestEz-1.0.9/api_test_ez/project/configs/
+-rw-rw-rw-   0        0        0     4979 2022-06-20 10:57:04.000000 ApiTestEz-1.0.9/api_test_ez/project/configs/__init__.py
+-rw-rw-rw-   0        0        0      172 2022-06-20 12:00:27.000000 ApiTestEz-1.0.9/api_test_ez/project/configs/default_configs.cfg
+drwxrwxrwx   0        0        0        0 2022-07-04 03:26:42.419539 ApiTestEz-1.0.9/api_test_ez/project/settings/
+-rw-rw-rw-   0        0        0     2045 2022-06-22 05:49:45.000000 ApiTestEz-1.0.9/api_test_ez/project/settings/__init__.py
+-rw-rw-rw-   0        0        0      718 2022-06-18 04:50:05.000000 ApiTestEz-1.0.9/api_test_ez/project/settings/default_settings.py
+-rw-rw-rw-   0        0        0       42 2022-07-04 03:26:42.556580 ApiTestEz-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2022-07-04 03:21:53.000000 ApiTestEz-1.0.9/setup.py
```

### Comparing `ApiTestEz-1.0.8/ApiTestEz.egg-info/PKG-INFO` & `ApiTestEz-1.0.9/ApiTestEz.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ApiTestEz
-Version: 1.0.8
+Version: 1.0.9
 Summary: An easier api test framework.
 Home-page: https://github.com/bruce4520196/ApiTestEz
 Author: Bruce Cai
 Maintainer: Bruce Cai
 Maintainer-email: whiteghostcat@gmail.com
 Classifier: Framework :: Scrapy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
```

### Comparing `ApiTestEz-1.0.8/ApiTestEz.egg-info/SOURCES.txt` & `ApiTestEz-1.0.9/ApiTestEz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/PKG-INFO` & `ApiTestEz-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ApiTestEz
-Version: 1.0.8
+Version: 1.0.9
 Summary: An easier api test framework.
 Home-page: https://github.com/bruce4520196/ApiTestEz
 Author: Bruce Cai
 Maintainer: Bruce Cai
 Maintainer-email: whiteghostcat@gmail.com
 Classifier: Framework :: Scrapy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
```

### Comparing `ApiTestEz-1.0.8/README.md` & `ApiTestEz-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -398,14 +398,28 @@
             ps = PhoneSchema()
             ps.context["request"] = self.request
             self.response.validate(ps)
     ```
 
 ---
 
+### 测试报告
+
+- HtmlReporter
+
+```python
+from api_test_ez.core.report import HtmlReporter, BRReporter
+
+report = HtmlReporter(case_path='<some_case_path>')
+report.run()
+```
+`HtmlReporter`对象接收3个参数:<br>
+`case_path`: 用例脚本文件路径，如果**目录**将会遍历目录下的python文件以找到**所有**测试用例。
+`report_title`: 报告页面中的title，如果为*None*将会读取项目settings.py文件中的`REPORT_TITLE`字段。
+`report_desc`: 报告页面中的描述，如果为*None*将会读取项目settings.py文件中的`REPORT_DESC`字段。
 
 ### TODO
 1.  用例支持入参，例：f"{'X-Forwarded-For': ${province_ip} }"
 2.  url拆分host + path
 3.  ~~报告~~
 4.  ~~ORM响应断言实现~~
 5.  cmdline
```

### Comparing `ApiTestEz-1.0.8/api_test_ez/core/case/__init__.py` & `ApiTestEz-1.0.9/api_test_ez/core/case/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/core/case/frame/frame_unittest.py` & `ApiTestEz-1.0.9/api_test_ez/core/case/frame/frame_unittest.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/core/case/http/request.py` & `ApiTestEz-1.0.9/api_test_ez/core/case/http/request.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/core/case/http/response.py` & `ApiTestEz-1.0.9/api_test_ez/core/case/http/response.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/core/report/__init__.py` & `ApiTestEz-1.0.9/api_test_ez/core/report/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,22 @@
             self.logger.info("********TEST END*********")
             fp.close()
 
 
 class BRReporter(Reporter):
     """BeautifulReport"""
 
+    def __init__(self, case_path, report_theme=None,  *args, **kwargs):
+        super().__init__(case_path, *args, **kwargs)
+        self.report_theme = report_theme
+
     def run(self):
         if not os.path.exists(self.report_dir):
             os.makedirs(self.report_dir)
         suit = self.load_tests()
         result = BeautifulReport(suit)
         result.report(
             filename=self.report_file_name,
             description=self.report_title,
             report_dir=self.report_dir,
-            theme='theme_default'
+            theme=self.report_theme
         )
```

### Comparing `ApiTestEz-1.0.8/api_test_ez/ez/decorator/jsonbean.py` & `ApiTestEz-1.0.9/api_test_ez/ez/decorator/jsonbean.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/ez/http/http.py` & `ApiTestEz-1.0.9/api_test_ez/ez/http/http.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/ez/log/log.py` & `ApiTestEz-1.0.9/api_test_ez/ez/log/log.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/ez/serialize/errors.py` & `ApiTestEz-1.0.9/api_test_ez/ez/serialize/errors.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/ez/serialize/fields.py` & `ApiTestEz-1.0.9/api_test_ez/ez/serialize/fields.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/ez/serialize/models.py` & `ApiTestEz-1.0.9/api_test_ez/ez/serialize/models.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/libs/HTMLTestRunner.py` & `ApiTestEz-1.0.9/api_test_ez/libs/HTMLTestRunner.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/project/__init__.py` & `ApiTestEz-1.0.9/api_test_ez/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/project/configs/__init__.py` & `ApiTestEz-1.0.9/api_test_ez/project/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/project/settings/__init__.py` & `ApiTestEz-1.0.9/api_test_ez/project/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/api_test_ez/project/settings/default_settings.py` & `ApiTestEz-1.0.9/api_test_ez/project/settings/default_settings.py`

 * *Files identical despite different names*

### Comparing `ApiTestEz-1.0.8/setup.py` & `ApiTestEz-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         'Framework :: Scrapy',
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
```

