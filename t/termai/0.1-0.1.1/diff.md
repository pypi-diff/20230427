# Comparing `tmp/termai-0.1.tar.gz` & `tmp/termai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termai-0.1.tar", last modified: Wed Apr 26 20:36:03 2023, max compression
+gzip compressed data, was "termai-0.1.1.tar", last modified: Wed Apr 26 23:01:59 2023, max compression
```

## Comparing `termai-0.1.tar` & `termai-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brad      (1000) users      (984)        0 2023-04-26 20:36:03.290490 termai-0.1/
--rw-r--r--   0 brad      (1000) users      (984)      216 2023-04-26 20:36:03.290490 termai-0.1/PKG-INFO
--rw-r--r--   0 brad      (1000) users      (984)     1938 2023-04-26 20:24:19.000000 termai-0.1/README.md
--rw-r--r--   0 brad      (1000) users      (984)       38 2023-04-26 20:36:03.290490 termai-0.1/setup.cfg
--rw-r--r--   0 brad      (1000) users      (984)      581 2023-04-26 20:34:11.000000 termai-0.1/setup.py
-drwxr-xr-x   0 brad      (1000) users      (984)        0 2023-04-26 20:36:03.290490 termai-0.1/termai/
--rw-r--r--   0 brad      (1000) users      (984)        0 2023-04-26 20:34:38.000000 termai-0.1/termai/__init__.py
--rwxr-xr-x   0 brad      (1000) users      (984)      727 2023-04-26 20:35:20.000000 termai-0.1/termai/termchat.py
--rwxr-xr-x   0 brad      (1000) users      (984)     1218 2023-04-26 20:35:34.000000 termai-0.1/termai/termpics.py
-drwxr-xr-x   0 brad      (1000) users      (984)        0 2023-04-26 20:36:03.290490 termai-0.1/termai.egg-info/
--rw-r--r--   0 brad      (1000) users      (984)      216 2023-04-26 20:36:03.000000 termai-0.1/termai.egg-info/PKG-INFO
--rw-r--r--   0 brad      (1000) users      (984)      257 2023-04-26 20:36:03.000000 termai-0.1/termai.egg-info/SOURCES.txt
--rw-r--r--   0 brad      (1000) users      (984)        1 2023-04-26 20:36:03.000000 termai-0.1/termai.egg-info/dependency_links.txt
--rw-r--r--   0 brad      (1000) users      (984)       82 2023-04-26 20:36:03.000000 termai-0.1/termai.egg-info/entry_points.txt
--rw-r--r--   0 brad      (1000) users      (984)       59 2023-04-26 20:36:03.000000 termai-0.1/termai.egg-info/requires.txt
--rw-r--r--   0 brad      (1000) users      (984)        7 2023-04-26 20:36:03.000000 termai-0.1/termai.egg-info/top_level.txt
+drwxr-xr-x   0 brad      (1000) users      (984)        0 2023-04-26 23:01:59.334071 termai-0.1.1/
+-rw-r--r--   0 brad      (1000) users      (984)      182 2023-04-26 23:01:59.334071 termai-0.1.1/PKG-INFO
+-rw-r--r--   0 brad      (1000) users      (984)     1938 2023-04-26 20:24:19.000000 termai-0.1.1/README.md
+-rw-r--r--   0 brad      (1000) users      (984)       38 2023-04-26 23:01:59.334071 termai-0.1.1/setup.cfg
+-rw-r--r--   0 brad      (1000) users      (984)      564 2023-04-26 23:01:55.000000 termai-0.1.1/setup.py
+drwxr-xr-x   0 brad      (1000) users      (984)        0 2023-04-26 23:01:59.334071 termai-0.1.1/termai/
+-rw-r--r--   0 brad      (1000) users      (984)       27 2023-04-26 22:58:04.000000 termai-0.1.1/termai/__init__.py
+-rwxr-xr-x   0 brad      (1000) users      (984)      727 2023-04-26 20:35:20.000000 termai-0.1.1/termai/termchat.py
+-rwxr-xr-x   0 brad      (1000) users      (984)     1218 2023-04-26 20:35:34.000000 termai-0.1.1/termai/termpics.py
+drwxr-xr-x   0 brad      (1000) users      (984)        0 2023-04-26 23:01:59.334071 termai-0.1.1/termai.egg-info/
+-rw-r--r--   0 brad      (1000) users      (984)      182 2023-04-26 23:01:59.000000 termai-0.1.1/termai.egg-info/PKG-INFO
+-rw-r--r--   0 brad      (1000) users      (984)      257 2023-04-26 23:01:59.000000 termai-0.1.1/termai.egg-info/SOURCES.txt
+-rw-r--r--   0 brad      (1000) users      (984)        1 2023-04-26 23:01:59.000000 termai-0.1.1/termai.egg-info/dependency_links.txt
+-rw-r--r--   0 brad      (1000) users      (984)       82 2023-04-26 23:01:59.000000 termai-0.1.1/termai.egg-info/entry_points.txt
+-rw-r--r--   0 brad      (1000) users      (984)       59 2023-04-26 23:01:59.000000 termai-0.1.1/termai.egg-info/requires.txt
+-rw-r--r--   0 brad      (1000) users      (984)        7 2023-04-26 23:01:59.000000 termai-0.1.1/termai.egg-info/top_level.txt
```

### Comparing `termai-0.1/README.md` & `termai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `termai-0.1/termai/termchat.py` & `termai-0.1.1/termai/termchat.py`

 * *Files identical despite different names*

### Comparing `termai-0.1/termai/termpics.py` & `termai-0.1.1/termai/termpics.py`

 * *Files identical despite different names*

