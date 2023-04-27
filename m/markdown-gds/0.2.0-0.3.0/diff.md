# Comparing `tmp/markdown-gds-0.2.0.tar.gz` & `tmp/markdown_gds-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-gds-0.2.0.tar", max compression
+gzip compressed data, was "markdown_gds-0.3.0.tar", max compression
```

## Comparing `markdown-gds-0.2.0.tar` & `markdown_gds-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1091 2022-08-05 13:56:44.101531 markdown-gds-0.2.0/LICENSE
--rw-r--r--   0        0        0       36 2022-08-05 11:40:52.963385 markdown-gds-0.2.0/markdown_gds/__init__.py
--rw-r--r--   0        0        0     1034 2022-08-08 10:53:44.011677 markdown-gds-0.2.0/markdown_gds/extension.py
--rw-r--r--   0        0        0      411 2022-08-08 11:06:43.535065 markdown-gds-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      644 2022-08-08 11:07:24.237423 markdown-gds-0.2.0/setup.py
--rw-r--r--   0        0        0      338 2022-08-08 11:07:24.237563 markdown-gds-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-08-05 13:56:44.101531 markdown_gds-0.3.0/LICENSE
+-rw-r--r--   0        0        0       36 2022-08-05 11:40:52.963385 markdown_gds-0.3.0/markdown_gds/__init__.py
+-rw-r--r--   0        0        0     1412 2023-04-27 12:34:46.359257 markdown_gds-0.3.0/markdown_gds/extension.py
+-rw-r--r--   0        0        0      411 2023-04-27 12:43:57.563866 markdown_gds-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 markdown_gds-0.3.0/PKG-INFO
```

### Comparing `markdown-gds-0.2.0/LICENSE` & `markdown_gds-0.3.0/LICENSE`

 * *Files identical despite different names*

