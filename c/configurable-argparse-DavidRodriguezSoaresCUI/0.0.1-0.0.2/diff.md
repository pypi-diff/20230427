# Comparing `tmp/configurable_argparse_DavidRodriguezSoaresCUI-0.0.1.tar.gz` & `tmp/configurable_argparse_DavidRodriguezSoaresCUI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configurable_argparse_DavidRodriguezSoaresCUI-0.0.1.tar", last modified: Sat Apr 22 17:58:53 2023, max compression
+gzip compressed data, was "configurable_argparse_DavidRodriguezSoaresCUI-0.0.2.tar", last modified: Thu Apr 27 20:19:34 2023, max compression
```

## Comparing `configurable_argparse_DavidRodriguezSoaresCUI-0.0.1.tar` & `configurable_argparse_DavidRodriguezSoaresCUI-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 17:58:53.038501 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/
--rw-rw-rw-   0        0        0     6430 2023-04-22 17:10:32.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     7638 2023-04-22 17:58:53.037499 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-22 17:10:32.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/README.md
--rw-rw-rw-   0        0        0      929 2023-04-22 17:18:46.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 17:58:53.038501 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 17:58:53.027490 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/
--rw-rw-rw-   0        0        0     7664 2023-04-22 17:46:52.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:58:53.037499 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     7638 2023-04-22 17:58:53.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-04-22 17:58:53.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 17:58:53.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-22 17:58:53.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-22 17:58:53.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 20:19:34.202509 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/
+-rw-rw-rw-   0        0        0     6430 2023-04-22 17:10:32.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    10696 2023-04-27 20:19:34.201509 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3265 2023-04-22 18:51:06.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/README.md
+-rw-rw-rw-   0        0        0      927 2023-04-27 20:17:11.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 20:19:34.202509 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 20:19:34.180491 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/
+-rw-rw-rw-   0        0        0     7676 2023-04-27 20:14:24.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse.py
+drwxrwxrwx   0        0        0        0 2023-04-27 20:19:34.201509 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0    10696 2023-04-27 20:19:34.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-27 20:19:34.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 20:19:34.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-27 20:19:34.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-27 20:19:34.000000 configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/LICENSE` & `configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/pyproject.toml` & `configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "configurable_argparse_DavidRodriguezSoaresCUI"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="DavidRodriguezSoaresCUI", email="fireblaze904+argparse@gmail.com" },
 ]
-description = "Argparse-based way of CLI argument management boosted by YAML reusable configurations"
+description = "Argparse-based way of CLI argument handling boosted by YAML reusable configurations"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
```

### Comparing `configurable_argparse_DavidRodriguezSoaresCUI-0.0.1/src/configurable_argparse.py` & `configurable_argparse_DavidRodriguezSoaresCUI-0.0.2/src/configurable_argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         )
         _spacer = "" if len(_help) == 0 else " "
         self.kwargs["help"] = _help + _spacer + f"Default: {_default_repr}"
 
     def is_present_in_namespace(self, namespace: argparse.Namespace) -> bool:
         """Checks whether group is represented in namespace"""
         for name in self.names:
-            if hasattr(namespace, name.lstrip("-")):
+            if getattr(namespace, name.lstrip("-"), None) is not None:
                 return True
         return False
 
     def add_argument(
         self,
         parser: Union[argparse.ArgumentParser, argparse._MutuallyExclusiveGroup],
         reserved_name: str,
@@ -166,16 +166,16 @@
             setattr(namespace, k, v)
 
     # Ensure required arguments are present
     for arg in arguments:
         if arg.required:
             assertTrue(
                 arg.is_present_in_namespace(namespace),
-                "Error: one of the arguments {} is required. namespace={}",
-                arg,
+                "Error: argument {} is required. namespace={}",
+                arg.names,
                 namespace,
             )
 
     if not cfg:
         user_input = input(
             "Save arguments into YAML config file for later use (leave blank to skip) ? "
         )
```

