# Comparing `tmp/latch_o11y-0.1.0.tar.gz` & `tmp/latch_o11y-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_o11y-0.1.0.tar", max compression
+gzip compressed data, was "latch_o11y-0.1.1.tar", max compression
```

## Comparing `latch_o11y-0.1.0.tar` & `latch_o11y-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.0/LICENSE
--rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.0/README.md
--rw-r--r--   0        0        0     6840 2023-04-27 21:02:53.439523 latch_o11y-0.1.0/latch_o11y/o11y.py
--rw-r--r--   0        0        0      953 2023-04-27 21:16:43.221224 latch_o11y-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.0/setup.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.1/LICENSE
+-rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.1/README.md
+-rw-r--r--   0        0        0     6840 2023-04-27 21:02:53.439523 latch_o11y-0.1.1/latch_o11y/o11y.py
+-rw-r--r--   0        0        0      953 2023-04-27 21:19:48.977493 latch_o11y-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.1/setup.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.1/PKG-INFO
```

### Comparing `latch_o11y-0.1.0/LICENSE` & `latch_o11y-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_o11y-0.1.0/latch_o11y/o11y.py` & `latch_o11y-0.1.1/latch_o11y/o11y.py`

 * *Files identical despite different names*

### Comparing `latch_o11y-0.1.0/pyproject.toml` & `latch_o11y-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-o11y"
-version = "0.1.0"
+version = "0.1.1"
 description = "Observability for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_o11y"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_o11y-0.1.0/setup.py` & `latch_o11y-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'opentelemetry-exporter-otlp-proto-grpc>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'orjson>=3.8.5,<4.0.0',
  'structlog>=22.3.0,<23.0.0']
 
 setup_kwargs = {
     'name': 'latch-o11y',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Observability for latch python backend services',
     'long_description': '# python-o11y\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_o11y-0.1.0/PKG-INFO` & `latch_o11y-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-o11y
-Version: 0.1.0
+Version: 0.1.1
 Summary: Observability for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

