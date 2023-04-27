# Comparing `tmp/django-rest-witchcraft-0.8.3.tar.gz` & `tmp/django-rest-witchcraft-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rest-witchcraft-0.8.3.tar", last modified: Thu Jun 27 02:33:53 2019, max compression
+gzip compressed data, was "dist/django-rest-witchcraft-0.9.0.tar", last modified: Fri Jun 28 13:18:59 2019, max compression
```

## Comparing `django-rest-witchcraft-0.8.3.tar` & `django-rest-witchcraft-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/
--rw-r--r--   0 serkan    (1000) serkan    (1000)     8177 2019-06-27 02:33:19.000000 django-rest-witchcraft-0.8.3/HISTORY.rst
--rw-r--r--   0 serkan    (1000) serkan    (1000)      107 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/MANIFEST.in
--rw-r--r--   0 serkan    (1000) serkan    (1000)    10300 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/PKG-INFO
--rw-r--r--   0 serkan    (1000) serkan    (1000)     7137 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/README.rst
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/
--rw-r--r--   0 serkan    (1000) serkan    (1000)    10300 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/PKG-INFO
--rw-r--r--   0 serkan    (1000) serkan    (1000)      803 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/SOURCES.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)        1 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/dependency_links.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)       39 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/requires.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)       16 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/top_level.txt
--rw-r--r--   0 serkan    (1000) serkan    (1000)      240 2019-06-25 11:21:23.000000 django-rest-witchcraft-0.8.3/requirements.txt
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      190 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      256 2019-06-27 02:33:19.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/__version__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3262 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/field_mapping.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3064 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/fields.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2196 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/generics.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4039 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/mixins.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1962 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/routers.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    38160 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/serializers.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1078 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/utils.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     1434 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/rest_witchcraft/viewsets.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      403 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/setup.cfg
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2283 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/setup.py
-drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-27 02:33:53.000000 django-rest-witchcraft-0.8.3/tests/
--rw-r--r--   0 serkan    (1000) serkan    (1000)      304 2019-06-25 11:21:23.000000 django-rest-witchcraft-0.8.3/tests/__init__.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     4023 2019-06-25 11:21:23.000000 django-rest-witchcraft-0.8.3/tests/models.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      837 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/models_composite.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3912 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_field_mapping.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3963 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_fields.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     2183 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_generics.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     3679 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_mixins.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)     8357 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_routers.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)    58116 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_serializers.py
--rw-r--r--   0 serkan    (1000) serkan    (1000)      668 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.8.3/tests/test_utils.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     8285 2019-06-28 13:18:34.000000 django-rest-witchcraft-0.9.0/HISTORY.rst
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      107 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.9.0/MANIFEST.in
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    10444 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/PKG-INFO
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     7266 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/README.rst
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    10444 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/PKG-INFO
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      803 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)        1 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       61 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/requires.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)       16 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/top_level.txt
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      240 2019-06-25 11:21:23.000000 django-rest-witchcraft-0.9.0/requirements.txt
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      190 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      256 2019-06-28 13:18:34.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/__version__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3290 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/field_mapping.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2041 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/fields.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2196 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/generics.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4040 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/mixins.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1962 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/routers.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    38161 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/serializers.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1078 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/utils.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     1434 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.9.0/rest_witchcraft/viewsets.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      403 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/setup.cfg
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2307 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/setup.py
+drwxr-xr-x   0 serkan    (1000) serkan    (1000)        0 2019-06-28 13:18:59.000000 django-rest-witchcraft-0.9.0/tests/
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      304 2019-06-25 11:21:23.000000 django-rest-witchcraft-0.9.0/tests/__init__.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     4023 2019-06-25 11:21:23.000000 django-rest-witchcraft-0.9.0/tests/models.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      837 2019-04-13 12:39:07.000000 django-rest-witchcraft-0.9.0/tests/models_composite.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3940 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_field_mapping.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2235 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_fields.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     2184 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_generics.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     3681 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_mixins.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)     8358 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_routers.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)    58117 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_serializers.py
+-rw-r--r--   0 serkan    (1000) serkan    (1000)      668 2019-06-28 13:16:30.000000 django-rest-witchcraft-0.9.0/tests/test_utils.py
```

### Comparing `django-rest-witchcraft-0.8.3/HISTORY.rst` & `django-rest-witchcraft-0.9.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Changelog
 =========
 
 
-0.8.3 (2019-06-26)
+0.9.0 (2019-06-28)
 -----------------------------
+- Drop enumfield and update importanize config (#45) [Serkan Hosca]
+
+
+0.8.3 (2019-06-27)
+------------------
 - Fix module test runner target (#44) [Serkan Hosca]
 - Switching to tox-travis and tox matrix (#43) [Miroslav Shubernetskiy]
 - Run tests with pg (#42) [Serkan Hosca]
 - Update pre-commit (#41) [Serkan Hosca]
 
 
 0.8.2 (2019-02-11)
```

### Comparing `django-rest-witchcraft-0.8.3/PKG-INFO` & `django-rest-witchcraft-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: django-rest-witchcraft
-Version: 0.8.3
+Version: 0.9.0
 Summary: Django REST Framework and SQLAlchemy integration
 Home-page: https://github.com/shosca/django-rest-witchcraft
 Author: Serkan Hosca
 Author-email: serkan@hosca.com
 License: MIT
 Description: Django REST Witchcraft
         ======================
         
-        |Build Status| |Read The Docs| |PyPI version| |Coveralls Status|
+        |Build Status| |Read The Docs| |PyPI version| |Coveralls Status| |Black|
         
         **Django REST Framework integration with SQLAlchemy**
         
         django-rest-witchcraft is an extension for Django REST Framework that adds support for SQLAlchemy. It aims to provide
         a similar development experience to building REST api's with Django REST Framework with Django ORM, except with
         SQLAlchemy.
         
@@ -173,15 +173,15 @@
         .. code:: python
         
             group = Group(name='Admin')
             session.add(group)
             session.flush()
         
             serializer = UserSerializer(user, data={
-                'group': {'id': group.id
+                'group': {'id': group.id}
             })
             serializer.is_valid()
             serializer.save()
         
             user = serializer.instance
         
         Now, our user looks like:
@@ -255,18 +255,20 @@
            :target: https://travis-ci.org/shosca/django-rest-witchcraft
         .. |Read The Docs| image:: https://readthedocs.org/projects/django-rest-witchcraft/badge/?version=latest
            :target: http://django-rest-witchcraft.readthedocs.io/en/latest/?badge=latest
         .. |PyPI version| image:: https://badge.fury.io/py/django-rest-witchcraft.svg
            :target: https://badge.fury.io/py/django-rest-witchcraft
         .. |Coveralls Status| image:: https://coveralls.io/repos/github/shosca/django-rest-witchcraft/badge.svg?branch=master
            :target: https://coveralls.io/github/shosca/django-rest-witchcraft?branch=master
+        .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+           :target: https://github.com/ambv/black
         
 Keywords: sqlalchemy django rest framework drf rest_framework
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `django-rest-witchcraft-0.8.3/README.rst` & `django-rest-witchcraft-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django REST Witchcraft
 ======================
 
-|Build Status| |Read The Docs| |PyPI version| |Coveralls Status|
+|Build Status| |Read The Docs| |PyPI version| |Coveralls Status| |Black|
 
 **Django REST Framework integration with SQLAlchemy**
 
 django-rest-witchcraft is an extension for Django REST Framework that adds support for SQLAlchemy. It aims to provide
 a similar development experience to building REST api's with Django REST Framework with Django ORM, except with
 SQLAlchemy.
 
@@ -165,15 +165,15 @@
 .. code:: python
 
     group = Group(name='Admin')
     session.add(group)
     session.flush()
 
     serializer = UserSerializer(user, data={
-        'group': {'id': group.id
+        'group': {'id': group.id}
     })
     serializer.is_valid()
     serializer.save()
 
     user = serializer.instance
 
 Now, our user looks like:
@@ -247,7 +247,9 @@
    :target: https://travis-ci.org/shosca/django-rest-witchcraft
 .. |Read The Docs| image:: https://readthedocs.org/projects/django-rest-witchcraft/badge/?version=latest
    :target: http://django-rest-witchcraft.readthedocs.io/en/latest/?badge=latest
 .. |PyPI version| image:: https://badge.fury.io/py/django-rest-witchcraft.svg
    :target: https://badge.fury.io/py/django-rest-witchcraft
 .. |Coveralls Status| image:: https://coveralls.io/repos/github/shosca/django-rest-witchcraft/badge.svg?branch=master
    :target: https://coveralls.io/github/shosca/django-rest-witchcraft?branch=master
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/ambv/black
```

### Comparing `django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/PKG-INFO` & `django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: django-rest-witchcraft
-Version: 0.8.3
+Version: 0.9.0
 Summary: Django REST Framework and SQLAlchemy integration
 Home-page: https://github.com/shosca/django-rest-witchcraft
 Author: Serkan Hosca
 Author-email: serkan@hosca.com
 License: MIT
 Description: Django REST Witchcraft
         ======================
         
-        |Build Status| |Read The Docs| |PyPI version| |Coveralls Status|
+        |Build Status| |Read The Docs| |PyPI version| |Coveralls Status| |Black|
         
         **Django REST Framework integration with SQLAlchemy**
         
         django-rest-witchcraft is an extension for Django REST Framework that adds support for SQLAlchemy. It aims to provide
         a similar development experience to building REST api's with Django REST Framework with Django ORM, except with
         SQLAlchemy.
         
@@ -173,15 +173,15 @@
         .. code:: python
         
             group = Group(name='Admin')
             session.add(group)
             session.flush()
         
             serializer = UserSerializer(user, data={
-                'group': {'id': group.id
+                'group': {'id': group.id}
             })
             serializer.is_valid()
             serializer.save()
         
             user = serializer.instance
         
         Now, our user looks like:
@@ -255,18 +255,20 @@
            :target: https://travis-ci.org/shosca/django-rest-witchcraft
         .. |Read The Docs| image:: https://readthedocs.org/projects/django-rest-witchcraft/badge/?version=latest
            :target: http://django-rest-witchcraft.readthedocs.io/en/latest/?badge=latest
         .. |PyPI version| image:: https://badge.fury.io/py/django-rest-witchcraft.svg
            :target: https://badge.fury.io/py/django-rest-witchcraft
         .. |Coveralls Status| image:: https://coveralls.io/repos/github/shosca/django-rest-witchcraft/badge.svg?branch=master
            :target: https://coveralls.io/github/shosca/django-rest-witchcraft?branch=master
+        .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+           :target: https://github.com/ambv/black
         
 Keywords: sqlalchemy django rest framework drf rest_framework
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `django-rest-witchcraft-0.8.3/django_rest_witchcraft.egg-info/SOURCES.txt` & `django-rest-witchcraft-0.9.0/django_rest_witchcraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/field_mapping.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/field_mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 """
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 import datetime
 import decimal
 
 import six
-from rest_framework import fields
 
 from sqlalchemy.dialects import postgresql
 from sqlalchemy.sql import sqltypes
 
 from django_sorcery.db import meta
 
-from .fields import CharMappingField, EnumField
+from rest_framework import fields
+
+from rest_enumfield import EnumField
+
+from .fields import CharMappingField
 
 
 def get_detail_view_name(model):
     """
     Given a model class, return the view name to use for URL relationships
     that rever to instances of the model.
     """
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/fields.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/fields.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 """
 Some SQLAlchemy specific field types.
 """
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
 import six
-from rest_framework import fields, relations
 
 from django.db.models.constants import LOOKUP_SEP
 
 from django_sorcery.db import meta
-from django_sorcery.utils import suppress
+
+from rest_framework import fields, relations
 
 
 class HyperlinkedIdentityField(relations.HyperlinkedIdentityField):
     def get_url(self, obj, view_name, request, format):
         info = meta.model_info(obj.__class__)
 
         # Unsaved objects will not yet have a valid URL.
@@ -38,45 +38,14 @@
     def get_url(self, obj, view_name, request, format):
         """
         Same as basic HyperlinkedIdentityField except return uri vs full url.
         """
         return super(UriField, self).get_url(obj, view_name, None, format)
 
 
-class EnumField(fields.ChoiceField):
-    """
-    Used for SQLAlchemy's Enum column type used in either mapping python Enum's, or
-    a list of valid fields for the column.
-    """
-
-    def __init__(
-        self, enum_class=None, choices=None, to_choice=lambda x: (x.name, x.value), to_repr=lambda x: x.name, **kwargs
-    ):
-        self.enum_class = enum_class or choices
-        self.to_repr = to_repr
-        self.to_choice = to_choice
-        kwargs["choices"] = [to_choice(e) for e in self.enum_class]
-        kwargs.pop("max_length", None)
-        super(EnumField, self).__init__(**kwargs)
-
-    def to_internal_value(self, data):
-        with suppress(KeyError, ValueError):
-            return self.enum_class[data]
-        with suppress(KeyError, ValueError):
-            return self.enum_class(data)
-
-        self.fail("invalid_choice", input=data)
-
-    def to_representation(self, value):
-        if not value:
-            return None
-
-        return self.to_repr(value)
-
-
 class CharMappingField(fields.DictField):
     """
     Used for Postgresql HSTORE columns for storing key-value pairs.
     """
 
     child = fields.CharField(allow_null=True)
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/generics.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/generics.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
-from rest_framework import generics
-
 from sqlalchemy.exc import InvalidRequestError
 
 from django.http import Http404
 
 from django_sorcery.db.meta import model_info
 from django_sorcery.utils import suppress
 
+from rest_framework import generics
+
 
 class GenericAPIView(generics.GenericAPIView):
     """
     Base class for sqlalchemy specific views
     """
 
     @classmethod
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/mixins.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 from itertools import chain
 
 import six
-from rest_framework import mixins
 
 from sqlalchemy import orm
 
 from django.db.models.constants import LOOKUP_SEP
 
 from django_sorcery.db import meta
 
+from rest_framework import mixins
+
 
 class DestroyModelMixin(mixins.DestroyModelMixin):
     """
     Deletes a model instance
     """
 
     def perform_destroy(self, instance):
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/routers.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/routers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
-from rest_framework import routers
-
 from django_sorcery.db import meta
 
+from rest_framework import routers
+
 
 class DefaultRouter(routers.DefaultRouter):
     def get_default_base_name(self, viewset):
 
         model = getattr(viewset, "get_model", lambda: None)()
 
         assert model is not None, (
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/serializers.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 from __future__ import absolute_import, print_function, unicode_literals
 import copy
 import re
 from collections import OrderedDict, namedtuple
 from itertools import groupby
 
 import six
-from rest_framework import fields, serializers
-from rest_framework.exceptions import ValidationError
-from rest_framework.settings import api_settings
 
 from sqlalchemy.orm.interfaces import ONETOMANY
 
 from django.core.exceptions import ImproperlyConfigured, ValidationError as DjangoValidationError
 from django.db.models.constants import LOOKUP_SEP
 from django.http import QueryDict
 from django.utils.text import capfirst
 
 from django_sorcery.db import meta
 
+from rest_framework import fields, serializers
+from rest_framework.exceptions import ValidationError
+from rest_framework.settings import api_settings
+
 from .field_mapping import get_field_type, get_url_kwargs
 from .fields import ImplicitExpandableListField, UriField
 from .utils import django_to_drf_validation_error
 
 
 ALL_FIELDS = "__all__"
 REGEX_TYPE = type(re.compile(""))
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/utils.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
+from django.core.exceptions import NON_FIELD_ERRORS, ValidationError as DjangoValidationError
+
 from rest_framework.serializers import ValidationError
 from rest_framework.settings import api_settings
 
-from django.core.exceptions import NON_FIELD_ERRORS, ValidationError as DjangoValidationError
-
 
 def _django_to_drf(e):
     if hasattr(e, "error_dict") or isinstance(e, dict):
         return {
             k if not k == NON_FIELD_ERRORS else api_settings.NON_FIELD_ERRORS_KEY: _django_to_drf(v)
             for k, v in getattr(e, "error_dict", e).items()
         }
```

### Comparing `django-rest-witchcraft-0.8.3/rest_witchcraft/viewsets.py` & `django-rest-witchcraft-0.9.0/rest_witchcraft/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-rest-witchcraft-0.8.3/setup.py` & `django-rest-witchcraft-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,24 +32,24 @@
     os.system("make clean")
     sys.exit()
 
 setup(
     author=about["__author__"],
     author_email=about["__author_email__"],
     description=about["__description__"],
-    install_requires=["djangorestframework", "six", "django-sorcery"],
+    install_requires=["djangorestframework", "six", "django-sorcery", "django-rest-enumfield"],
     license="MIT",
     long_description=read("README.rst"),
     name="django-rest-witchcraft",
     packages=find_packages(exclude=["tests"]),
     url="https://github.com/shosca/django-rest-witchcraft",
     version=about["__version__"],
     keywords="sqlalchemy django rest framework drf rest_framework",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django :: 1.11",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `django-rest-witchcraft-0.8.3/tests/models.py` & `django-rest-witchcraft-0.9.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-rest-witchcraft-0.8.3/tests/models_composite.py` & `django-rest-witchcraft-0.9.0/tests/models_composite.py`

 * *Files identical despite different names*

### Comparing `django-rest-witchcraft-0.8.3/tests/test_field_mapping.py` & `django-rest-witchcraft-0.9.0/tests/test_field_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
-from rest_framework import fields
-from rest_witchcraft import field_mapping
-from rest_witchcraft.fields import CharMappingField, EnumField
-
 import sqlalchemy as sqa
 from sqlalchemy.dialects import postgresql
 
 from django.test import SimpleTestCase
 
+from rest_framework import fields
+
+from rest_enumfield import EnumField
+
+from rest_witchcraft import field_mapping
+from rest_witchcraft.fields import CharMappingField
+
 from .models import Owner
 
 
 class TestModelViewName(SimpleTestCase):
     def test_get_detail_view_name(self):
 
         name = field_mapping.get_detail_view_name(EnumField)
```

### Comparing `django-rest-witchcraft-0.8.3/tests/test_generics.py` & `django-rest-witchcraft-0.9.0/tests/test_generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
-from rest_framework.test import APIRequestFactory
-from rest_witchcraft import serializers, viewsets
-
 from sqlalchemy import Column, create_engine, orm, types
 from sqlalchemy.ext.declarative import declarative_base
 
 from django.http import Http404
 from django.test import SimpleTestCase
 
+from rest_framework.test import APIRequestFactory
+
+from rest_witchcraft import serializers, viewsets
+
 
 factory = APIRequestFactory()
 
 engine = create_engine("sqlite://")
 session = orm.scoped_session(orm.sessionmaker(bind=engine))
 Base = declarative_base()
 Base.query = session.query_property()
```

### Comparing `django-rest-witchcraft-0.8.3/tests/test_mixins.py` & `django-rest-witchcraft-0.9.0/tests/test_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
 import six
+
+from sqlalchemy.orm import joinedload
+
+from django.test import SimpleTestCase
+
 from rest_framework.fields import IntegerField
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.test import APIRequestFactory
 from rest_framework.viewsets import GenericViewSet, ModelViewSet
+
 from rest_witchcraft.mixins import ExpandableQuerySerializerMixin
 from rest_witchcraft.serializers import ExpandableModelSerializer, ModelSerializer
 
-from sqlalchemy.orm import joinedload
-
-from django.test import SimpleTestCase
-
 from .models import Vehicle, session
 from .test_routers import UnAuthMixin
 
 
 class DummySerializer(ModelSerializer):
     class Meta(object):
         session = session
```

### Comparing `django-rest-witchcraft-0.8.3/tests/test_routers.py` & `django-rest-witchcraft-0.9.0/tests/test_routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 
 import simplejson as json
-from rest_witchcraft import routers, serializers, viewsets
 
 from django.conf.urls import include, url
 from django.test import SimpleTestCase, override_settings
 
+from rest_witchcraft import routers, serializers, viewsets
+
 from .models_composite import RouterTestCompositeKeyModel, RouterTestModel, session
 
 
 class RouterTestModelSerializer(serializers.ModelSerializer):
     class Meta:
         model = RouterTestModel
         session = session
```

### Comparing `django-rest-witchcraft-0.8.3/tests/test_serializers.py` & `django-rest-witchcraft-0.9.0/tests/test_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 import copy
 from collections import OrderedDict
 from decimal import Decimal
 
+from django.core.exceptions import ImproperlyConfigured, ValidationError as DjangoValidationError
+from django.test import SimpleTestCase
+
+from django_sorcery.db.meta import model_info
+
 from rest_framework import fields
 from rest_framework.exceptions import ErrorDetail, ValidationError
 from rest_framework.serializers import ListSerializer, Serializer
 from rest_framework.settings import api_settings
 from rest_framework.test import APIRequestFactory
+
 from rest_witchcraft.fields import HyperlinkedIdentityField
 from rest_witchcraft.serializers import BaseSerializer, CompositeSerializer, ExpandableModelSerializer, ModelSerializer
 
-from django.core.exceptions import ImproperlyConfigured, ValidationError as DjangoValidationError
-from django.test import SimpleTestCase
-
-from django_sorcery.db.meta import model_info
-
 from .models import COLORS, Engine, ModelWithJson, Option, Owner, Vehicle, VehicleOther, VehicleType, session
 
 
 class VehicleOwnerStubSerializer(Serializer):
     id = fields.IntegerField(source="_owner_id")
```

### Comparing `django-rest-witchcraft-0.8.3/tests/test_utils.py` & `django-rest-witchcraft-0.9.0/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, print_function, unicode_literals
 import unittest
 
-from rest_witchcraft.utils import _django_to_drf
-
 from django.core.exceptions import ValidationError
 
+from rest_witchcraft.utils import _django_to_drf
+
 
 class TestUtils(unittest.TestCase):
     def test_django_to_drf(self):
         self.assertEqual(_django_to_drf("hello"), "hello")
         self.assertEqual(_django_to_drf(["hello"]), ["hello"])
         self.assertEqual(_django_to_drf({"hello": "world"}), {"hello": "world"})
         self.assertEqual(_django_to_drf(ValidationError("hello")), ["hello"])
```

