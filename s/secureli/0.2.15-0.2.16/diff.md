# Comparing `tmp/secureli-0.2.15.tar.gz` & `tmp/secureli-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.2.15.tar", max compression
+gzip compressed data, was "secureli-0.2.16.tar", max compression
```

## Comparing `secureli-0.2.15.tar` & `secureli-0.2.16.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11358 2023-04-24 20:24:13.308241 secureli-0.2.15/LICENSE
--rw-r--r--   0        0        0    10572 2023-04-24 20:24:13.308241 secureli-0.2.15/README.md
--rw-r--r--   0        0        0     1781 2023-04-24 20:24:13.308241 secureli-0.2.15/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    30307 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10747 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10013 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/scan.py
--rw-r--r--   0        0        0      787 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-04-24 20:24:13.308241 secureli-0.2.15/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/main.py
--rw-r--r--   0        0        0        0 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3884 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/build.txt
--rw-r--r--   0        0        0     1271 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      478 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      619 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      409 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      642 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2211 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/language_support.py
--rw-r--r--   0        0        0     4090 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-04-24 20:24:13.312241 secureli-0.2.15/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0    11370 1970-01-01 00:00:00.000000 secureli-0.2.15/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-27 17:31:56.805059 secureli-0.2.16/LICENSE
+-rw-r--r--   0        0        0    10572 2023-04-27 17:31:56.805059 secureli-0.2.16/README.md
+-rw-r--r--   0        0        0     1781 2023-04-27 17:31:56.805059 secureli-0.2.16/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    30307 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10747 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10013 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/scan.py
+-rw-r--r--   0        0        0      787 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3884 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0     1271 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      478 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      619 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      409 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      642 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2211 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4090 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-04-27 17:31:56.805059 secureli-0.2.16/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0    11370 1970-01-01 00:00:00.000000 secureli-0.2.16/PKG-INFO
```

### Comparing `secureli-0.2.15/LICENSE` & `secureli-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/README.md` & `secureli-0.2.16/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/pyproject.toml` & `secureli-0.2.16/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.2.15"
+version = "0.2.16"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.2.15/secureli/abstractions/echo.py` & `secureli-0.2.16/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/abstractions/lexer_guesser.py` & `secureli-0.2.16/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/abstractions/pre_commit.py` & `secureli-0.2.16/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/actions/action.py` & `secureli-0.2.16/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/actions/build.py` & `secureli-0.2.16/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/actions/initializer.py` & `secureli-0.2.16/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/actions/scan.py` & `secureli-0.2.16/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/actions/setup.py` & `secureli-0.2.16/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/actions/update.py` & `secureli-0.2.16/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/container.py` & `secureli-0.2.16/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/main.py` & `secureli-0.2.16/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/repositories/repo_files.py` & `secureli-0.2.16/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/repositories/secureli_config.py` & `secureli-0.2.16/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/repositories/settings.py` & `secureli-0.2.16/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/files/build.txt` & `secureli-0.2.16/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.2.16/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.2.16/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.2.16/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.2.16/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/read_resource.py` & `secureli-0.2.16/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/resources/slugify.py` & `secureli-0.2.16/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/git_ignore.py` & `secureli-0.2.16/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/language_analyzer.py` & `secureli-0.2.16/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/language_support.py` & `secureli-0.2.16/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/logging.py` & `secureli-0.2.16/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/scanner.py` & `secureli-0.2.16/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/secureli_ignore.py` & `secureli-0.2.16/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/services/updater.py` & `secureli-0.2.16/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/settings.py` & `secureli-0.2.16/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/utilities/git_meta.py` & `secureli-0.2.16/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/secureli/utilities/patterns.py` & `secureli-0.2.16/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.2.15/PKG-INFO` & `secureli-0.2.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.2.15
+Version: 0.2.16
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

