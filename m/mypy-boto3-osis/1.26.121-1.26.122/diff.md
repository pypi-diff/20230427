# Comparing `tmp/mypy-boto3-osis-1.26.121.tar.gz` & `tmp/mypy-boto3-osis-1.26.122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.26.121.tar", last modified: Wed Apr 26 19:32:07 2023, max compression
+gzip compressed data, was "mypy-boto3-osis-1.26.122.tar", last modified: Thu Apr 27 19:33:42 2023, max compression
```

## Comparing `mypy-boto3-osis-1.26.121.tar` & `mypy-boto3-osis-1.26.122.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:32:07.439670 mypy-boto3-osis-1.26.121/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-26 19:32:07.439670 mypy-boto3-osis-1.26.121/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:32:07.439670 mypy-boto3-osis-1.26.121/mypy_boto3_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-26 19:31:58.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-26 19:31:58.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-26 19:31:58.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-26 19:31:58.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-26 19:31:58.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:32:07.439670 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-26 19:32:07.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-26 19:32:07.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:32:07.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:32:07.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 19:32:07.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 19:32:07.000000 mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:32:07.439670 mypy-boto3-osis-1.26.121/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 19:31:57.000000 mypy-boto3-osis-1.26.121/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/mypy_boto3_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-27 19:33:00.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-27 19:33:00.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 19:33:42.000000 mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:33:42.860103 mypy-boto3-osis-1.26.122/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-27 19:32:59.000000 mypy-boto3-osis-1.26.122/setup.py
```

### Comparing `mypy-boto3-osis-1.26.121/LICENSE` & `mypy-boto3-osis-1.26.122/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/PKG-INFO` & `mypy-boto3-osis-1.26.122/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.26.121
-Summary: Type annotations for boto3.OpenSearchIngestion 1.26.121 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.122
+Summary: Type annotations for boto3.OpenSearchIngestion 1.26.122 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.26.121](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-osis-1.26.121/README.md` & `mypy-boto3-osis-1.26.122/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.26.121](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/__main__.py` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchIngestion 1.26.121\nVersion:        "
-        " 1.26.121\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpenSearchIngestion 1.26.122\nVersion:        "
+        " 1.26.122\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.121")
+    print("1.26.122")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/client.py` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/client.pyi` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/literals.py` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/literals.pyi` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/type_defs.py` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis/type_defs.pyi` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/PKG-INFO` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.26.121
-Summary: Type annotations for boto3.OpenSearchIngestion 1.26.121 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.122
+Summary: Type annotations for boto3.OpenSearchIngestion 1.26.122 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.26.121](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.26.122](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-osis-1.26.121/mypy_boto3_osis.egg-info/SOURCES.txt` & `mypy-boto3-osis-1.26.122/mypy_boto3_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.26.121/setup.py` & `mypy-boto3-osis-1.26.122/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-osis",
-    version="1.26.121",
+    version="1.26.122",
     packages=["mypy_boto3_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchIngestion 1.26.121 service generated with"
+        "Type annotations for boto3.OpenSearchIngestion 1.26.122 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

