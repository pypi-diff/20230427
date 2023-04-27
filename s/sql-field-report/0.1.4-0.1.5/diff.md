# Comparing `tmp/sql_field_report-0.1.4.tar.gz` & `tmp/sql_field_report-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.1.4.tar", max compression
+gzip compressed data, was "sql_field_report-0.1.5.tar", max compression
```

## Comparing `sql_field_report-0.1.4.tar` & `sql_field_report-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      676 2023-04-27 15:18:44.287215 sql_field_report-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.4/sql_field_report/__init__.py
--rw-r--r--   0        0        0       68 2023-04-27 13:15:20.467845 sql_field_report-0.1.4/sql_field_report/__main__.py
--rw-r--r--   0        0        0    11743 2023-04-27 15:16:27.718777 sql_field_report-0.1.4/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 sql_field_report-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      676 2023-04-27 15:21:47.585955 sql_field_report-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 11:53:49.547739 sql_field_report-0.1.5/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-27 13:15:20.467845 sql_field_report-0.1.5/sql_field_report/__main__.py
+-rw-r--r--   0        0        0    11751 2023-04-27 15:21:41.034351 sql_field_report-0.1.5/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 sql_field_report-0.1.5/PKG-INFO
```

### Comparing `sql_field_report-0.1.4/pyproject.toml` & `sql_field_report-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `sql_field_report-0.1.4/README.md` & `sql_field_report-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.1.4/sql_field_report/sql_field_report.py` & `sql_field_report-0.1.5/sql_field_report/sql_field_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,12 +365,12 @@
     if not output_file_name.endswith(".xlsx"):
         output_file_name = "{}.xlsx".format(output_file_name.split(".")[0])
 
     with MSSQLConnection(server, port, user, password, database_name) as conn:
         objects = pd.read_sql(
             text("SELECT DISTINCT(TABLE_NAME) FROM INFORMATION_SCHEMA.COLUMNS"), conn
         )["TABLE_NAME"].to_list()
-        build_field_report(output_file_name, objects, conn)
+        build_field_report(output_file_name, objects, schema, conn)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `sql_field_report-0.1.4/PKG-INFO` & `sql_field_report-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```

