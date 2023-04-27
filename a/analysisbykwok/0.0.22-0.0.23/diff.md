# Comparing `tmp/analysisbykwok-0.0.22.tar.gz` & `tmp/analysisbykwok-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.22.tar", last modified: Thu Apr 27 07:53:22 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.23.tar", last modified: Thu Apr 27 10:34:08 2023, max compression
```

## Comparing `analysisbykwok-0.0.22.tar` & `analysisbykwok-0.0.23.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/
--rw-rw-rw-   0        0        0       62 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/analysisbykwok/
--rw-rw-rw-   0        0        0    17172 2023-04-27 07:52:46.000000 analysisbykwok-0.0.22/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-27 07:52:55.000000 analysisbykwok-0.0.22/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 07:53:22.000000 analysisbykwok-0.0.22/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-04-27 07:52:55.000000 analysisbykwok-0.0.22/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 07:53:22.736614 analysisbykwok-0.0.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 10:34:08.413973 analysisbykwok-0.0.23/
+-rw-rw-rw-   0        0        0       62 2023-04-27 10:34:08.412974 analysisbykwok-0.0.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 10:34:08.409408 analysisbykwok-0.0.23/analysisbykwok/
+-rw-rw-rw-   0        0        0    17172 2023-04-27 10:30:28.000000 analysisbykwok-0.0.23/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-27 10:30:43.000000 analysisbykwok-0.0.23/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:34:08.412974 analysisbykwok-0.0.23/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 10:34:08.000000 analysisbykwok-0.0.23/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-27 10:30:50.000000 analysisbykwok-0.0.23/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:34:08.413973 analysisbykwok-0.0.23/setup.cfg
```

### Comparing `analysisbykwok-0.0.22/analysisbykwok/__init__.py` & `analysisbykwok-0.0.23/analysisbykwok/__init__.py`

 * *Files identical despite different names*

