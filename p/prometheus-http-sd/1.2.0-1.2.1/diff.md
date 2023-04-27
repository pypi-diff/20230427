# Comparing `tmp/prometheus_http_sd-1.2.0.tar.gz` & `tmp/prometheus_http_sd-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.2.0.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.2.1.tar", max compression
```

## Comparing `prometheus_http_sd-1.2.0.tar` & `prometheus_http_sd-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-27 08:15:30.787916 prometheus_http_sd-1.2.0/LICENSE
--rw-r--r--   0        0        0    11097 2023-04-27 08:15:30.787916 prometheus_http_sd-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3400 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     2398 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/config.py
--rw-r--r--   0        0        0       45 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/const.py
--rw-r--r--   0        0        0     6504 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/decorator.py
--rw-r--r--   0        0        0        0 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     1165 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/mem_perf.py
--rw-r--r--   0        0        0     5948 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2118 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2023-04-27 08:15:30.791916 prometheus_http_sd-1.2.0/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      566 2023-04-27 08:15:30.795916 prometheus_http_sd-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11787 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 08:34:14.317610 prometheus_http_sd-1.2.1/LICENSE
+-rw-r--r--   0        0        0    11097 2023-04-27 08:34:14.317610 prometheus_http_sd-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3400 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     2398 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0       45 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/const.py
+-rw-r--r--   0        0        0     6504 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/decorator.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     1165 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/mem_perf.py
+-rw-r--r--   0        0        0     6265 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2118 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      566 2023-04-27 08:34:14.321610 prometheus_http_sd-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11787 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.1/PKG-INFO
```

### Comparing `prometheus_http_sd-1.2.0/LICENSE` & `prometheus_http_sd-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/README.md` & `prometheus_http_sd-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/app.py` & `prometheus_http_sd-1.2.1/prometheus_http_sd/app.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/cli.py` & `prometheus_http_sd-1.2.1/prometheus_http_sd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/decorator.py` & `prometheus_http_sd-1.2.1/prometheus_http_sd/decorator.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/mem_perf.py` & `prometheus_http_sd-1.2.1/prometheus_http_sd/mem_perf.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.2.1/prometheus_http_sd/sd.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,39 +158,52 @@
     result = python_targets_cache.get(key)
     if not result:
         return None
 
     if time.time() - result.created_timestamp > 60:
         return None
 
+    logger.info("Cache hit for key: %s", key)
     return result.value
 
 
 def get_lock(path):
     if path not in python_targets_locks:
         python_targets_locks[path] = Lock()
     return python_targets_locks[path]
 
 
+def get_cache_key(path, **extra_args):
+    keys = sorted(extra_args.keys())
+
+    cache_key = path
+    for key in keys:
+        cache_key += f"/{key}:{extra_args[key]}"
+
+    return cache_key
+
+
 def run_python(generator_path, **extra_args) -> TargetList:
     logger.debug(f"start to import module {generator_path}...")
 
-    cached = _get_cache(generator_path)
+    cache_key = get_cache_key(generator_path, **extra_args)
+
+    cached = _get_cache(cache_key)
     if cached:
         return cached
-    logger.info("%s Cache not hit")
+    logger.info("%s Cache not hit", cache_key)
 
-    lock = get_lock(generator_path)
+    lock = get_lock(cache_key)
 
     with lock:
-        cached = _get_cache(generator_path)
+        cached = _get_cache(cache_key)
         if cached:
-            logger.info("%s Cache hit in lock")
+            logger.info("%s Cache hit in lock", cache_key)
             return cached
-        logger.info("%s Cache not hit in lock, run script...")
+        logger.info("%s Cache not hit in lock, run script...", cache_key)
 
         loader = importlib.machinery.SourceFileLoader(
             "mymodule", generator_path
         )
         spec = importlib.util.spec_from_loader("mymodule", loader)
         if spec:
             mymodule = importlib.util.module_from_spec(spec)
```

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.2.1/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.2.1/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.0/pyproject.toml` & `prometheus_http_sd-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.2.0"
+version = "1.2.1"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Flask = "^2.1.3"
@@ -13,15 +13,15 @@
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.2.0"]
+requires = ["poetry-core>=1.2.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.2.0/PKG-INFO` & `prometheus_http_sd-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-http-sd
-Version: 1.2.0
+Version: 1.2.1
 Summary: Prometheus HTTP SD framework.
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

