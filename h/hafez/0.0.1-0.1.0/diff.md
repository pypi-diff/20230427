# Comparing `tmp/hafez-0.0.1.tar.gz` & `tmp/hafez-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hafez-0.0.1.tar", last modified: Tue Apr 25 23:40:33 2023, max compression
+gzip compressed data, was "hafez-0.1.0.tar", last modified: Thu Apr 27 00:41:49 2023, max compression
```

## Comparing `hafez-0.0.1.tar` & `hafez-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-25 23:40:33.574652 hafez-0.0.1/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1073 2023-04-25 23:36:29.000000 hafez-0.0.1/LICENSE
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       40 2023-03-28 05:39:02.000000 hafez-0.0.1/MANIFEST.in
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      492 2023-04-25 23:40:33.574513 hafez-0.0.1/PKG-INFO
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       20 2023-04-25 23:36:29.000000 hafez-0.0.1/README.md
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-25 23:40:33.574347 hafez-0.0.1/hafez.egg-info/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      492 2023-04-25 23:40:33.000000 hafez-0.0.1/hafez.egg-info/PKG-INFO
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      214 2023-04-25 23:40:33.000000 hafez-0.0.1/hafez.egg-info/SOURCES.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-25 23:40:33.000000 hafez-0.0.1/hafez.egg-info/dependency_links.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       48 2023-04-25 23:40:33.000000 hafez-0.0.1/hafez.egg-info/requires.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-25 23:40:33.000000 hafez-0.0.1/hafez.egg-info/top_level.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      465 2023-04-25 23:39:37.000000 hafez-0.0.1/pyproject.toml
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       47 2023-04-25 23:39:49.000000 hafez-0.0.1/requirements.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       38 2023-04-25 23:40:33.574704 hafez-0.0.1/setup.cfg
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      365 2023-03-28 05:53:03.000000 hafez-0.0.1/setup.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.333198 hafez-0.1.0/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1073 2023-04-25 23:36:29.000000 hafez-0.1.0/LICENSE
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       40 2023-03-28 05:39:02.000000 hafez-0.1.0/MANIFEST.in
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 00:41:49.333025 hafez-0.1.0/PKG-INFO
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     2563 2023-04-26 03:17:25.000000 hafez-0.1.0/README.md
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.331322 hafez-0.1.0/hafez/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      130 2023-04-26 02:31:37.000000 hafez-0.1.0/hafez/__init__.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1281 2023-04-26 03:08:57.000000 hafez-0.1.0/hafez/main.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.332383 hafez-0.1.0/hafez/utils/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-26 01:48:50.000000 hafez-0.1.0/hafez/utils/__init__.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1229 2023-04-27 00:30:32.000000 hafez-0.1.0/hafez/utils/db.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      792 2023-04-26 02:32:50.000000 hafez-0.1.0/hafez/utils/formating.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.331991 hafez-0.1.0/hafez.egg-info/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/PKG-INFO
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      313 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/SOURCES.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/dependency_links.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/requires.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        6 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/top_level.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      465 2023-04-26 02:35:56.000000 hafez-0.1.0/pyproject.toml
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-26 02:13:01.000000 hafez-0.1.0/requirements.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       38 2023-04-27 00:41:49.333243 hafez-0.1.0/setup.cfg
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      365 2023-03-28 05:53:03.000000 hafez-0.1.0/setup.py
```

### Comparing `hafez-0.0.1/LICENSE` & `hafez-0.1.0/LICENSE`

 * *Files identical despite different names*

