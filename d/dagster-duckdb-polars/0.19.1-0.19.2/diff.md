# Comparing `tmp/dagster-duckdb-polars-0.19.1.tar.gz` & `tmp/dagster-duckdb-polars-0.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.19.1.tar", last modified: Thu Apr 20 21:16:43 2023, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.19.2.tar", last modified: Thu Apr 27 19:37:39 2023, max compression
```

## Comparing `dagster-duckdb-polars-0.19.1.tar` & `dagster-duckdb-polars-0.19.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:16:43.422555 dagster-duckdb-polars-0.19.1/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-20 21:16:43.422555 dagster-duckdb-polars-0.19.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:16:43.422555 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7372 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:16:43.422555 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-20 21:16:43.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-20 21:16:43.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:16:43.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:16:43.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-20 21:16:43.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-20 21:16:43.000000 dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-20 21:16:43.422555 dagster-duckdb-polars-0.19.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-20 21:07:09.000000 dagster-duckdb-polars-0.19.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:37:39.508975 dagster-duckdb-polars-0.19.2/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 19:37:39.508975 dagster-duckdb-polars-0.19.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:37:39.508975 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:37:39.508975 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 19:37:39.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-27 19:37:39.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:37:39.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:37:39.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-27 19:37:39.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 19:37:39.000000 dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 19:37:39.508975 dagster-duckdb-polars-0.19.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-27 18:30:35.000000 dagster-duckdb-polars-0.19.2/setup.py
```

### Comparing `dagster-duckdb-polars-0.19.1/LICENSE` & `dagster-duckdb-polars-0.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.19.1/PKG-INFO` & `dagster-duckdb-polars-0.19.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.19.1
+Version: 0.19.2
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.19.1/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.19.2/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.19.1/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.19.2/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.19.1
+Version: 0.19.2
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.19.1/setup.py` & `dagster-duckdb-polars-0.19.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.1",
-        "dagster-duckdb==0.19.1",
+        "dagster==1.3.2",
+        "dagster-duckdb==0.19.2",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

