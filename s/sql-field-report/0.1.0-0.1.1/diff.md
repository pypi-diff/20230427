# Comparing `tmp/sql_field_report-0.1.0.tar.gz` & `tmp/sql_field_report-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.1.0.tar", max compression
+gzip compressed data, was "sql_field_report-0.1.1.tar", max compression
```

## Comparing `sql_field_report-0.1.0.tar` & `sql_field_report-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      675 2023-04-27 11:50:04.996284 sql_field_report-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 11:26:45.567266 sql_field_report-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.0/sql_field_report/__init__.py
--rw-r--r--   0        0        0    11592 2023-04-27 11:48:21.413755 sql_field_report-0.1.0/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 sql_field_report-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      676 2023-04-27 13:15:52.188736 sql_field_report-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-04-27 12:33:08.136098 sql_field_report-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.1/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-27 13:15:20.467845 sql_field_report-0.1.1/sql_field_report/__main__.py
+-rw-r--r--   0        0        0    11592 2023-04-27 11:48:21.413755 sql_field_report-0.1.1/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 sql_field_report-0.1.1/PKG-INFO
```

### Comparing `sql_field_report-0.1.0/sql_field_report/sql_field_report.py` & `sql_field_report-0.1.1/sql_field_report/sql_field_report.py`

 * *Files identical despite different names*

