# Comparing `tmp/Meringue-0.3a6.tar.gz` & `tmp/meringue-0.4.0b1.dev17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Meringue-0.3a6.tar", last modified: Sun Jul 13 22:08:12 2014, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `Meringue-0.3a6.tar` & `meringue-0.4.0b1.dev17.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/Meringue.egg-info/
--rw-r--r--   0 dd        (1000) dd        (1000)       47 2014-07-13 22:08:12.000000 Meringue-0.3a6/Meringue.egg-info/requires.txt
--rw-r--r--   0 dd        (1000) dd        (1000)      969 2014-07-13 22:08:12.000000 Meringue-0.3a6/Meringue.egg-info/SOURCES.txt
--rw-r--r--   0 dd        (1000) dd        (1000)     4131 2014-07-13 22:08:12.000000 Meringue-0.3a6/Meringue.egg-info/PKG-INFO
--rw-r--r--   0 dd        (1000) dd        (1000)        1 2014-07-13 22:08:12.000000 Meringue-0.3a6/Meringue.egg-info/dependency_links.txt
--rw-r--r--   0 dd        (1000) dd        (1000)        9 2014-07-13 22:08:12.000000 Meringue-0.3a6/Meringue.egg-info/top_level.txt
--rw-r--r--   0 dd        (1000) dd        (1000)        1 2014-07-13 22:01:34.000000 Meringue-0.3a6/Meringue.egg-info/zip-safe
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/
--rw-r--r--   0 dd        (1000) dd        (1000)      190 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/context_processors.py
--rw-r--r--   0 dd        (1000) dd        (1000)     2140 2014-07-13 21:40:28.000000 Meringue-0.3a6/meringue/fields.py
--rw-r--r--   0 dd        (1000) dd        (1000)     3570 2014-07-13 21:39:25.000000 Meringue-0.3a6/meringue/widgets.py
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/utils/
--rw-r--r--   0 dd        (1000) dd        (1000)      167 2014-07-13 21:40:16.000000 Meringue-0.3a6/meringue/utils/admin.py
--rw-r--r--   0 dd        (1000) dd        (1000)      126 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/utils/__init__.py
--rw-r--r--   0 dd        (1000) dd        (1000)     1038 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/utils/urls.py
--rw-r--r--   0 dd        (1000) dd        (1000)     6842 2014-07-13 21:40:10.000000 Meringue-0.3a6/meringue/utils/thumbnails.py
--rw-r--r--   0 dd        (1000) dd        (1000)      165 2014-07-13 22:07:51.000000 Meringue-0.3a6/meringue/__init__.py
--rw-r--r--   0 dd        (1000) dd        (1000)      784 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/upload_handlers.py
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/templates/
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/templates/wo_nucleum/
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/templates/wo_nucleum/edit_inline/
--rw-r--r--   0 dd        (1000) dd        (1000)     3911 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/templates/wo_nucleum/edit_inline/gallery.html
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/templates/admin/
--rw-r--r--   0 dd        (1000) dd        (1000)      833 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/templates/admin/filter.html
--rw-r--r--   0 dd        (1000) dd        (1000)        0 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/templates/robots.txt
--rw-r--r--   0 dd        (1000) dd        (1000)      664 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/templates/404.html
--rw-r--r--   0 dd        (1000) dd        (1000)      640 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/templates/500.html
--rw-r--r--   0 dd        (1000) dd        (1000)     1154 2014-07-13 21:40:23.000000 Meringue-0.3a6/meringue/middleware.py
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/templatetags/
--rw-r--r--   0 dd        (1000) dd        (1000)        0 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/templatetags/__init__.py
--rw-r--r--   0 dd        (1000) dd        (1000)     2516 2014-07-13 21:40:20.000000 Meringue-0.3a6/meringue/templatetags/thumbnails.py
--rw-r--r--   0 dd        (1000) dd        (1000)      613 2014-07-13 21:40:18.000000 Meringue-0.3a6/meringue/templatetags/weboven_base.py
--rw-r--r--   0 dd        (1000) dd        (1000)      817 2014-07-13 21:40:56.000000 Meringue-0.3a6/meringue/settings.py
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/static/
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/static/css/
--rw-r--r--   0 dd        (1000) dd        (1000)     1266 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/static/css/inline-gallery.css
--rw-r--r--   0 dd        (1000) dd        (1000)     1106 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/static/css/reset.css
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/static/js/
--rw-r--r--   0 dd        (1000) dd        (1000)    83615 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/static/js/jquery-2.1.0.min.js
-drwxr-xr-x   0 dd        (1000) dd        (1000)        0 2014-07-13 22:08:12.000000 Meringue-0.3a6/meringue/static/images/
--rw-r--r--   0 dd        (1000) dd        (1000)       43 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/static/images/none.gif
--rw-r--r--   0 dd        (1000) dd        (1000)    11594 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/static/images/noise.png
--rw-r--r--   0 dd        (1000) dd        (1000)     4310 2014-07-13 16:41:17.000000 Meringue-0.3a6/meringue/models.py
--rw-r--r--   0 dd        (1000) dd        (1000)      190 2014-07-13 21:44:06.000000 Meringue-0.3a6/MANIFEST.in
--rw-r--r--   0 dd        (1000) dd        (1000)     1496 2014-07-13 22:00:08.000000 Meringue-0.3a6/setup.py
--rw-r--r--   0 dd        (1000) dd        (1000)     4131 2014-07-13 22:08:12.000000 Meringue-0.3a6/PKG-INFO
--rw-r--r--   0 dd        (1000) dd        (1000)       59 2014-07-13 22:08:12.000000 Meringue-0.3a6/setup.cfg
--rw-r--r--   0 dd        (1000) dd        (1000)     2444 2014-07-13 21:38:28.000000 Meringue-0.3a6/README.rst
--rw-r--r--   0 dd        (1000) dd        (1000)    35146 2014-07-13 15:23:48.000000 Meringue-0.3a6/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/__init__.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/fields.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/forms.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/middleware.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/widgets.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/admin/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/admin/apps.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/admin/static/css/inline-gallery.css
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/admin/static/images/noise.png
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/admin/static/images/none.gif
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/admin/templates/admin/filter.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/apps.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/decorators.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/errors.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/managers.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/models.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/options.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/query.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/translation.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/views.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/static/css/inline-gallery.css
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/static/css/reset.css
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/static/css/reset.min.css
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/static/images/noise.png
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/static/images/none.gif
+-rw-r--r--   0        0        0    83615 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/static/js/jquery-2.1.0.min.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templates/404.html
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templates/500.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templates/robots.txt
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templates/meringue/edit_inline/gallery.html
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templates/rest_framework/base.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/templatetags/meringue_thumbnails.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/utils/paginator.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/utils/unify.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/utils/thumbnails/__init__.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/utils/thumbnails/methods.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/meringue/core/utils/thumbnails/properties.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/AUTHORS
+-rw-r--r--   0        0        0    35146 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/LICENSE
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/README.md
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/pyproject.toml
+-rw-r--r--   0        0        0    44731 2020-02-02 00:00:00.000000 meringue-0.4.0b1.dev17/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Meringue-0.3a6/meringue/fields.py` & `meringue-0.4.0b1.dev17/meringue/fields.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import mimetypes
 
 from django import forms
 from django.core.files.images import ImageFile, get_image_dimensions
 from django.db.models.fields.files import FieldFile, ImageField
 
-from south.modelsinspector import add_introspection_rules
+from . import widgets as self_widgets
 
 
 class UploadFieldFile(ImageFile, FieldFile):
 
     def save(self, name, content, save=True):
         type, format = self.mime()
         if type == 'image' and format in ('jpeg', 'png', 'gif', 'tiff'):
@@ -47,18 +47,18 @@
 class UploadField(ImageField):
 
     attr_class = UploadFieldFile
 
     def formfield(self, **kwargs):
         defaults = {'form_class': forms.FileField}
         defaults.update(kwargs)
-        return super(ImageField, self).formfield(**defaults)
-        # return super(UploadField, self).formfield(**defaults)
-add_introspection_rules([], ["^meringue\.fields\.UploadField"])
+        return super(UploadField, self).formfield(**defaults)
+        # return super(ImageField, self).formfield(**defaults)
+        # what?
 
 
 class PreviewImageField(ImageField):
 
     def formfield(self, **kwargs):
-        kwargs['widget'] = PreviewImageFileInput
+        kwargs['widget'] = self_widgets.PreviewImageFileInput
         defaults = kwargs
         return super(PreviewImageField, self).formfield(**defaults)
```

### Comparing `Meringue-0.3a6/meringue/widgets.py` & `meringue-0.4.0b1.dev17/meringue/widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding:utf-8 -*-
 
 from django import forms
-from django.db import models
 from django.utils.encoding import force_text
 from django.utils.html import conditional_escape, format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
-from meringue.utils.thumbnails import get_thumbnail
+from .utils.thumbnails import get_thumbnail
 
 
 class PreviewImageFileInput(forms.widgets.FileInput):
     '''
     TO-DO:
         информация о изображении
         изображение при инициализации
```

### Comparing `Meringue-0.3a6/meringue/templates/wo_nucleum/edit_inline/gallery.html` & `meringue-0.4.0b1.dev17/meringue/core/templates/meringue/edit_inline/gallery.html`

 * *Files identical despite different names*

### Comparing `Meringue-0.3a6/meringue/templates/404.html` & `meringue-0.4.0b1.dev17/meringue/core/templates/500.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 {% extends "base.html" %}
 
 {% load static i18n %}
 
 
-{% block title %}{% trans 'ошибка' %} 404 :: {{ SITE_NAME }}{% endblock %}
+{% block title %}{% trans 'ошибка' %} 500 :: {{ SITE_NAME }}{% endblock %}
 
 {% block extrahead %}
-	<link type="text/css" rel="stylesheet" href="{% static 'css/weboven::main.css' %}" >
+	{# <link type="text/css" rel="stylesheet" href="{% static 'css/weboven::main.css' %}" > #}
 {% endblock %}
 
-{% block content %}<div class="error_list error404">
-	<p class="error_number_line" >{% trans 'ошибка' %} <span class="error_number" >404</span></p>
-	<p class="error_text" >такой страницы не существует, попробуйте начать <a href="/">сначала</a> или вернитесь <a href="{{ request.META.HTTP_REFERER }}">назад</a></p>
+{% block content %}<div class='error_list error500'>
+	<p class="error_number_line" >{% trans 'ошибка' %} <span class="error_number" >500</span></p>
+	<p class="error_text" >{% trans 'guru meditation' %}</p>
+	<p class="error_text" ><a href="/">{% trans 'на главную' %}</a> <a href="{{ request.META.HTTP_REFERER }}">{% trans 'назад' %}</a></p>
 </div>{% endblock %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% extends "base.html" %} {% load static i18n %} {% block title %}{% trans
-'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 404 :: {{ SITE_NAME }}{% endblock %} {% block extrahead %}
- {% endblock %} {% block content %}
-{% trans 'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 404
-ÑÐ°ÐºÐ¾Ð¹ ÑÑÑÐ°Ð½Ð¸ÑÑ Ð½Ðµ ÑÑÑÐµÑÑÐ²ÑÐµÑ, Ð¿Ð¾Ð¿ÑÐ¾Ð±ÑÐ¹ÑÐµ
-Ð½Ð°ÑÐ°ÑÑ ÑÐ½Ð°ÑÐ°Ð»Ð° Ð¸Ð»Ð¸ Ð²ÐµÑÐ½Ð¸ÑÐµÑÑ Ð½Ð°Ð·Ð°Ð´
+'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 500 :: {{ SITE_NAME }}{% endblock %} {% block extrahead %} {#
+ #} {% endblock %} {% block content %}
+{% trans 'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 500
+{% trans 'guru meditation' %}
+{%_trans_'Ð½Ð°_Ð³Ð»Ð°Ð²Ð½ÑÑ'_%} {%_trans_'Ð½Ð°Ð·Ð°Ð´'_%}
 {% endblock %}
```

### Comparing `Meringue-0.3a6/meringue/templates/500.html` & `meringue-0.4.0b1.dev17/meringue/core/templates/404.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 {% extends "base.html" %}
 
 {% load static i18n %}
 
 
-{% block title %}{% trans 'ошибка' %} 500 :: {{ SITE_NAME }}{% endblock %}
+{% block title %}{% trans 'ошибка' %} 404 :: {{ SITE_NAME }}{% endblock %}
 
 {% block extrahead %}
-	<link type="text/css" rel="stylesheet" href="{% static 'css/weboven::main.css' %}" >
+	{# <link type="text/css" rel="stylesheet" href="{% static 'css/weboven::main.css' %}" > #}
 {% endblock %}
 
-{% block content %}<div class='error_list error500'>
-	<p class="error_number_line" >{% trans 'ошибка' %} <span class="error_number" >500</span></p>
-	<p class="error_text" >{% trans 'guru meditation' %}</p>
-	<p class="error_text" ><a href="/">{% trans 'на главную' %}</a> <a href="{{ request.META.HTTP_REFERER }}">{% trans 'назад' %}</a></p>
+{% block content %}<div class="error_list error404">
+	<p class="error_number_line" >{% trans 'ошибка' %} <span class="error_number" >404</span></p>
+	<p class="error_text" >{% trans 'такой страницы не существует, попробуйте начать' %} <a href="/">{% trans 'сначала' %}</a> {% trans 'или вернитесь' %} <a href="{{ request.META.HTTP_REFERER }}">{% trans 'назад' %}</a></p>
 </div>{% endblock %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% extends "base.html" %} {% load static i18n %} {% block title %}{% trans
-'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 500 :: {{ SITE_NAME }}{% endblock %} {% block extrahead %}
- {% endblock %} {% block content %}
-{% trans 'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 500
-{% trans 'guru meditation' %}
-{%_trans_'Ð½Ð°_Ð³Ð»Ð°Ð²Ð½ÑÑ'_%} {%_trans_'Ð½Ð°Ð·Ð°Ð´'_%}
+'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 404 :: {{ SITE_NAME }}{% endblock %} {% block extrahead %} {#
+ #} {% endblock %} {% block content %}
+{% trans 'Ð¾ÑÐ¸Ð±ÐºÐ°' %} 404
+{% trans 'ÑÐ°ÐºÐ¾Ð¹ ÑÑÑÐ°Ð½Ð¸ÑÑ Ð½Ðµ ÑÑÑÐµÑÑÐ²ÑÐµÑ,
+Ð¿Ð¾Ð¿ÑÐ¾Ð±ÑÐ¹ÑÐµ Ð½Ð°ÑÐ°ÑÑ' %} {%_trans_'ÑÐ½Ð°ÑÐ°Ð»Ð°'_%} {% trans
+'Ð¸Ð»Ð¸ Ð²ÐµÑÐ½Ð¸ÑÐµÑÑ' %} {%_trans_'Ð½Ð°Ð·Ð°Ð´'_%}
 {% endblock %}
```

### Comparing `Meringue-0.3a6/meringue/middleware.py` & `meringue-0.4.0b1.dev17/meringue/middleware.py`

 * *Files identical despite different names*

### Comparing `Meringue-0.3a6/meringue/templatetags/thumbnails.py` & `meringue-0.4.0b1.dev17/meringue/core/templatetags/meringue_thumbnails.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from django.template import Library
 
-from meringue.utils.thumbnails import get_thumbnail
-
 
 register = Library()
 
 
 @register.filter
 def thumbnail(filename, args=''):
     '''
@@ -18,27 +16,30 @@
     s:600x400,resize,s:400x400,crop - сначала задас целевой размер изображения
     600x400, далее скукожит (или растянет изображение в зависимости от
     исходного и других параметров) до 600x400, потом установит новый целевой
     размер 400x400 и отрежет лишнее.
 
     Аргументы фильтра:
         s:<width>x<height> - указывает целевой размер изображения для
-            последующий фенуций
+            последующих функций
+        maxw:<width> - указывает максимальную ширину
         crop - изменения размера холста до последнего установленного
         resize - изменение размера изображения до последнего установленного
         q:<quality> - укажет качество конечного изображения 0-100
             (используется в последний момент при сохранении)
         c:<color> - цвет заливки для кропа в формате rgba
             (c:255 255 255 255)
-        rm:scale|inscribe|stretch - метод ресайза вписать в размер или
+        rm:cover|contain|stretch - метод ресайза вписать в размер или
             растянуть
         cm:left|center|rigth top|center|bottom - точка отсчёта для кропа
 
     TO-DO:
         watermark
         определение лица и использование в роли центра изображения
         указание максимальной ширины или высоты
         определение фокуса
     '''
 
+    from meringue.core.utils.thumbnails import get_thumbnail
+
     task_list = args.split(',')
     return get_thumbnail(filename=filename, task_list=task_list)
```

### Comparing `Meringue-0.3a6/meringue/static/css/inline-gallery.css` & `meringue-0.4.0b1.dev17/meringue/admin/static/css/inline-gallery.css`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,13 @@
 	font-family: inherit;
 	font-size: inherit;
 	font-style: inherit;
 	font-weight: inherit;
 }
 
 input,button,textarea,select {
-	*font-size: 100%;
+	font-size: 100%;
 }
 
 input {
 	background: -webkit-gradient(linear, left top, left bottom, from(#FFF), to(#FFF));
 }
```

### Comparing `Meringue-0.3a6/meringue/static/css/reset.css` & `meringue-0.4.0b1.dev17/meringue/core/static/css/reset.css`

 * *Files 16% similar despite different names*

```diff
@@ -69,9 +69,9 @@
 }
 
 input,button,textarea,select {
 	*font-size: 100%;
 }
 
 input {
-	background: -webkit-gradient(linear, left top, left bottom, from(#FFF), to(#FFF));
+	background: #fff; /*-webkit-gradient(linear, left top, left bottom, from(#FFF), to(#FFF));*/
 }
```

### Comparing `Meringue-0.3a6/meringue/static/js/jquery-2.1.0.min.js` & `meringue-0.4.0b1.dev17/meringue/core/static/js/jquery-2.1.0.min.js`

 * *Files identical despite different names*

### Comparing `Meringue-0.3a6/meringue/static/images/noise.png` & `meringue-0.4.0b1.dev17/meringue/admin/static/images/noise.png`

 * *Files identical despite different names*

### Comparing `Meringue-0.3a6/meringue/models.py` & `meringue-0.4.0b1.dev17/meringue/core/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,128 +1,122 @@
 # -*- coding: utf-8 -*-
 
-from django.conf import settings
+import logging  # noqa
+
+# from django.conf import settings
 from django.db import models
-from django.db.models.query import QuerySet
 from django.utils.translation import ugettext_lazy as _
-import django.db.models.options as options
 
-if 'django_hosts' in settings.INSTALLED_APPS:
-    from django_hosts.reverse import reverse_full
-else:
-    from django.core.urlresolvers import reverse
+# if 'django_hosts' in settings.INSTALLED_APPS:
+#     from django_hosts.resolvers import reverse
+# else:
+#     from django.urls import reverse
+
+from .managers import PublishManager
+# from meringue import configuration
 
 
-options.DEFAULT_NAMES = options.DEFAULT_NAMES + (
-    'host_name',
-    'view',
-    'reverse_args',
-)
+logger = logging.getLogger('meringue')
 
 
 ##########
 # mixins #
 ##########
 
-class GetAbsoluteUrlMixin(object):
-
-    '''
-        Миксин автоматизирующий получение абсолютного адреса
-        Для получения адреса использует стандартную функцию reverse (в
-    случае если установлен django_hosts то reverse_full)
-
-        При реверсе предполагается следующая схема:
-
-            * host_name - название верхнего модуля в нижнем регистре
-        (используется в случае установенного django_hosts)
-
-            * view - '<namespace>:<url_name>':
-                - namespace - название приложения приведённое к нижнему
-            регистру и точки заменённые на нижнее подчёркивание
-                - url_name - название класса приведённое к нижнему регистру
-            с приставкой '-detail'
-
-            * args - по умолчанию pk модели
-
-        При определении класса модели можно предустановить параметры:
-            * host_name - название целевого хоста (string)
-            * view - целевой url (string)
-            * reverse_args - список атрибутов модели (list)
-    '''
-
-    def _host_name(self):
-        if not hasattr(self._meta, 'host_name'):
-            module_name = self.__module__.split('.')[0]
-            module = __import__(module_name)
-            self._meta.host_name = getattr(module, 'host_name',
-                                           module_name.lower())
-        return self._meta.host_name
-
-    def _view(self):
-        if not hasattr(self._meta, 'view'):
-            namespace = self.__module__[:-7].lower().replace('.', '_')
-
-            cls = self.__class__.__name__.lower()
-            view = '%s-detail' % cls
-
-            self._meta.view = '%s:%s' % (namespace, view)
-        return self._meta.view
-
-    def _reverse_args(self):
-        reverse_args = getattr(self._meta, 'reverse_args', ['pk'])
-        return [getattr(self, key) for key in reverse_args]
+class CMTimeMixin(models.Model):
+    ctime = models.DateTimeField(auto_now_add=True)
+    mtime = models.DateTimeField(auto_now=True)
 
-    def get_absolute_url(self):
-        if 'django_hosts' in settings.INSTALLED_APPS:
-            return reverse_full(host=self._host_name(),
-                                view=self._view(),
-                                view_args=self._reverse_args())
-        return reverse(self._view(), args=self._reverse_args())
-
-
-#############
-# querysets #
-#############
-
-class PublishQuerySet(QuerySet):
-
-    def published(self, **kwargs):
-        return self.filter(is_published=True, **kwargs)
-
-
-############
-# managers #
-############
-
-class PublishManager(models.Manager):
-    use_for_related_fields = True
-
-    def get_query_set(self):
-        return PublishQuerySet(self.model)
+    class Meta:
+        abstract = True
 
-    def published(self, *args, **kwargs):
-        return self.get_query_set().published(*args, **kwargs)
 
+class SortingMixin(models.Model):
+    sorting = models.SmallIntegerField(verbose_name=_('Порядок'),
+                                       help_text=_('Порядок сортировки'),
+                                       default=0, )
+    class Meta:
+        ordering = ['sorting', ]
+        abstract = True
 
-##########
-# models #
-##########
 
-class PublishModel(GetAbsoluteUrlMixin, models.Model):
+# class GetAbsoluteUrlMixin(object):
 
-    '''
-        Абстрактная модель с признаком публикации (поле is_published)
-        менеджер имеет метод published() аналог стандартного filter() с
-    заранее указанными is_published=True
-        так же наследует GetAbsoluteUrlMixin
-    '''
+#     '''
+#         Примесь автоматизирующая получение абсолютного адреса
+#         Для получения адреса использует стандартную функцию reverse (в
+#     случае если установлен django_hosts то reverse_full)
+
+#         При реверсе предполагается следующая схема:
+
+#             * host_name - название верхнего модуля в нижнем регистре
+#         (используется в случае установенного django_hosts)
+
+#             * view - '<namespace>:<url_name>':
+#                 - namespace - название приложения приведённое к нижнему
+#             регистру и точки заменённые на нижнее подчёркивание
+#                 - url_name - название класса приведённое к нижнему регистру
+#             с приставкой '-detail'
+
+#             * args - по умолчанию pk модели
+
+#         При определении класса модели можно предустановить параметры:
+#             * host_name - название целевого хоста (string)
+#             * view - целевой url (string)
+#             * reverse_args - список атрибутов модели (list)
+#     '''
+
+#     def _host_name(self):
+#         if not hasattr(self._meta, 'host_name'):
+#             module_name = self.__module__.split('.')[0]
+#             module = __import__(module_name)
+#             self._meta.host_name = getattr(module, 'host_name',
+#                                            module_name.lower())
+#         return self._meta.host_name
+
+#     def _view(self):
+#         if not hasattr(self._meta, 'view'):
+#             namespace = self.__module__[:-7].lower().replace('.', '_')
+
+#             cls = self._meta.model_name
+#             view = '%s-detail' % cls
+
+#             self._meta.view = '%s:%s' % (namespace, view)
+#         return self._meta.view
+
+#     def _reverse_args(self):
+#         reverse_args = getattr(self._meta, 'reverse_args', ['pk'])
+#         return [getattr(self, key) for key in reverse_args]
+
+#     def get_absolute_url(self):
+#         reverse_args = {
+#             'viewname': self._view(),
+#             'args': self._reverse_args(),
+#         }
+#         if 'django_hosts' in settings.INSTALLED_APPS:
+#             reverse_args.update({
+#                 'host': self._host_name(),
+#                 'port': configuration.PORT,
+#             })
+#         return reverse(**reverse_args)
+
+
+###################
+# Abstract models #
+###################
+
+class PublishedBase(models.Model):
+    """
+        publish abstract model
+        managr has method published() like a filter()
+    """
 
     is_published = models.BooleanField(
-        verbose_name=_(u'публикация'),
-        help_text=_(u'Отображать/Скрыть'),
+        verbose_name=_('публикация'),
+        help_text=_('Отображать/Скрыть'),
         default=True,
         db_index=True,
     )
 
     objects = PublishManager()
 
     class Meta:
```

### Comparing `Meringue-0.3a6/LICENSE` & `meringue-0.4.0b1.dev17/LICENSE`

 * *Files identical despite different names*

