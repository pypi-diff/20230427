# Comparing `tmp/linkit-0.1.6.tar.gz` & `tmp/linkit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linkit-0.1.6.tar", last modified: Fri Jan 15 09:23:48 2021, max compression
+gzip compressed data, was "linkit-0.1.7.tar", last modified: Thu Apr 27 11:19:09 2023, max compression
```

## Comparing `linkit-0.1.6.tar` & `linkit-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.291147 linkit-0.1.6/
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1064 2019-05-21 12:21:54.000000 linkit-0.1.6/LICENSE
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.271278 linkit-0.1.6/LinkIt.egg-info/
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     5362 2021-01-15 09:23:48.000000 linkit-0.1.6/LinkIt.egg-info/PKG-INFO
--rw-r--r--   0 sidneywidmer   (501) staff       (20)      702 2021-01-15 09:23:48.000000 linkit-0.1.6/LinkIt.egg-info/SOURCES.txt
--rw-r--r--   0 sidneywidmer   (501) staff       (20)        1 2021-01-15 09:23:48.000000 linkit-0.1.6/LinkIt.egg-info/dependency_links.txt
--rw-r--r--   0 sidneywidmer   (501) staff       (20)        7 2021-01-15 09:23:48.000000 linkit-0.1.6/LinkIt.egg-info/top_level.txt
--rw-r--r--   0 sidneywidmer   (501) staff       (20)       58 2019-07-18 12:53:52.000000 linkit-0.1.6/MANIFEST.in
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     5362 2021-01-15 09:23:48.290763 linkit-0.1.6/PKG-INFO
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     3833 2019-07-18 12:53:52.000000 linkit-0.1.6/README.md
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.277974 linkit-0.1.6/linkit/
--rw-r--r--   0 sidneywidmer   (501) staff       (20)        0 2019-05-10 06:22:02.000000 linkit-0.1.6/linkit/__init__.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)       63 2021-01-15 09:21:42.000000 linkit-0.1.6/linkit/__version__.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)       87 2019-05-10 06:22:02.000000 linkit-0.1.6/linkit/apps.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1088 2019-07-19 06:34:59.000000 linkit-0.1.6/linkit/form_fields.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     2745 2019-07-24 11:14:40.000000 linkit-0.1.6/linkit/link.py
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.279788 linkit-0.1.6/linkit/migrations/
--rw-r--r--   0 sidneywidmer   (501) staff       (20)      748 2019-05-10 06:22:02.000000 linkit-0.1.6/linkit/migrations/0001_initial.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)        0 2019-05-10 06:22:02.000000 linkit-0.1.6/linkit/migrations/__init__.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     2864 2021-01-15 09:21:42.000000 linkit-0.1.6/linkit/model_fields.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)      447 2020-07-02 15:37:52.000000 linkit-0.1.6/linkit/models.py
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.261417 linkit-0.1.6/linkit/templates/
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.261653 linkit-0.1.6/linkit/templates/django/
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.261873 linkit-0.1.6/linkit/templates/django/forms/
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.280696 linkit-0.1.6/linkit/templates/django/forms/widgets/
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1523 2021-01-15 09:21:39.000000 linkit-0.1.6/linkit/templates/django/forms/widgets/link.html
-drwxr-xr-x   0 sidneywidmer   (501) staff       (20)        0 2021-01-15 09:23:48.289969 linkit-0.1.6/linkit/types/
--rw-r--r--   0 sidneywidmer   (501) staff       (20)      311 2019-06-25 13:50:10.000000 linkit-0.1.6/linkit/types/__init__.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     2673 2019-07-19 06:34:38.000000 linkit-0.1.6/linkit/types/contracts.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1728 2019-06-25 13:50:10.000000 linkit-0.1.6/linkit/types/file.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)      745 2019-06-25 13:50:10.000000 linkit-0.1.6/linkit/types/input.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1549 2019-06-25 13:50:10.000000 linkit-0.1.6/linkit/types/manager.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1136 2021-01-15 09:21:39.000000 linkit-0.1.6/linkit/types/model.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     1156 2021-01-15 09:21:39.000000 linkit-0.1.6/linkit/types/page.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     4804 2019-06-25 13:50:10.000000 linkit-0.1.6/linkit/widgets.py
--rw-r--r--   0 sidneywidmer   (501) staff       (20)       38 2021-01-15 09:23:48.291262 linkit-0.1.6/setup.cfg
--rw-r--r--   0 sidneywidmer   (501) staff       (20)     2972 2020-07-02 15:37:52.000000 linkit-0.1.6/setup.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:09.005290 linkit-0.1.7/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1064 2023-03-06 15:48:51.000000 linkit-0.1.7/LICENSE
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       58 2023-03-06 15:48:51.000000 linkit-0.1.7/MANIFEST.in
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4481 2023-04-27 11:19:09.004935 linkit-0.1.7/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     3833 2023-03-06 15:48:51.000000 linkit-0.1.7/README.md
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.996087 linkit-0.1.7/linkit/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       63 2023-04-27 11:16:02.000000 linkit-0.1.7/linkit/__version__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       87 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/apps.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1088 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/form_fields.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2745 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/link.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.998759 linkit-0.1.7/linkit/migrations/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      748 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/migrations/0001_initial.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/migrations/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2864 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/model_fields.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      447 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/models.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.987099 linkit-0.1.7/linkit/templates/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.987302 linkit-0.1.7/linkit/templates/django/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.987503 linkit-0.1.7/linkit/templates/django/forms/
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.999109 linkit-0.1.7/linkit/templates/django/forms/widgets/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1523 2023-04-18 13:59:43.000000 linkit-0.1.7/linkit/templates/django/forms/widgets/link.html
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:09.004197 linkit-0.1.7/linkit/types/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      311 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/__init__.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2673 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/contracts.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1728 2023-04-18 14:03:16.000000 linkit-0.1.7/linkit/types/file.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      745 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/input.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1549 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/manager.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1136 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/model.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1156 2023-03-06 15:48:51.000000 linkit-0.1.7/linkit/types/page.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     5044 2023-04-27 11:17:01.000000 linkit-0.1.7/linkit/widgets.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-04-27 11:19:08.997746 linkit-0.1.7/linkit.egg-info/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4481 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      582 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/SOURCES.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        1 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/dependency_links.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        7 2023-04-27 11:19:08.000000 linkit-0.1.7/linkit.egg-info/top_level.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       38 2023-04-27 11:19:09.005407 linkit-0.1.7/setup.cfg
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2972 2023-03-06 15:48:51.000000 linkit-0.1.7/setup.py
```

### Comparing `linkit-0.1.6/LICENSE` & `linkit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/LinkIt.egg-info/PKG-INFO` & `linkit-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,127 @@
 Metadata-Version: 2.1
 Name: linkit
-Version: 0.1.6
+Version: 0.1.7
 Summary: Painless link handling - be it a custom model, file or cms page
 Home-page: https://github.com/dreipol/linkit
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
-Description: 
-        # 🔗 LinkIt
-        
-        LinkIt gives you a new field type `LinkField` to use on your models which allows you to effortlessly link to different models on your site. This could be a django-cms Page model,
-        a filer File or anything custom like a News model.
-        
-        <img src="https://github.com/dreipol/linkit/raw/master/doc/linkit.gif"/>
-        
-        ## Installation 
-        Install the latest version with pip and add `linkit` to your `INSTALLED_APPS` - and you're good to go.
-        
-            $ pip install LinkIt
-        
-        ## Usage    
-        You're now able to use the new `LinkField` on any of your models:
-        
-        ```python
-        from django.db.models import Model, CharField
-        from linkit.model_fields import LinkField
-        
-        class Foo(Model):
-            title = CharField(max_length=255)
-            link = LinkField(types=['page', 'file', 'input'])  # <-- Yay!
-        ```
-        
-        If you register this model in django admin you'll get a dropdown field where yru can choose between cms pages, filer files or just a plain input field. 
-        Your model is now able to link to any of these entities with one single field.  
-        
-        In a template you could use this link field like this:
-        ````html
-        <a href="{{ instance.link.href }}" target="{{ instance.link.target }}">{{ instance.link.label }}</a>
-        ````
-            
-        ## Configuration
-        The `LinkField` takes some options which will define how the rendered widget looks and what options the content editor has:
-        
-        - `types: list = None` Defines which link types are allowed (see more bellow in the section «Types») 
-        - `allow_target: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `_target` of the link  
-        - `allow_label: bool = True` Renders an additonal input field so a custom label can be set
-        - `allow_no_follow: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `rel="nofollow"` for the link  
-        
-        ## Types
-        Out of the Box LinkIt ships with three types: input, file, page. The `LinkType` base class makes it easy to implement your own link type, whatever
-        it may be. If you want to link to another existing model in your app, e.g. News, all you need to do is register a new link type.
-        
-        1. Create a file `link_types.py` in any of your apps:
-        
-        ```python
-        from linkit.types.model import ModelLinkType
-        
-        
-        class NewsLinkType(ModelLinkType):
-            identifier = 'news'
-            type_label = 'News'
-            model = News
-        
-        ```
-        
-        2. Register the new type, preferably in a `AppConfig` `ready` method:
-        
-        ````python
-        from django.apps import AppConfig
-        from django.utils.translation import ugettext_lazy as _
-        
-        
-        class ContentConfig(AppConfig):
-            name = 'contents'
-        
-            def ready(self):
-                from contents.link_types import NewsLinkType
-                from linkit.types import type_manager as linkit_manager
-        
-        
-                linkit_manager.register(NewsLinkType)
-        ````
-        
-        3. Profit! You can now create a field like this on any of your models: `link = LinkField(types=['news', 'page])` and link to any of your news or cms pages.
-        
-        Check `linkit/types` to see how the core types are implemented.
-        
-        ### EmailType example
-        Say we have a totally different new type we want to implement and can't just extend from the `ModelLinkType`. See the example bellow
-        of a link type used to link to e-mail addresses with a optional subject field.
-        
-        ````python
-        class EmailTypeForm(TypeForm):
-            address = EmailField(label='E-Mail', required=True)
-            subject = CharField(label='Subject', required=False, max_length=20)
-        
-        
-        class EmailType(LinkType):
-            identifier = 'email'
-            type_label = 'E-Mail'
-            form_class = EmailTypeForm
-        
-            def real_value(self):
-                return self.link.data('value')
-        
-            @property
-            def href(self) -> Optional[str]:
-                mail = self.real_value().get('address')
-                subject = self.real_value().get('subject', '')
-        
-                return f'mailto:{mail}?subject={subject}'
-        
-            @property
-            def label(self) -> Optional[str]:
-                return self.real_value().get('address')
-        ````
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# 🔗 LinkIt
+
+LinkIt gives you a new field type `LinkField` to use on your models which allows you to effortlessly link to different models on your site. This could be a django-cms Page model,
+a filer File or anything custom like a News model.
+
+<img src="https://github.com/dreipol/linkit/raw/master/doc/linkit.gif"/>
+
+## Installation 
+Install the latest version with pip and add `linkit` to your `INSTALLED_APPS` - and you're good to go.
+
+    $ pip install LinkIt
+
+## Usage    
+You're now able to use the new `LinkField` on any of your models:
+
+```python
+from django.db.models import Model, CharField
+from linkit.model_fields import LinkField
+
+class Foo(Model):
+    title = CharField(max_length=255)
+    link = LinkField(types=['page', 'file', 'input'])  # <-- Yay!
+```
+
+If you register this model in django admin you'll get a dropdown field where yru can choose between cms pages, filer files or just a plain input field. 
+Your model is now able to link to any of these entities with one single field.  
+
+In a template you could use this link field like this:
+````html
+<a href="{{ instance.link.href }}" target="{{ instance.link.target }}">{{ instance.link.label }}</a>
+````
+    
+## Configuration
+The `LinkField` takes some options which will define how the rendered widget looks and what options the content editor has:
+
+- `types: list = None` Defines which link types are allowed (see more bellow in the section «Types») 
+- `allow_target: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `_target` of the link  
+- `allow_label: bool = True` Renders an additonal input field so a custom label can be set
+- `allow_no_follow: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `rel="nofollow"` for the link  
+
+## Types
+Out of the Box LinkIt ships with three types: input, file, page. The `LinkType` base class makes it easy to implement your own link type, whatever
+it may be. If you want to link to another existing model in your app, e.g. News, all you need to do is register a new link type.
+
+1. Create a file `link_types.py` in any of your apps:
+
+```python
+from linkit.types.model import ModelLinkType
+
+
+class NewsLinkType(ModelLinkType):
+    identifier = 'news'
+    type_label = 'News'
+    model = News
+
+```
+
+2. Register the new type, preferably in a `AppConfig` `ready` method:
+
+````python
+from django.apps import AppConfig
+from django.utils.translation import ugettext_lazy as _
+
+
+class ContentConfig(AppConfig):
+    name = 'contents'
+
+    def ready(self):
+        from contents.link_types import NewsLinkType
+        from linkit.types import type_manager as linkit_manager
+
+
+        linkit_manager.register(NewsLinkType)
+````
+
+3. Profit! You can now create a field like this on any of your models: `link = LinkField(types=['news', 'page])` and link to any of your news or cms pages.
+
+Check `linkit/types` to see how the core types are implemented.
+
+### EmailType example
+Say we have a totally different new type we want to implement and can't just extend from the `ModelLinkType`. See the example bellow
+of a link type used to link to e-mail addresses with a optional subject field.
+
+````python
+class EmailTypeForm(TypeForm):
+    address = EmailField(label='E-Mail', required=True)
+    subject = CharField(label='Subject', required=False, max_length=20)
+
+
+class EmailType(LinkType):
+    identifier = 'email'
+    type_label = 'E-Mail'
+    form_class = EmailTypeForm
+
+    def real_value(self):
+        return self.link.data('value')
+
+    @property
+    def href(self) -> Optional[str]:
+        mail = self.real_value().get('address')
+        subject = self.real_value().get('subject', '')
+
+        return f'mailto:{mail}?subject={subject}'
+
+    @property
+    def label(self) -> Optional[str]:
+        return self.real_value().get('address')
+````
```

### Comparing `linkit-0.1.6/PKG-INFO` & `linkit-0.1.7/linkit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,127 @@
 Metadata-Version: 2.1
 Name: linkit
-Version: 0.1.6
+Version: 0.1.7
 Summary: Painless link handling - be it a custom model, file or cms page
 Home-page: https://github.com/dreipol/linkit
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
-Description: 
-        # 🔗 LinkIt
-        
-        LinkIt gives you a new field type `LinkField` to use on your models which allows you to effortlessly link to different models on your site. This could be a django-cms Page model,
-        a filer File or anything custom like a News model.
-        
-        <img src="https://github.com/dreipol/linkit/raw/master/doc/linkit.gif"/>
-        
-        ## Installation 
-        Install the latest version with pip and add `linkit` to your `INSTALLED_APPS` - and you're good to go.
-        
-            $ pip install LinkIt
-        
-        ## Usage    
-        You're now able to use the new `LinkField` on any of your models:
-        
-        ```python
-        from django.db.models import Model, CharField
-        from linkit.model_fields import LinkField
-        
-        class Foo(Model):
-            title = CharField(max_length=255)
-            link = LinkField(types=['page', 'file', 'input'])  # <-- Yay!
-        ```
-        
-        If you register this model in django admin you'll get a dropdown field where yru can choose between cms pages, filer files or just a plain input field. 
-        Your model is now able to link to any of these entities with one single field.  
-        
-        In a template you could use this link field like this:
-        ````html
-        <a href="{{ instance.link.href }}" target="{{ instance.link.target }}">{{ instance.link.label }}</a>
-        ````
-            
-        ## Configuration
-        The `LinkField` takes some options which will define how the rendered widget looks and what options the content editor has:
-        
-        - `types: list = None` Defines which link types are allowed (see more bellow in the section «Types») 
-        - `allow_target: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `_target` of the link  
-        - `allow_label: bool = True` Renders an additonal input field so a custom label can be set
-        - `allow_no_follow: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `rel="nofollow"` for the link  
-        
-        ## Types
-        Out of the Box LinkIt ships with three types: input, file, page. The `LinkType` base class makes it easy to implement your own link type, whatever
-        it may be. If you want to link to another existing model in your app, e.g. News, all you need to do is register a new link type.
-        
-        1. Create a file `link_types.py` in any of your apps:
-        
-        ```python
-        from linkit.types.model import ModelLinkType
-        
-        
-        class NewsLinkType(ModelLinkType):
-            identifier = 'news'
-            type_label = 'News'
-            model = News
-        
-        ```
-        
-        2. Register the new type, preferably in a `AppConfig` `ready` method:
-        
-        ````python
-        from django.apps import AppConfig
-        from django.utils.translation import ugettext_lazy as _
-        
-        
-        class ContentConfig(AppConfig):
-            name = 'contents'
-        
-            def ready(self):
-                from contents.link_types import NewsLinkType
-                from linkit.types import type_manager as linkit_manager
-        
-        
-                linkit_manager.register(NewsLinkType)
-        ````
-        
-        3. Profit! You can now create a field like this on any of your models: `link = LinkField(types=['news', 'page])` and link to any of your news or cms pages.
-        
-        Check `linkit/types` to see how the core types are implemented.
-        
-        ### EmailType example
-        Say we have a totally different new type we want to implement and can't just extend from the `ModelLinkType`. See the example bellow
-        of a link type used to link to e-mail addresses with a optional subject field.
-        
-        ````python
-        class EmailTypeForm(TypeForm):
-            address = EmailField(label='E-Mail', required=True)
-            subject = CharField(label='Subject', required=False, max_length=20)
-        
-        
-        class EmailType(LinkType):
-            identifier = 'email'
-            type_label = 'E-Mail'
-            form_class = EmailTypeForm
-        
-            def real_value(self):
-                return self.link.data('value')
-        
-            @property
-            def href(self) -> Optional[str]:
-                mail = self.real_value().get('address')
-                subject = self.real_value().get('subject', '')
-        
-                return f'mailto:{mail}?subject={subject}'
-        
-            @property
-            def label(self) -> Optional[str]:
-                return self.real_value().get('address')
-        ````
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# 🔗 LinkIt
+
+LinkIt gives you a new field type `LinkField` to use on your models which allows you to effortlessly link to different models on your site. This could be a django-cms Page model,
+a filer File or anything custom like a News model.
+
+<img src="https://github.com/dreipol/linkit/raw/master/doc/linkit.gif"/>
+
+## Installation 
+Install the latest version with pip and add `linkit` to your `INSTALLED_APPS` - and you're good to go.
+
+    $ pip install LinkIt
+
+## Usage    
+You're now able to use the new `LinkField` on any of your models:
+
+```python
+from django.db.models import Model, CharField
+from linkit.model_fields import LinkField
+
+class Foo(Model):
+    title = CharField(max_length=255)
+    link = LinkField(types=['page', 'file', 'input'])  # <-- Yay!
+```
+
+If you register this model in django admin you'll get a dropdown field where yru can choose between cms pages, filer files or just a plain input field. 
+Your model is now able to link to any of these entities with one single field.  
+
+In a template you could use this link field like this:
+````html
+<a href="{{ instance.link.href }}" target="{{ instance.link.target }}">{{ instance.link.label }}</a>
+````
+    
+## Configuration
+The `LinkField` takes some options which will define how the rendered widget looks and what options the content editor has:
+
+- `types: list = None` Defines which link types are allowed (see more bellow in the section «Types») 
+- `allow_target: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `_target` of the link  
+- `allow_label: bool = True` Renders an additonal input field so a custom label can be set
+- `allow_no_follow: bool = False` If set to true, the widget renders a checkbox so the editor can choose the `rel="nofollow"` for the link  
+
+## Types
+Out of the Box LinkIt ships with three types: input, file, page. The `LinkType` base class makes it easy to implement your own link type, whatever
+it may be. If you want to link to another existing model in your app, e.g. News, all you need to do is register a new link type.
+
+1. Create a file `link_types.py` in any of your apps:
+
+```python
+from linkit.types.model import ModelLinkType
+
+
+class NewsLinkType(ModelLinkType):
+    identifier = 'news'
+    type_label = 'News'
+    model = News
+
+```
+
+2. Register the new type, preferably in a `AppConfig` `ready` method:
+
+````python
+from django.apps import AppConfig
+from django.utils.translation import ugettext_lazy as _
+
+
+class ContentConfig(AppConfig):
+    name = 'contents'
+
+    def ready(self):
+        from contents.link_types import NewsLinkType
+        from linkit.types import type_manager as linkit_manager
+
+
+        linkit_manager.register(NewsLinkType)
+````
+
+3. Profit! You can now create a field like this on any of your models: `link = LinkField(types=['news', 'page])` and link to any of your news or cms pages.
+
+Check `linkit/types` to see how the core types are implemented.
+
+### EmailType example
+Say we have a totally different new type we want to implement and can't just extend from the `ModelLinkType`. See the example bellow
+of a link type used to link to e-mail addresses with a optional subject field.
+
+````python
+class EmailTypeForm(TypeForm):
+    address = EmailField(label='E-Mail', required=True)
+    subject = CharField(label='Subject', required=False, max_length=20)
+
+
+class EmailType(LinkType):
+    identifier = 'email'
+    type_label = 'E-Mail'
+    form_class = EmailTypeForm
+
+    def real_value(self):
+        return self.link.data('value')
+
+    @property
+    def href(self) -> Optional[str]:
+        mail = self.real_value().get('address')
+        subject = self.real_value().get('subject', '')
+
+        return f'mailto:{mail}?subject={subject}'
+
+    @property
+    def label(self) -> Optional[str]:
+        return self.real_value().get('address')
+````
```

### Comparing `linkit-0.1.6/README.md` & `linkit-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/form_fields.py` & `linkit-0.1.7/linkit/form_fields.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/link.py` & `linkit-0.1.7/linkit/link.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/migrations/0001_initial.py` & `linkit-0.1.7/linkit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/model_fields.py` & `linkit-0.1.7/linkit/model_fields.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/templates/django/forms/widgets/link.html` & `linkit-0.1.7/linkit/templates/django/forms/widgets/link.html`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/types/contracts.py` & `linkit-0.1.7/linkit/types/contracts.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/types/file.py` & `linkit-0.1.7/linkit/types/file.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/types/input.py` & `linkit-0.1.7/linkit/types/input.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/types/manager.py` & `linkit-0.1.7/linkit/types/manager.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/types/model.py` & `linkit-0.1.7/linkit/types/model.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/types/page.py` & `linkit-0.1.7/linkit/types/page.py`

 * *Files identical despite different names*

### Comparing `linkit-0.1.6/linkit/widgets.py` & `linkit-0.1.7/linkit/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,22 @@
 
     @staticmethod
     def type_fields(link: Link) -> dict:
         """ Generate all fields for the different link types that are allowed in this link instance. """
         types = {}
         for link_type in link.config('types'):
             instance = type_manager.instance(link_type, link)
+            try:
+                markup = instance.render()
+            except Exception:
+                # Reset link value if target is no longer available
+                instance.link._data['value'] = {}
+                markup = instance.render()
             types[link_type] = {
-                'markup': instance.render(),
+                'markup': markup,
                 'instance': instance,
             }
 
         return types
 
     @staticmethod
     def other_fields(link: Link, field_name: str) -> dict:
```

### Comparing `linkit-0.1.6/setup.py` & `linkit-0.1.7/setup.py`

 * *Files identical despite different names*

