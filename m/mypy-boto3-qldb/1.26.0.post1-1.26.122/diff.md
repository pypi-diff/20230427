# Comparing `tmp/mypy-boto3-qldb-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-qldb-1.26.122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:51 2022, max compression
+gzip compressed data, was "mypy-boto3-qldb-1.26.122.tar", last modified: Thu Apr 27 19:33:42 2023, max compression
```

## Comparing `mypy-boto3-qldb-1.26.0.post1.tar` & `mypy-boto3-qldb-1.26.122.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:51.668842 mypy-boto3-qldb-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-11-01 21:43:51.668842 mypy-boto3-qldb-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12326 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:51.664842 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15305 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15279 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17753 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17726 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:51.668842 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-11-01 21:43:51.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-11-01 21:43:51.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:51.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:51.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:51.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-01 21:43:51.000000 mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:51.668842 mypy-boto3-qldb-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-11-01 21:39:25.000000 mypy-boto3-qldb-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-04-27 19:33:02.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-04-27 19:33:01.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 19:33:42.000000 mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:42.832103 mypy-boto3-qldb-1.26.122/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-27 19:33:00.000000 mypy-boto3-qldb-1.26.122/setup.py
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/LICENSE` & `mypy-boto3-qldb-1.26.122/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/PKG-INFO` & `mypy-boto3-qldb-1.26.122/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.QLDB 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.122
+Summary: Type annotations for boto3.QLDB 1.26.122 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-qldb"></a>
 
 # mypy-boto3-qldb
 
 [![PyPI - mypy-boto3-qldb](https://img.shields.io/pypi/v/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,42 +364,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/README.md` & `mypy-boto3-qldb-1.26.122/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-qldb"></a>
 
 # mypy-boto3-qldb
 
 [![PyPI - mypy-boto3-qldb](https://img.shields.io/pypi/v/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,42 +332,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/__main__.py` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDB 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.QLDB 1.26.122\nVersion:         1.26.122\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.122")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/client.py` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,48 +231,47 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#get_revision)
         """
 
     def list_journal_kinesis_streams_for_ledger(
         self, *, LedgerName: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJournalKinesisStreamsForLedgerResponseTypeDef:
         """
-        Returns an array of all Amazon QLDB journal stream descriptors for a given
-        ledger.
+        Returns all Amazon QLDB journal streams for a given ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_kinesis_streams_for_ledger)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_journal_kinesis_streams_for_ledger)
         """
 
     def list_journal_s3_exports(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJournalS3ExportsResponseTypeDef:
         """
-        Returns an array of journal export job descriptions for all ledgers that are
-        associated with the current Amazon Web Services account and Region.
+        Returns all journal export jobs for all ledgers that are associated with the
+        current Amazon Web Services account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_s3_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_journal_s3_exports)
         """
 
     def list_journal_s3_exports_for_ledger(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJournalS3ExportsForLedgerResponseTypeDef:
         """
-        Returns an array of journal export job descriptions for a specified ledger.
+        Returns all journal export jobs for a specified ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_s3_exports_for_ledger)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_journal_s3_exports_for_ledger)
         """
 
     def list_ledgers(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListLedgersResponseTypeDef:
         """
-        Returns an array of ledger summaries that are associated with the current Amazon
-        Web Services account and Region.
+        Returns all ledgers that are associated with the current Amazon Web Services
+        account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_ledgers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_ledgers)
         """
 
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/client.pyi` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -214,45 +214,44 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#get_revision)
         """
     def list_journal_kinesis_streams_for_ledger(
         self, *, LedgerName: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJournalKinesisStreamsForLedgerResponseTypeDef:
         """
-        Returns an array of all Amazon QLDB journal stream descriptors for a given
-        ledger.
+        Returns all Amazon QLDB journal streams for a given ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_kinesis_streams_for_ledger)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_journal_kinesis_streams_for_ledger)
         """
     def list_journal_s3_exports(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJournalS3ExportsResponseTypeDef:
         """
-        Returns an array of journal export job descriptions for all ledgers that are
-        associated with the current Amazon Web Services account and Region.
+        Returns all journal export jobs for all ledgers that are associated with the
+        current Amazon Web Services account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_s3_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_journal_s3_exports)
         """
     def list_journal_s3_exports_for_ledger(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJournalS3ExportsForLedgerResponseTypeDef:
         """
-        Returns an array of journal export job descriptions for a specified ledger.
+        Returns all journal export jobs for a specified ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_journal_s3_exports_for_ledger)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_journal_s3_exports_for_ledger)
         """
     def list_ledgers(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListLedgersResponseTypeDef:
         """
-        Returns an array of ledger summaries that are associated with the current Amazon
-        Web Services account and Region.
+        Returns all ledgers that are associated with the current Amazon Web Services
+        account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.list_ledgers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/client/#list_ledgers)
         """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns all tags for a specified Amazon QLDB resource.
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/literals.py` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "EncryptionStatusType",
     "ErrorCauseType",
     "ExportStatusType",
     "LedgerStateType",
     "OutputFormatType",
     "PermissionsModeType",
@@ -30,15 +29,14 @@
     "StreamStatusType",
     "QLDBServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 EncryptionStatusType = Literal["ENABLED", "KMS_KEY_INACCESSIBLE", "UPDATING"]
 ErrorCauseType = Literal["IAM_PERMISSION_REVOKED", "KINESIS_STREAM_NOT_FOUND"]
 ExportStatusType = Literal["CANCELLED", "COMPLETED", "IN_PROGRESS"]
 LedgerStateType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 OutputFormatType = Literal["ION_BINARY", "ION_TEXT", "JSON"]
 PermissionsModeType = Literal["ALLOW_ALL", "STANDARD"]
 S3ObjectEncryptionTypeType = Literal["NO_ENCRYPTION", "SSE_KMS", "SSE_S3"]
@@ -64,14 +62,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -81,27 +80,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -130,14 +133,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -182,51 +186,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -258,28 +268,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -288,14 +303,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -306,55 +322,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/literals.pyi` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "EncryptionStatusType",
     "ErrorCauseType",
     "ExportStatusType",
     "LedgerStateType",
     "OutputFormatType",
     "PermissionsModeType",
@@ -29,14 +30,15 @@
     "StreamStatusType",
     "QLDBServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 EncryptionStatusType = Literal["ENABLED", "KMS_KEY_INACCESSIBLE", "UPDATING"]
 ErrorCauseType = Literal["IAM_PERMISSION_REVOKED", "KINESIS_STREAM_NOT_FOUND"]
 ExportStatusType = Literal["CANCELLED", "COMPLETED", "IN_PROGRESS"]
 LedgerStateType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 OutputFormatType = Literal["ION_BINARY", "ION_TEXT", "JSON"]
 PermissionsModeType = Literal["ALLOW_ALL", "STANDARD"]
 S3ObjectEncryptionTypeType = Literal["NO_ENCRYPTION", "SSE_KMS", "SSE_S3"]
@@ -62,14 +64,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -79,27 +82,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -128,14 +135,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -180,51 +188,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -256,28 +270,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -286,14 +305,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -304,55 +324,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/type_defs.py` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb/type_defs.pyi` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/PKG-INFO` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.QLDB 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.122
+Summary: Type annotations for boto3.QLDB 1.26.122 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-qldb"></a>
 
 # mypy-boto3-qldb
 
 [![PyPI - mypy-boto3-qldb](https://img.shields.io/pypi/v/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-qldb?color=blue)](https://pypistats.org/packages/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,42 +364,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-qldb-1.26.0.post1/mypy_boto3_qldb.egg-info/SOURCES.txt` & `mypy-boto3-qldb-1.26.122/mypy_boto3_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.26.0.post1/setup.py` & `mypy-boto3-qldb-1.26.122/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-qldb.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb",
-    version="1.26.0.post1",
+    version="1.26.122",
     packages=["mypy_boto3_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDB 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.QLDB 1.26.122 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 qldb type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_qldb": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_qldb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

