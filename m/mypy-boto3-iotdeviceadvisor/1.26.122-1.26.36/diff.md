# Comparing `tmp/mypy-boto3-iotdeviceadvisor-1.26.122.tar.gz` & `tmp/mypy-boto3-iotdeviceadvisor-1.26.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.26.122.tar", last modified: Thu Apr 27 19:33:40 2023, max compression
+gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.26.36.tar", last modified: Thu Dec 22 20:32:39 2022, max compression
```

## Comparing `mypy-boto3-iotdeviceadvisor-1.26.122.tar` & `mypy-boto3-iotdeviceadvisor-1.26.36.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:40.656081 mypy-boto3-iotdeviceadvisor-1.26.122/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-04-27 19:33:40.648081 mypy-boto3-iotdeviceadvisor-1.26.122/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:40.648081 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:40.648081 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-04-27 19:33:40.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 19:33:40.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:40.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:40.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:40.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 19:33:40.000000 mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:40.656081 mypy-boto3-iotdeviceadvisor-1.26.122/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 19:32:50.000000 mypy-boto3-iotdeviceadvisor-1.26.122/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.100698 mypy-boto3-iotdeviceadvisor-1.26.36/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2022-12-22 20:32:39.100698 mypy-boto3-iotdeviceadvisor-1.26.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.092698 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.100698 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2022-12-22 20:32:38.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-22 20:32:38.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:32:38.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:32:38.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-22 20:32:38.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-22 20:32:38.000000 mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 20:32:39.100698 mypy-boto3-iotdeviceadvisor-1.26.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2022-12-22 20:32:19.000000 mypy-boto3-iotdeviceadvisor-1.26.36/setup.py
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/LICENSE` & `mypy-boto3-iotdeviceadvisor-1.26.36/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.26.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.26.122
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.36
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.26.36 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-iotdeviceadvisor"></a>
 
 # mypy-boto3-iotdeviceadvisor
 
 [![PyPI - mypy-boto3-iotdeviceadvisor](https://img.shields.io/pypi/v/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,28 +277,27 @@
 ### Literals
 
 `mypy_boto3_iotdeviceadvisor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.literals import (
-    AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
     TestCaseScenarioTypeType,
     IoTDeviceAdvisorServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: AuthenticationMethodType) -> bool:
+def check_value(value: ProtocolType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -351,42 +350,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/README.md` & `mypy-boto3-iotdeviceadvisor-1.26.36/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotdeviceadvisor"></a>
 
 # mypy-boto3-iotdeviceadvisor
 
 [![PyPI - mypy-boto3-iotdeviceadvisor](https://img.shields.io/pypi/v/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -245,28 +245,27 @@
 ### Literals
 
 `mypy_boto3_iotdeviceadvisor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.literals import (
-    AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
     TestCaseScenarioTypeType,
     IoTDeviceAdvisorServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: AuthenticationMethodType) -> bool:
+def check_value(value: ProtocolType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -319,42 +318,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/__main__.py` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.26.122\nVersion:         1.26.122\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTDeviceAdvisor 1.26.36\nVersion:         1.26.36\nBuilder"
+        " version: 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.122")
+    print("1.26.36")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/client.py` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     client: IoTDeviceAdvisorClient = session.client("iotdeviceadvisor")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import AuthenticationMethodType
 from .type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
@@ -117,20 +116,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#generate_presigned_url)
         """
 
     def get_endpoint(
-        self,
-        *,
-        thingArn: str = ...,
-        certificateArn: str = ...,
-        deviceRoleArn: str = ...,
-        authenticationMethod: AuthenticationMethodType = ...
+        self, *, thingArn: str = ..., certificateArn: str = ...
     ) -> GetEndpointResponseTypeDef:
         """
         Gets information about an Device Advisor endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#get_endpoint)
         """
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/client.pyi` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     client: IoTDeviceAdvisorClient = session.client("iotdeviceadvisor")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import AuthenticationMethodType
 from .type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
@@ -108,20 +107,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#generate_presigned_url)
         """
     def get_endpoint(
-        self,
-        *,
-        thingArn: str = ...,
-        certificateArn: str = ...,
-        deviceRoleArn: str = ...,
-        authenticationMethod: AuthenticationMethodType = ...
+        self, *, thingArn: str = ..., certificateArn: str = ...
     ) -> GetEndpointResponseTypeDef:
         """
         Gets information about an Device Advisor endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.get_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#get_endpoint)
         """
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/literals.py` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/literals.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,43 +2,39 @@
 Type annotations for iotdeviceadvisor service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotdeviceadvisor.literals import AuthenticationMethodType
+    from mypy_boto3_iotdeviceadvisor.literals import ProtocolType
 
-    data: AuthenticationMethodType = "SignatureVersion4"
+    data: ProtocolType = "MqttV3_1_1"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
-    "AuthenticationMethodType",
     "ProtocolType",
     "StatusType",
     "SuiteRunStatusType",
     "TestCaseScenarioStatusType",
     "TestCaseScenarioTypeType",
     "IoTDeviceAdvisorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
-AuthenticationMethodType = Literal["SignatureVersion4", "X509ClientCertificate"]
-ProtocolType = Literal["MqttV3_1_1", "MqttV3_1_1_OverWebSocket", "MqttV5", "MqttV5_OverWebSocket"]
+ProtocolType = Literal["MqttV3_1_1", "MqttV5"]
 StatusType = Literal[
     "CANCELED",
     "ERROR",
     "FAIL",
     "PASS",
     "PASS_WITH_WARNINGS",
     "PENDING",
@@ -109,26 +105,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
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
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -214,15 +208,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -233,20 +226,18 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -303,15 +294,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -393,20 +383,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/literals.pyi` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 Type annotations for iotdeviceadvisor service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotdeviceadvisor.literals import AuthenticationMethodType
+    from mypy_boto3_iotdeviceadvisor.literals import ProtocolType
 
-    data: AuthenticationMethodType = "SignatureVersion4"
+    data: ProtocolType = "MqttV3_1_1"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
-    "AuthenticationMethodType",
     "ProtocolType",
     "StatusType",
     "SuiteRunStatusType",
     "TestCaseScenarioStatusType",
     "TestCaseScenarioTypeType",
     "IoTDeviceAdvisorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-AuthenticationMethodType = Literal["SignatureVersion4", "X509ClientCertificate"]
-ProtocolType = Literal["MqttV3_1_1", "MqttV3_1_1_OverWebSocket", "MqttV5", "MqttV5_OverWebSocket"]
+
+ProtocolType = Literal["MqttV3_1_1", "MqttV5"]
 StatusType = Literal[
     "CANCELED",
     "ERROR",
     "FAIL",
     "PASS",
     "PASS_WITH_WARNINGS",
     "PENDING",
@@ -107,26 +107,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
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
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -212,15 +210,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -231,20 +228,18 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -301,15 +296,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -391,20 +385,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/type_defs.py` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
-    AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
     TestCaseScenarioTypeType,
 )
 
@@ -86,26 +85,23 @@
 )
 
 DeviceUnderTestTypeDef = TypedDict(
     "DeviceUnderTestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
-        "deviceRoleArn": str,
     },
     total=False,
 )
 
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
-        "deviceRoleArn": str,
-        "authenticationMethod": AuthenticationMethodType,
     },
     total=False,
 )
 
 _RequiredGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSuiteDefinitionRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor/type_defs.pyi` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
-    AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
     TestCaseScenarioTypeType,
 )
 
@@ -85,26 +84,23 @@
 )
 
 DeviceUnderTestTypeDef = TypedDict(
     "DeviceUnderTestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
-        "deviceRoleArn": str,
     },
     total=False,
 )
 
 GetEndpointRequestRequestTypeDef = TypedDict(
     "GetEndpointRequestRequestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
-        "deviceRoleArn": str,
-        "authenticationMethod": AuthenticationMethodType,
     },
     total=False,
 )
 
 _RequiredGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSuiteDefinitionRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.26.122
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.26.122 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.36
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.26.36 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-iotdeviceadvisor"></a>
 
 # mypy-boto3-iotdeviceadvisor
 
 [![PyPI - mypy-boto3-iotdeviceadvisor](https://img.shields.io/pypi/v/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,28 +277,27 @@
 ### Literals
 
 `mypy_boto3_iotdeviceadvisor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.literals import (
-    AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
     TestCaseScenarioTypeType,
     IoTDeviceAdvisorServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: AuthenticationMethodType) -> bool:
+def check_value(value: ProtocolType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -351,42 +350,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt` & `mypy-boto3-iotdeviceadvisor-1.26.36/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.26.122/setup.py` & `mypy-boto3-iotdeviceadvisor-1.26.36/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-iotdeviceadvisor.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-iotdeviceadvisor",
-    version="1.26.122",
+    version="1.26.36",
     packages=["mypy_boto3_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.26.122 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoTDeviceAdvisor 1.26.36 service generated with"
+        " mypy-boto3-builder 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

