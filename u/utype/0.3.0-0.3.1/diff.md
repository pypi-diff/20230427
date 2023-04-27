# Comparing `tmp/utype-0.3.0.tar.gz` & `tmp/utype-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utype-0.3.0.tar", last modified: Thu Mar  9 13:01:05 2023, max compression
+gzip compressed data, was "utype-0.3.1.tar", last modified: Thu Apr 27 03:12:23 2023, max compression
```

## Comparing `utype-0.3.0.tar` & `utype-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 13:01:05.395845 utype-0.3.0/
--rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     9845 2023-03-09 13:01:05.394847 utype-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     8413 2023-03-09 13:00:20.000000 utype-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-09 13:01:05.395845 utype-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 13:01:05.371909 utype-0.3.0/utype/
--rw-rw-rw-   0        0        0     1231 2023-03-07 13:00:43.000000 utype-0.3.0/utype/__init__.py
--rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.3.0/utype/decorator.py
-drwxrwxrwx   0        0        0        0 2023-03-09 13:01:05.389862 utype-0.3.0/utype/parser/
--rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.3.0/utype/parser/__init__.py
--rw-rw-rw-   0        0        0    22472 2023-03-04 14:13:02.000000 utype-0.3.0/utype/parser/base.py
--rw-rw-rw-   0        0        0    20295 2023-03-04 14:13:02.000000 utype-0.3.0/utype/parser/cls.py
--rw-rw-rw-   0        0        0    47187 2023-03-07 11:36:34.000000 utype-0.3.0/utype/parser/field.py
--rw-rw-rw-   0        0        0    36201 2023-03-06 10:25:57.000000 utype-0.3.0/utype/parser/func.py
--rw-rw-rw-   0        0        0    16323 2023-02-05 12:58:24.000000 utype-0.3.0/utype/parser/options.py
--rw-rw-rw-   0        0        0    66625 2023-03-07 08:37:00.000000 utype-0.3.0/utype/parser/rule.py
--rw-rw-rw-   0        0        0    18006 2023-03-07 13:07:37.000000 utype-0.3.0/utype/schema.py
-drwxrwxrwx   0        0        0        0 2023-03-09 13:01:05.390858 utype-0.3.0/utype/specs/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.0/utype/specs/__init__.py
--rw-rw-rw-   0        0        0    12612 2023-03-06 10:25:57.000000 utype-0.3.0/utype/specs/json_schema.py
--rw-rw-rw-   0        0        0     5503 2023-03-03 08:10:28.000000 utype-0.3.0/utype/types.py
-drwxrwxrwx   0        0        0        0 2023-03-09 13:01:05.394847 utype-0.3.0/utype/utils/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.0/utype/utils/__init__.py
--rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.3.0/utype/utils/base.py
--rw-rw-rw-   0        0        0     3260 2023-02-18 09:22:30.000000 utype-0.3.0/utype/utils/compat.py
--rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.3.0/utype/utils/datastructures.py
--rw-rw-rw-   0        0        0     2809 2023-02-08 13:05:18.000000 utype-0.3.0/utype/utils/encode.py
--rw-rw-rw-   0        0        0     7155 2022-12-16 09:43:52.000000 utype-0.3.0/utype/utils/exceptions.py
--rw-rw-rw-   0        0        0     1184 2022-12-16 05:01:12.000000 utype-0.3.0/utype/utils/functional.py
--rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.3.0/utype/utils/style.py
--rw-rw-rw-   0        0        0    22314 2023-02-08 09:49:08.000000 utype-0.3.0/utype/utils/transform.py
-drwxrwxrwx   0        0        0        0 2023-03-09 13:01:05.386875 utype-0.3.0/utype.egg-info/
--rw-rw-rw-   0        0        0     9845 2023-03-09 13:01:05.000000 utype-0.3.0/utype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2023-03-09 13:01:05.000000 utype-0.3.0/utype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 13:01:05.000000 utype-0.3.0/utype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-09 13:01:05.000000 utype-0.3.0/utype.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-09 13:01:05.000000 utype-0.3.0/utype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.618145 utype-0.3.1/
+-rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     9845 2023-04-27 03:12:23.618145 utype-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8413 2023-04-27 03:11:22.000000 utype-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 03:12:23.618145 utype-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.544938 utype-0.3.1/utype/
+-rw-rw-rw-   0        0        0     1231 2023-04-27 03:11:22.000000 utype-0.3.1/utype/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.3.1/utype/decorator.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.576854 utype-0.3.1/utype/parser/
+-rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.3.1/utype/parser/__init__.py
+-rw-rw-rw-   0        0        0    22638 2023-03-14 16:30:18.000000 utype-0.3.1/utype/parser/base.py
+-rw-rw-rw-   0        0        0    20646 2023-03-21 10:41:05.000000 utype-0.3.1/utype/parser/cls.py
+-rw-rw-rw-   0        0        0    47187 2023-03-07 11:36:34.000000 utype-0.3.1/utype/parser/field.py
+-rw-rw-rw-   0        0        0    36288 2023-03-11 14:32:10.000000 utype-0.3.1/utype/parser/func.py
+-rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.3.1/utype/parser/options.py
+-rw-rw-rw-   0        0        0    66625 2023-03-07 08:37:00.000000 utype-0.3.1/utype/parser/rule.py
+-rw-rw-rw-   0        0        0    18006 2023-03-07 13:07:37.000000 utype-0.3.1/utype/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.583233 utype-0.3.1/utype/specs/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.1/utype/specs/__init__.py
+-rw-rw-rw-   0        0        0    12612 2023-03-06 10:25:57.000000 utype-0.3.1/utype/specs/json_schema.py
+-rw-rw-rw-   0        0        0     5515 2023-03-19 14:44:00.000000 utype-0.3.1/utype/types.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.617143 utype-0.3.1/utype/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.1/utype/utils/__init__.py
+-rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.3.1/utype/utils/base.py
+-rw-rw-rw-   0        0        0     3260 2023-02-18 09:22:30.000000 utype-0.3.1/utype/utils/compat.py
+-rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.3.1/utype/utils/datastructures.py
+-rw-rw-rw-   0        0        0     2957 2023-04-17 07:53:54.000000 utype-0.3.1/utype/utils/encode.py
+-rw-rw-rw-   0        0        0     7155 2022-12-16 09:43:52.000000 utype-0.3.1/utype/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1184 2022-12-16 05:01:12.000000 utype-0.3.1/utype/utils/functional.py
+-rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.3.1/utype/utils/style.py
+-rw-rw-rw-   0        0        0    23130 2023-03-10 09:41:24.000000 utype-0.3.1/utype/utils/transform.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.560895 utype-0.3.1/utype.egg-info/
+-rw-rw-rw-   0        0        0     9845 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/top_level.txt
```

### Comparing `utype-0.3.0/LICENSE` & `utype-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/PKG-INFO` & `utype-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.3.0
+Version: 0.3.1
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
@@ -39,15 +39,15 @@
 [![Test Coverage](https://img.shields.io/codecov/c/github/utilmeta/utype?color=green)](https://app.codecov.io/github/utilmeta/utype)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/utype/month)](https://pepy.tech/project/utype)
 
 utype is a data types declaration & parsing library based on Python type annotations, 
 enforce types and constraints for classes and functions at runtime
 
-* Version: `0.3.0` [test]
+* Version: `0.3.1` [test]
 * Author: [@voidZXL](https://github.com/voidZXL)
 * License: Apache 2.0
 * Source Code: [https://github.com/utilmeta/utype](https://github.com/utilmeta/utype)
 * Documentation: [https://utype.io](https://utype.io)
 * 中文文档: [https://utype.io/zh](https://utype.io/zh)
```

### Comparing `utype-0.3.0/README.md` & `utype-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Test Coverage](https://img.shields.io/codecov/c/github/utilmeta/utype?color=green)](https://app.codecov.io/github/utilmeta/utype)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/utype/month)](https://pepy.tech/project/utype)
 
 utype is a data types declaration & parsing library based on Python type annotations, 
 enforce types and constraints for classes and functions at runtime
 
-* Version: `0.3.0` [test]
+* Version: `0.3.1` [test]
 * Author: [@voidZXL](https://github.com/voidZXL)
 * License: Apache 2.0
 * Source Code: [https://github.com/utilmeta/utype](https://github.com/utilmeta/utype)
 * Documentation: [https://utype.io](https://utype.io)
 * 中文文档: [https://utype.io/zh](https://utype.io/zh)
```

### Comparing `utype-0.3.0/setup.py` & `utype-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/__init__.py` & `utype-0.3.1/utype/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .utils.transform import (TypeTransformer, type_transform)
 from .utils.datastructures import unprovided
 from .specs.json_schema import JsonSchemaGenerator
 
 register_transformer = TypeTransformer.registry.register
 
 
-VERSION = (0, 3, 0, None)
+VERSION = (0, 3, 1, None)
 
 
 def _get_version():
     pre_release = VERSION[3] if len(VERSION) > 3 else ""
     version = ".".join([str(v) for v in VERSION[:3]])
     if pre_release:
         version += f"-{pre_release}"
```

### Comparing `utype-0.3.0/utype/decorator.py` & `utype-0.3.1/utype/decorator.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/parser/base.py` & `utype-0.3.1/utype/parser/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     options_cls = Options
     parser_field_cls = ParserField
 
     # DEFAULT_EXCLUDE_VARS = {"__options__", "__class__"}
 
     @classmethod
     def resolve_parser(cls, obj):
+        parser = getattr(obj, "__dict__", {}).get("__parser__")
+        # get to the __dict__ first
+        if isinstance(parser, cls):
+            return parser
         global __parsers__
         if obj in __parsers__:
             return __parsers__[obj]
         parser = getattr(obj, "__parser__", None)
         if isinstance(parser, cls):
             return parser
         return None
```

### Comparing `utype-0.3.0/utype/parser/cls.py` & `utype-0.3.1/utype/parser/cls.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,22 @@
             ):
                 # key is not consider a valid field
                 # and not
                 exclude_vars.add(key)
                 continue
             if key in exclude_vars:
                 continue
+            if attr is Ellipsis and key in self.fields:
+                # class base(Schema):
+                #     f: int
+                # class sub(base):
+                #     f = ...
+                # means that sub schema has dropped field [f] (not declaring the annotation)
+                self.fields.pop(key)
+                continue
             fields.append(
                 self.parser_field_cls.generate(
                     attname=key,
                     annotation=None,
                     default=attr,
                     global_vars=global_vars,
                     forward_refs=self.forward_refs,
```

### Comparing `utype-0.3.0/utype/parser/field.py` & `utype-0.3.1/utype/parser/field.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/parser/func.py` & `utype-0.3.1/utype/parser/func.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,14 +487,15 @@
     def wrap(
         self,
         options: Options = None,
         first_reserve: bool = None,
         parse_params: bool = None,
         parse_result: bool = None,
         eager_parse: bool = False,
+        ignore_methods: bool = False,
     ):
 
         if self.is_async_generator:
             f = self.get_async_generator(
                 options=options,
                 first_reserve=first_reserve,
                 parse_params=parse_params,
@@ -531,18 +532,19 @@
                     context=context,
                     first_reserve=first_reserve,
                     parse_params=parse_params,
                     parse_result=parse_result,
                 )
 
         f.__parser__ = self
-        if self.classmethod:
-            return classmethod(f)
-        elif self.staticmethod:
-            return staticmethod(f)
+        if not ignore_methods:
+            if self.classmethod:
+                return classmethod(f)
+            elif self.staticmethod:
+                return staticmethod(f)
         return f
 
     def parse_pos_type(self, index: int, value, context: RuntimeContext):
         options = context.options
         pos_type = self.position_type
         # we should just ignore the runtime addition type
         if not pos_type:
```

### Comparing `utype-0.3.0/utype/parser/options.py` & `utype-0.3.1/utype/parser/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,16 @@
                 )
 
         if not unprovided(force_default):
             if no_default:
                 raise exc.ConfigError(
                     "Options force_default and no_default can not both specify"
                 )
+            # force default implies ignore_required
+            ignore_required = True
 
         if not collect_errors:
             if max_errors:
                 warnings.warn(
                     f"Options with max_errors: {max_errors} should turn on collect_errors=True"
                 )
                 max_errors = None
```

### Comparing `utype-0.3.0/utype/parser/rule.py` & `utype-0.3.1/utype/parser/rule.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/schema.py` & `utype-0.3.1/utype/schema.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/specs/json_schema.py` & `utype-0.3.1/utype/specs/json_schema.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/types.py` & `utype-0.3.1/utype/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from enum import Enum
 from datetime import datetime, timedelta, date
 from uuid import UUID
 from typing import Union, Optional, Tuple, List, Set, Mapping, \
     Dict, Type, Callable, Any, TYPE_CHECKING, Iterator, ClassVar
 from .utils.compat import Literal, Annotated, Final, ForwardRef
 from .parser.rule import Lax, Rule
-from .utils import exceptions as exc
 
 # from typing import TypeVar
 # T = TypeVar('T')
 
 
 class Number(Rule):
     primitive = "number"
@@ -95,14 +94,15 @@
     @classmethod
     def post_validate(cls, value, options=None):
         import math
 
         if not math.isnan(value):
             # do not use const = float('nan')
             # cause NaN can not use equal operator
+            from .utils import exceptions as exc
             raise exc.ConstraintError(constraint="const", constraint_value=float("nan"))
         return value
 
 
 class InfinityFloat(Float):
     enum = [float("inf"), float("-inf")]
```

### Comparing `utype-0.3.0/utype/utils/base.py` & `utype-0.3.1/utype/utils/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/utils/compat.py` & `utype-0.3.1/utype/utils/compat.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/utils/datastructures.py` & `utype-0.3.1/utype/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/utils/encode.py` & `utype-0.3.1/utype/utils/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,24 @@
 
 
 @register_encoder(Mapping)
 def from_mapping(data):
     return dict(data)
 
 
+@register_encoder(set)
+def from_set(data):
+    return list(data)
+
+
+@register_encoder(tuple)
+def from_tuple(data):
+    return list(data)
+
+
 @register_encoder(unprovided.__class__)
 def from_unprovided(data):
     return None
 
 
 @register_encoder(bytes)
 def from_bytes(data: bytes):
```

### Comparing `utype-0.3.0/utype/utils/exceptions.py` & `utype-0.3.1/utype/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/utils/functional.py` & `utype-0.3.1/utype/utils/functional.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/utils/style.py` & `utype-0.3.1/utype/utils/style.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.0/utype/utils/transform.py` & `utype-0.3.1/utype/utils/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,42 @@
 
 class DateFormat:
     DATETIME = "%Y-%m-%d %H:%M:%S"
     DATETIME_DF = "%Y-%m-%d %H:%M:%S.%f"
     DATETIME_F = "%Y-%m-%d %H:%M:%S %f"
     DATETIME_P = "%Y-%m-%d %I:%M:%S %p"
     DATETIME_T = "%Y-%m-%dT%H:%M:%S"
-    DATETIME_TZ = "%Y-%m-%dT%H:%M:%SZ"
-    DATETIME_TFZ = "%Y-%m-%dT%H:%M:%S.%fZ"
+    # DATETIME_TZ = "%Y-%m-%dT%H:%M:%SZ"
+    # DATETIME_TFZ = "%Y-%m-%dT%H:%M:%S.%fZ"
     DATETIME_TF = "%Y-%m-%dT%H:%M:%S.%f"
-    DATETIME_ISO = "%Y-%m-%dT%H:%M:%S.%fTZD"
-    DATETIME_GMT = "%a, %d %b %Y %H:%M:%S GMT"
+    # DATETIME_ISO = "%Y-%m-%dT%H:%M:%S.%fTZD"
+    DATETIME_HTTP = "%a, %d %b %Y %H:%M:%S"
+    # DATETIME_GMT = "%a, %d %b %Y %H:%M:%S GMT"
     DATETIME_PS = "%a %b %d %H:%M:%S %Y"
-    DATETIME_GMT2 = "%b %d %H:%M:%S %Y GMT"
+    DATETIME_GMT = "%b %d %H:%M:%S %Y"
     DATE = "%Y-%m-%d"
     # TIME = '%H:%M:%S'
 
 
 class TypeTransformer:
     registry = TypeRegistry('transformer', shortcut='__transformer__', cache=True)
     
     # ----- preferences
     # can be override
     DATETIME_FORMATS = [
-        v for k, v in DateFormat.__dict__.items() if k.startswith("DATE")
+        DateFormat.DATETIME,
+        DateFormat.DATETIME_DF,
+        DateFormat.DATETIME_F,
+        DateFormat.DATETIME_P,
+        DateFormat.DATETIME_T,
+        DateFormat.DATETIME_TF,
+        DateFormat.DATETIME_HTTP,
+        DateFormat.DATETIME_PS,
+        DateFormat.DATETIME_GMT,
+        DateFormat.DATE
     ]
     EPOCH = datetime(1970, 1, 1)
     MS_WATERSHED = int(2e10)
     ARRAY_SEPARATORS = (",", ";")
     NULL_VALUES = ("null", "none", "nil")
     FALSE_VALUES = ("0", "false", "no", "off", "f")
     TRUE_VALUES = ("1", "true", "yes", "on", "t", "y")
@@ -477,25 +487,37 @@
             pass
         else:
             while abs(num) > self.MS_WATERSHED:
                 num /= 1000
             return t.utcfromtimestamp(num).replace(tzinfo=timezone.utc)
 
         data = self._from_byte_like(data)
+        is_utc = "GMT" in data or 'UTC' in data or data.endswith("Z") and "T" in data
+        data = data.replace('GMT', '').replace('UTC', '').replace('TZD', '').rstrip('Z').strip()
 
         for f in self.DATETIME_FORMATS:
             try:
                 val = t.strptime(data, f)
-                if data.endswith("GMT") or data.endswith("Z") and "T" in data:
+                if is_utc:
                     val = val.replace(tzinfo=timezone.utc)
                 return val
             except (TypeError, ValueError, re.error):
                 continue
 
-        raise TypeError
+        if '+' in str(data):
+            for f in self.DATETIME_FORMATS:
+                try:
+                    val = t.strptime(data, f + ' %z')
+                    if is_utc:
+                        val = val.replace(tzinfo=timezone.utc)
+                    return val
+                except (TypeError, ValueError, re.error):
+                    continue
+
+        raise TypeError('invalid datetime')
 
     @registry.register(timedelta)
     def to_timedelta(self, data, t: Type[timedelta] = timedelta) -> timedelta:
         if isinstance(data, t):
             return data
         data = self._from_byte_like(self._attempt_from(data))
         try:
```

### Comparing `utype-0.3.0/utype.egg-info/PKG-INFO` & `utype-0.3.1/utype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.3.0
+Version: 0.3.1
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
@@ -39,15 +39,15 @@
 [![Test Coverage](https://img.shields.io/codecov/c/github/utilmeta/utype?color=green)](https://app.codecov.io/github/utilmeta/utype)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/utype/month)](https://pepy.tech/project/utype)
 
 utype is a data types declaration & parsing library based on Python type annotations, 
 enforce types and constraints for classes and functions at runtime
 
-* Version: `0.3.0` [test]
+* Version: `0.3.1` [test]
 * Author: [@voidZXL](https://github.com/voidZXL)
 * License: Apache 2.0
 * Source Code: [https://github.com/utilmeta/utype](https://github.com/utilmeta/utype)
 * Documentation: [https://utype.io](https://utype.io)
 * 中文文档: [https://utype.io/zh](https://utype.io/zh)
```

### Comparing `utype-0.3.0/utype.egg-info/SOURCES.txt` & `utype-0.3.1/utype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

