# Comparing `tmp/resoto-plugin-digitalocean-k8s-3.3.3.tar.gz` & `tmp/resoto-plugin-digitalocean-k8s-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.3.3.tar", last modified: Fri Apr 21 14:35:32 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.3.4.tar", last modified: Wed Apr 26 16:52:35 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-k8s-3.3.3.tar` & `resoto-plugin-digitalocean-k8s-3.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:32.143221 resoto-plugin-digitalocean-k8s-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-21 14:35:32.143221 resoto-plugin-digitalocean-k8s-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:32.143221 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:32.143221 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 14:35:32.000000 resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:35:32.143221 resoto-plugin-digitalocean-k8s-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:32.143221 resoto-plugin-digitalocean-k8s-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-21 14:33:12.000000 resoto-plugin-digitalocean-k8s-3.3.3/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:35.381675 resoto-plugin-digitalocean-k8s-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 16:52:35.385675 resoto-plugin-digitalocean-k8s-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:35.377675 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:35.381675 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 16:52:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:52:35.385675 resoto-plugin-digitalocean-k8s-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:35.381675 resoto-plugin-digitalocean-k8s-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-26 16:49:35.000000 resoto-plugin-digitalocean-k8s-3.3.4/test/test_collector.py
```

### Comparing `resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s/__init__.py` & `resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.3.3/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-k8s-3.3.4/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.3.3/setup.py` & `resoto-plugin-digitalocean-k8s-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-digitalocean-k8s",
-    version="3.3.3",
+    version="3.3.4",
     description="Resoto DigitalOcean-K8s Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": ["digitalocean_k8s_collector = resoto_plugin_digitalocean_k8s:DigitalOceanK8sCollectorPlugin"]
```

### Comparing `resoto-plugin-digitalocean-k8s-3.3.3/test/test_collector.py` & `resoto-plugin-digitalocean-k8s-3.3.4/test/test_collector.py`

 * *Files identical despite different names*

