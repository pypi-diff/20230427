# Comparing `tmp/django-models-logging-2.2a0.tar.gz` & `tmp/django-models-logging-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-models-logging-2.2a0.tar", last modified: Thu Dec 29 08:43:08 2022, max compression
+gzip compressed data, was "django-models-logging-2.3.tar", last modified: Thu Apr 27 12:41:45 2023, max compression
```

## Comparing `django-models-logging-2.2a0.tar` & `django-models-logging-2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1066 2022-12-17 10:37:50.000000 django-models-logging-2.2a0/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)     1187 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     3279 2022-12-17 10:37:50.000000 django-models-logging-2.2a0/README.md
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/django_models_logging.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1187 2022-12-29 08:43:08.000000 django-models-logging-2.2a0/django_models_logging.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1315 2022-12-29 08:43:08.000000 django-models-logging-2.2a0/django_models_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2022-12-29 08:43:08.000000 django-models-logging-2.2a0/django_models_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       28 2022-12-29 08:43:08.000000 django-models-logging-2.2a0/django_models_logging.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       15 2022-12-29 08:43:08.000000 django-models-logging-2.2a0/django_models_logging.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/models_logging/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1880 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     9482 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/admin.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      335 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/apps.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2864 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/helpers.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.598554 django-models-logging-2.2a0/models_logging/management/
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/models_logging/management/commands/
--rw-rw-r--   0 legion    (1000) legion    (1000)        0 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/management/commands/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1182 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/management/commands/delete_changes.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1158 2022-12-28 15:14:17.000000 django-models-logging-2.2a0/models_logging/middleware.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/models_logging/migrations/
--rw-rw-r--   0 legion    (1000) legion    (1000)     3356 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0001_initial.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      595 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0002_auto_20161012_2025.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2995 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0003_auto_20170726_1552.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      510 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0004_auto_20171124_1445.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      945 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0005_auto_20200804_1305.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      443 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0006_auto_20211020_2036.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      490 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0007_migrate_old_fields.py
--rw-rw-r--   0 legion    (1000) legion    (1000)      566 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/0008_change_extras.py
--rw-rw-r--   0 legion    (1000) legion    (1000)        0 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/migrations/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     6325 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/models.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1272 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/settings.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1124 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/setup.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1333 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/signals.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.598554 django-models-logging-2.2a0/models_logging/templates/
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/models_logging/templates/models_logging/
--rw-rw-r--   0 legion    (1000) legion    (1000)      349 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/templates/models_logging/change_form.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     2837 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/templates/models_logging/object_history.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     1538 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/templates/models_logging/revert_changes_confirmation.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     2167 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/templates/models_logging/revert_revision_confirmation.html
--rw-rw-r--   0 legion    (1000) legion    (1000)     2929 2022-12-28 15:07:44.000000 django-models-logging-2.2a0/models_logging/utils.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2022-12-29 08:43:08.602554 django-models-logging-2.2a0/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1546 2022-12-29 08:40:19.000000 django-models-logging-2.2a0/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.889213 django-models-logging-2.3/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1066 2023-04-27 12:40:48.000000 django-models-logging-2.3/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1185 2023-04-27 12:41:45.885213 django-models-logging-2.3/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     3279 2023-04-27 12:40:48.000000 django-models-logging-2.3/README.md
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/django_models_logging.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1185 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1315 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       28 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       15 2023-04-27 12:41:45.000000 django-models-logging-2.3/django_models_logging.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1880 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     9573 2023-04-27 12:40:50.000000 django-models-logging-2.3/models_logging/admin.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      335 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/apps.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2864 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/helpers.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/management/
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/management/commands/
+-rw-rw-r--   0 legion    (1000) legion    (1000)        0 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/management/commands/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1182 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/management/commands/delete_changes.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1158 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/middleware.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/migrations/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     3356 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0001_initial.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      595 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0002_auto_20161012_2025.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2995 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0003_auto_20170726_1552.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      510 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0004_auto_20171124_1445.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      945 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/migrations/0005_auto_20200804_1305.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      443 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/0006_auto_20211020_2036.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      490 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/migrations/0007_migrate_old_fields.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)      566 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/migrations/0008_change_extras.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)        0 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/migrations/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     6563 2023-04-27 12:40:50.000000 django-models-logging-2.3/models_logging/models.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1272 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/settings.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1124 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/setup.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1333 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/signals.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/templates/
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-04-27 12:41:45.885213 django-models-logging-2.3/models_logging/templates/models_logging/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      349 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/templates/models_logging/change_form.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2824 2023-04-27 12:40:50.000000 django-models-logging-2.3/models_logging/templates/models_logging/object_history.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1538 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/templates/models_logging/revert_changes_confirmation.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2167 2023-01-05 14:55:39.000000 django-models-logging-2.3/models_logging/templates/models_logging/revert_revision_confirmation.html
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2929 2023-04-27 12:40:48.000000 django-models-logging-2.3/models_logging/utils.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-04-27 12:41:45.889213 django-models-logging-2.3/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1545 2023-04-27 12:40:50.000000 django-models-logging-2.3/setup.py
```

### Comparing `django-models-logging-2.2a0/LICENSE` & `django-models-logging-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/PKG-INFO` & `django-models-logging-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-models-logging
-Version: 2.2a0
+Version: 2.3
 Summary: Add logging of models from save, delete signals
 Home-page: https://github.com/legion-an/django-models-logging
 Author: legion
 Author-email: legion.andrey.89@gmail.com
 License: MIT
 Keywords: django logging,django history,django logging models,django history models
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-models-logging-2.2a0/README.md` & `django-models-logging-2.3/README.md`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/django_models_logging.egg-info/PKG-INFO` & `django-models-logging-2.3/django_models_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-models-logging
-Version: 2.2a0
+Version: 2.3
 Summary: Add logging of models from save, delete signals
 Home-page: https://github.com/legion-an/django-models-logging
 Author: legion
 Author-email: legion.andrey.89@gmail.com
 License: MIT
 Keywords: django logging,django history,django logging models,django history models
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-models-logging-2.2a0/django_models_logging.egg-info/SOURCES.txt` & `django-models-logging-2.3/django_models_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/__init__.py` & `django-models-logging-2.3/models_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/admin.py` & `django-models-logging-2.3/models_logging/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,23 @@
     list_select_related = ('user', 'content_type')
 
     def get_comment(self, obj):
         return '%s: %s' % (obj.action, obj.object_repr)
 
     def get_link_admin_object(self, obj):
         try:
-            if obj.object and obj.content_type.model_class() in admin.site._registry:
-                return format_html('<a href="%s">%s</a>' % (
-                    reverse('admin:%s_%s_change' % (obj.content_type.app_label, obj.content_type.model),
+            if obj.object_id and obj.content_type.model_class() in admin.site._registry:
+                return format_html(
+                    '<a href="%s">%s</a>' % (
+                        reverse(
+                            'admin:%s_%s_change' % (obj.content_type.app_label, obj.content_type.model),
                             args=[obj.object_id]
-                    ),
-                    obj.object)
+                        ),
+                        obj.object_repr
+                    )
                 )
         except AttributeError:
             return None
 
     def has_add_permission(self, request, *args, **kwargs):
         return
```

### Comparing `django-models-logging-2.2a0/models_logging/helpers.py` & `django-models-logging-2.3/models_logging/helpers.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/management/commands/delete_changes.py` & `django-models-logging-2.3/models_logging/management/commands/delete_changes.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/middleware.py` & `django-models-logging-2.3/models_logging/middleware.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/migrations/0001_initial.py` & `django-models-logging-2.3/models_logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/migrations/0002_auto_20161012_2025.py` & `django-models-logging-2.3/models_logging/migrations/0002_auto_20161012_2025.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/migrations/0003_auto_20170726_1552.py` & `django-models-logging-2.3/models_logging/migrations/0003_auto_20170726_1552.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/migrations/0005_auto_20200804_1305.py` & `django-models-logging-2.3/models_logging/migrations/0005_auto_20200804_1305.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/migrations/0008_change_extras.py` & `django-models-logging-2.3/models_logging/migrations/0008_change_extras.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/models.py` & `django-models-logging-2.3/models_logging/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 
-from .settings import ADDED, CHANGED, DELETED, LOGGING_USER_MODEL, JSON_ENCODER_PATH
-
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.utils.module_loading import import_string
-
 from django.db import models, transaction
+from django.db.models.functions import Cast
 from django.urls import reverse
+from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 from six import python_2_unicode_compatible
 
+from .settings import ADDED, CHANGED, DELETED, LOGGING_USER_MODEL, JSON_ENCODER_PATH
+
 
 def get_encoder(*args, **kwargs):
     encoder_cls = import_string(JSON_ENCODER_PATH)
     return encoder_cls(*args, **kwargs)
 
 
 @python_2_unicode_compatible
@@ -97,26 +97,31 @@
         for rel_model in related_objects:
             if isinstance(rel_model, models.OneToOneRel):
                 try:
                     values = [getattr(obj, rel_model.get_accessor_name()).pk]
                 except rel_model.related_model.DoesNotExist:
                     continue
             elif isinstance(rel_model, models.ManyToOneRel):
-                values = getattr(obj, rel_model.get_accessor_name()).all().values_list('pk', flat=True)
+                values = getattr(obj, rel_model.get_accessor_name()).annotate(
+                    pk_str=Cast('pk', output_field=models.TextField())
+                ).values_list('pk_str', flat=True)
             elif isinstance(rel_model, models.ForeignKey):
                 values = [getattr(obj, rel_model.get_attname())]
             elif isinstance(rel_model, models.ManyToManyField):
-                values = getattr(obj, rel_model.get_attname()).all().values_list('pk', flat=True)
+                values = getattr(obj, rel_model.get_attname()).annotate(
+                    pk_str=Cast('pk', output_field=models.TextField())
+                ).values_list('pk_str', flat=True)
             else:
                 continue
 
             history_objects.append(
                 {'content_type_id': ContentType.objects.get_for_model(rel_model.related_model).id,
                  'values': values}
             )
+
         qobj = models.Q()
         for v in history_objects:
             qobj.add(models.Q(content_type_id=v['content_type_id'], object_id__in=v['values']), models.Q.OR)
         return Change.objects.filter(qobj).select_related('user')
 
     def revert(self):
         with transaction.atomic():
```

### Comparing `django-models-logging-2.2a0/models_logging/settings.py` & `django-models-logging-2.3/models_logging/settings.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/setup.py` & `django-models-logging-2.3/models_logging/setup.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/signals.py` & `django-models-logging-2.3/models_logging/signals.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/templates/models_logging/object_history.html` & `django-models-logging-2.3/models_logging/templates/models_logging/object_history.html`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                                     <a href="{% url 'admin:models_logging_change_change' change.id %}">{{ change.date_created|date:"DATETIME_FORMAT"}}</a>
                                   {% else %}
                                     {{ change.date_created|date:"DATETIME_FORMAT"}}
                                   {% endif %}
                                 </th>
                                 <td>
                                     {% if change.user %}
-                                        {{ change.user.get_username }}
+                                        {{ change.user }}
                                         {% if change.user.get_full_name %} ({{ change.user.get_full_name }}){% endif %}
                                     {% else %}
                                         &mdash;
                                     {% endif %}
                                 </td>
                                 <td>
                                     {{ change.object_repr }}
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 {% extends "admin/object_history.html" %} {% load i18n %} {% block content %}
 {% blocktrans %}Choose a date from the list below to revert to a previous
 version of this object.{% endblocktrans %}
 {% if changes %}
-{% trans 'Date/time' %}   {% trans 'User' %}                                         {% trans 'Object'  {% trans      {% trans 'Changed data' %}
-                                                                                     %}                 'Action' %}
+{% trans 'Date/time' %}   {% trans 'User' %}                                                         {% trans 'Object'  {% trans      {% trans 'Changed data' %}
+                                                                                                     %}                 'Action' %}
 {% if changes_admin %} {
-{                                                                                                                     {% for field, values in
-change.date_created|date:                                                            {                  {             change.display_changed_data.items
-"DATETIME_FORMAT"}} {%    {% if change.user %} {{ change.user.get_username }} {% if  {                  {             %}
-else %} {                 change.user.get_full_name %} ({{ change.user.get_full_name change.object_repr change.action {{ field }}: {{ values.old }} ->
-{                         }}){% endif %} {% else %} — {% endif %}                  }}                 }}            {{ values.new }}
-change.date_created|date:                                                                                             {% endfor %}
+{                                                                                                                                     {% for field, values in
+change.date_created|date:                                                                            {                  {             change.display_changed_data.items
+"DATETIME_FORMAT"}} {%    {% if change.user %} {{ change.user }} {% if change.user.get_full_name %}  {                  {             %}
+else %} {                 ({{ change.user.get_full_name }}){% endif %} {% else %} — {% endif %}    change.object_repr change.action {{ field }}: {{ values.old }} ->
+{                                                                                                    }}                 }}            {{ values.new }}
+change.date_created|date:                                                                                                             {% endfor %}
 "DATETIME_FORMAT"}} {%
 endif %}
 {% else %}
 {% trans "This object doesn't have a change history. It probably wasn't added
 via this admin site." %}
 {% endif %}
 {% endblock %}
```

### Comparing `django-models-logging-2.2a0/models_logging/templates/models_logging/revert_changes_confirmation.html` & `django-models-logging-2.3/models_logging/templates/models_logging/revert_changes_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/templates/models_logging/revert_revision_confirmation.html` & `django-models-logging-2.3/models_logging/templates/models_logging/revert_revision_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/models_logging/utils.py` & `django-models-logging-2.3/models_logging/utils.py`

 * *Files identical despite different names*

### Comparing `django-models-logging-2.2a0/setup.py` & `django-models-logging-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 files = ["templates/models_logging/*", "migrations/*", "management/commands/*"]
 
 setup(
     name='django-models-logging',
-    version='2.2a',
+    version='2.3',
     packages=['models_logging'],
     url='https://github.com/legion-an/django-models-logging',
     package_data={'models_logging' : files},
     license='MIT',
     author='legion',
     author_email='legion.andrey.89@gmail.com',
     description='Add logging of models from save, delete signals',
```

