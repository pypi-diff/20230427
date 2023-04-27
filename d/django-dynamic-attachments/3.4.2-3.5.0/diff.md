# Comparing `tmp/django-dynamic-attachments-3.4.2.tar.gz` & `tmp/django-dynamic-attachments-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-attachments-3.4.2.tar", last modified: Fri Apr 22 19:04:18 2022, max compression
+gzip compressed data, was "django-dynamic-attachments-3.5.0.tar", last modified: Thu Apr 27 14:01:10 2023, max compression
```

## Comparing `django-dynamic-attachments-3.4.2.tar` & `django-dynamic-attachments-3.5.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.420900 django-dynamic-attachments-3.4.2/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/LICENSE
--rw-rw----   0 ruttenb   (1328) ims        (100)       83 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/MANIFEST.in
--rw-r--r--   0 ruttenb   (1328) ims        (100)      605 2022-04-22 19:04:18.421903 django-dynamic-attachments-3.4.2/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)      190 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/README.md
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.202907 django-dynamic-attachments-3.4.2/attachments/
--rw-r--r--   0 ruttenb   (1328) ims        (100)      360 2022-04-22 19:01:49.000000 django-dynamic-attachments-3.4.2/attachments/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1264 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/admin.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      514 2020-08-14 14:31:07.000000 django-dynamic-attachments-3.4.2/attachments/apps.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      464 2019-10-24 15:47:50.000000 django-dynamic-attachments-3.4.2/attachments/exceptions.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     4160 2021-03-24 17:20:13.000000 django-dynamic-attachments-3.4.2/attachments/forms.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.280898 django-dynamic-attachments-3.4.2/attachments/migrations/
--rw-rw----   0 ruttenb   (1328) ims        (100)     2912 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0001_initial.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1306 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0002_property.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      372 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0003_auto_20150317_1319.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      632 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0004_auto_20150507_1438.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      857 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0005_auto_20150708_1435.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      554 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0006_session_content_type.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      447 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0007_property_required.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      427 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0008_session_data.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1082 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0009_auto_20170202_1700.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      463 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0010_property_is_editable.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      540 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0011_session_allowed_file_types.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      859 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0012_auto_20180906_1449.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1554 2019-11-07 16:25:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/0013_auto_20191107_1122.py
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/migrations/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)    14941 2021-09-22 14:03:07.000000 django-dynamic-attachments-3.4.2/attachments/models.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      734 2019-10-24 15:47:50.000000 django-dynamic-attachments-3.4.2/attachments/signals.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.087898 django-dynamic-attachments-3.4.2/attachments/static/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.089925 django-dynamic-attachments-3.4.2/attachments/static/attachments/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.291900 django-dynamic-attachments-3.4.2/attachments/static/attachments/css/
--rw-rw----   0 ruttenb   (1328) ims        (100)      151 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/static/attachments/css/attachments.css
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.305899 django-dynamic-attachments-3.4.2/attachments/static/attachments/js/
--rw-r-----   0 ruttenb   (1328) ims        (100)     6375 2022-02-03 14:03:54.000000 django-dynamic-attachments-3.4.2/attachments/static/attachments/js/attachments.js
--rw-rw----   0 ruttenb   (1328) ims        (100)    10468 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/static/attachments/js/jquery.iframe-transport.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.092899 django-dynamic-attachments-3.4.2/attachments/templates/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.337900 django-dynamic-attachments-3.4.2/attachments/templates/attachments/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1011 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/templates/attachments/edit_properties.html
--rw-rw----   0 ruttenb   (1328) ims        (100)       47 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/templates/attachments/form.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1116 2019-10-24 15:47:50.000000 django-dynamic-attachments-3.4.2/attachments/templates/attachments/list.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      951 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/templates/attachments/view_properties.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.364899 django-dynamic-attachments-3.4.2/attachments/templatetags/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/templatetags/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      678 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/templatetags/attachments.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      701 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.4.2/attachments/urls.py
--rw-r-----   0 ruttenb   (1328) ims        (100)     4629 2022-02-03 14:03:54.000000 django-dynamic-attachments-3.4.2/attachments/utils.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     9303 2022-04-22 19:01:49.000000 django-dynamic-attachments-3.4.2/attachments/views.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2022-04-22 19:04:18.416906 django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/
--rw-rw----   0 ruttenb   (1328) ims        (100)      605 2022-04-22 19:04:13.000000 django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)     1621 2022-04-22 19:04:13.000000 django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/SOURCES.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        1 2022-04-22 19:04:13.000000 django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/dependency_links.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)       71 2022-04-22 19:04:13.000000 django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/requires.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)       12 2022-04-22 19:04:13.000000 django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/top_level.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)      456 2022-04-22 19:04:18.424903 django-dynamic-attachments-3.4.2/setup.cfg
--rw-rw----   0 ruttenb   (1328) ims        (100)      892 2021-09-22 14:03:07.000000 django-dynamic-attachments-3.4.2/setup.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.147634 django-dynamic-attachments-3.5.0/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/LICENSE
+-rw-rw----   0 ruttenb   (1328) ims        (100)       83 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/MANIFEST.in
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      605 2023-04-27 14:01:10.148635 django-dynamic-attachments-3.5.0/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)      190 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/README.md
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.018644 django-dynamic-attachments-3.5.0/attachments/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      360 2023-04-27 14:00:52.000000 django-dynamic-attachments-3.5.0/attachments/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1264 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/admin.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      514 2020-08-14 14:31:07.000000 django-dynamic-attachments-3.5.0/attachments/apps.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      464 2019-10-24 15:47:50.000000 django-dynamic-attachments-3.5.0/attachments/exceptions.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     4160 2021-03-24 17:20:13.000000 django-dynamic-attachments-3.5.0/attachments/forms.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.078633 django-dynamic-attachments-3.5.0/attachments/migrations/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2912 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0001_initial.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1306 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0002_property.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      372 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0003_auto_20150317_1319.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      632 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0004_auto_20150507_1438.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      857 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0005_auto_20150708_1435.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      554 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0006_session_content_type.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      447 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0007_property_required.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      427 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0008_session_data.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1082 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0009_auto_20170202_1700.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      463 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0010_property_is_editable.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      540 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0011_session_allowed_file_types.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      859 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0012_auto_20180906_1449.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1554 2019-11-07 16:25:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0013_auto_20191107_1122.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      540 2023-04-27 14:00:52.000000 django-dynamic-attachments-3.5.0/attachments/migrations/0014_auto_20220615_1524.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/migrations/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    14938 2023-04-27 14:00:52.000000 django-dynamic-attachments-3.5.0/attachments/models.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      734 2019-10-24 15:47:50.000000 django-dynamic-attachments-3.5.0/attachments/signals.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:09.934631 django-dynamic-attachments-3.5.0/attachments/static/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:09.937624 django-dynamic-attachments-3.5.0/attachments/static/attachments/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.082628 django-dynamic-attachments-3.5.0/attachments/static/attachments/css/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      151 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/static/attachments/css/attachments.css
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.091626 django-dynamic-attachments-3.5.0/attachments/static/attachments/js/
+-rw-r-----   0 ruttenb   (1328) ims        (100)     6375 2022-02-03 14:03:54.000000 django-dynamic-attachments-3.5.0/attachments/static/attachments/js/attachments.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)    10468 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/static/attachments/js/jquery.iframe-transport.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:09.939661 django-dynamic-attachments-3.5.0/attachments/templates/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.108633 django-dynamic-attachments-3.5.0/attachments/templates/attachments/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1011 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/templates/attachments/edit_properties.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)       47 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/templates/attachments/form.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1116 2019-10-24 15:47:50.000000 django-dynamic-attachments-3.5.0/attachments/templates/attachments/list.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      951 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/templates/attachments/view_properties.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.117627 django-dynamic-attachments-3.5.0/attachments/templatetags/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/templatetags/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      678 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/templatetags/attachments.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      701 2019-10-24 15:47:34.000000 django-dynamic-attachments-3.5.0/attachments/urls.py
+-rw-r-----   0 ruttenb   (1328) ims        (100)     4629 2022-02-03 14:03:54.000000 django-dynamic-attachments-3.5.0/attachments/utils.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     9303 2022-04-22 19:01:49.000000 django-dynamic-attachments-3.5.0/attachments/views.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-27 14:01:10.143635 django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      605 2023-04-27 14:01:08.000000 django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1671 2023-04-27 14:01:09.000000 django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/SOURCES.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-04-27 14:01:08.000000 django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/dependency_links.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)       71 2023-04-27 14:01:08.000000 django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/requires.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)       12 2023-04-27 14:01:08.000000 django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/top_level.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)      456 2023-04-27 14:01:10.151631 django-dynamic-attachments-3.5.0/setup.cfg
+-rw-rw----   0 ruttenb   (1328) ims        (100)      892 2021-09-22 14:03:07.000000 django-dynamic-attachments-3.5.0/setup.py
```

### Comparing `django-dynamic-attachments-3.4.2/LICENSE` & `django-dynamic-attachments-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/PKG-INFO` & `django-dynamic-attachments-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-attachments
-Version: 3.4.2
+Version: 3.5.0
 Summary: A Django application for handling file uploads and attaching them to arbitrary models.
 Home-page: https://github.com/imsweb/django-dynamic-attachments
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-dynamic-attachments-3.4.2/attachments/admin.py` & `django-dynamic-attachments-3.5.0/attachments/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/apps.py` & `django-dynamic-attachments-3.5.0/attachments/apps.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/forms.py` & `django-dynamic-attachments-3.5.0/attachments/forms.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0001_initial.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0002_property.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0002_property.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0004_auto_20150507_1438.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0004_auto_20150507_1438.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0005_auto_20150708_1435.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0005_auto_20150708_1435.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0006_session_content_type.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0006_session_content_type.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0009_auto_20170202_1700.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0009_auto_20170202_1700.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0011_session_allowed_file_types.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0011_session_allowed_file_types.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0012_auto_20180906_1449.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0012_auto_20180906_1449.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/migrations/0013_auto_20191107_1122.py` & `django-dynamic-attachments-3.5.0/attachments/migrations/0013_auto_20191107_1122.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/models.py` & `django-dynamic-attachments-3.5.0/attachments/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from __future__ import unicode_literals
-
 from django.conf import settings
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.files import File
 from django.db import models
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 
-from .signals import attachments_attached
-from .utils import JSONField, get_context_key, get_default_path, get_storage, import_class, sizeof_fmt, Centos7ClamdUnixSocket
-from .exceptions import VirusFoundException, InvalidExtensionException, InvalidFileTypeException, FileSizeException
+from attachments.signals import attachments_attached
+from attachments.utils import JSONField, get_context_key, get_default_path, get_storage, import_class, sizeof_fmt, Centos7ClamdUnixSocket
+from attachments.exceptions import VirusFoundException, InvalidExtensionException, InvalidFileTypeException, FileSizeException
 
 import os
 import magic
 import mimetypes
 import ntpath
 
 
@@ -53,15 +51,15 @@
             content_object=obj
         )
 
 
 class Attachment (models.Model):
     file_path = models.TextField(unique=True)
     file_name = models.CharField(max_length=200)
-    file_size = models.IntegerField()
+    file_size = models.BigIntegerField()
     user = models.ForeignKey(settings.AUTH_USER_MODEL, related_name='attachments', null=True, blank=True, on_delete=models.SET_NULL)
     context = models.CharField(max_length=200, blank=True, db_index=True)
     date_created = models.DateTimeField(default=timezone.now, editable=False)
 
     # User-defined data, stored as JSON in a text field.
     data = JSONField(null=True)
 
@@ -282,15 +280,15 @@
                 raise InvalidExtensionException("{} - Error: Unsupported file format. Supported file formats are: {}".format(
                     upload.file_name, ', '.join(allowed_exts)))
 
             # Checking whether file contents comply with the allowed file extensions (if the file has data).
             # This ensures that file types not allowed are rejected even if they are renamed.
             if upload.file_size != 0:
                 file_mime = magic.from_file(upload.file_path, mime=True)
- 
+
                 if (set(mimetypes.guess_all_extensions(file_mime)).isdisjoint(set(allowed_exts)) and 
                     file_mime not in mime_types_overrides.get(ext, [])):
                     # In case our check for extensions didn't pass we check if the file type (not mimetype)
                     # is white-listed. If so, we can allow the file to be uploaded.
                     allowed_types = self.allowed_file_types.split('\n')
                     file_type = magic.from_file(upload.file_path, mime=False)
                     if file_type not in allowed_types:
@@ -319,15 +317,15 @@
                 raise VirusFoundException('**WARNING** virus: "{}" found in the file: "{}", could not upload!'.format(virus[upload.file_path][1], upload.file_name))
 
 
 class Upload (models.Model):
     session = models.ForeignKey(Session, related_name='uploads', on_delete=models.CASCADE)
     file_path = models.TextField(unique=True)
     file_name = models.CharField(max_length=200)
-    file_size = models.IntegerField()
+    file_size = models.BigIntegerField()
     date_created = models.DateTimeField(default=timezone.now)
 
     def __str__(self):
         return self.file_name
 
     def delete(self, **kwargs):
         try:
```

### Comparing `django-dynamic-attachments-3.4.2/attachments/signals.py` & `django-dynamic-attachments-3.5.0/attachments/signals.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/static/attachments/js/attachments.js` & `django-dynamic-attachments-3.5.0/attachments/static/attachments/js/attachments.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/static/attachments/js/jquery.iframe-transport.js` & `django-dynamic-attachments-3.5.0/attachments/static/attachments/js/jquery.iframe-transport.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/templates/attachments/edit_properties.html` & `django-dynamic-attachments-3.5.0/attachments/templates/attachments/edit_properties.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/templates/attachments/list.html` & `django-dynamic-attachments-3.5.0/attachments/templates/attachments/list.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/templates/attachments/view_properties.html` & `django-dynamic-attachments-3.5.0/attachments/templates/attachments/view_properties.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/templatetags/attachments.py` & `django-dynamic-attachments-3.5.0/attachments/templatetags/attachments.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/urls.py` & `django-dynamic-attachments-3.5.0/attachments/urls.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/utils.py` & `django-dynamic-attachments-3.5.0/attachments/utils.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/attachments/views.py` & `django-dynamic-attachments-3.5.0/attachments/views.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/PKG-INFO` & `django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-attachments
-Version: 3.4.2
+Version: 3.5.0
 Summary: A Django application for handling file uploads and attaching them to arbitrary models.
 Home-page: https://github.com/imsweb/django-dynamic-attachments
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-dynamic-attachments-3.4.2/django_dynamic_attachments.egg-info/SOURCES.txt` & `django-dynamic-attachments-3.5.0/django_dynamic_attachments.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 attachments/migrations/0007_property_required.py
 attachments/migrations/0008_session_data.py
 attachments/migrations/0009_auto_20170202_1700.py
 attachments/migrations/0010_property_is_editable.py
 attachments/migrations/0011_session_allowed_file_types.py
 attachments/migrations/0012_auto_20180906_1449.py
 attachments/migrations/0013_auto_20191107_1122.py
+attachments/migrations/0014_auto_20220615_1524.py
 attachments/migrations/__init__.py
 attachments/static/attachments/css/attachments.css
 attachments/static/attachments/js/attachments.js
 attachments/static/attachments/js/jquery.iframe-transport.js
 attachments/templates/attachments/edit_properties.html
 attachments/templates/attachments/form.html
 attachments/templates/attachments/list.html
```

### Comparing `django-dynamic-attachments-3.4.2/setup.py` & `django-dynamic-attachments-3.5.0/setup.py`

 * *Files identical despite different names*

