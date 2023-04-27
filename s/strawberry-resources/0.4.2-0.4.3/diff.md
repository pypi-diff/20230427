# Comparing `tmp/strawberry_resources-0.4.2.tar.gz` & `tmp/strawberry_resources-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_resources-0.4.2.tar", max compression
+gzip compressed data, was "strawberry_resources-0.4.3.tar", max compression
```

## Comparing `strawberry_resources-0.4.2.tar` & `strawberry_resources-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/LICENSE
--rw-r--r--   0        0        0     9125 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/README.md
--rw-r--r--   0        0        0     4057 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/__init__.py
--rw-r--r--   0        0        0       59 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/__main__.py
--rw-r--r--   0        0        0      123 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/cli/__init__.py
--rw-r--r--   0        0        0     1268 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/cli/export.py
--rw-r--r--   0        0        0     2828 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/exporter.py
--rw-r--r--   0        0        0      124 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/integrations/__init__.py
--rw-r--r--   0        0        0     1660 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/integrations/base.py
--rw-r--r--   0        0        0     9224 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/integrations/django.py
--rw-r--r--   0        0        0        0 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/py.typed
--rw-r--r--   0        0        0      628 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/queries.py
--rw-r--r--   0        0        0     7602 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/resolver.py
--rw-r--r--   0        0        0     7143 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/types.py
--rw-r--r--   0        0        0        0 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/utils/__init__.py
--rw-r--r--   0        0        0     2049 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/utils/inspect.py
--rw-r--r--   0        0        0      662 2023-03-27 21:41:14.376159 strawberry_resources-0.4.2/strawberry_resources/utils/pyutils.py
--rw-r--r--   0        0        0    10950 1970-01-01 00:00:00.000000 strawberry_resources-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/LICENSE
+-rw-r--r--   0        0        0     9125 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/README.md
+-rw-r--r--   0        0        0     4057 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/__main__.py
+-rw-r--r--   0        0        0      123 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/cli/__init__.py
+-rw-r--r--   0        0        0     1268 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/cli/export.py
+-rw-r--r--   0        0        0     2828 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/exporter.py
+-rw-r--r--   0        0        0      124 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/integrations/__init__.py
+-rw-r--r--   0        0        0     1660 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/integrations/base.py
+-rw-r--r--   0        0        0     9393 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/integrations/django.py
+-rw-r--r--   0        0        0        0 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/py.typed
+-rw-r--r--   0        0        0      628 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/queries.py
+-rw-r--r--   0        0        0     7570 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/resolver.py
+-rw-r--r--   0        0        0     7143 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/types.py
+-rw-r--r--   0        0        0        0 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/utils/__init__.py
+-rw-r--r--   0        0        0     2033 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/utils/inspect.py
+-rw-r--r--   0        0        0      662 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/utils/pyutils.py
+-rw-r--r--   0        0        0    10950 1970-01-01 00:00:00.000000 strawberry_resources-0.4.3/PKG-INFO
```

### Comparing `strawberry_resources-0.4.2/LICENSE` & `strawberry_resources-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/README.md` & `strawberry_resources-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/pyproject.toml` & `strawberry_resources-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-resources"
-version = "0.4.2"
+version = "0.4.3"
 description = "Introspection utilities to extract data from strawberry graphql"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-resources"
 repository = "https://github.com/blb-ventures/strawberry-resources"
 documentation = "https://github.com/blb-ventures/strawberry-resources"
@@ -47,15 +47,15 @@
 django-types = "^0.17.0"
 django-phonenumber-field = "^7.0.0"
 codecov = "^2.1.12"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 ipython = "^8.4.0"
 pytest-asyncio = "^0.21.0"
-ruff = "^0.0.259"
+ruff = "^0.0.263"
 pytest-django = "^4.5.2"
 
 [tool.poetry.extras]
 django = ["django", "strawberry-graphql-django"]
 django-plus = [
   "django",
   "strawberry-graphql-django",
@@ -103,25 +103,26 @@
   "PGH",
   "PL",
   "RSE",
   "RUF",
   "TRY",
   "SLF",
 ]
-
 ignore = [
+  "D1",
   "D203",
   "D213",
   "TCH001",
   "TCH002",
   "TCH003",
   "PGH003",
   "PLR09",
   "PLR2004",
-  "D1",
+  "SLF001",
+  "TRY003",
 ]
 target-version = "py38"
 exclude = [
   ".eggs",
   ".git",
   ".hg",
   ".mypy_cache",
@@ -181,12 +182,11 @@
 strictSetInference = true
 
 [tool.pytest.ini_options]
 python_files = "tests/test_*.py"
 DJANGO_SETTINGS_MODULE = "tests.django_settings"
 addopts = "-p no:warnings --cov=./ --cov-report term-missing:skip-covered"
 asyncio_mode = "auto"
-testpaths = ["tests/"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `strawberry_resources-0.4.2/strawberry_resources/__init__.py` & `strawberry_resources-0.4.3/strawberry_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/strawberry_resources/cli/export.py` & `strawberry_resources-0.4.3/strawberry_resources/cli/export.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/strawberry_resources/exporter.py` & `strawberry_resources-0.4.3/strawberry_resources/exporter.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/strawberry_resources/integrations/base.py` & `strawberry_resources-0.4.3/strawberry_resources/integrations/base.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/strawberry_resources/integrations/django.py` & `strawberry_resources-0.4.3/strawberry_resources/integrations/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.db.models.fields import NOT_PROVIDED
 from strawberry import UNSET
 from strawberry.field import StrawberryField
 from strawberry.scalars import JSON
+from strawberry.type import StrawberryOptional
 from strawberry_django.fields.types import (
     DjangoFileType,
     DjangoImageType,
     resolve_model_field_name,
 )
 from strawberry_django.type import StrawberryDjangoType
 from typing_extensions import Annotated, get_args, get_origin
@@ -74,15 +75,15 @@
 
 
 @_cache
 def _get_model_field(
     model: Type[models.Model],
     field: str,
 ) -> Optional[Union[models.Field, models.ForeignObjectRel]]:
-    meta = model._meta  # noqa: SLF001
+    meta = model._meta
     for f in meta.get_fields():
         name = cast(str, resolve_model_field_name(f, is_input=False, is_filter=False))
         if name == field:
             return f
 
     return None
 
@@ -216,24 +217,26 @@
     elif isinstance(dj_field, (models.IPAddressField, models.GenericIPAddressField)):
         options["kind"] = FieldKind.IP
     elif isinstance(dj_field, models.EmailField):
         options["kind"] = FieldKind.EMAIL
     elif isinstance(dj_field, models.CharField):
         options["kind"] = FieldKind.STRING
         options["validation"] = StringFieldValidation(
+            required=not isinstance(field.type, StrawberryOptional),
             min_length=0 if dj_field.blank else 1,
             max_length=dj_field.max_length,
         )
     elif isinstance(dj_field, models.UUIDField):
         options["kind"] = FieldKind.UUID
     elif isinstance(dj_field, models.URLField):
         options["kind"] = FieldKind.URL
     elif isinstance(dj_field, models.DecimalField):
         options["kind"] = FieldKind.DECIMAL
         options["validation"] = DecimalFieldValidation(
+            required=not isinstance(field.type, StrawberryOptional),
             max_digits=dj_field.max_digits,
             decimal_places=dj_field.decimal_places,
         )
     elif isinstance(dj_field, models.FloatField):
         options["kind"] = FieldKind.FLOAT
     elif isinstance(dj_field, models.AutoField):
         options["kind"] = FieldKind.ID
```

### Comparing `strawberry_resources-0.4.2/strawberry_resources/queries.py` & `strawberry_resources-0.4.3/strawberry_resources/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/strawberry_resources/resolver.py` & `strawberry_resources-0.4.3/strawberry_resources/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 name=type_def.name,
                 fields=list(resolve_fields_for_type(type_def.origin)),
             )
             seen.add(type_def.name)
 
 
 def resolve_fields_for_type(type_: type, *, depth: int = 0):
-    type_def = cast(TypeDefinition, type_._type_definition)  # type: ignore  # noqa: SLF001
+    type_def = cast(TypeDefinition, type_._type_definition)  # type: ignore
     integrations = get_all()
 
     for field in type_def.fields:
         cname = field.graphql_name or to_camel_case(field.name)
         hidden = False
         options: FieldOrFieldObjectOptions = {
             "label": field.name,
@@ -194,15 +194,15 @@
         # If this is another type, we should return a FieldObject instead
         if "obj_kind" in options or hasattr(f_type, "_type_definition"):
             if depth > MAX_DEPTH:
                 continue
 
             inner_type_def = cast(
                 TypeDefinition,
-                f_type._type_definition,  # type: ignore  # noqa: SLF001
+                f_type._type_definition,  # type: ignore
             )
 
             assert isinstance(f_type, type)
             obj_kind = options.get("obj_kind")
             if obj_kind is None:
                 obj_kind_map: Dict[Tuple[bool, bool], FieldObjectKind] = {
                     (False, False): FieldObjectKind.OBJECT,
```

### Comparing `strawberry_resources-0.4.2/strawberry_resources/types.py` & `strawberry_resources-0.4.3/strawberry_resources/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/strawberry_resources/utils/inspect.py` & `strawberry_resources-0.4.3/strawberry_resources/utils/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,8 @@
         yield gql_type
         return
 
     for t in get_possible_types(gql_type):
         if isinstance(t, TypeDefinition):
             yield t
         elif hasattr(t, "_type_definition"):
-            yield t._type_definition  # type: ignore  # noqa: SLF001
+            yield t._type_definition  # type: ignore
```

### Comparing `strawberry_resources-0.4.2/strawberry_resources/utils/pyutils.py` & `strawberry_resources-0.4.3/strawberry_resources/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.2/PKG-INFO` & `strawberry_resources-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-resources
-Version: 0.4.2
+Version: 0.4.3
 Summary: Introspection utilities to extract data from strawberry graphql
 Home-page: https://github.com/blb-ventures/strawberry-resources
 License: MIT
 Keywords: strawberry,django,graphql,resources,forms
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

