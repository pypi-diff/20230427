# Comparing `tmp/syncthing2-2.4.4.tar.gz` & `tmp/syncthing2-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncthing2-2.4.4.tar", last modified: Thu Mar 23 13:55:22 2023, max compression
+gzip compressed data, was "syncthing2-2.4.5.tar", last modified: Thu Apr 27 12:48:27 2023, max compression
```

## Comparing `syncthing2-2.4.4.tar` & `syncthing2-2.4.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-03-23 13:55:22.119629 syncthing2-2.4.4/
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1091 2023-01-31 13:47:14.000000 syncthing2-2.4.4/LICENSE
--rw-r--r--   0 wangx     (1000) wangx     (1000)       46 2023-01-31 13:47:14.000000 syncthing2-2.4.4/MANIFEST.in
--rw-r--r--   0 wangx     (1000) wangx     (1000)      882 2023-03-23 13:55:22.119629 syncthing2-2.4.4/PKG-INFO
--rw-r--r--   0 wangx     (1000) wangx     (1000)     3103 2023-01-31 13:47:14.000000 syncthing2-2.4.4/README.md
--rw-r--r--   0 wangx     (1000) wangx     (1000)       79 2023-03-23 13:55:22.122625 syncthing2-2.4.4/setup.cfg
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1385 2023-03-21 14:28:47.000000 syncthing2-2.4.4/setup.py
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-03-23 13:55:22.065522 syncthing2-2.4.4/syncthing/
--rw-r--r--   0 wangx     (1000) wangx     (1000)    32179 2023-01-31 13:47:14.000000 syncthing2-2.4.4/syncthing/__init__.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)      888 2023-01-31 13:47:14.000000 syncthing2-2.4.4/syncthing/meta.py
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-03-23 13:55:22.093654 syncthing2-2.4.4/syncthing2.egg-info/
--rw-r--r--   0 wangx     (1000) wangx     (1000)      882 2023-03-23 13:55:21.000000 syncthing2-2.4.4/syncthing2.egg-info/PKG-INFO
--rw-r--r--   0 wangx     (1000) wangx     (1000)      365 2023-03-23 13:55:21.000000 syncthing2-2.4.4/syncthing2.egg-info/SOURCES.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2023-03-23 13:55:21.000000 syncthing2-2.4.4/syncthing2.egg-info/dependency_links.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)      105 2023-03-23 13:55:21.000000 syncthing2-2.4.4/syncthing2.egg-info/requires.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)       10 2023-03-23 13:55:21.000000 syncthing2-2.4.4/syncthing2.egg-info/top_level.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2023-01-31 13:48:41.000000 syncthing2-2.4.4/syncthing2.egg-info/zip-safe
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-03-23 13:55:22.117661 syncthing2-2.4.4/tests/
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1859 2023-01-31 13:47:14.000000 syncthing2-2.4.4/tests/test_parse_datetime.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1963 2023-01-31 13:47:14.000000 syncthing2-2.4.4/tests/test_scan_folder.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)     3415 2023-01-31 13:47:14.000000 syncthing2-2.4.4/tests/test_syncthing.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-04-27 12:48:27.845206 syncthing2-2.4.5/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1091 2023-01-31 13:47:14.000000 syncthing2-2.4.5/LICENSE
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       46 2023-01-31 13:47:14.000000 syncthing2-2.4.5/MANIFEST.in
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     4026 2023-04-27 12:48:27.845206 syncthing2-2.4.5/PKG-INFO
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     3103 2023-01-31 13:47:14.000000 syncthing2-2.4.5/README.md
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       79 2023-04-27 12:48:27.848199 syncthing2-2.4.5/setup.cfg
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1714 2023-04-27 12:47:54.000000 syncthing2-2.4.5/setup.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-04-27 12:48:27.818284 syncthing2-2.4.5/syncthing/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)    32179 2023-01-31 13:47:14.000000 syncthing2-2.4.5/syncthing/__init__.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      888 2023-01-31 13:47:14.000000 syncthing2-2.4.5/syncthing/meta.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-04-27 12:48:27.840220 syncthing2-2.4.5/syncthing2.egg-info/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     4026 2023-04-27 12:48:27.000000 syncthing2-2.4.5/syncthing2.egg-info/PKG-INFO
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      365 2023-04-27 12:48:27.000000 syncthing2-2.4.5/syncthing2.egg-info/SOURCES.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2023-04-27 12:48:27.000000 syncthing2-2.4.5/syncthing2.egg-info/dependency_links.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      100 2023-04-27 12:48:27.000000 syncthing2-2.4.5/syncthing2.egg-info/requires.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       10 2023-04-27 12:48:27.000000 syncthing2-2.4.5/syncthing2.egg-info/top_level.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2023-01-31 13:48:41.000000 syncthing2-2.4.5/syncthing2.egg-info/zip-safe
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2023-04-27 12:48:27.844209 syncthing2-2.4.5/tests/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1859 2023-01-31 13:47:14.000000 syncthing2-2.4.5/tests/test_parse_datetime.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1963 2023-01-31 13:47:14.000000 syncthing2-2.4.5/tests/test_scan_folder.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     3415 2023-01-31 13:47:14.000000 syncthing2-2.4.5/tests/test_syncthing.py
```

### Comparing `syncthing2-2.4.4/LICENSE` & `syncthing2-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syncthing2-2.4.4/README.md` & `syncthing2-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `syncthing2-2.4.4/syncthing/__init__.py` & `syncthing2-2.4.5/syncthing/__init__.py`

 * *Files identical despite different names*

### Comparing `syncthing2-2.4.4/syncthing/meta.py` & `syncthing2-2.4.5/syncthing/meta.py`

 * *Files identical despite different names*

### Comparing `syncthing2-2.4.4/tests/test_parse_datetime.py` & `syncthing2-2.4.5/tests/test_parse_datetime.py`

 * *Files identical despite different names*

### Comparing `syncthing2-2.4.4/tests/test_scan_folder.py` & `syncthing2-2.4.5/tests/test_scan_folder.py`

 * *Files identical despite different names*

### Comparing `syncthing2-2.4.4/tests/test_syncthing.py` & `syncthing2-2.4.5/tests/test_syncthing.py`

 * *Files identical despite different names*

