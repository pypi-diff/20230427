# Comparing `tmp/latch_config-0.1.0.tar.gz` & `tmp/latch_config-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_config-0.1.0.tar", max compression
+gzip compressed data, was "latch_config-0.1.1.tar", max compression
```

## Comparing `latch_config-0.1.0.tar` & `latch_config-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.0/LICENSE
--rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.0/README.md
--rw-r--r--   0        0        0     2050 2023-04-27 20:56:23.022261 latch_config-0.1.0/latch_config/config.py
--rw-r--r--   0        0        0      782 2023-04-27 20:53:01.386593 latch_config-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.0/setup.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.1/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.1/README.md
+-rw-r--r--   0        0        0     2081 2023-04-27 21:03:15.353972 latch_config-0.1.1/latch_config/config.py
+-rw-r--r--   0        0        0      782 2023-04-27 21:03:33.072975 latch_config-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.1/setup.py
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.1/PKG-INFO
```

### Comparing `latch_config-0.1.0/LICENSE` & `latch_config-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.0/latch_config/config.py` & `latch_config-0.1.1/latch_config/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,7 +80,10 @@
                 val = f.default
             else:
                 raise RuntimeError(f"missing value for '{f.name}' (${env_name})")
 
         res[f.name] = val
 
     return x(**res)
+
+
+config = read_config(Config)
```

### Comparing `latch_config-0.1.0/pyproject.toml` & `latch_config-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-config"
-version = "0.1.0"
+version = "0.1.1"
 description = "Shared config for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_config-0.1.0/setup.py` & `latch_config-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['latch_config']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'latch-config',
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

