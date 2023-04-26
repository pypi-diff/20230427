# Comparing `tmp/graphandlerpy-0.0.1.tar.gz` & `tmp/graphandlerpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\yashn\Desktop\python\dist\.tmp-gpatae9v\graphandlerpy-0.0.1.tar", last modified: Wed Apr 26 20:08:08 2023, max compression
+gzip compressed data, was "C:\Users\yashn\Desktop\python\dist\.tmp-0cmzq2xo\graphandlerpy-0.0.2.tar", last modified: Wed Apr 26 22:53:01 2023, max compression
```

## Comparing `graphandlerpy-0.0.1.tar` & `graphandlerpy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:08:08.284486 graphandlerpy-0.0.1/
--rw-rw-rw-   0        0        0      353 2023-04-26 20:08:08.282487 graphandlerpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-04-26 20:07:09.000000 graphandlerpy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 20:08:08.284486 graphandlerpy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 20:08:08.256491 graphandlerpy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:08:08.265493 graphandlerpy-0.0.1/src/graphandlerpy/
--rw-rw-rw-   0        0        0        0 2023-04-26 19:59:56.000000 graphandlerpy-0.0.1/src/graphandlerpy/__init__.py
--rw-rw-rw-   0        0        0     6614 2023-04-26 20:00:42.000000 graphandlerpy-0.0.1/src/graphandlerpy/ai.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:08:08.279493 graphandlerpy-0.0.1/src/graphandlerpy.egg-info/
--rw-rw-rw-   0        0        0      353 2023-04-26 20:08:08.000000 graphandlerpy-0.0.1/src/graphandlerpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-26 20:08:08.000000 graphandlerpy-0.0.1/src/graphandlerpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:08:08.000000 graphandlerpy-0.0.1/src/graphandlerpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 20:08:08.000000 graphandlerpy-0.0.1/src/graphandlerpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 22:53:01.766158 graphandlerpy-0.0.2/
+-rw-rw-rw-   0        0        0      353 2023-04-26 22:53:01.764135 graphandlerpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-04-26 22:52:41.000000 graphandlerpy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 22:53:01.766158 graphandlerpy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 22:53:01.732087 graphandlerpy-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 22:53:01.741084 graphandlerpy-0.0.2/src/graphandlerpy/
+-rw-rw-rw-   0        0        0        0 2023-04-26 19:59:56.000000 graphandlerpy-0.0.2/src/graphandlerpy/__init__.py
+-rw-rw-rw-   0        0        0     8221 2023-04-26 22:51:38.000000 graphandlerpy-0.0.2/src/graphandlerpy/ai.py
+drwxrwxrwx   0        0        0        0 2023-04-26 22:53:01.760157 graphandlerpy-0.0.2/src/graphandlerpy.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-04-26 22:53:01.000000 graphandlerpy-0.0.2/src/graphandlerpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:53:01.000000 graphandlerpy-0.0.2/src/graphandlerpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 22:53:01.000000 graphandlerpy-0.0.2/src/graphandlerpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 22:53:01.000000 graphandlerpy-0.0.2/src/graphandlerpy.egg-info/top_level.txt
```

