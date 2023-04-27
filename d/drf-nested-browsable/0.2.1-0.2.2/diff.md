# Comparing `tmp/drf_nested_browsable-0.2.1.tar.gz` & `tmp/drf_nested_browsable-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_nested_browsable-0.2.1.tar", max compression
+gzip compressed data, was "drf_nested_browsable-0.2.2.tar", max compression
```

## Comparing `drf_nested_browsable-0.2.1.tar` & `drf_nested_browsable-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1361 2023-04-24 15:12:49.325818 drf_nested_browsable-0.2.1/README.md
--rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.2.1/drf_nested_browsable/__init__.py
--rw-r--r--   0        0        0     5122 2023-04-26 09:30:40.887333 drf_nested_browsable-0.2.1/drf_nested_browsable/serializers.py
--rw-r--r--   0        0        0     3463 2023-04-26 07:51:44.002578 drf_nested_browsable-0.2.1/drf_nested_browsable/templates/writable_list.html
--rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.2.1/drf_nested_browsable/templatetags/__init__.py
--rw-r--r--   0        0        0     1809 2023-04-26 07:48:30.548905 drf_nested_browsable-0.2.1/drf_nested_browsable/templatetags/drf_nested_browsable.py
--rw-r--r--   0        0        0     1099 2023-04-26 09:30:58.520686 drf_nested_browsable-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.1/setup.py
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1406 2023-04-26 09:34:59.200966 drf_nested_browsable-0.2.2/README.md
+-rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.2.2/drf_nested_browsable/__init__.py
+-rw-r--r--   0        0        0     6869 2023-04-27 08:33:09.588163 drf_nested_browsable-0.2.2/drf_nested_browsable/serializers.py
+-rw-r--r--   0        0        0     3419 2023-04-27 08:33:09.588163 drf_nested_browsable-0.2.2/drf_nested_browsable/templates/writable_list.html
+-rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.2.2/drf_nested_browsable/templatetags/__init__.py
+-rw-r--r--   0        0        0     4200 2023-04-27 08:33:45.024918 drf_nested_browsable-0.2.2/drf_nested_browsable/templatetags/drf_nested_browsable.py
+-rw-r--r--   0        0        0     1145 2023-04-27 08:33:09.588163 drf_nested_browsable-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.2/setup.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.2/PKG-INFO
```

### Comparing `drf_nested_browsable-0.2.1/README.md` & `drf_nested_browsable-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 This project's dependencies are managed using [`poetry`](https://python-poetry.org/)
 
 ```bash
 git clone https://github.com/pcouy/drf-nested-browsable
 cd drf-nested-browsable
 poetry install
 cd example
+poetry shell
 python manage.py migrate
 python manage.py runserver
 ```
 
 The above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.
 
 ## Current state of the project
 
 ### Done
 
 * Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class
 * Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API
+* Arbitrary nesting depth
+* Dynamically removing the parent field from serializers when used as an inner serializer
 * Basic example
 
 ### To do
 
 * Make the current example work :
-  * Do not show `parent` select list when showing forms as children of another form
   * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer
 * Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)
 * Write tests/specs
```

### Comparing `drf_nested_browsable-0.2.1/drf_nested_browsable/serializers.py` & `drf_nested_browsable-0.2.2/drf_nested_browsable/serializers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,35 @@
 """
-Provides writable serializers for Django Rest Framework
+Provides abstract writable nested serializers for Django Rest Framework
 
-Using these serializers requires a little more configuration than basic
-serializers.
-TODO: Mettre au propre
+These serializers require some additionnal configuration, that is done through the Meta
+class of the concrete classes
 """
 from rest_framework.serializers import ListSerializer, ModelSerializer
 
 
 class WritableNestedListSerializer(ListSerializer):
+    """
+    Can be set as the `list_serializer_class` for any serializer. This will make the
+    `many=True` version of the serializer writable and render an appropriate browsable
+    API form.
+
+    ```python
+    class InnerSerializer(ModelSerializer):
+        class Meta:
+            model = InnerModel
+            fields = ["key", "value", "inner_parent"]
+            list_serializer_class = WritableNestedListSerializer
+            update_keys = "key"
+    ```
+
+    You must use `InnerSerializer(many=True, ...)` either as the root serializer for a
+    `ListAPIView` or as a field of a `WritableNestedModelSerializer`.
+    """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._parent_instance = None
         self._parent_field_name = None
 
         self.style.update({"template": "writable_list.html"})
@@ -33,25 +50,33 @@
                 "`WritableNestedModelSerializer`"
             )
 
         self._parent_field_name = self.parent.Meta.model_related_name
 
     @property
     def parent_data(self):
+        """
+        Provides the data from the parent serializer. You must call
+        `WritableNestedListSerializer.set_parent_instance(instance)`
+        before accessing this property.
+        """
         self._set_parent_field_name()
         if "_parent_instance" not in dir(self) or self._parent_instance is None:
             raise AttributeError(
                 "You must call"
                 "`WritableNestedListSerializer.set_parent_instance(instance)`"
                 "before accessing `WritableNestedListSerializer.parent_data`"
             )
 
         return {self._parent_field_name: self._parent_instance}
 
     def set_parent_instance(self, parent_instance):
+        """
+        Must be called before acessing the `parent_data` property
+        """
         self._parent_instance = parent_instance
 
     def create(self, validated_data):
         return super().create([{**elem, **self.parent_data} for elem in validated_data])
 
     def update(
         self,
@@ -85,46 +110,72 @@
                     elem = self.child.create(full_elem)
                 updated_ids.append(elem.id)
 
             instance.exclude(id__in=updated_ids).delete()
 
 
 class WritableNestedModelSerializer(ModelSerializer):
+    """
+    Abstract class for making model serializers that can write to nested models
+
+    ```python
+    class OuterSerializer(WritableNestedModelSerializer):
+        middle_children = MiddleSerializer(many=True, required=False, default=[])
+
+        class Meta:
+            model = OuterModel
+            model_related_name = "middle_parent"
+            fields = ["key", "value", "middle_children"]
+    ```
+
+    When using this as a base serializer, you must define `Meta.model_related_name`,
+    which is the child model field name for the relationship to the parent.
+    """
+
     class Meta:
         model_related_name = None
 
     def __init__(self, *args, **kwargs):
         if (
             "model_related_name" not in dir(self.Meta)
             or self.Meta.model_related_name is None
         ):
             raise ValueError(
                 "You must define `model_related_name` when you inherit from"
                 "`WritableNestedModelSerializer`"
             )
 
-        for field_name, field in self._declared_fields.items():
+        for field in self._declared_fields.values():  # pylint: disable=no-member
             if (
                 isinstance(field, WritableNestedListSerializer)
                 and self.Meta.model_related_name in field.child.fields.keys()
             ):
-                new_fields = []
-                for old_field in field.child.__class__.Meta.fields:
-                    if old_field != self.Meta.model_related_name:
-                        new_fields.append(old_field)
-
-                class NewChild(field.child.__class__):
-                    class Meta(field.child.__class__.Meta):
-                        fields = new_fields
-
-                NewChild.__name__ = field.child.__class__.__name__
-                field.child.__class__ = NewChild
+                self.alter_nested_child(field)
 
         super().__init__(*args, **kwargs)
 
+    def alter_nested_child(self, field):
+        """
+        Removes fields representing the current serializer from nested child
+        serializers (if it exists).
+
+        This uses `Meta.model_related_name`
+        """
+        new_fields = []
+        for old_field in field.child.__class__.Meta.fields:
+            if old_field != self.Meta.model_related_name:
+                new_fields.append(old_field)
+
+        class _NewChild(field.child.__class__):
+            class Meta(field.child.__class__.Meta):
+                fields = new_fields
+
+        _NewChild.__name__ = field.child.__class__.__name__
+        field.child.__class__ = _NewChild
+
     def create(self, validated_data):
         many_children = {}
         for k, ser in self.fields.items():
             if isinstance(ser, WritableNestedListSerializer):
                 many_children.update({k: (ser, validated_data.pop(k, None))})
         instance = super().create(validated_data)
         for k, (ser, list_data) in many_children.items():
```

### Comparing `drf_nested_browsable-0.2.1/drf_nested_browsable/templates/writable_list.html` & `drf_nested_browsable-0.2.2/drf_nested_browsable/templates/writable_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,14 @@
           {% render_nested field.child prefix=field.name|addstr:"["|addstr:placeholder|addstr:"]" %}
           <button class="del-entry" data-field="{{field.name}}">-</button>
         </div>
       </div>
       {% endwith %}
       {% endif %}
 
-      <pre>
-{{ field.child }}
-      </pre>
-
       {% for entry in field.value %}
         <div class="inner-form-entry" data-index="{{ forloop.counter0 }}">
           {% if field.proxied is None %}
             {% render_nested field.child data=entry prefix=field.name|addstr:"["|addstr:forloop.counter0|addstr:"]" %}
             Not proxied
           {% else %}
             {% render_nested field.proxied.child data=entry prefix=field.name|addstr:"["|addstr:forloop.counter0|addstr:"]" %}
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
 {% load rest_framework %} {% load drf_nested_browsable %}  {% if field.label %}
  {{ field.label }}
 {% endif %} {% with templateId=field.name|addstr:"-form-template" %}
 {% if field.tree_root is None or field.tree_root %} {% with
 placeholder=field.name|fieldname_to_placeholder %}
 {% render_nested field.child prefix=field.name|addstr:"["|addstr:
 placeholder|addstr:"]" %} -
-{% endwith %} {% endif %}
-{{ field.child }}
-{% for entry in field.value %}
+{% endwith %} {% endif %} {% for entry in field.value %}
 {% if field.proxied is None %} {% render_nested field.child data=entry
 prefix=field.name|addstr:"["|addstr:forloop.counter0|addstr:"]" %} Not proxied
 {% else %} {% render_nested field.proxied.child data=entry
 prefix=field.name|addstr:"["|addstr:forloop.counter0|addstr:"]" %} Proxied {%
 endif %} -
 {% endfor %}
 +
```

### Comparing `drf_nested_browsable-0.2.1/pyproject.toml` & `drf_nested_browsable-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-nested-browsable"
-version = "0.2.1"
+version = "0.2.2"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Framework :: Django",
     "Intended Audience :: Developers"
 ]
 description = "Writable nested serializers with forms for the Browsable API"
 keywords = ["django", "rest framework", "drf", "browsable api", "nested serializers"]
@@ -30,13 +30,15 @@
 django-stubs = "^1.16.0"
 pylint-django = "^2.5.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.pylint]
+no-docstring-rgx = "^(_|Meta$)"
 
 [tool.pylint.format]
 max-line-length = "88"
 
 [tool.pylint.design]
 min-public-methods = 0
```

### Comparing `drf_nested_browsable-0.2.1/setup.py` & `drf_nested_browsable-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'drf_nested_browsable': ['templates/*']}
 
 install_requires = \
 ['django>=4.2,<5.0', 'djangorestframework>=3.14.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'drf-nested-browsable',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Writable nested serializers with forms for the Browsable API',
-    'long_description': ":warning: Work In Progress :warning:\n\n# Writable Nested Serializers with Browsable API Forms\n\nThis plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.\n\n## Try it out\n\nThis project's dependencies are managed using [`poetry`](https://python-poetry.org/)\n\n```bash\ngit clone https://github.com/pcouy/drf-nested-browsable\ncd drf-nested-browsable\npoetry install\ncd example\npython manage.py migrate\npython manage.py runserver\n```\n\nThe above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.\n\n## Current state of the project\n\n### Done\n\n* Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class\n* Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API\n* Basic example\n\n### To do\n\n* Make the current example work :\n  * Do not show `parent` select list when showing forms as children of another form\n  * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer\n* Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)\n* Write tests/specs\n",
+    'long_description': ":warning: Work In Progress :warning:\n\n# Writable Nested Serializers with Browsable API Forms\n\nThis plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.\n\n## Try it out\n\nThis project's dependencies are managed using [`poetry`](https://python-poetry.org/)\n\n```bash\ngit clone https://github.com/pcouy/drf-nested-browsable\ncd drf-nested-browsable\npoetry install\ncd example\npoetry shell\npython manage.py migrate\npython manage.py runserver\n```\n\nThe above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.\n\n## Current state of the project\n\n### Done\n\n* Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class\n* Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API\n* Arbitrary nesting depth\n* Dynamically removing the parent field from serializers when used as an inner serializer\n* Basic example\n\n### To do\n\n* Make the current example work :\n  * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer\n* Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)\n* Write tests/specs\n",
     'author': 'Pierre Couy',
     'author_email': 'contact@pierre-couy.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pierre-couy.dev/projects/drf-nested-browsable.html',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `drf_nested_browsable-0.2.1/PKG-INFO` & `drf_nested_browsable-0.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-nested-browsable
-Version: 0.2.1
+Version: 0.2.2
 Summary: Writable nested serializers with forms for the Browsable API
 Home-page: https://pierre-couy.dev/projects/drf-nested-browsable.html
 License: MIT
 Keywords: django,rest framework,drf,browsable api,nested serializers
 Author: Pierre Couy
 Author-email: contact@pierre-couy.dev
 Requires-Python: >=3.10,<4.0
@@ -31,29 +31,31 @@
 This project's dependencies are managed using [`poetry`](https://python-poetry.org/)
 
 ```bash
 git clone https://github.com/pcouy/drf-nested-browsable
 cd drf-nested-browsable
 poetry install
 cd example
+poetry shell
 python manage.py migrate
 python manage.py runserver
 ```
 
 The above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.
 
 ## Current state of the project
 
 ### Done
 
 * Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class
 * Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API
+* Arbitrary nesting depth
+* Dynamically removing the parent field from serializers when used as an inner serializer
 * Basic example
 
 ### To do
 
 * Make the current example work :
-  * Do not show `parent` select list when showing forms as children of another form
   * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer
 * Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)
 * Write tests/specs
```

