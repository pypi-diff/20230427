# Comparing `tmp/Meringue-0.3.4.tar.gz` & `tmp/meringue-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Meringue-0.3.4.tar", last modified: Sat Aug 22 20:45:31 2015, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `Meringue-0.3.4.tar` & `meringue-0.4.0.post1.tar`

### file list

```diff
@@ -1,59 +1,50 @@
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/
--rw-r--r--   0 dd         (501) staff       (20)     5630 2015-08-22 20:34:49.000000 Meringue-0.3.4/CHANGELOG.rst
--rw-r--r--   0 dd         (501) staff       (20)    35146 2015-08-17 21:37:49.000000 Meringue-0.3.4/LICENSE.txt
--rw-r--r--   0 dd         (501) staff       (20)      216 2015-08-17 21:37:49.000000 Meringue-0.3.4/MANIFEST.in
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/
--rw-r--r--   0 dd         (501) staff       (20)      285 2015-08-22 20:35:01.000000 Meringue-0.3.4/meringue/__init__.py
--rw-r--r--   0 dd         (501) staff       (20)      223 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/context_processors.py
--rw-r--r--   0 dd         (501) staff       (20)     1155 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/decorators.py
--rw-r--r--   0 dd         (501) staff       (20)      218 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/errors.py
--rw-r--r--   0 dd         (501) staff       (20)     2140 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/fields.py
--rw-r--r--   0 dd         (501) staff       (20)     2394 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/forms.py
--rw-r--r--   0 dd         (501) staff       (20)     1154 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/middleware.py
--rw-r--r--   0 dd         (501) staff       (20)     4503 2015-08-22 20:34:49.000000 Meringue-0.3.4/meringue/models.py
--rw-r--r--   0 dd         (501) staff       (20)     1483 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/settings.py
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/static/
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/static/css/
--rw-r--r--   0 dd         (501) staff       (20)     1265 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/static/css/inline-gallery.css
--rw-r--r--   0 dd         (501) staff       (20)     1116 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/static/css/reset.css
--rw-r--r--   0 dd         (501) staff       (20)      667 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/static/css/reset.min.css
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/static/images/
--rw-r--r--   0 dd         (501) staff       (20)    11594 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/static/images/noise.png
--rw-r--r--   0 dd         (501) staff       (20)       43 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/static/images/none.gif
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/static/js/
--rw-r--r--   0 dd         (501) staff       (20)    83615 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/static/js/jquery-2.1.0.min.js
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/templates/
--rw-r--r--   0 dd         (501) staff       (20)      726 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templates/404.html
--rw-r--r--   0 dd         (501) staff       (20)      646 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templates/500.html
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/templates/admin/
--rw-r--r--   0 dd         (501) staff       (20)      833 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templates/admin/filter.html
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/templates/meringue/
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/templates/meringue/edit_inline/
--rw-r--r--   0 dd         (501) staff       (20)     3911 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templates/meringue/edit_inline/gallery.html
--rw-r--r--   0 dd         (501) staff       (20)        0 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templates/robots.txt
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/templatetags/
--rw-r--r--   0 dd         (501) staff       (20)        0 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templatetags/__init__.py
--rw-r--r--   0 dd         (501) staff       (20)     2936 2015-08-22 20:34:49.000000 Meringue-0.3.4/meringue/templatetags/forms_utils_new.py
--rw-r--r--   0 dd         (501) staff       (20)     5764 2015-08-22 20:34:49.000000 Meringue-0.3.4/meringue/templatetags/meringue_base.py
--rw-r--r--   0 dd         (501) staff       (20)     2516 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/templatetags/thumbnails.py
--rw-r--r--   0 dd         (501) staff       (20)      797 2015-08-22 20:34:49.000000 Meringue-0.3.4/meringue/upload_handlers.py
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/meringue/utils/
--rw-r--r--   0 dd         (501) staff       (20)      159 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/utils/__init__.py
--rw-r--r--   0 dd         (501) staff       (20)      167 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/utils/admin.py
--rw-r--r--   0 dd         (501) staff       (20)     6886 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/utils/thumbnails.py
--rw-r--r--   0 dd         (501) staff       (20)      905 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/utils/unifying.py
--rw-r--r--   0 dd         (501) staff       (20)     1038 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/utils/urls.py
--rw-r--r--   0 dd         (501) staff       (20)      347 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/utils/version.py
--rw-r--r--   0 dd         (501) staff       (20)      126 2015-08-22 20:34:49.000000 Meringue-0.3.4/meringue/views.py
--rw-r--r--   0 dd         (501) staff       (20)     3570 2015-08-17 21:37:49.000000 Meringue-0.3.4/meringue/widgets.py
-drwxr-xr-x   0 dd         (501) staff       (20)        0 2015-08-22 20:45:31.000000 Meringue-0.3.4/Meringue.egg-info/
--rw-r--r--   0 dd         (501) staff       (20)        1 2015-08-22 20:45:31.000000 Meringue-0.3.4/Meringue.egg-info/dependency_links.txt
--rw-r--r--   0 dd         (501) staff       (20)        1 2015-08-22 20:31:34.000000 Meringue-0.3.4/Meringue.egg-info/not-zip-safe
--rw-r--r--   0 dd         (501) staff       (20)     8093 2015-08-22 20:45:31.000000 Meringue-0.3.4/Meringue.egg-info/PKG-INFO
--rw-r--r--   0 dd         (501) staff       (20)       49 2015-08-22 20:45:31.000000 Meringue-0.3.4/Meringue.egg-info/requires.txt
--rw-r--r--   0 dd         (501) staff       (20)     1196 2015-08-22 20:45:31.000000 Meringue-0.3.4/Meringue.egg-info/SOURCES.txt
--rw-r--r--   0 dd         (501) staff       (20)        9 2015-08-22 20:45:31.000000 Meringue-0.3.4/Meringue.egg-info/top_level.txt
--rw-r--r--   0 dd         (501) staff       (20)     8093 2015-08-22 20:45:31.000000 Meringue-0.3.4/PKG-INFO
--rw-r--r--   0 dd         (501) staff       (20)      152 2015-08-22 20:34:49.000000 Meringue-0.3.4/README.rst
--rw-r--r--   0 dd         (501) staff       (20)       59 2015-08-22 20:45:31.000000 Meringue-0.3.4/setup.cfg
--rwxr-xr-x   0 dd         (501) staff       (20)     1747 2015-08-22 20:34:49.000000 Meringue-0.3.4/setup.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/__init__.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/fields.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/forms.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/middleware.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/widgets.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/apps.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/static/css/inline-gallery.css
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/static/images/noise.png
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/static/images/none.gif
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/admin/templates/admin/filter.html
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/apps.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/decorators.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/errors.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/managers.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/models.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/options.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/query.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/translation.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/views.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/css/inline-gallery.css
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/css/reset.css
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/css/reset.min.css
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/images/noise.png
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/images/none.gif
+-rw-r--r--   0        0        0    83615 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/static/js/jquery-2.1.0.min.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/404.html
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/500.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/robots.txt
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/meringue/edit_inline/gallery.html
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templates/rest_framework/base.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/templatetags/meringue_thumbnails.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/paginator.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/unify.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/thumbnails/__init__.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/thumbnails/methods.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/meringue/core/utils/thumbnails/properties.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/LICENSE
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/README.md
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 meringue-0.4.0.post1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Meringue-0.3.4/meringue/decorators.py` & `meringue-0.4.0.post1/meringue/core/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # -*- coding: utf-8 -*-
 
+import logging  # noqa
+
 from functools import update_wrapper
 
 from django.http import HttpResponseRedirect, HttpResponseForbidden
 
 
+logger = logging.getLogger('meringue')
+
+
 class CheckAccount(object):
     """
-    "По образу и подобию django.contrib.auth.decorators._CheckLogin"(c)
+    По образу и подобию django.contrib.auth.decorators._CheckLogin"(c)
     """
 
     def __init__(self, view_func, test_func, redirect_url=None):
         self.view_func = view_func
         self.test_func = test_func
         self.redirect_url = redirect_url
         update_wrapper(self, view_func)
@@ -24,13 +29,19 @@
         if self.test_func(request.user):
             return self.view_func(request, *args, **kwargs)
         if self.redirect_url:
             return HttpResponseRedirect(self.redirect_url)
         return HttpResponseForbidden()
 
 
+def default_check_func(user):
+    return user.is_anonymous()
+
+
 def anonymous_required(function=None, redirect_url=None):
-    t = lambda u: u.is_anonymous()
-    decorator = lambda f: CheckAccount(f, t, redirect_url)
+    def decorator(fn):
+        return CheckAccount(fn, default_check_func, redirect_url)
+
     if function:
         return decorator(function)
+
     return decorator
```

### Comparing `Meringue-0.3.4/meringue/fields.py` & `meringue-0.4.0.post1/meringue/fields.py`

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

### Comparing `Meringue-0.3.4/meringue/forms.py` & `meringue-0.4.0.post1/meringue/forms.py`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/middleware.py` & `meringue-0.4.0.post1/meringue/middleware.py`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/models.py` & `meringue-0.4.0.post1/meringue/core/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,123 @@
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
-    from django_hosts.resolvers import reverse
-else:
-    from django.core.urlresolvers import reverse
+# if 'django_hosts' in settings.INSTALLED_APPS:
+#     from django_hosts.resolvers import reverse
+# else:
+#     from django.urls import reverse
 
-from . import settings as meringue_settings
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
-        Примесь автоматизирующая получение абсолютного адреса
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
-            cls = self._meta.model_name
-            view = '%s-detail' % cls
-
-            self._meta.view = '%s:%s' % (namespace, view)
-        return self._meta.view
-
-    def _reverse_args(self):
-        reverse_args = getattr(self._meta, 'reverse_args', ['pk'])
-        return [getattr(self, key) for key in reverse_args]
-
-    def get_absolute_url(self):
-        reverse_args = {
-            'viewname': self._view(),
-            'args': self._reverse_args(),
-        }
-        if 'django_hosts' in settings.INSTALLED_APPS:
-            reverse_args.update({
-                'host': self._host_name(),
-                'port': meringue_settings.PORT,
-            })
-        return reverse(**reverse_args)
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
+class CMTimeMixin(models.Model):
+    ctime = models.DateTimeField(auto_now_add=True)
+    mtime = models.DateTimeField(auto_now=True)
 
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
-    ctime = models.DateTimeField(auto_now_add=True)
-    mtime = models.DateTimeField(auto_now=True)
 
     objects = PublishManager()
 
     class Meta:
         abstract = True
```

### Comparing `Meringue-0.3.4/meringue/static/css/inline-gallery.css` & `meringue-0.4.0.post1/meringue/admin/static/css/inline-gallery.css`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/static/css/reset.css` & `meringue-0.4.0.post1/meringue/core/static/css/reset.css`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/static/css/reset.min.css` & `meringue-0.4.0.post1/meringue/core/static/css/reset.min.css`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/static/images/noise.png` & `meringue-0.4.0.post1/meringue/admin/static/images/noise.png`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/static/js/jquery-2.1.0.min.js` & `meringue-0.4.0.post1/meringue/core/static/js/jquery-2.1.0.min.js`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/templates/404.html` & `meringue-0.4.0.post1/meringue/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/templates/500.html` & `meringue-0.4.0.post1/meringue/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/templates/meringue/edit_inline/gallery.html` & `meringue-0.4.0.post1/meringue/core/templates/meringue/edit_inline/gallery.html`

 * *Files identical despite different names*

### Comparing `Meringue-0.3.4/meringue/templatetags/thumbnails.py` & `meringue-0.4.0.post1/meringue/core/templatetags/meringue_thumbnails.py`

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

### Comparing `Meringue-0.3.4/meringue/widgets.py` & `meringue-0.4.0.post1/meringue/widgets.py`

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

