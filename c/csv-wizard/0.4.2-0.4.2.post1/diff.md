# Comparing `tmp/csv-wizard-0.4.2.tar.gz` & `tmp/csv-wizard-0.4.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-wizard-0.4.2.tar", last modified: Wed Apr 26 13:37:01 2023, max compression
+gzip compressed data, was "csv-wizard-0.4.2.post1.tar", last modified: Thu Apr 27 20:09:19 2023, max compression
```

## Comparing `csv-wizard-0.4.2.tar` & `csv-wizard-0.4.2.post1.tar`

### file list

```diff
@@ -1,28 +1,22 @@
--rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-0.4.2/LICENSE
--rw-r--r--   0        0        0      528 2023-04-26 13:36:44.013526 csv-wizard-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     9063 2023-04-26 12:18:53.685144 csv-wizard-0.4.2/README.md
--rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-0.4.2/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-0.4.2/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-0.4.2/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-0.4.2/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-0.4.2/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-0.4.2/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0      602 2023-03-12 19:20:33.474055 csv-wizard-0.4.2/tests/blank_rows.csv
--rw-r--r--   0        0        0        0 2023-02-25 01:56:18.464794 csv-wizard-0.4.2/tests/empty.csv
--rw-r--r--   0        0        0    10763 2023-03-06 13:13:06.791537 csv-wizard-0.4.2/tests/everyone 246.csv
--rw-r--r--   0        0        0    10841 2023-03-06 13:01:51.287843 csv-wizard-0.4.2/tests/everyone 248.csv
--rw-r--r--   0        0        0      605 2023-02-25 02:31:25.668851 csv-wizard-0.4.2/tests/has_dups.csv
--rw-r--r--   0        0        0      221 2023-03-12 19:20:35.022067 csv-wizard-0.4.2/tests/small0.csv
--rw-r--r--   0        0        0      265 2023-03-12 19:08:47.060612 csv-wizard-0.4.2/tests/small1.csv
--rw-r--r--   0        0        0      689 2023-04-25 12:46:45.058770 csv-wizard-0.4.2/tests/test_divide.py
--rw-r--r--   0        0        0      261 2023-04-25 12:46:45.043745 csv-wizard-0.4.2/tests/test_encoding.py
--rw-r--r--   0        0        0      628 2023-04-25 12:48:02.485401 csv-wizard-0.4.2/tests/test_find_common_rows.py
--rw-r--r--   0        0        0      541 2023-04-25 12:46:45.073859 csv-wizard-0.4.2/tests/test_find_different_rows.py
--rw-r--r--   0        0        0      616 2023-04-25 12:48:02.522568 csv-wizard-0.4.2/tests/test_get_all_rows.py
--rw-r--r--   0        0        0      979 2023-04-25 12:48:02.541536 csv-wizard-0.4.2/tests/test_get_dialect.py
--rw-r--r--   0        0        0      846 2023-04-25 12:46:45.068689 csv-wizard-0.4.2/tests/test_get_duplicates.py
--rw-r--r--   0        0        0      431 2023-04-25 12:48:02.573957 csv-wizard-0.4.2/tests/test_get_headers.py
--rw-r--r--   0        0        0     1541 2023-04-25 12:48:02.592401 csv-wizard-0.4.2/tests/test_misc.py
--rw-r--r--   0        0        0      284 2023-04-25 12:48:02.609419 csv-wizard-0.4.2/tests/test_slice.py
--rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 csv-wizard-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-0.4.2.post1/LICENSE
+-rw-r--r--   0        0        0      493 2023-04-27 20:09:07.666783 csv-wizard-0.4.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     9074 2023-04-26 21:18:31.649684 csv-wizard-0.4.2.post1/README.md
+-rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-0.4.2.post1/src/csv_wizard/__init__.py
+-rw-r--r--   0        0        0    11621 2023-04-25 12:48:02.175388 csv-wizard-0.4.2.post1/src/csv_wizard/csv_wizard.py
+-rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-0.4.2.post1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-0.4.2.post1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-0.4.2.post1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-0.4.2.post1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-0.4.2.post1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-0.4.2.post1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      689 2023-04-25 12:46:45.058770 csv-wizard-0.4.2.post1/tests/test_divide.py
+-rw-r--r--   0        0        0      261 2023-04-25 12:46:45.043745 csv-wizard-0.4.2.post1/tests/test_encoding.py
+-rw-r--r--   0        0        0      628 2023-04-25 12:48:02.485401 csv-wizard-0.4.2.post1/tests/test_find_common_rows.py
+-rw-r--r--   0        0        0      541 2023-04-25 12:46:45.073859 csv-wizard-0.4.2.post1/tests/test_find_different_rows.py
+-rw-r--r--   0        0        0      616 2023-04-25 12:48:02.522568 csv-wizard-0.4.2.post1/tests/test_get_all_rows.py
+-rw-r--r--   0        0        0      979 2023-04-25 12:48:02.541536 csv-wizard-0.4.2.post1/tests/test_get_dialect.py
+-rw-r--r--   0        0        0      846 2023-04-25 12:46:45.068689 csv-wizard-0.4.2.post1/tests/test_get_duplicates.py
+-rw-r--r--   0        0        0      431 2023-04-25 12:48:02.573957 csv-wizard-0.4.2.post1/tests/test_get_headers.py
+-rw-r--r--   0        0        0     1541 2023-04-25 12:48:02.592401 csv-wizard-0.4.2.post1/tests/test_misc.py
+-rw-r--r--   0        0        0      284 2023-04-25 12:48:02.609419 csv-wizard-0.4.2.post1/tests/test_slice.py
+-rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 csv-wizard-0.4.2.post1/PKG-INFO
```

### Comparing `csv-wizard-0.4.2/LICENSE` & `csv-wizard-0.4.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/README.md` & `csv-wizard-0.4.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# CSV Divider
+# CSV Wizard
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 ***
-## Import a CSV file by only giving the `CSVParser` class a `string` containing the full name of the file without the *.csv* part.
+## Import a CSV file by only giving the `CSVParser` class a `string` containing the full name of the file without the *.csv* extension.
 > `new_file = CSVParser("my_file")`
 ***
 ## Handling decoding/encoding on a file.
 All methods have an optional `encoding` argument.
-If left empty, csv_parser will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
+If left empty, csv_wizard will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
 The encoding parameter accepts strings.
 ```
 > file1.get_row_count(encoding='utf-8') 
 ```
 ***
 ### Getting the characters that define the CSV file's layout. The `get_dialect` method.
 Calling this method on a CSVParser object returns it's dialect property.
@@ -25,15 +25,15 @@
 * skipinitialspace
 > `new_file.get_dialect().delimiter`
 
 > `new_file.get_dialect().lineterminator`
 
 > `new_file.get_dialect().quoting`
 ***
-### The `create()`. An easier way to create a file, optionally specify a path.
+### The `create()` method. An easier way to create a file, optionally specify a path.
 The create method receives a string as required argument and it creates a new CSV file using that string. 
 
 **Specifing a path to create the folder in**
 
 Optionally, this method receives a *path* argument to specify a folder to create the file in. If this is not specified, the file will be created in the current directory.
 
 For security reasons, when using this method in a client-facing app feature, it is recommended to limit the access to parent folders, to avoid the creation of files in vulnerable locations.
```

### Comparing `csv-wizard-0.4.2/tests/test_divide.py` & `csv-wizard-0.4.2.post1/tests/test_divide.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/tests/test_find_common_rows.py` & `csv-wizard-0.4.2.post1/tests/test_find_common_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/tests/test_find_different_rows.py` & `csv-wizard-0.4.2.post1/tests/test_find_different_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/tests/test_get_all_rows.py` & `csv-wizard-0.4.2.post1/tests/test_get_all_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/tests/test_get_dialect.py` & `csv-wizard-0.4.2.post1/tests/test_get_dialect.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/tests/test_get_duplicates.py` & `csv-wizard-0.4.2.post1/tests/test_get_duplicates.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/tests/test_misc.py` & `csv-wizard-0.4.2.post1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.2/PKG-INFO` & `csv-wizard-0.4.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: csv_wizard
-Version: 0.4.2
+Version: 0.4.2.post1
 Summary: Handy extension to Python csv standard library package
 License: MIT
 Author-email: liquidsnake <bentsoft365@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# CSV Divider
+# CSV Wizard
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 ***
-## Import a CSV file by only giving the `CSVParser` class a `string` containing the full name of the file without the *.csv* part.
+## Import a CSV file by only giving the `CSVParser` class a `string` containing the full name of the file without the *.csv* extension.
 > `new_file = CSVParser("my_file")`
 ***
 ## Handling decoding/encoding on a file.
 All methods have an optional `encoding` argument.
-If left empty, csv_parser will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
+If left empty, csv_wizard will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
 The encoding parameter accepts strings.
 ```
 > file1.get_row_count(encoding='utf-8') 
 ```
 ***
 ### Getting the characters that define the CSV file's layout. The `get_dialect` method.
 Calling this method on a CSVParser object returns it's dialect property.
@@ -34,15 +34,15 @@
 * skipinitialspace
 > `new_file.get_dialect().delimiter`
 
 > `new_file.get_dialect().lineterminator`
 
 > `new_file.get_dialect().quoting`
 ***
-### The `create()`. An easier way to create a file, optionally specify a path.
+### The `create()` method. An easier way to create a file, optionally specify a path.
 The create method receives a string as required argument and it creates a new CSV file using that string. 
 
 **Specifing a path to create the folder in**
 
 Optionally, this method receives a *path* argument to specify a folder to create the file in. If this is not specified, the file will be created in the current directory.
 
 For security reasons, when using this method in a client-facing app feature, it is recommended to limit the access to parent folders, to avoid the creation of files in vulnerable locations.
```

