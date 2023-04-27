# Comparing `tmp/resotoeventlog-3.3.4.tar.gz` & `tmp/resotoeventlog-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoeventlog-3.3.4.tar", last modified: Wed Apr 26 16:51:05 2023, max compression
+gzip compressed data, was "resotoeventlog-3.4.0.tar", last modified: Thu Apr 27 11:21:25 2023, max compression
```

## Comparing `resotoeventlog-3.3.4.tar` & `resotoeventlog-3.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:05.888543 resotoeventlog-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 16:51:05.888543 resotoeventlog-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:05.884543 resotoeventlog-3.3.4/resotoeventlog/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:05.888543 resotoeventlog-3.3.4/resotoeventlog/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/logs/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:05.888543 resotoeventlog-3.3.4/resotoeventlog/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:05.888543 resotoeventlog-3.3.4/resotoeventlog/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/resotoeventlog/web/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:05.888543 resotoeventlog-3.3.4/resotoeventlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 16:51:05.000000 resotoeventlog-3.3.4/resotoeventlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-26 16:51:05.000000 resotoeventlog-3.3.4/resotoeventlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:05.000000 resotoeventlog-3.3.4/resotoeventlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 16:51:05.000000 resotoeventlog-3.3.4/resotoeventlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 16:51:05.000000 resotoeventlog-3.3.4/resotoeventlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 16:51:05.000000 resotoeventlog-3.3.4/resotoeventlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 16:51:05.892543 resotoeventlog-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-26 16:49:30.000000 resotoeventlog-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.765789 resotoeventlog-3.4.0/resotoeventlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.765789 resotoeventlog-3.4.0/resotoeventlog/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/logs/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/resotoeventlog/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/resotoeventlog/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/web/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.765789 resotoeventlog-3.4.0/resotoeventlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/setup.py
```

### Comparing `resotoeventlog-3.3.4/resotoeventlog/__main__.py` & `resotoeventlog-3.4.0/resotoeventlog/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/resotoeventlog/logs/log_handler.py` & `resotoeventlog-3.4.0/resotoeventlog/logs/log_handler.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/resotoeventlog/model.py` & `resotoeventlog-3.4.0/resotoeventlog/model.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/resotoeventlog/web/api.py` & `resotoeventlog-3.4.0/resotoeventlog/web/api.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/resotoeventlog/web/directives.py` & `resotoeventlog-3.4.0/resotoeventlog/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/resotoeventlog.egg-info/SOURCES.txt` & `resotoeventlog-3.4.0/resotoeventlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/setup.cfg` & `resotoeventlog-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.4/setup.py` & `resotoeventlog-3.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return [str(requirement) for requirement in pkg_resources.parse_requirements(read(fname))]
 
 
 setup_requirements = ["pytest-runner"]
 
 setup(
     name="resotoeventlog",
-    version="3.3.4",
+    version="3.4.0",
     description="Event log aggregator for resoto.",
     python_requires=">=3.5",
     classifiers=["Programming Language :: Python :: 3"],
     entry_points={"console_scripts": ["resotoeventlog=resotoeventlog.__main__:main"]},
     install_requires=read_requirements("requirements.txt"),
     license="Apache Software License 2.0",
     long_description=read("README.md"),
```

