# Comparing `tmp/marshmallow_dataclass-8.5.8.tar.gz` & `tmp/marshmallow_dataclass-8.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshmallow_dataclass-8.5.8.tar", last modified: Wed Apr 27 16:21:03 2022, max compression
+gzip compressed data, was "marshmallow_dataclass-8.5.9.tar", last modified: Tue Oct  4 17:25:10 2022, max compression
```

## Comparing `marshmallow_dataclass-8.5.8.tar` & `marshmallow_dataclass-8.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 16:21:03.073189 marshmallow_dataclass-8.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10786 2022-04-27 16:21:03.073189 marshmallow_dataclass-8.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9737 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 16:21:03.073189 marshmallow_dataclass-8.5.8/marshmallow_dataclass/
--rw-r--r--   0 runner    (1001) docker     (121)    29107 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/collection_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/lazy_class_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/mypy.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass/union_field.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 16:21:03.073189 marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10786 2022-04-27 16:21:03.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-04-27 16:21:03.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 16:21:03.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-04-27 16:21:03.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-27 16:21:03.000000 marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-04-27 16:21:03.073189 marshmallow_dataclass-8.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-04-27 16:20:51.000000 marshmallow_dataclass-8.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:25:10.229235 marshmallow_dataclass-8.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10766 2022-10-04 17:25:10.229235 marshmallow_dataclass-8.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9737 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:25:10.229235 marshmallow_dataclass-8.5.9/marshmallow_dataclass/
+-rw-r--r--   0 runner    (1001) docker     (121)    29090 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/collection_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/lazy_class_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass/union_field.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:25:10.229235 marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10766 2022-10-04 17:25:10.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-10-04 17:25:10.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 17:25:10.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-04 17:25:10.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-04 17:25:10.000000 marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-04 17:25:10.229235 marshmallow_dataclass-8.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-10-04 17:25:02.000000 marshmallow_dataclass-8.5.9/setup.py
```

### Comparing `marshmallow_dataclass-8.5.8/LICENSE` & `marshmallow_dataclass-8.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/PKG-INFO` & `marshmallow_dataclass-8.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: marshmallow_dataclass
-Version: 8.5.8
+Version: 8.5.9
 Summary: Python library to convert dataclasses into marshmallow schemas.
 Home-page: https://github.com/lovasoa/marshmallow_dataclass
 Author: Ophir LOJKINE
 Author-email: pere.jobs@gmail.com
 License: MIT
 Keywords: marshmallow,dataclass,serialization
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -337,9 +336,7 @@
 ## Documentation
 
 The project documentation is hosted on GitHub Pages: https://lovasoa.github.io/marshmallow_dataclass/
 
 ## Contributing
 
 To install this project and make changes to it locally, follow the instructions in [`CONTRIBUTING.md`](./CONTRIBUTING.md).
-
-
```

### Comparing `marshmallow_dataclass-8.5.8/README.md` & `marshmallow_dataclass-8.5.9/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass/__init__.py` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from functools import lru_cache, partial
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Mapping,
+    NewType as typing_NewType,
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
@@ -379,18 +380,18 @@
                 "marshmallow_dataclass, or define the schema explicitly using "
                 "field(metadata=dict(marshmallow_field=...)). For more information, see "
                 "https://github.com/lovasoa/marshmallow_dataclass/issues/51 "
                 "****** WARNING ******"
             )
             created_dataclass: type = dataclasses.dataclass(clazz)
             return _internal_class_schema(created_dataclass, base_schema, clazz_frame)
-        except Exception:
+        except Exception as exc:
             raise TypeError(
                 f"{getattr(clazz, '__name__', repr(clazz))} is not a dataclass and cannot be turned into one."
-            )
+            ) from exc
 
     # Copy all marshmallow hooks and whitelisted members of the dataclass to the schema.
     attributes = {
         k: v
         for k, v in inspect.getmembers(clazz)
         if hasattr(v, "__marshmallow_hook__") or k in MEMBERS_WHITELIST
     }
@@ -801,20 +802,16 @@
     ContactInfo(mail='anonymous@example.org')
     >>> ContactInfo.Schema().load({"mail": "grumble grumble"})
     Traceback (most recent call last):
     ...
     marshmallow.exceptions.ValidationError: {'mail': ['Not a valid email address.']}
     """
 
-    def new_type(x: _U):
-        return x
-
-    new_type.__name__ = name
     # noinspection PyTypeHints
-    new_type.__supertype__ = typ  # type: ignore
+    new_type = typing_NewType(name, typ)  # type: ignore
     # noinspection PyTypeHints
     new_type._marshmallow_field = field  # type: ignore
     # noinspection PyTypeHints
     new_type._marshmallow_args = kwargs  # type: ignore
     return new_type
```

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass/collection_field.py` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass/collection_field.py`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass/lazy_class_attribute.py` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass/lazy_class_attribute.py`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass/mypy.py` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass/mypy.py`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass/union_field.py` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass/union_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,32 +30,36 @@
         for typ, field in self.union_fields:
             field = copy.deepcopy(field)
             field._bind_to_schema(field_name, self)
             new_union_fields.append((typ, field))
 
         self.union_fields = new_union_fields
 
-    def _serialize(self, value: Any, attr: str, obj, **kwargs) -> Any:
+    def _serialize(self, value: Any, attr: Optional[str], obj, **kwargs) -> Any:
         errors = []
         if value is None:
             return value
         for typ, field in self.union_fields:
             try:
-                typeguard.check_type(attr, value, typ)
+                typeguard.check_type(
+                    value=value, expected_type=typ, argname=attr or "anonymous"
+                )
                 return field._serialize(value, attr, obj, **kwargs)
             except TypeError as e:
                 errors.append(e)
         raise TypeError(
             f"Unable to serialize value with any of the fields in the union: {errors}"
         )
 
     def _deserialize(self, value: Any, attr: Optional[str], data, **kwargs) -> Any:
         errors = []
         for typ, field in self.union_fields:
             try:
                 result = field.deserialize(value, **kwargs)
-                typeguard.check_type(attr or "anonymous", result, typ)
+                typeguard.check_type(
+                    value=result, expected_type=typ, argname=attr or "anonymous"
+                )
                 return result
             except (TypeError, ValidationError) as e:
                 errors.append(e)
 
         raise ValidationError(errors)
```

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/PKG-INFO` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: marshmallow-dataclass
-Version: 8.5.8
+Version: 8.5.9
 Summary: Python library to convert dataclasses into marshmallow schemas.
 Home-page: https://github.com/lovasoa/marshmallow_dataclass
 Author: Ophir LOJKINE
 Author-email: pere.jobs@gmail.com
 License: MIT
 Keywords: marshmallow,dataclass,serialization
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -337,9 +336,7 @@
 ## Documentation
 
 The project documentation is hosted on GitHub Pages: https://lovasoa.github.io/marshmallow_dataclass/
 
 ## Contributing
 
 To install this project and make changes to it locally, follow the instructions in [`CONTRIBUTING.md`](./CONTRIBUTING.md).
-
-
```

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/SOURCES.txt` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/marshmallow_dataclass.egg-info/requires.txt` & `marshmallow_dataclass-8.5.9/marshmallow_dataclass.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `marshmallow_dataclass-8.5.8/setup.py` & `marshmallow_dataclass-8.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "8.5.8"
+VERSION = "8.5.9"
 
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

