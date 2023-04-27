# Comparing `tmp/m3-django-composite-foreignkey-1.0.2.tar.gz` & `tmp/m3-django-composite-foreignkey-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-django-composite-foreignkey-1.0.2.tar", last modified: Tue Jul 19 06:40:54 2022, max compression
+gzip compressed data, was "m3-django-composite-foreignkey-1.0.3.tar", last modified: Thu Apr 27 08:17:52 2023, max compression
```

## Comparing `m3-django-composite-foreignkey-1.0.2.tar` & `m3-django-composite-foreignkey-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 06:40:54.511083 m3-django-composite-foreignkey-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     3315 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    35141 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       60 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5955 2022-07-19 06:40:54.511083 m3-django-composite-foreignkey-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4576 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 06:40:54.508083 m3-django-composite-foreignkey-1.0.2/compositefk/
--rw-r--r--   0 root         (0) root         (0)       70 2022-07-19 06:40:42.000000 m3-django-composite-foreignkey-1.0.2/compositefk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      685 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/compositefk/compat.py
--rw-r--r--   0 root         (0) root         (0)    15499 2022-07-19 06:40:42.000000 m3-django-composite-foreignkey-1.0.2/compositefk/fields.py
--rw-r--r--   0 root         (0) root         (0)     2112 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/compositefk/related_descriptors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 06:40:54.511083 m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5955 2022-07-19 06:40:53.000000 m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2022-07-19 06:40:54.000000 m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 06:40:53.000000 m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-29 12:30:22.000000 m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-19 06:40:54.000000 m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      266 2022-07-19 06:40:54.511083 m3-django-composite-foreignkey-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2143 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:17:52.287385 m3-django-composite-foreignkey-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     3315 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    35141 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       60 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5955 2023-04-27 08:17:52.287385 m3-django-composite-foreignkey-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4576 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:17:52.284385 m3-django-composite-foreignkey-1.0.3/compositefk/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 08:17:43.000000 m3-django-composite-foreignkey-1.0.3/compositefk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      685 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/compositefk/compat.py
+-rw-r--r--   0 root         (0) root         (0)    19211 2023-04-27 08:17:43.000000 m3-django-composite-foreignkey-1.0.3/compositefk/fields.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/compositefk/related_descriptors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:17:52.287385 m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5955 2023-04-27 08:17:52.000000 m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-27 08:17:52.000000 m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 08:17:52.000000 m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-29 12:30:22.000000 m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-27 08:17:52.000000 m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-27 08:17:52.288385 m3-django-composite-foreignkey-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2143 2022-03-29 12:30:07.000000 m3-django-composite-foreignkey-1.0.3/setup.py
```

### Comparing `m3-django-composite-foreignkey-1.0.2/CONTRIBUTING.rst` & `m3-django-composite-foreignkey-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `m3-django-composite-foreignkey-1.0.2/LICENSE` & `m3-django-composite-foreignkey-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `m3-django-composite-foreignkey-1.0.2/PKG-INFO` & `m3-django-composite-foreignkey-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-django-composite-foreignkey
-Version: 1.0.2
+Version: 1.0.3
 Summary: composite foreignkey support for django
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-django-composite-foreignkey
 Author: BARS Group
 Author-email: contact@xornot.fr
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: django composite foreignkey
 Classifier: Development Status :: 4 - Beta
```

### Comparing `m3-django-composite-foreignkey-1.0.2/README.rst` & `m3-django-composite-foreignkey-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `m3-django-composite-foreignkey-1.0.2/compositefk/compat.py` & `m3-django-composite-foreignkey-1.0.3/compositefk/compat.py`

 * *Files identical despite different names*

### Comparing `m3-django-composite-foreignkey-1.0.2/compositefk/fields.py` & `m3-django-composite-foreignkey-1.0.3/compositefk/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-from __future__ import (
-    absolute_import,
-    print_function,
-    unicode_literals,
-)
 
 import logging
 import operator
 from collections import (
     OrderedDict,
 )
+from dataclasses import (
+    dataclass,
+)
 from functools import (
     reduce,
     wraps,
 )
+from typing import (
+    List,
+)
 
 from compositefk.related_descriptors import (
     CompositeForwardManyToOneDescriptor,
 )
 from django.core import (
     checks,
 )
 from django.core.exceptions import (
     FieldDoesNotExist,
 )
 from django.db.models import (
+    DateField,
     FilteredRelation,
     Q,
 )
 from django.db.models.deletion import (
     Collector,
 )
 from django.db.models.fields.related import (
@@ -45,15 +44,14 @@
 )
 from django.utils.translation import (
     gettext_lazy as _,
 )
 
 
 logger = logging.getLogger(__name__)
-__author__ = 'darius.bernard'
 
 
 class CompositeForeignKey(ForeignObject):
     requires_unique_target = False
 
     def __init__(self, to, **kwargs):
         """
@@ -406,28 +404,82 @@
 
 class LocalFieldValue(CompositePart):
     """
     implicitly used, represent the value of a local field
     """
     is_local_field = True
 
+@dataclass
+class CompositeRelatedField:
+    """ Правило соответствия составного поля модели для уточняющей фильтрации
+    зависимых записей при удалении основных записей.
+    Например: Модель TaxesReestr(T) имеет составной ключ charge на модель InOutCharge(I) c отношением полей:
+    T.charge_id = I.id  и  T.period_date = I.period_date.  Например если есть необходимость при удалении записей из модели I
+    каскадно удалять записи из модели T с уточненной фильтрацией по полю period_date из I, следует в модели T определить
+    поле атрибут collector_extra_filter_fields = [CompositeRelatedField(composite_field=charge, related_fields=['period_date'])]
+    В related_fields указываются поля из модели Т, в которой определен составной ключ на модель I
+    """
+    slots = [
+        'composite_field', 'related_fields'
+    ]
+    # ссылка на составное поле
+    composite_field: CompositeForeignKey
+    # список названий полей в связанной модели
+    related_fields: List[str]
 
 class CompositeFKCollector(Collector):
     """ Специальный коллектор для партицированных моделей для поддержки каскадного удаления """
     def related_objects(self, related_model, related_fields, objs):
         """
         Переопределяет правило создания фильтра для подтягивания записей,
         ссылающихся на партицированную модель
         """
         field_filters = []
         for related_field in related_fields:
             if isinstance(related_field, CompositeForeignKey):
                 from_field_index = related_field.to_fields.index(related_model._meta.pk.name)
                 field_name = related_field.from_fields[from_field_index]
                 field_filters.append(Q(**{'%s__in' % field_name: [obj.pk for obj in objs]}))
+                self._extend_conditions(related_model, objs, field_filters)
             else:
                 field_name = related_field.name
                 field_filters.append(Q(**{'%s__in' % field_name: objs}))
 
-        predicate = reduce(operator.or_, field_filters)
+        predicate = reduce(operator.and_, field_filters)
 
         return related_model._base_manager.using(self.using).filter(predicate)
+
+    @staticmethod
+    def _extend_conditions(related_model, deleted_records, field_filters):
+        """
+        Дополнение уточняющей фильтрацией связанной внешней модели
+        Args:
+            related_model: связанная с удаляемыми данными модель
+            deleted_records: удаляемые данные
+            field_filters: дополняемый queryset фильтр для связанной модели
+        """
+        collector_extra_filter_fields = getattr(related_model, 'collector_extra_filter_fields', [])
+        for collector_extra_filter_field in collector_extra_filter_fields:
+            reverse_related_fields = related_model._meta.get_field(
+                collector_extra_filter_field.composite_field.attname
+            ).reverse_related_fields
+            # формирование списка соотношений поля удяляемых записей и поля зависимых записей
+            fields = [
+                (parent_field, related_field)
+                for parent_field, related_field in reverse_related_fields
+                if related_field.attname in collector_extra_filter_field.related_fields
+            ]
+            for parent_field, related_field in fields:
+                parent_values = {getattr(obj, parent_field.attname) for obj in deleted_records}
+                if isinstance(parent_field, DateField):
+                    # Для поля с типом Дата вычисляется диапазон дат из списка удаляемых объектов objs
+                    # FIXME Скорей всего можно обойтись без диапазона для даты, используя простое условие IN
+                    min_date = min(parent_values)
+                    max_date = max(parent_values)
+                    field_filters.append(
+                        Q(**{
+                            f'{related_field.attname}__gte': min_date,
+                            f'{related_field.attname}__lte': max_date,
+                        })
+                    )
+                else:
+                    field_filters.append(Q(**{f'{related_field.attname}__in': parent_values}))
```

### Comparing `m3-django-composite-foreignkey-1.0.2/compositefk/related_descriptors.py` & `m3-django-composite-foreignkey-1.0.3/compositefk/related_descriptors.py`

 * *Files identical despite different names*

### Comparing `m3-django-composite-foreignkey-1.0.2/m3_django_composite_foreignkey.egg-info/PKG-INFO` & `m3-django-composite-foreignkey-1.0.3/m3_django_composite_foreignkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-django-composite-foreignkey
-Version: 1.0.2
+Version: 1.0.3
 Summary: composite foreignkey support for django
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-django-composite-foreignkey
 Author: BARS Group
 Author-email: contact@xornot.fr
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: django composite foreignkey
 Classifier: Development Status :: 4 - Beta
```

### Comparing `m3-django-composite-foreignkey-1.0.2/setup.py` & `m3-django-composite-foreignkey-1.0.3/setup.py`

 * *Files identical despite different names*

