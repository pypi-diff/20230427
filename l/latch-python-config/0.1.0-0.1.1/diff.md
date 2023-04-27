# Comparing `tmp/latch_python_config-0.1.0.tar.gz` & `tmp/latch_python_config-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_python_config-0.1.0.tar", max compression
+gzip compressed data, was "latch_python_config-0.1.1.tar", max compression
```

## Comparing `latch_python_config-0.1.0.tar` & `latch_python_config-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_python_config-0.1.0/LICENSE
--rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_python_config-0.1.0/README.md
--rw-r--r--   0        0        0     2252 2023-04-27 16:46:35.474156 latch_python_config-0.1.0/latch_python_config/config.py
--rw-r--r--   0        0        0      792 2023-04-27 17:03:41.028753 latch_python_config-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 latch_python_config-0.1.0/setup.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 latch_python_config-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_python_config-0.1.1/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_python_config-0.1.1/README.md
+-rw-r--r--   0        0        0     2252 2023-04-27 16:46:35.474156 latch_python_config-0.1.1/latch_python_config/config.py
+-rw-r--r--   0        0        0      796 2023-04-27 17:13:03.729319 latch_python_config-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 latch_python_config-0.1.1/setup.py
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 latch_python_config-0.1.1/PKG-INFO
```

### Comparing `latch_python_config-0.1.0/LICENSE` & `latch_python_config-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_python_config-0.1.0/latch_python_config/config.py` & `latch_python_config-0.1.1/latch_python_config/config.py`

 * *Files identical despite different names*

### Comparing `latch_python_config-0.1.0/pyproject.toml` & `latch_python_config-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "latch-python-config"
-version = "0.1.0"
+version = "0.1.1"
 description = "Shared config for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
-license = "CC0"
+license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_python_config"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `latch_python_config-0.1.0/setup.py` & `latch_python_config-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['latch_python_config']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'latch-python-config',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Shared config for latch python backend services',
     'long_description': '# python-config\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

