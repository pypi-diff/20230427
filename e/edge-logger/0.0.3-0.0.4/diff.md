# Comparing `tmp/edge_logger-0.0.3.tar.gz` & `tmp/edge_logger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_logger-0.0.3.tar", max compression
+gzip compressed data, was "edge_logger-0.0.4.tar", max compression
```

## Comparing `edge_logger-0.0.3.tar` & `edge_logger-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.3/edge_logger/__init__.py
--rw-r--r--   0        0        0     3726 2023-04-18 04:37:54.415892 edge_logger-0.0.3/edge_logger/edge_logger.py
--rw-r--r--   0        0        0      359 2023-04-18 04:38:13.960200 edge_logger-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 edge_logger-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.4/edge_logger/__init__.py
+-rw-r--r--   0        0        0     5325 2023-04-27 03:18:19.983133 edge_logger-0.0.4/edge_logger/edge_logger.py
+-rw-r--r--   0        0        0      380 2023-04-27 03:23:08.613589 edge_logger-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.4/PKG-INFO
```

### Comparing `edge_logger-0.0.3/LICENSE` & `edge_logger-0.0.4/LICENSE`

 * *Files identical despite different names*

