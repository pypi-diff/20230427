# Comparing `tmp/sqlalchemy-spanner-1.5.0.tar.gz` & `tmp/sqlalchemy-spanner-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-spanner-1.5.0.tar", last modified: Wed Apr 19 07:47:15 2023, max compression
+gzip compressed data, was "sqlalchemy-spanner-1.6.0.tar", last modified: Thu Apr 27 11:41:31 2023, max compression
```

## Comparing `sqlalchemy-spanner-1.5.0.tar` & `sqlalchemy-spanner-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/LICENSE
--rw-r--r--   0 root         (0)     1003    17665 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    17292 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.117831 sqlalchemy-spanner-1.5.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.117831 sqlalchemy-spanner-1.5.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.117831 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/
--rw-rw-r--   0 root         (0)     1003      651 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1988 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003      792 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/provision.py
--rw-rw-r--   0 root         (0)     1003     3140 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/requirements.py
--rw-rw-r--   0 root         (0)     1003    49547 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
--rw-rw-r--   0 root         (0)     1003      261 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2431 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003    17665 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      742 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       87 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      155 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-19 07:47:15.000000 sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 07:47:15.121830 sqlalchemy-spanner-1.5.0/test/
--rw-rw-r--   0 root         (0)     1003    68740 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/test/test_suite_13.py
--rw-rw-r--   0 root         (0)     1003    81211 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/test/test_suite_14.py
--rw-rw-r--   0 root         (0)     1003   102613 2023-04-19 07:45:10.000000 sqlalchemy-spanner-1.5.0/test/test_suite_20.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/LICENSE
+-rw-r--r--   0 root         (0)     1003    17665 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    17292 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.238699 sqlalchemy-spanner-1.6.0/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.238699 sqlalchemy-spanner-1.6.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.238699 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/
+-rw-rw-r--   0 root         (0)     1003      651 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1988 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003      792 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/provision.py
+-rw-rw-r--   0 root         (0)     1003     3140 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/requirements.py
+-rw-rw-r--   0 root         (0)     1003    50036 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
+-rw-rw-r--   0 root         (0)     1003      261 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2431 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003    17665 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      742 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       87 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      155 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/test/
+-rw-rw-r--   0 root         (0)     1003    69178 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/test/test_suite_13.py
+-rw-rw-r--   0 root         (0)     1003    81649 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/test/test_suite_14.py
+-rw-rw-r--   0 root         (0)     1003   103981 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/test/test_suite_20.py
```

### Comparing `sqlalchemy-spanner-1.5.0/LICENSE` & `sqlalchemy-spanner-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/PKG-INFO` & `sqlalchemy-spanner-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.5.0
+Version: 1.6.0
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
```

### Comparing `sqlalchemy-spanner-1.5.0/README.rst` & `sqlalchemy-spanner-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/__init__.py` & `sqlalchemy-spanner-1.6.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/cloud/__init__.py` & `sqlalchemy-spanner-1.6.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/__init__.py` & `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py` & `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/provision.py` & `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/provision.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/requirements.py` & `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py` & `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,19 +641,22 @@
     def create_connect_args(self, url):
         """Parse connection args from the given URL.
 
         The method prepares args suitable to send to the DB API `connect()` function.
 
         The given URL follows the style:
         `spanner:///projects/{project-id}/instances/{instance-id}/databases/{database-id}`
+        or `spanner:///projects/{project-id}/instances/{instance-id}`. For the latter,
+        database operations will be not be possible and if required a new engine with
+        database-id set will need to be created.
         """
         match = re.match(
             (
                 r"^projects/(?P<project>.+?)/instances/"
-                "(?P<instance>.+?)/databases/(?P<database>.+?)$"
+                "(?P<instance>.+?)(/databases/(?P<database>.+)|$)"
             ),
             url.database,
         )
         dist = pkg_resources.get_distribution("sqlalchemy-spanner")
         return (
             [match.group("instance"), match.group("database"), match.group("project")],
             {"user_agent": f"gl-{dist.project_name}/{dist.version}"},
@@ -1342,25 +1345,37 @@
 
         if dbapi_connection._transaction and (
             dbapi_connection._transaction.rolled_back
             or dbapi_connection._transaction.committed
         ):
             pass
         else:
-            trace_attributes = {"db.instance": dbapi_connection.database.name}
+            trace_attributes = {
+                "db.instance": dbapi_connection.database.name
+                if dbapi_connection.database
+                else ""
+            }
             with trace_call("SpannerSqlAlchemy.Rollback", trace_attributes):
                 dbapi_connection.rollback()
 
     def do_commit(self, dbapi_connection):
-        trace_attributes = {"db.instance": dbapi_connection.database.name}
+        trace_attributes = {
+            "db.instance": dbapi_connection.database.name
+            if dbapi_connection.database
+            else ""
+        }
         with trace_call("SpannerSqlAlchemy.Commit", trace_attributes):
             dbapi_connection.commit()
 
     def do_close(self, dbapi_connection):
-        trace_attributes = {"db.instance": dbapi_connection.database.name}
+        trace_attributes = {
+            "db.instance": dbapi_connection.database.name
+            if dbapi_connection.database
+            else ""
+        }
         with trace_call("SpannerSqlAlchemy.Close", trace_attributes):
             dbapi_connection.close()
 
     def do_executemany(self, cursor, statement, parameters, context=None):
         trace_attributes = {
             "db.statement": statement,
             "db.params": parameters,
```

### Comparing `sqlalchemy-spanner-1.5.0/setup.py` & `sqlalchemy-spanner-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/PKG-INFO` & `sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.5.0
+Version: 1.6.0
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
```

### Comparing `sqlalchemy-spanner-1.5.0/sqlalchemy_spanner.egg-info/SOURCES.txt` & `sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.5.0/test/test_suite_13.py` & `sqlalchemy-spanner-1.6.0/test/test_suite_13.py`

 * *Files 1% similar despite different names*

```diff
@@ -2041,7 +2041,21 @@
         Object passed to enginer mismatch, error is thrown.
         """
         client = Client(project="project_id")
         engine = create_engine(get_db_url(), connect_args={"client": client})
 
         with pytest.raises(ValueError):
             engine.connect()
+
+
+class CreateEngineWithoutDatabaseTest(fixtures.TestBase):
+    def test_create_engine_wo_database(self):
+        """
+        SPANNER TEST:
+
+        Check that we can connect to SqlAlchemy
+        without passing database id in the
+        connection URL.
+        """
+        engine = create_engine(get_db_url().split("/database")[0])
+        with engine.connect() as connection:
+            assert connection.connection.database is None
```

### Comparing `sqlalchemy-spanner-1.5.0/test/test_suite_14.py` & `sqlalchemy-spanner-1.6.0/test/test_suite_14.py`

 * *Files 1% similar despite different names*

```diff
@@ -5069,8 +5069,36 @@
 00013cc0: 6e67 696e 6528 6765 745f 6462 5f75 726c  ngine(get_db_url
 00013cd0: 2829 2c20 636f 6e6e 6563 745f 6172 6773  (), connect_args
 00013ce0: 3d7b 2263 6c69 656e 7422 3a20 636c 6965  ={"client": clie
 00013cf0: 6e74 7d29 0a0a 2020 2020 2020 2020 7769  nt})..        wi
 00013d00: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
 00013d10: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
 00013d20: 2020 2020 2020 2020 2020 656e 6769 6e65            engine
-00013d30: 2e63 6f6e 6e65 6374 2829 0a              .connect().
+00013d30: 2e63 6f6e 6e65 6374 2829 0a0a 0a63 6c61  .connect()...cla
+00013d40: 7373 2043 7265 6174 6545 6e67 696e 6557  ss CreateEngineW
+00013d50: 6974 686f 7574 4461 7461 6261 7365 5465  ithoutDatabaseTe
+00013d60: 7374 2866 6978 7475 7265 732e 5465 7374  st(fixtures.Test
+00013d70: 4261 7365 293a 0a20 2020 2064 6566 2074  Base):.    def t
+00013d80: 6573 745f 6372 6561 7465 5f65 6e67 696e  est_create_engin
+00013d90: 655f 776f 5f64 6174 6162 6173 6528 7365  e_wo_database(se
+00013da0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00013db0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+00013dc0: 2054 4553 543a 0a0a 2020 2020 2020 2020   TEST:..        
+00013dd0: 4368 6563 6b20 7468 6174 2077 6520 6361  Check that we ca
+00013de0: 6e20 636f 6e6e 6563 7420 746f 2053 716c  n connect to Sql
+00013df0: 416c 6368 656d 790a 2020 2020 2020 2020  Alchemy.        
+00013e00: 7769 7468 6f75 7420 7061 7373 696e 6720  without passing 
+00013e10: 6461 7461 6261 7365 2069 6420 696e 2074  database id in t
+00013e20: 6865 0a20 2020 2020 2020 2063 6f6e 6e65  he.        conne
+00013e30: 6374 696f 6e20 5552 4c2e 0a20 2020 2020  ction URL..     
+00013e40: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+00013e50: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
+00013e60: 6e67 696e 6528 6765 745f 6462 5f75 726c  ngine(get_db_url
+00013e70: 2829 2e73 706c 6974 2822 2f64 6174 6162  ().split("/datab
+00013e80: 6173 6522 295b 305d 290a 2020 2020 2020  ase")[0]).      
+00013e90: 2020 7769 7468 2065 6e67 696e 652e 636f    with engine.co
+00013ea0: 6e6e 6563 7428 2920 6173 2063 6f6e 6e65  nnect() as conne
+00013eb0: 6374 696f 6e3a 0a20 2020 2020 2020 2020  ction:.         
+00013ec0: 2020 2061 7373 6572 7420 636f 6e6e 6563     assert connec
+00013ed0: 7469 6f6e 2e63 6f6e 6e65 6374 696f 6e2e  tion.connection.
+00013ee0: 6461 7461 6261 7365 2069 7320 4e6f 6e65  database is None
+00013ef0: 0a                                       .
```

### Comparing `sqlalchemy-spanner-1.5.0/test/test_suite_20.py` & `sqlalchemy-spanner-1.6.0/test/test_suite_20.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,6371 +44,6456 @@
 000002b0: 7572 6365 730a 696d 706f 7274 2070 7974  urces.import pyt
 000002c0: 6573 740a 696d 706f 7274 2072 616e 646f  est.import rando
 000002d0: 6d0a 696d 706f 7274 2074 696d 650a 6672  m.import time.fr
 000002e0: 6f6d 2075 6e69 7474 6573 7420 696d 706f  om unittest impo
 000002f0: 7274 206d 6f63 6b0a 0a66 726f 6d20 676f  rt mock..from go
 00000300: 6f67 6c65 2e63 6c6f 7564 2e73 7061 6e6e  ogle.cloud.spann
 00000310: 6572 5f76 3120 696d 706f 7274 2052 6571  er_v1 import Req
-00000320: 7565 7374 4f70 7469 6f6e 730a 696d 706f  uestOptions.impo
-00000330: 7274 2073 716c 616c 6368 656d 790a 6672  rt sqlalchemy.fr
-00000340: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
-00000350: 706f 7274 2063 7265 6174 655f 656e 6769  port create_engi
-00000360: 6e65 0a66 726f 6d20 7371 6c61 6c63 6865  ne.from sqlalche
-00000370: 6d79 2e65 6e67 696e 6520 696d 706f 7274  my.engine import
-00000380: 2049 6e73 7065 6374 6f72 0a66 726f 6d20   Inspector.from 
-00000390: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
-000003a0: 7420 696e 7370 6563 740a 6672 6f6d 2073  t inspect.from s
-000003b0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
-000003c0: 2074 6573 7469 6e67 0a66 726f 6d20 7371   testing.from sq
-000003d0: 6c61 6c63 6865 6d79 2069 6d70 6f72 7420  lalchemy import 
-000003e0: 466f 7265 6967 6e4b 6579 0a66 726f 6d20  ForeignKey.from 
-000003f0: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
-00000400: 7420 4d65 7461 4461 7461 0a66 726f 6d20  t MetaData.from 
-00000410: 7371 6c61 6c63 6865 6d79 2e65 6e67 696e  sqlalchemy.engin
-00000420: 6520 696d 706f 7274 204f 626a 6563 744b  e import ObjectK
-00000430: 696e 640a 6672 6f6d 2073 716c 616c 6368  ind.from sqlalch
-00000440: 656d 792e 656e 6769 6e65 2069 6d70 6f72  emy.engine impor
-00000450: 7420 4f62 6a65 6374 5363 6f70 650a 6672  t ObjectScope.fr
-00000460: 6f6d 2073 716c 616c 6368 656d 792e 7363  om sqlalchemy.sc
-00000470: 6865 6d61 2069 6d70 6f72 7420 4444 4c0a  hema import DDL.
-00000480: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
-00000490: 7363 6865 6d61 2069 6d70 6f72 7420 436f  schema import Co
-000004a0: 6d70 7574 6564 0a66 726f 6d20 7371 6c61  mputed.from sqla
-000004b0: 6c63 6865 6d79 2e74 6573 7469 6e67 2069  lchemy.testing i
-000004c0: 6d70 6f72 7420 636f 6e66 6967 0a66 726f  mport config.fro
-000004d0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-000004e0: 7469 6e67 2069 6d70 6f72 7420 656e 6769  ting import engi
-000004f0: 6e65 730a 6672 6f6d 2073 716c 616c 6368  nes.from sqlalch
-00000500: 656d 792e 7465 7374 696e 6720 696d 706f  emy.testing impo
-00000510: 7274 2065 715f 0a66 726f 6d20 7371 6c61  rt eq_.from sqla
-00000520: 6c63 6865 6d79 2e74 6573 7469 6e67 2069  lchemy.testing i
-00000530: 6d70 6f72 7420 7072 6f76 6964 655f 6d65  mport provide_me
-00000540: 7461 6461 7461 2c20 656d 6974 735f 7761  tadata, emits_wa
-00000550: 726e 696e 670a 6672 6f6d 2073 716c 616c  rning.from sqlal
-00000560: 6368 656d 792e 7465 7374 696e 6720 696d  chemy.testing im
-00000570: 706f 7274 2066 6978 7475 7265 730a 6672  port fixtures.fr
-00000580: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
-00000590: 7374 696e 672e 7072 6f76 6973 696f 6e20  sting.provision 
-000005a0: 696d 706f 7274 2074 656d 705f 7461 626c  import temp_tabl
-000005b0: 655f 6b65 7977 6f72 645f 6172 6773 0a66  e_keyword_args.f
-000005c0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-000005d0: 6573 7469 6e67 2e73 6368 656d 6120 696d  esting.schema im
-000005e0: 706f 7274 2043 6f6c 756d 6e0a 6672 6f6d  port Column.from
-000005f0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000600: 696e 672e 7363 6865 6d61 2069 6d70 6f72  ing.schema impor
-00000610: 7420 5461 626c 650a 6672 6f6d 2073 716c  t Table.from sql
-00000620: 616c 6368 656d 7920 696d 706f 7274 206c  alchemy import l
-00000630: 6974 6572 616c 5f63 6f6c 756d 6e0a 6672  iteral_column.fr
-00000640: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
-00000650: 706f 7274 2073 656c 6563 740a 6672 6f6d  port select.from
-00000660: 2073 716c 616c 6368 656d 7920 696d 706f   sqlalchemy impo
-00000670: 7274 2075 7469 6c0a 6672 6f6d 2073 716c  rt util.from sql
-00000680: 616c 6368 656d 7920 696d 706f 7274 2075  alchemy import u
-00000690: 6e69 6f6e 0a66 726f 6d20 7371 6c61 6c63  nion.from sqlalc
-000006a0: 6865 6d79 2069 6d70 6f72 7420 6576 656e  hemy import even
-000006b0: 740a 6672 6f6d 2073 716c 616c 6368 656d  t.from sqlalchem
-000006c0: 7920 696d 706f 7274 2065 7869 7374 730a  y import exists.
-000006d0: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
-000006e0: 696d 706f 7274 2042 6f6f 6c65 616e 0a66  import Boolean.f
-000006f0: 726f 6d20 7371 6c61 6c63 6865 6d79 2069  rom sqlalchemy i
-00000700: 6d70 6f72 7420 466c 6f61 740a 6672 6f6d  mport Float.from
-00000710: 2073 716c 616c 6368 656d 7920 696d 706f   sqlalchemy impo
-00000720: 7274 204c 6172 6765 4269 6e61 7279 0a66  rt LargeBinary.f
-00000730: 726f 6d20 7371 6c61 6c63 6865 6d79 2069  rom sqlalchemy i
-00000740: 6d70 6f72 7420 5374 7269 6e67 0a66 726f  mport String.fro
-00000750: 6d20 7371 6c61 6c63 6865 6d79 2e65 7874  m sqlalchemy.ext
-00000760: 2e64 6563 6c61 7261 7469 7665 2069 6d70  .declarative imp
-00000770: 6f72 7420 6465 636c 6172 6174 6976 655f  ort declarative_
-00000780: 6261 7365 0a66 726f 6d20 7371 6c61 6c63  base.from sqlalc
-00000790: 6865 6d79 2e6f 726d 2069 6d70 6f72 7420  hemy.orm import 
-000007a0: 7265 6c61 7469 6f6e 7368 6970 0a66 726f  relationship.fro
-000007b0: 6d20 7371 6c61 6c63 6865 6d79 2e6f 726d  m sqlalchemy.orm
-000007c0: 2069 6d70 6f72 7420 5365 7373 696f 6e0a   import Session.
-000007d0: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
-000007e0: 7479 7065 7320 696d 706f 7274 2049 6e74  types import Int
-000007f0: 6567 6572 0a66 726f 6d20 7371 6c61 6c63  eger.from sqlalc
-00000800: 6865 6d79 2e74 7970 6573 2069 6d70 6f72  hemy.types impor
-00000810: 7420 4e75 6d65 7269 630a 6672 6f6d 2073  t Numeric.from s
-00000820: 716c 616c 6368 656d 792e 7479 7065 7320  qlalchemy.types 
-00000830: 696d 706f 7274 2054 6578 740a 6672 6f6d  import Text.from
-00000840: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000850: 696e 6720 696d 706f 7274 2072 6571 7569  ing import requi
-00000860: 7265 730a 6672 6f6d 2073 716c 616c 6368  res.from sqlalch
-00000870: 656d 792e 7465 7374 696e 6720 696d 706f  emy.testing impo
-00000880: 7274 2069 735f 7472 7565 0a66 726f 6d20  rt is_true.from 
-00000890: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
-000008a0: 7420 496e 6465 780a 6672 6f6d 2073 716c  t Index.from sql
-000008b0: 616c 6368 656d 7920 696d 706f 7274 2074  alchemy import t
-000008c0: 7970 6573 0a66 726f 6d20 7371 6c61 6c63  ypes.from sqlalc
-000008d0: 6865 6d79 2e74 6573 7469 6e67 2e66 6978  hemy.testing.fix
-000008e0: 7475 7265 7320 696d 706f 7274 2028 0a20  tures import (. 
-000008f0: 2020 2043 6f6d 7075 7465 6452 6566 6c65     ComputedRefle
-00000900: 6374 696f 6e46 6978 7475 7265 5465 7374  ctionFixtureTest
-00000910: 2061 7320 5f43 6f6d 7075 7465 6452 6566   as _ComputedRef
-00000920: 6c65 6374 696f 6e46 6978 7475 7265 5465  lectionFixtureTe
-00000930: 7374 2c0a 290a 0a66 726f 6d20 676f 6f67  st,.)..from goog
-00000940: 6c65 2e61 7069 5f63 6f72 652e 6461 7465  le.api_core.date
-00000950: 7469 6d65 5f68 656c 7065 7273 2069 6d70  time_helpers imp
-00000960: 6f72 7420 4461 7465 7469 6d65 5769 7468  ort DatetimeWith
-00000970: 4e61 6e6f 7365 636f 6e64 730a 0a66 726f  Nanoseconds..fro
-00000980: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2069  m google.cloud i
-00000990: 6d70 6f72 7420 7370 616e 6e65 725f 6462  mport spanner_db
-000009a0: 6170 690a 0a66 726f 6d20 7371 6c61 6c63  api..from sqlalc
-000009b0: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-000009c0: 7465 2e74 6573 745f 6374 6520 696d 706f  te.test_cte impo
-000009d0: 7274 202a 2020 2320 6e6f 7161 3a20 4634  rt *  # noqa: F4
-000009e0: 3031 2c20 4634 3033 0a66 726f 6d20 7371  01, F403.from sq
-000009f0: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
-00000a00: 2e73 7569 7465 2e74 6573 745f 6464 6c20  .suite.test_ddl 
-00000a10: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
-00000a20: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
-00000a30: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000a40: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
-00000a50: 6469 616c 6563 7420 696d 706f 7274 202a  dialect import *
-00000a60: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
-00000a70: 4634 3033 0a66 726f 6d20 7371 6c61 6c63  F403.from sqlalc
-00000a80: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-00000a90: 7465 2e74 6573 745f 696e 7365 7274 2069  te.test_insert i
-00000aa0: 6d70 6f72 7420 2a20 2023 206e 6f71 613a  mport *  # noqa:
-00000ab0: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
-00000ac0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000ad0: 696e 672e 7375 6974 652e 7465 7374 5f72  ing.suite.test_r
-00000ae0: 6566 6c65 6374 696f 6e20 696d 706f 7274  eflection import
-00000af0: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
-00000b00: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
-00000b10: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00000b20: 7569 7465 2e74 6573 745f 6465 7072 6563  uite.test_deprec
-00000b30: 6174 696f 6e73 2069 6d70 6f72 7420 2a20  ations import * 
-00000b40: 2023 206e 6f71 613a 2046 3430 312c 2046   # noqa: F401, F
-00000b50: 3430 330a 6672 6f6d 2073 716c 616c 6368  403.from sqlalch
-00000b60: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
-00000b70: 652e 7465 7374 5f72 6573 756c 7473 2069  e.test_results i
-00000b80: 6d70 6f72 7420 2a20 2023 206e 6f71 613a  mport *  # noqa:
-00000b90: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
-00000ba0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000bb0: 696e 672e 7375 6974 652e 7465 7374 5f73  ing.suite.test_s
-00000bc0: 656c 6563 7420 696d 706f 7274 202a 2020  elect import *  
-00000bd0: 2320 6e6f 7161 3a20 4634 3031 2c20 4634  # noqa: F401, F4
-00000be0: 3033 0a66 726f 6d20 7371 6c61 6c63 6865  03.from sqlalche
-00000bf0: 6d79 2e74 6573 7469 6e67 2e73 7569 7465  my.testing.suite
-00000c00: 2e74 6573 745f 7365 7175 656e 6365 2069  .test_sequence i
-00000c10: 6d70 6f72 7420 2a20 2023 206e 6f71 613a  mport *  # noqa:
-00000c20: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
-00000c30: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000c40: 696e 672e 7375 6974 652e 7465 7374 5f75  ing.suite.test_u
-00000c50: 6e69 636f 6465 5f64 646c 2069 6d70 6f72  nicode_ddl impor
-00000c60: 7420 2a20 2023 206e 6f71 613a 2046 3430  t *  # noqa: F40
-00000c70: 312c 2046 3430 330a 6672 6f6d 2073 716c  1, F403.from sql
-00000c80: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
-00000c90: 7375 6974 652e 7465 7374 5f75 7064 6174  suite.test_updat
-00000ca0: 655f 6465 6c65 7465 2069 6d70 6f72 7420  e_delete import 
-00000cb0: 2a20 2023 206e 6f71 613a 2046 3430 312c  *  # noqa: F401,
-00000cc0: 2046 3430 330a 6672 6f6d 2073 716c 616c   F403.from sqlal
-00000cd0: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
-00000ce0: 6974 652e 7465 7374 5f63 7465 2069 6d70  ite.test_cte imp
-00000cf0: 6f72 7420 4354 4554 6573 7420 6173 205f  ort CTETest as _
-00000d00: 4354 4554 6573 740a 6672 6f6d 2073 716c  CTETest.from sql
-00000d10: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
-00000d20: 7375 6974 652e 7465 7374 5f64 646c 2069  suite.test_ddl i
-00000d30: 6d70 6f72 7420 5461 626c 6544 444c 5465  mport TableDDLTe
-00000d40: 7374 2061 7320 5f54 6162 6c65 4444 4c54  st as _TableDDLT
-00000d50: 6573 740a 6672 6f6d 2073 716c 616c 6368  est.from sqlalch
-00000d60: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
-00000d70: 652e 7465 7374 5f64 646c 2069 6d70 6f72  e.test_ddl impor
-00000d80: 7420 280a 2020 2020 4675 7475 7265 5461  t (.    FutureTa
-00000d90: 626c 6544 444c 5465 7374 2061 7320 5f46  bleDDLTest as _F
-00000da0: 7574 7572 6554 6162 6c65 4444 4c54 6573  utureTableDDLTes
-00000db0: 742c 0a20 2020 204c 6f6e 674e 616d 6542  t,.    LongNameB
-00000dc0: 6c6f 776f 7574 5465 7374 2061 7320 5f4c  lowoutTest as _L
-00000dd0: 6f6e 674e 616d 6542 6c6f 776f 7574 5465  ongNameBlowoutTe
-00000de0: 7374 2c0a 290a 6672 6f6d 2073 716c 616c  st,.).from sqlal
-00000df0: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
-00000e00: 6974 652e 7465 7374 5f75 7064 6174 655f  ite.test_update_
-00000e10: 6465 6c65 7465 2069 6d70 6f72 7420 280a  delete import (.
-00000e20: 2020 2020 5369 6d70 6c65 5570 6461 7465      SimpleUpdate
-00000e30: 4465 6c65 7465 5465 7374 2061 7320 5f53  DeleteTest as _S
-00000e40: 696d 706c 6555 7064 6174 6544 656c 6574  impleUpdateDelet
-00000e50: 6554 6573 742c 0a29 0a66 726f 6d20 7371  eTest,.).from sq
-00000e60: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
-00000e70: 2e73 7569 7465 2e74 6573 745f 6469 616c  .suite.test_dial
-00000e80: 6563 7420 696d 706f 7274 2028 0a20 2020  ect import (.   
-00000e90: 2044 6966 6669 6375 6c74 5061 7261 6d65   DifficultParame
-00000ea0: 7465 7273 5465 7374 2061 7320 5f44 6966  tersTest as _Dif
-00000eb0: 6669 6375 6c74 5061 7261 6d65 7465 7273  ficultParameters
-00000ec0: 5465 7374 2c0a 2020 2020 4573 6361 7069  Test,.    Escapi
-00000ed0: 6e67 5465 7374 2061 7320 5f45 7363 6170  ngTest as _Escap
-00000ee0: 696e 6754 6573 742c 0a20 2020 2052 6574  ingTest,.    Ret
-00000ef0: 7572 6e69 6e67 4775 6172 6473 5465 7374  urningGuardsTest
-00000f00: 2061 7320 5f52 6574 7572 6e69 6e67 4775   as _ReturningGu
-00000f10: 6172 6473 5465 7374 2c0a 290a 6672 6f6d  ardsTest,.).from
-00000f20: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00000f30: 696e 672e 7375 6974 652e 7465 7374 5f69  ing.suite.test_i
-00000f40: 6e73 6572 7420 696d 706f 7274 2028 0a20  nsert import (. 
-00000f50: 2020 2049 6e73 6572 7442 6568 6176 696f     InsertBehavio
-00000f60: 7254 6573 7420 6173 205f 496e 7365 7274  rTest as _Insert
-00000f70: 4265 6861 7669 6f72 5465 7374 2c0a 290a  BehaviorTest,.).
-00000f80: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
-00000f90: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
-00000fa0: 7374 5f73 656c 6563 7420 696d 706f 7274  st_select import
-00000fb0: 2028 2020 2320 6e6f 7161 3a20 4634 3031   (  # noqa: F401
-00000fc0: 2c20 4634 3033 0a20 2020 2043 6f6d 706f  , F403.    Compo
-00000fd0: 756e 6453 656c 6563 7454 6573 7420 6173  undSelectTest as
-00000fe0: 205f 436f 6d70 6f75 6e64 5365 6c65 6374   _CompoundSelect
-00000ff0: 5465 7374 2c0a 2020 2020 4578 6973 7473  Test,.    Exists
-00001000: 5465 7374 2061 7320 5f45 7869 7374 7354  Test as _ExistsT
-00001010: 6573 742c 0a20 2020 2046 6574 6368 4c69  est,.    FetchLi
-00001020: 6d69 744f 6666 7365 7454 6573 7420 6173  mitOffsetTest as
-00001030: 205f 4665 7463 684c 696d 6974 4f66 6673   _FetchLimitOffs
-00001040: 6574 5465 7374 2c0a 2020 2020 4964 656e  etTest,.    Iden
-00001050: 7469 7479 4175 746f 696e 6372 656d 656e  tityAutoincremen
-00001060: 7454 6573 7420 6173 205f 4964 656e 7469  tTest as _Identi
-00001070: 7479 4175 746f 696e 6372 656d 656e 7454  tyAutoincrementT
-00001080: 6573 742c 0a20 2020 2049 734f 7249 734e  est,.    IsOrIsN
-00001090: 6f74 4469 7374 696e 6374 4672 6f6d 5465  otDistinctFromTe
-000010a0: 7374 2061 7320 5f49 734f 7249 734e 6f74  st as _IsOrIsNot
-000010b0: 4469 7374 696e 6374 4672 6f6d 5465 7374  DistinctFromTest
-000010c0: 2c0a 2020 2020 4c69 6b65 4675 6e63 7469  ,.    LikeFuncti
-000010d0: 6f6e 7354 6573 7420 6173 205f 4c69 6b65  onsTest as _Like
-000010e0: 4675 6e63 7469 6f6e 7354 6573 742c 0a20  FunctionsTest,. 
-000010f0: 2020 204f 7264 6572 4279 4c61 6265 6c54     OrderByLabelT
-00001100: 6573 7420 6173 205f 4f72 6465 7242 794c  est as _OrderByL
-00001110: 6162 656c 5465 7374 2c0a 2020 2020 506f  abelTest,.    Po
-00001120: 7374 436f 6d70 696c 6550 6172 616d 7354  stCompileParamsT
-00001130: 6573 7420 6173 205f 506f 7374 436f 6d70  est as _PostComp
-00001140: 696c 6550 6172 616d 7354 6573 742c 0a20  ileParamsTest,. 
-00001150: 2020 2053 616d 654e 616d 6564 5363 6865     SameNamedSche
-00001160: 6d61 5461 626c 6554 6573 7420 6173 205f  maTableTest as _
-00001170: 5361 6d65 4e61 6d65 6453 6368 656d 6154  SameNamedSchemaT
-00001180: 6162 6c65 5465 7374 2c0a 290a 6672 6f6d  ableTest,.).from
-00001190: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-000011a0: 696e 672e 7375 6974 652e 7465 7374 5f72  ing.suite.test_r
-000011b0: 6566 6c65 6374 696f 6e20 696d 706f 7274  eflection import
-000011c0: 2028 2020 2320 6e6f 7161 3a20 4634 3031   (  # noqa: F401
-000011d0: 2c20 4634 3033 0a20 2020 2043 6f6d 706f  , F403.    Compo
-000011e0: 6e65 6e74 5265 666c 6563 7469 6f6e 5465  nentReflectionTe
-000011f0: 7374 4578 7472 6120 6173 205f 436f 6d70  stExtra as _Comp
-00001200: 6f6e 656e 7452 6566 6c65 6374 696f 6e54  onentReflectionT
-00001210: 6573 7445 7874 7261 2c0a 2020 2020 5175  estExtra,.    Qu
-00001220: 6f74 6564 4e61 6d65 4172 6775 6d65 6e74  otedNameArgument
-00001230: 5465 7374 2061 7320 5f51 756f 7465 644e  Test as _QuotedN
-00001240: 616d 6541 7267 756d 656e 7454 6573 742c  ameArgumentTest,
-00001250: 0a20 2020 2043 6f6d 706f 6e65 6e74 5265  .    ComponentRe
-00001260: 666c 6563 7469 6f6e 5465 7374 2061 7320  flectionTest as 
-00001270: 5f43 6f6d 706f 6e65 6e74 5265 666c 6563  _ComponentReflec
-00001280: 7469 6f6e 5465 7374 2c0a 2020 2020 436f  tionTest,.    Co
-00001290: 6d70 6f73 6974 654b 6579 5265 666c 6563  mpositeKeyReflec
-000012a0: 7469 6f6e 5465 7374 2061 7320 5f43 6f6d  tionTest as _Com
-000012b0: 706f 7369 7465 4b65 7952 6566 6c65 6374  positeKeyReflect
-000012c0: 696f 6e54 6573 742c 0a20 2020 2043 6f6d  ionTest,.    Com
-000012d0: 7075 7465 6452 6566 6c65 6374 696f 6e54  putedReflectionT
-000012e0: 6573 7420 6173 205f 436f 6d70 7574 6564  est as _Computed
-000012f0: 5265 666c 6563 7469 6f6e 5465 7374 2c0a  ReflectionTest,.
-00001300: 2020 2020 4861 7349 6e64 6578 5465 7374      HasIndexTest
-00001310: 2061 7320 5f48 6173 496e 6465 7854 6573   as _HasIndexTes
-00001320: 742c 0a20 2020 2048 6173 5461 626c 6554  t,.    HasTableT
-00001330: 6573 7420 6173 205f 4861 7354 6162 6c65  est as _HasTable
-00001340: 5465 7374 2c0a 290a 6672 6f6d 2073 716c  Test,.).from sql
-00001350: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
-00001360: 7375 6974 652e 7465 7374 5f72 6573 756c  suite.test_resul
-00001370: 7473 2069 6d70 6f72 7420 280a 2020 2020  ts import (.    
-00001380: 526f 7746 6574 6368 5465 7374 2061 7320  RowFetchTest as 
-00001390: 5f52 6f77 4665 7463 6854 6573 742c 0a29  _RowFetchTest,.)
-000013a0: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
-000013b0: 2e74 6573 7469 6e67 2e73 7569 7465 2e74  .testing.suite.t
-000013c0: 6573 745f 7479 7065 7320 696d 706f 7274  est_types import
-000013d0: 2028 2020 2320 6e6f 7161 3a20 4634 3031   (  # noqa: F401
-000013e0: 2c20 4634 3033 0a20 2020 2042 6f6f 6c65  , F403.    Boole
-000013f0: 616e 5465 7374 2061 7320 5f42 6f6f 6c65  anTest as _Boole
-00001400: 616e 5465 7374 2c0a 2020 2020 4461 7465  anTest,.    Date
-00001410: 5465 7374 2061 7320 5f44 6174 6554 6573  Test as _DateTes
-00001420: 742c 0a20 2020 205f 4461 7465 4669 7874  t,.    _DateFixt
-00001430: 7572 6520 6173 205f 5f44 6174 6546 6978  ure as __DateFix
-00001440: 7475 7265 2c0a 2020 2020 4461 7465 5469  ture,.    DateTi
-00001450: 6d65 4869 7374 6f72 6963 5465 7374 2c0a  meHistoricTest,.
-00001460: 2020 2020 4461 7465 5469 6d65 436f 6572      DateTimeCoer
-00001470: 6365 6454 6f44 6174 6554 696d 6554 6573  cedToDateTimeTes
-00001480: 7420 6173 205f 4461 7465 5469 6d65 436f  t as _DateTimeCo
-00001490: 6572 6365 6454 6f44 6174 6554 696d 6554  ercedToDateTimeT
-000014a0: 6573 742c 0a20 2020 2044 6174 6554 696d  est,.    DateTim
-000014b0: 654d 6963 726f 7365 636f 6e64 7354 6573  eMicrosecondsTes
-000014c0: 7420 6173 205f 4461 7465 5469 6d65 4d69  t as _DateTimeMi
-000014d0: 6372 6f73 6563 6f6e 6473 5465 7374 2c0a  crosecondsTest,.
-000014e0: 2020 2020 4461 7465 5469 6d65 5465 7374      DateTimeTest
-000014f0: 2061 7320 5f44 6174 6554 696d 6554 6573   as _DateTimeTes
-00001500: 742c 0a20 2020 2049 6e74 6567 6572 5465  t,.    IntegerTe
-00001510: 7374 2061 7320 5f49 6e74 6567 6572 5465  st as _IntegerTe
-00001520: 7374 2c0a 2020 2020 4a53 4f4e 5465 7374  st,.    JSONTest
-00001530: 2061 7320 5f4a 534f 4e54 6573 742c 0a20   as _JSONTest,. 
-00001540: 2020 205f 4c69 7465 7261 6c52 6f75 6e64     _LiteralRound
-00001550: 5472 6970 4669 7874 7572 652c 0a20 2020  TripFixture,.   
-00001560: 204e 756d 6572 6963 5465 7374 2061 7320   NumericTest as 
-00001570: 5f4e 756d 6572 6963 5465 7374 2c0a 2020  _NumericTest,.  
-00001580: 2020 5374 7269 6e67 5465 7374 2061 7320    StringTest as 
-00001590: 5f53 7472 696e 6754 6573 742c 0a20 2020  _StringTest,.   
-000015a0: 2054 6578 7454 6573 7420 6173 205f 5465   TextTest as _Te
-000015b0: 7874 5465 7374 2c0a 2020 2020 5469 6d65  xtTest,.    Time
-000015c0: 5465 7374 2061 7320 5f54 696d 6554 6573  Test as _TimeTes
-000015d0: 742c 0a20 2020 2054 696d 654d 6963 726f  t,.    TimeMicro
-000015e0: 7365 636f 6e64 7354 6573 7420 6173 205f  secondsTest as _
-000015f0: 5469 6d65 4d69 6372 6f73 6563 6f6e 6473  TimeMicroseconds
-00001600: 5465 7374 2c0a 2020 2020 5469 6d65 7374  Test,.    Timest
-00001610: 616d 704d 6963 726f 7365 636f 6e64 7354  ampMicrosecondsT
-00001620: 6573 742c 0a20 2020 2055 6e69 636f 6465  est,.    Unicode
-00001630: 5661 7263 6861 7254 6573 7420 6173 205f  VarcharTest as _
-00001640: 556e 6963 6f64 6556 6172 6368 6172 5465  UnicodeVarcharTe
-00001650: 7374 2c0a 2020 2020 556e 6963 6f64 6554  st,.    UnicodeT
-00001660: 6578 7454 6573 7420 6173 205f 556e 6963  extTest as _Unic
-00001670: 6f64 6554 6578 7454 6573 742c 0a20 2020  odeTextTest,.   
-00001680: 205f 556e 6963 6f64 6546 6978 7475 7265   _UnicodeFixture
-00001690: 2061 7320 5f5f 556e 6963 6f64 6546 6978   as __UnicodeFix
-000016a0: 7475 7265 2c0a 2920 2023 206e 6f71 613a  ture,.)  # noqa:
-000016b0: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
-000016c0: 2074 6573 742e 5f68 656c 7065 7273 2069   test._helpers i
-000016d0: 6d70 6f72 7420 6765 745f 6462 5f75 726c  mport get_db_url
-000016e0: 0a0a 636f 6e66 6967 2e74 6573 745f 7363  ..config.test_sc
-000016f0: 6865 6d61 203d 2022 220a 0a0a 636c 6173  hema = ""...clas
-00001700: 7320 426f 6f6c 6561 6e54 6573 7428 5f42  s BooleanTest(_B
-00001710: 6f6f 6c65 616e 5465 7374 293a 0a20 2020  ooleanTest):.   
-00001720: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
-00001730: 6970 280a 2020 2020 2020 2020 2254 6865  ip(.        "The
-00001740: 206f 7269 6769 6e61 6c20 7465 7374 2063   original test c
-00001750: 6173 6520 7761 7320 7370 6c69 7420 696e  ase was split in
-00001760: 746f 2032 2070 6172 7473 3a20 220a 2020  to 2 parts: ".  
-00001770: 2020 2020 2020 2274 6573 745f 7265 6e64        "test_rend
-00001780: 6572 5f6c 6974 6572 616c 5f62 6f6f 6c5f  er_literal_bool_
-00001790: 7472 7565 2061 6e64 2074 6573 745f 7265  true and test_re
-000017a0: 6e64 6572 5f6c 6974 6572 616c 5f62 6f6f  nder_literal_boo
-000017b0: 6c5f 6661 6c73 6522 0a20 2020 2029 0a20  l_false".    ). 
-000017c0: 2020 2064 6566 2074 6573 745f 7265 6e64     def test_rend
-000017d0: 6572 5f6c 6974 6572 616c 5f62 6f6f 6c28  er_literal_bool(
-000017e0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000017f0: 6173 730a 0a20 2020 2064 6566 2074 6573  ass..    def tes
-00001800: 745f 7265 6e64 6572 5f6c 6974 6572 616c  t_render_literal
-00001810: 5f62 6f6f 6c5f 7472 7565 2873 656c 662c  _bool_true(self,
-00001820: 206c 6974 6572 616c 5f72 6f75 6e64 5f74   literal_round_t
-00001830: 7269 7029 3a0a 2020 2020 2020 2020 2222  rip):.        ""
-00001840: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
-00001850: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
-00001860: 2020 2020 2043 6c6f 7564 2053 7061 6e6e       Cloud Spann
-00001870: 6572 2073 7570 706f 7274 7320 7461 626c  er supports tabl
-00001880: 6573 2077 6974 6820 616e 2065 6d70 7479  es with an empty
-00001890: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
-000018a0: 740a 2020 2020 2020 2020 6f6e 6c79 2061  t.        only a
-000018b0: 2073 696e 676c 6520 726f 7720 6361 6e20   single row can 
-000018c0: 6265 2069 6e73 6572 7465 6420 696e 746f  be inserted into
-000018d0: 2073 7563 6820 6120 7461 626c 6520 2d0a   such a table -.
-000018e0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
-000018f0: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
-00001900: 6c20 6661 696c 2077 6974 6820 6052 6f77  l fail with `Row
-00001910: 205b 5d20 616c 7265 6164 7920 6578 6973   [] already exis
-00001920: 7473 222e 0a20 2020 2020 2020 204f 7665  ts"..        Ove
-00001930: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
-00001940: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
-00001950: 6d65 2066 6169 6c75 7265 2e0a 2020 2020  me failure..    
-00001960: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00001970: 6c69 7465 7261 6c5f 726f 756e 645f 7472  literal_round_tr
-00001980: 6970 2842 6f6f 6c65 616e 2829 2c20 5b54  ip(Boolean(), [T
-00001990: 7275 655d 2c20 5b54 7275 655d 290a 0a20  rue], [True]).. 
-000019a0: 2020 2064 6566 2074 6573 745f 7265 6e64     def test_rend
-000019b0: 6572 5f6c 6974 6572 616c 5f62 6f6f 6c5f  er_literal_bool_
-000019c0: 6661 6c73 6528 7365 6c66 2c20 6c69 7465  false(self, lite
-000019d0: 7261 6c5f 726f 756e 645f 7472 6970 293a  ral_round_trip):
-000019e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000019f0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-00001a00: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
-00001a10: 436c 6f75 6420 5370 616e 6e65 7220 7375  Cloud Spanner su
-00001a20: 7070 6f72 7473 2074 6162 6c65 7320 7769  pports tables wi
-00001a30: 7468 2061 6e20 656d 7074 7920 7072 696d  th an empty prim
-00001a40: 6172 7920 6b65 792c 2062 7574 0a20 2020  ary key, but.   
-00001a50: 2020 2020 206f 6e6c 7920 6120 7369 6e67       only a sing
-00001a60: 6c65 2072 6f77 2063 616e 2062 6520 696e  le row can be in
-00001a70: 7365 7274 6564 2069 6e74 6f20 7375 6368  serted into such
-00001a80: 2061 2074 6162 6c65 202d 0a20 2020 2020   a table -.     
-00001a90: 2020 2066 6f6c 6c6f 7769 6e67 2069 6e73     following ins
-00001aa0: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
-00001ab0: 6c20 7769 7468 2060 526f 7720 5b5d 2061  l with `Row [] a
-00001ac0: 6c72 6561 6479 2065 7869 7374 7322 2e0a  lready exists"..
-00001ad0: 2020 2020 2020 2020 4f76 6572 7269 6469          Overridi
-00001ae0: 6e67 2074 6865 2074 6573 7420 746f 2061  ng the test to a
-00001af0: 766f 6964 2074 6865 2073 616d 6520 6661  void the same fa
-00001b00: 696c 7572 652e 0a20 2020 2020 2020 2022  ilure..        "
-00001b10: 2222 0a20 2020 2020 2020 206c 6974 6572  "".        liter
-00001b20: 616c 5f72 6f75 6e64 5f74 7269 7028 426f  al_round_trip(Bo
-00001b30: 6f6c 6561 6e28 292c 205b 4661 6c73 655d  olean(), [False]
-00001b40: 2c20 5b46 616c 7365 5d29 0a0a 2020 2020  , [False])..    
-00001b50: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00001b60: 7028 224e 6f74 2073 7570 706f 7274 6564  p("Not supported
-00001b70: 2062 7920 436c 6f75 6420 5370 616e 6e65   by Cloud Spanne
-00001b80: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
-00001b90: 5f77 6865 7265 636c 6175 7365 2873 656c  _whereclause(sel
-00001ba0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00001bb0: 0a0a 0a63 6c61 7373 2043 6f6d 706f 6e65  ...class Compone
-00001bc0: 6e74 5265 666c 6563 7469 6f6e 5465 7374  ntReflectionTest
-00001bd0: 4578 7472 6128 5f43 6f6d 706f 6e65 6e74  Extra(_Component
-00001be0: 5265 666c 6563 7469 6f6e 5465 7374 4578  ReflectionTestEx
-00001bf0: 7472 6129 3a0a 2020 2020 4074 6573 7469  tra):.    @testi
-00001c00: 6e67 2e72 6571 7569 7265 732e 7461 626c  ng.requires.tabl
-00001c10: 655f 7265 666c 6563 7469 6f6e 0a20 2020  e_reflection.   
-00001c20: 2064 6566 2074 6573 745f 6e75 6c6c 6162   def test_nullab
-00001c30: 6c65 5f72 6566 6c65 6374 696f 6e28 7365  le_reflection(se
-00001c40: 6c66 2c20 636f 6e6e 6563 7469 6f6e 2c20  lf, connection, 
-00001c50: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
-00001c60: 2020 2074 203d 2054 6162 6c65 280a 2020     t = Table(.  
-00001c70: 2020 2020 2020 2020 2020 2274 222c 0a20            "t",. 
-00001c80: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00001c90: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00001ca0: 2043 6f6c 756d 6e28 2261 222c 2049 6e74   Column("a", Int
-00001cb0: 6567 6572 2c20 6e75 6c6c 6162 6c65 3d54  eger, nullable=T
-00001cc0: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-00001cd0: 2020 436f 6c75 6d6e 2822 6222 2c20 496e    Column("b", In
-00001ce0: 7465 6765 722c 206e 756c 6c61 626c 653d  teger, nullable=
-00001cf0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-00001d00: 290a 2020 2020 2020 2020 742e 6372 6561  ).        t.crea
-00001d10: 7465 2863 6f6e 6e65 6374 696f 6e29 0a20  te(connection). 
-00001d20: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-00001d30: 6e2e 636f 6e6e 6563 7469 6f6e 2e63 6f6d  n.connection.com
-00001d40: 6d69 7428 290a 2020 2020 2020 2020 6571  mit().        eq
-00001d50: 5f28 0a20 2020 2020 2020 2020 2020 2064  _(.            d
-00001d60: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
-00001d70: 2020 2020 2028 636f 6c5b 226e 616d 6522       (col["name"
-00001d80: 5d2c 2063 6f6c 5b22 6e75 6c6c 6162 6c65  ], col["nullable
-00001d90: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-00001da0: 2020 2020 666f 7220 636f 6c20 696e 2069      for col in i
-00001db0: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
-00001dc0: 6e29 2e67 6574 5f63 6f6c 756d 6e73 2822  n).get_columns("
-00001dd0: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-00001de0: 292c 0a20 2020 2020 2020 2020 2020 207b  ),.            {
-00001df0: 2261 223a 2054 7275 652c 2022 6222 3a20  "a": True, "b": 
-00001e00: 4661 6c73 657d 2c0a 2020 2020 2020 2020  False},.        
-00001e10: 290a 0a20 2020 2064 6566 205f 7479 7065  )..    def _type
-00001e20: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
-00001e30: 2c20 636f 6e6e 6563 7469 6f6e 2c20 6d65  , connection, me
-00001e40: 7461 6461 7461 2c20 2a74 7970 6573 293a  tadata, *types):
-00001e50: 0a20 2020 2020 2020 2074 203d 2054 6162  .        t = Tab
-00001e60: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00001e70: 2274 222c 206d 6574 6164 6174 612c 202a  "t", metadata, *
-00001e80: 5b43 6f6c 756d 6e28 2274 2564 2220 2520  [Column("t%d" % 
-00001e90: 692c 2074 7970 655f 2920 666f 7220 692c  i, type_) for i,
-00001ea0: 2074 7970 655f 2069 6e20 656e 756d 6572   type_ in enumer
-00001eb0: 6174 6528 7479 7065 7329 5d0a 2020 2020  ate(types)].    
-00001ec0: 2020 2020 290a 2020 2020 2020 2020 742e      ).        t.
-00001ed0: 6372 6561 7465 2863 6f6e 6e65 6374 696f  create(connectio
-00001ee0: 6e29 0a20 2020 2020 2020 2063 6f6e 6e65  n).        conne
-00001ef0: 6374 696f 6e2e 636f 6e6e 6563 7469 6f6e  ction.connection
-00001f00: 2e63 6f6d 6d69 7428 290a 0a20 2020 2020  .commit()..     
-00001f10: 2020 2072 6574 7572 6e20 5b63 5b22 7479     return [c["ty
-00001f20: 7065 225d 2066 6f72 2063 2069 6e20 696e  pe"] for c in in
-00001f30: 7370 6563 7428 636f 6e6e 6563 7469 6f6e  spect(connection
-00001f40: 292e 6765 745f 636f 6c75 6d6e 7328 2274  ).get_columns("t
-00001f50: 2229 5d0a 0a20 2020 2040 7465 7374 696e  ")]..    @testin
-00001f60: 672e 7265 7175 6972 6573 2e74 6162 6c65  g.requires.table
-00001f70: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
-00001f80: 6465 6620 7465 7374 5f6e 756d 6572 6963  def test_numeric
-00001f90: 5f72 6566 6c65 6374 696f 6e28 7365 6c66  _reflection(self
-00001fa0: 2c20 636f 6e6e 6563 7469 6f6e 2c20 6d65  , connection, me
-00001fb0: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
-00001fc0: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-00001fd0: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-00001fe0: 2020 2020 2020 2020 5370 616e 6e65 7220          Spanner 
-00001ff0: 6465 6669 6e65 7320 4e55 4d45 5249 4320  defines NUMERIC 
-00002000: 7479 7065 2077 6974 6820 7468 6520 636f  type with the co
-00002010: 6e73 7461 6e74 2070 7265 6369 7369 6f6e  nstant precision
-00002020: 3d33 380a 2020 2020 2020 2020 616e 6420  =38.        and 
-00002030: 7363 616c 653d 392e 204f 7665 7272 6964  scale=9. Overrid
-00002040: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
-00002050: 6368 6563 6b20 6966 2074 6865 204e 554d  check if the NUM
-00002060: 4552 4943 0a20 2020 2020 2020 2063 6f6c  ERIC.        col
-00002070: 756d 6e20 6973 2073 7563 6365 7373 6675  umn is successfu
-00002080: 6c6c 7920 6372 6561 7465 6420 616e 6420  lly created and 
-00002090: 6861 7320 6469 6d65 6e73 696f 6e73 0a20  has dimensions. 
-000020a0: 2020 2020 2020 2063 6f72 7265 6374 2066         correct f
-000020b0: 6f72 2043 6c6f 7564 2053 7061 6e6e 6572  or Cloud Spanner
-000020c0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000020d0: 2020 2020 2020 666f 7220 7479 7020 696e        for typ in
-000020e0: 2073 656c 662e 5f74 7970 655f 726f 756e   self._type_roun
-000020f0: 645f 7472 6970 2863 6f6e 6e65 6374 696f  d_trip(connectio
-00002100: 6e2c 206d 6574 6164 6174 612c 204e 756d  n, metadata, Num
-00002110: 6572 6963 2831 382c 2035 2929 3a0a 2020  eric(18, 5)):.  
-00002120: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00002130: 2069 7369 6e73 7461 6e63 6528 7479 702c   isinstance(typ,
-00002140: 204e 756d 6572 6963 290a 2020 2020 2020   Numeric).      
-00002150: 2020 2020 2020 6571 5f28 7479 702e 7072        eq_(typ.pr
-00002160: 6563 6973 696f 6e2c 2033 3829 0a20 2020  ecision, 38).   
-00002170: 2020 2020 2020 2020 2065 715f 2874 7970           eq_(typ
-00002180: 2e73 6361 6c65 2c20 3929 0a0a 2020 2020  .scale, 9)..    
-00002190: 4074 6573 7469 6e67 2e72 6571 7569 7265  @testing.require
-000021a0: 732e 7461 626c 655f 7265 666c 6563 7469  s.table_reflecti
-000021b0: 6f6e 0a20 2020 2064 6566 2074 6573 745f  on.    def test_
-000021c0: 6269 6e61 7279 5f72 6566 6c65 6374 696f  binary_reflectio
-000021d0: 6e28 7365 6c66 2c20 636f 6e6e 6563 7469  n(self, connecti
-000021e0: 6f6e 2c20 6d65 7461 6461 7461 293a 0a20  on, metadata):. 
-000021f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002200: 2020 2043 6865 636b 2074 6861 7420 6120     Check that a 
-00002210: 4259 5445 5320 636f 6c75 6d6e 2077 6974  BYTES column wit
-00002220: 6820 616e 2065 7870 6c69 6369 746c 790a  h an explicitly.
-00002230: 2020 2020 2020 2020 7365 7420 7369 7a65          set size
-00002240: 2069 7320 636f 7272 6563 746c 7920 7265   is correctly re
-00002250: 666c 6563 7465 642e 0a20 2020 2020 2020  flected..       
-00002260: 2022 2222 0a20 2020 2020 2020 2066 6f72   """.        for
-00002270: 2074 7970 2069 6e20 7365 6c66 2e5f 7479   typ in self._ty
-00002280: 7065 5f72 6f75 6e64 5f74 7269 7028 636f  pe_round_trip(co
-00002290: 6e6e 6563 7469 6f6e 2c20 6d65 7461 6461  nnection, metada
-000022a0: 7461 2c20 4c61 7267 6542 696e 6172 7928  ta, LargeBinary(
-000022b0: 3230 2929 3a0a 2020 2020 2020 2020 2020  20)):.          
-000022c0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-000022d0: 6e63 6528 7479 702c 204c 6172 6765 4269  nce(typ, LargeBi
-000022e0: 6e61 7279 290a 2020 2020 2020 2020 2020  nary).          
-000022f0: 2020 6571 5f28 7479 702e 6c65 6e67 7468    eq_(typ.length
-00002300: 2c20 3230 290a 0a0a 636c 6173 7320 436f  , 20)...class Co
-00002310: 6d70 7574 6564 5265 666c 6563 7469 6f6e  mputedReflection
-00002320: 4669 7874 7572 6554 6573 7428 5f43 6f6d  FixtureTest(_Com
-00002330: 7075 7465 6452 6566 6c65 6374 696f 6e46  putedReflectionF
-00002340: 6978 7475 7265 5465 7374 293a 0a20 2020  ixtureTest):.   
-00002350: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00002360: 2020 6465 6620 6465 6669 6e65 5f74 6162    def define_tab
-00002370: 6c65 7328 636c 732c 206d 6574 6164 6174  les(cls, metadat
-00002380: 6129 3a0a 2020 2020 2020 2020 2222 2253  a):.        """S
-00002390: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-000023a0: 0a0a 2020 2020 2020 2020 4176 6f69 6420  ..        Avoid 
-000023b0: 7573 696e 6720 6465 6661 756c 7420 7661  using default va
-000023c0: 6c75 6573 2066 6f72 2063 6f6d 7075 7465  lues for compute
-000023d0: 6420 636f 6c75 6d6e 732e 0a20 2020 2020  d columns..     
-000023e0: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-000023f0: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
-00002400: 2020 2263 6f6d 7075 7465 645f 6465 6661    "computed_defa
-00002410: 756c 745f 7461 626c 6522 2c0a 2020 2020  ult_table",.    
-00002420: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00002430: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-00002440: 6c75 6d6e 2822 6964 222c 2049 6e74 6567  lumn("id", Integ
-00002450: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
-00002460: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00002470: 2020 2043 6f6c 756d 6e28 226e 6f72 6d61     Column("norma
-00002480: 6c22 2c20 496e 7465 6765 7229 2c0a 2020  l", Integer),.  
-00002490: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-000024a0: 2822 636f 6d70 7574 6564 5f63 6f6c 222c  ("computed_col",
-000024b0: 2049 6e74 6567 6572 2c20 436f 6d70 7574   Integer, Comput
-000024c0: 6564 2822 6e6f 726d 616c 202b 2034 3222  ed("normal + 42"
-000024d0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000024e0: 436f 6c75 6d6e 2822 7769 7468 5f64 6566  Column("with_def
-000024f0: 6175 6c74 222c 2049 6e74 6567 6572 292c  ault", Integer),
-00002500: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00002510: 2020 2020 7420 3d20 5461 626c 6528 0a20      t = Table(. 
-00002520: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
-00002530: 7574 6564 5f63 6f6c 756d 6e5f 7461 626c  uted_column_tabl
-00002540: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00002550: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00002560: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
-00002570: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
-00002580: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
-00002590: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-000025a0: 6e28 226e 6f72 6d61 6c22 2c20 496e 7465  n("normal", Inte
-000025b0: 6765 7229 2c0a 2020 2020 2020 2020 2020  ger),.          
-000025c0: 2020 436f 6c75 6d6e 2822 636f 6d70 7574    Column("comput
-000025d0: 6564 5f6e 6f5f 666c 6167 222c 2049 6e74  ed_no_flag", Int
-000025e0: 6567 6572 2c20 436f 6d70 7574 6564 2822  eger, Computed("
-000025f0: 6e6f 726d 616c 202b 2034 3222 2929 2c0a  normal + 42")),.
-00002600: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00002610: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
-00002620: 7175 6972 6573 2e63 6f6d 7075 7465 645f  quires.computed_
-00002630: 636f 6c75 6d6e 735f 7669 7274 7561 6c2e  columns_virtual.
-00002640: 656e 6162 6c65 643a 0a20 2020 2020 2020  enabled:.       
-00002650: 2020 2020 2074 2e61 7070 656e 645f 636f       t.append_co
-00002660: 6c75 6d6e 280a 2020 2020 2020 2020 2020  lumn(.          
-00002670: 2020 2020 2020 436f 6c75 6d6e 280a 2020        Column(.  
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2263 6f6d 7075 7465 645f 7669 7274    "computed_virt
-000026a0: 7561 6c22 2c0a 2020 2020 2020 2020 2020  ual",.          
-000026b0: 2020 2020 2020 2020 2020 496e 7465 6765            Intege
-000026c0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-000026d0: 2020 2020 2020 2043 6f6d 7075 7465 6428         Computed(
-000026e0: 226e 6f72 6d61 6c20 2b20 3222 2c20 7065  "normal + 2", pe
-000026f0: 7273 6973 7465 643d 4661 6c73 6529 2c0a  rsisted=False),.
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00002720: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
-00002730: 6e67 2e72 6571 7569 7265 732e 636f 6d70  ng.requires.comp
-00002740: 7574 6564 5f63 6f6c 756d 6e73 5f73 746f  uted_columns_sto
-00002750: 7265 642e 656e 6162 6c65 643a 0a20 2020  red.enabled:.   
-00002760: 2020 2020 2020 2020 2074 2e61 7070 656e           t.appen
-00002770: 645f 636f 6c75 6d6e 280a 2020 2020 2020  d_column(.      
-00002780: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00002790: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000027a0: 2020 2020 2020 2263 6f6d 7075 7465 645f        "computed_
-000027b0: 7374 6f72 6564 222c 0a20 2020 2020 2020  stored",.       
-000027c0: 2020 2020 2020 2020 2020 2020 2049 6e74               Int
-000027d0: 6567 6572 2c0a 2020 2020 2020 2020 2020  eger,.          
-000027e0: 2020 2020 2020 2020 2020 436f 6d70 7574            Comput
-000027f0: 6564 2822 6e6f 726d 616c 202d 2034 3222  ed("normal - 42"
-00002800: 2c20 7065 7273 6973 7465 643d 5472 7565  , persisted=True
-00002810: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00002820: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00002830: 2029 0a0a 0a63 6c61 7373 2043 6f6d 7075   )...class Compu
-00002840: 7465 6452 6566 6c65 6374 696f 6e54 6573  tedReflectionTes
-00002850: 7428 5f43 6f6d 7075 7465 6452 6566 6c65  t(_ComputedRefle
-00002860: 6374 696f 6e54 6573 742c 2043 6f6d 7075  ctionTest, Compu
-00002870: 7465 6452 6566 6c65 6374 696f 6e46 6978  tedReflectionFix
-00002880: 7475 7265 5465 7374 293a 0a20 2020 2040  tureTest):.    @
-00002890: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
-000028a0: 2e73 6368 656d 6173 0a20 2020 2064 6566  .schemas.    def
-000028b0: 2074 6573 745f 6765 745f 636f 6c75 6d6e   test_get_column
-000028c0: 5f72 6574 7572 6e73 5f70 6572 7369 7374  _returns_persist
-000028d0: 6564 5f77 6974 685f 7363 6865 6d61 2873  ed_with_schema(s
-000028e0: 656c 6629 3a0a 2020 2020 2020 2020 696e  elf):.        in
-000028f0: 7370 203d 2069 6e73 7065 6374 2863 6f6e  sp = inspect(con
-00002900: 6669 672e 6462 290a 0a20 2020 2020 2020  fig.db)..       
-00002910: 2063 6f6c 7320 3d20 696e 7370 2e67 6574   cols = insp.get
-00002920: 5f63 6f6c 756d 6e73 2822 636f 6d70 7574  _columns("comput
-00002930: 6564 5f63 6f6c 756d 6e5f 7461 626c 6522  ed_column_table"
-00002940: 2c20 7363 6865 6d61 3d63 6f6e 6669 672e  , schema=config.
-00002950: 7465 7374 5f73 6368 656d 6129 0a20 2020  test_schema).   
-00002960: 2020 2020 2064 6174 6120 3d20 7b63 5b22       data = {c["
-00002970: 6e61 6d65 225d 3a20 6320 666f 7220 6320  name"]: c for c 
-00002980: 696e 2063 6f6c 737d 0a0a 2020 2020 2020  in cols}..      
-00002990: 2020 7365 6c66 2e63 6865 636b 5f63 6f6c    self.check_col
-000029a0: 756d 6e28 0a20 2020 2020 2020 2020 2020  umn(.           
-000029b0: 2064 6174 612c 0a20 2020 2020 2020 2020   data,.         
-000029c0: 2020 2022 636f 6d70 7574 6564 5f6e 6f5f     "computed_no_
-000029d0: 666c 6167 222c 0a20 2020 2020 2020 2020  flag",.         
-000029e0: 2020 2022 6e6f 726d 616c 2b34 3222 2c0a     "normal+42",.
-000029f0: 2020 2020 2020 2020 2020 2020 7465 7374              test
-00002a00: 696e 672e 7265 7175 6972 6573 2e63 6f6d  ing.requires.com
-00002a10: 7075 7465 645f 636f 6c75 6d6e 735f 6465  puted_columns_de
-00002a20: 6661 756c 745f 7065 7273 6973 7465 642e  fault_persisted.
-00002a30: 656e 6162 6c65 642c 0a20 2020 2020 2020  enabled,.       
-00002a40: 2029 0a20 2020 2020 2020 2069 6620 7465   ).        if te
-00002a50: 7374 696e 672e 7265 7175 6972 6573 2e63  sting.requires.c
-00002a60: 6f6d 7075 7465 645f 636f 6c75 6d6e 735f  omputed_columns_
-00002a70: 7669 7274 7561 6c2e 656e 6162 6c65 643a  virtual.enabled:
-00002a80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002a90: 662e 6368 6563 6b5f 636f 6c75 6d6e 280a  f.check_column(.
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00002ac0: 2020 2020 2020 2263 6f6d 7075 7465 645f        "computed_
-00002ad0: 7669 7274 7561 6c22 2c0a 2020 2020 2020  virtual",.      
-00002ae0: 2020 2020 2020 2020 2020 226e 6f72 6d61            "norma
-00002af0: 6c2f 3222 2c0a 2020 2020 2020 2020 2020  l/2",.          
-00002b00: 2020 2020 2020 4661 6c73 652c 0a20 2020        False,.   
-00002b10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00002b20: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
-00002b30: 7175 6972 6573 2e63 6f6d 7075 7465 645f  quires.computed_
-00002b40: 636f 6c75 6d6e 735f 7374 6f72 6564 2e65  columns_stored.e
-00002b50: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-00002b60: 2020 2020 7365 6c66 2e63 6865 636b 5f63      self.check_c
-00002b70: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-00002b80: 2020 2020 2020 2064 6174 612c 0a20 2020         data,.   
-00002b90: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00002ba0: 6d70 7574 6564 5f73 746f 7265 6422 2c0a  mputed_stored",.
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 226e 6f72 6d61 6c2d 3432 222c 0a20 2020  "normal-42",.   
-00002bd0: 2020 2020 2020 2020 2020 2020 2054 7275               Tru
-00002be0: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-00002bf0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00002c00: 726b 2e73 6b69 7028 2244 6566 6175 6c74  rk.skip("Default
-00002c10: 2076 616c 7565 7320 6172 6520 6e6f 7420   values are not 
-00002c20: 7375 7070 6f72 7465 642e 2229 0a20 2020  supported.").   
-00002c30: 2064 6566 2074 6573 745f 636f 6d70 7574   def test_comput
-00002c40: 6564 5f63 6f6c 5f64 6566 6175 6c74 5f6e  ed_col_default_n
-00002c50: 6f74 5f73 6574 2873 656c 6629 3a0a 2020  ot_set(self):.  
-00002c60: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00002c70: 6465 6620 7465 7374 5f67 6574 5f63 6f6c  def test_get_col
-00002c80: 756d 6e5f 7265 7475 726e 735f 636f 6d70  umn_returns_comp
-00002c90: 7574 6564 2873 656c 6629 3a0a 2020 2020  uted(self):.    
-00002ca0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002cb0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
-00002cc0: 3a0a 0a20 2020 2020 2020 2049 6e20 5370  :..        In Sp
-00002cd0: 616e 6e65 7220 616c 6c20 7468 6520 6765  anner all the ge
-00002ce0: 6e65 7261 7465 6420 636f 6c75 6d6e 7320  nerated columns 
-00002cf0: 6172 6520 5354 4f52 4544 2c0a 2020 2020  are STORED,.    
-00002d00: 2020 2020 6d65 616e 696e 6720 7468 6572      meaning ther
-00002d10: 6520 6172 6520 6e6f 2070 6572 7369 7374  e are no persist
-00002d20: 6564 2061 6e64 206e 6f74 2070 6572 7369  ed and not persi
-00002d30: 7374 6564 0a20 2020 2020 2020 2028 696e  sted.        (in
-00002d40: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
-00002d50: 6520 5351 4c41 6c63 6865 6d79 2920 636f  e SQLAlchemy) co
-00002d60: 6c75 6d6e 732e 2054 6865 0a20 2020 2020  lumns. The.     
-00002d70: 2020 206d 6574 686f 6420 6f76 6572 7269     method overri
-00002d80: 6465 206f 6d69 7473 2074 6865 2070 6572  de omits the per
-00002d90: 7369 7374 656e 6365 2072 6566 6c65 6374  sistence reflect
-00002da0: 696f 6e20 6368 6563 6b73 2e0a 2020 2020  ion checks..    
-00002db0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002dc0: 696e 7370 203d 2069 6e73 7065 6374 2863  insp = inspect(c
-00002dd0: 6f6e 6669 672e 6462 290a 0a20 2020 2020  onfig.db)..     
-00002de0: 2020 2063 6f6c 7320 3d20 696e 7370 2e67     cols = insp.g
-00002df0: 6574 5f63 6f6c 756d 6e73 2822 636f 6d70  et_columns("comp
-00002e00: 7574 6564 5f64 6566 6175 6c74 5f74 6162  uted_default_tab
-00002e10: 6c65 2229 0a20 2020 2020 2020 2064 6174  le").        dat
-00002e20: 6120 3d20 7b63 5b22 6e61 6d65 225d 3a20  a = {c["name"]: 
-00002e30: 6320 666f 7220 6320 696e 2063 6f6c 737d  c for c in cols}
-00002e40: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-00002e50: 2069 6e20 2822 6964 222c 2022 6e6f 726d   in ("id", "norm
-00002e60: 616c 222c 2022 7769 7468 5f64 6566 6175  al", "with_defau
-00002e70: 6c74 2229 3a0a 2020 2020 2020 2020 2020  lt"):.          
-00002e80: 2020 6973 5f74 7275 6528 2263 6f6d 7075    is_true("compu
-00002e90: 7465 6422 206e 6f74 2069 6e20 6461 7461  ted" not in data
-00002ea0: 5b6b 6579 5d29 0a20 2020 2020 2020 2063  [key]).        c
-00002eb0: 6f6d 7044 6174 6120 3d20 6461 7461 5b22  ompData = data["
-00002ec0: 636f 6d70 7574 6564 5f63 6f6c 225d 0a20  computed_col"]. 
-00002ed0: 2020 2020 2020 2069 735f 7472 7565 2822         is_true("
-00002ee0: 636f 6d70 7574 6564 2220 696e 2063 6f6d  computed" in com
-00002ef0: 7044 6174 6129 0a20 2020 2020 2020 2069  pData).        i
-00002f00: 735f 7472 7565 2822 7371 6c74 6578 7422  s_true("sqltext"
-00002f10: 2069 6e20 636f 6d70 4461 7461 5b22 636f   in compData["co
-00002f20: 6d70 7574 6564 225d 290a 2020 2020 2020  mputed"]).      
-00002f30: 2020 6571 5f28 7365 6c66 2e6e 6f72 6d61    eq_(self.norma
-00002f40: 6c69 7a65 2863 6f6d 7044 6174 615b 2263  lize(compData["c
-00002f50: 6f6d 7075 7465 6422 5d5b 2273 716c 7465  omputed"]["sqlte
-00002f60: 7874 225d 292c 2022 6e6f 726d 616c 2b34  xt"]), "normal+4
-00002f70: 3222 290a 0a20 2020 2064 6566 2074 6573  2")..    def tes
-00002f80: 745f 6372 6561 7465 5f6e 6f74 5f6e 756c  t_create_not_nul
-00002f90: 6c5f 636f 6d70 7574 6564 5f63 6f6c 756d  l_computed_colum
-00002fa0: 6e28 7365 6c66 2c20 636f 6e6e 6563 7469  n(self, connecti
-00002fb0: 6f6e 293a 0a20 2020 2020 2020 2022 2222  on):.        """
-00002fc0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-00002fd0: 2054 4553 543a 0a0a 2020 2020 2020 2020   TEST:..        
-00002fe0: 4368 6563 6b20 7468 6174 206f 6e20 6372  Check that on cr
-00002ff0: 6561 7469 6e67 2061 2063 6f6d 7075 7465  eating a compute
-00003000: 6420 636f 6c75 6d6e 2077 6974 6820 6120  d column with a 
-00003010: 4e4f 5420 4e55 4c4c 0a20 2020 2020 2020  NOT NULL.       
-00003020: 2063 6c61 7573 6520 7468 6520 636c 6175   clause the clau
-00003030: 7365 2069 7320 7365 7420 696e 2066 726f  se is set in fro
-00003040: 6e74 206f 6620 7468 6520 636f 6d70 7574  nt of the comput
-00003050: 6564 2063 6f6c 756d 6e0a 2020 2020 2020  ed column.      
-00003060: 2020 7374 6174 656d 656e 7420 6465 6669    statement defi
-00003070: 6e69 7469 6f6e 2061 6e64 2064 6f65 736e  nition and doesn
-00003080: 2774 2063 6175 7365 2066 6169 6c75 7265  't cause failure
-00003090: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-000030a0: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-000030b0: 3d20 4d65 7461 4461 7461 2829 0a0a 2020  = MetaData()..  
-000030c0: 2020 2020 2020 5461 626c 6528 0a20 2020        Table(.   
-000030d0: 2020 2020 2020 2020 2022 5369 6e67 6572           "Singer
-000030e0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000030f0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00003100: 2020 2020 2020 436f 6c75 6d6e 2822 5369        Column("Si
-00003110: 6e67 6572 4964 222c 2053 7472 696e 6728  ngerId", String(
-00003120: 3336 292c 2070 7269 6d61 7279 5f6b 6579  36), primary_key
-00003130: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
-00003140: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-00003150: 2020 2020 436f 6c75 6d6e 2822 4669 7273      Column("Firs
-00003160: 744e 616d 6522 2c20 5374 7269 6e67 2832  tName", String(2
-00003170: 3030 2929 2c0a 2020 2020 2020 2020 2020  00)),.          
-00003180: 2020 436f 6c75 6d6e 2822 4c61 7374 4e61    Column("LastNa
-00003190: 6d65 222c 2053 7472 696e 6728 3230 3029  me", String(200)
-000031a0: 2c20 6e75 6c6c 6162 6c65 3d46 616c 7365  , nullable=False
-000031b0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-000031c0: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-000031d0: 2020 2020 2020 2022 4675 6c6c 4e61 6d65         "FullName
-000031e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000031f0: 2020 2053 7472 696e 6728 3430 3029 2c0a     String(400),.
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 436f 6d70 7574 6564 2822 434f 414c 4553  Computed("COALES
-00003220: 4345 2846 6972 7374 4e61 6d65 207c 7c20  CE(FirstName || 
-00003230: 2720 272c 2027 2729 207c 7c20 4c61 7374  ' ', '') || Last
-00003240: 4e61 6d65 2229 2c0a 2020 2020 2020 2020  Name"),.        
-00003250: 2020 2020 2020 2020 6e75 6c6c 6162 6c65          nullable
-00003260: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00003270: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
-00003280: 0a0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
-00003290: 7461 2e63 7265 6174 655f 616c 6c28 636f  ta.create_all(co
-000032a0: 6e6e 6563 7469 6f6e 290a 0a0a 636c 6173  nnection)...clas
-000032b0: 7320 436f 6d70 6f6e 656e 7452 6566 6c65  s ComponentRefle
-000032c0: 6374 696f 6e54 6573 7428 5f43 6f6d 706f  ctionTest(_Compo
-000032d0: 6e65 6e74 5265 666c 6563 7469 6f6e 5465  nentReflectionTe
-000032e0: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
-000032f0: 2e6d 6172 6b2e 736b 6970 2822 536b 6970  .mark.skip("Skip
-00003300: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-00003310: 6e6f 745f 6578 6973 7469 6e67 5f74 6162  not_existing_tab
-00003320: 6c65 2873 656c 662c 206d 6574 686f 642c  le(self, method,
-00003330: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
-00003340: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003350: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00003360: 2064 6566 2064 6566 696e 655f 7461 626c   def define_tabl
-00003370: 6573 2863 6c73 2c20 6d65 7461 6461 7461  es(cls, metadata
-00003380: 293a 0a20 2020 2020 2020 2063 6c73 2e64  ):.        cls.d
-00003390: 6566 696e 655f 7265 666c 6563 7465 645f  efine_reflected_
-000033a0: 7461 626c 6573 286d 6574 6164 6174 612c  tables(metadata,
-000033b0: 204e 6f6e 6529 0a0a 2020 2020 4063 6c61   None)..    @cla
-000033c0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-000033d0: 2064 6566 696e 655f 7669 6577 7328 636c   define_views(cl
-000033e0: 732c 206d 6574 6164 6174 612c 2073 6368  s, metadata, sch
-000033f0: 656d 6129 3a0a 2020 2020 2020 2020 7461  ema):.        ta
-00003400: 626c 655f 696e 666f 203d 207b 0a20 2020  ble_info = {.   
-00003410: 2020 2020 2020 2020 2022 6469 6e67 616c           "dingal
-00003420: 696e 6773 223a 205b 0a20 2020 2020 2020  ings": [.       
-00003430: 2020 2020 2020 2020 2022 6469 6e67 616c           "dingal
-00003440: 696e 675f 6964 222c 0a20 2020 2020 2020  ing_id",.       
-00003450: 2020 2020 2020 2020 2022 6164 6472 6573           "addres
-00003460: 735f 6964 222c 0a20 2020 2020 2020 2020  s_id",.         
-00003470: 2020 2020 2020 2022 6461 7461 222c 0a20         "data",. 
-00003480: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003490: 6964 5f75 7365 7222 2c0a 2020 2020 2020  id_user",.      
-000034a0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-000034b0: 2020 2020 2022 7573 6572 7322 3a20 5b22       "users": ["
-000034c0: 7573 6572 5f69 6422 2c20 2274 6573 7431  user_id", "test1
-000034d0: 222c 2022 7465 7374 3222 5d2c 0a20 2020  ", "test2"],.   
-000034e0: 2020 2020 2020 2020 2022 656d 6169 6c5f           "email_
-000034f0: 6164 6472 6573 7365 7322 3a20 5b22 6164  addresses": ["ad
-00003500: 6472 6573 735f 6964 222c 2022 7265 6d6f  dress_id", "remo
-00003510: 7465 5f75 7365 725f 6964 222c 2022 656d  te_user_id", "em
-00003520: 6169 6c5f 6164 6472 6573 7322 5d2c 0a20  ail_address"],. 
-00003530: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00003540: 2069 6620 7465 7374 696e 672e 7265 7175   if testing.requ
-00003550: 6972 6573 2e73 656c 665f 7265 6665 7265  ires.self_refere
-00003560: 6e74 6961 6c5f 666f 7265 6967 6e5f 6b65  ntial_foreign_ke
-00003570: 7973 2e65 6e61 626c 6564 3a0a 2020 2020  ys.enabled:.    
-00003580: 2020 2020 2020 2020 7461 626c 655f 696e          table_in
-00003590: 666f 5b22 7573 6572 7322 5d20 3d20 7461  fo["users"] = ta
-000035a0: 626c 655f 696e 666f 5b22 7573 6572 7322  ble_info["users"
-000035b0: 5d20 2b20 5b22 7061 7265 6e74 5f75 7365  ] + ["parent_use
-000035c0: 725f 6964 225d 0a20 2020 2020 2020 2069  r_id"].        i
-000035d0: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
-000035e0: 6573 2e6d 6174 6572 6961 6c69 7a65 645f  es.materialized_
-000035f0: 7669 6577 732e 656e 6162 6c65 643a 0a20  views.enabled:. 
-00003600: 2020 2020 2020 2020 2020 206d 6174 6572             mater
-00003610: 6961 6c69 7a65 6420 3d20 7b22 6469 6e67  ialized = {"ding
-00003620: 616c 696e 6773 227d 0a20 2020 2020 2020  alings"}.       
-00003630: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003640: 2020 206d 6174 6572 6961 6c69 7a65 6420     materialized 
-00003650: 3d20 7365 7428 290a 2020 2020 2020 2020  = set().        
-00003660: 666f 7220 7461 626c 655f 6e61 6d65 2069  for table_name i
-00003670: 6e20 2822 7573 6572 7322 2c20 2265 6d61  n ("users", "ema
-00003680: 696c 5f61 6464 7265 7373 6573 222c 2022  il_addresses", "
-00003690: 6469 6e67 616c 696e 6773 2229 3a0a 2020  dingalings"):.  
-000036a0: 2020 2020 2020 2020 2020 6675 6c6c 6e61            fullna
-000036b0: 6d65 203d 2074 6162 6c65 5f6e 616d 650a  me = table_name.
-000036c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000036d0: 6368 656d 613a 0a20 2020 2020 2020 2020  chema:.         
-000036e0: 2020 2020 2020 2066 756c 6c6e 616d 6520         fullname 
-000036f0: 3d20 6622 7b73 6368 656d 617d 2e7b 7461  = f"{schema}.{ta
-00003700: 626c 655f 6e61 6d65 7d22 0a20 2020 2020  ble_name}".     
-00003710: 2020 2020 2020 2076 6965 775f 6e61 6d65         view_name
-00003720: 203d 2066 756c 6c6e 616d 6520 2b20 225f   = fullname + "_
-00003730: 7622 0a20 2020 2020 2020 2020 2020 2070  v".            p
-00003740: 7265 6669 7820 3d20 224d 4154 4552 4941  refix = "MATERIA
-00003750: 4c49 5a45 4420 2220 6966 2074 6162 6c65  LIZED " if table
-00003760: 5f6e 616d 6520 696e 206d 6174 6572 6961  _name in materia
-00003770: 6c69 7a65 6420 656c 7365 2022 220a 2020  lized else "".  
-00003780: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00003790: 7320 3d20 2222 0a20 2020 2020 2020 2020  s = "".         
-000037a0: 2020 2066 6f72 2063 6f6c 756d 6e20 696e     for column in
-000037b0: 2074 6162 6c65 5f69 6e66 6f5b 7461 626c   table_info[tabl
-000037c0: 655f 6e61 6d65 5d3a 0a20 2020 2020 2020  e_name]:.       
-000037d0: 2020 2020 2020 2020 2073 746d 7420 3d20           stmt = 
-000037e0: 7461 626c 655f 6e61 6d65 202b 2022 2e22  table_name + "."
-000037f0: 202b 2063 6f6c 756d 6e20 2b20 2220 4153   + column + " AS
-00003800: 2022 202b 2063 6f6c 756d 6e0a 2020 2020   " + column.    
-00003810: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00003820: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
-00003830: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00003840: 6d6e 7320 3d20 636f 6c75 6d6e 7320 2b20  mns = columns + 
-00003850: 222c 2022 202b 2073 746d 740a 2020 2020  ", " + stmt.    
-00003860: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003870: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003880: 2020 2020 2020 636f 6c75 6d6e 7320 3d20        columns = 
-00003890: 7374 6d74 0a20 2020 2020 2020 2020 2020  stmt.           
-000038a0: 2071 7565 7279 203d 2066 2222 2243 5245   query = f"""CRE
-000038b0: 4154 4520 7b70 7265 6669 787d 5649 4557  ATE {prefix}VIEW
-000038c0: 207b 7669 6577 5f6e 616d 657d 0a20 2020   {view_name}.   
-000038d0: 2020 2020 2020 2020 2020 2020 2053 514c               SQL
-000038e0: 2053 4543 5552 4954 5920 494e 564f 4b45   SECURITY INVOKE
-000038f0: 520a 2020 2020 2020 2020 2020 2020 2020  R.              
-00003900: 2020 4153 2053 454c 4543 5420 7b63 6f6c    AS SELECT {col
-00003910: 756d 6e73 7d0a 2020 2020 2020 2020 2020  umns}.          
-00003920: 2020 2020 2020 4652 4f4d 207b 6675 6c6c        FROM {full
-00003930: 6e61 6d65 7d22 2222 0a0a 2020 2020 2020  name}"""..      
-00003940: 2020 2020 2020 6576 656e 742e 6c69 7374        event.list
-00003950: 656e 286d 6574 6164 6174 612c 2022 6166  en(metadata, "af
-00003960: 7465 725f 6372 6561 7465 222c 2044 444c  ter_create", DDL
-00003970: 2871 7565 7279 2929 0a20 2020 2020 2020  (query)).       
-00003980: 2020 2020 2069 6620 7461 626c 655f 6e61       if table_na
-00003990: 6d65 2069 6e20 6d61 7465 7269 616c 697a  me in materializ
-000039a0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-000039b0: 2020 2020 696e 6465 785f 6e61 6d65 203d      index_name =
-000039c0: 2022 6d61 745f 696e 6465 7822 0a20 2020   "mat_index".   
-000039d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000039e0: 7363 6865 6d61 2061 6e64 2074 6573 7469  schema and testi
-000039f0: 6e67 2e61 6761 696e 7374 2822 6f72 6163  ng.against("orac
-00003a00: 6c65 2229 3a0a 2020 2020 2020 2020 2020  le"):.          
-00003a10: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-00003a20: 6e61 6d65 203d 2066 227b 7363 6865 6d61  name = f"{schema
-00003a30: 7d2e 7b69 6e64 6578 5f6e 616d 657d 220a  }.{index_name}".
-00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 6964 7820 3d20 6622 4352 4541 5445 2049  idx = f"CREATE I
-00003a60: 4e44 4558 207b 696e 6465 785f 6e61 6d65  NDEX {index_name
-00003a70: 7d20 4f4e 207b 7669 6577 5f6e 616d 657d  } ON {view_name}
-00003a80: 2864 6174 6129 220a 2020 2020 2020 2020  (data)".        
-00003a90: 2020 2020 2020 2020 6576 656e 742e 6c69          event.li
-00003aa0: 7374 656e 286d 6574 6164 6174 612c 2022  sten(metadata, "
-00003ab0: 6166 7465 725f 6372 6561 7465 222c 2044  after_create", D
-00003ac0: 444c 2869 6478 2929 0a20 2020 2020 2020  DL(idx)).       
-00003ad0: 2020 2020 2065 7665 6e74 2e6c 6973 7465       event.liste
-00003ae0: 6e28 6d65 7461 6461 7461 2c20 2262 6566  n(metadata, "bef
-00003af0: 6f72 655f 6472 6f70 222c 2044 444c 2866  ore_drop", DDL(f
-00003b00: 2244 524f 5020 7b70 7265 6669 787d 5649  "DROP {prefix}VI
-00003b10: 4557 207b 7669 6577 5f6e 616d 657d 2229  EW {view_name}")
-00003b20: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-00003b30: 686f 640a 2020 2020 6465 6620 6465 6669  hod.    def defi
-00003b40: 6e65 5f72 6566 6c65 6374 6564 5f74 6162  ne_reflected_tab
-00003b50: 6c65 7328 636c 732c 206d 6574 6164 6174  les(cls, metadat
-00003b60: 612c 2073 6368 656d 6129 3a0a 2020 2020  a, schema):.    
-00003b70: 2020 2020 6966 2073 6368 656d 613a 0a20      if schema:. 
-00003b80: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00003b90: 615f 7072 6566 6978 203d 2073 6368 656d  a_prefix = schem
-00003ba0: 6120 2b20 222e 220a 2020 2020 2020 2020  a + ".".        
-00003bb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003bc0: 2020 7363 6865 6d61 5f70 7265 6669 7820    schema_prefix 
-00003bd0: 3d20 2222 0a0a 2020 2020 2020 2020 6966  = ""..        if
-00003be0: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
-00003bf0: 732e 7365 6c66 5f72 6566 6572 656e 7469  s.self_referenti
-00003c00: 616c 5f66 6f72 6569 676e 5f6b 6579 732e  al_foreign_keys.
-00003c10: 656e 6162 6c65 643a 0a20 2020 2020 2020  enabled:.       
-00003c20: 2020 2020 2075 7365 7273 203d 2054 6162       users = Tab
-00003c30: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00003c40: 2020 2020 2275 7365 7273 222c 0a20 2020      "users",.   
-00003c50: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00003c60: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
-00003c70: 2020 2020 2020 2043 6f6c 756d 6e28 2275         Column("u
-00003c80: 7365 725f 6964 222c 2073 716c 616c 6368  ser_id", sqlalch
-00003c90: 656d 792e 494e 542c 2070 7269 6d61 7279  emy.INT, primary
-00003ca0: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
-00003cb0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00003cc0: 6d6e 2822 7465 7374 3122 2c20 7371 6c61  mn("test1", sqla
-00003cd0: 6c63 6865 6d79 2e43 4841 5228 3529 2c20  lchemy.CHAR(5), 
-00003ce0: 6e75 6c6c 6162 6c65 3d46 616c 7365 292c  nullable=False),
-00003cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d00: 2043 6f6c 756d 6e28 2274 6573 7432 222c   Column("test2",
-00003d10: 2073 716c 616c 6368 656d 792e 466c 6f61   sqlalchemy.Floa
-00003d20: 7428 3529 2c20 6e75 6c6c 6162 6c65 3d46  t(5), nullable=F
-00003d30: 616c 7365 292c 0a20 2020 2020 2020 2020  alse),.         
-00003d40: 2020 2020 2020 2043 6f6c 756d 6e28 0a20         Column(. 
-00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d60: 2020 2022 7061 7265 6e74 5f75 7365 725f     "parent_user_
-00003d70: 6964 222c 0a20 2020 2020 2020 2020 2020  id",.           
-00003d80: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-00003d90: 656d 792e 496e 7465 6765 722c 0a20 2020  emy.Integer,.   
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2073 716c 616c 6368 656d 792e 466f 7265   sqlalchemy.Fore
-00003dc0: 6967 6e4b 6579 280a 2020 2020 2020 2020  ignKey(.        
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2225 7375 7365 7273 2e75 7365 725f 6964  "%susers.user_id
-00003df0: 2220 2520 7363 6865 6d61 5f70 7265 6669  " % schema_prefi
-00003e00: 782c 206e 616d 653d 2275 7365 725f 6964  x, name="user_id
-00003e10: 5f66 6b22 0a20 2020 2020 2020 2020 2020  _fk".           
-00003e20: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00003e30: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003e50: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
-00003e60: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00003e70: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
-00003e80: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00003e90: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00003ea0: 2020 2020 2020 2020 2020 7573 6572 7320            users 
-00003eb0: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
-00003ec0: 2020 2020 2020 2020 2022 7573 6572 7322           "users"
-00003ed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003ee0: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
-00003ef0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00003f00: 6d6e 2822 7573 6572 5f69 6422 2c20 7371  mn("user_id", sq
-00003f10: 6c61 6c63 6865 6d79 2e49 4e54 2c20 7072  lalchemy.INT, pr
-00003f20: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
-00003f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f40: 2043 6f6c 756d 6e28 2274 6573 7431 222c   Column("test1",
-00003f50: 2073 716c 616c 6368 656d 792e 4348 4152   sqlalchemy.CHAR
-00003f60: 2835 292c 206e 756c 6c61 626c 653d 4661  (5), nullable=Fa
-00003f70: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
-00003f80: 2020 2020 2020 436f 6c75 6d6e 2822 7465        Column("te
-00003f90: 7374 3222 2c20 7371 6c61 6c63 6865 6d79  st2", sqlalchemy
-00003fa0: 2e46 6c6f 6174 2835 292c 206e 756c 6c61  .Float(5), nulla
-00003fb0: 626c 653d 4661 6c73 6529 2c0a 2020 2020  ble=False),.    
-00003fc0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-00003fd0: 6d61 3d73 6368 656d 612c 0a20 2020 2020  ma=schema,.     
-00003fe0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-00003ff0: 6e65 6564 735f 666b 3d54 7275 652c 0a20  needs_fk=True,. 
-00004000: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00004010: 2020 2020 2020 5461 626c 6528 0a20 2020        Table(.   
-00004020: 2020 2020 2020 2020 2022 6469 6e67 616c           "dingal
-00004030: 696e 6773 222c 0a20 2020 2020 2020 2020  ings",.         
-00004040: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
-00004050: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00004060: 2264 696e 6761 6c69 6e67 5f69 6422 2c20  "dingaling_id", 
-00004070: 7371 6c61 6c63 6865 6d79 2e49 6e74 6567  sqlalchemy.Integ
-00004080: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
-00004090: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-000040a0: 2020 2043 6f6c 756d 6e28 0a20 2020 2020     Column(.     
-000040b0: 2020 2020 2020 2020 2020 2022 6164 6472             "addr
-000040c0: 6573 735f 6964 222c 0a20 2020 2020 2020  ess_id",.       
-000040d0: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-000040e0: 656d 792e 496e 7465 6765 722c 0a20 2020  emy.Integer,.   
-000040f0: 2020 2020 2020 2020 2020 2020 2073 716c               sql
-00004100: 616c 6368 656d 792e 466f 7265 6967 6e4b  alchemy.ForeignK
-00004110: 6579 2822 2573 656d 6169 6c5f 6164 6472  ey("%semail_addr
-00004120: 6573 7365 732e 6164 6472 6573 735f 6964  esses.address_id
-00004130: 2220 2520 7363 6865 6d61 5f70 7265 6669  " % schema_prefi
-00004140: 7829 2c0a 2020 2020 2020 2020 2020 2020  x),.            
-00004150: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00004160: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-00004170: 2020 2020 2020 2022 6964 5f75 7365 7222         "id_user"
-00004180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004190: 2020 7371 6c61 6c63 6865 6d79 2e49 6e74    sqlalchemy.Int
-000041a0: 6567 6572 2c0a 2020 2020 2020 2020 2020  eger,.          
-000041b0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-000041c0: 2e46 6f72 6569 676e 4b65 7928 2225 7375  .ForeignKey("%su
-000041d0: 7365 7273 2e75 7365 725f 6964 2220 2520  sers.user_id" % 
-000041e0: 7363 6865 6d61 5f70 7265 6669 7829 2c0a  schema_prefix),.
-000041f0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00004200: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00004210: 6e28 2264 6174 6122 2c20 7371 6c61 6c63  n("data", sqlalc
-00004220: 6865 6d79 2e53 7472 696e 6728 3330 2929  hemy.String(30))
-00004230: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
-00004240: 6865 6d61 3d73 6368 656d 612c 0a20 2020  hema=schema,.   
-00004250: 2020 2020 2020 2020 2074 6573 745f 6e65           test_ne
-00004260: 6564 735f 666b 3d54 7275 652c 0a20 2020  eds_fk=True,.   
-00004270: 2020 2020 2029 0a20 2020 2020 2020 2054       ).        T
-00004280: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
-00004290: 2020 2265 6d61 696c 5f61 6464 7265 7373    "email_address
-000042a0: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
-000042b0: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-000042c0: 2020 2020 2020 2043 6f6c 756d 6e28 2261         Column("a
-000042d0: 6464 7265 7373 5f69 6422 2c20 7371 6c61  ddress_id", sqla
-000042e0: 6c63 6865 6d79 2e49 6e74 6567 6572 2c20  lchemy.Integer, 
-000042f0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00004300: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00004310: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-00004320: 2020 2020 2020 2022 7265 6d6f 7465 5f75         "remote_u
-00004330: 7365 725f 6964 222c 0a20 2020 2020 2020  ser_id",.       
-00004340: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-00004350: 656d 792e 496e 7465 6765 722c 0a20 2020  emy.Integer,.   
-00004360: 2020 2020 2020 2020 2020 2020 2073 716c               sql
-00004370: 616c 6368 656d 792e 466f 7265 6967 6e4b  alchemy.ForeignK
-00004380: 6579 2875 7365 7273 2e63 2e75 7365 725f  ey(users.c.user_
-00004390: 6964 292c 0a20 2020 2020 2020 2020 2020  id),.           
-000043a0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-000043b0: 436f 6c75 6d6e 2822 656d 6169 6c5f 6164  Column("email_ad
-000043c0: 6472 6573 7322 2c20 7371 6c61 6c63 6865  dress", sqlalche
-000043d0: 6d79 2e53 7472 696e 6728 3230 2929 2c0a  my.String(20)),.
-000043e0: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-000043f0: 6c63 6865 6d79 2e50 7269 6d61 7279 4b65  lchemy.PrimaryKe
-00004400: 7943 6f6e 7374 7261 696e 7428 2261 6464  yConstraint("add
-00004410: 7265 7373 5f69 6422 2c20 6e61 6d65 3d22  ress_id", name="
-00004420: 656d 6169 6c5f 6164 5f70 6b22 292c 0a20  email_ad_pk"),. 
-00004430: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00004440: 613d 7363 6865 6d61 2c0a 2020 2020 2020  a=schema,.      
-00004450: 2020 2020 2020 7465 7374 5f6e 6565 6473        test_needs
-00004460: 5f66 6b3d 5472 7565 2c0a 2020 2020 2020  _fk=True,.      
-00004470: 2020 290a 2020 2020 2020 2020 5461 626c    ).        Tabl
-00004480: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00004490: 636f 6d6d 656e 745f 7465 7374 222c 0a20  comment_test",. 
-000044a0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-000044b0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-000044c0: 2043 6f6c 756d 6e28 2269 6422 2c20 7371   Column("id", sq
-000044d0: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
-000044e0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-000044f0: 7565 2c20 636f 6d6d 656e 743d 2269 6420  ue, comment="id 
-00004500: 636f 6d6d 656e 7422 292c 0a20 2020 2020  comment"),.     
-00004510: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
-00004520: 6174 6122 2c20 7371 6c61 6c63 6865 6d79  ata", sqlalchemy
-00004530: 2e53 7472 696e 6728 3230 292c 2063 6f6d  .String(20), com
-00004540: 6d65 6e74 3d22 6461 7461 2025 2063 6f6d  ment="data % com
-00004550: 6d65 6e74 2229 2c0a 2020 2020 2020 2020  ment"),.        
-00004560: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
-00004570: 2020 2020 2020 2020 2020 2020 2264 3222              "d2"
-00004580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004590: 2020 7371 6c61 6c63 6865 6d79 2e53 7472    sqlalchemy.Str
-000045a0: 696e 6728 3230 292c 0a20 2020 2020 2020  ing(20),.       
-000045b0: 2020 2020 2020 2020 2063 6f6d 6d65 6e74           comment
-000045c0: 3d72 2222 2243 6f6d 6d65 6e74 2074 7970  =r"""Comment typ
-000045d0: 6573 2074 7970 6520 7370 6565 6469 6c79  es type speedily
-000045e0: 2027 2022 205c 2027 2720 4675 6e21 2222   ' " \ '' Fun!""
-000045f0: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00004600: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
-00004610: 6865 6d61 3d73 6368 656d 612c 0a20 2020  hema=schema,.   
-00004620: 2020 2020 2020 2020 2063 6f6d 6d65 6e74           comment
-00004630: 3d72 2222 2274 6865 2074 6573 7420 2520  =r"""the test % 
-00004640: 2720 2220 5c20 7461 626c 6520 636f 6d6d  ' " \ table comm
-00004650: 656e 7422 2222 2c0a 2020 2020 2020 2020  ent""",.        
-00004660: 290a 2020 2020 2020 2020 5461 626c 6528  ).        Table(
-00004670: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00004680: 5f63 6f6e 7374 7261 696e 7473 222c 0a20  _constraints",. 
-00004690: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-000046a0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-000046b0: 2043 6f6c 756d 6e28 2264 6174 6122 2c20   Column("data", 
-000046c0: 7371 6c61 6c63 6865 6d79 2e53 7472 696e  sqlalchemy.Strin
-000046d0: 6728 3230 2929 2c0a 2020 2020 2020 2020  g(20)),.        
-000046e0: 2020 2020 7363 6865 6d61 3d73 6368 656d      schema=schem
-000046f0: 612c 0a20 2020 2020 2020 2029 0a0a 2020  a,.        )..  
-00004700: 2020 2020 2020 6966 2074 6573 7469 6e67        if testing
-00004710: 2e72 6571 7569 7265 732e 6372 6f73 735f  .requires.cross_
-00004720: 7363 6865 6d61 5f66 6b5f 7265 666c 6563  schema_fk_reflec
-00004730: 7469 6f6e 2e65 6e61 626c 6564 3a0a 2020  tion.enabled:.  
-00004740: 2020 2020 2020 2020 2020 6966 2073 6368            if sch
-00004750: 656d 6120 6973 204e 6f6e 653a 0a20 2020  ema is None:.   
-00004760: 2020 2020 2020 2020 2020 2020 2054 6162               Tab
-00004770: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00004780: 2020 2020 2020 2020 226c 6f63 616c 5f74          "local_t
-00004790: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
-000047a0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-000047b0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-000047c0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-000047d0: 2269 6422 2c20 7371 6c61 6c63 6865 6d79  "id", sqlalchemy
-000047e0: 2e49 6e74 6567 6572 2c20 7072 696d 6172  .Integer, primar
-000047f0: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2043 6f6c 756d 6e28 2264 6174 6122 2c20   Column("data", 
-00004820: 7371 6c61 6c63 6865 6d79 2e53 7472 696e  sqlalchemy.Strin
-00004830: 6728 3230 2929 2c0a 2020 2020 2020 2020  g(20)),.        
-00004840: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00004850: 6d6e 280a 2020 2020 2020 2020 2020 2020  mn(.            
-00004860: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
-00004870: 6f74 655f 6964 222c 0a20 2020 2020 2020  ote_id",.       
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2046 6f72 6569 676e 4b65 7928 2225 732e   ForeignKey("%s.
-000048a0: 7265 6d6f 7465 5f74 6162 6c65 5f32 2e69  remote_table_2.i
-000048b0: 6422 2025 2074 6573 7469 6e67 2e63 6f6e  d" % testing.con
-000048c0: 6669 672e 7465 7374 5f73 6368 656d 6129  fig.test_schema)
-000048d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000048e0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-000048f0: 2020 2020 2020 2020 2020 2020 2074 6573               tes
-00004900: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
-00004910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004920: 2020 2020 2073 6368 656d 613d 636f 6e66       schema=conf
-00004930: 6967 2e64 622e 6469 616c 6563 742e 6465  ig.db.dialect.de
-00004940: 6661 756c 745f 7363 6865 6d61 5f6e 616d  fault_schema_nam
-00004950: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00004960: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00004970: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00004980: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
-00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2272 656d 6f74 655f 7461 626c 6522    "remote_table"
-000049b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000049c0: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 436f 6c75 6d6e 2822 6964 222c      Column("id",
-000049f0: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
-00004a00: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00004a10: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00004a20: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00004a30: 6d6e 280a 2020 2020 2020 2020 2020 2020  mn(.            
-00004a40: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
-00004a50: 616c 5f69 6422 2c0a 2020 2020 2020 2020  al_id",.        
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 466f 7265 6967 6e4b 6579 280a 2020 2020  ForeignKey(.    
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2020 2020 2020 2225 732e 6c6f 6361          "%s.loca
-00004aa0: 6c5f 7461 626c 652e 6964 2220 2520 636f  l_table.id" % co
-00004ab0: 6e66 6967 2e64 622e 6469 616c 6563 742e  nfig.db.dialect.
-00004ac0: 6465 6661 756c 745f 7363 6865 6d61 5f6e  default_schema_n
-00004ad0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00004ae0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00000320: 7565 7374 4f70 7469 6f6e 732c 2043 6c69  uestOptions, Cli
+00000330: 656e 740a 696d 706f 7274 2073 716c 616c  ent.import sqlal
+00000340: 6368 656d 790a 6672 6f6d 2073 716c 616c  chemy.from sqlal
+00000350: 6368 656d 7920 696d 706f 7274 2063 7265  chemy import cre
+00000360: 6174 655f 656e 6769 6e65 0a66 726f 6d20  ate_engine.from 
+00000370: 7371 6c61 6c63 6865 6d79 2e65 6e67 696e  sqlalchemy.engin
+00000380: 6520 696d 706f 7274 2049 6e73 7065 6374  e import Inspect
+00000390: 6f72 0a66 726f 6d20 7371 6c61 6c63 6865  or.from sqlalche
+000003a0: 6d79 2069 6d70 6f72 7420 696e 7370 6563  my import inspec
+000003b0: 740a 6672 6f6d 2073 716c 616c 6368 656d  t.from sqlalchem
+000003c0: 7920 696d 706f 7274 2074 6573 7469 6e67  y import testing
+000003d0: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
+000003e0: 2069 6d70 6f72 7420 466f 7265 6967 6e4b   import ForeignK
+000003f0: 6579 0a66 726f 6d20 7371 6c61 6c63 6865  ey.from sqlalche
+00000400: 6d79 2069 6d70 6f72 7420 4d65 7461 4461  my import MetaDa
+00000410: 7461 0a66 726f 6d20 7371 6c61 6c63 6865  ta.from sqlalche
+00000420: 6d79 2e65 6e67 696e 6520 696d 706f 7274  my.engine import
+00000430: 204f 626a 6563 744b 696e 640a 6672 6f6d   ObjectKind.from
+00000440: 2073 716c 616c 6368 656d 792e 656e 6769   sqlalchemy.engi
+00000450: 6e65 2069 6d70 6f72 7420 4f62 6a65 6374  ne import Object
+00000460: 5363 6f70 650a 6672 6f6d 2073 716c 616c  Scope.from sqlal
+00000470: 6368 656d 792e 7363 6865 6d61 2069 6d70  chemy.schema imp
+00000480: 6f72 7420 4444 4c0a 6672 6f6d 2073 716c  ort DDL.from sql
+00000490: 616c 6368 656d 792e 7363 6865 6d61 2069  alchemy.schema i
+000004a0: 6d70 6f72 7420 436f 6d70 7574 6564 0a66  mport Computed.f
+000004b0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+000004c0: 6573 7469 6e67 2069 6d70 6f72 7420 636f  esting import co
+000004d0: 6e66 6967 0a66 726f 6d20 7371 6c61 6c63  nfig.from sqlalc
+000004e0: 6865 6d79 2e74 6573 7469 6e67 2069 6d70  hemy.testing imp
+000004f0: 6f72 7420 656e 6769 6e65 730a 6672 6f6d  ort engines.from
+00000500: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000510: 696e 6720 696d 706f 7274 2065 715f 0a66  ing import eq_.f
+00000520: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000530: 6573 7469 6e67 2069 6d70 6f72 7420 7072  esting import pr
+00000540: 6f76 6964 655f 6d65 7461 6461 7461 2c20  ovide_metadata, 
+00000550: 656d 6974 735f 7761 726e 696e 670a 6672  emits_warning.fr
+00000560: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
+00000570: 7374 696e 6720 696d 706f 7274 2066 6978  sting import fix
+00000580: 7475 7265 730a 6672 6f6d 2073 716c 616c  tures.from sqlal
+00000590: 6368 656d 792e 7465 7374 696e 672e 7072  chemy.testing.pr
+000005a0: 6f76 6973 696f 6e20 696d 706f 7274 2074  ovision import t
+000005b0: 656d 705f 7461 626c 655f 6b65 7977 6f72  emp_table_keywor
+000005c0: 645f 6172 6773 0a66 726f 6d20 7371 6c61  d_args.from sqla
+000005d0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
+000005e0: 6368 656d 6120 696d 706f 7274 2043 6f6c  chema import Col
+000005f0: 756d 6e0a 6672 6f6d 2073 716c 616c 6368  umn.from sqlalch
+00000600: 656d 792e 7465 7374 696e 672e 7363 6865  emy.testing.sche
+00000610: 6d61 2069 6d70 6f72 7420 5461 626c 650a  ma import Table.
+00000620: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+00000630: 696d 706f 7274 206c 6974 6572 616c 5f63  import literal_c
+00000640: 6f6c 756d 6e0a 6672 6f6d 2073 716c 616c  olumn.from sqlal
+00000650: 6368 656d 7920 696d 706f 7274 2073 656c  chemy import sel
+00000660: 6563 740a 6672 6f6d 2073 716c 616c 6368  ect.from sqlalch
+00000670: 656d 7920 696d 706f 7274 2075 7469 6c0a  emy import util.
+00000680: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+00000690: 696d 706f 7274 2075 6e69 6f6e 0a66 726f  import union.fro
+000006a0: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
+000006b0: 6f72 7420 6576 656e 740a 6672 6f6d 2073  ort event.from s
+000006c0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
+000006d0: 2065 7869 7374 730a 6672 6f6d 2073 716c   exists.from sql
+000006e0: 616c 6368 656d 7920 696d 706f 7274 2042  alchemy import B
+000006f0: 6f6f 6c65 616e 0a66 726f 6d20 7371 6c61  oolean.from sqla
+00000700: 6c63 6865 6d79 2069 6d70 6f72 7420 466c  lchemy import Fl
+00000710: 6f61 740a 6672 6f6d 2073 716c 616c 6368  oat.from sqlalch
+00000720: 656d 7920 696d 706f 7274 204c 6172 6765  emy import Large
+00000730: 4269 6e61 7279 0a66 726f 6d20 7371 6c61  Binary.from sqla
+00000740: 6c63 6865 6d79 2069 6d70 6f72 7420 5374  lchemy import St
+00000750: 7269 6e67 0a66 726f 6d20 7371 6c61 6c63  ring.from sqlalc
+00000760: 6865 6d79 2e65 7874 2e64 6563 6c61 7261  hemy.ext.declara
+00000770: 7469 7665 2069 6d70 6f72 7420 6465 636c  tive import decl
+00000780: 6172 6174 6976 655f 6261 7365 0a66 726f  arative_base.fro
+00000790: 6d20 7371 6c61 6c63 6865 6d79 2e6f 726d  m sqlalchemy.orm
+000007a0: 2069 6d70 6f72 7420 7265 6c61 7469 6f6e   import relation
+000007b0: 7368 6970 0a66 726f 6d20 7371 6c61 6c63  ship.from sqlalc
+000007c0: 6865 6d79 2e6f 726d 2069 6d70 6f72 7420  hemy.orm import 
+000007d0: 5365 7373 696f 6e0a 6672 6f6d 2073 716c  Session.from sql
+000007e0: 616c 6368 656d 792e 7479 7065 7320 696d  alchemy.types im
+000007f0: 706f 7274 2049 6e74 6567 6572 0a66 726f  port Integer.fro
+00000800: 6d20 7371 6c61 6c63 6865 6d79 2e74 7970  m sqlalchemy.typ
+00000810: 6573 2069 6d70 6f72 7420 4e75 6d65 7269  es import Numeri
+00000820: 630a 6672 6f6d 2073 716c 616c 6368 656d  c.from sqlalchem
+00000830: 792e 7479 7065 7320 696d 706f 7274 2054  y.types import T
+00000840: 6578 740a 6672 6f6d 2073 716c 616c 6368  ext.from sqlalch
+00000850: 656d 792e 7465 7374 696e 6720 696d 706f  emy.testing impo
+00000860: 7274 2072 6571 7569 7265 730a 6672 6f6d  rt requires.from
+00000870: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000880: 696e 6720 696d 706f 7274 2069 735f 7472  ing import is_tr
+00000890: 7565 0a66 726f 6d20 7371 6c61 6c63 6865  ue.from sqlalche
+000008a0: 6d79 2069 6d70 6f72 7420 496e 6465 780a  my import Index.
+000008b0: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+000008c0: 696d 706f 7274 2074 7970 6573 0a66 726f  import types.fro
+000008d0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+000008e0: 7469 6e67 2e66 6978 7475 7265 7320 696d  ting.fixtures im
+000008f0: 706f 7274 2028 0a20 2020 2043 6f6d 7075  port (.    Compu
+00000900: 7465 6452 6566 6c65 6374 696f 6e46 6978  tedReflectionFix
+00000910: 7475 7265 5465 7374 2061 7320 5f43 6f6d  tureTest as _Com
+00000920: 7075 7465 6452 6566 6c65 6374 696f 6e46  putedReflectionF
+00000930: 6978 7475 7265 5465 7374 2c0a 290a 0a66  ixtureTest,.)..f
+00000940: 726f 6d20 676f 6f67 6c65 2e61 7069 5f63  rom google.api_c
+00000950: 6f72 652e 6461 7465 7469 6d65 5f68 656c  ore.datetime_hel
+00000960: 7065 7273 2069 6d70 6f72 7420 4461 7465  pers import Date
+00000970: 7469 6d65 5769 7468 4e61 6e6f 7365 636f  timeWithNanoseco
+00000980: 6e64 730a 0a66 726f 6d20 676f 6f67 6c65  nds..from google
+00000990: 2e63 6c6f 7564 2069 6d70 6f72 7420 7370  .cloud import sp
+000009a0: 616e 6e65 725f 6462 6170 690a 0a66 726f  anner_dbapi..fro
+000009b0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+000009c0: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
+000009d0: 6374 6520 696d 706f 7274 202a 2020 2320  cte import *  # 
+000009e0: 6e6f 7161 3a20 4634 3031 2c20 4634 3033  noqa: F401, F403
+000009f0: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
+00000a00: 2e74 6573 7469 6e67 2e73 7569 7465 2e74  .testing.suite.t
+00000a10: 6573 745f 6464 6c20 696d 706f 7274 202a  est_ddl import *
+00000a20: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
+00000a30: 4634 3033 0a66 726f 6d20 7371 6c61 6c63  F403.from sqlalc
+00000a40: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
+00000a50: 7465 2e74 6573 745f 6469 616c 6563 7420  te.test_dialect 
+00000a60: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
+00000a70: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
+00000a80: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+00000a90: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
+00000aa0: 696e 7365 7274 2069 6d70 6f72 7420 2a20  insert import * 
+00000ab0: 2023 206e 6f71 613a 2046 3430 312c 2046   # noqa: F401, F
+00000ac0: 3430 330a 6672 6f6d 2073 716c 616c 6368  403.from sqlalch
+00000ad0: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
+00000ae0: 652e 7465 7374 5f72 6566 6c65 6374 696f  e.test_reflectio
+00000af0: 6e20 696d 706f 7274 202a 2020 2320 6e6f  n import *  # no
+00000b00: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
+00000b10: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000b20: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+00000b30: 745f 6465 7072 6563 6174 696f 6e73 2069  t_deprecations i
+00000b40: 6d70 6f72 7420 2a20 2023 206e 6f71 613a  mport *  # noqa:
+00000b50: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
+00000b60: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000b70: 696e 672e 7375 6974 652e 7465 7374 5f72  ing.suite.test_r
+00000b80: 6573 756c 7473 2069 6d70 6f72 7420 2a20  esults import * 
+00000b90: 2023 206e 6f71 613a 2046 3430 312c 2046   # noqa: F401, F
+00000ba0: 3430 330a 6672 6f6d 2073 716c 616c 6368  403.from sqlalch
+00000bb0: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
+00000bc0: 652e 7465 7374 5f73 656c 6563 7420 696d  e.test_select im
+00000bd0: 706f 7274 202a 2020 2320 6e6f 7161 3a20  port *  # noqa: 
+00000be0: 4634 3031 2c20 4634 3033 0a66 726f 6d20  F401, F403.from 
+00000bf0: 7371 6c61 6c63 6865 6d79 2e74 6573 7469  sqlalchemy.testi
+00000c00: 6e67 2e73 7569 7465 2e74 6573 745f 7365  ng.suite.test_se
+00000c10: 7175 656e 6365 2069 6d70 6f72 7420 2a20  quence import * 
+00000c20: 2023 206e 6f71 613a 2046 3430 312c 2046   # noqa: F401, F
+00000c30: 3430 330a 6672 6f6d 2073 716c 616c 6368  403.from sqlalch
+00000c40: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
+00000c50: 652e 7465 7374 5f75 6e69 636f 6465 5f64  e.test_unicode_d
+00000c60: 646c 2069 6d70 6f72 7420 2a20 2023 206e  dl import *  # n
+00000c70: 6f71 613a 2046 3430 312c 2046 3430 330a  oqa: F401, F403.
+00000c80: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00000c90: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
+00000ca0: 7374 5f75 7064 6174 655f 6465 6c65 7465  st_update_delete
+00000cb0: 2069 6d70 6f72 7420 2a20 2023 206e 6f71   import *  # noq
+00000cc0: 613a 2046 3430 312c 2046 3430 330a 6672  a: F401, F403.fr
+00000cd0: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
+00000ce0: 7374 696e 672e 7375 6974 652e 7465 7374  sting.suite.test
+00000cf0: 5f63 7465 2069 6d70 6f72 7420 4354 4554  _cte import CTET
+00000d00: 6573 7420 6173 205f 4354 4554 6573 740a  est as _CTETest.
+00000d10: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00000d20: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
+00000d30: 7374 5f64 646c 2069 6d70 6f72 7420 5461  st_ddl import Ta
+00000d40: 626c 6544 444c 5465 7374 2061 7320 5f54  bleDDLTest as _T
+00000d50: 6162 6c65 4444 4c54 6573 740a 6672 6f6d  ableDDLTest.from
+00000d60: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000d70: 696e 672e 7375 6974 652e 7465 7374 5f64  ing.suite.test_d
+00000d80: 646c 2069 6d70 6f72 7420 280a 2020 2020  dl import (.    
+00000d90: 4675 7475 7265 5461 626c 6544 444c 5465  FutureTableDDLTe
+00000da0: 7374 2061 7320 5f46 7574 7572 6554 6162  st as _FutureTab
+00000db0: 6c65 4444 4c54 6573 742c 0a20 2020 204c  leDDLTest,.    L
+00000dc0: 6f6e 674e 616d 6542 6c6f 776f 7574 5465  ongNameBlowoutTe
+00000dd0: 7374 2061 7320 5f4c 6f6e 674e 616d 6542  st as _LongNameB
+00000de0: 6c6f 776f 7574 5465 7374 2c0a 290a 6672  lowoutTest,.).fr
+00000df0: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
+00000e00: 7374 696e 672e 7375 6974 652e 7465 7374  sting.suite.test
+00000e10: 5f75 7064 6174 655f 6465 6c65 7465 2069  _update_delete i
+00000e20: 6d70 6f72 7420 280a 2020 2020 5369 6d70  mport (.    Simp
+00000e30: 6c65 5570 6461 7465 4465 6c65 7465 5465  leUpdateDeleteTe
+00000e40: 7374 2061 7320 5f53 696d 706c 6555 7064  st as _SimpleUpd
+00000e50: 6174 6544 656c 6574 6554 6573 742c 0a29  ateDeleteTest,.)
+00000e60: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
+00000e70: 2e74 6573 7469 6e67 2e73 7569 7465 2e74  .testing.suite.t
+00000e80: 6573 745f 6469 616c 6563 7420 696d 706f  est_dialect impo
+00000e90: 7274 2028 0a20 2020 2044 6966 6669 6375  rt (.    Difficu
+00000ea0: 6c74 5061 7261 6d65 7465 7273 5465 7374  ltParametersTest
+00000eb0: 2061 7320 5f44 6966 6669 6375 6c74 5061   as _DifficultPa
+00000ec0: 7261 6d65 7465 7273 5465 7374 2c0a 2020  rametersTest,.  
+00000ed0: 2020 4573 6361 7069 6e67 5465 7374 2061    EscapingTest a
+00000ee0: 7320 5f45 7363 6170 696e 6754 6573 742c  s _EscapingTest,
+00000ef0: 0a20 2020 2052 6574 7572 6e69 6e67 4775  .    ReturningGu
+00000f00: 6172 6473 5465 7374 2061 7320 5f52 6574  ardsTest as _Ret
+00000f10: 7572 6e69 6e67 4775 6172 6473 5465 7374  urningGuardsTest
+00000f20: 2c0a 290a 6672 6f6d 2073 716c 616c 6368  ,.).from sqlalch
+00000f30: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
+00000f40: 652e 7465 7374 5f69 6e73 6572 7420 696d  e.test_insert im
+00000f50: 706f 7274 2028 0a20 2020 2049 6e73 6572  port (.    Inser
+00000f60: 7442 6568 6176 696f 7254 6573 7420 6173  tBehaviorTest as
+00000f70: 205f 496e 7365 7274 4265 6861 7669 6f72   _InsertBehavior
+00000f80: 5465 7374 2c0a 290a 6672 6f6d 2073 716c  Test,.).from sql
+00000f90: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
+00000fa0: 7375 6974 652e 7465 7374 5f73 656c 6563  suite.test_selec
+00000fb0: 7420 696d 706f 7274 2028 2020 2320 6e6f  t import (  # no
+00000fc0: 7161 3a20 4634 3031 2c20 4634 3033 0a20  qa: F401, F403. 
+00000fd0: 2020 2043 6f6d 706f 756e 6453 656c 6563     CompoundSelec
+00000fe0: 7454 6573 7420 6173 205f 436f 6d70 6f75  tTest as _Compou
+00000ff0: 6e64 5365 6c65 6374 5465 7374 2c0a 2020  ndSelectTest,.  
+00001000: 2020 4578 6973 7473 5465 7374 2061 7320    ExistsTest as 
+00001010: 5f45 7869 7374 7354 6573 742c 0a20 2020  _ExistsTest,.   
+00001020: 2046 6574 6368 4c69 6d69 744f 6666 7365   FetchLimitOffse
+00001030: 7454 6573 7420 6173 205f 4665 7463 684c  tTest as _FetchL
+00001040: 696d 6974 4f66 6673 6574 5465 7374 2c0a  imitOffsetTest,.
+00001050: 2020 2020 4964 656e 7469 7479 4175 746f      IdentityAuto
+00001060: 696e 6372 656d 656e 7454 6573 7420 6173  incrementTest as
+00001070: 205f 4964 656e 7469 7479 4175 746f 696e   _IdentityAutoin
+00001080: 6372 656d 656e 7454 6573 742c 0a20 2020  crementTest,.   
+00001090: 2049 734f 7249 734e 6f74 4469 7374 696e   IsOrIsNotDistin
+000010a0: 6374 4672 6f6d 5465 7374 2061 7320 5f49  ctFromTest as _I
+000010b0: 734f 7249 734e 6f74 4469 7374 696e 6374  sOrIsNotDistinct
+000010c0: 4672 6f6d 5465 7374 2c0a 2020 2020 4c69  FromTest,.    Li
+000010d0: 6b65 4675 6e63 7469 6f6e 7354 6573 7420  keFunctionsTest 
+000010e0: 6173 205f 4c69 6b65 4675 6e63 7469 6f6e  as _LikeFunction
+000010f0: 7354 6573 742c 0a20 2020 204f 7264 6572  sTest,.    Order
+00001100: 4279 4c61 6265 6c54 6573 7420 6173 205f  ByLabelTest as _
+00001110: 4f72 6465 7242 794c 6162 656c 5465 7374  OrderByLabelTest
+00001120: 2c0a 2020 2020 506f 7374 436f 6d70 696c  ,.    PostCompil
+00001130: 6550 6172 616d 7354 6573 7420 6173 205f  eParamsTest as _
+00001140: 506f 7374 436f 6d70 696c 6550 6172 616d  PostCompileParam
+00001150: 7354 6573 742c 0a20 2020 2053 616d 654e  sTest,.    SameN
+00001160: 616d 6564 5363 6865 6d61 5461 626c 6554  amedSchemaTableT
+00001170: 6573 7420 6173 205f 5361 6d65 4e61 6d65  est as _SameName
+00001180: 6453 6368 656d 6154 6162 6c65 5465 7374  dSchemaTableTest
+00001190: 2c0a 290a 6672 6f6d 2073 716c 616c 6368  ,.).from sqlalch
+000011a0: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
+000011b0: 652e 7465 7374 5f72 6566 6c65 6374 696f  e.test_reflectio
+000011c0: 6e20 696d 706f 7274 2028 2020 2320 6e6f  n import (  # no
+000011d0: 7161 3a20 4634 3031 2c20 4634 3033 0a20  qa: F401, F403. 
+000011e0: 2020 2043 6f6d 706f 6e65 6e74 5265 666c     ComponentRefl
+000011f0: 6563 7469 6f6e 5465 7374 4578 7472 6120  ectionTestExtra 
+00001200: 6173 205f 436f 6d70 6f6e 656e 7452 6566  as _ComponentRef
+00001210: 6c65 6374 696f 6e54 6573 7445 7874 7261  lectionTestExtra
+00001220: 2c0a 2020 2020 5175 6f74 6564 4e61 6d65  ,.    QuotedName
+00001230: 4172 6775 6d65 6e74 5465 7374 2061 7320  ArgumentTest as 
+00001240: 5f51 756f 7465 644e 616d 6541 7267 756d  _QuotedNameArgum
+00001250: 656e 7454 6573 742c 0a20 2020 2043 6f6d  entTest,.    Com
+00001260: 706f 6e65 6e74 5265 666c 6563 7469 6f6e  ponentReflection
+00001270: 5465 7374 2061 7320 5f43 6f6d 706f 6e65  Test as _Compone
+00001280: 6e74 5265 666c 6563 7469 6f6e 5465 7374  ntReflectionTest
+00001290: 2c0a 2020 2020 436f 6d70 6f73 6974 654b  ,.    CompositeK
+000012a0: 6579 5265 666c 6563 7469 6f6e 5465 7374  eyReflectionTest
+000012b0: 2061 7320 5f43 6f6d 706f 7369 7465 4b65   as _CompositeKe
+000012c0: 7952 6566 6c65 6374 696f 6e54 6573 742c  yReflectionTest,
+000012d0: 0a20 2020 2043 6f6d 7075 7465 6452 6566  .    ComputedRef
+000012e0: 6c65 6374 696f 6e54 6573 7420 6173 205f  lectionTest as _
+000012f0: 436f 6d70 7574 6564 5265 666c 6563 7469  ComputedReflecti
+00001300: 6f6e 5465 7374 2c0a 2020 2020 4861 7349  onTest,.    HasI
+00001310: 6e64 6578 5465 7374 2061 7320 5f48 6173  ndexTest as _Has
+00001320: 496e 6465 7854 6573 742c 0a20 2020 2048  IndexTest,.    H
+00001330: 6173 5461 626c 6554 6573 7420 6173 205f  asTableTest as _
+00001340: 4861 7354 6162 6c65 5465 7374 2c0a 290a  HasTableTest,.).
+00001350: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00001360: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
+00001370: 7374 5f72 6573 756c 7473 2069 6d70 6f72  st_results impor
+00001380: 7420 280a 2020 2020 526f 7746 6574 6368  t (.    RowFetch
+00001390: 5465 7374 2061 7320 5f52 6f77 4665 7463  Test as _RowFetc
+000013a0: 6854 6573 742c 0a29 0a66 726f 6d20 7371  hTest,.).from sq
+000013b0: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+000013c0: 2e73 7569 7465 2e74 6573 745f 7479 7065  .suite.test_type
+000013d0: 7320 696d 706f 7274 2028 2020 2320 6e6f  s import (  # no
+000013e0: 7161 3a20 4634 3031 2c20 4634 3033 0a20  qa: F401, F403. 
+000013f0: 2020 2042 6f6f 6c65 616e 5465 7374 2061     BooleanTest a
+00001400: 7320 5f42 6f6f 6c65 616e 5465 7374 2c0a  s _BooleanTest,.
+00001410: 2020 2020 4461 7465 5465 7374 2061 7320      DateTest as 
+00001420: 5f44 6174 6554 6573 742c 0a20 2020 205f  _DateTest,.    _
+00001430: 4461 7465 4669 7874 7572 6520 6173 205f  DateFixture as _
+00001440: 5f44 6174 6546 6978 7475 7265 2c0a 2020  _DateFixture,.  
+00001450: 2020 4461 7465 5469 6d65 4869 7374 6f72    DateTimeHistor
+00001460: 6963 5465 7374 2c0a 2020 2020 4461 7465  icTest,.    Date
+00001470: 5469 6d65 436f 6572 6365 6454 6f44 6174  TimeCoercedToDat
+00001480: 6554 696d 6554 6573 7420 6173 205f 4461  eTimeTest as _Da
+00001490: 7465 5469 6d65 436f 6572 6365 6454 6f44  teTimeCoercedToD
+000014a0: 6174 6554 696d 6554 6573 742c 0a20 2020  ateTimeTest,.   
+000014b0: 2044 6174 6554 696d 654d 6963 726f 7365   DateTimeMicrose
+000014c0: 636f 6e64 7354 6573 7420 6173 205f 4461  condsTest as _Da
+000014d0: 7465 5469 6d65 4d69 6372 6f73 6563 6f6e  teTimeMicrosecon
+000014e0: 6473 5465 7374 2c0a 2020 2020 4461 7465  dsTest,.    Date
+000014f0: 5469 6d65 5465 7374 2061 7320 5f44 6174  TimeTest as _Dat
+00001500: 6554 696d 6554 6573 742c 0a20 2020 2049  eTimeTest,.    I
+00001510: 6e74 6567 6572 5465 7374 2061 7320 5f49  ntegerTest as _I
+00001520: 6e74 6567 6572 5465 7374 2c0a 2020 2020  ntegerTest,.    
+00001530: 4a53 4f4e 5465 7374 2061 7320 5f4a 534f  JSONTest as _JSO
+00001540: 4e54 6573 742c 0a20 2020 205f 4c69 7465  NTest,.    _Lite
+00001550: 7261 6c52 6f75 6e64 5472 6970 4669 7874  ralRoundTripFixt
+00001560: 7572 652c 0a20 2020 204e 756d 6572 6963  ure,.    Numeric
+00001570: 5465 7374 2061 7320 5f4e 756d 6572 6963  Test as _Numeric
+00001580: 5465 7374 2c0a 2020 2020 5374 7269 6e67  Test,.    String
+00001590: 5465 7374 2061 7320 5f53 7472 696e 6754  Test as _StringT
+000015a0: 6573 742c 0a20 2020 2054 6578 7454 6573  est,.    TextTes
+000015b0: 7420 6173 205f 5465 7874 5465 7374 2c0a  t as _TextTest,.
+000015c0: 2020 2020 5469 6d65 5465 7374 2061 7320      TimeTest as 
+000015d0: 5f54 696d 6554 6573 742c 0a20 2020 2054  _TimeTest,.    T
+000015e0: 696d 654d 6963 726f 7365 636f 6e64 7354  imeMicrosecondsT
+000015f0: 6573 7420 6173 205f 5469 6d65 4d69 6372  est as _TimeMicr
+00001600: 6f73 6563 6f6e 6473 5465 7374 2c0a 2020  osecondsTest,.  
+00001610: 2020 5469 6d65 7374 616d 704d 6963 726f    TimestampMicro
+00001620: 7365 636f 6e64 7354 6573 742c 0a20 2020  secondsTest,.   
+00001630: 2055 6e69 636f 6465 5661 7263 6861 7254   UnicodeVarcharT
+00001640: 6573 7420 6173 205f 556e 6963 6f64 6556  est as _UnicodeV
+00001650: 6172 6368 6172 5465 7374 2c0a 2020 2020  archarTest,.    
+00001660: 556e 6963 6f64 6554 6578 7454 6573 7420  UnicodeTextTest 
+00001670: 6173 205f 556e 6963 6f64 6554 6578 7454  as _UnicodeTextT
+00001680: 6573 742c 0a20 2020 205f 556e 6963 6f64  est,.    _Unicod
+00001690: 6546 6978 7475 7265 2061 7320 5f5f 556e  eFixture as __Un
+000016a0: 6963 6f64 6546 6978 7475 7265 2c0a 2920  icodeFixture,.) 
+000016b0: 2023 206e 6f71 613a 2046 3430 312c 2046   # noqa: F401, F
+000016c0: 3430 330a 6672 6f6d 2074 6573 742e 5f68  403.from test._h
+000016d0: 656c 7065 7273 2069 6d70 6f72 7420 6765  elpers import ge
+000016e0: 745f 6462 5f75 726c 2c20 6765 745f 7072  t_db_url, get_pr
+000016f0: 6f6a 6563 740a 0a63 6f6e 6669 672e 7465  oject..config.te
+00001700: 7374 5f73 6368 656d 6120 3d20 2222 0a0a  st_schema = ""..
+00001710: 0a63 6c61 7373 2042 6f6f 6c65 616e 5465  .class BooleanTe
+00001720: 7374 285f 426f 6f6c 6561 6e54 6573 7429  st(_BooleanTest)
+00001730: 3a0a 2020 2020 4070 7974 6573 742e 6d61  :.    @pytest.ma
+00001740: 726b 2e73 6b69 7028 0a20 2020 2020 2020  rk.skip(.       
+00001750: 2022 5468 6520 6f72 6967 696e 616c 2074   "The original t
+00001760: 6573 7420 6361 7365 2077 6173 2073 706c  est case was spl
+00001770: 6974 2069 6e74 6f20 3220 7061 7274 733a  it into 2 parts:
+00001780: 2022 0a20 2020 2020 2020 2022 7465 7374   ".        "test
+00001790: 5f72 656e 6465 725f 6c69 7465 7261 6c5f  _render_literal_
+000017a0: 626f 6f6c 5f74 7275 6520 616e 6420 7465  bool_true and te
+000017b0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
+000017c0: 6c5f 626f 6f6c 5f66 616c 7365 220a 2020  l_bool_false".  
+000017d0: 2020 290a 2020 2020 6465 6620 7465 7374    ).    def test
+000017e0: 5f72 656e 6465 725f 6c69 7465 7261 6c5f  _render_literal_
+000017f0: 626f 6f6c 2873 656c 6629 3a0a 2020 2020  bool(self):.    
+00001800: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00001810: 6620 7465 7374 5f72 656e 6465 725f 6c69  f test_render_li
+00001820: 7465 7261 6c5f 626f 6f6c 5f74 7275 6528  teral_bool_true(
+00001830: 7365 6c66 2c20 6c69 7465 7261 6c5f 726f  self, literal_ro
+00001840: 756e 645f 7472 6970 293a 0a20 2020 2020  und_trip):.     
+00001850: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00001860: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
+00001870: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
+00001880: 5370 616e 6e65 7220 7375 7070 6f72 7473  Spanner supports
+00001890: 2074 6162 6c65 7320 7769 7468 2061 6e20   tables with an 
+000018a0: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
+000018b0: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
+000018c0: 6e6c 7920 6120 7369 6e67 6c65 2072 6f77  nly a single row
+000018d0: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
+000018e0: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
+000018f0: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
+00001900: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
+00001910: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
+00001920: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
+00001930: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
+00001940: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
+00001950: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
+00001960: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
+00001970: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001980: 2020 2020 206c 6974 6572 616c 5f72 6f75       literal_rou
+00001990: 6e64 5f74 7269 7028 426f 6f6c 6561 6e28  nd_trip(Boolean(
+000019a0: 292c 205b 5472 7565 5d2c 205b 5472 7565  ), [True], [True
+000019b0: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+000019c0: 5f72 656e 6465 725f 6c69 7465 7261 6c5f  _render_literal_
+000019d0: 626f 6f6c 5f66 616c 7365 2873 656c 662c  bool_false(self,
+000019e0: 206c 6974 6572 616c 5f72 6f75 6e64 5f74   literal_round_t
+000019f0: 7269 7029 3a0a 2020 2020 2020 2020 2222  rip):.        ""
+00001a00: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
+00001a10: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
+00001a20: 2020 2020 2043 6c6f 7564 2053 7061 6e6e       Cloud Spann
+00001a30: 6572 2073 7570 706f 7274 7320 7461 626c  er supports tabl
+00001a40: 6573 2077 6974 6820 616e 2065 6d70 7479  es with an empty
+00001a50: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
+00001a60: 740a 2020 2020 2020 2020 6f6e 6c79 2061  t.        only a
+00001a70: 2073 696e 676c 6520 726f 7720 6361 6e20   single row can 
+00001a80: 6265 2069 6e73 6572 7465 6420 696e 746f  be inserted into
+00001a90: 2073 7563 6820 6120 7461 626c 6520 2d0a   such a table -.
+00001aa0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
+00001ab0: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
+00001ac0: 6c20 6661 696c 2077 6974 6820 6052 6f77  l fail with `Row
+00001ad0: 205b 5d20 616c 7265 6164 7920 6578 6973   [] already exis
+00001ae0: 7473 222e 0a20 2020 2020 2020 204f 7665  ts"..        Ove
+00001af0: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
+00001b00: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
+00001b10: 6d65 2066 6169 6c75 7265 2e0a 2020 2020  me failure..    
+00001b20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001b30: 6c69 7465 7261 6c5f 726f 756e 645f 7472  literal_round_tr
+00001b40: 6970 2842 6f6f 6c65 616e 2829 2c20 5b46  ip(Boolean(), [F
+00001b50: 616c 7365 5d2c 205b 4661 6c73 655d 290a  alse], [False]).
+00001b60: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00001b70: 6b2e 736b 6970 2822 4e6f 7420 7375 7070  k.skip("Not supp
+00001b80: 6f72 7465 6420 6279 2043 6c6f 7564 2053  orted by Cloud S
+00001b90: 7061 6e6e 6572 2229 0a20 2020 2064 6566  panner").    def
+00001ba0: 2074 6573 745f 7768 6572 6563 6c61 7573   test_whereclaus
+00001bb0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00001bc0: 2070 6173 730a 0a0a 636c 6173 7320 436f   pass...class Co
+00001bd0: 6d70 6f6e 656e 7452 6566 6c65 6374 696f  mponentReflectio
+00001be0: 6e54 6573 7445 7874 7261 285f 436f 6d70  nTestExtra(_Comp
+00001bf0: 6f6e 656e 7452 6566 6c65 6374 696f 6e54  onentReflectionT
+00001c00: 6573 7445 7874 7261 293a 0a20 2020 2040  estExtra):.    @
+00001c10: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
+00001c20: 2e74 6162 6c65 5f72 6566 6c65 6374 696f  .table_reflectio
+00001c30: 6e0a 2020 2020 6465 6620 7465 7374 5f6e  n.    def test_n
+00001c40: 756c 6c61 626c 655f 7265 666c 6563 7469  ullable_reflecti
+00001c50: 6f6e 2873 656c 662c 2063 6f6e 6e65 6374  on(self, connect
+00001c60: 696f 6e2c 206d 6574 6164 6174 6129 3a0a  ion, metadata):.
+00001c70: 2020 2020 2020 2020 7420 3d20 5461 626c          t = Tabl
+00001c80: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
+00001c90: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00001ca0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00001cb0: 2020 2020 2020 436f 6c75 6d6e 2822 6122        Column("a"
+00001cc0: 2c20 496e 7465 6765 722c 206e 756c 6c61  , Integer, nulla
+00001cd0: 626c 653d 5472 7565 292c 0a20 2020 2020  ble=True),.     
+00001ce0: 2020 2020 2020 2043 6f6c 756d 6e28 2262         Column("b
+00001cf0: 222c 2049 6e74 6567 6572 2c20 6e75 6c6c  ", Integer, null
+00001d00: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
+00001d10: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
+00001d20: 2e63 7265 6174 6528 636f 6e6e 6563 7469  .create(connecti
+00001d30: 6f6e 290a 2020 2020 2020 2020 636f 6e6e  on).        conn
+00001d40: 6563 7469 6f6e 2e63 6f6e 6e65 6374 696f  ection.connectio
+00001d50: 6e2e 636f 6d6d 6974 2829 0a20 2020 2020  n.commit().     
+00001d60: 2020 2065 715f 280a 2020 2020 2020 2020     eq_(.        
+00001d70: 2020 2020 6469 6374 280a 2020 2020 2020      dict(.      
+00001d80: 2020 2020 2020 2020 2020 2863 6f6c 5b22            (col["
+00001d90: 6e61 6d65 225d 2c20 636f 6c5b 226e 756c  name"], col["nul
+00001da0: 6c61 626c 6522 5d29 0a20 2020 2020 2020  lable"]).       
+00001db0: 2020 2020 2020 2020 2066 6f72 2063 6f6c           for col
+00001dc0: 2069 6e20 696e 7370 6563 7428 636f 6e6e   in inspect(conn
+00001dd0: 6563 7469 6f6e 292e 6765 745f 636f 6c75  ection).get_colu
+00001de0: 6d6e 7328 2274 2229 0a20 2020 2020 2020  mns("t").       
+00001df0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00001e00: 2020 2020 7b22 6122 3a20 5472 7565 2c20      {"a": True, 
+00001e10: 2262 223a 2046 616c 7365 7d2c 0a20 2020  "b": False},.   
+00001e20: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00001e30: 5f74 7970 655f 726f 756e 645f 7472 6970  _type_round_trip
+00001e40: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+00001e50: 6e2c 206d 6574 6164 6174 612c 202a 7479  n, metadata, *ty
+00001e60: 7065 7329 3a0a 2020 2020 2020 2020 7420  pes):.        t 
+00001e70: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
+00001e80: 2020 2020 2022 7422 2c20 6d65 7461 6461       "t", metada
+00001e90: 7461 2c20 2a5b 436f 6c75 6d6e 2822 7425  ta, *[Column("t%
+00001ea0: 6422 2025 2069 2c20 7479 7065 5f29 2066  d" % i, type_) f
+00001eb0: 6f72 2069 2c20 7479 7065 5f20 696e 2065  or i, type_ in e
+00001ec0: 6e75 6d65 7261 7465 2874 7970 6573 295d  numerate(types)]
+00001ed0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00001ee0: 2020 2074 2e63 7265 6174 6528 636f 6e6e     t.create(conn
+00001ef0: 6563 7469 6f6e 290a 2020 2020 2020 2020  ection).        
+00001f00: 636f 6e6e 6563 7469 6f6e 2e63 6f6e 6e65  connection.conne
+00001f10: 6374 696f 6e2e 636f 6d6d 6974 2829 0a0a  ction.commit()..
+00001f20: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+00001f30: 635b 2274 7970 6522 5d20 666f 7220 6320  c["type"] for c 
+00001f40: 696e 2069 6e73 7065 6374 2863 6f6e 6e65  in inspect(conne
+00001f50: 6374 696f 6e29 2e67 6574 5f63 6f6c 756d  ction).get_colum
+00001f60: 6e73 2822 7422 295d 0a0a 2020 2020 4074  ns("t")]..    @t
+00001f70: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00001f80: 7461 626c 655f 7265 666c 6563 7469 6f6e  table_reflection
+00001f90: 0a20 2020 2064 6566 2074 6573 745f 6e75  .    def test_nu
+00001fa0: 6d65 7269 635f 7265 666c 6563 7469 6f6e  meric_reflection
+00001fb0: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+00001fc0: 6e2c 206d 6574 6164 6174 6129 3a0a 2020  n, metadata):.  
+00001fd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00001fe0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+00001ff0: 4445 3a0a 0a20 2020 2020 2020 2053 7061  DE:..        Spa
+00002000: 6e6e 6572 2064 6566 696e 6573 204e 554d  nner defines NUM
+00002010: 4552 4943 2074 7970 6520 7769 7468 2074  ERIC type with t
+00002020: 6865 2063 6f6e 7374 616e 7420 7072 6563  he constant prec
+00002030: 6973 696f 6e3d 3338 0a20 2020 2020 2020  ision=38.       
+00002040: 2061 6e64 2073 6361 6c65 3d39 2e20 4f76   and scale=9. Ov
+00002050: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
+00002060: 7420 746f 2063 6865 636b 2069 6620 7468  t to check if th
+00002070: 6520 4e55 4d45 5249 430a 2020 2020 2020  e NUMERIC.      
+00002080: 2020 636f 6c75 6d6e 2069 7320 7375 6363    column is succ
+00002090: 6573 7366 756c 6c79 2063 7265 6174 6564  essfully created
+000020a0: 2061 6e64 2068 6173 2064 696d 656e 7369   and has dimensi
+000020b0: 6f6e 730a 2020 2020 2020 2020 636f 7272  ons.        corr
+000020c0: 6563 7420 666f 7220 436c 6f75 6420 5370  ect for Cloud Sp
+000020d0: 616e 6e65 722e 0a20 2020 2020 2020 2022  anner..        "
+000020e0: 2222 0a20 2020 2020 2020 2066 6f72 2074  "".        for t
+000020f0: 7970 2069 6e20 7365 6c66 2e5f 7479 7065  yp in self._type
+00002100: 5f72 6f75 6e64 5f74 7269 7028 636f 6e6e  _round_trip(conn
+00002110: 6563 7469 6f6e 2c20 6d65 7461 6461 7461  ection, metadata
+00002120: 2c20 4e75 6d65 7269 6328 3138 2c20 3529  , Numeric(18, 5)
+00002130: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+00002140: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00002150: 2874 7970 2c20 4e75 6d65 7269 6329 0a20  (typ, Numeric). 
+00002160: 2020 2020 2020 2020 2020 2065 715f 2874             eq_(t
+00002170: 7970 2e70 7265 6369 7369 6f6e 2c20 3338  yp.precision, 38
+00002180: 290a 2020 2020 2020 2020 2020 2020 6571  ).            eq
+00002190: 5f28 7479 702e 7363 616c 652c 2039 290a  _(typ.scale, 9).
+000021a0: 0a20 2020 2040 7465 7374 696e 672e 7265  .    @testing.re
+000021b0: 7175 6972 6573 2e74 6162 6c65 5f72 6566  quires.table_ref
+000021c0: 6c65 6374 696f 6e0a 2020 2020 6465 6620  lection.    def 
+000021d0: 7465 7374 5f62 696e 6172 795f 7265 666c  test_binary_refl
+000021e0: 6563 7469 6f6e 2873 656c 662c 2063 6f6e  ection(self, con
+000021f0: 6e65 6374 696f 6e2c 206d 6574 6164 6174  nection, metadat
+00002200: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
+00002210: 2020 2020 2020 2020 4368 6563 6b20 7468          Check th
+00002220: 6174 2061 2042 5954 4553 2063 6f6c 756d  at a BYTES colum
+00002230: 6e20 7769 7468 2061 6e20 6578 706c 6963  n with an explic
+00002240: 6974 6c79 0a20 2020 2020 2020 2073 6574  itly.        set
+00002250: 2073 697a 6520 6973 2063 6f72 7265 6374   size is correct
+00002260: 6c79 2072 6566 6c65 6374 6564 2e0a 2020  ly reflected..  
+00002270: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00002280: 2020 666f 7220 7479 7020 696e 2073 656c    for typ in sel
+00002290: 662e 5f74 7970 655f 726f 756e 645f 7472  f._type_round_tr
+000022a0: 6970 2863 6f6e 6e65 6374 696f 6e2c 206d  ip(connection, m
+000022b0: 6574 6164 6174 612c 204c 6172 6765 4269  etadata, LargeBi
+000022c0: 6e61 7279 2832 3029 293a 0a20 2020 2020  nary(20)):.     
+000022d0: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
+000022e0: 696e 7374 616e 6365 2874 7970 2c20 4c61  instance(typ, La
+000022f0: 7267 6542 696e 6172 7929 0a20 2020 2020  rgeBinary).     
+00002300: 2020 2020 2020 2065 715f 2874 7970 2e6c         eq_(typ.l
+00002310: 656e 6774 682c 2032 3029 0a0a 0a63 6c61  ength, 20)...cla
+00002320: 7373 2043 6f6d 7075 7465 6452 6566 6c65  ss ComputedRefle
+00002330: 6374 696f 6e46 6978 7475 7265 5465 7374  ctionFixtureTest
+00002340: 285f 436f 6d70 7574 6564 5265 666c 6563  (_ComputedReflec
+00002350: 7469 6f6e 4669 7874 7572 6554 6573 7429  tionFixtureTest)
+00002360: 3a0a 2020 2020 4063 6c61 7373 6d65 7468  :.    @classmeth
+00002370: 6f64 0a20 2020 2064 6566 2064 6566 696e  od.    def defin
+00002380: 655f 7461 626c 6573 2863 6c73 2c20 6d65  e_tables(cls, me
+00002390: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
+000023a0: 2022 2222 5350 414e 4e45 5220 4f56 4552   """SPANNER OVER
+000023b0: 5249 4445 3a0a 0a20 2020 2020 2020 2041  RIDE:..        A
+000023c0: 766f 6964 2075 7369 6e67 2064 6566 6175  void using defau
+000023d0: 6c74 2076 616c 7565 7320 666f 7220 636f  lt values for co
+000023e0: 6d70 7574 6564 2063 6f6c 756d 6e73 2e0a  mputed columns..
+000023f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002400: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
+00002410: 2020 2020 2020 2022 636f 6d70 7574 6564         "computed
+00002420: 5f64 6566 6175 6c74 5f74 6162 6c65 222c  _default_table",
+00002430: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00002440: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
+00002450: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
+00002460: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
+00002470: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
+00002480: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00002490: 6e6f 726d 616c 222c 2049 6e74 6567 6572  normal", Integer
+000024a0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+000024b0: 6f6c 756d 6e28 2263 6f6d 7075 7465 645f  olumn("computed_
+000024c0: 636f 6c22 2c20 496e 7465 6765 722c 2043  col", Integer, C
+000024d0: 6f6d 7075 7465 6428 226e 6f72 6d61 6c20  omputed("normal 
+000024e0: 2b20 3432 2229 292c 0a20 2020 2020 2020  + 42")),.       
+000024f0: 2020 2020 2043 6f6c 756d 6e28 2277 6974       Column("wit
+00002500: 685f 6465 6661 756c 7422 2c20 496e 7465  h_default", Inte
+00002510: 6765 7229 2c0a 2020 2020 2020 2020 290a  ger),.        ).
+00002520: 0a20 2020 2020 2020 2074 203d 2054 6162  .        t = Tab
+00002530: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00002540: 2263 6f6d 7075 7465 645f 636f 6c75 6d6e  "computed_column
+00002550: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+00002560: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00002570: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00002580: 6e28 2269 6422 2c20 496e 7465 6765 722c  n("id", Integer,
+00002590: 2070 7269 6d61 7279 5f6b 6579 3d54 7275   primary_key=Tru
+000025a0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+000025b0: 436f 6c75 6d6e 2822 6e6f 726d 616c 222c  Column("normal",
+000025c0: 2049 6e74 6567 6572 292c 0a20 2020 2020   Integer),.     
+000025d0: 2020 2020 2020 2043 6f6c 756d 6e28 2263         Column("c
+000025e0: 6f6d 7075 7465 645f 6e6f 5f66 6c61 6722  omputed_no_flag"
+000025f0: 2c20 496e 7465 6765 722c 2043 6f6d 7075  , Integer, Compu
+00002600: 7465 6428 226e 6f72 6d61 6c20 2b20 3432  ted("normal + 42
+00002610: 2229 292c 0a20 2020 2020 2020 2029 0a0a  ")),.        )..
+00002620: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
+00002630: 6e67 2e72 6571 7569 7265 732e 636f 6d70  ng.requires.comp
+00002640: 7574 6564 5f63 6f6c 756d 6e73 5f76 6972  uted_columns_vir
+00002650: 7475 616c 2e65 6e61 626c 6564 3a0a 2020  tual.enabled:.  
+00002660: 2020 2020 2020 2020 2020 742e 6170 7065            t.appe
+00002670: 6e64 5f63 6f6c 756d 6e28 0a20 2020 2020  nd_column(.     
+00002680: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00002690: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+000026a0: 2020 2020 2020 2022 636f 6d70 7574 6564         "computed
+000026b0: 5f76 6972 7475 616c 222c 0a20 2020 2020  _virtual",.     
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+000026d0: 6e74 6567 6572 2c0a 2020 2020 2020 2020  nteger,.        
+000026e0: 2020 2020 2020 2020 2020 2020 436f 6d70              Comp
+000026f0: 7574 6564 2822 6e6f 726d 616c 202b 2032  uted("normal + 2
+00002700: 222c 2070 6572 7369 7374 6564 3d46 616c  ", persisted=Fal
+00002710: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
+00002720: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00002730: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00002740: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
+00002750: 2e63 6f6d 7075 7465 645f 636f 6c75 6d6e  .computed_column
+00002760: 735f 7374 6f72 6564 2e65 6e61 626c 6564  s_stored.enabled
+00002770: 3a0a 2020 2020 2020 2020 2020 2020 742e  :.            t.
+00002780: 6170 7065 6e64 5f63 6f6c 756d 6e28 0a20  append_column(. 
+00002790: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+000027a0: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
+000027b0: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
+000027c0: 7574 6564 5f73 746f 7265 6422 2c0a 2020  uted_stored",.  
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 2020 496e 7465 6765 722c 0a20 2020 2020    Integer,.     
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00002800: 6f6d 7075 7465 6428 226e 6f72 6d61 6c20  omputed("normal 
+00002810: 2d20 3432 222c 2070 6572 7369 7374 6564  - 42", persisted
+00002820: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00002830: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00002840: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+00002850: 436f 6d70 7574 6564 5265 666c 6563 7469  ComputedReflecti
+00002860: 6f6e 5465 7374 285f 436f 6d70 7574 6564  onTest(_Computed
+00002870: 5265 666c 6563 7469 6f6e 5465 7374 2c20  ReflectionTest, 
+00002880: 436f 6d70 7574 6564 5265 666c 6563 7469  ComputedReflecti
+00002890: 6f6e 4669 7874 7572 6554 6573 7429 3a0a  onFixtureTest):.
+000028a0: 2020 2020 4074 6573 7469 6e67 2e72 6571      @testing.req
+000028b0: 7569 7265 732e 7363 6865 6d61 730a 2020  uires.schemas.  
+000028c0: 2020 6465 6620 7465 7374 5f67 6574 5f63    def test_get_c
+000028d0: 6f6c 756d 6e5f 7265 7475 726e 735f 7065  olumn_returns_pe
+000028e0: 7273 6973 7465 645f 7769 7468 5f73 6368  rsisted_with_sch
+000028f0: 656d 6128 7365 6c66 293a 0a20 2020 2020  ema(self):.     
+00002900: 2020 2069 6e73 7020 3d20 696e 7370 6563     insp = inspec
+00002910: 7428 636f 6e66 6967 2e64 6229 0a0a 2020  t(config.db)..  
+00002920: 2020 2020 2020 636f 6c73 203d 2069 6e73        cols = ins
+00002930: 702e 6765 745f 636f 6c75 6d6e 7328 2263  p.get_columns("c
+00002940: 6f6d 7075 7465 645f 636f 6c75 6d6e 5f74  omputed_column_t
+00002950: 6162 6c65 222c 2073 6368 656d 613d 636f  able", schema=co
+00002960: 6e66 6967 2e74 6573 745f 7363 6865 6d61  nfig.test_schema
+00002970: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+00002980: 207b 635b 226e 616d 6522 5d3a 2063 2066   {c["name"]: c f
+00002990: 6f72 2063 2069 6e20 636f 6c73 7d0a 0a20  or c in cols}.. 
+000029a0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+000029b0: 6b5f 636f 6c75 6d6e 280a 2020 2020 2020  k_column(.      
+000029c0: 2020 2020 2020 6461 7461 2c0a 2020 2020        data,.    
+000029d0: 2020 2020 2020 2020 2263 6f6d 7075 7465          "compute
+000029e0: 645f 6e6f 5f66 6c61 6722 2c0a 2020 2020  d_no_flag",.    
+000029f0: 2020 2020 2020 2020 226e 6f72 6d61 6c2b          "normal+
+00002a00: 3432 222c 0a20 2020 2020 2020 2020 2020  42",.           
+00002a10: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
+00002a20: 732e 636f 6d70 7574 6564 5f63 6f6c 756d  s.computed_colum
+00002a30: 6e73 5f64 6566 6175 6c74 5f70 6572 7369  ns_default_persi
+00002a40: 7374 6564 2e65 6e61 626c 6564 2c0a 2020  sted.enabled,.  
+00002a50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002a60: 6966 2074 6573 7469 6e67 2e72 6571 7569  if testing.requi
+00002a70: 7265 732e 636f 6d70 7574 6564 5f63 6f6c  res.computed_col
+00002a80: 756d 6e73 5f76 6972 7475 616c 2e65 6e61  umns_virtual.ena
+00002a90: 626c 6564 3a0a 2020 2020 2020 2020 2020  bled:.          
+00002aa0: 2020 7365 6c66 2e63 6865 636b 5f63 6f6c    self.check_col
+00002ab0: 756d 6e28 0a20 2020 2020 2020 2020 2020  umn(.           
+00002ac0: 2020 2020 2064 6174 612c 0a20 2020 2020       data,.     
+00002ad0: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
+00002ae0: 7574 6564 5f76 6972 7475 616c 222c 0a20  uted_virtual",. 
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002b00: 6e6f 726d 616c 2f32 222c 0a20 2020 2020  normal/2",.     
+00002b10: 2020 2020 2020 2020 2020 2046 616c 7365             False
+00002b20: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00002b30: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
+00002b40: 6e67 2e72 6571 7569 7265 732e 636f 6d70  ng.requires.comp
+00002b50: 7574 6564 5f63 6f6c 756d 6e73 5f73 746f  uted_columns_sto
+00002b60: 7265 642e 656e 6162 6c65 643a 0a20 2020  red.enabled:.   
+00002b70: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00002b80: 6563 6b5f 636f 6c75 6d6e 280a 2020 2020  eck_column(.    
+00002b90: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00002ba0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002bb0: 2020 2263 6f6d 7075 7465 645f 7374 6f72    "computed_stor
+00002bc0: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
+00002bd0: 2020 2020 2022 6e6f 726d 616c 2d34 3222       "normal-42"
+00002be0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002bf0: 2020 5472 7565 2c0a 2020 2020 2020 2020    True,.        
+00002c00: 2020 2020 290a 0a20 2020 2040 7079 7465      )..    @pyte
+00002c10: 7374 2e6d 6172 6b2e 736b 6970 2822 4465  st.mark.skip("De
+00002c20: 6661 756c 7420 7661 6c75 6573 2061 7265  fault values are
+00002c30: 206e 6f74 2073 7570 706f 7274 6564 2e22   not supported."
+00002c40: 290a 2020 2020 6465 6620 7465 7374 5f63  ).    def test_c
+00002c50: 6f6d 7075 7465 645f 636f 6c5f 6465 6661  omputed_col_defa
+00002c60: 756c 745f 6e6f 745f 7365 7428 7365 6c66  ult_not_set(self
+00002c70: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00002c80: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
+00002c90: 745f 636f 6c75 6d6e 5f72 6574 7572 6e73  t_column_returns
+00002ca0: 5f63 6f6d 7075 7465 6428 7365 6c66 293a  _computed(self):
+00002cb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002cc0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
+00002cd0: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
+00002ce0: 496e 2053 7061 6e6e 6572 2061 6c6c 2074  In Spanner all t
+00002cf0: 6865 2067 656e 6572 6174 6564 2063 6f6c  he generated col
+00002d00: 756d 6e73 2061 7265 2053 544f 5245 442c  umns are STORED,
+00002d10: 0a20 2020 2020 2020 206d 6561 6e69 6e67  .        meaning
+00002d20: 2074 6865 7265 2061 7265 206e 6f20 7065   there are no pe
+00002d30: 7273 6973 7465 6420 616e 6420 6e6f 7420  rsisted and not 
+00002d40: 7065 7273 6973 7465 640a 2020 2020 2020  persisted.      
+00002d50: 2020 2869 6e20 7468 6520 7465 726d 7320    (in the terms 
+00002d60: 6f66 2074 6865 2053 514c 416c 6368 656d  of the SQLAlchem
+00002d70: 7929 2063 6f6c 756d 6e73 2e20 5468 650a  y) columns. The.
+00002d80: 2020 2020 2020 2020 6d65 7468 6f64 206f          method o
+00002d90: 7665 7272 6964 6520 6f6d 6974 7320 7468  verride omits th
+00002da0: 6520 7065 7273 6973 7465 6e63 6520 7265  e persistence re
+00002db0: 666c 6563 7469 6f6e 2063 6865 636b 732e  flection checks.
+00002dc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002dd0: 2020 2020 2069 6e73 7020 3d20 696e 7370       insp = insp
+00002de0: 6563 7428 636f 6e66 6967 2e64 6229 0a0a  ect(config.db)..
+00002df0: 2020 2020 2020 2020 636f 6c73 203d 2069          cols = i
+00002e00: 6e73 702e 6765 745f 636f 6c75 6d6e 7328  nsp.get_columns(
+00002e10: 2263 6f6d 7075 7465 645f 6465 6661 756c  "computed_defaul
+00002e20: 745f 7461 626c 6522 290a 2020 2020 2020  t_table").      
+00002e30: 2020 6461 7461 203d 207b 635b 226e 616d    data = {c["nam
+00002e40: 6522 5d3a 2063 2066 6f72 2063 2069 6e20  e"]: c for c in 
+00002e50: 636f 6c73 7d0a 2020 2020 2020 2020 666f  cols}.        fo
+00002e60: 7220 6b65 7920 696e 2028 2269 6422 2c20  r key in ("id", 
+00002e70: 226e 6f72 6d61 6c22 2c20 2277 6974 685f  "normal", "with_
+00002e80: 6465 6661 756c 7422 293a 0a20 2020 2020  default"):.     
+00002e90: 2020 2020 2020 2069 735f 7472 7565 2822         is_true("
+00002ea0: 636f 6d70 7574 6564 2220 6e6f 7420 696e  computed" not in
+00002eb0: 2064 6174 615b 6b65 795d 290a 2020 2020   data[key]).    
+00002ec0: 2020 2020 636f 6d70 4461 7461 203d 2064      compData = d
+00002ed0: 6174 615b 2263 6f6d 7075 7465 645f 636f  ata["computed_co
+00002ee0: 6c22 5d0a 2020 2020 2020 2020 6973 5f74  l"].        is_t
+00002ef0: 7275 6528 2263 6f6d 7075 7465 6422 2069  rue("computed" i
+00002f00: 6e20 636f 6d70 4461 7461 290a 2020 2020  n compData).    
+00002f10: 2020 2020 6973 5f74 7275 6528 2273 716c      is_true("sql
+00002f20: 7465 7874 2220 696e 2063 6f6d 7044 6174  text" in compDat
+00002f30: 615b 2263 6f6d 7075 7465 6422 5d29 0a20  a["computed"]). 
+00002f40: 2020 2020 2020 2065 715f 2873 656c 662e         eq_(self.
+00002f50: 6e6f 726d 616c 697a 6528 636f 6d70 4461  normalize(compDa
+00002f60: 7461 5b22 636f 6d70 7574 6564 225d 5b22  ta["computed"]["
+00002f70: 7371 6c74 6578 7422 5d29 2c20 226e 6f72  sqltext"]), "nor
+00002f80: 6d61 6c2b 3432 2229 0a0a 2020 2020 6465  mal+42")..    de
+00002f90: 6620 7465 7374 5f63 7265 6174 655f 6e6f  f test_create_no
+00002fa0: 745f 6e75 6c6c 5f63 6f6d 7075 7465 645f  t_null_computed_
+00002fb0: 636f 6c75 6d6e 2873 656c 662c 2063 6f6e  column(self, con
+00002fc0: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+00002fd0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00002fe0: 414e 4e45 5220 5445 5354 3a0a 0a20 2020  ANNER TEST:..   
+00002ff0: 2020 2020 2043 6865 636b 2074 6861 7420       Check that 
+00003000: 6f6e 2063 7265 6174 696e 6720 6120 636f  on creating a co
+00003010: 6d70 7574 6564 2063 6f6c 756d 6e20 7769  mputed column wi
+00003020: 7468 2061 204e 4f54 204e 554c 4c0a 2020  th a NOT NULL.  
+00003030: 2020 2020 2020 636c 6175 7365 2074 6865        clause the
+00003040: 2063 6c61 7573 6520 6973 2073 6574 2069   clause is set i
+00003050: 6e20 6672 6f6e 7420 6f66 2074 6865 2063  n front of the c
+00003060: 6f6d 7075 7465 6420 636f 6c75 6d6e 0a20  omputed column. 
+00003070: 2020 2020 2020 2073 7461 7465 6d65 6e74         statement
+00003080: 2064 6566 696e 6974 696f 6e20 616e 6420   definition and 
+00003090: 646f 6573 6e27 7420 6361 7573 6520 6661  doesn't cause fa
+000030a0: 696c 7572 6573 2e0a 2020 2020 2020 2020  ilures..        
+000030b0: 2222 220a 2020 2020 2020 2020 6d65 7461  """.        meta
+000030c0: 6461 7461 203d 204d 6574 6144 6174 6128  data = MetaData(
+000030d0: 290a 0a20 2020 2020 2020 2054 6162 6c65  )..        Table
+000030e0: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
+000030f0: 696e 6765 7273 222c 0a20 2020 2020 2020  ingers",.       
+00003100: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00003110: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00003120: 6e28 2253 696e 6765 7249 6422 2c20 5374  n("SingerId", St
+00003130: 7269 6e67 2833 3629 2c20 7072 696d 6172  ring(36), primar
+00003140: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
+00003150: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
+00003160: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00003170: 2246 6972 7374 4e61 6d65 222c 2053 7472  "FirstName", Str
+00003180: 696e 6728 3230 3029 292c 0a20 2020 2020  ing(200)),.     
+00003190: 2020 2020 2020 2043 6f6c 756d 6e28 224c         Column("L
+000031a0: 6173 744e 616d 6522 2c20 5374 7269 6e67  astName", String
+000031b0: 2832 3030 292c 206e 756c 6c61 626c 653d  (200), nullable=
+000031c0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
+000031d0: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
+000031e0: 2020 2020 2020 2020 2020 2020 2246 756c              "Ful
+000031f0: 6c4e 616d 6522 2c0a 2020 2020 2020 2020  lName",.        
+00003200: 2020 2020 2020 2020 5374 7269 6e67 2834          String(4
+00003210: 3030 292c 0a20 2020 2020 2020 2020 2020  00),.           
+00003220: 2020 2020 2043 6f6d 7075 7465 6428 2243       Computed("C
+00003230: 4f41 4c45 5343 4528 4669 7273 744e 616d  OALESCE(FirstNam
+00003240: 6520 7c7c 2027 2027 2c20 2727 2920 7c7c  e || ' ', '') ||
+00003250: 204c 6173 744e 616d 6522 292c 0a20 2020   LastName"),.   
+00003260: 2020 2020 2020 2020 2020 2020 206e 756c               nul
+00003270: 6c61 626c 653d 4661 6c73 652c 0a20 2020  lable=False,.   
+00003280: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00003290: 2020 2020 290a 0a20 2020 2020 2020 206d      )..        m
+000032a0: 6574 6164 6174 612e 6372 6561 7465 5f61  etadata.create_a
+000032b0: 6c6c 2863 6f6e 6e65 6374 696f 6e29 0a0a  ll(connection)..
+000032c0: 0a63 6c61 7373 2043 6f6d 706f 6e65 6e74  .class Component
+000032d0: 5265 666c 6563 7469 6f6e 5465 7374 285f  ReflectionTest(_
+000032e0: 436f 6d70 6f6e 656e 7452 6566 6c65 6374  ComponentReflect
+000032f0: 696f 6e54 6573 7429 3a0a 2020 2020 4070  ionTest):.    @p
+00003300: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+00003310: 2253 6b69 7022 290a 2020 2020 6465 6620  "Skip").    def 
+00003320: 7465 7374 5f6e 6f74 5f65 7869 7374 696e  test_not_existin
+00003330: 675f 7461 626c 6528 7365 6c66 2c20 6d65  g_table(self, me
+00003340: 7468 6f64 2c20 636f 6e6e 6563 7469 6f6e  thod, connection
+00003350: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00003360: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00003370: 640a 2020 2020 6465 6620 6465 6669 6e65  d.    def define
+00003380: 5f74 6162 6c65 7328 636c 732c 206d 6574  _tables(cls, met
+00003390: 6164 6174 6129 3a0a 2020 2020 2020 2020  adata):.        
+000033a0: 636c 732e 6465 6669 6e65 5f72 6566 6c65  cls.define_refle
+000033b0: 6374 6564 5f74 6162 6c65 7328 6d65 7461  cted_tables(meta
+000033c0: 6461 7461 2c20 4e6f 6e65 290a 0a20 2020  data, None)..   
+000033d0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+000033e0: 2020 6465 6620 6465 6669 6e65 5f76 6965    def define_vie
+000033f0: 7773 2863 6c73 2c20 6d65 7461 6461 7461  ws(cls, metadata
+00003400: 2c20 7363 6865 6d61 293a 0a20 2020 2020  , schema):.     
+00003410: 2020 2074 6162 6c65 5f69 6e66 6f20 3d20     table_info = 
+00003420: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
+00003430: 696e 6761 6c69 6e67 7322 3a20 5b0a 2020  ingalings": [.  
+00003440: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00003450: 696e 6761 6c69 6e67 5f69 6422 2c0a 2020  ingaling_id",.  
+00003460: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00003470: 6464 7265 7373 5f69 6422 2c0a 2020 2020  ddress_id",.    
+00003480: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
+00003490: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
+000034a0: 2020 2020 2269 645f 7573 6572 222c 0a20      "id_user",. 
+000034b0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+000034c0: 2020 2020 2020 2020 2020 2275 7365 7273            "users
+000034d0: 223a 205b 2275 7365 725f 6964 222c 2022  ": ["user_id", "
+000034e0: 7465 7374 3122 2c20 2274 6573 7432 225d  test1", "test2"]
+000034f0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00003500: 6d61 696c 5f61 6464 7265 7373 6573 223a  mail_addresses":
+00003510: 205b 2261 6464 7265 7373 5f69 6422 2c20   ["address_id", 
+00003520: 2272 656d 6f74 655f 7573 6572 5f69 6422  "remote_user_id"
+00003530: 2c20 2265 6d61 696c 5f61 6464 7265 7373  , "email_address
+00003540: 225d 2c0a 2020 2020 2020 2020 7d0a 2020  "],.        }.  
+00003550: 2020 2020 2020 6966 2074 6573 7469 6e67        if testing
+00003560: 2e72 6571 7569 7265 732e 7365 6c66 5f72  .requires.self_r
+00003570: 6566 6572 656e 7469 616c 5f66 6f72 6569  eferential_forei
+00003580: 676e 5f6b 6579 732e 656e 6162 6c65 643a  gn_keys.enabled:
+00003590: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+000035a0: 6c65 5f69 6e66 6f5b 2275 7365 7273 225d  le_info["users"]
+000035b0: 203d 2074 6162 6c65 5f69 6e66 6f5b 2275   = table_info["u
+000035c0: 7365 7273 225d 202b 205b 2270 6172 656e  sers"] + ["paren
+000035d0: 745f 7573 6572 5f69 6422 5d0a 2020 2020  t_user_id"].    
+000035e0: 2020 2020 6966 2074 6573 7469 6e67 2e72      if testing.r
+000035f0: 6571 7569 7265 732e 6d61 7465 7269 616c  equires.material
+00003600: 697a 6564 5f76 6965 7773 2e65 6e61 626c  ized_views.enabl
+00003610: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00003620: 6d61 7465 7269 616c 697a 6564 203d 207b  materialized = {
+00003630: 2264 696e 6761 6c69 6e67 7322 7d0a 2020  "dingalings"}.  
+00003640: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00003650: 2020 2020 2020 2020 6d61 7465 7269 616c          material
+00003660: 697a 6564 203d 2073 6574 2829 0a20 2020  ized = set().   
+00003670: 2020 2020 2066 6f72 2074 6162 6c65 5f6e       for table_n
+00003680: 616d 6520 696e 2028 2275 7365 7273 222c  ame in ("users",
+00003690: 2022 656d 6169 6c5f 6164 6472 6573 7365   "email_addresse
+000036a0: 7322 2c20 2264 696e 6761 6c69 6e67 7322  s", "dingalings"
+000036b0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+000036c0: 756c 6c6e 616d 6520 3d20 7461 626c 655f  ullname = table_
+000036d0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+000036e0: 2069 6620 7363 6865 6d61 3a0a 2020 2020   if schema:.    
+000036f0: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
+00003700: 6e61 6d65 203d 2066 227b 7363 6865 6d61  name = f"{schema
+00003710: 7d2e 7b74 6162 6c65 5f6e 616d 657d 220a  }.{table_name}".
+00003720: 2020 2020 2020 2020 2020 2020 7669 6577              view
+00003730: 5f6e 616d 6520 3d20 6675 6c6c 6e61 6d65  _name = fullname
+00003740: 202b 2022 5f76 220a 2020 2020 2020 2020   + "_v".        
+00003750: 2020 2020 7072 6566 6978 203d 2022 4d41      prefix = "MA
+00003760: 5445 5249 414c 495a 4544 2022 2069 6620  TERIALIZED " if 
+00003770: 7461 626c 655f 6e61 6d65 2069 6e20 6d61  table_name in ma
+00003780: 7465 7269 616c 697a 6564 2065 6c73 6520  terialized else 
+00003790: 2222 0a20 2020 2020 2020 2020 2020 2063  "".            c
+000037a0: 6f6c 756d 6e73 203d 2022 220a 2020 2020  olumns = "".    
+000037b0: 2020 2020 2020 2020 666f 7220 636f 6c75          for colu
+000037c0: 6d6e 2069 6e20 7461 626c 655f 696e 666f  mn in table_info
+000037d0: 5b74 6162 6c65 5f6e 616d 655d 3a0a 2020  [table_name]:.  
+000037e0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000037f0: 6d74 203d 2074 6162 6c65 5f6e 616d 6520  mt = table_name 
+00003800: 2b20 222e 2220 2b20 636f 6c75 6d6e 202b  + "." + column +
+00003810: 2022 2041 5320 2220 2b20 636f 6c75 6d6e   " AS " + column
+00003820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003830: 2069 6620 636f 6c75 6d6e 733a 0a20 2020   if columns:.   
+00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003850: 2063 6f6c 756d 6e73 203d 2063 6f6c 756d   columns = colum
+00003860: 6e73 202b 2022 2c20 2220 2b20 7374 6d74  ns + ", " + stmt
+00003870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003880: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003890: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+000038a0: 6e73 203d 2073 746d 740a 2020 2020 2020  ns = stmt.      
+000038b0: 2020 2020 2020 7175 6572 7920 3d20 6622        query = f"
+000038c0: 2222 4352 4541 5445 207b 7072 6566 6978  ""CREATE {prefix
+000038d0: 7d56 4945 5720 7b76 6965 775f 6e61 6d65  }VIEW {view_name
+000038e0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000038f0: 2020 5351 4c20 5345 4355 5249 5459 2049    SQL SECURITY I
+00003900: 4e56 4f4b 4552 0a20 2020 2020 2020 2020  NVOKER.         
+00003910: 2020 2020 2020 2041 5320 5345 4c45 4354         AS SELECT
+00003920: 207b 636f 6c75 6d6e 737d 0a20 2020 2020   {columns}.     
+00003930: 2020 2020 2020 2020 2020 2046 524f 4d20             FROM 
+00003940: 7b66 756c 6c6e 616d 657d 2222 220a 0a20  {fullname}""".. 
+00003950: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+00003960: 2e6c 6973 7465 6e28 6d65 7461 6461 7461  .listen(metadata
+00003970: 2c20 2261 6674 6572 5f63 7265 6174 6522  , "after_create"
+00003980: 2c20 4444 4c28 7175 6572 7929 290a 2020  , DDL(query)).  
+00003990: 2020 2020 2020 2020 2020 6966 2074 6162            if tab
+000039a0: 6c65 5f6e 616d 6520 696e 206d 6174 6572  le_name in mater
+000039b0: 6961 6c69 7a65 643a 0a20 2020 2020 2020  ialized:.       
+000039c0: 2020 2020 2020 2020 2069 6e64 6578 5f6e           index_n
+000039d0: 616d 6520 3d20 226d 6174 5f69 6e64 6578  ame = "mat_index
+000039e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000039f0: 2020 6966 2073 6368 656d 6120 616e 6420    if schema and 
+00003a00: 7465 7374 696e 672e 6167 6169 6e73 7428  testing.against(
+00003a10: 226f 7261 636c 6522 293a 0a20 2020 2020  "oracle"):.     
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003a30: 6e64 6578 5f6e 616d 6520 3d20 6622 7b73  ndex_name = f"{s
+00003a40: 6368 656d 617d 2e7b 696e 6465 785f 6e61  chema}.{index_na
+00003a50: 6d65 7d22 0a20 2020 2020 2020 2020 2020  me}".           
+00003a60: 2020 2020 2069 6478 203d 2066 2243 5245       idx = f"CRE
+00003a70: 4154 4520 494e 4445 5820 7b69 6e64 6578  ATE INDEX {index
+00003a80: 5f6e 616d 657d 204f 4e20 7b76 6965 775f  _name} ON {view_
+00003a90: 6e61 6d65 7d28 6461 7461 2922 0a20 2020  name}(data)".   
+00003aa0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
+00003ab0: 6e74 2e6c 6973 7465 6e28 6d65 7461 6461  nt.listen(metada
+00003ac0: 7461 2c20 2261 6674 6572 5f63 7265 6174  ta, "after_creat
+00003ad0: 6522 2c20 4444 4c28 6964 7829 290a 2020  e", DDL(idx)).  
+00003ae0: 2020 2020 2020 2020 2020 6576 656e 742e            event.
+00003af0: 6c69 7374 656e 286d 6574 6164 6174 612c  listen(metadata,
+00003b00: 2022 6265 666f 7265 5f64 726f 7022 2c20   "before_drop", 
+00003b10: 4444 4c28 6622 4452 4f50 207b 7072 6566  DDL(f"DROP {pref
+00003b20: 6978 7d56 4945 5720 7b76 6965 775f 6e61  ix}VIEW {view_na
+00003b30: 6d65 7d22 2929 0a0a 2020 2020 4063 6c61  me}"))..    @cla
+00003b40: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00003b50: 2064 6566 696e 655f 7265 666c 6563 7465   define_reflecte
+00003b60: 645f 7461 626c 6573 2863 6c73 2c20 6d65  d_tables(cls, me
+00003b70: 7461 6461 7461 2c20 7363 6865 6d61 293a  tadata, schema):
+00003b80: 0a20 2020 2020 2020 2069 6620 7363 6865  .        if sche
+00003b90: 6d61 3a0a 2020 2020 2020 2020 2020 2020  ma:.            
+00003ba0: 7363 6865 6d61 5f70 7265 6669 7820 3d20  schema_prefix = 
+00003bb0: 7363 6865 6d61 202b 2022 2e22 0a20 2020  schema + ".".   
+00003bc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003bd0: 2020 2020 2020 2073 6368 656d 615f 7072         schema_pr
+00003be0: 6566 6978 203d 2022 220a 0a20 2020 2020  efix = ""..     
+00003bf0: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
+00003c00: 7175 6972 6573 2e73 656c 665f 7265 6665  quires.self_refe
+00003c10: 7265 6e74 6961 6c5f 666f 7265 6967 6e5f  rential_foreign_
+00003c20: 6b65 7973 2e65 6e61 626c 6564 3a0a 2020  keys.enabled:.  
+00003c30: 2020 2020 2020 2020 2020 7573 6572 7320            users 
+00003c40: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
+00003c50: 2020 2020 2020 2020 2022 7573 6572 7322           "users"
+00003c60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003c70: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
+00003c80: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00003c90: 6d6e 2822 7573 6572 5f69 6422 2c20 7371  mn("user_id", sq
+00003ca0: 6c61 6c63 6865 6d79 2e49 4e54 2c20 7072  lalchemy.INT, pr
+00003cb0: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
+00003cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cd0: 2043 6f6c 756d 6e28 2274 6573 7431 222c   Column("test1",
+00003ce0: 2073 716c 616c 6368 656d 792e 4348 4152   sqlalchemy.CHAR
+00003cf0: 2835 292c 206e 756c 6c61 626c 653d 4661  (5), nullable=Fa
+00003d00: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
+00003d10: 2020 2020 2020 436f 6c75 6d6e 2822 7465        Column("te
+00003d20: 7374 3222 2c20 7371 6c61 6c63 6865 6d79  st2", sqlalchemy
+00003d30: 2e46 6c6f 6174 2835 292c 206e 756c 6c61  .Float(5), nulla
+00003d40: 626c 653d 4661 6c73 6529 2c0a 2020 2020  ble=False),.    
+00003d50: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00003d60: 6d6e 280a 2020 2020 2020 2020 2020 2020  mn(.            
+00003d70: 2020 2020 2020 2020 2270 6172 656e 745f          "parent_
+00003d80: 7573 6572 5f69 6422 2c0a 2020 2020 2020  user_id",.      
+00003d90: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+00003da0: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
+00003db0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003dc0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+00003dd0: 2e46 6f72 6569 676e 4b65 7928 0a20 2020  .ForeignKey(.   
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 2020 2022 2573 7573 6572 732e 7573       "%susers.us
+00003e00: 6572 5f69 6422 2025 2073 6368 656d 615f  er_id" % schema_
+00003e10: 7072 6566 6978 2c20 6e61 6d65 3d22 7573  prefix, name="us
+00003e20: 6572 5f69 645f 666b 220a 2020 2020 2020  er_id_fk".      
+00003e30: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00003e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e50: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00003e60: 2020 2020 7363 6865 6d61 3d73 6368 656d      schema=schem
+00003e70: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00003e80: 2020 2074 6573 745f 6e65 6564 735f 666b     test_needs_fk
+00003e90: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00003ea0: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+00003eb0: 653a 0a20 2020 2020 2020 2020 2020 2075  e:.            u
+00003ec0: 7365 7273 203d 2054 6162 6c65 280a 2020  sers = Table(.  
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00003ee0: 7365 7273 222c 0a20 2020 2020 2020 2020  sers",.         
+00003ef0: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
+00003f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f10: 2043 6f6c 756d 6e28 2275 7365 725f 6964   Column("user_id
+00003f20: 222c 2073 716c 616c 6368 656d 792e 494e  ", sqlalchemy.IN
+00003f30: 542c 2070 7269 6d61 7279 5f6b 6579 3d54  T, primary_key=T
+00003f40: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+00003f50: 2020 2020 2020 436f 6c75 6d6e 2822 7465        Column("te
+00003f60: 7374 3122 2c20 7371 6c61 6c63 6865 6d79  st1", sqlalchemy
+00003f70: 2e43 4841 5228 3529 2c20 6e75 6c6c 6162  .CHAR(5), nullab
+00003f80: 6c65 3d46 616c 7365 292c 0a20 2020 2020  le=False),.     
+00003f90: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00003fa0: 6e28 2274 6573 7432 222c 2073 716c 616c  n("test2", sqlal
+00003fb0: 6368 656d 792e 466c 6f61 7428 3529 2c20  chemy.Float(5), 
+00003fc0: 6e75 6c6c 6162 6c65 3d46 616c 7365 292c  nullable=False),
+00003fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003fe0: 2073 6368 656d 613d 7363 6865 6d61 2c0a   schema=schema,.
+00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004000: 7465 7374 5f6e 6565 6473 5f66 6b3d 5472  test_needs_fk=Tr
+00004010: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00004020: 290a 0a20 2020 2020 2020 2054 6162 6c65  )..        Table
+00004030: 280a 2020 2020 2020 2020 2020 2020 2264  (.            "d
+00004040: 696e 6761 6c69 6e67 7322 2c0a 2020 2020  ingalings",.    
+00004050: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+00004060: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+00004070: 6c75 6d6e 2822 6469 6e67 616c 696e 675f  lumn("dingaling_
+00004080: 6964 222c 2073 716c 616c 6368 656d 792e  id", sqlalchemy.
+00004090: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
+000040a0: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
+000040b0: 2020 2020 2020 2020 436f 6c75 6d6e 280a          Column(.
+000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040d0: 2261 6464 7265 7373 5f69 6422 2c0a 2020  "address_id",.  
+000040e0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+000040f0: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
+00004100: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004110: 2020 7371 6c61 6c63 6865 6d79 2e46 6f72    sqlalchemy.For
+00004120: 6569 676e 4b65 7928 2225 7365 6d61 696c  eignKey("%semail
+00004130: 5f61 6464 7265 7373 6573 2e61 6464 7265  _addresses.addre
+00004140: 7373 5f69 6422 2025 2073 6368 656d 615f  ss_id" % schema_
+00004150: 7072 6566 6978 292c 0a20 2020 2020 2020  prefix),.       
+00004160: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00004170: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
+00004180: 2020 2020 2020 2020 2020 2020 2269 645f              "id_
+00004190: 7573 6572 222c 0a20 2020 2020 2020 2020  user",.         
+000041a0: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
+000041b0: 792e 496e 7465 6765 722c 0a20 2020 2020  y.Integer,.     
+000041c0: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
+000041d0: 6368 656d 792e 466f 7265 6967 6e4b 6579  chemy.ForeignKey
+000041e0: 2822 2573 7573 6572 732e 7573 6572 5f69  ("%susers.user_i
+000041f0: 6422 2025 2073 6368 656d 615f 7072 6566  d" % schema_pref
+00004200: 6978 292c 0a20 2020 2020 2020 2020 2020  ix),.           
+00004210: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00004220: 436f 6c75 6d6e 2822 6461 7461 222c 2073  Column("data", s
+00004230: 716c 616c 6368 656d 792e 5374 7269 6e67  qlalchemy.String
+00004240: 2833 3029 292c 0a20 2020 2020 2020 2020  (30)),.         
+00004250: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
+00004260: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
+00004270: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
+00004280: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00004290: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
+000042a0: 2020 2020 2020 2022 656d 6169 6c5f 6164         "email_ad
+000042b0: 6472 6573 7365 7322 2c0a 2020 2020 2020  dresses",.      
+000042c0: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
+000042d0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+000042e0: 6d6e 2822 6164 6472 6573 735f 6964 222c  mn("address_id",
+000042f0: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
+00004300: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+00004310: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00004320: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
+00004330: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
+00004340: 6f74 655f 7573 6572 5f69 6422 2c0a 2020  ote_user_id",.  
+00004350: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+00004360: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
+00004370: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004380: 2020 7371 6c61 6c63 6865 6d79 2e46 6f72    sqlalchemy.For
+00004390: 6569 676e 4b65 7928 7573 6572 732e 632e  eignKey(users.c.
+000043a0: 7573 6572 5f69 6429 2c0a 2020 2020 2020  user_id),.      
+000043b0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+000043c0: 2020 2020 2043 6f6c 756d 6e28 2265 6d61       Column("ema
+000043d0: 696c 5f61 6464 7265 7373 222c 2073 716c  il_address", sql
+000043e0: 616c 6368 656d 792e 5374 7269 6e67 2832  alchemy.String(2
+000043f0: 3029 292c 0a20 2020 2020 2020 2020 2020  0)),.           
+00004400: 2073 716c 616c 6368 656d 792e 5072 696d   sqlalchemy.Prim
+00004410: 6172 794b 6579 436f 6e73 7472 6169 6e74  aryKeyConstraint
+00004420: 2822 6164 6472 6573 735f 6964 222c 206e  ("address_id", n
+00004430: 616d 653d 2265 6d61 696c 5f61 645f 706b  ame="email_ad_pk
+00004440: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00004450: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+00004460: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+00004470: 6e65 6564 735f 666b 3d54 7275 652c 0a20  needs_fk=True,. 
+00004480: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004490: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+000044a0: 2020 2020 2263 6f6d 6d65 6e74 5f74 6573      "comment_tes
+000044b0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+000044c0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+000044d0: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+000044e0: 222c 2073 716c 616c 6368 656d 792e 496e  ", sqlalchemy.In
+000044f0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+00004500: 6579 3d54 7275 652c 2063 6f6d 6d65 6e74  ey=True, comment
+00004510: 3d22 6964 2063 6f6d 6d65 6e74 2229 2c0a  ="id comment"),.
+00004520: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00004530: 6d6e 2822 6461 7461 222c 2073 716c 616c  mn("data", sqlal
+00004540: 6368 656d 792e 5374 7269 6e67 2832 3029  chemy.String(20)
+00004550: 2c20 636f 6d6d 656e 743d 2264 6174 6120  , comment="data 
+00004560: 2520 636f 6d6d 656e 7422 292c 0a20 2020  % comment"),.   
+00004570: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00004580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004590: 2022 6432 222c 0a20 2020 2020 2020 2020   "d2",.         
+000045a0: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
+000045b0: 792e 5374 7269 6e67 2832 3029 2c0a 2020  y.String(20),.  
+000045c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000045d0: 6d6d 656e 743d 7222 2222 436f 6d6d 656e  mment=r"""Commen
+000045e0: 7420 7479 7065 7320 7479 7065 2073 7065  t types type spe
+000045f0: 6564 696c 7920 2720 2220 5c20 2727 2046  edily ' " \ '' F
+00004600: 756e 2122 2222 2c0a 2020 2020 2020 2020  un!""",.        
+00004610: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00004620: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
+00004630: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00004640: 6d6d 656e 743d 7222 2222 7468 6520 7465  mment=r"""the te
+00004650: 7374 2025 2027 2022 205c 2074 6162 6c65  st % ' " \ table
+00004660: 2063 6f6d 6d65 6e74 2222 222c 0a20 2020   comment""",.   
+00004670: 2020 2020 2029 0a20 2020 2020 2020 2054       ).        T
+00004680: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+00004690: 2020 226e 6f5f 636f 6e73 7472 6169 6e74    "no_constraint
+000046a0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+000046b0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+000046c0: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
+000046d0: 7461 222c 2073 716c 616c 6368 656d 792e  ta", sqlalchemy.
+000046e0: 5374 7269 6e67 2832 3029 292c 0a20 2020  String(20)),.   
+000046f0: 2020 2020 2020 2020 2073 6368 656d 613d           schema=
+00004700: 7363 6865 6d61 2c0a 2020 2020 2020 2020  schema,.        
+00004710: 290a 0a20 2020 2020 2020 2069 6620 7465  )..        if te
+00004720: 7374 696e 672e 7265 7175 6972 6573 2e63  sting.requires.c
+00004730: 726f 7373 5f73 6368 656d 615f 666b 5f72  ross_schema_fk_r
+00004740: 6566 6c65 6374 696f 6e2e 656e 6162 6c65  eflection.enable
+00004750: 643a 0a20 2020 2020 2020 2020 2020 2069  d:.            i
+00004760: 6620 7363 6865 6d61 2069 7320 4e6f 6e65  f schema is None
+00004770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004780: 2020 5461 626c 6528 0a20 2020 2020 2020    Table(.       
+00004790: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
+000047a0: 6361 6c5f 7461 626c 6522 2c0a 2020 2020  cal_table",.    
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+000047d0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+000047e0: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
+000047f0: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
+00004800: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+00004810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004820: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
+00004830: 7461 222c 2073 716c 616c 6368 656d 792e  ta", sqlalchemy.
+00004840: 5374 7269 6e67 2832 3029 292c 0a20 2020  String(20)),.   
+00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004860: 2043 6f6c 756d 6e28 0a20 2020 2020 2020   Column(.       
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2022 7265 6d6f 7465 5f69 6422 2c0a 2020   "remote_id",.  
+00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048a0: 2020 2020 2020 466f 7265 6967 6e4b 6579        ForeignKey
+000048b0: 2822 2573 2e72 656d 6f74 655f 7461 626c  ("%s.remote_tabl
+000048c0: 655f 322e 6964 2220 2520 7465 7374 696e  e_2.id" % testin
+000048d0: 672e 636f 6e66 6967 2e74 6573 745f 7363  g.config.test_sc
+000048e0: 6865 6d61 292c 0a20 2020 2020 2020 2020  hema),.         
+000048f0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004910: 2020 7465 7374 5f6e 6565 6473 5f66 6b3d    test_needs_fk=
+00004920: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00004930: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00004940: 3d63 6f6e 6669 672e 6462 2e64 6961 6c65  =config.db.diale
+00004950: 6374 2e64 6566 6175 6c74 5f73 6368 656d  ct.default_schem
+00004960: 615f 6e61 6d65 2c0a 2020 2020 2020 2020  a_name,.        
+00004970: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00004980: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00004990: 2020 2020 2020 2020 2020 2020 5461 626c              Tabl
+000049a0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+000049b0: 2020 2020 2020 2022 7265 6d6f 7465 5f74         "remote_t
+000049c0: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
+000049d0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+000049e0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+000049f0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00004a00: 2269 6422 2c20 7371 6c61 6c63 6865 6d79  "id", sqlalchemy
+00004a10: 2e49 6e74 6567 6572 2c20 7072 696d 6172  .Integer, primar
+00004a20: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
+00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a40: 2043 6f6c 756d 6e28 0a20 2020 2020 2020   Column(.       
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a60: 2022 6c6f 6361 6c5f 6964 222c 0a20 2020   "local_id",.   
+00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a80: 2020 2020 2046 6f72 6569 676e 4b65 7928       ForeignKey(
+00004a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004aa0: 2020 2020 2020 2020 2020 2020 2022 2573               "%s
+00004ab0: 2e6c 6f63 616c 5f74 6162 6c65 2e69 6422  .local_table.id"
+00004ac0: 2025 2063 6f6e 6669 672e 6462 2e64 6961   % config.db.dia
+00004ad0: 6c65 6374 2e64 6566 6175 6c74 5f73 6368  lect.default_sch
+00004ae0: 656d 615f 6e61 6d65 0a20 2020 2020 2020  ema_name.       
 00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00004b10: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00004b20: 2822 6461 7461 222c 2073 716c 616c 6368  ("data", sqlalch
-00004b30: 656d 792e 5374 7269 6e67 2832 3029 292c  emy.String(20)),
-00004b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b50: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
-00004b60: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
-00004b70: 2020 2020 2020 2020 7465 7374 5f6e 6565          test_nee
-00004b80: 6473 5f66 6b3d 5472 7565 2c0a 2020 2020  ds_fk=True,.    
-00004b90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 5461                Ta
-00004bb0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00004bc0: 2020 2020 2020 2020 2022 7265 6d6f 7465           "remote
-00004bd0: 5f74 6162 6c65 5f32 222c 0a20 2020 2020  _table_2",.     
-00004be0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00004bf0: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
-00004c00: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
-00004c10: 756d 6e28 2269 6422 2c20 7371 6c61 6c63  umn("id", sqlalc
-00004c20: 6865 6d79 2e49 6e74 6567 6572 2c20 7072  hemy.Integer, pr
-00004c30: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
-00004c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c50: 2020 2020 2043 6f6c 756d 6e28 2264 6174       Column("dat
-00004c60: 6122 2c20 7371 6c61 6c63 6865 6d79 2e53  a", sqlalchemy.S
-00004c70: 7472 696e 6728 3230 2929 2c0a 2020 2020  tring(20)),.    
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 2020 2074 6573 745f 6e65 6564 735f 666b     test_needs_fk
-00004cc0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00004cd0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00004ce0: 2020 6966 2074 6573 7469 6e67 2e72 6571    if testing.req
-00004cf0: 7569 7265 732e 696e 6465 785f 7265 666c  uires.index_refl
-00004d00: 6563 7469 6f6e 2e65 6e61 626c 6564 3a0a  ection.enabled:.
-00004d10: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-00004d20: 6c63 6865 6d79 2e49 6e64 6578 2822 7573  lchemy.Index("us
-00004d30: 6572 735f 745f 6964 7822 2c20 7573 6572  ers_t_idx", user
-00004d40: 732e 632e 7465 7374 312c 2075 7365 7273  s.c.test1, users
-00004d50: 2e63 2e74 6573 7432 2c20 756e 6971 7565  .c.test2, unique
-00004d60: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00004d70: 2020 2073 716c 616c 6368 656d 792e 496e     sqlalchemy.In
-00004d80: 6465 7828 0a20 2020 2020 2020 2020 2020  dex(.           
-00004d90: 2020 2020 2022 7573 6572 735f 616c 6c5f       "users_all_
-00004da0: 6964 7822 2c20 7573 6572 732e 632e 7573  idx", users.c.us
-00004db0: 6572 5f69 642c 2075 7365 7273 2e63 2e74  er_id, users.c.t
-00004dc0: 6573 7432 2c20 7573 6572 732e 632e 7465  est2, users.c.te
-00004dd0: 7374 310a 2020 2020 2020 2020 2020 2020  st1.            
-00004de0: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00004df0: 6620 6e6f 7420 7363 6865 6d61 3a0a 2020  f not schema:.  
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00004e10: 7465 7374 5f6e 6565 6473 5f66 6b20 6973  test_needs_fk is
-00004e20: 2061 7420 7468 6520 6d6f 6d65 6e74 2074   at the moment t
-00004e30: 6f20 666f 7263 6520 4d79 5351 4c20 496e  o force MySQL In
-00004e40: 6e6f 4442 0a20 2020 2020 2020 2020 2020  noDB.           
-00004e50: 2020 2020 206e 6f6e 636f 6c5f 6964 785f       noncol_idx_
-00004e60: 7465 7374 5f6e 6f70 6b20 3d20 5461 626c  test_nopk = Tabl
-00004e70: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00004e80: 2020 2020 2020 2022 6e6f 6e63 6f6c 5f69         "noncol_i
-00004e90: 6478 5f74 6573 745f 6e6f 706b 222c 0a20  dx_test_nopk",. 
-00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004eb0: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2043 6f6c 756d 6e28 2269 6422 2c20 7371   Column("id", sq
-00004ee0: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
-00004ef0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-00004f00: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-00004f10: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00004f20: 2271 222c 2073 716c 616c 6368 656d 792e  "q", sqlalchemy.
-00004f30: 5374 7269 6e67 2835 2929 2c0a 2020 2020  String(5)),.    
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 7465 7374 5f6e 6565 6473 5f66 6b3d 5472  test_needs_fk=Tr
-00004f60: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00004f70: 2020 2020 2020 2020 6578 7465 6e64 5f65          extend_e
-00004f80: 7869 7374 696e 673d 5472 7565 2c0a 2020  xisting=True,.  
-00004f90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00004fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004fb0: 206e 6f6e 636f 6c5f 6964 785f 7465 7374   noncol_idx_test
-00004fc0: 5f70 6b20 3d20 5461 626c 6528 0a20 2020  _pk = Table(.   
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2022 6e6f 6e63 6f6c 5f69 6478 5f74 6573   "noncol_idx_tes
-00004ff0: 745f 706b 222c 0a20 2020 2020 2020 2020  t_pk",.         
-00005000: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00005010: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00005020: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00005030: 2269 6422 2c20 7371 6c61 6c63 6865 6d79  "id", sqlalchemy
-00005040: 2e49 6e74 6567 6572 2c20 7072 696d 6172  .Integer, primar
-00005050: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005070: 2043 6f6c 756d 6e28 2271 222c 2073 716c   Column("q", sql
-00005080: 616c 6368 656d 792e 5374 7269 6e67 2835  alchemy.String(5
-00005090: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000050a0: 2020 2020 2020 2020 7465 7374 5f6e 6565          test_nee
-000050b0: 6473 5f66 6b3d 5472 7565 2c0a 2020 2020  ds_fk=True,.    
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050d0: 6578 7465 6e64 5f65 7869 7374 696e 673d  extend_existing=
-000050e0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-000050f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00005100: 2020 2020 2020 2020 2069 6620 7465 7374           if test
-00005110: 696e 672e 7265 7175 6972 6573 2e69 6e64  ing.requires.ind
-00005120: 6578 6573 5f77 6974 685f 6173 6364 6573  exes_with_ascdes
-00005130: 632e 656e 6162 6c65 643a 0a20 2020 2020  c.enabled:.     
-00005140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005150: 716c 616c 6368 656d 792e 496e 6465 7828  qlalchemy.Index(
-00005160: 226e 6f6e 636f 6c5f 6964 785f 6e6f 706b  "noncol_idx_nopk
-00005170: 222c 206e 6f6e 636f 6c5f 6964 785f 7465  ", noncol_idx_te
-00005180: 7374 5f6e 6f70 6b2e 632e 712e 6465 7363  st_nopk.c.q.desc
-00005190: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-000051a0: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
-000051b0: 6d79 2e49 6e64 6578 2822 6e6f 6e63 6f6c  my.Index("noncol
-000051c0: 5f69 6478 5f70 6b22 2c20 6e6f 6e63 6f6c  _idx_pk", noncol
-000051d0: 5f69 6478 5f74 6573 745f 706b 2e63 2e71  _idx_test_pk.c.q
-000051e0: 2e64 6573 6328 2929 0a0a 2020 2020 2020  .desc())..      
-000051f0: 2020 6966 2074 6573 7469 6e67 2e72 6571    if testing.req
-00005200: 7569 7265 732e 7669 6577 5f63 6f6c 756d  uires.view_colum
-00005210: 6e5f 7265 666c 6563 7469 6f6e 2e65 6e61  n_reflection.ena
-00005220: 626c 6564 2061 6e64 206e 6f74 2062 6f6f  bled and not boo
-00005230: 6c28 0a20 2020 2020 2020 2020 2020 206f  l(.            o
-00005240: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
-00005250: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
-00005260: 484f 5354 2229 0a20 2020 2020 2020 2029  HOST").        )
-00005270: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-00005280: 732e 6465 6669 6e65 5f76 6965 7773 286d  s.define_views(m
-00005290: 6574 6164 6174 612c 2073 6368 656d 6129  etadata, schema)
-000052a0: 0a0a 2020 2020 4074 6573 7469 6e67 2e63  ..    @testing.c
-000052b0: 6f6d 6269 6e61 7469 6f6e 7328 0a20 2020  ombinations(.   
-000052c0: 2020 2020 2028 4661 6c73 652c 2046 616c       (False, Fal
-000052d0: 7365 292c 0a20 2020 2020 2020 2028 4661  se),.        (Fa
-000052e0: 6c73 652c 2054 7275 652c 2074 6573 7469  lse, True, testi
-000052f0: 6e67 2e72 6571 7569 7265 732e 7363 6865  ng.requires.sche
-00005300: 6d61 7329 2c0a 2020 2020 2020 2020 2854  mas),.        (T
-00005310: 7275 652c 2046 616c 7365 2c20 7465 7374  rue, False, test
-00005320: 696e 672e 7265 7175 6972 6573 2e76 6965  ing.requires.vie
-00005330: 775f 7265 666c 6563 7469 6f6e 292c 0a20  w_reflection),. 
-00005340: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-00005350: 2020 2020 2054 7275 652c 0a20 2020 2020       True,.     
-00005360: 2020 2020 2020 2054 7275 652c 0a20 2020         True,.   
-00005370: 2020 2020 2020 2020 2074 6573 7469 6e67           testing
-00005380: 2e72 6571 7569 7265 732e 7363 6865 6d61  .requires.schema
-00005390: 7320 2b20 7465 7374 696e 672e 7265 7175  s + testing.requ
-000053a0: 6972 6573 2e76 6965 775f 7265 666c 6563  ires.view_reflec
-000053b0: 7469 6f6e 2c0a 2020 2020 2020 2020 292c  tion,.        ),
-000053c0: 0a20 2020 2020 2020 2061 7267 6e61 6d65  .        argname
-000053d0: 733d 2275 7365 5f76 6965 7773 2c75 7365  s="use_views,use
-000053e0: 5f73 6368 656d 6122 2c0a 2020 2020 290a  _schema",.    ).
-000053f0: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-00005400: 5f63 6f6c 756d 6e73 2873 656c 662c 2063  _columns(self, c
-00005410: 6f6e 6e65 6374 696f 6e2c 2075 7365 5f76  onnection, use_v
-00005420: 6965 7773 2c20 7573 655f 7363 6865 6d61  iews, use_schema
-00005430: 293a 0a20 2020 2020 2020 2069 6620 7573  ):.        if us
-00005440: 655f 7669 6577 7320 616e 6420 626f 6f6c  e_views and bool
-00005450: 286f 732e 656e 7669 726f 6e2e 6765 7428  (os.environ.get(
-00005460: 2253 5041 4e4e 4552 5f45 4d55 4c41 544f  "SPANNER_EMULATO
-00005470: 525f 484f 5354 2229 293a 0a20 2020 2020  R_HOST")):.     
-00005480: 2020 2020 2020 2070 7974 6573 742e 736b         pytest.sk
-00005490: 6970 2822 536b 6970 7065 6420 6f6e 2065  ip("Skipped on e
-000054a0: 6d75 6c61 746f 7222 290a 0a20 2020 2020  mulator")..     
-000054b0: 2020 2073 6368 656d 6120 3d20 4e6f 6e65     schema = None
-000054c0: 0a0a 2020 2020 2020 2020 7573 6572 732c  ..        users,
-000054d0: 2061 6464 7265 7373 6573 203d 2028 7365   addresses = (se
-000054e0: 6c66 2e74 6162 6c65 732e 7573 6572 732c  lf.tables.users,
-000054f0: 2073 656c 662e 7461 626c 6573 2e65 6d61   self.tables.ema
-00005500: 696c 5f61 6464 7265 7373 6573 290a 2020  il_addresses).  
-00005510: 2020 2020 2020 6966 2075 7365 5f76 6965        if use_vie
-00005520: 7773 3a0a 2020 2020 2020 2020 2020 2020  ws:.            
-00005530: 7461 626c 655f 6e61 6d65 7320 3d20 5b22  table_names = ["
-00005540: 7573 6572 735f 7622 2c20 2265 6d61 696c  users_v", "email
-00005550: 5f61 6464 7265 7373 6573 5f76 222c 2022  _addresses_v", "
-00005560: 6469 6e67 616c 696e 6773 5f76 225d 0a20  dingalings_v"]. 
-00005570: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005580: 2020 2020 2020 2020 2074 6162 6c65 5f6e           table_n
-00005590: 616d 6573 203d 205b 2275 7365 7273 222c  ames = ["users",
-000055a0: 2022 656d 6169 6c5f 6164 6472 6573 7365   "email_addresse
-000055b0: 7322 5d0a 0a20 2020 2020 2020 2069 6e73  s"]..        ins
-000055c0: 7020 3d20 696e 7370 6563 7428 636f 6e6e  p = inspect(conn
-000055d0: 6563 7469 6f6e 290a 2020 2020 2020 2020  ection).        
-000055e0: 666f 7220 7461 626c 655f 6e61 6d65 2c20  for table_name, 
-000055f0: 7461 626c 6520 696e 207a 6970 2874 6162  table in zip(tab
-00005600: 6c65 5f6e 616d 6573 2c20 2875 7365 7273  le_names, (users
-00005610: 2c20 6164 6472 6573 7365 7329 293a 0a20  , addresses)):. 
-00005620: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00005630: 615f 6e61 6d65 203d 2073 6368 656d 610a  a_name = schema.
-00005640: 2020 2020 2020 2020 2020 2020 636f 6c73              cols
-00005650: 203d 2069 6e73 702e 6765 745f 636f 6c75   = insp.get_colu
-00005660: 6d6e 7328 7461 626c 655f 6e61 6d65 2c20  mns(table_name, 
-00005670: 7363 6865 6d61 3d73 6368 656d 615f 6e61  schema=schema_na
-00005680: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-00005690: 6973 5f74 7275 6528 6c65 6e28 636f 6c73  is_true(len(cols
-000056a0: 2920 3e20 302c 206c 656e 2863 6f6c 7329  ) > 0, len(cols)
-000056b0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-000056c0: 2073 686f 756c 6420 6265 2069 6e20 6f72   should be in or
-000056d0: 6465 720a 0a20 2020 2020 2020 2020 2020  der..           
-000056e0: 2066 6f72 2069 2c20 636f 6c20 696e 2065   for i, col in e
-000056f0: 6e75 6d65 7261 7465 2874 6162 6c65 2e63  numerate(table.c
-00005700: 6f6c 756d 6e73 293a 0a20 2020 2020 2020  olumns):.       
-00005710: 2020 2020 2020 2020 2065 715f 2863 6f6c           eq_(col
-00005720: 2e6e 616d 652c 2063 6f6c 735b 695d 5b22  .name, cols[i]["
-00005730: 6e61 6d65 225d 290a 2020 2020 2020 2020  name"]).        
-00005740: 2020 2020 2020 2020 6374 7970 6520 3d20          ctype = 
-00005750: 636f 6c73 5b69 5d5b 2274 7970 6522 5d2e  cols[i]["type"].
-00005760: 5f5f 636c 6173 735f 5f0a 2020 2020 2020  __class__.      
-00005770: 2020 2020 2020 2020 2020 6374 7970 655f            ctype_
-00005780: 6465 6620 3d20 636f 6c2e 7479 7065 0a20  def = col.type. 
-00005790: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000057a0: 6620 6973 696e 7374 616e 6365 2863 7479  f isinstance(cty
-000057b0: 7065 5f64 6566 2c20 7371 6c61 6c63 6865  pe_def, sqlalche
-000057c0: 6d79 2e74 7970 6573 2e54 7970 6545 6e67  my.types.TypeEng
-000057d0: 696e 6529 3a0a 2020 2020 2020 2020 2020  ine):.          
-000057e0: 2020 2020 2020 2020 2020 6374 7970 655f            ctype_
-000057f0: 6465 6620 3d20 6374 7970 655f 6465 662e  def = ctype_def.
-00005800: 5f5f 636c 6173 735f 5f0a 0a20 2020 2020  __class__..     
-00005810: 2020 2020 2020 2020 2020 2023 204f 7261             # Ora
-00005820: 636c 6520 7265 7475 726e 7320 4461 7465  cle returns Date
-00005830: 2066 6f72 2044 6174 6554 696d 652e 0a0a   for DateTime...
-00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005850: 6966 2074 6573 7469 6e67 2e61 6761 696e  if testing.again
-00005860: 7374 2822 6f72 6163 6c65 2229 2061 6e64  st("oracle") and
-00005870: 2063 7479 7065 5f64 6566 2069 6e20 280a   ctype_def in (.
-00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005890: 2020 2020 7479 7065 732e 4461 7465 2c0a      types.Date,.
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2020 7479 7065 732e 4461 7465 5469      types.DateTi
-000058c0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-000058d0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-000058e0: 2020 2020 2020 2020 2020 2063 7479 7065             ctype
-000058f0: 5f64 6566 203d 2074 7970 6573 2e44 6174  _def = types.Dat
-00005900: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-00005910: 2020 2023 2061 7373 6572 7420 7468 6174     # assert that
-00005920: 2074 6865 2064 6573 6972 6564 2074 7970   the desired typ
-00005930: 6520 616e 6420 7265 7475 726e 2074 7970  e and return typ
-00005940: 6520 7368 6172 650a 2020 2020 2020 2020  e share.        
-00005950: 2020 2020 2020 2020 2320 6120 6261 7365          # a base
-00005960: 2077 6974 6869 6e20 6f6e 6520 6f66 2074   within one of t
-00005970: 6865 2067 656e 6572 6963 2074 7970 6573  he generic types
-00005980: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00005990: 2020 2069 735f 7472 7565 280a 2020 2020     is_true(.    
-000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059b0: 6c65 6e28 0a20 2020 2020 2020 2020 2020  len(.           
-000059c0: 2020 2020 2020 2020 2020 2020 2073 6574               set
-000059d0: 2863 7479 7065 2e5f 5f6d 726f 5f5f 290a  (ctype.__mro__).
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 2020 2020 2020 2020 2e69 6e74 6572 7365          .interse
-00005a00: 6374 696f 6e28 6374 7970 655f 6465 662e  ction(ctype_def.
-00005a10: 5f5f 6d72 6f5f 5f29 0a20 2020 2020 2020  __mro__).       
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 202e 696e 7465 7273 6563 7469 6f6e 280a   .intersection(.
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00004b00: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00004b10: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00004b30: 6f6c 756d 6e28 2264 6174 6122 2c20 7371  olumn("data", sq
+00004b40: 6c61 6c63 6865 6d79 2e53 7472 696e 6728  lalchemy.String(
+00004b50: 3230 2929 2c0a 2020 2020 2020 2020 2020  20)),.          
+00004b60: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00004b70: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+00004b80: 2020 2020 2020 2020 2020 2020 2074 6573               tes
+00004b90: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
+00004ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004bb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00004bc0: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
+00004bd0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00004be0: 656d 6f74 655f 7461 626c 655f 3222 2c0a  emote_table_2",.
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
+00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c20: 2020 436f 6c75 6d6e 2822 6964 222c 2073    Column("id", s
+00004c30: 716c 616c 6368 656d 792e 496e 7465 6765  qlalchemy.Intege
+00004c40: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+00004c50: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+00004c60: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+00004c70: 2822 6461 7461 222c 2073 716c 616c 6368  ("data", sqlalch
+00004c80: 656d 792e 5374 7269 6e67 2832 3029 292c  emy.String(20)),
+00004c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ca0: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
+00004cb0: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
+00004cc0: 2020 2020 2020 2020 7465 7374 5f6e 6565          test_nee
+00004cd0: 6473 5f66 6b3d 5472 7565 2c0a 2020 2020  ds_fk=True,.    
+00004ce0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00004cf0: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
+00004d00: 672e 7265 7175 6972 6573 2e69 6e64 6578  g.requires.index
+00004d10: 5f72 6566 6c65 6374 696f 6e2e 656e 6162  _reflection.enab
+00004d20: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+00004d30: 2073 716c 616c 6368 656d 792e 496e 6465   sqlalchemy.Inde
+00004d40: 7828 2275 7365 7273 5f74 5f69 6478 222c  x("users_t_idx",
+00004d50: 2075 7365 7273 2e63 2e74 6573 7431 2c20   users.c.test1, 
+00004d60: 7573 6572 732e 632e 7465 7374 322c 2075  users.c.test2, u
+00004d70: 6e69 7175 653d 5472 7565 290a 2020 2020  nique=True).    
+00004d80: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
+00004d90: 6d79 2e49 6e64 6578 280a 2020 2020 2020  my.Index(.      
+00004da0: 2020 2020 2020 2020 2020 2275 7365 7273            "users
+00004db0: 5f61 6c6c 5f69 6478 222c 2075 7365 7273  _all_idx", users
+00004dc0: 2e63 2e75 7365 725f 6964 2c20 7573 6572  .c.user_id, user
+00004dd0: 732e 632e 7465 7374 322c 2075 7365 7273  s.c.test2, users
+00004de0: 2e63 2e74 6573 7431 0a20 2020 2020 2020  .c.test1.       
+00004df0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00004e00: 2020 2020 6966 206e 6f74 2073 6368 656d      if not schem
+00004e10: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
+00004e20: 2020 2023 2074 6573 745f 6e65 6564 735f     # test_needs_
+00004e30: 666b 2069 7320 6174 2074 6865 206d 6f6d  fk is at the mom
+00004e40: 656e 7420 746f 2066 6f72 6365 204d 7953  ent to force MyS
+00004e50: 514c 2049 6e6e 6f44 420a 2020 2020 2020  QL InnoDB.      
+00004e60: 2020 2020 2020 2020 2020 6e6f 6e63 6f6c            noncol
+00004e70: 5f69 6478 5f74 6573 745f 6e6f 706b 203d  _idx_test_nopk =
+00004e80: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00004e90: 2020 2020 2020 2020 2020 2020 226e 6f6e              "non
+00004ea0: 636f 6c5f 6964 785f 7465 7374 5f6e 6f70  col_idx_test_nop
+00004eb0: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
+00004ec0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+00004ed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004ee0: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+00004ef0: 222c 2073 716c 616c 6368 656d 792e 496e  ", sqlalchemy.In
+00004f00: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+00004f10: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
+00004f20: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00004f30: 6c75 6d6e 2822 7122 2c20 7371 6c61 6c63  lumn("q", sqlalc
+00004f40: 6865 6d79 2e53 7472 696e 6728 3529 292c  hemy.String(5)),
+00004f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f60: 2020 2020 2074 6573 745f 6e65 6564 735f       test_needs_
+00004f70: 666b 3d54 7275 652c 0a20 2020 2020 2020  fk=True,.       
+00004f80: 2020 2020 2020 2020 2020 2020 2065 7874               ext
+00004f90: 656e 645f 6578 6973 7469 6e67 3d54 7275  end_existing=Tru
+00004fa0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00004fb0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00004fc0: 2020 2020 2020 6e6f 6e63 6f6c 5f69 6478        noncol_idx
+00004fd0: 5f74 6573 745f 706b 203d 2054 6162 6c65  _test_pk = Table
+00004fe0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004ff0: 2020 2020 2020 226e 6f6e 636f 6c5f 6964        "noncol_id
+00005000: 785f 7465 7374 5f70 6b22 2c0a 2020 2020  x_test_pk",.    
+00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005020: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00005030: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00005040: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
+00005050: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
+00005060: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+00005070: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005080: 2020 2020 2020 436f 6c75 6d6e 2822 7122        Column("q"
+00005090: 2c20 7371 6c61 6c63 6865 6d79 2e53 7472  , sqlalchemy.Str
+000050a0: 696e 6728 3529 292c 0a20 2020 2020 2020  ing(5)),.       
+000050b0: 2020 2020 2020 2020 2020 2020 2074 6573               tes
+000050c0: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
+000050d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000050e0: 2020 2020 2065 7874 656e 645f 6578 6973       extend_exis
+000050f0: 7469 6e67 3d54 7275 652c 0a20 2020 2020  ting=True,.     
+00005100: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00005110: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005120: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
+00005130: 732e 696e 6465 7865 735f 7769 7468 5f61  s.indexes_with_a
+00005140: 7363 6465 7363 2e65 6e61 626c 6564 3a0a  scdesc.enabled:.
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 7371 6c61 6c63 6865 6d79 2e49      sqlalchemy.I
+00005170: 6e64 6578 2822 6e6f 6e63 6f6c 5f69 6478  ndex("noncol_idx
+00005180: 5f6e 6f70 6b22 2c20 6e6f 6e63 6f6c 5f69  _nopk", noncol_i
+00005190: 6478 5f74 6573 745f 6e6f 706b 2e63 2e71  dx_test_nopk.c.q
+000051a0: 2e64 6573 6328 2929 0a20 2020 2020 2020  .desc()).       
+000051b0: 2020 2020 2020 2020 2020 2020 2073 716c               sql
+000051c0: 616c 6368 656d 792e 496e 6465 7828 226e  alchemy.Index("n
+000051d0: 6f6e 636f 6c5f 6964 785f 706b 222c 206e  oncol_idx_pk", n
+000051e0: 6f6e 636f 6c5f 6964 785f 7465 7374 5f70  oncol_idx_test_p
+000051f0: 6b2e 632e 712e 6465 7363 2829 290a 0a20  k.c.q.desc()).. 
+00005200: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
+00005210: 672e 7265 7175 6972 6573 2e76 6965 775f  g.requires.view_
+00005220: 636f 6c75 6d6e 5f72 6566 6c65 6374 696f  column_reflectio
+00005230: 6e2e 656e 6162 6c65 6420 616e 6420 6e6f  n.enabled and no
+00005240: 7420 626f 6f6c 280a 2020 2020 2020 2020  t bool(.        
+00005250: 2020 2020 6f73 2e65 6e76 6972 6f6e 2e67      os.environ.g
+00005260: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
+00005270: 4154 4f52 5f48 4f53 5422 290a 2020 2020  ATOR_HOST").    
+00005280: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00005290: 2020 2063 6c73 2e64 6566 696e 655f 7669     cls.define_vi
+000052a0: 6577 7328 6d65 7461 6461 7461 2c20 7363  ews(metadata, sc
+000052b0: 6865 6d61 290a 0a20 2020 2040 7465 7374  hema)..    @test
+000052c0: 696e 672e 636f 6d62 696e 6174 696f 6e73  ing.combinations
+000052d0: 280a 2020 2020 2020 2020 2846 616c 7365  (.        (False
+000052e0: 2c20 4661 6c73 6529 2c0a 2020 2020 2020  , False),.      
+000052f0: 2020 2846 616c 7365 2c20 5472 7565 2c20    (False, True, 
+00005300: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
+00005310: 2e73 6368 656d 6173 292c 0a20 2020 2020  .schemas),.     
+00005320: 2020 2028 5472 7565 2c20 4661 6c73 652c     (True, False,
+00005330: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
+00005340: 732e 7669 6577 5f72 6566 6c65 6374 696f  s.view_reflectio
+00005350: 6e29 2c0a 2020 2020 2020 2020 280a 2020  n),.        (.  
+00005360: 2020 2020 2020 2020 2020 5472 7565 2c0a            True,.
+00005370: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00005380: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
+00005390: 7374 696e 672e 7265 7175 6972 6573 2e73  sting.requires.s
+000053a0: 6368 656d 6173 202b 2074 6573 7469 6e67  chemas + testing
+000053b0: 2e72 6571 7569 7265 732e 7669 6577 5f72  .requires.view_r
+000053c0: 6566 6c65 6374 696f 6e2c 0a20 2020 2020  eflection,.     
+000053d0: 2020 2029 2c0a 2020 2020 2020 2020 6172     ),.        ar
+000053e0: 676e 616d 6573 3d22 7573 655f 7669 6577  gnames="use_view
+000053f0: 732c 7573 655f 7363 6865 6d61 222c 0a20  s,use_schema",. 
+00005400: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
+00005410: 745f 6765 745f 636f 6c75 6d6e 7328 7365  t_get_columns(se
+00005420: 6c66 2c20 636f 6e6e 6563 7469 6f6e 2c20  lf, connection, 
+00005430: 7573 655f 7669 6577 732c 2075 7365 5f73  use_views, use_s
+00005440: 6368 656d 6129 3a0a 2020 2020 2020 2020  chema):.        
+00005450: 6966 2075 7365 5f76 6965 7773 2061 6e64  if use_views and
+00005460: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
+00005470: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
+00005480: 554c 4154 4f52 5f48 4f53 5422 2929 3a0a  ULATOR_HOST")):.
+00005490: 2020 2020 2020 2020 2020 2020 7079 7465              pyte
+000054a0: 7374 2e73 6b69 7028 2253 6b69 7070 6564  st.skip("Skipped
+000054b0: 206f 6e20 656d 756c 6174 6f72 2229 0a0a   on emulator")..
+000054c0: 2020 2020 2020 2020 7363 6865 6d61 203d          schema =
+000054d0: 204e 6f6e 650a 0a20 2020 2020 2020 2075   None..        u
+000054e0: 7365 7273 2c20 6164 6472 6573 7365 7320  sers, addresses 
+000054f0: 3d20 2873 656c 662e 7461 626c 6573 2e75  = (self.tables.u
+00005500: 7365 7273 2c20 7365 6c66 2e74 6162 6c65  sers, self.table
+00005510: 732e 656d 6169 6c5f 6164 6472 6573 7365  s.email_addresse
+00005520: 7329 0a20 2020 2020 2020 2069 6620 7573  s).        if us
+00005530: 655f 7669 6577 733a 0a20 2020 2020 2020  e_views:.       
+00005540: 2020 2020 2074 6162 6c65 5f6e 616d 6573       table_names
+00005550: 203d 205b 2275 7365 7273 5f76 222c 2022   = ["users_v", "
+00005560: 656d 6169 6c5f 6164 6472 6573 7365 735f  email_addresses_
+00005570: 7622 2c20 2264 696e 6761 6c69 6e67 735f  v", "dingalings_
+00005580: 7622 5d0a 2020 2020 2020 2020 656c 7365  v"].        else
+00005590: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+000055a0: 626c 655f 6e61 6d65 7320 3d20 5b22 7573  ble_names = ["us
+000055b0: 6572 7322 2c20 2265 6d61 696c 5f61 6464  ers", "email_add
+000055c0: 7265 7373 6573 225d 0a0a 2020 2020 2020  resses"]..      
+000055d0: 2020 696e 7370 203d 2069 6e73 7065 6374    insp = inspect
+000055e0: 2863 6f6e 6e65 6374 696f 6e29 0a20 2020  (connection).   
+000055f0: 2020 2020 2066 6f72 2074 6162 6c65 5f6e       for table_n
+00005600: 616d 652c 2074 6162 6c65 2069 6e20 7a69  ame, table in zi
+00005610: 7028 7461 626c 655f 6e61 6d65 732c 2028  p(table_names, (
+00005620: 7573 6572 732c 2061 6464 7265 7373 6573  users, addresses
+00005630: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00005640: 7363 6865 6d61 5f6e 616d 6520 3d20 7363  schema_name = sc
+00005650: 6865 6d61 0a20 2020 2020 2020 2020 2020  hema.           
+00005660: 2063 6f6c 7320 3d20 696e 7370 2e67 6574   cols = insp.get
+00005670: 5f63 6f6c 756d 6e73 2874 6162 6c65 5f6e  _columns(table_n
+00005680: 616d 652c 2073 6368 656d 613d 7363 6865  ame, schema=sche
+00005690: 6d61 5f6e 616d 6529 0a20 2020 2020 2020  ma_name).       
+000056a0: 2020 2020 2069 735f 7472 7565 286c 656e       is_true(len
+000056b0: 2863 6f6c 7329 203e 2030 2c20 6c65 6e28  (cols) > 0, len(
+000056c0: 636f 6c73 2929 0a0a 2020 2020 2020 2020  cols))..        
+000056d0: 2020 2020 2320 7368 6f75 6c64 2062 6520      # should be 
+000056e0: 696e 206f 7264 6572 0a0a 2020 2020 2020  in order..      
+000056f0: 2020 2020 2020 666f 7220 692c 2063 6f6c        for i, col
+00005700: 2069 6e20 656e 756d 6572 6174 6528 7461   in enumerate(ta
+00005710: 626c 652e 636f 6c75 6d6e 7329 3a0a 2020  ble.columns):.  
+00005720: 2020 2020 2020 2020 2020 2020 2020 6571                eq
+00005730: 5f28 636f 6c2e 6e61 6d65 2c20 636f 6c73  _(col.name, cols
+00005740: 5b69 5d5b 226e 616d 6522 5d29 0a20 2020  [i]["name"]).   
+00005750: 2020 2020 2020 2020 2020 2020 2063 7479               cty
+00005760: 7065 203d 2063 6f6c 735b 695d 5b22 7479  pe = cols[i]["ty
+00005770: 7065 225d 2e5f 5f63 6c61 7373 5f5f 0a20  pe"].__class__. 
+00005780: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005790: 7479 7065 5f64 6566 203d 2063 6f6c 2e74  type_def = col.t
+000057a0: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
+000057b0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000057c0: 6528 6374 7970 655f 6465 662c 2073 716c  e(ctype_def, sql
+000057d0: 616c 6368 656d 792e 7479 7065 732e 5479  alchemy.types.Ty
+000057e0: 7065 456e 6769 6e65 293a 0a20 2020 2020  peEngine):.     
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005800: 7479 7065 5f64 6566 203d 2063 7479 7065  type_def = ctype
+00005810: 5f64 6566 2e5f 5f63 6c61 7373 5f5f 0a0a  _def.__class__..
+00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005830: 2320 4f72 6163 6c65 2072 6574 7572 6e73  # Oracle returns
+00005840: 2044 6174 6520 666f 7220 4461 7465 5469   Date for DateTi
+00005850: 6d65 2e0a 0a20 2020 2020 2020 2020 2020  me...           
+00005860: 2020 2020 2069 6620 7465 7374 696e 672e       if testing.
+00005870: 6167 6169 6e73 7428 226f 7261 636c 6522  against("oracle"
+00005880: 2920 616e 6420 6374 7970 655f 6465 6620  ) and ctype_def 
+00005890: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
+000058a0: 2020 2020 2020 2020 2074 7970 6573 2e44           types.D
+000058b0: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
+000058c0: 2020 2020 2020 2020 2074 7970 6573 2e44           types.D
+000058d0: 6174 6554 696d 652c 0a20 2020 2020 2020  ateTime,.       
+000058e0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 6374 7970 655f 6465 6620 3d20 7479 7065  ctype_def = type
+00005910: 732e 4461 7465 0a0a 2020 2020 2020 2020  s.Date..        
+00005920: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
+00005930: 2074 6861 7420 7468 6520 6465 7369 7265   that the desire
+00005940: 6420 7479 7065 2061 6e64 2072 6574 7572  d type and retur
+00005950: 6e20 7479 7065 2073 6861 7265 0a20 2020  n type share.   
+00005960: 2020 2020 2020 2020 2020 2020 2023 2061               # a
+00005970: 2062 6173 6520 7769 7468 696e 206f 6e65   base within one
+00005980: 206f 6620 7468 6520 6765 6e65 7269 6320   of the generic 
+00005990: 7479 7065 732e 0a0a 2020 2020 2020 2020  types...        
+000059a0: 2020 2020 2020 2020 6973 5f74 7275 6528          is_true(
+000059b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059c0: 2020 2020 206c 656e 280a 2020 2020 2020       len(.      
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059e0: 2020 7365 7428 6374 7970 652e 5f5f 6d72    set(ctype.__mr
+000059f0: 6f5f 5f29 0a20 2020 2020 2020 2020 2020  o__).           
+00005a00: 2020 2020 2020 2020 2020 2020 202e 696e               .in
+00005a10: 7465 7273 6563 7469 6f6e 2863 7479 7065  tersection(ctype
+00005a20: 5f64 6566 2e5f 5f6d 726f 5f5f 290a 2020  _def.__mro__).  
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 2020 2020 2020 2e69 6e74 6572 7365 6374        .intersect
+00005a50: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
 00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a70: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00005a80: 7065 732e 496e 7465 6765 722c 0a20 2020  pes.Integer,.   
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005aa0: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00005ab0: 6573 2e4e 756d 6572 6963 2c0a 2020 2020  es.Numeric,.    
-00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ad0: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00005ae0: 732e 4461 7465 5469 6d65 2c0a 2020 2020  s.DateTime,.    
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00005b10: 732e 4461 7465 2c0a 2020 2020 2020 2020  s.Date,.        
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 2020 2020 2020 7479 7065 732e 5469          types.Ti
-00005b40: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 7479 7065 732e 5374 7269 6e67      types.String
-00005b70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2020 7479 7065 732e 5f42 696e 6172 792c    types._Binary,
-00005ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005bb0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+00005a70: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2074 7970 6573 2e49 6e74 6567 6572     types.Integer
+00005aa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 2020 7479 7065 732e 4e75 6d65 7269 632c    types.Numeric,
+00005ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005af0: 2074 7970 6573 2e44 6174 6554 696d 652c   types.DateTime,
+00005b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b20: 2074 7970 6573 2e44 6174 652c 0a20 2020   types.Date,.   
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b40: 2020 2020 2020 2020 2020 2020 2074 7970               typ
+00005b50: 6573 2e54 696d 652c 0a20 2020 2020 2020  es.Time,.       
+00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b70: 2020 2020 2020 2020 2074 7970 6573 2e53           types.S
+00005b80: 7472 696e 672c 0a20 2020 2020 2020 2020  tring,.         
+00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ba0: 2020 2020 2020 2074 7970 6573 2e5f 4269         types._Bi
+00005bb0: 6e61 7279 2c0a 2020 2020 2020 2020 2020  nary,.          
 00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005be0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00005bd0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00005be0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 203e 2030 2c0a 2020 2020 2020 2020     > 0,.        
-00005c10: 2020 2020 2020 2020 2020 2020 2225 7328              "%s(
-00005c20: 2573 292c 2025 7328 2573 2922 2025 2028  %s), %s(%s)" % (
-00005c30: 636f 6c2e 6e61 6d65 2c20 636f 6c2e 7479  col.name, col.ty
-00005c40: 7065 2c20 636f 6c73 5b69 5d5b 226e 616d  pe, cols[i]["nam
-00005c50: 6522 5d2c 2063 7479 7065 292c 0a20 2020  e"], ctype),.   
-00005c60: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 6966 206e 6f74 2063 6f6c 2e70 7269 6d61  if not col.prima
-00005c90: 7279 5f6b 6579 3a0a 2020 2020 2020 2020  ry_key:.        
-00005ca0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00005cb0: 7274 2063 6f6c 735b 695d 5b22 6465 6661  rt cols[i]["defa
-00005cc0: 756c 7422 5d20 6973 204e 6f6e 650a 0a20  ult"] is None.. 
-00005cd0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00005ce0: 736b 6970 6966 280a 2020 2020 2020 2020  skipif(.        
-00005cf0: 626f 6f6c 286f 732e 656e 7669 726f 6e2e  bool(os.environ.
-00005d00: 6765 7428 2253 5041 4e4e 4552 5f45 4d55  get("SPANNER_EMU
-00005d10: 4c41 544f 525f 484f 5354 2229 292c 2072  LATOR_HOST")), r
-00005d20: 6561 736f 6e3d 2253 6b69 7070 6564 206f  eason="Skipped o
-00005d30: 6e20 656d 756c 6174 6f72 220a 2020 2020  n emulator".    
-00005d40: 290a 2020 2020 4074 6573 7469 6e67 2e72  ).    @testing.r
-00005d50: 6571 7569 7265 732e 7669 6577 5f72 6566  equires.view_ref
-00005d60: 6c65 6374 696f 6e0a 2020 2020 6465 6620  lection.    def 
-00005d70: 7465 7374 5f67 6574 5f76 6965 775f 6465  test_get_view_de
-00005d80: 6669 6e69 7469 6f6e 280a 2020 2020 2020  finition(.      
-00005d90: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00005da0: 636f 6e6e 6563 7469 6f6e 2c0a 2020 2020  connection,.    
-00005db0: 293a 0a20 2020 2020 2020 2073 6368 656d  ):.        schem
-00005dc0: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
-00005dd0: 2069 6e73 7020 3d20 696e 7370 6563 7428   insp = inspect(
-00005de0: 636f 6e6e 6563 7469 6f6e 290a 2020 2020  connection).    
-00005df0: 2020 2020 666f 7220 7669 6577 2069 6e20      for view in 
-00005e00: 5b22 7573 6572 735f 7622 2c20 2265 6d61  ["users_v", "ema
-00005e10: 696c 5f61 6464 7265 7373 6573 5f76 222c  il_addresses_v",
-00005e20: 2022 6469 6e67 616c 696e 6773 5f76 225d   "dingalings_v"]
-00005e30: 3a0a 2020 2020 2020 2020 2020 2020 7620  :.            v 
-00005e40: 3d20 696e 7370 2e67 6574 5f76 6965 775f  = insp.get_view_
-00005e50: 6465 6669 6e69 7469 6f6e 2876 6965 772c  definition(view,
-00005e60: 2073 6368 656d 613d 7363 6865 6d61 290a   schema=schema).
-00005e70: 2020 2020 2020 2020 2020 2020 6973 5f74              is_t
-00005e80: 7275 6528 626f 6f6c 2876 2929 0a0a 2020  rue(bool(v))..  
-00005e90: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00005ea0: 6b69 7069 6628 0a20 2020 2020 2020 2062  kipif(.        b
-00005eb0: 6f6f 6c28 6f73 2e65 6e76 6972 6f6e 2e67  ool(os.environ.g
-00005ec0: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
-00005ed0: 4154 4f52 5f48 4f53 5422 2929 2c20 7265  ATOR_HOST")), re
-00005ee0: 6173 6f6e 3d22 536b 6970 7065 6420 6f6e  ason="Skipped on
-00005ef0: 2065 6d75 6c61 746f 7222 0a20 2020 2029   emulator".    )
-00005f00: 0a20 2020 2040 7465 7374 696e 672e 7265  .    @testing.re
-00005f10: 7175 6972 6573 2e76 6965 775f 7265 666c  quires.view_refl
-00005f20: 6563 7469 6f6e 0a20 2020 2064 6566 2074  ection.    def t
-00005f30: 6573 745f 6765 745f 7669 6577 5f64 6566  est_get_view_def
-00005f40: 696e 6974 696f 6e5f 646f 6573 5f6e 6f74  inition_does_not
-00005f50: 5f65 7869 7374 2873 656c 662c 2063 6f6e  _exist(self, con
-00005f60: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-00005f70: 2020 7375 7065 7228 292e 7465 7374 5f67    super().test_g
-00005f80: 6574 5f76 6965 775f 6465 6669 6e69 7469  et_view_definiti
-00005f90: 6f6e 5f64 6f65 735f 6e6f 745f 6578 6973  on_does_not_exis
-00005fa0: 7428 636f 6e6e 6563 7469 6f6e 290a 0a20  t(connection).. 
-00005fb0: 2020 2064 6566 2066 696c 7465 725f 6e61     def filter_na
-00005fc0: 6d65 5f76 616c 7565 7328 293a 0a20 2020  me_values():.   
-00005fd0: 2020 2020 2072 6574 7572 6e20 7465 7374       return test
-00005fe0: 696e 672e 636f 6d62 696e 6174 696f 6e73  ing.combinations
-00005ff0: 2854 7275 652c 2046 616c 7365 2c20 6172  (True, False, ar
-00006000: 676e 616d 6573 3d22 7573 655f 6669 6c74  gnames="use_filt
-00006010: 6572 2229 0a0a 2020 2020 4066 696c 7465  er")..    @filte
-00006020: 725f 6e61 6d65 5f76 616c 7565 7328 290a  r_name_values().
-00006030: 2020 2020 4074 6573 7469 6e67 2e72 6571      @testing.req
-00006040: 7569 7265 732e 696e 6465 785f 7265 666c  uires.index_refl
-00006050: 6563 7469 6f6e 0a20 2020 2064 6566 2074  ection.    def t
-00006060: 6573 745f 6765 745f 6d75 6c74 695f 696e  est_get_multi_in
-00006070: 6465 7865 7328 0a20 2020 2020 2020 2073  dexes(.        s
-00006080: 656c 662c 0a20 2020 2020 2020 2067 6574  elf,.        get
-00006090: 5f6d 756c 7469 5f65 7870 2c0a 2020 2020  _multi_exp,.    
-000060a0: 2020 2020 7573 655f 6669 6c74 6572 2c0a      use_filter,.
-000060b0: 2020 2020 2020 2020 7363 6865 6d61 3d4e          schema=N
-000060c0: 6f6e 652c 0a20 2020 2020 2020 2073 636f  one,.        sco
-000060d0: 7065 3d4f 626a 6563 7453 636f 7065 2e44  pe=ObjectScope.D
-000060e0: 4546 4155 4c54 2c0a 2020 2020 2020 2020  EFAULT,.        
-000060f0: 6b69 6e64 3d4f 626a 6563 744b 696e 642e  kind=ObjectKind.
-00006100: 5441 424c 452c 0a20 2020 2029 3a0a 2020  TABLE,.    ):.  
-00006110: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006120: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-00006130: 4445 3a0a 0a20 2020 2020 2020 2053 7061  DE:..        Spa
-00006140: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-00006150: 706f 7274 2069 6e64 6578 6573 206f 6e20  port indexes on 
-00006160: 7669 6577 7320 616e 640a 2020 2020 2020  views and.      
-00006170: 2020 646f 6573 6e27 7420 7375 7070 6f72    doesn't suppor
-00006180: 7420 7465 6d70 6f72 6172 7920 7461 626c  t temporary tabl
-00006190: 6573 2c20 736f 2072 6561 6c20 7461 626c  es, so real tabl
-000061a0: 6573 2061 7265 0a20 2020 2020 2020 2075  es are.        u
-000061b0: 7365 6420 666f 7220 7465 7374 696e 672e  sed for testing.
-000061c0: 2041 7320 7468 6520 6f72 6967 696e 616c   As the original
-000061d0: 2074 6573 7420 6578 7065 6374 7320 6f6e   test expects on
-000061e0: 6c79 2072 6561 6c0a 2020 2020 2020 2020  ly real.        
-000061f0: 7461 626c 6573 2074 6f20 6265 2072 6561  tables to be rea
-00006200: 642c 2061 6e64 2069 6e20 5370 616e 6e65  d, and in Spanne
-00006210: 7220 616c 6c20 7468 6520 7461 626c 6573  r all the tables
-00006220: 2061 7265 2072 6561 6c2c 0a20 2020 2020   are real,.     
-00006230: 2020 2065 7870 6563 7465 6420 7265 7375     expected resu
-00006240: 6c74 7320 6f76 6572 7269 6465 2069 7320  lts override is 
-00006250: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
-00006260: 2020 2222 220a 2020 2020 2020 2020 696e    """.        in
-00006270: 7370 2c20 6b77 732c 2065 7870 203d 2067  sp, kws, exp = g
-00006280: 6574 5f6d 756c 7469 5f65 7870 280a 2020  et_multi_exp(.  
-00006290: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-000062a0: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
-000062b0: 6f70 652c 0a20 2020 2020 2020 2020 2020  ope,.           
-000062c0: 206b 696e 642c 0a20 2020 2020 2020 2020   kind,.         
-000062d0: 2020 2075 7365 5f66 696c 7465 722c 0a20     use_filter,. 
-000062e0: 2020 2020 2020 2020 2020 2049 6e73 7065             Inspe
-000062f0: 6374 6f72 2e67 6574 5f69 6e64 6578 6573  ctor.get_indexes
-00006300: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00006310: 6c66 2e65 7870 5f69 6e64 6578 6573 2c0a  lf.exp_indexes,.
-00006320: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006330: 2020 5f69 676e 6f72 655f 7461 626c 6573    _ignore_tables
-00006340: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00006350: 2028 4e6f 6e65 2c20 2263 6f6d 6d65 6e74   (None, "comment
-00006360: 5f74 6573 7422 292c 0a20 2020 2020 2020  _test"),.       
-00006370: 2020 2020 2028 4e6f 6e65 2c20 2264 696e       (None, "din
-00006380: 6761 6c69 6e67 7322 292c 0a20 2020 2020  galings"),.     
-00006390: 2020 2020 2020 2028 4e6f 6e65 2c20 2265         (None, "e
-000063a0: 6d61 696c 5f61 6464 7265 7373 6573 2229  mail_addresses")
-000063b0: 2c0a 2020 2020 2020 2020 2020 2020 284e  ,.            (N
-000063c0: 6f6e 652c 2022 6e6f 5f63 6f6e 7374 7261  one, "no_constra
-000063d0: 696e 7473 2229 2c0a 2020 2020 2020 2020  ints"),.        
-000063e0: 5d0a 2020 2020 2020 2020 6578 7020 3d20  ].        exp = 
-000063f0: 7b6b 3a20 7620 666f 7220 6b2c 2076 2069  {k: v for k, v i
-00006400: 6e20 6578 702e 6974 656d 7328 2920 6966  n exp.items() if
-00006410: 206b 206e 6f74 2069 6e20 5f69 676e 6f72   k not in _ignor
-00006420: 655f 7461 626c 6573 7d0a 0a20 2020 2020  e_tables}..     
-00006430: 2020 2066 6f72 206b 7720 696e 206b 7773     for kw in kws
-00006440: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-00006450: 7370 2e63 6c65 6172 5f63 6163 6865 2829  sp.clear_cache()
-00006460: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006470: 756c 7420 3d20 696e 7370 2e67 6574 5f6d  ult = insp.get_m
-00006480: 756c 7469 5f69 6e64 6578 6573 282a 2a6b  ulti_indexes(**k
-00006490: 7729 0a20 2020 2020 2020 2020 2020 2073  w).            s
-000064a0: 656c 662e 5f63 6865 636b 5f74 6162 6c65  elf._check_table
-000064b0: 5f64 6963 7428 7265 7375 6c74 2c20 6578  _dict(result, ex
-000064c0: 702c 2073 656c 662e 5f72 6571 7569 7265  p, self._require
-000064d0: 645f 696e 6465 785f 6b65 7973 290a 0a20  d_index_keys).. 
-000064e0: 2020 2064 6566 2065 7870 5f70 6b73 280a     def exp_pks(.
-000064f0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00006500: 2020 2020 2020 7363 6865 6d61 3d4e 6f6e        schema=Non
-00006510: 652c 0a20 2020 2020 2020 2073 636f 7065  e,.        scope
-00006520: 3d4f 626a 6563 7453 636f 7065 2e41 4e59  =ObjectScope.ANY
-00006530: 2c0a 2020 2020 2020 2020 6b69 6e64 3d4f  ,.        kind=O
-00006540: 626a 6563 744b 696e 642e 414e 592c 0a20  bjectKind.ANY,. 
-00006550: 2020 2020 2020 2066 696c 7465 725f 6e61         filter_na
-00006560: 6d65 733d 4e6f 6e65 2c0a 2020 2020 293a  mes=None,.    ):
-00006570: 0a20 2020 2020 2020 2064 6566 2070 6b28  .        def pk(
-00006580: 2a63 6f6c 732c 206e 616d 653d 6d6f 636b  *cols, name=mock
-00006590: 2e41 4e59 2c20 636f 6d6d 656e 743d 4e6f  .ANY, comment=No
-000065a0: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
-000065b0: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-000065c0: 2020 2020 2020 2020 2020 2263 6f6e 7374            "const
-000065d0: 7261 696e 6564 5f63 6f6c 756d 6e73 223a  rained_columns":
-000065e0: 206c 6973 7428 636f 6c73 292c 0a20 2020   list(cols),.   
-000065f0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00006600: 6d65 223a 206e 616d 652c 0a20 2020 2020  me": name,.     
-00006610: 2020 2020 2020 2020 2020 2022 636f 6d6d             "comm
-00006620: 656e 7422 3a20 636f 6d6d 656e 742c 0a20  ent": comment,. 
-00006630: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
-00006640: 2020 2020 2020 656d 7074 7920 3d20 706b        empty = pk
-00006650: 286e 616d 653d 4e6f 6e65 290a 2020 2020  (name=None).    
-00006660: 2020 2020 6966 2074 6573 7469 6e67 2e72      if testing.r
-00006670: 6571 7569 7265 732e 6d61 7465 7269 616c  equires.material
-00006680: 697a 6564 5f76 6965 7773 5f72 6566 6c65  ized_views_refle
-00006690: 6374 5f70 6b2e 656e 6162 6c65 643a 0a20  ct_pk.enabled:. 
-000066a0: 2020 2020 2020 2020 2020 206d 6174 6572             mater
-000066b0: 6961 6c69 7a65 6420 3d20 7b28 7363 6865  ialized = {(sche
-000066c0: 6d61 2c20 2264 696e 6761 6c69 6e67 735f  ma, "dingalings_
-000066d0: 7622 293a 2070 6b28 2264 696e 6761 6c69  v"): pk("dingali
-000066e0: 6e67 5f69 6422 297d 0a20 2020 2020 2020  ng_id")}.       
-000066f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00006700: 2020 206d 6174 6572 6961 6c69 7a65 6420     materialized 
-00006710: 3d20 7b28 7363 6865 6d61 2c20 2264 696e  = {(schema, "din
-00006720: 6761 6c69 6e67 735f 7622 293a 2065 6d70  galings_v"): emp
-00006730: 7479 7d0a 2020 2020 2020 2020 7669 6577  ty}.        view
-00006740: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-00006750: 2020 2873 6368 656d 612c 2022 656d 6169    (schema, "emai
-00006760: 6c5f 6164 6472 6573 7365 735f 7622 293a  l_addresses_v"):
-00006770: 2065 6d70 7479 2c0a 2020 2020 2020 2020   empty,.        
-00006780: 2020 2020 2873 6368 656d 612c 2022 7573      (schema, "us
-00006790: 6572 735f 7622 293a 2065 6d70 7479 2c0a  ers_v"): empty,.
-000067a0: 2020 2020 2020 2020 2020 2020 2873 6368              (sch
-000067b0: 656d 612c 2022 7573 6572 5f74 6d70 5f76  ema, "user_tmp_v
-000067c0: 2229 3a20 656d 7074 792c 0a20 2020 2020  "): empty,.     
-000067d0: 2020 207d 0a20 2020 2020 2020 2073 656c     }.        sel
-000067e0: 662e 5f72 6573 6f6c 7665 5f76 6965 7773  f._resolve_views
-000067f0: 2876 6965 7773 2c20 6d61 7465 7269 616c  (views, material
-00006800: 697a 6564 290a 2020 2020 2020 2020 7461  ized).        ta
-00006810: 626c 6573 203d 207b 0a20 2020 2020 2020  bles = {.       
-00006820: 2020 2020 2028 7363 6865 6d61 2c20 2275       (schema, "u
-00006830: 7365 7273 2229 3a20 706b 2822 7573 6572  sers"): pk("user
-00006840: 5f69 6422 292c 0a20 2020 2020 2020 2020  _id"),.         
-00006850: 2020 2028 7363 6865 6d61 2c20 2264 696e     (schema, "din
-00006860: 6761 6c69 6e67 7322 293a 2070 6b28 2264  galings"): pk("d
-00006870: 696e 6761 6c69 6e67 5f69 6422 292c 0a20  ingaling_id"),. 
-00006880: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
-00006890: 6d61 2c20 2265 6d61 696c 5f61 6464 7265  ma, "email_addre
-000068a0: 7373 6573 2229 3a20 706b 280a 2020 2020  sses"): pk(.    
-000068b0: 2020 2020 2020 2020 2020 2020 2261 6464              "add
-000068c0: 7265 7373 5f69 6422 2c20 6e61 6d65 3d22  ress_id", name="
-000068d0: 656d 6169 6c5f 6164 5f70 6b22 2c20 636f  email_ad_pk", co
-000068e0: 6d6d 656e 743d 2265 6120 706b 2063 6f6d  mment="ea pk com
-000068f0: 6d65 6e74 220a 2020 2020 2020 2020 2020  ment".          
-00006900: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00006910: 2028 7363 6865 6d61 2c20 2263 6f6d 6d65   (schema, "comme
-00006920: 6e74 5f74 6573 7422 293a 2070 6b28 2269  nt_test"): pk("i
-00006930: 6422 292c 0a20 2020 2020 2020 2020 2020  d"),.           
-00006940: 2028 7363 6865 6d61 2c20 226e 6f5f 636f   (schema, "no_co
-00006950: 6e73 7472 6169 6e74 7322 293a 2065 6d70  nstraints"): emp
-00006960: 7479 2c0a 2020 2020 2020 2020 2020 2020  ty,.            
-00006970: 2873 6368 656d 612c 2022 6c6f 6361 6c5f  (schema, "local_
-00006980: 7461 626c 6522 293a 2070 6b28 2269 6422  table"): pk("id"
-00006990: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000069a0: 7363 6865 6d61 2c20 2272 656d 6f74 655f  schema, "remote_
-000069b0: 7461 626c 6522 293a 2070 6b28 2269 6422  table"): pk("id"
-000069c0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000069d0: 7363 6865 6d61 2c20 2272 656d 6f74 655f  schema, "remote_
-000069e0: 7461 626c 655f 3222 293a 2070 6b28 2269  table_2"): pk("i
-000069f0: 6422 292c 0a20 2020 2020 2020 2020 2020  d"),.           
-00006a00: 2028 7363 6865 6d61 2c20 226e 6f6e 636f   (schema, "nonco
-00006a10: 6c5f 6964 785f 7465 7374 5f6e 6f70 6b22  l_idx_test_nopk"
-00006a20: 293a 2070 6b28 2269 6422 292c 0a20 2020  ): pk("id"),.   
-00006a30: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
-00006a40: 2c20 226e 6f6e 636f 6c5f 6964 785f 7465  , "noncol_idx_te
-00006a50: 7374 5f70 6b22 293a 2070 6b28 2269 6422  st_pk"): pk("id"
-00006a60: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00006a70: 7363 6865 6d61 2c20 7365 6c66 2e74 656d  schema, self.tem
-00006a80: 705f 7461 626c 655f 6e61 6d65 2829 293a  p_table_name()):
-00006a90: 2070 6b28 2269 6422 292c 0a20 2020 2020   pk("id"),.     
-00006aa0: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
-00006ab0: 6e6f 7420 7465 7374 696e 672e 7265 7175  not testing.requ
-00006ac0: 6972 6573 2e72 6566 6c65 6374 735f 706b  ires.reflects_pk
-00006ad0: 5f6e 616d 6573 2e65 6e61 626c 6564 3a0a  _names.enabled:.
-00006ae0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00006af0: 7661 6c20 696e 2074 6162 6c65 732e 7661  val in tables.va
-00006b00: 6c75 6573 2829 3a0a 2020 2020 2020 2020  lues():.        
-00006b10: 2020 2020 2020 2020 6966 2076 616c 5b22          if val["
-00006b20: 6e61 6d65 225d 2069 7320 6e6f 7420 4e6f  name"] is not No
-00006b30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006b40: 2020 2020 2020 2020 7661 6c5b 226e 616d          val["nam
-00006b50: 6522 5d20 3d20 6d6f 636b 2e41 4e59 0a20  e"] = mock.ANY. 
-00006b60: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-00006b70: 662e 5f72 6573 6f6c 7665 5f6b 696e 6428  f._resolve_kind(
-00006b80: 6b69 6e64 2c20 7461 626c 6573 2c20 7669  kind, tables, vi
-00006b90: 6577 732c 206d 6174 6572 6961 6c69 7a65  ews, materialize
-00006ba0: 6429 0a20 2020 2020 2020 2072 6573 203d  d).        res =
-00006bb0: 2073 656c 662e 5f72 6573 6f6c 7665 5f6e   self._resolve_n
-00006bc0: 616d 6573 2873 6368 656d 612c 2073 636f  ames(schema, sco
-00006bd0: 7065 2c20 6669 6c74 6572 5f6e 616d 6573  pe, filter_names
-00006be0: 2c20 7265 7329 0a20 2020 2020 2020 2072  , res).        r
-00006bf0: 6574 7572 6e20 7265 730a 0a20 2020 2040  eturn res..    @
-00006c00: 6669 6c74 6572 5f6e 616d 655f 7661 6c75  filter_name_valu
-00006c10: 6573 2829 0a20 2020 2040 7465 7374 696e  es().    @testin
-00006c20: 672e 7265 7175 6972 6573 2e70 7269 6d61  g.requires.prima
-00006c30: 7279 5f6b 6579 5f63 6f6e 7374 7261 696e  ry_key_constrain
-00006c40: 745f 7265 666c 6563 7469 6f6e 0a20 2020  t_reflection.   
-00006c50: 2064 6566 2074 6573 745f 6765 745f 6d75   def test_get_mu
-00006c60: 6c74 695f 706b 5f63 6f6e 7374 7261 696e  lti_pk_constrain
-00006c70: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-00006c80: 0a20 2020 2020 2020 2067 6574 5f6d 756c  .        get_mul
-00006c90: 7469 5f65 7870 2c0a 2020 2020 2020 2020  ti_exp,.        
-00006ca0: 7573 655f 6669 6c74 6572 2c0a 2020 2020  use_filter,.    
-00006cb0: 2020 2020 7363 6865 6d61 3d4e 6f6e 652c      schema=None,
-00006cc0: 0a20 2020 2020 2020 2073 636f 7065 3d4f  .        scope=O
-00006cd0: 626a 6563 7453 636f 7065 2e44 4546 4155  bjectScope.DEFAU
-00006ce0: 4c54 2c0a 2020 2020 2020 2020 6b69 6e64  LT,.        kind
-00006cf0: 3d4f 626a 6563 744b 696e 642e 5441 424c  =ObjectKind.TABL
-00006d00: 452c 0a20 2020 2029 3a0a 2020 2020 2020  E,.    ):.      
-00006d10: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-00006d20: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-00006d30: 0a20 2020 2020 2020 2053 7061 6e6e 6572  .        Spanner
-00006d40: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-00006d50: 2074 656d 706f 7261 7279 2074 6162 6c65   temporary table
-00006d60: 732c 2073 6f20 7265 616c 2074 6162 6c65  s, so real table
-00006d70: 7320 6172 650a 2020 2020 2020 2020 7573  s are.        us
-00006d80: 6564 2066 6f72 2074 6573 7469 6e67 2e20  ed for testing. 
-00006d90: 4173 2074 6865 206f 7269 6769 6e61 6c20  As the original 
-00006da0: 7465 7374 2065 7870 6563 7473 206f 6e6c  test expects onl
-00006db0: 7920 7265 616c 0a20 2020 2020 2020 2074  y real.        t
-00006dc0: 6162 6c65 7320 746f 2062 6520 7265 6164  ables to be read
-00006dd0: 2c20 616e 6420 696e 2053 7061 6e6e 6572  , and in Spanner
-00006de0: 2061 6c6c 2074 6865 2074 6162 6c65 7320   all the tables 
-00006df0: 6172 6520 7265 616c 2c0a 2020 2020 2020  are real,.      
-00006e00: 2020 6578 7065 6374 6564 2072 6573 756c    expected resul
-00006e10: 7473 206f 7665 7272 6964 6520 6973 2072  ts override is r
-00006e20: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
-00006e30: 2022 2222 0a20 2020 2020 2020 2069 6e73   """.        ins
-00006e40: 702c 206b 7773 2c20 6578 7020 3d20 6765  p, kws, exp = ge
-00006e50: 745f 6d75 6c74 695f 6578 7028 0a20 2020  t_multi_exp(.   
-00006e60: 2020 2020 2020 2020 2073 6368 656d 612c           schema,
-00006e70: 0a20 2020 2020 2020 2020 2020 2073 636f  .            sco
-00006e80: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00006e90: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
-00006ea0: 2020 7573 655f 6669 6c74 6572 2c0a 2020    use_filter,.  
-00006eb0: 2020 2020 2020 2020 2020 496e 7370 6563            Inspec
-00006ec0: 746f 722e 6765 745f 706b 5f63 6f6e 7374  tor.get_pk_const
-00006ed0: 7261 696e 742c 0a20 2020 2020 2020 2020  raint,.         
-00006ee0: 2020 2073 656c 662e 6578 705f 706b 732c     self.exp_pks,
-00006ef0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00006f00: 2020 205f 6967 6e6f 7265 5f74 6162 6c65     _ignore_table
-00006f10: 7320 3d20 5b28 4e6f 6e65 2c20 226e 6f5f  s = [(None, "no_
-00006f20: 636f 6e73 7472 6169 6e74 7322 295d 0a20  constraints")]. 
-00006f30: 2020 2020 2020 2065 7870 203d 207b 6b3a         exp = {k:
-00006f40: 2076 2066 6f72 206b 2c20 7620 696e 2065   v for k, v in e
-00006f50: 7870 2e69 7465 6d73 2829 2069 6620 6b20  xp.items() if k 
-00006f60: 6e6f 7420 696e 205f 6967 6e6f 7265 5f74  not in _ignore_t
-00006f70: 6162 6c65 737d 0a0a 2020 2020 2020 2020  ables}..        
-00006f80: 666f 7220 6b77 2069 6e20 6b77 733a 0a20  for kw in kws:. 
-00006f90: 2020 2020 2020 2020 2020 2069 6e73 702e             insp.
-00006fa0: 636c 6561 725f 6361 6368 6528 290a 2020  clear_cache().  
-00006fb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00006fc0: 203d 2069 6e73 702e 6765 745f 6d75 6c74   = insp.get_mult
-00006fd0: 695f 706b 5f63 6f6e 7374 7261 696e 7428  i_pk_constraint(
-00006fe0: 2a2a 6b77 290a 2020 2020 2020 2020 2020  **kw).          
-00006ff0: 2020 7365 6c66 2e5f 6368 6563 6b5f 7461    self._check_ta
-00007000: 626c 655f 6469 6374 2872 6573 756c 742c  ble_dict(result,
-00007010: 2065 7870 2c20 7365 6c66 2e5f 7265 7175   exp, self._requ
-00007020: 6972 6564 5f70 6b5f 6b65 7973 2c20 6d61  ired_pk_keys, ma
-00007030: 6b65 5f6c 6973 7473 3d54 7275 6529 0a0a  ke_lists=True)..
-00007040: 2020 2020 6465 6620 6578 705f 666b 7328      def exp_fks(
-00007050: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00007060: 2020 2020 2020 2073 6368 656d 613d 4e6f         schema=No
-00007070: 6e65 2c0a 2020 2020 2020 2020 7363 6f70  ne,.        scop
-00007080: 653d 4f62 6a65 6374 5363 6f70 652e 414e  e=ObjectScope.AN
-00007090: 592c 0a20 2020 2020 2020 206b 696e 643d  Y,.        kind=
-000070a0: 4f62 6a65 6374 4b69 6e64 2e41 4e59 2c0a  ObjectKind.ANY,.
-000070b0: 2020 2020 2020 2020 6669 6c74 6572 5f6e          filter_n
-000070c0: 616d 6573 3d4e 6f6e 652c 0a20 2020 2029  ames=None,.    )
-000070d0: 3a0a 2020 2020 2020 2020 636c 6173 7320  :.        class 
-000070e0: 7474 3a0a 2020 2020 2020 2020 2020 2020  tt:.            
-000070f0: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-00007100: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00007110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007120: 6f74 6865 7220 6973 204e 6f6e 6520 6f72  other is None or
-00007130: 2063 6f6e 6669 672e 6462 2e64 6961 6c65   config.db.diale
-00007140: 6374 2e64 6566 6175 6c74 5f73 6368 656d  ct.default_schem
-00007150: 615f 6e61 6d65 203d 3d20 6f74 6865 720a  a_name == other.
-00007160: 0a20 2020 2020 2020 2064 6566 2066 6b28  .        def fk(
-00007170: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00007180: 732c 0a20 2020 2020 2020 2020 2020 2072  s,.            r
-00007190: 6566 5f63 6f6c 2c0a 2020 2020 2020 2020  ef_col,.        
-000071a0: 2020 2020 7265 665f 7461 626c 652c 0a20      ref_table,. 
-000071b0: 2020 2020 2020 2020 2020 2072 6566 5f73             ref_s
-000071c0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
-000071d0: 2020 2020 2020 2020 2020 6e61 6d65 3d6d            name=m
-000071e0: 6f63 6b2e 414e 592c 0a20 2020 2020 2020  ock.ANY,.       
-000071f0: 2020 2020 2063 6f6d 6d65 6e74 3d4e 6f6e       comment=Non
-00007200: 652c 0a20 2020 2020 2020 2029 3a0a 2020  e,.        ):.  
-00007210: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007220: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00007230: 2020 2022 636f 6e73 7472 6169 6e65 645f     "constrained_
-00007240: 636f 6c75 6d6e 7322 3a20 636f 6c73 2c0a  columns": cols,.
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2272 6566 6572 7265 645f 636f 6c75 6d6e  "referred_column
-00007270: 7322 3a20 7265 665f 636f 6c2c 0a20 2020  s": ref_col,.   
-00007280: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00007290: 6d65 223a 206e 616d 652c 0a20 2020 2020  me": name,.     
-000072a0: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
-000072b0: 6f6e 7322 3a20 6d6f 636b 2e41 4e59 2c0a  ons": mock.ANY,.
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2272 6566 6572 7265 645f 7363 6865 6d61  "referred_schema
-000072e0: 223a 2072 6566 5f73 6368 656d 6120 6966  ": ref_schema if
-000072f0: 2072 6566 5f73 6368 656d 6120 6973 206e   ref_schema is n
-00007300: 6f74 204e 6f6e 6520 656c 7365 2074 7428  ot None else tt(
-00007310: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00007320: 2020 2022 7265 6665 7272 6564 5f74 6162     "referred_tab
-00007330: 6c65 223a 2072 6566 5f74 6162 6c65 2c0a  le": ref_table,.
-00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2263 6f6d 6d65 6e74 223a 2063 6f6d 6d65  "comment": comme
-00007360: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-00007370: 7d0a 0a20 2020 2020 2020 206d 6174 6572  }..        mater
-00007380: 6961 6c69 7a65 6420 3d20 7b7d 0a20 2020  ialized = {}.   
-00007390: 2020 2020 2076 6965 7773 203d 207b 7d0a       views = {}.
-000073a0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-000073b0: 736f 6c76 655f 7669 6577 7328 7669 6577  solve_views(view
-000073c0: 732c 206d 6174 6572 6961 6c69 7a65 6429  s, materialized)
-000073d0: 0a20 2020 2020 2020 2074 6162 6c65 7320  .        tables 
-000073e0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-000073f0: 2873 6368 656d 612c 2022 7573 6572 7322  (schema, "users"
-00007400: 293a 205b 0a20 2020 2020 2020 2020 2020  ): [.           
-00007410: 2020 2020 2066 6b28 5b22 7061 7265 6e74       fk(["parent
-00007420: 5f75 7365 725f 6964 225d 2c20 5b22 7573  _user_id"], ["us
-00007430: 6572 5f69 6422 5d2c 2022 7573 6572 7322  er_id"], "users"
-00007440: 2c20 6e61 6d65 3d22 7573 6572 5f69 645f  , name="user_id_
-00007450: 666b 2229 0a20 2020 2020 2020 2020 2020  fk").           
-00007460: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00007470: 2873 6368 656d 612c 2022 6469 6e67 616c  (schema, "dingal
-00007480: 696e 6773 2229 3a20 5b0a 2020 2020 2020  ings"): [.      
-00007490: 2020 2020 2020 2020 2020 666b 285b 2261            fk(["a
-000074a0: 6464 7265 7373 5f69 6422 5d2c 205b 2261  ddress_id"], ["a
-000074b0: 6464 7265 7373 5f69 6422 5d2c 2022 656d  ddress_id"], "em
-000074c0: 6169 6c5f 6164 6472 6573 7365 7322 292c  ail_addresses"),
-000074d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000074e0: 2066 6b28 5b22 6964 5f75 7365 7222 5d2c   fk(["id_user"],
-000074f0: 205b 2275 7365 725f 6964 225d 2c20 2275   ["user_id"], "u
-00007500: 7365 7273 2229 2c0a 2020 2020 2020 2020  sers"),.        
-00007510: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00007520: 2020 2028 7363 6865 6d61 2c20 2265 6d61     (schema, "ema
-00007530: 696c 5f61 6464 7265 7373 6573 2229 3a20  il_addresses"): 
-00007540: 5b66 6b28 5b22 7265 6d6f 7465 5f75 7365  [fk(["remote_use
-00007550: 725f 6964 225d 2c20 5b22 7573 6572 5f69  r_id"], ["user_i
-00007560: 6422 5d2c 2022 7573 6572 7322 295d 2c0a  d"], "users")],.
-00007570: 2020 2020 2020 2020 2020 2020 2873 6368              (sch
-00007580: 656d 612c 2022 6c6f 6361 6c5f 7461 626c  ema, "local_tabl
-00007590: 6522 293a 205b 0a20 2020 2020 2020 2020  e"): [.         
-000075a0: 2020 2020 2020 2066 6b28 0a20 2020 2020         fk(.     
-000075b0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000075c0: 2272 656d 6f74 655f 6964 225d 2c0a 2020  "remote_id"],.  
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075e0: 2020 5b22 6964 225d 2c0a 2020 2020 2020    ["id"],.      
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00007600: 656d 6f74 655f 7461 626c 655f 3222 2c0a  emote_table_2",.
-00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007620: 2020 2020 7265 665f 7363 6865 6d61 3d63      ref_schema=c
-00007630: 6f6e 6669 672e 7465 7374 5f73 6368 656d  onfig.test_schem
-00007640: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00007650: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00007660: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00007670: 2873 6368 656d 612c 2022 7265 6d6f 7465  (schema, "remote
-00007680: 5f74 6162 6c65 2229 3a20 5b0a 2020 2020  _table"): [.    
-00007690: 2020 2020 2020 2020 2020 2020 666b 285b              fk([
-000076a0: 226c 6f63 616c 5f69 6422 5d2c 205b 2269  "local_id"], ["i
-000076b0: 6422 5d2c 2022 6c6f 6361 6c5f 7461 626c  d"], "local_tabl
-000076c0: 6522 2c20 7265 665f 7363 6865 6d61 3d4e  e", ref_schema=N
-000076d0: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
-000076e0: 205d 2c0a 2020 2020 2020 2020 7d0a 2020   ],.        }.  
-000076f0: 2020 2020 2020 6966 206e 6f74 2074 6573        if not tes
-00007700: 7469 6e67 2e72 6571 7569 7265 732e 7365  ting.requires.se
-00007710: 6c66 5f72 6566 6572 656e 7469 616c 5f66  lf_referential_f
-00007720: 6f72 6569 676e 5f6b 6579 732e 656e 6162  oreign_keys.enab
-00007730: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-00007740: 2074 6162 6c65 735b 2873 6368 656d 612c   tables[(schema,
-00007750: 2022 7573 6572 7322 295d 2e63 6c65 6172   "users")].clear
-00007760: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
-00007770: 7420 7465 7374 696e 672e 7265 7175 6972  t testing.requir
-00007780: 6573 2e6e 616d 6564 5f63 6f6e 7374 7261  es.named_constra
-00007790: 696e 7473 2e65 6e61 626c 6564 3a0a 2020  ints.enabled:.  
-000077a0: 2020 2020 2020 2020 2020 666f 7220 7661            for va
-000077b0: 6c73 2069 6e20 7461 626c 6573 2e76 616c  ls in tables.val
-000077c0: 7565 7328 293a 0a20 2020 2020 2020 2020  ues():.         
-000077d0: 2020 2020 2020 2066 6f72 2076 616c 2069         for val i
-000077e0: 6e20 7661 6c73 3a0a 2020 2020 2020 2020  n vals:.        
-000077f0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00007800: 616c 5b22 6e61 6d65 225d 2069 7320 6e6f  al["name"] is no
-00007810: 7420 6d6f 636b 2e41 4e59 3a0a 2020 2020  t mock.ANY:.    
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 7661 6c5b 226e 616d 6522 5d20      val["name"] 
-00007840: 3d20 6d6f 636b 2e41 4e59 0a0a 2020 2020  = mock.ANY..    
-00007850: 2020 2020 7265 7320 3d20 7365 6c66 2e5f      res = self._
-00007860: 7265 736f 6c76 655f 6b69 6e64 286b 696e  resolve_kind(kin
-00007870: 642c 2074 6162 6c65 732c 2076 6965 7773  d, tables, views
-00007880: 2c20 6d61 7465 7269 616c 697a 6564 290a  , materialized).
-00007890: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-000078a0: 6c66 2e5f 7265 736f 6c76 655f 6e61 6d65  lf._resolve_name
-000078b0: 7328 7363 6865 6d61 2c20 7363 6f70 652c  s(schema, scope,
-000078c0: 2066 696c 7465 725f 6e61 6d65 732c 2072   filter_names, r
-000078d0: 6573 290a 2020 2020 2020 2020 7265 7475  es).        retu
-000078e0: 726e 2072 6573 0a0a 2020 2020 4066 696c  rn res..    @fil
-000078f0: 7465 725f 6e61 6d65 5f76 616c 7565 7328  ter_name_values(
-00007900: 290a 2020 2020 4074 6573 7469 6e67 2e72  ).    @testing.r
-00007910: 6571 7569 7265 732e 666f 7265 6967 6e5f  equires.foreign_
-00007920: 6b65 795f 636f 6e73 7472 6169 6e74 5f72  key_constraint_r
-00007930: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
-00007940: 6620 7465 7374 5f67 6574 5f6d 756c 7469  f test_get_multi
-00007950: 5f66 6f72 6569 676e 5f6b 6579 7328 0a20  _foreign_keys(. 
-00007960: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00007970: 2020 2020 2067 6574 5f6d 756c 7469 5f65       get_multi_e
-00007980: 7870 2c0a 2020 2020 2020 2020 7573 655f  xp,.        use_
-00007990: 6669 6c74 6572 2c0a 2020 2020 2020 2020  filter,.        
-000079a0: 7363 6865 6d61 3d4e 6f6e 652c 0a20 2020  schema=None,.   
-000079b0: 2020 2020 2073 636f 7065 3d4f 626a 6563       scope=Objec
-000079c0: 7453 636f 7065 2e44 4546 4155 4c54 2c0a  tScope.DEFAULT,.
-000079d0: 2020 2020 2020 2020 6b69 6e64 3d4f 626a          kind=Obj
-000079e0: 6563 744b 696e 642e 5441 424c 452c 0a20  ectKind.TABLE,. 
-000079f0: 2020 2029 3a0a 0a20 2020 2020 2020 2022     ):..        "
-00007a00: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
-00007a10: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
-00007a20: 2020 2020 2020 5370 616e 6e65 7220 646f        Spanner do
-00007a30: 6573 6e27 7420 7375 7070 6f72 7420 7465  esn't support te
-00007a40: 6d70 6f72 6172 7920 7461 626c 6573 2c20  mporary tables, 
-00007a50: 736f 2072 6561 6c20 7461 626c 6573 2061  so real tables a
-00007a60: 7265 0a20 2020 2020 2020 2075 7365 6420  re.        used 
-00007a70: 666f 7220 7465 7374 696e 672e 2041 7320  for testing. As 
-00007a80: 7468 6520 6f72 6967 696e 616c 2074 6573  the original tes
-00007a90: 7420 6578 7065 6374 7320 6f6e 6c79 2072  t expects only r
-00007aa0: 6561 6c0a 2020 2020 2020 2020 7461 626c  eal.        tabl
-00007ab0: 6573 2074 6f20 6265 2072 6561 642c 2061  es to be read, a
-00007ac0: 6e64 2069 6e20 5370 616e 6e65 7220 616c  nd in Spanner al
-00007ad0: 6c20 7468 6520 7461 626c 6573 2061 7265  l the tables are
-00007ae0: 2072 6561 6c2c 0a20 2020 2020 2020 2065   real,.        e
-00007af0: 7870 6563 7465 6420 7265 7375 6c74 7320  xpected results 
-00007b00: 6f76 6572 7269 6465 2069 7320 7265 7175  override is requ
-00007b10: 6972 6564 2e0a 2020 2020 2020 2020 2222  ired..        ""
-00007b20: 220a 2020 2020 2020 2020 696e 7370 2c20  ".        insp, 
-00007b30: 6b77 732c 2065 7870 203d 2067 6574 5f6d  kws, exp = get_m
-00007b40: 756c 7469 5f65 7870 280a 2020 2020 2020  ulti_exp(.      
-00007b50: 2020 2020 2020 7363 6865 6d61 2c0a 2020        schema,.  
-00007b60: 2020 2020 2020 2020 2020 7363 6f70 652c            scope,
-00007b70: 0a20 2020 2020 2020 2020 2020 206b 696e  .            kin
-00007b80: 642c 0a20 2020 2020 2020 2020 2020 2075  d,.            u
-00007b90: 7365 5f66 696c 7465 722c 0a20 2020 2020  se_filter,.     
-00007ba0: 2020 2020 2020 2049 6e73 7065 6374 6f72         Inspector
-00007bb0: 2e67 6574 5f66 6f72 6569 676e 5f6b 6579  .get_foreign_key
-00007bc0: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
-00007bd0: 656c 662e 6578 705f 666b 732c 0a20 2020  elf.exp_fks,.   
-00007be0: 2020 2020 2029 0a20 2020 2020 2020 2066       ).        f
-00007bf0: 6f72 206b 7720 696e 206b 7773 3a0a 2020  or kw in kws:.  
-00007c00: 2020 2020 2020 2020 2020 696e 7370 2e63            insp.c
-00007c10: 6c65 6172 5f63 6163 6865 2829 0a20 2020  lear_cache().   
-00007c20: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00007c30: 3d20 696e 7370 2e67 6574 5f6d 756c 7469  = insp.get_multi
-00007c40: 5f66 6f72 6569 676e 5f6b 6579 7328 2a2a  _foreign_keys(**
-00007c50: 6b77 290a 2020 2020 2020 2020 2020 2020  kw).            
-00007c60: 7365 6c66 2e5f 6164 6a75 7374 5f73 6f72  self._adjust_sor
-00007c70: 7428 7265 7375 6c74 2c20 6578 702c 206c  t(result, exp, l
-00007c80: 616d 6264 6120 643a 2074 7570 6c65 2864  ambda d: tuple(d
-00007c90: 5b22 636f 6e73 7472 6169 6e65 645f 636f  ["constrained_co
-00007ca0: 6c75 6d6e 7322 5d29 290a 2020 2020 2020  lumns"])).      
-00007cb0: 2020 2020 2020 7365 6c66 2e5f 6368 6563        self._chec
-00007cc0: 6b5f 7461 626c 655f 6469 6374 280a 2020  k_table_dict(.  
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cf0: 2020 2020 6b65 793a 2073 6f72 7465 6428      key: sorted(
-00007d00: 7661 6c75 652c 206b 6579 3d6c 616d 6264  value, key=lambd
-00007d10: 6120 783a 2078 5b22 636f 6e73 7472 6169  a x: x["constrai
-00007d20: 6e65 645f 636f 6c75 6d6e 7322 5d29 0a20  ned_columns"]). 
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2066 6f72 206b 6579 2c20 7661 6c75     for key, valu
-00007d50: 6520 696e 2072 6573 756c 742e 6974 656d  e in result.item
-00007d60: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00007d70: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00007d80: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00007d90: 2020 2020 2020 2020 2020 2020 206b 6579               key
-00007da0: 3a20 736f 7274 6564 2876 616c 7565 2c20  : sorted(value, 
-00007db0: 6b65 793d 6c61 6d62 6461 2078 3a20 785b  key=lambda x: x[
-00007dc0: 2263 6f6e 7374 7261 696e 6564 5f63 6f6c  "constrained_col
-00007dd0: 756d 6e73 225d 290a 2020 2020 2020 2020  umns"]).        
-00007de0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00007df0: 6b65 792c 2076 616c 7565 2069 6e20 6578  key, value in ex
-00007e00: 702e 6974 656d 7328 290a 2020 2020 2020  p.items().      
-00007e10: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007e20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007e30: 662e 5f72 6571 7569 7265 645f 666b 5f6b  f._required_fk_k
-00007e40: 6579 732c 0a20 2020 2020 2020 2020 2020  eys,.           
-00007e50: 2029 0a0a 2020 2020 6465 6620 6578 705f   )..    def exp_
-00007e60: 636f 6c75 6d6e 7328 0a20 2020 2020 2020  columns(.       
-00007e70: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-00007e80: 6368 656d 613d 4e6f 6e65 2c0a 2020 2020  chema=None,.    
-00007e90: 2020 2020 7363 6f70 653d 4f62 6a65 6374      scope=Object
-00007ea0: 5363 6f70 652e 414e 592c 0a20 2020 2020  Scope.ANY,.     
-00007eb0: 2020 206b 696e 643d 4f62 6a65 6374 4b69     kind=ObjectKi
-00007ec0: 6e64 2e41 4e59 2c0a 2020 2020 2020 2020  nd.ANY,.        
-00007ed0: 6669 6c74 6572 5f6e 616d 6573 3d4e 6f6e  filter_names=Non
-00007ee0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00007ef0: 2020 6465 6620 636f 6c28 6e61 6d65 2c20    def col(name, 
-00007f00: 6175 746f 3d46 616c 7365 2c20 6465 6661  auto=False, defa
-00007f10: 756c 743d 6d6f 636b 2e41 4e59 2c20 636f  ult=mock.ANY, co
-00007f20: 6d6d 656e 743d 4e6f 6e65 2c20 6e75 6c6c  mment=None, null
-00007f30: 6162 6c65 3d54 7275 6529 3a0a 2020 2020  able=True):.    
-00007f40: 2020 2020 2020 2020 7265 7320 3d20 7b0a          res = {.
-00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f60: 226e 616d 6522 3a20 6e61 6d65 2c0a 2020  "name": name,.  
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00007f80: 7574 6f69 6e63 7265 6d65 6e74 223a 2061  utoincrement": a
-00007f90: 7574 6f2c 0a20 2020 2020 2020 2020 2020  uto,.           
-00007fa0: 2020 2020 2022 7479 7065 223a 206d 6f63       "type": moc
-00007fb0: 6b2e 414e 592c 0a20 2020 2020 2020 2020  k.ANY,.         
-00007fc0: 2020 2020 2020 2022 6465 6661 756c 7422         "default"
-00007fd0: 3a20 6465 6661 756c 742c 0a20 2020 2020  : default,.     
-00007fe0: 2020 2020 2020 2020 2020 2022 636f 6d6d             "comm
-00007ff0: 656e 7422 3a20 636f 6d6d 656e 742c 0a20  ent": comment,. 
-00008000: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008010: 6e75 6c6c 6162 6c65 223a 206e 756c 6c61  nullable": nulla
-00008020: 626c 652c 0a20 2020 2020 2020 2020 2020  ble,.           
-00008030: 207d 0a20 2020 2020 2020 2020 2020 2069   }.            i
-00008040: 6620 6175 746f 203d 3d20 226f 6d69 7422  f auto == "omit"
-00008050: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008060: 2020 7265 732e 706f 7028 2261 7574 6f69    res.pop("autoi
-00008070: 6e63 7265 6d65 6e74 2229 0a20 2020 2020  ncrement").     
-00008080: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00008090: 730a 0a20 2020 2020 2020 2064 6566 2070  s..        def p
-000080a0: 6b28 6e61 6d65 2c20 2a2a 6b77 293a 0a20  k(name, **kw):. 
-000080b0: 2020 2020 2020 2020 2020 206b 7720 3d20             kw = 
-000080c0: 7b22 6175 746f 223a 2054 7275 652c 2022  {"auto": True, "
-000080d0: 6465 6661 756c 7422 3a20 6d6f 636b 2e41  default": mock.A
-000080e0: 4e59 2c20 226e 756c 6c61 626c 6522 3a20  NY, "nullable": 
-000080f0: 4661 6c73 652c 202a 2a6b 777d 0a20 2020  False, **kw}.   
-00008100: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008110: 636f 6c28 6e61 6d65 2c20 2a2a 6b77 290a  col(name, **kw).
-00008120: 0a20 2020 2020 2020 206d 6174 6572 6961  .        materia
-00008130: 6c69 7a65 6420 3d20 7b0a 2020 2020 2020  lized = {.      
-00008140: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
-00008150: 6469 6e67 616c 696e 6773 5f76 2229 3a20  dingalings_v"): 
-00008160: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00008170: 2020 636f 6c28 2264 696e 6761 6c69 6e67    col("dingaling
-00008180: 5f69 6422 2c20 6175 746f 3d22 6f6d 6974  _id", auto="omit
-00008190: 222c 206e 756c 6c61 626c 653d 6d6f 636b  ", nullable=mock
-000081a0: 2e41 4e59 292c 0a20 2020 2020 2020 2020  .ANY),.         
-000081b0: 2020 2020 2020 2063 6f6c 2822 6164 6472         col("addr
-000081c0: 6573 735f 6964 2229 2c0a 2020 2020 2020  ess_id"),.      
-000081d0: 2020 2020 2020 2020 2020 636f 6c28 2269            col("i
-000081e0: 645f 7573 6572 2229 2c0a 2020 2020 2020  d_user"),.      
-000081f0: 2020 2020 2020 2020 2020 636f 6c28 2264            col("d
-00008200: 6174 6122 292c 0a20 2020 2020 2020 2020  ata"),.         
-00008210: 2020 205d 0a20 2020 2020 2020 207d 0a20     ].        }. 
-00008220: 2020 2020 2020 2076 6965 7773 203d 207b         views = {
-00008230: 0a20 2020 2020 2020 2020 2020 2028 7363  .            (sc
-00008240: 6865 6d61 2c20 2265 6d61 696c 5f61 6464  hema, "email_add
-00008250: 7265 7373 6573 5f76 2229 3a20 5b0a 2020  resses_v"): [.  
-00008260: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008270: 6c28 2261 6464 7265 7373 5f69 6422 2c20  l("address_id", 
-00008280: 6175 746f 3d22 6f6d 6974 222c 206e 756c  auto="omit", nul
-00008290: 6c61 626c 653d 6d6f 636b 2e41 4e59 292c  lable=mock.ANY),
-000082a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000082b0: 2063 6f6c 2822 7265 6d6f 7465 5f75 7365   col("remote_use
-000082c0: 725f 6964 2229 2c0a 2020 2020 2020 2020  r_id"),.        
-000082d0: 2020 2020 2020 2020 636f 6c28 2265 6d61          col("ema
-000082e0: 696c 5f61 6464 7265 7373 2229 2c0a 2020  il_address"),.  
-000082f0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00008300: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
-00008310: 2c20 2275 7365 7273 5f76 2229 3a20 5b0a  , "users_v"): [.
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 636f 6c28 2275 7365 725f 6964 222c 2061  col("user_id", a
-00008340: 7574 6f3d 226f 6d69 7422 2c20 6e75 6c6c  uto="omit", null
-00008350: 6162 6c65 3d6d 6f63 6b2e 414e 5929 2c0a  able=mock.ANY),.
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 636f 6c28 2274 6573 7431 222c 206e 756c  col("test1", nul
-00008380: 6c61 626c 653d 6d6f 636b 2e41 4e59 292c  lable=mock.ANY),
-00008390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083a0: 2063 6f6c 2822 7465 7374 3222 2c20 6e75   col("test2", nu
-000083b0: 6c6c 6162 6c65 3d6d 6f63 6b2e 414e 5929  llable=mock.ANY)
-000083c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000083d0: 2020 636f 6c28 2270 6172 656e 745f 7573    col("parent_us
-000083e0: 6572 5f69 6422 292c 0a20 2020 2020 2020  er_id"),.       
-000083f0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00008400: 2020 2020 2873 6368 656d 612c 2022 7573      (schema, "us
-00008410: 6572 5f74 6d70 5f76 2229 3a20 5b0a 2020  er_tmp_v"): [.  
-00008420: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008430: 6c28 2269 6422 2c20 6175 746f 3d22 6f6d  l("id", auto="om
-00008440: 6974 222c 206e 756c 6c61 626c 653d 6d6f  it", nullable=mo
-00008450: 636b 2e41 4e59 292c 0a20 2020 2020 2020  ck.ANY),.       
-00008460: 2020 2020 2020 2020 2063 6f6c 2822 6e61           col("na
-00008470: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
-00008480: 2020 2020 2020 636f 6c28 2266 6f6f 2229        col("foo")
-00008490: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
-000084a0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-000084b0: 2020 2073 656c 662e 5f72 6573 6f6c 7665     self._resolve
-000084c0: 5f76 6965 7773 2876 6965 7773 2c20 6d61  _views(views, ma
-000084d0: 7465 7269 616c 697a 6564 290a 2020 2020  terialized).    
-000084e0: 2020 2020 7461 626c 6573 203d 207b 0a20      tables = {. 
-000084f0: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
-00008500: 6d61 2c20 2275 7365 7273 2229 3a20 5b0a  ma, "users"): [.
-00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008520: 706b 2822 7573 6572 5f69 6422 292c 0a20  pk("user_id"),. 
-00008530: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008540: 6f6c 2822 7465 7374 3122 2c20 6e75 6c6c  ol("test1", null
-00008550: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
-00008560: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00008570: 2822 7465 7374 3222 2c20 6e75 6c6c 6162  ("test2", nullab
-00008580: 6c65 3d46 616c 7365 292c 0a20 2020 2020  le=False),.     
-00008590: 2020 2020 2020 2020 2020 2063 6f6c 2822             col("
-000085a0: 7061 7265 6e74 5f75 7365 725f 6964 2229  parent_user_id")
-000085b0: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
-000085c0: 0a20 2020 2020 2020 2020 2020 2028 7363  .            (sc
-000085d0: 6865 6d61 2c20 2264 696e 6761 6c69 6e67  hema, "dingaling
-000085e0: 7322 293a 205b 0a20 2020 2020 2020 2020  s"): [.         
-000085f0: 2020 2020 2020 2070 6b28 2264 696e 6761         pk("dinga
-00008600: 6c69 6e67 5f69 6422 292c 0a20 2020 2020  ling_id"),.     
-00008610: 2020 2020 2020 2020 2020 2063 6f6c 2822             col("
-00008620: 6164 6472 6573 735f 6964 2229 2c0a 2020  address_id"),.  
-00008630: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008640: 6c28 2269 645f 7573 6572 2229 2c0a 2020  l("id_user"),.  
-00008650: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008660: 6c28 2264 6174 6122 292c 0a20 2020 2020  l("data"),.     
-00008670: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00008680: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
-00008690: 656d 6169 6c5f 6164 6472 6573 7365 7322  email_addresses"
-000086a0: 293a 205b 0a20 2020 2020 2020 2020 2020  ): [.           
-000086b0: 2020 2020 2070 6b28 2261 6464 7265 7373       pk("address
-000086c0: 5f69 6422 292c 0a20 2020 2020 2020 2020  _id"),.         
-000086d0: 2020 2020 2020 2063 6f6c 2822 7265 6d6f         col("remo
-000086e0: 7465 5f75 7365 725f 6964 2229 2c0a 2020  te_user_id"),.  
-000086f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008700: 6c28 2265 6d61 696c 5f61 6464 7265 7373  l("email_address
-00008710: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00008720: 5d2c 0a20 2020 2020 2020 2020 2020 2028  ],.            (
-00008730: 7363 6865 6d61 2c20 2263 6f6d 6d65 6e74  schema, "comment
-00008740: 5f74 6573 7422 293a 205b 0a20 2020 2020  _test"): [.     
-00008750: 2020 2020 2020 2020 2020 2070 6b28 2269             pk("i
-00008760: 6422 2c20 636f 6d6d 656e 743d 2269 6420  d", comment="id 
-00008770: 636f 6d6d 656e 7422 292c 0a20 2020 2020  comment"),.     
-00008780: 2020 2020 2020 2020 2020 2063 6f6c 2822             col("
-00008790: 6461 7461 222c 2063 6f6d 6d65 6e74 3d22  data", comment="
-000087a0: 6461 7461 2025 2063 6f6d 6d65 6e74 2229  data % comment")
-000087b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000087c0: 2020 636f 6c28 0a20 2020 2020 2020 2020    col(.         
-000087d0: 2020 2020 2020 2020 2020 2022 6432 222c             "d2",
-000087e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000087f0: 2020 2020 2063 6f6d 6d65 6e74 3d72 2222       comment=r""
-00008800: 2243 6f6d 6d65 6e74 2074 7970 6573 2074  "Comment types t
-00008810: 7970 6520 7370 6565 6469 6c79 2027 2022  ype speedily ' "
-00008820: 205c 2027 2720 4675 6e21 2222 222c 0a20   \ '' Fun!""",. 
-00008830: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008840: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
-00008850: 0a20 2020 2020 2020 2020 2020 2028 7363  .            (sc
-00008860: 6865 6d61 2c20 226e 6f5f 636f 6e73 7472  hema, "no_constr
-00008870: 6169 6e74 7322 293a 205b 636f 6c28 2264  aints"): [col("d
-00008880: 6174 6122 295d 2c0a 2020 2020 2020 2020  ata")],.        
-00008890: 2020 2020 2873 6368 656d 612c 2022 6c6f      (schema, "lo
-000088a0: 6361 6c5f 7461 626c 6522 293a 205b 706b  cal_table"): [pk
-000088b0: 2822 6964 2229 2c20 636f 6c28 2264 6174  ("id"), col("dat
-000088c0: 6122 292c 2063 6f6c 2822 7265 6d6f 7465  a"), col("remote
-000088d0: 5f69 6422 295d 2c0a 2020 2020 2020 2020  _id")],.        
-000088e0: 2020 2020 2873 6368 656d 612c 2022 7265      (schema, "re
-000088f0: 6d6f 7465 5f74 6162 6c65 2229 3a20 5b70  mote_table"): [p
-00008900: 6b28 2269 6422 292c 2063 6f6c 2822 6c6f  k("id"), col("lo
-00008910: 6361 6c5f 6964 2229 2c20 636f 6c28 2264  cal_id"), col("d
-00008920: 6174 6122 295d 2c0a 2020 2020 2020 2020  ata")],.        
-00008930: 2020 2020 2873 6368 656d 612c 2022 7265      (schema, "re
-00008940: 6d6f 7465 5f74 6162 6c65 5f32 2229 3a20  mote_table_2"): 
-00008950: 5b70 6b28 2269 6422 292c 2063 6f6c 2822  [pk("id"), col("
-00008960: 6461 7461 2229 5d2c 0a20 2020 2020 2020  data")],.       
-00008970: 2020 2020 2028 7363 6865 6d61 2c20 226e       (schema, "n
-00008980: 6f6e 636f 6c5f 6964 785f 7465 7374 5f6e  oncol_idx_test_n
-00008990: 6f70 6b22 293a 205b 706b 2822 6964 2229  opk"): [pk("id")
-000089a0: 2c20 636f 6c28 2271 2229 5d2c 0a20 2020  , col("q")],.   
-000089b0: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
-000089c0: 2c20 226e 6f6e 636f 6c5f 6964 785f 7465  , "noncol_idx_te
-000089d0: 7374 5f70 6b22 293a 205b 706b 2822 6964  st_pk"): [pk("id
-000089e0: 2229 2c20 636f 6c28 2271 2229 5d2c 0a20  "), col("q")],. 
-000089f0: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
-00008a00: 6d61 2c20 7365 6c66 2e74 656d 705f 7461  ma, self.temp_ta
-00008a10: 626c 655f 6e61 6d65 2829 293a 205b 0a20  ble_name()): [. 
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008a30: 6b28 2269 6422 292c 0a20 2020 2020 2020  k("id"),.       
-00008a40: 2020 2020 2020 2020 2063 6f6c 2822 6e61           col("na
-00008a50: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
-00008a60: 2020 2020 2020 636f 6c28 2266 6f6f 2229        col("foo")
-00008a70: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
-00008a80: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00008a90: 2020 2072 6573 203d 2073 656c 662e 5f72     res = self._r
-00008aa0: 6573 6f6c 7665 5f6b 696e 6428 6b69 6e64  esolve_kind(kind
-00008ab0: 2c20 7461 626c 6573 2c20 7669 6577 732c  , tables, views,
-00008ac0: 206d 6174 6572 6961 6c69 7a65 6429 0a20   materialized). 
-00008ad0: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-00008ae0: 662e 5f72 6573 6f6c 7665 5f6e 616d 6573  f._resolve_names
-00008af0: 2873 6368 656d 612c 2073 636f 7065 2c20  (schema, scope, 
-00008b00: 6669 6c74 6572 5f6e 616d 6573 2c20 7265  filter_names, re
-00008b10: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
-00008b20: 6e20 7265 730a 0a20 2020 2040 6669 6c74  n res..    @filt
-00008b30: 6572 5f6e 616d 655f 7661 6c75 6573 2829  er_name_values()
-00008b40: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
-00008b50: 745f 6d75 6c74 695f 636f 6c75 6d6e 7328  t_multi_columns(
-00008b60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008b70: 2020 2020 2020 2067 6574 5f6d 756c 7469         get_multi
-00008b80: 5f65 7870 2c0a 2020 2020 2020 2020 7573  _exp,.        us
-00008b90: 655f 6669 6c74 6572 2c0a 2020 2020 2020  e_filter,.      
-00008ba0: 2020 7363 6865 6d61 3d4e 6f6e 652c 0a20    schema=None,. 
-00008bb0: 2020 2020 2020 2073 636f 7065 3d4f 626a         scope=Obj
-00008bc0: 6563 7453 636f 7065 2e44 4546 4155 4c54  ectScope.DEFAULT
-00008bd0: 2c0a 2020 2020 2020 2020 6b69 6e64 3d4f  ,.        kind=O
-00008be0: 626a 6563 744b 696e 642e 5441 424c 452c  bjectKind.TABLE,
-00008bf0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00008c00: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-00008c10: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-00008c20: 2020 2020 2020 2053 7061 6e6e 6572 2064         Spanner d
-00008c30: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-00008c40: 656d 706f 7261 7279 2074 6162 6c65 732c  emporary tables,
-00008c50: 2073 6f20 7265 616c 2074 6162 6c65 7320   so real tables 
-00008c60: 6172 650a 2020 2020 2020 2020 7573 6564  are.        used
-00008c70: 2066 6f72 2074 6573 7469 6e67 2e20 4173   for testing. As
-00008c80: 2074 6865 206f 7269 6769 6e61 6c20 7465   the original te
-00008c90: 7374 2065 7870 6563 7473 206f 6e6c 7920  st expects only 
-00008ca0: 7265 616c 0a20 2020 2020 2020 2074 6162  real.        tab
-00008cb0: 6c65 7320 746f 2062 6520 7265 6164 2c20  les to be read, 
-00008cc0: 616e 6420 696e 2053 7061 6e6e 6572 2061  and in Spanner a
-00008cd0: 6c6c 2074 6865 2074 6162 6c65 7320 6172  ll the tables ar
-00008ce0: 6520 7265 616c 2c0a 2020 2020 2020 2020  e real,.        
-00008cf0: 6578 7065 6374 6564 2072 6573 756c 7473  expected results
-00008d00: 206f 7665 7272 6964 6520 6973 2072 6571   override is req
-00008d10: 7569 7265 642e 0a20 2020 2020 2020 2022  uired..        "
-00008d20: 2222 0a20 2020 2020 2020 2069 6e73 702c  "".        insp,
-00008d30: 206b 7773 2c20 6578 7020 3d20 6765 745f   kws, exp = get_
-00008d40: 6d75 6c74 695f 6578 7028 0a20 2020 2020  multi_exp(.     
-00008d50: 2020 2020 2020 2073 6368 656d 612c 0a20         schema,. 
-00008d60: 2020 2020 2020 2020 2020 2073 636f 7065             scope
-00008d70: 2c0a 2020 2020 2020 2020 2020 2020 6b69  ,.            ki
-00008d80: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-00008d90: 7573 655f 6669 6c74 6572 2c0a 2020 2020  use_filter,.    
-00008da0: 2020 2020 2020 2020 496e 7370 6563 746f          Inspecto
-00008db0: 722e 6765 745f 636f 6c75 6d6e 732c 0a20  r.get_columns,. 
-00008dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008dd0: 6578 705f 636f 6c75 6d6e 732c 0a20 2020  exp_columns,.   
-00008de0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00008df0: 666f 7220 6b77 2069 6e20 6b77 733a 0a20  for kw in kws:. 
-00008e00: 2020 2020 2020 2020 2020 2069 6e73 702e             insp.
-00008e10: 636c 6561 725f 6361 6368 6528 290a 2020  clear_cache().  
-00008e20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00008e30: 203d 2069 6e73 702e 6765 745f 6d75 6c74   = insp.get_mult
-00008e40: 695f 636f 6c75 6d6e 7328 2a2a 6b77 290a  i_columns(**kw).
-00008e50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008e60: 2e5f 6368 6563 6b5f 7461 626c 655f 6469  ._check_table_di
-00008e70: 6374 2872 6573 756c 742c 2065 7870 2c20  ct(result, exp, 
-00008e80: 7365 6c66 2e5f 7265 7175 6972 6564 5f63  self._required_c
-00008e90: 6f6c 756d 6e5f 6b65 7973 290a 0a20 2020  olumn_keys)..   
-00008ea0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
-00008eb0: 6970 280a 2020 2020 2020 2020 2252 6571  ip(.        "Req
-00008ec0: 7569 7265 7320 616e 2069 6e74 726f 7370  uires an introsp
-00008ed0: 6563 7469 6f6e 206d 6574 686f 6420 746f  ection method to
-00008ee0: 2062 6520 696d 706c 656d 656e 7465 6420   be implemented 
-00008ef0: 696e 2053 514c 416c 6368 656d 7920 6669  in SQLAlchemy fi
-00008f00: 7273 7422 0a20 2020 2029 0a20 2020 2064  rst".    ).    d
-00008f10: 6566 2074 6573 745f 6765 745f 6d75 6c74  ef test_get_mult
-00008f20: 695f 756e 6971 7565 5f63 6f6e 7374 7261  i_unique_constra
-00008f30: 696e 7473 2829 3a0a 2020 2020 2020 2020  ints():.        
-00008f40: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-00008f50: 742e 6d61 726b 2e73 6b69 7028 0a20 2020  t.mark.skip(.   
-00008f60: 2020 2020 2022 5265 7175 6972 6573 2061       "Requires a
-00008f70: 6e20 696e 7472 6f73 7065 6374 696f 6e20  n introspection 
-00008f80: 6d65 7468 6f64 2074 6f20 6265 2069 6d70  method to be imp
-00008f90: 6c65 6d65 6e74 6564 2069 6e20 5351 4c41  lemented in SQLA
-00008fa0: 6c63 6865 6d79 2066 6972 7374 220a 2020  lchemy first".  
-00008fb0: 2020 290a 2020 2020 6465 6620 7465 7374    ).    def test
-00008fc0: 5f67 6574 5f6d 756c 7469 5f63 6865 636b  _get_multi_check
-00008fd0: 5f63 6f6e 7374 7261 696e 7473 2829 3a0a  _constraints():.
-00008fe0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00008ff0: 2020 4074 6573 7469 6e67 2e63 6f6d 6269    @testing.combi
-00009000: 6e61 7469 6f6e 7328 2846 616c 7365 2c29  nations((False,)
-00009010: 2c20 6172 676e 616d 6573 3d22 7573 655f  , argnames="use_
-00009020: 7363 6865 6d61 2229 0a20 2020 2040 7465  schema").    @te
-00009030: 7374 696e 672e 7265 7175 6972 6573 2e66  sting.requires.f
-00009040: 6f72 6569 676e 5f6b 6579 5f63 6f6e 7374  oreign_key_const
-00009050: 7261 696e 745f 7265 666c 6563 7469 6f6e  raint_reflection
-00009060: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
-00009070: 745f 666f 7265 6967 6e5f 6b65 7973 2873  t_foreign_keys(s
-00009080: 656c 662c 2063 6f6e 6e65 6374 696f 6e2c  elf, connection,
-00009090: 2075 7365 5f73 6368 656d 6129 3a0a 2020   use_schema):.  
-000090a0: 2020 2020 2020 6966 2075 7365 5f73 6368        if use_sch
-000090b0: 656d 613a 0a20 2020 2020 2020 2020 2020  ema:.           
-000090c0: 2073 6368 656d 6120 3d20 636f 6e66 6967   schema = config
-000090d0: 2e74 6573 745f 7363 6865 6d61 0a20 2020  .test_schema.   
-000090e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000090f0: 2020 2020 2020 2073 6368 656d 6120 3d20         schema = 
-00009100: 4e6f 6e65 0a0a 2020 2020 2020 2020 7573  None..        us
-00009110: 6572 732c 2061 6464 7265 7373 6573 203d  ers, addresses =
-00009120: 2028 7365 6c66 2e74 6162 6c65 732e 7573   (self.tables.us
-00009130: 6572 732c 2073 656c 662e 7461 626c 6573  ers, self.tables
-00009140: 2e65 6d61 696c 5f61 6464 7265 7373 6573  .email_addresses
-00009150: 290a 2020 2020 2020 2020 696e 7370 203d  ).        insp =
-00009160: 2069 6e73 7065 6374 2863 6f6e 6e65 6374   inspect(connect
-00009170: 696f 6e29 0a20 2020 2020 2020 2065 7870  ion).        exp
-00009180: 6563 7465 645f 7363 6865 6d61 203d 2073  ected_schema = s
-00009190: 6368 656d 610a 2020 2020 2020 2020 2320  chema.        # 
-000091a0: 7573 6572 730a 0a20 2020 2020 2020 2069  users..        i
-000091b0: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
-000091c0: 6573 2e73 656c 665f 7265 6665 7265 6e74  es.self_referent
-000091d0: 6961 6c5f 666f 7265 6967 6e5f 6b65 7973  ial_foreign_keys
-000091e0: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
-000091f0: 2020 2020 2020 7573 6572 735f 666b 6579        users_fkey
-00009200: 7320 3d20 696e 7370 2e67 6574 5f66 6f72  s = insp.get_for
-00009210: 6569 676e 5f6b 6579 7328 7573 6572 732e  eign_keys(users.
-00009220: 6e61 6d65 2c20 7363 6865 6d61 3d73 6368  name, schema=sch
-00009230: 656d 6129 0a20 2020 2020 2020 2020 2020  ema).           
-00009240: 2066 6b65 7931 203d 2075 7365 7273 5f66   fkey1 = users_f
-00009250: 6b65 7973 5b30 5d0a 0a20 2020 2020 2020  keys[0]..       
-00009260: 2020 2020 2077 6974 6820 7465 7374 696e       with testin
-00009270: 672e 7265 7175 6972 6573 2e6e 616d 6564  g.requires.named
-00009280: 5f63 6f6e 7374 7261 696e 7473 2e66 6169  _constraints.fai
-00009290: 6c5f 6966 2829 3a0a 2020 2020 2020 2020  l_if():.        
-000092a0: 2020 2020 2020 2020 6571 5f28 666b 6579          eq_(fkey
-000092b0: 315b 226e 616d 6522 5d2c 2022 7573 6572  1["name"], "user
-000092c0: 5f69 645f 666b 2229 0a0a 2020 2020 2020  _id_fk")..      
-000092d0: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
-000092e0: 2272 6566 6572 7265 645f 7363 6865 6d61  "referred_schema
-000092f0: 225d 2c20 6578 7065 6374 6564 5f73 6368  "], expected_sch
-00009300: 656d 6129 0a20 2020 2020 2020 2020 2020  ema).           
-00009310: 2065 715f 2866 6b65 7931 5b22 7265 6665   eq_(fkey1["refe
-00009320: 7272 6564 5f74 6162 6c65 225d 2c20 7573  rred_table"], us
-00009330: 6572 732e 6e61 6d65 290a 2020 2020 2020  ers.name).      
-00009340: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
-00009350: 2272 6566 6572 7265 645f 636f 6c75 6d6e  "referred_column
-00009360: 7322 5d2c 205b 2275 7365 725f 6964 225d  s"], ["user_id"]
-00009370: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00009380: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
-00009390: 732e 7365 6c66 5f72 6566 6572 656e 7469  s.self_referenti
-000093a0: 616c 5f66 6f72 6569 676e 5f6b 6579 732e  al_foreign_keys.
-000093b0: 656e 6162 6c65 643a 0a20 2020 2020 2020  enabled:.       
-000093c0: 2020 2020 2020 2020 2065 715f 2866 6b65           eq_(fke
-000093d0: 7931 5b22 636f 6e73 7472 6169 6e65 645f  y1["constrained_
-000093e0: 636f 6c75 6d6e 7322 5d2c 205b 2270 6172  columns"], ["par
-000093f0: 656e 745f 7573 6572 5f69 6422 5d29 0a0a  ent_user_id"])..
-00009400: 2020 2020 2020 2020 2320 6164 6472 6573          # addres
-00009410: 7365 730a 2020 2020 2020 2020 6164 6472  ses.        addr
-00009420: 5f66 6b65 7973 203d 2069 6e73 702e 6765  _fkeys = insp.ge
-00009430: 745f 666f 7265 6967 6e5f 6b65 7973 2861  t_foreign_keys(a
-00009440: 6464 7265 7373 6573 2e6e 616d 652c 2073  ddresses.name, s
-00009450: 6368 656d 613d 7363 6865 6d61 290a 2020  chema=schema).  
-00009460: 2020 2020 2020 666b 6579 3120 3d20 6164        fkey1 = ad
-00009470: 6472 5f66 6b65 7973 5b30 5d0a 0a20 2020  dr_fkeys[0]..   
-00009480: 2020 2020 2077 6974 6820 7465 7374 696e       with testin
-00009490: 672e 7265 7175 6972 6573 2e69 6d70 6c69  g.requires.impli
-000094a0: 6369 746c 795f 6e61 6d65 645f 636f 6e73  citly_named_cons
-000094b0: 7472 6169 6e74 732e 6661 696c 5f69 6628  traints.fail_if(
-000094c0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000094d0: 656c 662e 6173 7365 7274 5f28 666b 6579  elf.assert_(fkey
-000094e0: 315b 226e 616d 6522 5d20 6973 206e 6f74  1["name"] is not
-000094f0: 204e 6f6e 6529 0a0a 2020 2020 2020 2020   None)..        
-00009500: 6571 5f28 666b 6579 315b 2272 6566 6572  eq_(fkey1["refer
-00009510: 7265 645f 7363 6865 6d61 225d 2c20 6578  red_schema"], ex
-00009520: 7065 6374 6564 5f73 6368 656d 6129 0a20  pected_schema). 
-00009530: 2020 2020 2020 2065 715f 2866 6b65 7931         eq_(fkey1
-00009540: 5b22 7265 6665 7272 6564 5f74 6162 6c65  ["referred_table
-00009550: 225d 2c20 7573 6572 732e 6e61 6d65 290a  "], users.name).
-00009560: 2020 2020 2020 2020 6571 5f28 666b 6579          eq_(fkey
-00009570: 315b 2272 6566 6572 7265 645f 636f 6c75  1["referred_colu
-00009580: 6d6e 7322 5d2c 205b 2275 7365 725f 6964  mns"], ["user_id
-00009590: 225d 290a 2020 2020 2020 2020 6571 5f28  "]).        eq_(
-000095a0: 666b 6579 315b 2263 6f6e 7374 7261 696e  fkey1["constrain
-000095b0: 6564 5f63 6f6c 756d 6e73 225d 2c20 5b22  ed_columns"], ["
-000095c0: 7265 6d6f 7465 5f75 7365 725f 6964 225d  remote_user_id"]
-000095d0: 290a 0a20 2020 2040 7465 7374 696e 672e  )..    @testing.
-000095e0: 636f 6d62 696e 6174 696f 6e73 280a 2020  combinations(.  
-000095f0: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
-00009600: 2020 2020 2822 666f 7265 6967 6e5f 6b65      ("foreign_ke
-00009610: 7922 2c20 7465 7374 696e 672e 7265 7175  y", testing.requ
-00009620: 6972 6573 2e66 6f72 6569 676e 5f6b 6579  ires.foreign_key
-00009630: 5f63 6f6e 7374 7261 696e 745f 7265 666c  _constraint_refl
-00009640: 6563 7469 6f6e 292c 0a20 2020 2020 2020  ection),.       
-00009650: 2061 7267 6e61 6d65 733d 226f 7264 6572   argnames="order
-00009660: 5f62 7922 2c0a 2020 2020 290a 2020 2020  _by",.    ).    
-00009670: 4074 6573 7469 6e67 2e63 6f6d 6269 6e61  @testing.combina
-00009680: 7469 6f6e 7328 0a20 2020 2020 2020 2028  tions(.        (
-00009690: 5472 7565 2c20 7465 7374 696e 672e 7265  True, testing.re
-000096a0: 7175 6972 6573 2e73 6368 656d 6173 292c  quires.schemas),
-000096b0: 2046 616c 7365 2c20 6172 676e 616d 6573   False, argnames
-000096c0: 3d22 7573 655f 7363 6865 6d61 220a 2020  ="use_schema".  
-000096d0: 2020 290a 2020 2020 6465 6620 7465 7374    ).    def test
-000096e0: 5f67 6574 5f74 6162 6c65 5f6e 616d 6573  _get_table_names
-000096f0: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
-00009700: 6e2c 206f 7264 6572 5f62 792c 2075 7365  n, order_by, use
-00009710: 5f73 6368 656d 6129 3a0a 0a20 2020 2020  _schema):..     
-00009720: 2020 2073 6368 656d 6120 3d20 4e6f 6e65     schema = None
-00009730: 0a0a 2020 2020 2020 2020 5f69 676e 6f72  ..        _ignor
-00009740: 655f 7461 626c 6573 203d 205b 0a20 2020  e_tables = [.   
-00009750: 2020 2020 2020 2020 2022 6163 636f 756e           "accoun
-00009760: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00009770: 2261 6c65 6d62 6963 5f76 6572 7369 6f6e  "alembic_version
-00009780: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00009790: 6279 7465 735f 7461 626c 6522 2c0a 2020  bytes_table",.  
-000097a0: 2020 2020 2020 2020 2020 2263 6f6d 6d65            "comme
-000097b0: 6e74 5f74 6573 7422 2c0a 2020 2020 2020  nt_test",.      
-000097c0: 2020 2020 2020 2264 6174 655f 7461 626c        "date_tabl
-000097d0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-000097e0: 226e 6f6e 636f 6c5f 6964 785f 7465 7374  "noncol_idx_test
-000097f0: 5f70 6b22 2c0a 2020 2020 2020 2020 2020  _pk",.          
-00009800: 2020 226e 6f6e 636f 6c5f 6964 785f 7465    "noncol_idx_te
-00009810: 7374 5f6e 6f70 6b22 2c0a 2020 2020 2020  st_nopk",.      
-00009820: 2020 2020 2020 226c 6f63 616c 5f74 6162        "local_tab
-00009830: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-00009840: 2022 7265 6d6f 7465 5f74 6162 6c65 222c   "remote_table",
-00009850: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00009860: 6d6f 7465 5f74 6162 6c65 5f32 222c 0a20  mote_table_2",. 
-00009870: 2020 2020 2020 2020 2020 2022 7465 7874             "text
-00009880: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
-00009890: 2020 2020 2022 7573 6572 5f74 6d70 222c       "user_tmp",
-000098a0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-000098b0: 5f63 6f6e 7374 7261 696e 7473 222c 0a20  _constraints",. 
-000098c0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-000098d0: 2020 696e 7370 203d 2069 6e73 7065 6374    insp = inspect
-000098e0: 2863 6f6e 6e65 6374 696f 6e29 0a0a 2020  (connection)..  
-000098f0: 2020 2020 2020 6966 206f 7264 6572 5f62        if order_b
-00009900: 793a 0a20 2020 2020 2020 2020 2020 2074  y:.            t
-00009910: 6162 6c65 7320 3d20 5b0a 2020 2020 2020  ables = [.      
-00009920: 2020 2020 2020 2020 2020 7265 635b 305d            rec[0]
-00009930: 2066 6f72 2072 6563 2069 6e20 696e 7370   for rec in insp
-00009940: 2e67 6574 5f73 6f72 7465 645f 7461 626c  .get_sorted_tabl
-00009950: 655f 616e 645f 666b 635f 6e61 6d65 7328  e_and_fkc_names(
-00009960: 7363 6865 6d61 2920 6966 2072 6563 5b30  schema) if rec[0
-00009970: 5d0a 2020 2020 2020 2020 2020 2020 5d0a  ].            ].
-00009980: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00009990: 2020 2020 2020 2020 2020 7461 626c 6573            tables
-000099a0: 203d 2069 6e73 702e 6765 745f 7461 626c   = insp.get_tabl
-000099b0: 655f 6e61 6d65 7328 7363 6865 6d61 290a  e_names(schema).
-000099c0: 2020 2020 2020 2020 7461 626c 655f 6e61          table_na
-000099d0: 6d65 7320 3d20 5b74 2066 6f72 2074 2069  mes = [t for t i
-000099e0: 6e20 7461 626c 6573 2069 6620 7420 6e6f  n tables if t no
-000099f0: 7420 696e 205f 6967 6e6f 7265 5f74 6162  t in _ignore_tab
-00009a00: 6c65 735d 0a0a 2020 2020 2020 2020 6966  les]..        if
-00009a10: 206f 7264 6572 5f62 7920 3d3d 2022 666f   order_by == "fo
-00009a20: 7265 6967 6e5f 6b65 7922 3a0a 2020 2020  reign_key":.    
-00009a30: 2020 2020 2020 2020 616e 7377 6572 203d          answer =
-00009a40: 205b 2275 7365 7273 222c 2022 656d 6169   ["users", "emai
-00009a50: 6c5f 6164 6472 6573 7365 7322 2c20 2264  l_addresses", "d
-00009a60: 696e 6761 6c69 6e67 7322 5d0a 2020 2020  ingalings"].    
-00009a70: 2020 2020 2020 2020 6571 5f28 7461 626c          eq_(tabl
-00009a80: 655f 6e61 6d65 732c 2061 6e73 7765 7229  e_names, answer)
-00009a90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00009aa0: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
-00009ab0: 7220 3d20 5b22 6469 6e67 616c 696e 6773  r = ["dingalings
-00009ac0: 222c 2022 656d 6169 6c5f 6164 6472 6573  ", "email_addres
-00009ad0: 7365 7322 2c20 2275 7365 7273 225d 0a20  ses", "users"]. 
-00009ae0: 2020 2020 2020 2020 2020 2065 715f 2873             eq_(s
-00009af0: 6f72 7465 6428 7461 626c 655f 6e61 6d65  orted(table_name
-00009b00: 7329 2c20 616e 7377 6572 290a 0a20 2020  s), answer)..   
-00009b10: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00009b20: 2020 6465 6620 6465 6669 6e65 5f74 656d    def define_tem
-00009b30: 705f 7461 626c 6573 2863 6c73 2c20 6d65  p_tables(cls, me
-00009b40: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
-00009b50: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-00009b60: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-00009b70: 2020 2020 2020 2020 496e 2043 6c6f 7564          In Cloud
-00009b80: 2053 7061 6e6e 6572 2075 6e69 7175 6520   Spanner unique 
-00009b90: 696e 6465 7865 7320 6172 6520 7573 6564  indexes are used
-00009ba0: 2069 6e73 7465 6164 206f 6620 6469 7265   instead of dire
-00009bb0: 6374 6c79 0a20 2020 2020 2020 2063 7265  ctly.        cre
-00009bc0: 6174 696e 6720 756e 6971 7565 2063 6f6e  ating unique con
-00009bd0: 7374 7261 696e 7473 2e20 4f76 6572 7269  straints. Overri
-00009be0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-00009bf0: 2072 6570 6c61 6365 0a20 2020 2020 2020   replace.       
-00009c00: 2063 6f6e 7374 7261 696e 7473 2077 6974   constraints wit
-00009c10: 6820 696e 6465 7865 7320 696e 2074 6573  h indexes in tes
-00009c20: 7469 6e67 2064 6174 612e 0a20 2020 2020  ting data..     
-00009c30: 2020 2022 2222 0a20 2020 2020 2020 206b     """.        k
-00009c40: 7720 3d20 7465 6d70 5f74 6162 6c65 5f6b  w = temp_table_k
-00009c50: 6579 776f 7264 5f61 7267 7328 636f 6e66  eyword_args(conf
-00009c60: 6967 2c20 636f 6e66 6967 2e64 6229 0a20  ig, config.db). 
-00009c70: 2020 2020 2020 2075 7365 725f 746d 7020         user_tmp 
-00009c80: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
-00009c90: 2020 2020 2022 7573 6572 5f74 6d70 222c       "user_tmp",
-00009ca0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00009cb0: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
-00009cc0: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
-00009cd0: 7371 6c61 6c63 6865 6d79 2e49 4e54 2c20  sqlalchemy.INT, 
-00009ce0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00009cf0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00009d00: 6f6c 756d 6e28 226e 616d 6522 2c20 7371  olumn("name", sq
-00009d10: 6c61 6c63 6865 6d79 2e56 4152 4348 4152  lalchemy.VARCHAR
-00009d20: 2835 3029 292c 0a20 2020 2020 2020 2020  (50)),.         
-00009d30: 2020 2043 6f6c 756d 6e28 2266 6f6f 222c     Column("foo",
-00009d40: 2073 716c 616c 6368 656d 792e 494e 5429   sqlalchemy.INT)
-00009d50: 2c0a 2020 2020 2020 2020 2020 2020 7371  ,.            sq
-00009d60: 6c61 6c63 6865 6d79 2e49 6e64 6578 2822  lalchemy.Index("
-00009d70: 7573 6572 5f74 6d70 5f75 7122 2c20 226e  user_tmp_uq", "n
-00009d80: 616d 6522 2c20 756e 6971 7565 3d54 7275  ame", unique=Tru
-00009d90: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00009da0: 7371 6c61 6c63 6865 6d79 2e49 6e64 6578  sqlalchemy.Index
-00009db0: 2822 7573 6572 5f74 6d70 5f69 7822 2c20  ("user_tmp_ix", 
-00009dc0: 2266 6f6f 2229 2c0a 2020 2020 2020 2020  "foo"),.        
-00009dd0: 2020 2020 6578 7465 6e64 5f65 7869 7374      extend_exist
-00009de0: 696e 673d 5472 7565 2c0a 2020 2020 2020  ing=True,.      
-00009df0: 2020 2020 2020 2a2a 6b77 2c0a 2020 2020        **kw,.    
-00009e00: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00009e10: 2028 0a20 2020 2020 2020 2020 2020 2074   (.            t
-00009e20: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00009e30: 7669 6577 5f72 6566 6c65 6374 696f 6e2e  view_reflection.
-00009e40: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
-00009e50: 2020 2020 616e 6420 7465 7374 696e 672e      and testing.
-00009e60: 7265 7175 6972 6573 2e74 656d 706f 7261  requires.tempora
-00009e70: 7279 5f76 6965 7773 2e65 6e61 626c 6564  ry_views.enabled
-00009e80: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-00009e90: 2020 2020 2020 2020 6576 656e 742e 6c69          event.li
-00009ea0: 7374 656e 280a 2020 2020 2020 2020 2020  sten(.          
-00009eb0: 2020 2020 2020 7573 6572 5f74 6d70 2c0a        user_tmp,.
-00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 2261 6674 6572 5f63 7265 6174 6522 2c0a  "after_create",.
-00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ef0: 4444 4c28 2263 7265 6174 6520 7465 6d70  DDL("create temp
-00009f00: 6f72 6172 7920 7669 6577 2075 7365 725f  orary view user_
-00009f10: 746d 705f 7620 6173 2022 2022 7365 6c65  tmp_v as " "sele
-00009f20: 6374 202a 2066 726f 6d20 7573 6572 5f74  ct * from user_t
-00009f30: 6d70 2229 2c0a 2020 2020 2020 2020 2020  mp"),.          
-00009f40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00009f50: 6576 656e 742e 6c69 7374 656e 2875 7365  event.listen(use
-00009f60: 725f 746d 702c 2022 6265 666f 7265 5f64  r_tmp, "before_d
-00009f70: 726f 7022 2c20 4444 4c28 2264 726f 7020  rop", DDL("drop 
-00009f80: 7669 6577 2075 7365 725f 746d 705f 7622  view user_tmp_v"
-00009f90: 2929 0a0a 2020 2020 4074 6573 7469 6e67  ))..    @testing
-00009fa0: 2e70 726f 7669 6465 5f6d 6574 6164 6174  .provide_metadat
-00009fb0: 610a 2020 2020 6465 6620 7465 7374 5f72  a.    def test_r
-00009fc0: 6566 6c65 6374 5f73 7472 696e 675f 636f  eflect_string_co
-00009fd0: 6c75 6d6e 5f6d 6178 5f6c 656e 2873 656c  lumn_max_len(sel
-00009fe0: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
-00009ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000a000: 2020 2020 5350 414e 4e45 5220 5350 4543      SPANNER SPEC
-0000a010: 4946 4943 2054 4553 543a 0a0a 2020 2020  IFIC TEST:..    
-0000a020: 2020 2020 496e 2053 7061 6e6e 6572 2063      In Spanner c
-0000a030: 6f6c 756d 6e20 6f66 2074 6865 2053 5452  olumn of the STR
-0000a040: 494e 4720 7479 7065 2063 616e 2062 650a  ING type can be.
-0000a050: 2020 2020 2020 2020 6372 6561 7465 6420          created 
-0000a060: 7769 7468 2073 697a 6520 6465 6669 6e65  with size define
-0000a070: 6420 6173 204d 4158 2e20 5468 6520 7465  d as MAX. The te
-0000a080: 7374 0a20 2020 2020 2020 2063 6865 636b  st.        check
-0000a090: 7320 7468 6174 2073 7563 6820 6120 636f  s that such a co
-0000a0a0: 6c75 6d6e 2069 7320 636f 7272 6563 746c  lumn is correctl
-0000a0b0: 7920 7265 666c 6563 7465 642e 0a20 2020  y reflected..   
-0000a0c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000a0d0: 206d 6574 6164 6174 6120 3d20 4d65 7461   metadata = Meta
-0000a0e0: 4461 7461 2829 0a20 2020 2020 2020 2054  Data().        T
-0000a0f0: 6162 6c65 2822 7465 7874 5f74 6162 6c65  able("text_table
-0000a100: 222c 206d 6574 6164 6174 612c 2043 6f6c  ", metadata, Col
-0000a110: 756d 6e28 2254 6573 7443 6f6c 756d 6e22  umn("TestColumn"
-0000a120: 2c20 5465 7874 2c20 6e75 6c6c 6162 6c65  , Text, nullable
-0000a130: 3d46 616c 7365 2929 0a20 2020 2020 2020  =False)).       
-0000a140: 206d 6574 6164 6174 612e 6372 6561 7465   metadata.create
-0000a150: 5f61 6c6c 2863 6f6e 6e65 6374 696f 6e29  _all(connection)
-0000a160: 0a0a 2020 2020 2020 2020 5461 626c 6528  ..        Table(
-0000a170: 2274 6578 745f 7461 626c 6522 2c20 6d65  "text_table", me
-0000a180: 7461 6461 7461 2c20 6175 746f 6c6f 6164  tadata, autoload
-0000a190: 3d54 7275 6529 0a0a 2020 2020 6465 6620  =True)..    def 
-0000a1a0: 7465 7374 5f72 6566 6c65 6374 5f62 7974  test_reflect_byt
-0000a1b0: 6573 5f63 6f6c 756d 6e5f 6d61 785f 6c65  es_column_max_le
-0000a1c0: 6e28 7365 6c66 2c20 636f 6e6e 6563 7469  n(self, connecti
-0000a1d0: 6f6e 293a 0a20 2020 2020 2020 2022 2222  on):.        """
-0000a1e0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-0000a1f0: 2053 5045 4349 4649 4320 5445 5354 3a0a   SPECIFIC TEST:.
-0000a200: 0a20 2020 2020 2020 2049 6e20 5370 616e  .        In Span
-0000a210: 6e65 7220 636f 6c75 6d6e 206f 6620 7468  ner column of th
-0000a220: 6520 4259 5445 5320 7479 7065 2063 616e  e BYTES type can
-0000a230: 2062 650a 2020 2020 2020 2020 6372 6561   be.        crea
-0000a240: 7465 6420 7769 7468 2073 697a 6520 6465  ted with size de
-0000a250: 6669 6e65 6420 6173 204d 4158 2e20 5468  fined as MAX. Th
-0000a260: 6520 7465 7374 0a20 2020 2020 2020 2063  e test.        c
-0000a270: 6865 636b 7320 7468 6174 2073 7563 6820  hecks that such 
-0000a280: 6120 636f 6c75 6d6e 2069 7320 636f 7272  a column is corr
-0000a290: 6563 746c 7920 7265 666c 6563 7465 642e  ectly reflected.
-0000a2a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a2b0: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
-0000a2c0: 4d65 7461 4461 7461 2829 0a20 2020 2020  MetaData().     
-0000a2d0: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
-0000a2e0: 2020 2020 2020 2262 7974 6573 5f74 6162        "bytes_tab
-0000a2f0: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-0000a300: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-0000a310: 2020 2020 2020 2043 6f6c 756d 6e28 2254         Column("T
-0000a320: 6573 7443 6f6c 756d 6e22 2c20 4c61 7267  estColumn", Larg
-0000a330: 6542 696e 6172 792c 206e 756c 6c61 626c  eBinary, nullabl
-0000a340: 653d 4661 6c73 6529 2c0a 2020 2020 2020  e=False),.      
-0000a350: 2020 290a 2020 2020 2020 2020 6d65 7461    ).        meta
-0000a360: 6461 7461 2e63 7265 6174 655f 616c 6c28  data.create_all(
-0000a370: 636f 6e6e 6563 7469 6f6e 290a 0a20 2020  connection)..   
-0000a380: 2020 2020 2054 6162 6c65 2822 6279 7465       Table("byte
-0000a390: 735f 7461 626c 6522 2c20 6d65 7461 6461  s_table", metada
-0000a3a0: 7461 2c20 6175 746f 6c6f 6164 3d54 7275  ta, autoload=Tru
-0000a3b0: 6529 0a0a 2020 2020 4074 6573 7469 6e67  e)..    @testing
-0000a3c0: 2e72 6571 7569 7265 732e 756e 6971 7565  .requires.unique
-0000a3d0: 5f63 6f6e 7374 7261 696e 745f 7265 666c  _constraint_refl
-0000a3e0: 6563 7469 6f6e 0a20 2020 2064 6566 2074  ection.    def t
-0000a3f0: 6573 745f 6765 745f 756e 6971 7565 5f63  est_get_unique_c
-0000a400: 6f6e 7374 7261 696e 7473 2873 656c 662c  onstraints(self,
-0000a410: 206d 6574 6164 6174 612c 2063 6f6e 6e65   metadata, conne
-0000a420: 6374 696f 6e2c 2075 7365 5f73 6368 656d  ction, use_schem
-0000a430: 613d 4661 6c73 6529 3a0a 2020 2020 2020  a=False):.      
-0000a440: 2020 2320 5351 4c69 7465 2064 6961 6c65    # SQLite diale
-0000a450: 6374 206e 6565 6473 2074 6f20 7061 7273  ct needs to pars
-0000a460: 6520 7468 6520 6e61 6d65 7320 6f66 2074  e the names of t
-0000a470: 6865 2063 6f6e 7374 7261 696e 7473 0a20  he constraints. 
-0000a480: 2020 2020 2020 2023 2073 6570 6172 6174         # separat
-0000a490: 656c 7920 6672 6f6d 2077 6861 7420 6974  ely from what it
-0000a4a0: 2067 6574 7320 6672 6f6d 2050 5241 474d   gets from PRAGM
-0000a4b0: 4120 696e 6465 785f 6c69 7374 2829 2c20  A index_list(), 
-0000a4c0: 616e 640a 2020 2020 2020 2020 2320 7468  and.        # th
-0000a4d0: 656e 206d 6174 6368 6573 2074 6865 6d20  en matches them 
-0000a4e0: 7570 2e20 2073 6f20 7361 6d65 2073 6574  up.  so same set
-0000a4f0: 206f 6620 636f 6c75 6d6e 5f6e 616d 6573   of column_names
-0000a500: 2069 6e20 7477 6f0a 2020 2020 2020 2020   in two.        
-0000a510: 2320 636f 6e73 7472 6169 6e74 7320 7769  # constraints wi
-0000a520: 6c6c 2063 6f6e 6675 7365 2069 742e 2020  ll confuse it.  
-0000a530: 2020 5065 7268 6170 7320 7765 2073 686f    Perhaps we sho
-0000a540: 756c 6420 6e6f 206c 6f6e 6765 720a 2020  uld no longer.  
-0000a550: 2020 2020 2020 2320 626f 7468 6572 2077        # bother w
-0000a560: 6974 6820 696e 6465 785f 6c69 7374 2829  ith index_list()
-0000a570: 2068 6572 6520 7369 6e63 6520 7765 2068   here since we h
-0000a580: 6176 6520 7468 6520 7768 6f6c 650a 2020  ave the whole.  
-0000a590: 2020 2020 2020 2320 4352 4541 5445 2054        # CREATE T
-0000a5a0: 4142 4c45 3f0a 0a20 2020 2020 2020 2069  ABLE?..        i
-0000a5b0: 6620 7573 655f 7363 6865 6d61 3a0a 2020  f use_schema:.  
-0000a5c0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-0000a5d0: 203d 2063 6f6e 6669 672e 7465 7374 5f73   = config.test_s
-0000a5e0: 6368 656d 610a 2020 2020 2020 2020 656c  chema.        el
-0000a5f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a600: 7363 6865 6d61 203d 204e 6f6e 650a 2020  schema = None.  
-0000a610: 2020 2020 2020 756e 6971 7565 7320 3d20        uniques = 
-0000a620: 736f 7274 6564 280a 2020 2020 2020 2020  sorted(.        
-0000a630: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-0000a640: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
-0000a650: 756e 6971 7565 5f61 222c 2022 636f 6c75  unique_a", "colu
-0000a660: 6d6e 5f6e 616d 6573 223a 205b 2261 225d  mn_names": ["a"]
-0000a670: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-0000a680: 2020 207b 226e 616d 6522 3a20 2275 6e69     {"name": "uni
-0000a690: 7175 655f 615f 625f 6322 2c20 2263 6f6c  que_a_b_c", "col
-0000a6a0: 756d 6e5f 6e61 6d65 7322 3a20 5b22 6122  umn_names": ["a"
-0000a6b0: 2c20 2262 222c 2022 6322 5d7d 2c0a 2020  , "b", "c"]},.  
-0000a6c0: 2020 2020 2020 2020 2020 2020 2020 7b22                {"
-0000a6d0: 6e61 6d65 223a 2022 756e 6971 7565 5f63  name": "unique_c
-0000a6e0: 5f61 5f62 222c 2022 636f 6c75 6d6e 5f6e  _a_b", "column_n
-0000a6f0: 616d 6573 223a 205b 2263 222c 2022 6122  ames": ["c", "a"
-0000a700: 2c20 2262 225d 7d2c 0a20 2020 2020 2020  , "b"]},.       
-0000a710: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-0000a720: 3a20 2275 6e69 7175 655f 6173 635f 6b65  : "unique_asc_ke
-0000a730: 7922 2c20 2263 6f6c 756d 6e5f 6e61 6d65  y", "column_name
-0000a740: 7322 3a20 5b22 6173 6322 2c20 226b 6579  s": ["asc", "key
-0000a750: 225d 7d2c 0a20 2020 2020 2020 2020 2020  "]},.           
-0000a760: 2020 2020 207b 226e 616d 6522 3a20 2269       {"name": "i
-0000a770: 2e68 6176 652e 646f 7473 222c 2022 636f  .have.dots", "co
-0000a780: 6c75 6d6e 5f6e 616d 6573 223a 205b 2262  lumn_names": ["b
-0000a790: 225d 7d2c 0a20 2020 2020 2020 2020 2020  "]},.           
-0000a7a0: 2020 2020 207b 226e 616d 6522 3a20 2269       {"name": "i
-0000a7b0: 2068 6176 6520 7370 6163 6573 222c 2022   have spaces", "
-0000a7c0: 636f 6c75 6d6e 5f6e 616d 6573 223a 205b  column_names": [
-0000a7d0: 2263 225d 7d2c 0a20 2020 2020 2020 2020  "c"]},.         
-0000a7e0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-0000a7f0: 2020 6b65 793d 6f70 6572 6174 6f72 2e69    key=operator.i
-0000a800: 7465 6d67 6574 7465 7228 226e 616d 6522  temgetter("name"
-0000a810: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
-0000a820: 2020 2020 2074 6162 6c65 203d 2054 6162       table = Tab
-0000a830: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-0000a840: 2274 6573 7474 626c 222c 0a20 2020 2020  "testtbl",.     
-0000a850: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
-0000a860: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-0000a870: 756d 6e28 2269 6422 2c20 7371 6c61 6c63  umn("id", sqlalc
-0000a880: 6865 6d79 2e49 4e54 2c20 7072 696d 6172  hemy.INT, primar
-0000a890: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-0000a8a0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-0000a8b0: 2261 222c 2053 7472 696e 6728 3230 2929  "a", String(20))
-0000a8c0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-0000a8d0: 6c75 6d6e 2822 6222 2c20 5374 7269 6e67  lumn("b", String
-0000a8e0: 2833 3029 292c 0a20 2020 2020 2020 2020  (30)),.         
-0000a8f0: 2020 2043 6f6c 756d 6e28 2263 222c 2049     Column("c", I
-0000a900: 6e74 6567 6572 292c 0a20 2020 2020 2020  nteger),.       
-0000a910: 2020 2020 2023 2072 6573 6572 7665 6420       # reserved 
-0000a920: 6964 656e 7469 6669 6572 730a 2020 2020  identifiers.    
-0000a930: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-0000a940: 6173 6322 2c20 5374 7269 6e67 2833 3029  asc", String(30)
-0000a950: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-0000a960: 6f6c 756d 6e28 226b 6579 222c 2053 7472  olumn("key", Str
-0000a970: 696e 6728 3330 2929 2c0a 2020 2020 2020  ing(30)),.      
-0000a980: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-0000a990: 2e49 6e64 6578 2822 756e 6971 7565 5f61  .Index("unique_a
-0000a9a0: 222c 2022 6122 2c20 756e 6971 7565 3d54  ", "a", unique=T
-0000a9b0: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000a9c0: 2020 7371 6c61 6c63 6865 6d79 2e49 6e64    sqlalchemy.Ind
-0000a9d0: 6578 2822 756e 6971 7565 5f61 5f62 5f63  ex("unique_a_b_c
-0000a9e0: 222c 2022 6122 2c20 2262 222c 2022 6322  ", "a", "b", "c"
-0000a9f0: 2c20 756e 6971 7565 3d54 7275 6529 2c0a  , unique=True),.
-0000aa00: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-0000aa10: 6c63 6865 6d79 2e49 6e64 6578 2822 756e  lchemy.Index("un
-0000aa20: 6971 7565 5f63 5f61 5f62 222c 2022 6322  ique_c_a_b", "c"
-0000aa30: 2c20 2261 222c 2022 6222 2c20 756e 6971  , "a", "b", uniq
-0000aa40: 7565 3d54 7275 6529 2c0a 2020 2020 2020  ue=True),.      
-0000aa50: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-0000aa60: 2e49 6e64 6578 2822 756e 6971 7565 5f61  .Index("unique_a
-0000aa70: 7363 5f6b 6579 222c 2022 6173 6322 2c20  sc_key", "asc", 
-0000aa80: 226b 6579 222c 2075 6e69 7175 653d 5472  "key", unique=Tr
-0000aa90: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-0000aaa0: 2073 6368 656d 613d 7363 6865 6d61 2c0a   schema=schema,.
-0000aab0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000aac0: 2020 7461 626c 652e 6372 6561 7465 2863    table.create(c
-0000aad0: 6f6e 6e65 6374 696f 6e29 0a20 2020 2020  onnection).     
-0000aae0: 2020 2063 6f6e 6e65 6374 696f 6e2e 636f     connection.co
-0000aaf0: 6e6e 6563 7469 6f6e 2e63 6f6d 6d69 7428  nnection.commit(
-0000ab00: 290a 0a20 2020 2020 2020 2069 6e73 7065  )..        inspe
-0000ab10: 6374 6f72 203d 2069 6e73 7065 6374 2863  ctor = inspect(c
-0000ab20: 6f6e 6e65 6374 696f 6e29 0a20 2020 2020  onnection).     
-0000ab30: 2020 2072 6566 6c65 6374 6564 203d 2073     reflected = s
-0000ab40: 6f72 7465 6428 0a20 2020 2020 2020 2020  orted(.         
-0000ab50: 2020 2069 6e73 7065 6374 6f72 2e67 6574     inspector.get
-0000ab60: 5f75 6e69 7175 655f 636f 6e73 7472 6169  _unique_constrai
-0000ab70: 6e74 7328 2274 6573 7474 626c 222c 2073  nts("testtbl", s
-0000ab80: 6368 656d 613d 7363 6865 6d61 292c 0a20  chema=schema),. 
-0000ab90: 2020 2020 2020 2020 2020 206b 6579 3d6f             key=o
-0000aba0: 7065 7261 746f 722e 6974 656d 6765 7474  perator.itemgett
-0000abb0: 6572 2822 6e61 6d65 2229 2c0a 2020 2020  er("name"),.    
-0000abc0: 2020 2020 290a 0a20 2020 2020 2020 206e      )..        n
-0000abd0: 616d 6573 5f74 6861 745f 6475 706c 6963  ames_that_duplic
-0000abe0: 6174 655f 696e 6465 7820 3d20 7365 7428  ate_index = set(
-0000abf0: 290a 0a20 2020 2020 2020 2066 6f72 206f  )..        for o
-0000ac00: 7269 672c 2072 6566 6c20 696e 207a 6970  rig, refl in zip
-0000ac10: 2875 6e69 7175 6573 2c20 7265 666c 6563  (uniques, reflec
-0000ac20: 7465 6429 3a0a 2020 2020 2020 2020 2020  ted):.          
-0000ac30: 2020 2320 4469 6666 6572 656e 7420 6469    # Different di
-0000ac40: 616c 6563 7473 2068 616e 646c 6520 6475  alects handle du
-0000ac50: 706c 6963 6174 6520 696e 6465 7820 616e  plicate index an
-0000ac60: 6420 636f 6e73 7472 6169 6e74 730a 2020  d constraints.  
-0000ac70: 2020 2020 2020 2020 2020 2320 6469 6666            # diff
-0000ac80: 6572 656e 746c 792c 2073 6f20 6967 6e6f  erently, so igno
-0000ac90: 7265 2074 6869 7320 666c 6167 0a20 2020  re this flag.   
-0000aca0: 2020 2020 2020 2020 2064 7570 6520 3d20           dupe = 
-0000acb0: 7265 666c 2e70 6f70 2822 6475 706c 6963  refl.pop("duplic
-0000acc0: 6174 6573 5f69 6e64 6578 222c 204e 6f6e  ates_index", Non
-0000acd0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
-0000ace0: 6620 6475 7065 3a0a 2020 2020 2020 2020  f dupe:.        
-0000acf0: 2020 2020 2020 2020 6e61 6d65 735f 7468          names_th
-0000ad00: 6174 5f64 7570 6c69 6361 7465 5f69 6e64  at_duplicate_ind
-0000ad10: 6578 2e61 6464 2864 7570 6529 0a20 2020  ex.add(dupe).   
-0000ad20: 2020 2020 2020 2020 2065 715f 286f 7269           eq_(ori
-0000ad30: 672c 2072 6566 6c29 0a0a 2020 2020 2020  g, refl)..      
-0000ad40: 2020 7265 666c 6563 7465 645f 6d65 7461    reflected_meta
-0000ad50: 6461 7461 203d 204d 6574 6144 6174 6128  data = MetaData(
-0000ad60: 290a 2020 2020 2020 2020 7265 666c 6563  ).        reflec
-0000ad70: 7465 6420 3d20 5461 626c 6528 0a20 2020  ted = Table(.   
-0000ad80: 2020 2020 2020 2020 2022 7465 7374 7462           "testtb
-0000ad90: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-0000ada0: 7265 666c 6563 7465 645f 6d65 7461 6461  reflected_metada
-0000adb0: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-0000adc0: 6175 746f 6c6f 6164 5f77 6974 683d 636f  autoload_with=co
-0000add0: 6e6e 6563 7469 6f6e 2c0a 2020 2020 2020  nnection,.      
-0000ade0: 2020 2020 2020 7363 6865 6d61 3d73 6368        schema=sch
-0000adf0: 656d 612c 0a20 2020 2020 2020 2029 0a0a  ema,.        )..
-0000ae00: 2020 2020 2020 2020 2320 7465 7374 2022          # test "
-0000ae10: 6465 6475 706c 6963 6174 6573 2066 6f72  deduplicates for
-0000ae20: 2069 6e64 6578 2220 6c6f 6769 632e 2020   index" logic.  
-0000ae30: 204d 7953 514c 2061 6e64 204f 7261 636c   MySQL and Oracl
-0000ae40: 650a 2020 2020 2020 2020 2320 2275 6e69  e.        # "uni
-0000ae50: 7175 6520 636f 6e73 7472 6169 6e74 7322  que constraints"
-0000ae60: 2061 7265 2061 6374 7561 6c6c 7920 756e   are actually un
-0000ae70: 6971 7565 2069 6e64 6578 6573 2028 7769  ique indexes (wi
-0000ae80: 7468 2070 6f73 7369 626c 650a 2020 2020  th possible.    
-0000ae90: 2020 2020 2320 6578 6365 7074 696f 6e20      # exception 
-0000aea0: 6f66 2061 2075 6e69 7175 6520 7468 6174  of a unique that
-0000aeb0: 2069 7320 6120 6475 7065 206f 6620 616e   is a dupe of an
-0000aec0: 6f74 6865 7220 6f6e 6520 696e 2074 6865  other one in the
-0000aed0: 2063 6173 650a 2020 2020 2020 2020 2320   case.        # 
-0000aee0: 6f66 204f 7261 636c 6529 2e20 206d 616b  of Oracle).  mak
-0000aef0: 6520 7375 7265 2023 2074 6865 7920 6172  e sure # they ar
-0000af00: 656e 2774 2064 7570 6c69 6361 7465 642e  en't duplicated.
-0000af10: 0a20 2020 2020 2020 2069 6478 5f6e 616d  .        idx_nam
-0000af20: 6573 203d 2073 6574 285b 6964 782e 6e61  es = set([idx.na
-0000af30: 6d65 2066 6f72 2069 6478 2069 6e20 7265  me for idx in re
-0000af40: 666c 6563 7465 642e 696e 6465 7865 735d  flected.indexes]
-0000af50: 290a 2020 2020 2020 2020 7571 5f6e 616d  ).        uq_nam
-0000af60: 6573 203d 2073 6574 280a 2020 2020 2020  es = set(.      
-0000af70: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-0000af80: 2020 2020 2020 2020 7571 2e6e 616d 650a          uq.name.
-0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afa0: 666f 7220 7571 2069 6e20 7265 666c 6563  for uq in reflec
-0000afb0: 7465 642e 636f 6e73 7472 6169 6e74 730a  ted.constraints.
-0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afd0: 6966 2069 7369 6e73 7461 6e63 6528 7571  if isinstance(uq
-0000afe0: 2c20 7371 6c61 6c63 6865 6d79 2e55 6e69  , sqlalchemy.Uni
-0000aff0: 7175 6543 6f6e 7374 7261 696e 7429 0a20  queConstraint). 
-0000b000: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0000b010: 2020 2020 2029 2e64 6966 6665 7265 6e63       ).differenc
-0000b020: 6528 5b22 756e 6971 7565 5f63 5f61 5f62  e(["unique_c_a_b
-0000b030: 225d 290a 0a20 2020 2020 2020 2061 7373  "])..        ass
-0000b040: 6572 7420 6e6f 7420 6964 785f 6e61 6d65  ert not idx_name
-0000b050: 732e 696e 7465 7273 6563 7469 6f6e 2875  s.intersection(u
-0000b060: 715f 6e61 6d65 7329 0a20 2020 2020 2020  q_names).       
-0000b070: 2069 6620 6e61 6d65 735f 7468 6174 5f64   if names_that_d
-0000b080: 7570 6c69 6361 7465 5f69 6e64 6578 3a0a  uplicate_index:.
-0000b090: 2020 2020 2020 2020 2020 2020 6571 5f28              eq_(
-0000b0a0: 6e61 6d65 735f 7468 6174 5f64 7570 6c69  names_that_dupli
-0000b0b0: 6361 7465 5f69 6e64 6578 2c20 6964 785f  cate_index, idx_
-0000b0c0: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
-0000b0d0: 2020 2065 715f 2875 715f 6e61 6d65 732c     eq_(uq_names,
-0000b0e0: 2073 6574 2829 290a 0a20 2020 2040 7465   set())..    @te
-0000b0f0: 7374 696e 672e 7072 6f76 6964 655f 6d65  sting.provide_me
-0000b100: 7461 6461 7461 0a20 2020 2064 6566 2074  tadata.    def t
-0000b110: 6573 745f 756e 6971 7565 5f63 6f6e 7374  est_unique_const
-0000b120: 7261 696e 745f 7261 6973 6573 2873 656c  raint_raises(sel
-0000b130: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
-0000b140: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b150: 2020 2020 4368 6563 6b69 6e67 2074 6861      Checking tha
-0000b160: 7420 756e 6971 7565 2063 6f6e 7374 7261  t unique constra
-0000b170: 696e 7420 6372 6561 7469 6f6e 0a20 2020  int creation.   
-0000b180: 2020 2020 2066 6169 6c73 2064 7565 2074       fails due t
-0000b190: 6f20 6120 5072 6f67 7261 6d6d 696e 6745  o a ProgrammingE
-0000b1a0: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
-0000b1b0: 220a 2020 2020 2020 2020 6d65 7461 6461  ".        metada
-0000b1c0: 7461 203d 204d 6574 6144 6174 6128 290a  ta = MetaData().
-0000b1d0: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
-0000b1e0: 2020 2020 2020 2020 2020 2022 7573 6572             "user
-0000b1f0: 5f74 6d70 5f66 6169 6c75 7265 222c 0a20  _tmp_failure",. 
-0000b200: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-0000b210: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-0000b220: 2043 6f6c 756d 6e28 2269 6422 2c20 7371   Column("id", sq
-0000b230: 6c61 6c63 6865 6d79 2e49 4e54 2c20 7072  lalchemy.INT, pr
-0000b240: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
-0000b250: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-0000b260: 756d 6e28 226e 616d 6522 2c20 7371 6c61  umn("name", sqla
-0000b270: 6c63 6865 6d79 2e56 4152 4348 4152 2835  lchemy.VARCHAR(5
-0000b280: 3029 292c 0a20 2020 2020 2020 2020 2020  0)),.           
-0000b290: 2073 716c 616c 6368 656d 792e 556e 6971   sqlalchemy.Uniq
-0000b2a0: 7565 436f 6e73 7472 6169 6e74 2822 6e61  ueConstraint("na
-0000b2b0: 6d65 222c 206e 616d 653d 2275 7365 725f  me", name="user_
-0000b2c0: 746d 705f 7571 2229 2c0a 2020 2020 2020  tmp_uq"),.      
-0000b2d0: 2020 290a 0a20 2020 2020 2020 2077 6974    )..        wit
-0000b2e0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-0000b2f0: 7370 616e 6e65 725f 6462 6170 692e 6578  spanner_dbapi.ex
-0000b300: 6365 7074 696f 6e73 2e50 726f 6772 616d  ceptions.Program
-0000b310: 6d69 6e67 4572 726f 7229 3a0a 2020 2020  mingError):.    
-0000b320: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000b330: 2e63 7265 6174 655f 616c 6c28 636f 6e6e  .create_all(conn
-0000b340: 6563 7469 6f6e 290a 0a20 2020 2040 7465  ection)..    @te
-0000b350: 7374 696e 672e 7072 6f76 6964 655f 6d65  sting.provide_me
-0000b360: 7461 6461 7461 0a20 2020 2064 6566 205f  tadata.    def _
-0000b370: 7465 7374 5f67 6574 5f74 6162 6c65 5f6e  test_get_table_n
-0000b380: 616d 6573 2873 656c 662c 2073 6368 656d  ames(self, schem
-0000b390: 613d 4e6f 6e65 2c20 7461 626c 655f 7479  a=None, table_ty
-0000b3a0: 7065 3d22 7461 626c 6522 2c20 6f72 6465  pe="table", orde
-0000b3b0: 725f 6279 3d4e 6f6e 6529 3a0a 2020 2020  r_by=None):.    
-0000b3c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000b3d0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
-0000b3e0: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
-0000b3f0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
-0000b400: 7274 2074 656d 706f 7261 7279 2074 6162  rt temporary tab
-0000b410: 6c65 732c 2073 6f20 7265 616c 2074 6162  les, so real tab
-0000b420: 6c65 7320 6172 650a 2020 2020 2020 2020  les are.        
-0000b430: 7573 6564 2066 6f72 2074 6573 7469 6e67  used for testing
-0000b440: 2e20 4173 2074 6865 206f 7269 6769 6e61  . As the origina
-0000b450: 6c20 7465 7374 2065 7870 6563 7473 206f  l test expects o
-0000b460: 6e6c 7920 7265 616c 0a20 2020 2020 2020  nly real.       
-0000b470: 2074 6162 6c65 7320 746f 2062 6520 7265   tables to be re
-0000b480: 6164 2c20 616e 6420 696e 2053 7061 6e6e  ad, and in Spann
-0000b490: 6572 2061 6c6c 2074 6865 2074 6162 6c65  er all the table
-0000b4a0: 7320 6172 6520 7265 616c 2c0a 2020 2020  s are real,.    
-0000b4b0: 2020 2020 6578 7065 6374 6564 2072 6573      expected res
-0000b4c0: 756c 7473 206f 7665 7272 6964 6520 6973  ults override is
-0000b4d0: 2072 6571 7569 7265 642e 0a20 2020 2020   required..     
-0000b4e0: 2020 2022 2222 0a20 2020 2020 2020 205f     """.        _
-0000b4f0: 6967 6e6f 7265 5f74 6162 6c65 7320 3d20  ignore_tables = 
-0000b500: 5b0a 2020 2020 2020 2020 2020 2020 2263  [.            "c
-0000b510: 6f6d 6d65 6e74 5f74 6573 7422 2c0a 2020  omment_test",.  
-0000b520: 2020 2020 2020 2020 2020 226e 6f6e 636f            "nonco
-0000b530: 6c5f 6964 785f 7465 7374 5f70 6b22 2c0a  l_idx_test_pk",.
-0000b540: 2020 2020 2020 2020 2020 2020 226e 6f6e              "non
-0000b550: 636f 6c5f 6964 785f 7465 7374 5f6e 6f70  col_idx_test_nop
-0000b560: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
-0000b570: 226c 6f63 616c 5f74 6162 6c65 222c 0a20  "local_table",. 
-0000b580: 2020 2020 2020 2020 2020 2022 7265 6d6f             "remo
-0000b590: 7465 5f74 6162 6c65 222c 0a20 2020 2020  te_table",.     
-0000b5a0: 2020 2020 2020 2022 7265 6d6f 7465 5f74         "remote_t
-0000b5b0: 6162 6c65 5f32 222c 0a20 2020 2020 2020  able_2",.       
-0000b5c0: 2020 2020 2022 6e6f 5f63 6f6e 7374 7261       "no_constra
-0000b5d0: 696e 7473 222c 0a20 2020 2020 2020 205d  ints",.        ]
-0000b5e0: 0a20 2020 2020 2020 206d 6574 6120 3d20  .        meta = 
-0000b5f0: 7365 6c66 2e6d 6574 6164 6174 610a 0a20  self.metadata.. 
-0000b600: 2020 2020 2020 2069 6e73 7020 3d20 696e         insp = in
-0000b610: 7370 6563 7428 6d65 7461 2e62 696e 6429  spect(meta.bind)
-0000b620: 0a0a 2020 2020 2020 2020 6966 2074 6162  ..        if tab
-0000b630: 6c65 5f74 7970 6520 3d3d 2022 7669 6577  le_type == "view
-0000b640: 2220 616e 6420 6e6f 7420 626f 6f6c 286f  " and not bool(o
-0000b650: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
-0000b660: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
-0000b670: 484f 5354 2229 293a 0a20 2020 2020 2020  HOST")):.       
-0000b680: 2020 2020 2074 6162 6c65 5f6e 616d 6573       table_names
-0000b690: 203d 2069 6e73 702e 6765 745f 7669 6577   = insp.get_view
-0000b6a0: 5f6e 616d 6573 2873 6368 656d 6129 0a20  _names(schema). 
-0000b6b0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-0000b6c0: 5f6e 616d 6573 2e73 6f72 7428 290a 2020  _names.sort().  
-0000b6d0: 2020 2020 2020 2020 2020 616e 7377 6572            answer
-0000b6e0: 203d 205b 2265 6d61 696c 5f61 6464 7265   = ["email_addre
-0000b6f0: 7373 6573 5f76 222c 2022 7573 6572 735f  sses_v", "users_
-0000b700: 7622 5d0a 2020 2020 2020 2020 2020 2020  v"].            
-0000b710: 6571 5f28 736f 7274 6564 2874 6162 6c65  eq_(sorted(table
-0000b720: 5f6e 616d 6573 292c 2061 6e73 7765 7229  _names), answer)
-0000b730: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000b740: 2020 2020 2020 2020 2020 2069 6620 6f72             if or
-0000b750: 6465 725f 6279 3a0a 2020 2020 2020 2020  der_by:.        
-0000b760: 2020 2020 2020 2020 7461 626c 6573 203d          tables =
-0000b770: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-0000b780: 2020 2020 2020 2072 6563 5b30 5d0a 2020         rec[0].  
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2020 666f 7220 7265 6320 696e 2069 6e73    for rec in ins
-0000b7b0: 702e 6765 745f 736f 7274 6564 5f74 6162  p.get_sorted_tab
-0000b7c0: 6c65 5f61 6e64 5f66 6b63 5f6e 616d 6573  le_and_fkc_names
-0000b7d0: 2873 6368 656d 6129 0a20 2020 2020 2020  (schema).       
-0000b7e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000b7f0: 7265 635b 305d 0a20 2020 2020 2020 2020  rec[0].         
-0000b800: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0000b810: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b820: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-0000b830: 7320 3d20 696e 7370 2e67 6574 5f74 6162  s = insp.get_tab
-0000b840: 6c65 5f6e 616d 6573 2873 6368 656d 6129  le_names(schema)
-0000b850: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-0000b860: 6c65 5f6e 616d 6573 203d 205b 7420 666f  le_names = [t fo
-0000b870: 7220 7420 696e 2074 6162 6c65 7320 6966  r t in tables if
-0000b880: 2074 206e 6f74 2069 6e20 5f69 676e 6f72   t not in _ignor
-0000b890: 655f 7461 626c 6573 5d0a 0a20 2020 2020  e_tables]..     
-0000b8a0: 2020 2020 2020 2069 6620 6f72 6465 725f         if order_
-0000b8b0: 6279 203d 3d20 2266 6f72 6569 676e 5f6b  by == "foreign_k
-0000b8c0: 6579 223a 0a20 2020 2020 2020 2020 2020  ey":.           
-0000b8d0: 2020 2020 2061 6e73 7765 7220 3d20 7b22       answer = {"
-0000b8e0: 6469 6e67 616c 696e 6773 222c 2022 656d  dingalings", "em
-0000b8f0: 6169 6c5f 6164 6472 6573 7365 7322 2c20  ail_addresses", 
-0000b900: 2275 7365 725f 746d 7022 2c20 2275 7365  "user_tmp", "use
-0000b910: 7273 227d 0a20 2020 2020 2020 2020 2020  rs"}.           
-0000b920: 2020 2020 2065 715f 2873 6574 2874 6162       eq_(set(tab
-0000b930: 6c65 5f6e 616d 6573 292c 2061 6e73 7765  le_names), answe
-0000b940: 7229 0a20 2020 2020 2020 2020 2020 2065  r).            e
-0000b950: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b960: 2020 2020 2061 6e73 7765 7220 3d20 5b22       answer = ["
-0000b970: 6469 6e67 616c 696e 6773 222c 2022 656d  dingalings", "em
-0000b980: 6169 6c5f 6164 6472 6573 7365 7322 2c20  ail_addresses", 
-0000b990: 2275 7365 725f 746d 7022 2c20 2275 7365  "user_tmp", "use
-0000b9a0: 7273 225d 0a20 2020 2020 2020 2020 2020  rs"].           
-0000b9b0: 2020 2020 2065 715f 2873 6f72 7465 6428       eq_(sorted(
-0000b9c0: 7461 626c 655f 6e61 6d65 7329 2c20 616e  table_names), an
-0000b9d0: 7377 6572 290a 0a20 2020 2040 7079 7465  swer)..    @pyte
-0000b9e0: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
-0000b9f0: 2020 2020 2020 2020 626f 6f6c 286f 732e          bool(os.
-0000ba00: 656e 7669 726f 6e2e 6765 7428 2253 5041  environ.get("SPA
-0000ba10: 4e4e 4552 5f45 4d55 4c41 544f 525f 484f  NNER_EMULATOR_HO
-0000ba20: 5354 2229 292c 2072 6561 736f 6e3d 2253  ST")), reason="S
-0000ba30: 6b69 7070 6564 206f 6e20 656d 756c 6174  kipped on emulat
-0000ba40: 6f72 220a 2020 2020 290a 2020 2020 6465  or".    ).    de
-0000ba50: 6620 7465 7374 5f67 6574 5f76 6965 775f  f test_get_view_
-0000ba60: 6e61 6d65 7328 7365 6c66 2c20 636f 6e6e  names(self, conn
-0000ba70: 6563 7469 6f6e 2c20 7573 655f 7363 6865  ection, use_sche
-0000ba80: 6d61 3d46 616c 7365 293a 0a20 2020 2020  ma=False):.     
-0000ba90: 2020 2069 6e73 7020 3d20 696e 7370 6563     insp = inspec
-0000baa0: 7428 636f 6e6e 6563 7469 6f6e 290a 2020  t(connection).  
-0000bab0: 2020 2020 2020 7363 6865 6d61 203d 204e        schema = N
-0000bac0: 6f6e 650a 2020 2020 2020 2020 7461 626c  one.        tabl
-0000bad0: 655f 6e61 6d65 7320 3d20 696e 7370 2e67  e_names = insp.g
-0000bae0: 6574 5f76 6965 775f 6e61 6d65 7328 7363  et_view_names(sc
-0000baf0: 6865 6d61 290a 2020 2020 2020 2020 6966  hema).        if
-0000bb00: 2074 6573 7469 6e67 2e72 6571 7569 7265   testing.require
-0000bb10: 732e 6d61 7465 7269 616c 697a 6564 5f76  s.materialized_v
-0000bb20: 6965 7773 2e65 6e61 626c 6564 3a0a 2020  iews.enabled:.  
-0000bb30: 2020 2020 2020 2020 2020 6571 5f28 736f            eq_(so
-0000bb40: 7274 6564 2874 6162 6c65 5f6e 616d 6573  rted(table_names
-0000bb50: 292c 205b 2265 6d61 696c 5f61 6464 7265  ), ["email_addre
-0000bb60: 7373 6573 5f76 222c 2022 7573 6572 735f  sses_v", "users_
-0000bb70: 7622 5d29 0a20 2020 2020 2020 2020 2020  v"]).           
-0000bb80: 2065 715f 2869 6e73 702e 6765 745f 6d61   eq_(insp.get_ma
-0000bb90: 7465 7269 616c 697a 6564 5f76 6965 775f  terialized_view_
-0000bba0: 6e61 6d65 7328 7363 6865 6d61 292c 205b  names(schema), [
-0000bbb0: 2264 696e 6761 6c69 6e67 735f 7622 5d29  "dingalings_v"])
-0000bbc0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000bbd0: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
-0000bbe0: 7220 3d20 5b22 6469 6e67 616c 696e 6773  r = ["dingalings
-0000bbf0: 5f76 222c 2022 656d 6169 6c5f 6164 6472  _v", "email_addr
-0000bc00: 6573 7365 735f 7622 2c20 2275 7365 7273  esses_v", "users
-0000bc10: 5f76 225d 0a20 2020 2020 2020 2020 2020  _v"].           
-0000bc20: 2065 715f 2873 6f72 7465 6428 7461 626c   eq_(sorted(tabl
-0000bc30: 655f 6e61 6d65 7329 2c20 616e 7377 6572  e_names), answer
-0000bc40: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
-0000bc50: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
-0000bc60: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
-0000bc70: 7420 7465 6d70 6f72 6172 7920 7461 626c  t temporary tabl
-0000bc80: 6573 2229 0a20 2020 2064 6566 2074 6573  es").    def tes
-0000bc90: 745f 6765 745f 7465 6d70 5f74 6162 6c65  t_get_temp_table
-0000bca0: 5f69 6e64 6578 6573 2873 656c 6629 3a0a  _indexes(self):.
-0000bcb0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000bcc0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-0000bcd0: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-0000bce0: 736e 2774 2073 7570 706f 7274 2074 656d  sn't support tem
-0000bcf0: 706f 7261 7279 2074 6162 6c65 7322 290a  porary tables").
-0000bd00: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-0000bd10: 5f74 656d 705f 7461 626c 655f 756e 6971  _temp_table_uniq
-0000bd20: 7565 5f63 6f6e 7374 7261 696e 7473 2873  ue_constraints(s
-0000bd30: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0000bd40: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-0000bd50: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
-0000bd60: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
-0000bd70: 7274 2074 656d 706f 7261 7279 2074 6162  rt temporary tab
-0000bd80: 6c65 7322 290a 2020 2020 6465 6620 7465  les").    def te
-0000bd90: 7374 5f67 6574 5f74 656d 705f 7461 626c  st_get_temp_tabl
-0000bda0: 655f 636f 6c75 6d6e 7328 7365 6c66 293a  e_columns(self):
-0000bdb0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0000bdc0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-0000bdd0: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
-0000bde0: 6573 6e27 7420 7375 7070 6f72 7420 7465  esn't support te
-0000bdf0: 6d70 6f72 6172 7920 7461 626c 6573 2229  mporary tables")
-0000be00: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-0000be10: 666c 6563 745f 7461 626c 655f 7465 6d70  flect_table_temp
-0000be20: 5f74 6162 6c65 2873 656c 662c 2063 6f6e  _table(self, con
-0000be30: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-0000be40: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0000be50: 6578 705f 696e 6465 7865 7328 0a20 2020  exp_indexes(.   
-0000be60: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000be70: 2020 2073 6368 656d 613d 4e6f 6e65 2c0a     schema=None,.
-0000be80: 2020 2020 2020 2020 7363 6f70 653d 4f62          scope=Ob
-0000be90: 6a65 6374 5363 6f70 652e 414e 592c 0a20  jectScope.ANY,. 
-0000bea0: 2020 2020 2020 206b 696e 643d 4f62 6a65         kind=Obje
-0000beb0: 6374 4b69 6e64 2e41 4e59 2c0a 2020 2020  ctKind.ANY,.    
-0000bec0: 2020 2020 6669 6c74 6572 5f6e 616d 6573      filter_names
-0000bed0: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
-0000bee0: 2020 2020 2020 6465 6620 6964 7828 0a20        def idx(. 
-0000bef0: 2020 2020 2020 2020 2020 202a 636f 6c73             *cols
-0000bf00: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
-0000bf10: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0000bf20: 756e 6971 7565 3d46 616c 7365 2c0a 2020  unique=False,.  
-0000bf30: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-0000bf40: 5f73 6f72 7469 6e67 3d4e 6f6e 652c 0a20  _sorting=None,. 
-0000bf50: 2020 2020 2020 2020 2020 2064 7570 6c69             dupli
-0000bf60: 6361 7465 733d 4661 6c73 652c 0a20 2020  cates=False,.   
-0000bf70: 2020 2020 2020 2020 2066 6b3d 4661 6c73           fk=Fals
-0000bf80: 652c 0a20 2020 2020 2020 2029 3a0a 2020  e,.        ):.  
-0000bf90: 2020 2020 2020 2020 2020 666b 5f72 6571            fk_req
-0000bfa0: 203d 2074 6573 7469 6e67 2e72 6571 7569   = testing.requi
-0000bfb0: 7265 732e 666f 7265 6967 6e5f 6b65 7973  res.foreign_keys
-0000bfc0: 5f72 6566 6c65 6374 5f61 735f 696e 6465  _reflect_as_inde
-0000bfd0: 780a 2020 2020 2020 2020 2020 2020 6475  x.            du
-0000bfe0: 705f 7265 7120 3d20 7465 7374 696e 672e  p_req = testing.
-0000bff0: 7265 7175 6972 6573 2e75 6e69 7175 655f  requires.unique_
-0000c000: 636f 6e73 7472 6169 6e74 735f 7265 666c  constraints_refl
-0000c010: 6563 745f 6173 5f69 6e64 6578 0a20 2020  ect_as_index.   
-0000c020: 2020 2020 2020 2020 2069 6620 2866 6b20           if (fk 
-0000c030: 616e 6420 6e6f 7420 666b 5f72 6571 2e65  and not fk_req.e
-0000c040: 6e61 626c 6564 2920 6f72 2028 6475 706c  nabled) or (dupl
-0000c050: 6963 6174 6573 2061 6e64 206e 6f74 2064  icates and not d
-0000c060: 7570 5f72 6571 2e65 6e61 626c 6564 293a  up_req.enabled):
-0000c070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c080: 2072 6574 7572 6e20 2829 0a20 2020 2020   return ().     
-0000c090: 2020 2020 2020 2072 6573 203d 207b 0a20         res = {. 
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c0b0: 756e 6971 7565 223a 2075 6e69 7175 652c  unique": unique,
-0000c0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c0d0: 2022 636f 6c75 6d6e 5f6e 616d 6573 223a   "column_names":
-0000c0e0: 206c 6973 7428 636f 6c73 292c 0a20 2020   list(cols),.   
-0000c0f0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-0000c100: 6d65 223a 206e 616d 652c 0a20 2020 2020  me": name,.     
-0000c110: 2020 2020 2020 2020 2020 2022 6469 616c             "dial
-0000c120: 6563 745f 6f70 7469 6f6e 7322 3a20 6d6f  ect_options": mo
-0000c130: 636b 2e41 4e59 2c0a 2020 2020 2020 2020  ck.ANY,.        
-0000c140: 2020 2020 2020 2020 2269 6e63 6c75 6465          "include
-0000c150: 5f63 6f6c 756d 6e73 223a 205b 5d2c 0a20  _columns": [],. 
-0000c160: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0000c170: 2020 2020 2020 2020 2069 6620 636f 6c75           if colu
-0000c180: 6d6e 5f73 6f72 7469 6e67 3a0a 2020 2020  mn_sorting:.    
-0000c190: 2020 2020 2020 2020 2020 2020 7265 735b              res[
-0000c1a0: 2263 6f6c 756d 6e5f 736f 7274 696e 6722  "column_sorting"
-0000c1b0: 5d20 3d20 7b22 7122 3a20 2244 4553 4322  ] = {"q": "DESC"
-0000c1c0: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-0000c1d0: 2064 7570 6c69 6361 7465 733a 0a20 2020   duplicates:.   
-0000c1e0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000c1f0: 5b22 6475 706c 6963 6174 6573 5f63 6f6e  ["duplicates_con
-0000c200: 7374 7261 696e 7422 5d20 3d20 6e61 6d65  straint"] = name
-0000c210: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000c220: 7572 6e20 5b72 6573 5d0a 0a20 2020 2020  urn [res]..     
-0000c230: 2020 206d 6174 6572 6961 6c69 7a65 6420     materialized 
-0000c240: 3d20 7b28 7363 6865 6d61 2c20 2264 696e  = {(schema, "din
-0000c250: 6761 6c69 6e67 735f 7622 293a 205b 5d7d  galings_v"): []}
-0000c260: 0a20 2020 2020 2020 2076 6965 7773 203d  .        views =
-0000c270: 207b 0a20 2020 2020 2020 2020 2020 2028   {.            (
-0000c280: 7363 6865 6d61 2c20 2265 6d61 696c 5f61  schema, "email_a
-0000c290: 6464 7265 7373 6573 5f76 2229 3a20 5b5d  ddresses_v"): []
-0000c2a0: 2c0a 2020 2020 2020 2020 2020 2020 2873  ,.            (s
-0000c2b0: 6368 656d 612c 2022 7573 6572 735f 7622  chema, "users_v"
-0000c2c0: 293a 205b 5d2c 0a20 2020 2020 2020 2020  ): [],.         
-0000c2d0: 2020 2028 7363 6865 6d61 2c20 2275 7365     (schema, "use
-0000c2e0: 725f 746d 705f 7622 293a 205b 5d2c 0a20  r_tmp_v"): [],. 
-0000c2f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0000c300: 2073 656c 662e 5f72 6573 6f6c 7665 5f76   self._resolve_v
-0000c310: 6965 7773 2876 6965 7773 2c20 6d61 7465  iews(views, mate
-0000c320: 7269 616c 697a 6564 290a 2020 2020 2020  rialized).      
-0000c330: 2020 6966 206d 6174 6572 6961 6c69 7a65    if materialize
-0000c340: 643a 0a20 2020 2020 2020 2020 2020 206d  d:.            m
-0000c350: 6174 6572 6961 6c69 7a65 645b 2873 6368  aterialized[(sch
-0000c360: 656d 612c 2022 6469 6e67 616c 696e 6773  ema, "dingalings
-0000c370: 5f76 2229 5d2e 6578 7465 6e64 2869 6478  _v")].extend(idx
-0000c380: 2822 6461 7461 222c 206e 616d 653d 226d  ("data", name="m
-0000c390: 6174 5f69 6e64 6578 2229 290a 2020 2020  at_index")).    
-0000c3a0: 2020 2020 7461 626c 6573 203d 207b 0a20      tables = {. 
-0000c3b0: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
-0000c3c0: 6d61 2c20 2275 7365 7273 2229 3a20 5b0a  ma, "users"): [.
-0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3e0: 2a69 6478 2822 7061 7265 6e74 5f75 7365  *idx("parent_use
-0000c3f0: 725f 6964 222c 206e 616d 653d 2275 7365  r_id", name="use
-0000c400: 725f 6964 5f66 6b22 2c20 666b 3d54 7275  r_id_fk", fk=Tru
-0000c410: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-0000c420: 2020 2020 2a69 6478 2822 7573 6572 5f69      *idx("user_i
-0000c430: 6422 2c20 2274 6573 7432 222c 2022 7465  d", "test2", "te
-0000c440: 7374 3122 2c20 6e61 6d65 3d22 7573 6572  st1", name="user
-0000c450: 735f 616c 6c5f 6964 7822 292c 0a20 2020  s_all_idx"),.   
-0000c460: 2020 2020 2020 2020 2020 2020 202a 6964               *id
-0000c470: 7828 2274 6573 7431 222c 2022 7465 7374  x("test1", "test
-0000c480: 3222 2c20 6e61 6d65 3d22 7573 6572 735f  2", name="users_
-0000c490: 745f 6964 7822 2c20 756e 6971 7565 3d54  t_idx", unique=T
-0000c4a0: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000c4b0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-0000c4c0: 2028 7363 6865 6d61 2c20 2264 696e 6761   (schema, "dinga
-0000c4d0: 6c69 6e67 7322 293a 205b 0a20 2020 2020  lings"): [.     
-0000c4e0: 2020 2020 2020 2020 2020 202a 6964 7828             *idx(
-0000c4f0: 2264 6174 6122 2c20 6e61 6d65 3d6d 6f63  "data", name=moc
-0000c500: 6b2e 414e 592c 2075 6e69 7175 653d 5472  k.ANY, unique=Tr
-0000c510: 7565 2c20 6475 706c 6963 6174 6573 3d54  ue, duplicates=T
-0000c520: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000c530: 2020 2020 2020 2a69 6478 2822 6964 5f75        *idx("id_u
-0000c540: 7365 7222 2c20 6e61 6d65 3d6d 6f63 6b2e  ser", name=mock.
-0000c550: 414e 592c 2066 6b3d 5472 7565 292c 0a20  ANY, fk=True),. 
-0000c560: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000c570: 6964 7828 0a20 2020 2020 2020 2020 2020  idx(.           
-0000c580: 2020 2020 2020 2020 2022 6164 6472 6573           "addres
-0000c590: 735f 6964 222c 0a20 2020 2020 2020 2020  s_id",.         
-0000c5a0: 2020 2020 2020 2020 2020 2022 6469 6e67             "ding
-0000c5b0: 616c 696e 675f 6964 222c 0a20 2020 2020  aling_id",.     
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000c5d0: 616d 653d 227a 7a5f 6469 6e67 616c 696e  ame="zz_dingalin
-0000c5e0: 6773 5f6d 756c 7469 706c 6522 2c0a 2020  gs_multiple",.  
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c600: 2020 756e 6971 7565 3d54 7275 652c 0a20    unique=True,. 
-0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2020 2064 7570 6c69 6361 7465 733d 5472     duplicates=Tr
-0000c630: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000c640: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-0000c650: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-0000c660: 2020 2873 6368 656d 612c 2022 656d 6169    (schema, "emai
-0000c670: 6c5f 6164 6472 6573 7365 7322 293a 205b  l_addresses"): [
-0000c680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c690: 202a 6964 7828 2265 6d61 696c 5f61 6464   *idx("email_add
-0000c6a0: 7265 7373 222c 206e 616d 653d 6d6f 636b  ress", name=mock
-0000c6b0: 2e41 4e59 292c 0a20 2020 2020 2020 2020  .ANY),.         
-0000c6c0: 2020 2020 2020 202a 6964 7828 2272 656d         *idx("rem
-0000c6d0: 6f74 655f 7573 6572 5f69 6422 2c20 6e61  ote_user_id", na
-0000c6e0: 6d65 3d6d 6f63 6b2e 414e 592c 2066 6b3d  me=mock.ANY, fk=
-0000c6f0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-0000c700: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-0000c710: 2020 2873 6368 656d 612c 2022 636f 6d6d    (schema, "comm
-0000c720: 656e 745f 7465 7374 2229 3a20 5b5d 2c0a  ent_test"): [],.
-0000c730: 2020 2020 2020 2020 2020 2020 2873 6368              (sch
-0000c740: 656d 612c 2022 6e6f 5f63 6f6e 7374 7261  ema, "no_constra
-0000c750: 696e 7473 2229 3a20 5b5d 2c0a 2020 2020  ints"): [],.    
-0000c760: 2020 2020 2020 2020 2873 6368 656d 612c          (schema,
-0000c770: 2022 6c6f 6361 6c5f 7461 626c 6522 293a   "local_table"):
-0000c780: 205b 2a69 6478 2822 7265 6d6f 7465 5f69   [*idx("remote_i
-0000c790: 6422 2c20 6e61 6d65 3d6d 6f63 6b2e 414e  d", name=mock.AN
-0000c7a0: 592c 2066 6b3d 5472 7565 295d 2c0a 2020  Y, fk=True)],.  
-0000c7b0: 2020 2020 2020 2020 2020 2873 6368 656d            (schem
-0000c7c0: 612c 2022 7265 6d6f 7465 5f74 6162 6c65  a, "remote_table
-0000c7d0: 2229 3a20 5b2a 6964 7828 226c 6f63 616c  "): [*idx("local
-0000c7e0: 5f69 6422 2c20 6e61 6d65 3d6d 6f63 6b2e  _id", name=mock.
-0000c7f0: 414e 592c 2066 6b3d 5472 7565 295d 2c0a  ANY, fk=True)],.
-0000c800: 2020 2020 2020 2020 2020 2020 2873 6368              (sch
-0000c810: 656d 612c 2022 7265 6d6f 7465 5f74 6162  ema, "remote_tab
-0000c820: 6c65 5f32 2229 3a20 5b5d 2c0a 2020 2020  le_2"): [],.    
-0000c830: 2020 2020 2020 2020 2873 6368 656d 612c          (schema,
-0000c840: 2022 6e6f 6e63 6f6c 5f69 6478 5f74 6573   "noncol_idx_tes
-0000c850: 745f 6e6f 706b 2229 3a20 5b0a 2020 2020  t_nopk"): [.    
-0000c860: 2020 2020 2020 2020 2020 2020 2a69 6478              *idx
-0000c870: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c880: 2020 2020 2020 2271 222c 0a20 2020 2020        "q",.     
-0000c890: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000c8a0: 616d 653d 226e 6f6e 636f 6c5f 6964 785f  ame="noncol_idx_
-0000c8b0: 6e6f 706b 222c 0a20 2020 2020 2020 2020  nopk",.         
-0000c8c0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000c8d0: 6e5f 736f 7274 696e 673d 7b22 7122 3a20  n_sorting={"q": 
-0000c8e0: 2244 4553 4322 7d2c 0a20 2020 2020 2020  "DESC"},.       
-0000c8f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000c900: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-0000c910: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
-0000c920: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
-0000c930: 706b 2229 3a20 5b0a 2020 2020 2020 2020  pk"): [.        
-0000c940: 2020 2020 2020 2020 2a69 6478 2822 7122          *idx("q"
-0000c950: 2c20 6e61 6d65 3d22 6e6f 6e63 6f6c 5f69  , name="noncol_i
-0000c960: 6478 5f70 6b22 2c20 636f 6c75 6d6e 5f73  dx_pk", column_s
-0000c970: 6f72 7469 6e67 3d7b 2271 223a 2022 4445  orting={"q": "DE
-0000c980: 5343 227d 290a 2020 2020 2020 2020 2020  SC"}).          
-0000c990: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-0000c9a0: 2028 7363 6865 6d61 2c20 7365 6c66 2e74   (schema, self.t
-0000c9b0: 656d 705f 7461 626c 655f 6e61 6d65 2829  emp_table_name()
-0000c9c0: 293a 205b 0a20 2020 2020 2020 2020 2020  ): [.           
-0000c9d0: 2020 2020 202a 6964 7828 2266 6f6f 222c       *idx("foo",
-0000c9e0: 206e 616d 653d 2275 7365 725f 746d 705f   name="user_tmp_
-0000c9f0: 6978 2229 2c0a 2020 2020 2020 2020 2020  ix"),.          
-0000ca00: 2020 2020 2020 2a69 6478 280a 2020 2020        *idx(.    
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca20: 226e 616d 6522 2c0a 2020 2020 2020 2020  "name",.        
-0000ca30: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000ca40: 3d66 2275 7365 725f 746d 705f 7571 5f7b  =f"user_tmp_uq_{
-0000ca50: 636f 6e66 6967 2e69 6465 6e74 7d22 2c0a  config.ident}",.
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2020 2020 6475 706c 6963 6174 6573 3d54      duplicates=T
-0000ca80: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0000ca90: 2020 2020 2020 2020 2075 6e69 7175 653d           unique=
-0000caa0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000cab0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-0000cac0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-0000cad0: 7d0a 2020 2020 2020 2020 6966 2028 0a20  }.        if (. 
-0000cae0: 2020 2020 2020 2020 2020 206e 6f74 2074             not t
-0000caf0: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-0000cb00: 696e 6465 7865 735f 7769 7468 5f61 7363  indexes_with_asc
-0000cb10: 6465 7363 2e65 6e61 626c 6564 0a20 2020  desc.enabled.   
-0000cb20: 2020 2020 2020 2020 206f 7220 6e6f 7420           or not 
-0000cb30: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
-0000cb40: 2e72 6566 6c65 6374 5f69 6e64 6578 6573  .reflect_indexes
-0000cb50: 5f77 6974 685f 6173 6364 6573 632e 656e  _with_ascdesc.en
-0000cb60: 6162 6c65 640a 2020 2020 2020 2020 293a  abled.        ):
-0000cb70: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-0000cb80: 6c65 735b 2873 6368 656d 612c 2022 6e6f  les[(schema, "no
-0000cb90: 6e63 6f6c 5f69 6478 5f74 6573 745f 6e6f  ncol_idx_test_no
-0000cba0: 706b 2229 5d2e 636c 6561 7228 290a 2020  pk")].clear().  
-0000cbb0: 2020 2020 2020 2020 2020 7461 626c 6573            tables
-0000cbc0: 5b28 7363 6865 6d61 2c20 226e 6f6e 636f  [(schema, "nonco
-0000cbd0: 6c5f 6964 785f 7465 7374 5f70 6b22 295d  l_idx_test_pk")]
-0000cbe0: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
-0000cbf0: 2072 6573 203d 2073 656c 662e 5f72 6573   res = self._res
-0000cc00: 6f6c 7665 5f6b 696e 6428 6b69 6e64 2c20  olve_kind(kind, 
-0000cc10: 7461 626c 6573 2c20 7669 6577 732c 206d  tables, views, m
-0000cc20: 6174 6572 6961 6c69 7a65 6429 0a20 2020  aterialized).   
-0000cc30: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-0000cc40: 5f72 6573 6f6c 7665 5f6e 616d 6573 2873  _resolve_names(s
-0000cc50: 6368 656d 612c 2073 636f 7065 2c20 6669  chema, scope, fi
-0000cc60: 6c74 6572 5f6e 616d 6573 2c20 7265 7329  lter_names, res)
-0000cc70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cc80: 7265 730a 0a20 2020 2064 6566 205f 6368  res..    def _ch
-0000cc90: 6563 6b5f 6c69 7374 2873 656c 662c 2072  eck_list(self, r
-0000cca0: 6573 756c 742c 2065 7870 2c20 7265 715f  esult, exp, req_
-0000ccb0: 6b65 7973 3d4e 6f6e 652c 206d 7367 3d4e  keys=None, msg=N
-0000ccc0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-0000ccd0: 2072 6571 5f6b 6579 7320 6973 204e 6f6e   req_keys is Non
-0000cce0: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
-0000ccf0: 715f 2872 6573 756c 742c 2065 7870 2c20  q_(result, exp, 
-0000cd00: 6d73 6729 0a20 2020 2020 2020 2065 6c73  msg).        els
-0000cd10: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
-0000cd20: 715f 286c 656e 2872 6573 756c 7429 2c20  q_(len(result), 
-0000cd30: 6c65 6e28 6578 7029 2c20 6d73 6729 0a20  len(exp), msg). 
-0000cd40: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-0000cd50: 2c20 6520 696e 207a 6970 2872 6573 756c  , e in zip(resul
-0000cd60: 742c 2065 7870 293a 0a20 2020 2020 2020  t, exp):.       
-0000cd70: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-0000cd80: 6e20 7365 7428 7229 207c 2073 6574 2865  n set(r) | set(e
-0000cd90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000cda0: 2020 2020 2020 2069 6620 286b 2069 6e20         if (k in 
-0000cdb0: 7265 715f 6b65 7973 2061 6e64 2028 6b20  req_keys and (k 
-0000cdc0: 696e 2072 2061 6e64 206b 2069 6e20 6529  in r and k in e)
-0000cdd0: 2920 6f72 2028 6b20 696e 2072 2061 6e64  ) or (k in r and
-0000cde0: 206b 2069 6e20 6529 3a0a 2020 2020 2020   k in e):.      
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000ce10: 725b 6b5d 2c20 6c69 7374 293a 0a20 2020  r[k], list):.   
-0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 2020 2020 2020 2020 2072 5b6b 5d2e 736f           r[k].so
-0000ce40: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 2065 5b6b 5d2e 736f 7274 2829 0a20 2020   e[k].sort().   
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce80: 2020 2020 2065 715f 2872 5b6b 5d2c 2065       eq_(r[k], e
-0000ce90: 5b6b 5d2c 2066 227b 6d73 677d 202d 207b  [k], f"{msg} - {
-0000cea0: 6b7d 202d 207b 727d 2229 0a0a 2020 2020  k} - {r}")..    
-0000ceb0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-0000cec0: 7069 6628 0a20 2020 2020 2020 2062 6f6f  pif(.        boo
-0000ced0: 6c28 6f73 2e65 6e76 6972 6f6e 2e67 6574  l(os.environ.get
-0000cee0: 2822 5350 414e 4e45 525f 454d 554c 4154  ("SPANNER_EMULAT
-0000cef0: 4f52 5f48 4f53 5422 2929 2c20 7265 6173  OR_HOST")), reas
-0000cf00: 6f6e 3d22 536b 6970 7065 6420 6f6e 2065  on="Skipped on e
-0000cf10: 6d75 6c61 746f 7222 0a20 2020 2029 0a20  mulator".    ). 
-0000cf20: 2020 2040 7465 7374 696e 672e 636f 6d62     @testing.comb
-0000cf30: 696e 6174 696f 6e73 2854 7275 652c 2046  inations(True, F
-0000cf40: 616c 7365 2c20 6172 676e 616d 6573 3d22  alse, argnames="
-0000cf50: 7573 655f 7363 6865 6d61 2229 0a20 2020  use_schema").   
-0000cf60: 2040 7465 7374 696e 672e 636f 6d62 696e   @testing.combin
-0000cf70: 6174 696f 6e73 2828 5472 7565 2c20 7465  ations((True, te
-0000cf80: 7374 696e 672e 7265 7175 6972 6573 2e76  sting.requires.v
-0000cf90: 6965 7773 292c 2046 616c 7365 2c20 6172  iews), False, ar
-0000cfa0: 676e 616d 6573 3d22 7669 6577 7322 290a  gnames="views").
-0000cfb0: 2020 2020 6465 6620 7465 7374 5f6d 6574      def test_met
-0000cfc0: 6164 6174 6128 7365 6c66 2c20 636f 6e6e  adata(self, conn
-0000cfd0: 6563 7469 6f6e 2c20 7573 655f 7363 6865  ection, use_sche
-0000cfe0: 6d61 2c20 7669 6577 7329 3a0a 2020 2020  ma, views):.    
-0000cff0: 2020 2020 6d20 3d20 4d65 7461 4461 7461      m = MetaData
-0000d000: 2829 0a20 2020 2020 2020 2073 6368 656d  ().        schem
-0000d010: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
-0000d020: 206d 2e72 6566 6c65 6374 2863 6f6e 6e65   m.reflect(conne
-0000d030: 6374 696f 6e2c 2073 6368 656d 613d 7363  ction, schema=sc
-0000d040: 6865 6d61 2c20 7669 6577 733d 7669 6577  hema, views=view
-0000d050: 732c 2072 6573 6f6c 7665 5f66 6b73 3d46  s, resolve_fks=F
-0000d060: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
-0000d070: 6e73 7020 3d20 696e 7370 6563 7428 636f  nsp = inspect(co
-0000d080: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
-0000d090: 2020 7461 626c 6573 203d 2069 6e73 702e    tables = insp.
-0000d0a0: 6765 745f 7461 626c 655f 6e61 6d65 7328  get_table_names(
-0000d0b0: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
-0000d0c0: 6966 2076 6965 7773 3a0a 2020 2020 2020  if views:.      
-0000d0d0: 2020 2020 2020 7461 626c 6573 202b 3d20        tables += 
-0000d0e0: 696e 7370 2e67 6574 5f76 6965 775f 6e61  insp.get_view_na
-0000d0f0: 6d65 7328 7363 6865 6d61 290a 2020 2020  mes(schema).    
-0000d100: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000d110: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-0000d120: 6c65 7320 2b3d 2069 6e73 702e 6765 745f  les += insp.get_
-0000d130: 6d61 7465 7269 616c 697a 6564 5f76 6965  materialized_vie
-0000d140: 775f 6e61 6d65 7328 7363 6865 6d61 290a  w_names(schema).
-0000d150: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000d160: 7074 204e 6f74 496d 706c 656d 656e 7465  pt NotImplemente
-0000d170: 6445 7272 6f72 3a0a 2020 2020 2020 2020  dError:.        
-0000d180: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-0000d190: 2020 2020 2069 6620 7363 6865 6d61 2069       if schema i
-0000d1a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000d1b0: 2020 2020 2020 2020 7461 626c 6573 203d          tables =
-0000d1c0: 205b 6622 7b73 6368 656d 617d 2e7b 747d   [f"{schema}.{t}
-0000d1d0: 2220 666f 7220 7420 696e 2074 6162 6c65  " for t in table
-0000d1e0: 735d 0a20 2020 2020 2020 2065 715f 2873  s].        eq_(s
-0000d1f0: 6f72 7465 6428 6d2e 7461 626c 6573 292c  orted(m.tables),
-0000d200: 2073 6f72 7465 6428 7461 626c 6573 2929   sorted(tables))
-0000d210: 0a0a 0a63 6c61 7373 2043 6f6d 706f 7369  ...class Composi
-0000d220: 7465 4b65 7952 6566 6c65 6374 696f 6e54  teKeyReflectionT
-0000d230: 6573 7428 5f43 6f6d 706f 7369 7465 4b65  est(_CompositeKe
-0000d240: 7952 6566 6c65 6374 696f 6e54 6573 7429  yReflectionTest)
-0000d250: 3a0a 2020 2020 4074 6573 7469 6e67 2e72  :.    @testing.r
-0000d260: 6571 7569 7265 732e 666f 7265 6967 6e5f  equires.foreign_
-0000d270: 6b65 795f 636f 6e73 7472 6169 6e74 5f72  key_constraint_r
-0000d280: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
-0000d290: 6620 7465 7374 5f66 6b5f 636f 6c75 6d6e  f test_fk_column
-0000d2a0: 5f6f 7264 6572 2873 656c 662c 2063 6f6e  _order(self, con
-0000d2b0: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-0000d2c0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-0000d2d0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-0000d2e0: 0a20 2020 2020 2020 2053 7061 6e6e 6572  .        Spanner
-0000d2f0: 2063 6f6c 756d 6e20 7573 6167 6520 7265   column usage re
-0000d300: 666c 6563 7469 6f6e 2064 6f65 736e 2774  flection doesn't
-0000d310: 2073 7570 706f 7274 2064 6574 6572 6d65   support determe
-0000d320: 6e69 7374 6963 0a20 2020 2020 2020 206f  nistic.        o
-0000d330: 7264 6572 696e 672e 204f 7665 7272 6964  rdering. Overrid
-0000d340: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
-0000d350: 6368 6563 6b20 7468 6174 2063 6f6c 756d  check that colum
-0000d360: 6e73 2061 7265 0a20 2020 2020 2020 2072  ns are.        r
-0000d370: 6566 6c65 6374 6564 2063 6f72 7265 6374  eflected correct
-0000d380: 6c79 2c20 7769 7468 6f75 7420 636f 6e73  ly, without cons
-0000d390: 6964 6572 696e 6720 7468 6569 7220 6f72  idering their or
-0000d3a0: 6465 722e 0a20 2020 2020 2020 2022 2222  der..        """
-0000d3b0: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
-0000d3c0: 666f 7220 6973 7375 6520 2335 3636 310a  for issue #5661.
-0000d3d0: 2020 2020 2020 2020 696e 7370 203d 2069          insp = i
-0000d3e0: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
-0000d3f0: 6e29 0a20 2020 2020 2020 2066 6f72 6569  n).        forei
-0000d400: 676e 5f6b 6579 7320 3d20 696e 7370 2e67  gn_keys = insp.g
-0000d410: 6574 5f66 6f72 6569 676e 5f6b 6579 7328  et_foreign_keys(
-0000d420: 7365 6c66 2e74 6162 6c65 732e 7462 322e  self.tables.tb2.
-0000d430: 6e61 6d65 290a 2020 2020 2020 2020 6571  name).        eq
-0000d440: 5f28 6c65 6e28 666f 7265 6967 6e5f 6b65  _(len(foreign_ke
-0000d450: 7973 292c 2031 290a 2020 2020 2020 2020  ys), 1).        
-0000d460: 666b 6579 3120 3d20 666f 7265 6967 6e5f  fkey1 = foreign_
-0000d470: 6b65 7973 5b30 5d0a 2020 2020 2020 2020  keys[0].        
-0000d480: 6571 5f28 7365 7428 666b 6579 312e 6765  eq_(set(fkey1.ge
-0000d490: 7428 2272 6566 6572 7265 645f 636f 6c75  t("referred_colu
-0000d4a0: 6d6e 7322 2929 2c20 7b22 6e61 6d65 222c  mns")), {"name",
-0000d4b0: 2022 6964 222c 2022 6174 7472 227d 290a   "id", "attr"}).
-0000d4c0: 2020 2020 2020 2020 6571 5f28 7365 7428          eq_(set(
-0000d4d0: 666b 6579 312e 6765 7428 2263 6f6e 7374  fkey1.get("const
-0000d4e0: 7261 696e 6564 5f63 6f6c 756d 6e73 2229  rained_columns")
-0000d4f0: 292c 207b 2270 6e61 6d65 222c 2022 7069  ), {"pname", "pi
-0000d500: 6422 2c20 2270 6174 7472 227d 290a 0a20  d", "pattr"}).. 
-0000d510: 2020 2040 7465 7374 696e 672e 7265 7175     @testing.requ
-0000d520: 6972 6573 2e70 7269 6d61 7279 5f6b 6579  ires.primary_key
-0000d530: 5f63 6f6e 7374 7261 696e 745f 7265 666c  _constraint_refl
-0000d540: 6563 7469 6f6e 0a20 2020 2064 6566 2074  ection.    def t
-0000d550: 6573 745f 706b 5f63 6f6c 756d 6e5f 6f72  est_pk_column_or
-0000d560: 6465 7228 7365 6c66 2c20 636f 6e6e 6563  der(self, connec
-0000d570: 7469 6f6e 293a 0a20 2020 2020 2020 2022  tion):.        "
-0000d580: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
-0000d590: 4552 204f 5645 5252 4944 453a 0a20 2020  ER OVERRIDE:.   
-0000d5a0: 2020 2020 2045 6d75 6c74 6f72 2064 6f65       Emultor doe
-0000d5b0: 736e 2774 2073 7570 706f 7274 2072 6574  sn't support ret
-0000d5c0: 7572 6e69 6e67 2070 6b20 736f 7274 6564  urning pk sorted
-0000d5d0: 2062 7920 6f72 6469 6e61 6c20 7661 6c75   by ordinal valu
-0000d5e0: 650a 2020 2020 2020 2020 6f66 2063 6f6c  e.        of col
-0000d5f0: 756d 6e73 2e0a 2020 2020 2020 2020 2222  umns..        ""
-0000d600: 220a 2020 2020 2020 2020 696e 7370 203d  ".        insp =
-0000d610: 2069 6e73 7065 6374 2863 6f6e 6e65 6374   inspect(connect
-0000d620: 696f 6e29 0a20 2020 2020 2020 2070 7269  ion).        pri
-0000d630: 6d61 7279 5f6b 6579 203d 2069 6e73 702e  mary_key = insp.
-0000d640: 6765 745f 706b 5f63 6f6e 7374 7261 696e  get_pk_constrain
-0000d650: 7428 7365 6c66 2e74 6162 6c65 732e 7462  t(self.tables.tb
-0000d660: 312e 6e61 6d65 290a 2020 2020 2020 2020  1.name).        
-0000d670: 6578 7020 3d20 280a 2020 2020 2020 2020  exp = (.        
-0000d680: 2020 2020 5b22 6964 222c 2022 6e61 6d65      ["id", "name
-0000d690: 222c 2022 6174 7472 225d 0a20 2020 2020  ", "attr"].     
-0000d6a0: 2020 2020 2020 2069 6620 626f 6f6c 286f         if bool(o
-0000d6b0: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
-0000d6c0: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
-0000d6d0: 484f 5354 2229 290a 2020 2020 2020 2020  HOST")).        
-0000d6e0: 2020 2020 656c 7365 205b 226e 616d 6522      else ["name"
-0000d6f0: 2c20 2269 6422 2c20 2261 7474 7222 5d0a  , "id", "attr"].
-0000d700: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d710: 2020 6571 5f28 7072 696d 6172 795f 6b65    eq_(primary_ke
-0000d720: 792e 6765 7428 2263 6f6e 7374 7261 696e  y.get("constrain
-0000d730: 6564 5f63 6f6c 756d 6e73 2229 2c20 6578  ed_columns"), ex
-0000d740: 7029 0a0a 0a40 7079 7465 7374 2e6d 6172  p)...@pytest.mar
-0000d750: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-0000d760: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-0000d770: 7175 6f74 6573 2069 6e20 7461 626c 6520  quotes in table 
-0000d780: 6e61 6d65 732e 2229 0a63 6c61 7373 2051  names.").class Q
-0000d790: 756f 7465 644e 616d 6541 7267 756d 656e  uotedNameArgumen
-0000d7a0: 7454 6573 7428 5f51 756f 7465 644e 616d  tTest(_QuotedNam
-0000d7b0: 6541 7267 756d 656e 7454 6573 7429 3a0a  eArgumentTest):.
-0000d7c0: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
-0000d7d0: 205f 4461 7465 4669 7874 7572 6528 5f5f   _DateFixture(__
-0000d7e0: 4461 7465 4669 7874 7572 6529 3a0a 2020  DateFixture):.  
-0000d7f0: 2020 636f 6d70 6172 6520 3d20 4e6f 6e65    compare = None
-0000d800: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-0000d810: 6f64 0a20 2020 2064 6566 2064 6566 696e  od.    def defin
-0000d820: 655f 7461 626c 6573 2863 6c73 2c20 6d65  e_tables(cls, me
-0000d830: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
-0000d840: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-0000d850: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-0000d860: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
-0000d870: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-0000d880: 7070 6f72 7420 6175 746f 2069 6e63 7265  pport auto incre
-0000d890: 6d65 6e74 696e 6720 6964 7320 6665 6174  menting ids feat
-0000d8a0: 7572 652c 0a20 2020 2020 2020 2077 6869  ure,.        whi
-0000d8b0: 6368 2069 7320 7573 6564 2062 7920 7468  ch is used by th
-0000d8c0: 6520 6f72 6967 696e 616c 2074 6573 742e  e original test.
-0000d8d0: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
-0000d8e0: 7465 7374 2064 6174 610a 2020 2020 2020  test data.      
-0000d8f0: 2020 6372 6561 7469 6f6e 206d 6574 686f    creation metho
-0000d900: 6420 746f 2064 6973 6162 6c65 2061 7574  d to disable aut
-0000d910: 6f69 6e63 7265 6d65 6e74 2061 6e64 206d  oincrement and m
-0000d920: 616b 6520 6964 2063 6f6c 756d 6e0a 2020  ake id column.  
-0000d930: 2020 2020 2020 6e75 6c6c 6162 6c65 2e0a        nullable..
-0000d940: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000d950: 2020 2020 2063 6c61 7373 2044 6563 6f72       class Decor
-0000d960: 6174 6564 2873 716c 616c 6368 656d 792e  ated(sqlalchemy.
-0000d970: 5479 7065 4465 636f 7261 746f 7229 3a0a  TypeDecorator):.
-0000d980: 2020 2020 2020 2020 2020 2020 696d 706c              impl
-0000d990: 203d 2063 6c73 2e64 6174 6174 7970 650a   = cls.datatype.
-0000d9a0: 2020 2020 2020 2020 2020 2020 6361 6368              cach
-0000d9b0: 655f 6f6b 203d 2054 7275 650a 0a20 2020  e_ok = True..   
-0000d9c0: 2020 2020 2054 6162 6c65 280a 2020 2020       Table(.    
-0000d9d0: 2020 2020 2020 2020 2264 6174 655f 7461          "date_ta
-0000d9e0: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-0000d9f0: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
-0000da00: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-0000da10: 6964 222c 2049 6e74 6567 6572 2c20 7072  id", Integer, pr
-0000da20: 696d 6172 795f 6b65 793d 5472 7565 2c20  imary_key=True, 
-0000da30: 6e75 6c6c 6162 6c65 3d54 7275 6529 2c0a  nullable=True),.
-0000da40: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-0000da50: 6d6e 2822 6461 7465 5f64 6174 6122 2c20  mn("date_data", 
-0000da60: 636c 732e 6461 7461 7479 7065 292c 0a20  cls.datatype),. 
-0000da70: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-0000da80: 6e28 2264 6563 6f72 6174 6564 5f64 6174  n("decorated_dat
-0000da90: 655f 6461 7461 222c 2044 6563 6f72 6174  e_data", Decorat
-0000daa0: 6564 292c 0a20 2020 2020 2020 2029 0a0a  ed),.        )..
-0000dab0: 0a63 6c61 7373 2044 6174 6554 6573 7428  .class DateTest(
-0000dac0: 5f44 6174 6554 6573 7429 3a0a 2020 2020  _DateTest):.    
-0000dad0: 2222 220a 2020 2020 5350 414e 4e45 5220  """.    SPANNER 
-0000dae0: 4f56 4552 5249 4445 3a0a 0a20 2020 2044  OVERRIDE:..    D
-0000daf0: 6174 6554 6573 7420 7465 7374 7320 7573  ateTest tests us
-0000db00: 6564 2073 616d 6520 636c 6173 7320 6d65  ed same class me
-0000db10: 7468 6f64 2074 6f20 6372 6561 7465 2074  thod to create t
-0000db20: 6162 6c65 2c20 736f 2074 6f20 6176 6f69  able, so to avoi
-0000db30: 6420 7468 6f73 6520 6661 696c 7572 6573  d those failures
-0000db40: 0a20 2020 2061 6e64 206d 6169 6e74 6169  .    and maintai
-0000db50: 6e20 4452 5920 636f 6e63 6570 7420 6a75  n DRY concept ju
-0000db60: 7374 2069 6e68 6572 6974 2074 6865 2063  st inherit the c
-0000db70: 6c61 7373 2074 6f20 7275 6e20 7465 7374  lass to run test
-0000db80: 7320 7375 6363 6573 7366 756c 6c79 2e0a  s successfully..
-0000db90: 2020 2020 2222 220a 0a20 2020 2040 7079      """..    @py
-0000dba0: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
-0000dbb0: 280a 2020 2020 2020 2020 626f 6f6c 286f  (.        bool(o
-0000dbc0: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
-0000dbd0: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
-0000dbe0: 484f 5354 2229 292c 2072 6561 736f 6e3d  HOST")), reason=
-0000dbf0: 2253 6b69 7070 6564 206f 6e20 656d 756c  "Skipped on emul
-0000dc00: 6174 6f72 220a 2020 2020 290a 2020 2020  ator".    ).    
-0000dc10: 6465 6620 7465 7374 5f6e 756c 6c5f 626f  def test_null_bo
-0000dc20: 756e 645f 636f 6d70 6172 6973 6f6e 2873  und_comparison(s
-0000dc30: 656c 6629 3a0a 2020 2020 2020 2020 7375  elf):.        su
-0000dc40: 7065 7228 292e 7465 7374 5f6e 756c 6c5f  per().test_null_
-0000dc50: 626f 756e 645f 636f 6d70 6172 6973 6f6e  bound_comparison
-0000dc60: 2829 0a0a 2020 2020 4070 7974 6573 742e  ()..    @pytest.
-0000dc70: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
-0000dc80: 2020 2020 2062 6f6f 6c28 6f73 2e65 6e76       bool(os.env
-0000dc90: 6972 6f6e 2e67 6574 2822 5350 414e 4e45  iron.get("SPANNE
-0000dca0: 525f 454d 554c 4154 4f52 5f48 4f53 5422  R_EMULATOR_HOST"
-0000dcb0: 2929 2c20 7265 6173 6f6e 3d22 536b 6970  )), reason="Skip
-0000dcc0: 7065 6420 6f6e 2065 6d75 6c61 746f 7222  ped on emulator"
-0000dcd0: 0a20 2020 2029 0a20 2020 2064 6566 2074  .    ).    def t
-0000dce0: 6573 745f 6e75 6c6c 2873 656c 662c 2063  est_null(self, c
-0000dcf0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
-0000dd00: 2020 2020 7375 7065 7228 292e 7465 7374      super().test
-0000dd10: 5f6e 756c 6c28 636f 6e6e 6563 7469 6f6e  _null(connection
-0000dd20: 290a 0a0a 636c 6173 7320 4354 4554 6573  )...class CTETes
-0000dd30: 7428 5f43 5445 5465 7374 293a 0a20 2020  t(_CTETest):.   
-0000dd40: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-0000dd50: 2020 6465 6620 6465 6669 6e65 5f74 6162    def define_tab
-0000dd60: 6c65 7328 636c 732c 206d 6574 6164 6174  les(cls, metadat
-0000dd70: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
-0000dd80: 2020 2020 2020 2020 5468 6520 6f72 6967          The orig
-0000dd90: 696e 616c 206d 6574 686f 6420 6372 6561  inal method crea
-0000dda0: 7465 7320 6120 666f 7265 6967 6e20 6b65  tes a foreign ke
-0000ddb0: 7920 7769 7468 6f75 7420 6120 6e61 6d65  y without a name
-0000ddc0: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
-0000ddd0: 6361 7573 6573 2074 726f 7562 6c65 7320  causes troubles 
-0000dde0: 6f6e 2074 6573 7420 636c 6561 6e75 702e  on test cleanup.
-0000ddf0: 204f 7665 7272 6964 696e 6720 7468 650a   Overriding the.
-0000de00: 2020 2020 2020 2020 6d65 7468 6f64 2074          method t
-0000de10: 6f20 6578 706c 6963 6974 6c79 2073 6574  o explicitly set
-0000de20: 2061 2066 6f72 6569 676e 206b 6579 206e   a foreign key n
-0000de30: 616d 652e 0a20 2020 2020 2020 2022 2222  ame..        """
-0000de40: 0a20 2020 2020 2020 2054 6162 6c65 280a  .        Table(.
-0000de50: 2020 2020 2020 2020 2020 2020 2273 6f6d              "som
-0000de60: 655f 7461 626c 6522 2c0a 2020 2020 2020  e_table",.      
-0000de70: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-0000de80: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-0000de90: 6d6e 2822 6964 222c 2049 6e74 6567 6572  mn("id", Integer
-0000dea0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-0000deb0: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-0000dec0: 2043 6f6c 756d 6e28 2264 6174 6122 2c20   Column("data", 
-0000ded0: 5374 7269 6e67 2835 3029 292c 0a20 2020  String(50)),.   
-0000dee0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-0000def0: 2270 6172 656e 745f 6964 222c 2046 6f72  "parent_id", For
-0000df00: 6569 676e 4b65 7928 2273 6f6d 655f 7461  eignKey("some_ta
-0000df10: 626c 652e 6964 222c 206e 616d 653d 2266  ble.id", name="f
-0000df20: 6b5f 736f 6d65 5f74 6162 6c65 2229 292c  k_some_table")),
-0000df30: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000df40: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
-0000df50: 2020 2020 2020 2022 736f 6d65 5f6f 7468         "some_oth
-0000df60: 6572 5f74 6162 6c65 222c 0a20 2020 2020  er_table",.     
-0000df70: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
-0000df80: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-0000df90: 756d 6e28 2269 6422 2c20 496e 7465 6765  umn("id", Intege
-0000dfa0: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-0000dfb0: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000dfc0: 2020 436f 6c75 6d6e 2822 6461 7461 222c    Column("data",
-0000dfd0: 2053 7472 696e 6728 3530 2929 2c0a 2020   String(50)),.  
-0000dfe0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-0000dff0: 2822 7061 7265 6e74 5f69 6422 2c20 496e  ("parent_id", In
-0000e000: 7465 6765 7229 2c0a 2020 2020 2020 2020  teger),.        
-0000e010: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
-0000e020: 6172 6b2e 736b 6970 2822 494e 5345 5254  ark.skip("INSERT
-0000e030: 2066 726f 6d20 5749 5448 2073 7562 7175   from WITH subqu
-0000e040: 6572 7920 6973 206e 6f74 2073 7570 706f  ery is not suppo
-0000e050: 7274 6564 2229 0a20 2020 2064 6566 2074  rted").    def t
-0000e060: 6573 745f 696e 7365 7274 5f66 726f 6d5f  est_insert_from_
-0000e070: 7365 6c65 6374 5f72 6f75 6e64 5f74 7269  select_round_tri
-0000e080: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0000e090: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
-0000e0a0: 2074 6573 7420 6368 6563 6b73 2069 6620   test checks if 
-0000e0b0: 616e 2049 4e53 4552 5420 6361 6e20 6265  an INSERT can be
-0000e0c0: 2064 6f6e 6520 6672 6f6d 2061 2063 7465   done from a cte
-0000e0d0: 2c20 6c69 6b65 3a0a 0a20 2020 2020 2020  , like:..       
-0000e0e0: 2057 4954 4820 736f 6d65 5f63 7465 2041   WITH some_cte A
-0000e0f0: 5320 282e 2e2e 290a 2020 2020 2020 2020  S (...).        
-0000e100: 494e 5345 5254 2049 4e54 4f20 736f 6d65  INSERT INTO some
-0000e110: 5f6f 7468 6572 5f74 6162 6c65 2028 2e2e  _other_table (..
-0000e120: 2e20 5345 4c45 4354 202a 2046 524f 4d20  . SELECT * FROM 
-0000e130: 736f 6d65 5f63 7465 290a 0a20 2020 2020  some_cte)..     
-0000e140: 2020 2053 7563 6820 7175 6572 6965 7320     Such queries 
-0000e150: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
-0000e160: 6420 6279 2053 7061 6e6e 6572 2e0a 2020  d by Spanner..  
-0000e170: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e180: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
-0000e190: 6573 742e 6d61 726b 2e73 6b69 7028 2244  est.mark.skip("D
-0000e1a0: 454c 4554 4520 6672 6f6d 2057 4954 4820  ELETE from WITH 
-0000e1b0: 7375 6271 7565 7279 2069 7320 6e6f 7420  subquery is not 
-0000e1c0: 7375 7070 6f72 7465 6422 290a 2020 2020  supported").    
-0000e1d0: 6465 6620 7465 7374 5f64 656c 6574 655f  def test_delete_
-0000e1e0: 7363 616c 6172 5f73 7562 715f 726f 756e  scalar_subq_roun
-0000e1f0: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
-0000e200: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e210: 2020 5468 6520 7465 7374 2063 6865 636b    The test check
-0000e220: 7320 6966 2061 2044 454c 4554 4520 6361  s if a DELETE ca
-0000e230: 6e20 6265 2064 6f6e 6520 6672 6f6d 2061  n be done from a
-0000e240: 2063 7465 2c20 6c69 6b65 3a0a 0a20 2020   cte, like:..   
-0000e250: 2020 2020 2057 4954 4820 736f 6d65 5f63       WITH some_c
-0000e260: 7465 2041 5320 282e 2e2e 290a 2020 2020  te AS (...).    
-0000e270: 2020 2020 4445 4c45 5445 2046 524f 4d20      DELETE FROM 
-0000e280: 736f 6d65 5f6f 7468 6572 5f74 6162 6c65  some_other_table
-0000e290: 2028 2e2e 2e20 5345 4c45 4354 202a 2046   (... SELECT * F
-0000e2a0: 524f 4d20 736f 6d65 5f63 7465 290a 0a20  ROM some_cte).. 
-0000e2b0: 2020 2020 2020 2053 7563 6820 7175 6572         Such quer
-0000e2c0: 6965 7320 6172 6520 6e6f 7420 7375 7070  ies are not supp
-0000e2d0: 6f72 7465 6420 6279 2053 7061 6e6e 6572  orted by Spanner
-0000e2e0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000e2f0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0000e300: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-0000e310: 7028 2244 454c 4554 4520 6672 6f6d 2057  p("DELETE from W
-0000e320: 4954 4820 7375 6271 7565 7279 2069 7320  ITH subquery is 
-0000e330: 6e6f 7420 7375 7070 6f72 7465 6422 290a  not supported").
-0000e340: 2020 2020 6465 6620 7465 7374 5f64 656c      def test_del
-0000e350: 6574 655f 6672 6f6d 5f72 6f75 6e64 5f74  ete_from_round_t
-0000e360: 7269 7028 7365 6c66 293a 0a20 2020 2020  rip(self):.     
-0000e370: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-0000e380: 6865 2074 6573 7420 6368 6563 6b73 2069  he test checks i
-0000e390: 6620 6120 4445 4c45 5445 2063 616e 2062  f a DELETE can b
-0000e3a0: 6520 646f 6e65 2066 726f 6d20 6120 6374  e done from a ct
-0000e3b0: 652c 206c 696b 653a 0a0a 2020 2020 2020  e, like:..      
-0000e3c0: 2020 5749 5448 2073 6f6d 655f 6374 6520    WITH some_cte 
-0000e3d0: 4153 2028 2e2e 2e29 0a20 2020 2020 2020  AS (...).       
-0000e3e0: 2044 454c 4554 4520 4652 4f4d 2073 6f6d   DELETE FROM som
-0000e3f0: 655f 6f74 6865 725f 7461 626c 6520 282e  e_other_table (.
-0000e400: 2e2e 2053 454c 4543 5420 2a20 4652 4f4d  .. SELECT * FROM
-0000e410: 2073 6f6d 655f 6374 6529 0a0a 2020 2020   some_cte)..    
-0000e420: 2020 2020 5375 6368 2071 7565 7269 6573      Such queries
-0000e430: 2061 7265 206e 6f74 2073 7570 706f 7274   are not support
-0000e440: 6564 2062 7920 5370 616e 6e65 722e 0a20  ed by Spanner.. 
-0000e450: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e460: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-0000e470: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-0000e480: 5550 4441 5445 2066 726f 6d20 5749 5448  UPDATE from WITH
-0000e490: 2073 7562 7175 6572 7920 6973 206e 6f74   subquery is not
-0000e4a0: 2073 7570 706f 7274 6564 2229 0a20 2020   supported").   
-0000e4b0: 2064 6566 2074 6573 745f 7570 6461 7465   def test_update
-0000e4c0: 5f66 726f 6d5f 726f 756e 645f 7472 6970  _from_round_trip
-0000e4d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e4e0: 2222 220a 2020 2020 2020 2020 5468 6520  """.        The 
-0000e4f0: 7465 7374 2063 6865 636b 7320 6966 2061  test checks if a
-0000e500: 6e20 5550 4441 5445 2063 616e 2062 6520  n UPDATE can be 
-0000e510: 646f 6e65 2066 726f 6d20 6120 6374 652c  done from a cte,
-0000e520: 206c 696b 653a 0a0a 2020 2020 2020 2020   like:..        
-0000e530: 5749 5448 2073 6f6d 655f 6374 6520 4153  WITH some_cte AS
-0000e540: 2028 2e2e 2e29 0a20 2020 2020 2020 2055   (...).        U
-0000e550: 5044 4154 4520 736f 6d65 5f6f 7468 6572  PDATE some_other
-0000e560: 5f74 6162 6c65 0a20 2020 2020 2020 2053  _table.        S
-0000e570: 4554 2028 2e2e 2e20 5345 4c45 4354 202a  ET (... SELECT *
-0000e580: 2046 524f 4d20 736f 6d65 5f63 7465 290a   FROM some_cte).
-0000e590: 0a20 2020 2020 2020 2053 7563 6820 7175  .        Such qu
-0000e5a0: 6572 6965 7320 6172 6520 6e6f 7420 7375  eries are not su
-0000e5b0: 7070 6f72 7465 6420 6279 2053 7061 6e6e  pported by Spann
-0000e5c0: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
-0000e5d0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000e5e0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-0000e5f0: 6b69 7028 2257 4954 4820 5245 4355 5253  kip("WITH RECURS
-0000e600: 4956 4520 7375 6271 7565 7269 6573 2061  IVE subqueries a
-0000e610: 7265 206e 6f74 2073 7570 706f 7274 6564  re not supported
-0000e620: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-0000e630: 7365 6c65 6374 5f72 6563 7572 7369 7665  select_recursive
-0000e640: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
-0000e650: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000e660: 0a0a 636c 6173 7320 4461 7465 5469 6d65  ..class DateTime
-0000e670: 4d69 6372 6f73 6563 6f6e 6473 5465 7374  MicrosecondsTest
-0000e680: 285f 4461 7465 5469 6d65 4d69 6372 6f73  (_DateTimeMicros
-0000e690: 6563 6f6e 6473 5465 7374 2c20 4461 7465  econdsTest, Date
-0000e6a0: 5465 7374 293a 0a20 2020 2040 7079 7465  Test):.    @pyte
-0000e6b0: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-0000e6c0: 616e 6e65 7220 6461 7465 7320 6172 6520  anner dates are 
-0000e6d0: 7469 6d65 207a 6f6e 6520 696e 6465 7065  time zone indepe
-0000e6e0: 6e64 656e 7422 290a 2020 2020 6465 6620  ndent").    def 
-0000e6f0: 7465 7374 5f73 656c 6563 745f 6469 7265  test_select_dire
-0000e700: 6374 2873 656c 6629 3a0a 2020 2020 2020  ct(self):.      
-0000e710: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0000e720: 7465 7374 5f72 6f75 6e64 5f74 7269 7028  test_round_trip(
-0000e730: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000e740: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
-0000e750: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
-0000e760: 2020 2020 2020 5370 616e 6e65 7220 636f        Spanner co
-0000e770: 6e76 6572 7473 2074 696d 6573 7461 6d70  nverts timestamp
-0000e780: 2069 6e74 6f20 6025 592d 256d 2d25 6454   into `%Y-%m-%dT
-0000e790: 2548 3a25 4d3a 2553 2e25 665a 6020 666f  %H:%M:%S.%fZ` fo
-0000e7a0: 726d 6174 2c20 736f 2074 6f20 6176 6f69  rmat, so to avoi
-0000e7b0: 640a 2020 2020 2020 2020 6173 7365 7274  d.        assert
-0000e7c0: 2066 6169 6c75 7265 7320 636f 6e76 6572   failures conver
-0000e7d0: 7420 6461 7465 7469 6d65 2069 6e70 7574  t datetime input
-0000e7e0: 2074 6f20 7468 6520 6465 7369 7265 2074   to the desire t
-0000e7f0: 696d 6573 7461 6d70 2066 6f72 6d61 742e  imestamp format.
-0000e800: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000e810: 2020 2020 2064 6174 655f 7461 626c 6520       date_table 
-0000e820: 3d20 7365 6c66 2e74 6162 6c65 732e 6461  = self.tables.da
-0000e830: 7465 5f74 6162 6c65 0a0a 2020 2020 2020  te_table..      
-0000e840: 2020 7769 7468 2063 6f6e 6669 672e 6462    with config.db
-0000e850: 2e63 6f6e 6e65 6374 2829 2061 7320 636f  .connect() as co
-0000e860: 6e6e 6563 7469 6f6e 3a0a 2020 2020 2020  nnection:.      
-0000e870: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-0000e880: 2e65 7865 6375 7465 2864 6174 655f 7461  .execute(date_ta
-0000e890: 626c 652e 696e 7365 7274 2829 2c20 7b22  ble.insert(), {"
-0000e8a0: 6461 7465 5f64 6174 6122 3a20 7365 6c66  date_data": self
-0000e8b0: 2e64 6174 612c 2022 6964 223a 2032 3530  .data, "id": 250
-0000e8c0: 7d29 0a20 2020 2020 2020 2020 2020 2072  }).            r
-0000e8d0: 6f77 203d 2063 6f6e 6e65 6374 696f 6e2e  ow = connection.
-0000e8e0: 6578 6563 7574 6528 7365 6c65 6374 2864  execute(select(d
-0000e8f0: 6174 655f 7461 626c 652e 632e 6461 7465  ate_table.c.date
-0000e900: 5f64 6174 6129 292e 6669 7273 7428 290a  _data)).first().
-0000e910: 0a20 2020 2020 2020 2063 6f6d 7061 7265  .        compare
-0000e920: 203d 2073 656c 662e 636f 6d70 6172 6520   = self.compare 
-0000e930: 6f72 2073 656c 662e 6461 7461 0a20 2020  or self.data.   
-0000e940: 2020 2020 2063 6f6d 7061 7265 203d 2063       compare = c
-0000e950: 6f6d 7061 7265 2e73 7472 6674 696d 6528  ompare.strftime(
-0000e960: 2225 592d 256d 2d25 6454 2548 3a25 4d3a  "%Y-%m-%dT%H:%M:
-0000e970: 2553 2e25 665a 2229 0a20 2020 2020 2020  %S.%fZ").       
-0000e980: 2065 715f 2872 6f77 5b30 5d2e 7266 6333   eq_(row[0].rfc3
-0000e990: 3333 3928 292c 2063 6f6d 7061 7265 290a  339(), compare).
-0000e9a0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000e9b0: 7369 6e73 7461 6e63 6528 726f 775b 305d  sinstance(row[0]
-0000e9c0: 2c20 4461 7465 7469 6d65 5769 7468 4e61  , DatetimeWithNa
-0000e9d0: 6e6f 7365 636f 6e64 7329 0a0a 2020 2020  noseconds)..    
-0000e9e0: 6465 6620 7465 7374 5f72 6f75 6e64 5f74  def test_round_t
-0000e9f0: 7269 705f 6465 636f 7261 7465 6428 7365  rip_decorated(se
-0000ea00: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
-0000ea10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ea20: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-0000ea30: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
-0000ea40: 5370 616e 6e65 7220 636f 6e76 6572 7473  Spanner converts
-0000ea50: 2074 696d 6573 7461 6d70 2069 6e74 6f20   timestamp into 
-0000ea60: 6025 592d 256d 2d25 6454 2548 3a25 4d3a  `%Y-%m-%dT%H:%M:
-0000ea70: 2553 2e25 665a 6020 666f 726d 6174 2c20  %S.%fZ` format, 
-0000ea80: 736f 2074 6f20 6176 6f69 640a 2020 2020  so to avoid.    
-0000ea90: 2020 2020 6173 7365 7274 2066 6169 6c75      assert failu
-0000eaa0: 7265 7320 636f 6e76 6572 7420 6461 7465  res convert date
-0000eab0: 7469 6d65 2069 6e70 7574 2074 6f20 7468  time input to th
-0000eac0: 6520 6465 7369 7265 2074 696d 6573 7461  e desire timesta
-0000ead0: 6d70 2066 6f72 6d61 742e 0a20 2020 2020  mp format..     
-0000eae0: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-0000eaf0: 6174 655f 7461 626c 6520 3d20 7365 6c66  ate_table = self
-0000eb00: 2e74 6162 6c65 732e 6461 7465 5f74 6162  .tables.date_tab
-0000eb10: 6c65 0a0a 2020 2020 2020 2020 636f 6e6e  le..        conn
-0000eb20: 6563 7469 6f6e 2e65 7865 6375 7465 280a  ection.execute(.
-0000eb30: 2020 2020 2020 2020 2020 2020 6461 7465              date
-0000eb40: 5f74 6162 6c65 2e69 6e73 6572 7428 292c  _table.insert(),
-0000eb50: 207b 2269 6422 3a20 312c 2022 6465 636f   {"id": 1, "deco
-0000eb60: 7261 7465 645f 6461 7465 5f64 6174 6122  rated_date_data"
-0000eb70: 3a20 7365 6c66 2e64 6174 617d 0a20 2020  : self.data}.   
-0000eb80: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000eb90: 726f 7720 3d20 636f 6e6e 6563 7469 6f6e  row = connection
-0000eba0: 2e65 7865 6375 7465 2873 656c 6563 7428  .execute(select(
-0000ebb0: 6461 7465 5f74 6162 6c65 2e63 2e64 6563  date_table.c.dec
-0000ebc0: 6f72 6174 6564 5f64 6174 655f 6461 7461  orated_date_data
-0000ebd0: 2929 2e66 6972 7374 2829 0a0a 2020 2020  )).first()..    
-0000ebe0: 2020 2020 636f 6d70 6172 6520 3d20 7365      compare = se
-0000ebf0: 6c66 2e63 6f6d 7061 7265 206f 7220 7365  lf.compare or se
-0000ec00: 6c66 2e64 6174 610a 2020 2020 2020 2020  lf.data.        
-0000ec10: 636f 6d70 6172 6520 3d20 636f 6d70 6172  compare = compar
-0000ec20: 652e 7374 7266 7469 6d65 2822 2559 2d25  e.strftime("%Y-%
-0000ec30: 6d2d 2564 5425 483a 254d 3a25 532e 2566  m-%dT%H:%M:%S.%f
-0000ec40: 5a22 290a 2020 2020 2020 2020 6571 5f28  Z").        eq_(
-0000ec50: 726f 775b 305d 2e72 6663 3333 3339 2829  row[0].rfc3339()
-0000ec60: 2c20 636f 6d70 6172 6529 0a20 2020 2020  , compare).     
-0000ec70: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-0000ec80: 616e 6365 2872 6f77 5b30 5d2c 2044 6174  ance(row[0], Dat
-0000ec90: 6574 696d 6557 6974 684e 616e 6f73 6563  etimeWithNanosec
-0000eca0: 6f6e 6473 290a 0a20 2020 2040 7079 7465  onds)..    @pyte
-0000ecb0: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
-0000ecc0: 2020 2020 2020 2020 626f 6f6c 286f 732e          bool(os.
-0000ecd0: 656e 7669 726f 6e2e 6765 7428 2253 5041  environ.get("SPA
-0000ece0: 4e4e 4552 5f45 4d55 4c41 544f 525f 484f  NNER_EMULATOR_HO
-0000ecf0: 5354 2229 292c 2072 6561 736f 6e3d 2253  ST")), reason="S
-0000ed00: 6b69 7070 6564 206f 6e20 656d 756c 6174  kipped on emulat
-0000ed10: 6f72 220a 2020 2020 290a 2020 2020 6465  or".    ).    de
-0000ed20: 6620 7465 7374 5f6e 756c 6c5f 626f 756e  f test_null_boun
-0000ed30: 645f 636f 6d70 6172 6973 6f6e 2873 656c  d_comparison(sel
-0000ed40: 6629 3a0a 2020 2020 2020 2020 7375 7065  f):.        supe
-0000ed50: 7228 292e 7465 7374 5f6e 756c 6c5f 626f  r().test_null_bo
-0000ed60: 756e 645f 636f 6d70 6172 6973 6f6e 2829  und_comparison()
-0000ed70: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0000ed80: 726b 2e73 6b69 7069 6628 0a20 2020 2020  rk.skipif(.     
-0000ed90: 2020 2062 6f6f 6c28 6f73 2e65 6e76 6972     bool(os.envir
-0000eda0: 6f6e 2e67 6574 2822 5350 414e 4e45 525f  on.get("SPANNER_
-0000edb0: 454d 554c 4154 4f52 5f48 4f53 5422 2929  EMULATOR_HOST"))
-0000edc0: 2c20 7265 6173 6f6e 3d22 536b 6970 7065  , reason="Skippe
-0000edd0: 6420 6f6e 2065 6d75 6c61 746f 7222 0a20  d on emulator". 
-0000ede0: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
-0000edf0: 745f 6e75 6c6c 2873 656c 662c 2063 6f6e  t_null(self, con
-0000ee00: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-0000ee10: 2020 7375 7065 7228 292e 7465 7374 5f6e    super().test_n
-0000ee20: 756c 6c28 636f 6e6e 6563 7469 6f6e 290a  ull(connection).
-0000ee30: 0a0a 636c 6173 7320 4461 7465 5469 6d65  ..class DateTime
-0000ee40: 5465 7374 285f 4461 7465 5469 6d65 5465  Test(_DateTimeTe
-0000ee50: 7374 2c20 4461 7465 5469 6d65 4d69 6372  st, DateTimeMicr
-0000ee60: 6f73 6563 6f6e 6473 5465 7374 293a 0a20  osecondsTest):. 
-0000ee70: 2020 2022 2222 0a20 2020 2053 5041 4e4e     """.    SPANN
-0000ee80: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
-0000ee90: 2020 4461 7465 5469 6d65 5465 7374 2074    DateTimeTest t
-0000eea0: 6573 7473 2068 6176 6520 7468 6520 7361  ests have the sa
-0000eeb0: 6d65 2066 6169 6c75 7265 7320 7361 6d65  me failures same
-0000eec0: 2061 7320 4461 7465 5469 6d65 4d69 6372   as DateTimeMicr
-0000eed0: 6f73 6563 6f6e 6473 5465 7374 2074 6573  osecondsTest tes
-0000eee0: 7473 2c0a 2020 2020 736f 2074 6f20 6176  ts,.    so to av
-0000eef0: 6f69 6420 7468 6f73 6520 6661 696c 7572  oid those failur
-0000ef00: 6573 2061 6e64 206d 6169 6e74 6169 6e20  es and maintain 
-0000ef10: 4452 5920 636f 6e63 6570 7420 6a75 7374  DRY concept just
-0000ef20: 2069 6e68 6572 6974 2074 6865 2063 6c61   inherit the cla
-0000ef30: 7373 2074 6f20 7275 6e0a 2020 2020 7465  ss to run.    te
-0000ef40: 7374 7320 7375 6363 6573 7366 756c 6c79  sts successfully
-0000ef50: 2e0a 2020 2020 2222 220a 0a20 2020 2040  ..    """..    @
-0000ef60: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000ef70: 6966 280a 2020 2020 2020 2020 626f 6f6c  if(.        bool
-0000ef80: 286f 732e 656e 7669 726f 6e2e 6765 7428  (os.environ.get(
-0000ef90: 2253 5041 4e4e 4552 5f45 4d55 4c41 544f  "SPANNER_EMULATO
-0000efa0: 525f 484f 5354 2229 292c 2072 6561 736f  R_HOST")), reaso
-0000efb0: 6e3d 2253 6b69 7070 6564 206f 6e20 656d  n="Skipped on em
-0000efc0: 756c 6174 6f72 220a 2020 2020 290a 2020  ulator".    ).  
-0000efd0: 2020 6465 6620 7465 7374 5f6e 756c 6c5f    def test_null_
-0000efe0: 626f 756e 645f 636f 6d70 6172 6973 6f6e  bound_comparison
-0000eff0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f000: 7375 7065 7228 292e 7465 7374 5f6e 756c  super().test_nul
-0000f010: 6c5f 626f 756e 645f 636f 6d70 6172 6973  l_bound_comparis
-0000f020: 6f6e 2829 0a0a 2020 2020 4070 7974 6573  on()..    @pytes
-0000f030: 742e 6d61 726b 2e73 6b69 7069 6628 0a20  t.mark.skipif(. 
-0000f040: 2020 2020 2020 2062 6f6f 6c28 6f73 2e65         bool(os.e
-0000f050: 6e76 6972 6f6e 2e67 6574 2822 5350 414e  nviron.get("SPAN
-0000f060: 4e45 525f 454d 554c 4154 4f52 5f48 4f53  NER_EMULATOR_HOS
-0000f070: 5422 2929 2c20 7265 6173 6f6e 3d22 536b  T")), reason="Sk
-0000f080: 6970 7065 6420 6f6e 2065 6d75 6c61 746f  ipped on emulato
-0000f090: 7222 0a20 2020 2029 0a20 2020 2064 6566  r".    ).    def
-0000f0a0: 2074 6573 745f 6e75 6c6c 2873 656c 662c   test_null(self,
-0000f0b0: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
-0000f0c0: 2020 2020 2020 7375 7065 7228 292e 7465        super().te
-0000f0d0: 7374 5f6e 756c 6c28 636f 6e6e 6563 7469  st_null(connecti
-0000f0e0: 6f6e 290a 0a20 2020 2040 7079 7465 7374  on)..    @pytest
-0000f0f0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-0000f100: 6e65 7220 6461 7465 7320 6172 6520 7469  ner dates are ti
-0000f110: 6d65 207a 6f6e 6520 696e 6465 7065 6e64  me zone independ
-0000f120: 656e 7422 290a 2020 2020 6465 6620 7465  ent").    def te
-0000f130: 7374 5f73 656c 6563 745f 6469 7265 6374  st_select_direct
-0000f140: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f150: 7061 7373 0a0a 0a40 7079 7465 7374 2e6d  pass...@pytest.m
-0000f160: 6172 6b2e 736b 6970 2822 4e6f 7420 7375  ark.skip("Not su
-0000f170: 7070 6f72 7465 6420 6279 2053 7061 6e6e  pported by Spann
-0000f180: 6572 2229 0a63 6c61 7373 2044 6966 6669  er").class Diffi
-0000f190: 6375 6c74 5061 7261 6d65 7465 7273 5465  cultParametersTe
-0000f1a0: 7374 285f 4469 6666 6963 756c 7450 6172  st(_DifficultPar
-0000f1b0: 616d 6574 6572 7354 6573 7429 3a0a 2020  ametersTest):.  
-0000f1c0: 2020 7061 7373 0a0a 0a63 6c61 7373 2046    pass...class F
-0000f1d0: 6574 6368 4c69 6d69 744f 6666 7365 7454  etchLimitOffsetT
-0000f1e0: 6573 7428 5f46 6574 6368 4c69 6d69 744f  est(_FetchLimitO
-0000f1f0: 6666 7365 7454 6573 7429 3a0a 2020 2020  ffsetTest):.    
-0000f200: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-0000f210: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
-0000f220: 2774 2073 7570 706f 7274 2063 6f6d 706f  't support compo
-0000f230: 7369 7465 204c 494d 4954 2061 6e64 204f  site LIMIT and O
-0000f240: 4646 5345 5420 636c 6175 7365 7322 290a  FFSET clauses").
-0000f250: 2020 2020 6465 6620 7465 7374 5f65 7870      def test_exp
-0000f260: 725f 6c69 6d69 7428 7365 6c66 2c20 636f  r_limit(self, co
-0000f270: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
-0000f280: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-0000f290: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-0000f2a0: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-0000f2b0: 7375 7070 6f72 7420 636f 6d70 6f73 6974  support composit
-0000f2c0: 6520 4c49 4d49 5420 616e 6420 4f46 4653  e LIMIT and OFFS
-0000f2d0: 4554 2063 6c61 7573 6573 2229 0a20 2020  ET clauses").   
-0000f2e0: 2064 6566 2074 6573 745f 6578 7072 5f6f   def test_expr_o
-0000f2f0: 6666 7365 7428 7365 6c66 2c20 636f 6e6e  ffset(self, conn
-0000f300: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
-0000f310: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-0000f320: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-0000f330: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-0000f340: 7070 6f72 7420 636f 6d70 6f73 6974 6520  pport composite 
-0000f350: 4c49 4d49 5420 616e 6420 4f46 4653 4554  LIMIT and OFFSET
-0000f360: 2063 6c61 7573 6573 2229 0a20 2020 2064   clauses").    d
-0000f370: 6566 2074 6573 745f 6578 7072 5f6c 696d  ef test_expr_lim
-0000f380: 6974 5f6f 6666 7365 7428 7365 6c66 2c20  it_offset(self, 
-0000f390: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
-0000f3a0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-0000f3b0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000f3c0: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-0000f3d0: 7420 7375 7070 6f72 7420 636f 6d70 6f73  t support compos
-0000f3e0: 6974 6520 4c49 4d49 5420 616e 6420 4f46  ite LIMIT and OF
-0000f3f0: 4653 4554 2063 6c61 7573 6573 2229 0a20  FSET clauses"). 
-0000f400: 2020 2064 6566 2074 6573 745f 6578 7072     def test_expr
-0000f410: 5f6c 696d 6974 5f73 696d 706c 655f 6f66  _limit_simple_of
-0000f420: 6673 6574 2873 656c 662c 2063 6f6e 6e65  fset(self, conne
-0000f430: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-0000f440: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-0000f450: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
-0000f460: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-0000f470: 706f 7274 2063 6f6d 706f 7369 7465 204c  port composite L
-0000f480: 494d 4954 2061 6e64 204f 4646 5345 5420  IMIT and OFFSET 
-0000f490: 636c 6175 7365 7322 290a 2020 2020 6465  clauses").    de
-0000f4a0: 6620 7465 7374 5f73 696d 706c 655f 6c69  f test_simple_li
-0000f4b0: 6d69 745f 6578 7072 5f6f 6666 7365 7428  mit_expr_offset(
-0000f4c0: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
-0000f4d0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000f4e0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0000f4f0: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-0000f500: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-0000f510: 636f 6d70 6f73 6974 6520 4c49 4d49 5420  composite LIMIT 
-0000f520: 616e 6420 4f46 4653 4554 2063 6c61 7573  and OFFSET claus
-0000f530: 6573 2229 0a20 2020 2064 6566 2074 6573  es").    def tes
-0000f540: 745f 626f 756e 645f 6f66 6673 6574 2873  t_bound_offset(s
-0000f550: 656c 662c 2063 6f6e 6e65 6374 696f 6e29  elf, connection)
-0000f560: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0000f570: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000f580: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
-0000f590: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
-0000f5a0: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
-0000f5b0: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
-0000f5c0: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
-0000f5d0: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
-0000f5e0: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
-0000f5f0: 6c69 6d69 745f 7265 6e64 6572 5f6d 756c  limit_render_mul
-0000f600: 7469 706c 655f 7469 6d65 7328 7365 6c66  tiple_times(self
-0000f610: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
-0000f620: 2020 2020 2020 2074 6162 6c65 203d 2073         table = s
-0000f630: 656c 662e 7461 626c 6573 2e73 6f6d 655f  elf.tables.some_
-0000f640: 7461 626c 650a 2020 2020 2020 2020 7374  table.        st
-0000f650: 6d74 203d 2073 656c 6563 7428 7461 626c  mt = select(tabl
-0000f660: 652e 632e 6964 292e 6c69 6d69 7428 3129  e.c.id).limit(1)
-0000f670: 2e73 6361 6c61 725f 7375 6271 7565 7279  .scalar_subquery
-0000f680: 2829 0a0a 2020 2020 2020 2020 7520 3d20  ()..        u = 
-0000f690: 756e 696f 6e28 7365 6c65 6374 2873 746d  union(select(stm
-0000f6a0: 7429 2c20 7365 6c65 6374 2873 746d 7429  t), select(stmt)
-0000f6b0: 292e 7375 6271 7565 7279 2829 2e73 656c  ).subquery().sel
-0000f6c0: 6563 7428 290a 0a20 2020 2020 2020 2073  ect()..        s
-0000f6d0: 656c 662e 5f61 7373 6572 745f 7265 7375  elf._assert_resu
-0000f6e0: 6c74 280a 2020 2020 2020 2020 2020 2020  lt(.            
-0000f6f0: 636f 6e6e 6563 7469 6f6e 2c0a 2020 2020  connection,.    
-0000f700: 2020 2020 2020 2020 752c 0a20 2020 2020          u,.     
-0000f710: 2020 2020 2020 205b 2831 2c29 5d2c 0a20         [(1,)],. 
-0000f720: 2020 2020 2020 2029 0a0a 2020 2020 4074         )..    @t
-0000f730: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-0000f740: 6f66 6673 6574 0a20 2020 2064 6566 2074  offset.    def t
-0000f750: 6573 745f 7369 6d70 6c65 5f6f 6666 7365  est_simple_offse
-0000f760: 7428 7365 6c66 2c20 636f 6e6e 6563 7469  t(self, connecti
-0000f770: 6f6e 293a 0a20 2020 2020 2020 2074 6162  on):.        tab
-0000f780: 6c65 203d 2073 656c 662e 7461 626c 6573  le = self.tables
-0000f790: 2e73 6f6d 655f 7461 626c 650a 2020 2020  .some_table.    
-0000f7a0: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
-0000f7b0: 5f72 6573 756c 7428 0a20 2020 2020 2020  _result(.       
-0000f7c0: 2020 2020 2063 6f6e 6e65 6374 696f 6e2c       connection,
-0000f7d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f7e0: 6563 7428 7461 626c 6529 2e6f 7264 6572  ect(table).order
-0000f7f0: 5f62 7928 7461 626c 652e 632e 6964 292e  _by(table.c.id).
-0000f800: 6f66 6673 6574 2832 292c 0a20 2020 2020  offset(2),.     
-0000f810: 2020 2020 2020 205b 2833 2c20 332c 2034         [(3, 3, 4
-0000f820: 292c 2028 342c 2034 2c20 3529 2c20 2835  ), (4, 4, 5), (5
-0000f830: 2c20 342c 2036 295d 2c0a 2020 2020 2020  , 4, 6)],.      
-0000f840: 2020 290a 0a0a 4070 7974 6573 742e 6d61    )...@pytest.ma
-0000f850: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-0000f860: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-0000f870: 2061 7574 6f69 6e63 7265 6d65 6e74 2229   autoincrement")
-0000f880: 0a63 6c61 7373 2049 6465 6e74 6974 7941  .class IdentityA
-0000f890: 7574 6f69 6e63 7265 6d65 6e74 5465 7374  utoincrementTest
-0000f8a0: 285f 4964 656e 7469 7479 4175 746f 696e  (_IdentityAutoin
-0000f8b0: 6372 656d 656e 7454 6573 7429 3a0a 2020  crementTest):.  
-0000f8c0: 2020 7061 7373 0a0a 0a40 7079 7465 7374    pass...@pytest
-0000f8d0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-0000f8e0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-0000f8f0: 6f72 7420 7265 7475 726e 696e 6722 290a  ort returning").
-0000f900: 636c 6173 7320 5265 7475 726e 696e 6747  class ReturningG
-0000f910: 7561 7264 7354 6573 7428 5f52 6574 7572  uardsTest(_Retur
-0000f920: 6e69 6e67 4775 6172 6473 5465 7374 293a  ningGuardsTest):
-0000f930: 0a20 2020 2070 6173 730a 0a0a 4070 7974  .    pass...@pyt
-0000f940: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
-0000f950: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
-0000f960: 7570 706f 7274 2075 7365 7220 6d61 6465  upport user made
-0000f970: 2073 6368 656d 6173 2229 0a63 6c61 7373   schemas").class
-0000f980: 2053 616d 654e 616d 6564 5363 6865 6d61   SameNamedSchema
-0000f990: 5461 626c 6554 6573 7428 5f53 616d 654e  TableTest(_SameN
-0000f9a0: 616d 6564 5363 6865 6d61 5461 626c 6554  amedSchemaTableT
-0000f9b0: 6573 7429 3a0a 2020 2020 7061 7373 0a0a  est):.    pass..
-0000f9c0: 0a63 6c61 7373 2045 7363 6170 696e 6754  .class EscapingT
-0000f9d0: 6573 7428 5f45 7363 6170 696e 6754 6573  est(_EscapingTes
-0000f9e0: 7429 3a0a 2020 2020 4070 726f 7669 6465  t):.    @provide
-0000f9f0: 5f6d 6574 6164 6174 610a 2020 2020 6465  _metadata.    de
-0000fa00: 6620 7465 7374 5f70 6572 6365 6e74 5f73  f test_percent_s
-0000fa10: 6967 6e5f 726f 756e 645f 7472 6970 2873  ign_round_trip(s
-0000fa20: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000fa30: 2254 6573 7420 7468 6174 2074 6865 2044  "Test that the D
-0000fa40: 4241 5049 2061 6363 6f6d 6d6f 6461 7465  BAPI accommodate
-0000fa50: 7320 666f 7220 6573 6361 7065 6420 2f20  s for escaped / 
-0000fa60: 6e6f 6e65 7363 6170 6564 0a20 2020 2020  nonescaped.     
-0000fa70: 2020 2070 6572 6365 6e74 2073 6967 6e73     percent signs
-0000fa80: 2069 6e20 6120 7761 7920 7468 6174 206d   in a way that m
-0000fa90: 6174 6368 6573 2074 6865 2063 6f6d 7069  atches the compi
-0000faa0: 6c65 720a 0a20 2020 2020 2020 2053 5041  ler..        SPA
-0000fab0: 4e4e 4552 204f 5645 5252 4944 450a 2020  NNER OVERRIDE.  
-0000fac0: 2020 2020 2020 436c 6f75 6420 5370 616e        Cloud Span
-0000fad0: 6e65 7220 7375 7070 6f72 7473 2074 6162  ner supports tab
-0000fae0: 6c65 7320 7769 7468 2065 6d70 7479 2070  les with empty p
-0000faf0: 7269 6d61 7279 206b 6579 2c20 6275 740a  rimary key, but.
-0000fb00: 2020 2020 2020 2020 6f6e 6c79 2073 696e          only sin
-0000fb10: 676c 6520 6f6e 6520 726f 7720 6361 6e20  gle one row can 
-0000fb20: 6265 2069 6e73 6572 7465 6420 696e 746f  be inserted into
-0000fb30: 2073 7563 6820 6120 7461 626c 6520 2d0a   such a table -.
-0000fb40: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
-0000fb50: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
-0000fb60: 6c20 6661 696c 2077 6974 6820 6052 6f77  l fail with `Row
-0000fb70: 205b 5d20 616c 7265 6164 7920 6578 6973   [] already exis
-0000fb80: 7473 222e 0a20 2020 2020 2020 204f 7665  ts"..        Ove
-0000fb90: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
-0000fba0: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
-0000fbb0: 6d65 2066 6169 6c75 7265 2e0a 2020 2020  me failure..    
-0000fbc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000fbd0: 6d20 3d20 7365 6c66 2e6d 6574 6164 6174  m = self.metadat
-0000fbe0: 610a 2020 2020 2020 2020 7420 3d20 5461  a.        t = Ta
-0000fbf0: 626c 6528 2274 222c 206d 2c20 436f 6c75  ble("t", m, Colu
-0000fc00: 6d6e 2822 6461 7461 222c 2053 7472 696e  mn("data", Strin
-0000fc10: 6728 3530 2929 290a 2020 2020 2020 2020  g(50))).        
-0000fc20: 742e 6372 6561 7465 2863 6f6e 6669 672e  t.create(config.
-0000fc30: 6462 290a 2020 2020 2020 2020 7769 7468  db).        with
-0000fc40: 2063 6f6e 6669 672e 6462 2e62 6567 696e   config.db.begin
-0000fc50: 2829 2061 7320 636f 6e6e 3a0a 2020 2020  () as conn:.    
-0000fc60: 2020 2020 2020 2020 636f 6e6e 2e65 7865          conn.exe
-0000fc70: 6375 7465 2874 2e69 6e73 6572 7428 292c  cute(t.insert(),
-0000fc80: 2064 6963 7428 6461 7461 3d22 736f 6d65   dict(data="some
-0000fc90: 2025 2076 616c 7565 2229 290a 0a20 2020   % value"))..   
-0000fca0: 2020 2020 2020 2020 2065 715f 280a 2020           eq_(.  
-0000fcb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000fcc0: 6e6e 2e73 6361 6c61 7228 0a20 2020 2020  nn.scalar(.     
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fce0: 656c 6563 7428 742e 632e 6461 7461 292e  elect(t.c.data).
-0000fcf0: 7768 6572 6528 742e 632e 6461 7461 203d  where(t.c.data =
-0000fd00: 3d20 6c69 7465 7261 6c5f 636f 6c75 6d6e  = literal_column
-0000fd10: 2822 2773 6f6d 6520 2520 7661 6c75 6527  ("'some % value'
-0000fd20: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-0000fd30: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-0000fd40: 2020 2020 2020 2022 736f 6d65 2025 2076         "some % v
-0000fd50: 616c 7565 222c 0a20 2020 2020 2020 2020  alue",.         
-0000fd60: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0000fd70: 2020 636f 6e6e 2e65 7865 6375 7465 2874    conn.execute(t
-0000fd80: 2e64 656c 6574 6528 2929 0a20 2020 2020  .delete()).     
-0000fd90: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
-0000fda0: 7574 6528 742e 696e 7365 7274 2829 2c20  ute(t.insert(), 
-0000fdb0: 6469 6374 2864 6174 613d 2273 6f6d 6520  dict(data="some 
-0000fdc0: 2525 206f 7468 6572 2076 616c 7565 2229  %% other value")
-0000fdd0: 290a 2020 2020 2020 2020 2020 2020 6571  ).            eq
-0000fde0: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
-0000fdf0: 2020 2063 6f6e 6e2e 7363 616c 6172 280a     conn.scalar(.
-0000fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe10: 2020 2020 7365 6c65 6374 2874 2e63 2e64      select(t.c.d
-0000fe20: 6174 6129 2e77 6865 7265 280a 2020 2020  ata).where(.    
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe40: 2020 2020 742e 632e 6461 7461 203d 3d20      t.c.data == 
-0000fe50: 6c69 7465 7261 6c5f 636f 6c75 6d6e 2822  literal_column("
-0000fe60: 2773 6f6d 6520 2525 206f 7468 6572 2076  'some %% other v
-0000fe70: 616c 7565 2722 290a 2020 2020 2020 2020  alue'").        
-0000fe80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-0000fea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000feb0: 2022 736f 6d65 2025 2520 6f74 6865 7220   "some %% other 
-0000fec0: 7661 6c75 6522 2c0a 2020 2020 2020 2020  value",.        
-0000fed0: 2020 2020 290a 0a0a 636c 6173 7320 4578      )...class Ex
-0000fee0: 6973 7473 5465 7374 285f 4578 6973 7473  istsTest(_Exists
-0000fef0: 5465 7374 293a 0a20 2020 2064 6566 2074  Test):.    def t
-0000ff00: 6573 745f 7365 6c65 6374 5f65 7869 7374  est_select_exist
-0000ff10: 7328 7365 6c66 2c20 636f 6e6e 6563 7469  s(self, connecti
-0000ff20: 6f6e 293a 0a20 2020 2020 2020 2022 2222  on):.        """
-0000ff30: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-0000ff40: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
-0000ff50: 2020 2020 5468 6520 6f72 6967 696e 616c      The original
-0000ff60: 2074 6573 7420 6973 2074 7279 696e 6720   test is trying 
-0000ff70: 746f 2065 7865 6375 7465 2061 2071 7565  to execute a que
-0000ff80: 7279 206c 696b 653a 0a0a 2020 2020 2020  ry like:..      
-0000ff90: 2020 5345 4c45 4354 202e 2e2e 0a20 2020    SELECT ....   
-0000ffa0: 2020 2020 2057 4845 5245 2045 5849 5354       WHERE EXIST
-0000ffb0: 5320 2853 454c 4543 5420 2e2e 2e29 0a0a  S (SELECT ...)..
-0000ffc0: 2020 2020 2020 2020 5345 4c45 4354 2057          SELECT W
-0000ffd0: 4845 5245 2077 6974 686f 7574 2046 524f  HERE without FRO
-0000ffe0: 4d20 636c 6175 7365 2069 7320 6e6f 7420  M clause is not 
-0000fff0: 7375 7070 6f72 7465 6420 6279 2053 7061  supported by Spa
-00010000: 6e6e 6572 2e0a 2020 2020 2020 2020 5265  nner..        Re
-00010010: 7772 6974 696e 6720 7468 6520 7465 7374  writing the test
-00010020: 2074 6f20 666f 7263 6520 6974 2074 6f20   to force it to 
-00010030: 6765 6e65 7261 7465 2061 2071 7565 7279  generate a query
-00010040: 206c 696b 653a 0a0a 2020 2020 2020 2020   like:..        
-00010050: 5345 4c45 4354 2045 5849 5354 5320 2853  SELECT EXISTS (S
-00010060: 454c 4543 5420 2e2e 2e29 0a20 2020 2020  ELECT ...).     
-00010070: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00010080: 7475 6666 203d 2073 656c 662e 7461 626c  tuff = self.tabl
-00010090: 6573 2e73 7475 6666 0a20 2020 2020 2020  es.stuff.       
-000100a0: 2065 715f 280a 2020 2020 2020 2020 2020   eq_(.          
-000100b0: 2020 636f 6e6e 6563 7469 6f6e 2e65 7865    connection.exe
-000100c0: 6375 7465 280a 2020 2020 2020 2020 2020  cute(.          
-000100d0: 2020 2020 2020 7365 6c65 6374 2865 7869        select(exi
-000100e0: 7374 7328 292e 7768 6572 6528 7374 7566  sts().where(stuf
-000100f0: 662e 632e 6461 7461 203d 3d20 2273 6f6d  f.c.data == "som
-00010100: 6520 6461 7461 2229 290a 2020 2020 2020  e data")).      
-00010110: 2020 2020 2020 292e 6665 7463 6861 6c6c        ).fetchall
-00010120: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00010130: 5b28 5472 7565 2c29 5d2c 0a20 2020 2020  [(True,)],.     
-00010140: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-00010150: 7374 5f73 656c 6563 745f 6578 6973 7473  st_select_exists
-00010160: 5f66 616c 7365 2873 656c 662c 2063 6f6e  _false(self, con
-00010170: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-00010180: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-00010190: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-000101a0: 0a20 2020 2020 2020 2054 6865 206f 7269  .        The ori
-000101b0: 6769 6e61 6c20 7465 7374 2069 7320 7472  ginal test is tr
-000101c0: 7969 6e67 2074 6f20 6578 6563 7574 6520  ying to execute 
-000101d0: 6120 7175 6572 7920 6c69 6b65 3a0a 0a20  a query like:.. 
-000101e0: 2020 2020 2020 2053 454c 4543 5420 2e2e         SELECT ..
-000101f0: 2e0a 2020 2020 2020 2020 5748 4552 4520  ..        WHERE 
-00010200: 4558 4953 5453 2028 5345 4c45 4354 202e  EXISTS (SELECT .
-00010210: 2e2e 290a 0a20 2020 2020 2020 2053 454c  ..)..        SEL
-00010220: 4543 5420 5748 4552 4520 7769 7468 6f75  ECT WHERE withou
-00010230: 7420 4652 4f4d 2063 6c61 7573 6520 6973  t FROM clause is
-00010240: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
-00010250: 7920 5370 616e 6e65 722e 0a20 2020 2020  y Spanner..     
-00010260: 2020 2052 6577 7269 7469 6e67 2074 6865     Rewriting the
-00010270: 2074 6573 7420 746f 2066 6f72 6365 2069   test to force i
-00010280: 7420 746f 2067 656e 6572 6174 6520 6120  t to generate a 
-00010290: 7175 6572 7920 6c69 6b65 3a0a 0a20 2020  query like:..   
-000102a0: 2020 2020 2053 454c 4543 5420 4558 4953       SELECT EXIS
-000102b0: 5453 2028 5345 4c45 4354 202e 2e2e 290a  TS (SELECT ...).
-000102c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000102d0: 2020 2020 7374 7566 6620 3d20 7365 6c66      stuff = self
-000102e0: 2e74 6162 6c65 732e 7374 7566 660a 2020  .tables.stuff.  
-000102f0: 2020 2020 2020 6571 5f28 0a20 2020 2020        eq_(.     
-00010300: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-00010310: 6e2e 6578 6563 7574 6528 0a20 2020 2020  n.execute(.     
-00010320: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00010330: 7428 6578 6973 7473 2829 2e77 6865 7265  t(exists().where
-00010340: 2873 7475 6666 2e63 2e64 6174 6120 3d3d  (stuff.c.data ==
-00010350: 2022 6e6f 2064 6174 6122 2929 0a20 2020   "no data")).   
-00010360: 2020 2020 2020 2020 2029 2e66 6574 6368           ).fetch
-00010370: 616c 6c28 292c 0a20 2020 2020 2020 2020  all(),.         
-00010380: 2020 205b 2846 616c 7365 2c29 5d2c 0a20     [(False,)],. 
-00010390: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
-000103a0: 2054 6162 6c65 4444 4c54 6573 7428 5f54   TableDDLTest(_T
-000103b0: 6162 6c65 4444 4c54 6573 7429 3a0a 2020  ableDDLTest):.  
-000103c0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-000103d0: 6b69 7028 0a20 2020 2020 2020 2022 5370  kip(.        "Sp
-000103e0: 616e 6e65 7220 7461 626c 6520 6e61 6d65  anner table name
-000103f0: 206d 7573 7420 7374 6172 7420 7769 7468   must start with
-00010400: 2061 6e20 7570 7065 7263 6173 6520 6f72   an uppercase or
-00010410: 206c 6f77 6572 6361 7365 206c 6574 7465   lowercase lette
-00010420: 7222 0a20 2020 2029 0a20 2020 2064 6566  r".    ).    def
-00010430: 2074 6573 745f 756e 6465 7273 636f 7265   test_underscore
-00010440: 5f6e 616d 6573 2873 656c 6629 3a0a 2020  _names(self):.  
-00010450: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00010460: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00010470: 7028 2254 6162 6c65 206e 616d 6573 2069  p("Table names i
-00010480: 6e63 7564 696e 6720 7363 6865 6d61 7320  ncuding schemas 
-00010490: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
-000104a0: 6420 6279 2053 7061 6e6e 6572 2229 0a20  d by Spanner"). 
-000104b0: 2020 2064 6566 2074 6573 745f 6372 6561     def test_crea
-000104c0: 7465 5f74 6162 6c65 5f73 6368 656d 6128  te_table_schema(
-000104d0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000104e0: 6173 730a 0a0a 636c 6173 7320 4675 7475  ass...class Futu
-000104f0: 7265 5461 626c 6544 444c 5465 7374 285f  reTableDDLTest(_
-00010500: 4675 7475 7265 5461 626c 6544 444c 5465  FutureTableDDLTe
-00010510: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
-00010520: 2e6d 6172 6b2e 736b 6970 2822 5461 626c  .mark.skip("Tabl
-00010530: 6520 6e61 6d65 7320 696e 6375 6469 6e67  e names incuding
-00010540: 2073 6368 656d 6173 2061 7265 206e 6f74   schemas are not
-00010550: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
-00010560: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
-00010570: 7465 7374 5f63 7265 6174 655f 7461 626c  test_create_tabl
-00010580: 655f 7363 6865 6d61 2873 656c 6629 3a0a  e_schema(self):.
-00010590: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000105a0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-000105b0: 6b69 7028 0a20 2020 2020 2020 2022 5370  kip(.        "Sp
-000105c0: 616e 6e65 7220 7461 626c 6520 6e61 6d65  anner table name
-000105d0: 206d 7573 7420 7374 6172 7420 7769 7468   must start with
-000105e0: 2061 6e20 7570 7065 7263 6173 6520 6f72   an uppercase or
-000105f0: 206c 6f77 6572 6361 7365 206c 6574 7465   lowercase lette
-00010600: 7222 0a20 2020 2029 0a20 2020 2064 6566  r".    ).    def
-00010610: 2074 6573 745f 756e 6465 7273 636f 7265   test_underscore
-00010620: 5f6e 616d 6573 2873 656c 6629 3a0a 2020  _names(self):.  
-00010630: 2020 2020 2020 7061 7373 0a0a 0a40 7079        pass...@py
-00010640: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00010650: 4d61 7820 6964 656e 7469 6669 6572 206c  Max identifier l
-00010660: 656e 6774 6820 696e 2053 7061 6e6e 6572  ength in Spanner
-00010670: 2069 7320 3132 3822 290a 636c 6173 7320   is 128").class 
-00010680: 4c6f 6e67 4e61 6d65 426c 6f77 6f75 7454  LongNameBlowoutT
-00010690: 6573 7428 5f4c 6f6e 674e 616d 6542 6c6f  est(_LongNameBlo
-000106a0: 776f 7574 5465 7374 293a 0a20 2020 2070  woutTest):.    p
-000106b0: 6173 730a 0a0a 4070 7974 6573 742e 6d61  ass...@pytest.ma
-000106c0: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-000106d0: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-000106e0: 2054 696d 6520 6461 7461 2074 7970 652e   Time data type.
-000106f0: 2229 0a63 6c61 7373 2054 696d 6554 6573  ").class TimeTes
-00010700: 7473 285f 5469 6d65 4d69 6372 6f73 6563  ts(_TimeMicrosec
-00010710: 6f6e 6473 5465 7374 2c20 5f54 696d 6554  ondsTest, _TimeT
-00010720: 6573 7429 3a0a 2020 2020 7061 7373 0a0a  est):.    pass..
-00010730: 0a40 7079 7465 7374 2e6d 6172 6b2e 736b  .@pytest.mark.sk
-00010740: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
-00010750: 6e27 7420 636f 6572 6365 2064 6174 6573  n't coerce dates
-00010760: 2066 726f 6d20 6461 7465 7469 6d65 2e22   from datetime."
-00010770: 290a 636c 6173 7320 4461 7465 5469 6d65  ).class DateTime
-00010780: 436f 6572 6365 6454 6f44 6174 6554 696d  CoercedToDateTim
-00010790: 6554 6573 7428 5f44 6174 6554 696d 6543  eTest(_DateTimeC
-000107a0: 6f65 7263 6564 546f 4461 7465 5469 6d65  oercedToDateTime
-000107b0: 5465 7374 293a 0a20 2020 2070 6173 730a  Test):.    pass.
-000107c0: 0a0a 636c 6173 7320 496e 7465 6765 7254  ..class IntegerT
-000107d0: 6573 7428 5f49 6e74 6567 6572 5465 7374  est(_IntegerTest
-000107e0: 293a 0a20 2020 2040 7072 6f76 6964 655f  ):.    @provide_
-000107f0: 6d65 7461 6461 7461 0a20 2020 2064 6566  metadata.    def
-00010800: 205f 726f 756e 645f 7472 6970 2873 656c   _round_trip(sel
-00010810: 662c 2064 6174 6174 7970 652c 2064 6174  f, datatype, dat
-00010820: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
-00010830: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
-00010840: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-00010850: 2020 2054 6869 7320 6973 2074 6865 2068     This is the h
-00010860: 656c 7065 7220 6d65 7468 6f64 2066 6f72  elper method for
-00010870: 2069 6e74 6567 6572 2063 6c61 7373 2074   integer class t
-00010880: 6573 7473 2077 6869 6368 2063 7265 6174  ests which creat
-00010890: 6573 2061 2074 6162 6c65 2061 6e64 0a20  es a table and. 
-000108a0: 2020 2020 2020 2070 6572 666f 726d 7320         performs 
-000108b0: 616e 2069 6e73 6572 7420 6f70 6572 6174  an insert operat
-000108c0: 696f 6e2e 0a20 2020 2020 2020 2043 6c6f  ion..        Clo
-000108d0: 7564 2053 7061 6e6e 6572 2073 7570 706f  ud Spanner suppo
-000108e0: 7274 7320 7461 626c 6573 2077 6974 6820  rts tables with 
-000108f0: 616e 2065 6d70 7479 2070 7269 6d61 7279  an empty primary
-00010900: 206b 6579 2c20 6275 7420 6f6e 6c79 206f   key, but only o
-00010910: 6e65 0a20 2020 2020 2020 2072 6f77 2063  ne.        row c
-00010920: 616e 2062 6520 696e 7365 7274 6564 2069  an be inserted i
-00010930: 6e74 6f20 7375 6368 2061 2074 6162 6c65  nto such a table
-00010940: 202d 2066 6f6c 6c6f 7769 6e67 2069 6e73   - following ins
-00010950: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
-00010960: 6c20 7769 7468 0a20 2020 2020 2020 2060  l with.        `
-00010970: 3430 3020 6964 206d 7573 7420 6e6f 7420  400 id must not 
-00010980: 6265 204e 554c 4c20 696e 2074 6162 6c65  be NULL in table
-00010990: 2064 6174 655f 7461 626c 6560 2e0a 2020   date_table`..  
-000109a0: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
-000109b0: 2074 6865 2074 6573 7473 2061 6e64 2061   the tests and a
-000109c0: 6464 696e 6720 6120 6d61 6e75 616c 2070  dding a manual p
-000109d0: 7269 6d61 7279 206b 6579 2076 616c 7565  rimary key value
-000109e0: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
-000109f0: 6d65 0a20 2020 2020 2020 2066 6169 6c75  me.        failu
-00010a00: 7265 732e 0a20 2020 2020 2020 2022 2222  res..        """
-00010a10: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00010a20: 6120 3d20 7365 6c66 2e6d 6574 6164 6174  a = self.metadat
-00010a30: 610a 2020 2020 2020 2020 696e 745f 7461  a.        int_ta
-00010a40: 626c 6520 3d20 5461 626c 6528 0a20 2020  ble = Table(.   
-00010a50: 2020 2020 2020 2020 2022 696e 7465 6765           "intege
-00010a60: 725f 7461 626c 6522 2c0a 2020 2020 2020  r_table",.      
-00010a70: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-00010a80: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00010a90: 6d6e 2822 6964 222c 2049 6e74 6567 6572  mn("id", Integer
-00010aa0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-00010ab0: 7565 2c20 7465 7374 5f6e 6565 6473 5f61  ue, test_needs_a
-00010ac0: 7574 6f69 6e63 7265 6d65 6e74 3d54 7275  utoincrement=Tru
-00010ad0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00010ae0: 436f 6c75 6d6e 2822 696e 7465 6765 725f  Column("integer_
-00010af0: 6461 7461 222c 2064 6174 6174 7970 6529  data", datatype)
-00010b00: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00010b10: 2020 2020 206d 6574 6164 6174 612e 6372       metadata.cr
-00010b20: 6561 7465 5f61 6c6c 2863 6f6e 6669 672e  eate_all(config.
-00010b30: 6462 290a 0a20 2020 2020 2020 2063 6f6e  db)..        con
-00010b40: 6669 672e 6462 2e65 7865 6375 7465 2869  fig.db.execute(i
-00010b50: 6e74 5f74 6162 6c65 2e69 6e73 6572 7428  nt_table.insert(
-00010b60: 292c 207b 2269 6422 3a20 312c 2022 696e  ), {"id": 1, "in
-00010b70: 7465 6765 725f 6461 7461 223a 2064 6174  teger_data": dat
-00010b80: 617d 290a 0a20 2020 2020 2020 2072 6f77  a})..        row
-00010b90: 203d 2063 6f6e 6669 672e 6462 2e65 7865   = config.db.exe
-00010ba0: 6375 7465 2873 656c 6563 7428 696e 745f  cute(select(int_
-00010bb0: 7461 626c 652e 632e 696e 7465 6765 725f  table.c.integer_
-00010bc0: 6461 7461 2929 2e66 6972 7374 2829 0a0a  data)).first()..
-00010bd0: 2020 2020 2020 2020 6571 5f28 726f 772c          eq_(row,
-00010be0: 2028 6461 7461 2c29 290a 0a20 2020 2020   (data,))..     
-00010bf0: 2020 2069 6620 7574 696c 2e70 7933 6b3a     if util.py3k:
-00010c00: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00010c10: 6572 7420 6973 696e 7374 616e 6365 2872  ert isinstance(r
-00010c20: 6f77 5b30 5d2c 2069 6e74 290a 2020 2020  ow[0], int).    
-00010c30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00010c40: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00010c50: 6e73 7461 6e63 6528 726f 775b 305d 2c20  nstance(row[0], 
-00010c60: 286c 6f6e 672c 2069 6e74 2929 2020 2320  (long, int))  # 
-00010c70: 6e6f 7161 0a0a 2020 2020 6465 6620 5f68  noqa..    def _h
-00010c80: 7567 655f 696e 7473 2829 3a0a 0a20 2020  uge_ints():..   
-00010c90: 2020 2020 2072 6574 7572 6e20 7465 7374       return test
-00010ca0: 696e 672e 636f 6d62 696e 6174 696f 6e73  ing.combinations
-00010cb0: 280a 2020 2020 2020 2020 2020 2020 3231  (.            21
-00010cc0: 3437 3438 3336 3439 2c20 2023 2033 3220  47483649,  # 32 
-00010cd0: 6269 7473 0a20 2020 2020 2020 2020 2020  bits.           
-00010ce0: 2032 3134 3734 3833 3634 382c 2020 2320   2147483648,  # 
-00010cf0: 3332 2062 6974 730a 2020 2020 2020 2020  32 bits.        
-00010d00: 2020 2020 3231 3437 3438 3336 3437 2c20      2147483647, 
-00010d10: 2023 2033 3120 6269 7473 0a20 2020 2020   # 31 bits.     
-00010d20: 2020 2020 2020 2032 3134 3734 3833 3634         214748364
-00010d30: 362c 2020 2320 3331 2062 6974 730a 2020  6,  # 31 bits.  
-00010d40: 2020 2020 2020 2020 2020 2d32 3134 3734            -21474
-00010d50: 3833 3634 392c 2020 2320 3332 2062 6974  83649,  # 32 bit
-00010d60: 730a 2020 2020 2020 2020 2020 2020 2d32  s.            -2
-00010d70: 3134 3734 3833 3634 382c 2020 2320 3332  147483648,  # 32
-00010d80: 2069 6e74 6572 6573 7469 6e67 6c79 2c20   interestingly, 
-00010d90: 6173 796e 6370 6720 6163 6365 7074 7320  asyncpg accepts 
-00010da0: 7468 6973 206f 6e65 2061 7320 696e 7433  this one as int3
-00010db0: 320a 2020 2020 2020 2020 2020 2020 2d32  2.            -2
-00010dc0: 3134 3734 3833 3634 372c 2020 2320 3331  147483647,  # 31
-00010dd0: 0a20 2020 2020 2020 2020 2020 202d 3231  .            -21
-00010de0: 3437 3438 3336 3436 2c20 2023 2033 310a  47483646,  # 31.
-00010df0: 2020 2020 2020 2020 2020 2020 302c 0a20              0,. 
-00010e00: 2020 2020 2020 2020 2020 2031 3337 3635             13765
-00010e10: 3337 3031 3833 3638 3132 372c 0a20 2020  37018368127,.   
-00010e20: 2020 2020 2020 2020 202d 3133 3736 3533           -137653
-00010e30: 3730 3138 3336 3831 3237 2c0a 2020 2020  7018368127,.    
-00010e40: 2020 2020 2020 2020 6172 676e 616d 6573          argnames
-00010e50: 3d22 696e 7476 616c 7565 222c 0a20 2020  ="intvalue",.   
-00010e60: 2020 2020 2029 0a0a 2020 2020 405f 6875       )..    @_hu
-00010e70: 6765 5f69 6e74 7328 290a 2020 2020 6465  ge_ints().    de
-00010e80: 6620 7465 7374 5f68 7567 655f 696e 745f  f test_huge_int_
-00010e90: 6175 746f 5f61 6363 6f6d 6d6f 6461 7469  auto_accommodati
-00010ea0: 6f6e 2873 656c 662c 2063 6f6e 6e65 6374  on(self, connect
-00010eb0: 696f 6e2c 2069 6e74 7661 6c75 6529 3a0a  ion, intvalue):.
-00010ec0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010ed0: 2020 2020 5370 616e 6e65 7220 646f 6573      Spanner does
-00010ee0: 206e 6f74 2061 6c6c 6f77 2071 7565 7279   not allow query
-00010ef0: 2074 6f20 6861 7665 2046 524f 4d20 636c   to have FROM cl
-00010f00: 6175 7365 2077 6974 686f 7574 2061 2057  ause without a W
-00010f10: 4845 5245 2063 6c61 7573 650a 2020 2020  HERE clause.    
-00010f20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010f30: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
-00010f40: 2063 6f6e 6e65 6374 696f 6e2e 7363 616c   connection.scal
-00010f50: 6172 2873 656c 6563 7428 696e 7476 616c  ar(select(intval
-00010f60: 7565 2929 2c0a 2020 2020 2020 2020 2020  ue)),.          
-00010f70: 2020 696e 7476 616c 7565 2c0a 2020 2020    intvalue,.    
-00010f80: 2020 2020 290a 0a0a 636c 6173 7320 5f55      )...class _U
-00010f90: 6e69 636f 6465 4669 7874 7572 6528 5f5f  nicodeFixture(__
-00010fa0: 556e 6963 6f64 6546 6978 7475 7265 293a  UnicodeFixture):
-00010fb0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00010fc0: 640a 2020 2020 6465 6620 6465 6669 6e65  d.    def define
-00010fd0: 5f74 6162 6c65 7328 636c 732c 206d 6574  _tables(cls, met
-00010fe0: 6164 6174 6129 3a0a 2020 2020 2020 2020  adata):.        
-00010ff0: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-00011000: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-00011010: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
-00011020: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-00011030: 706f 7274 2061 7574 6f20 696e 6372 656d  port auto increm
-00011040: 656e 7469 6e67 2069 6473 2066 6561 7475  enting ids featu
-00011050: 7265 2c0a 2020 2020 2020 2020 7768 6963  re,.        whic
-00011060: 6820 6973 2075 7365 6420 6279 2074 6865  h is used by the
-00011070: 206f 7269 6769 6e61 6c20 7465 7374 2e20   original test. 
-00011080: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
-00011090: 6573 7420 6461 7461 0a20 2020 2020 2020  est data.       
-000110a0: 2063 7265 6174 696f 6e20 6d65 7468 6f64   creation method
-000110b0: 2074 6f20 6469 7361 626c 6520 6175 746f   to disable auto
-000110c0: 696e 6372 656d 656e 7420 616e 6420 6d61  increment and ma
-000110d0: 6b65 2069 6420 636f 6c75 6d6e 0a20 2020  ke id column.   
-000110e0: 2020 2020 206e 756c 6c61 626c 652e 0a20       nullable.. 
-000110f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011100: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
-00011110: 2020 2020 2020 2275 6e69 636f 6465 5f74        "unicode_t
-00011120: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
-00011130: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
-00011140: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00011150: 2269 6422 2c20 496e 7465 6765 722c 2070  "id", Integer, p
-00011160: 7269 6d61 7279 5f6b 6579 3d54 7275 652c  rimary_key=True,
-00011170: 206e 756c 6c61 626c 653d 5472 7565 292c   nullable=True),
-00011180: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-00011190: 756d 6e28 2275 6e69 636f 6465 5f64 6174  umn("unicode_dat
-000111a0: 6122 2c20 636c 732e 6461 7461 7479 7065  a", cls.datatype
-000111b0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
-000111c0: 2020 6465 6620 7465 7374 5f72 6f75 6e64    def test_round
-000111d0: 5f74 7269 705f 6578 6563 7574 656d 616e  _trip_executeman
-000111e0: 7928 7365 6c66 2c20 636f 6e6e 6563 7469  y(self, connecti
-000111f0: 6f6e 293a 0a20 2020 2020 2020 2022 2222  on):.        """
-00011200: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-00011210: 204f 5645 5252 4944 450a 0a20 2020 2020   OVERRIDE..     
-00011220: 2020 2043 6c6f 7564 2053 7061 6e6e 6572     Cloud Spanner
-00011230: 2073 7570 706f 7274 7320 7461 626c 6573   supports tables
-00011240: 2077 6974 6820 656d 7074 7920 7072 696d   with empty prim
-00011250: 6172 7920 6b65 792c 2062 7574 0a20 2020  ary key, but.   
-00011260: 2020 2020 206f 6e6c 7920 7369 6e67 6c65       only single
-00011270: 206f 6e65 2072 6f77 2063 616e 2062 6520   one row can be 
-00011280: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
-00011290: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
-000112a0: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
-000112b0: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
-000112c0: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
-000112d0: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
-000112e0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
-000112f0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-00011300: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
-00011310: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
-00011320: 2022 2222 0a20 2020 2020 2020 2075 6e69   """.        uni
-00011330: 636f 6465 5f74 6162 6c65 203d 2073 656c  code_table = sel
-00011340: 662e 7461 626c 6573 2e75 6e69 636f 6465  f.tables.unicode
-00011350: 5f74 6162 6c65 0a0a 2020 2020 2020 2020  _table..        
-00011360: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
-00011370: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00011380: 756e 6963 6f64 655f 7461 626c 652e 696e  unicode_table.in
-00011390: 7365 7274 2829 2c0a 2020 2020 2020 2020  sert(),.        
-000113a0: 2020 2020 5b7b 2269 6422 3a20 692c 2022      [{"id": i, "
-000113b0: 756e 6963 6f64 655f 6461 7461 223a 2073  unicode_data": s
-000113c0: 656c 662e 6461 7461 7d20 666f 7220 6920  elf.data} for i 
-000113d0: 696e 2072 616e 6765 2831 2c20 3429 5d2c  in range(1, 4)],
-000113e0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000113f0: 2020 2020 726f 7773 203d 2063 6f6e 6e65      rows = conne
-00011400: 6374 696f 6e2e 6578 6563 7574 6528 7365  ction.execute(se
-00011410: 6c65 6374 2875 6e69 636f 6465 5f74 6162  lect(unicode_tab
-00011420: 6c65 2e63 2e75 6e69 636f 6465 5f64 6174  le.c.unicode_dat
-00011430: 6129 292e 6665 7463 6861 6c6c 2829 0a20  a)).fetchall(). 
-00011440: 2020 2020 2020 2065 715f 2872 6f77 732c         eq_(rows,
-00011450: 205b 2873 656c 662e 6461 7461 2c29 2066   [(self.data,) f
-00011460: 6f72 2069 2069 6e20 7261 6e67 6528 312c  or i in range(1,
-00011470: 2034 295d 290a 2020 2020 2020 2020 666f   4)]).        fo
-00011480: 7220 726f 7720 696e 2072 6f77 733a 0a20  r row in rows:. 
-00011490: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-000114a0: 7420 6973 696e 7374 616e 6365 2872 6f77  t isinstance(row
-000114b0: 5b30 5d2c 2073 7472 290a 0a20 2020 2040  [0], str)..    @
-000114c0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-000114d0: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-000114e0: 7420 7375 7070 6f72 7420 6e6f 6e2d 6173  t support non-as
-000114f0: 6369 6920 6368 6172 6163 7465 7273 2229  cii characters")
-00011500: 0a20 2020 2064 6566 2074 6573 745f 6c69  .    def test_li
-00011510: 7465 7261 6c28 7365 6c66 293a 0a20 2020  teral(self):.   
-00011520: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-00011530: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-00011540: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-00011550: 7420 7375 7070 6f72 7420 6e6f 6e2d 6173  t support non-as
-00011560: 6369 6920 6368 6172 6163 7465 7273 2229  cii characters")
-00011570: 0a20 2020 2064 6566 2074 6573 745f 6c69  .    def test_li
-00011580: 7465 7261 6c5f 6e6f 6e5f 6173 6369 6928  teral_non_ascii(
-00011590: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000115a0: 6173 730a 0a0a 636c 6173 7320 556e 6963  ass...class Unic
-000115b0: 6f64 6556 6172 6368 6172 5465 7374 285f  odeVarcharTest(_
-000115c0: 556e 6963 6f64 6546 6978 7475 7265 2c20  UnicodeFixture, 
-000115d0: 5f55 6e69 636f 6465 5661 7263 6861 7254  _UnicodeVarcharT
-000115e0: 6573 7429 3a0a 2020 2020 2222 220a 2020  est):.    """.  
-000115f0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-00011600: 4445 3a0a 0a20 2020 2055 6e69 636f 6465  DE:..    Unicode
-00011610: 5661 7263 6861 7254 6573 7420 636c 6173  VarcharTest clas
-00011620: 7320 696e 6865 7269 7473 2074 6865 205f  s inherits the _
-00011630: 5f55 6e69 636f 6465 4669 7874 7572 6520  _UnicodeFixture 
-00011640: 636c 6173 7327 7320 7465 7374 732c 0a20  class's tests,. 
-00011650: 2020 2073 6f20 746f 2061 766f 6964 2074     so to avoid t
-00011660: 686f 7365 2066 6169 6c75 7265 7320 616e  hose failures an
-00011670: 6420 6d61 696e 7461 696e 2044 5259 2063  d maintain DRY c
-00011680: 6f6e 6365 7074 206a 7573 7420 696e 6865  oncept just inhe
-00011690: 7269 7420 7468 6520 636c 6173 7320 746f  rit the class to
-000116a0: 2072 756e 0a20 2020 2074 6573 7473 2073   run.    tests s
-000116b0: 7563 6365 7373 6675 6c6c 792e 0a20 2020  uccessfully..   
-000116c0: 2022 2222 0a0a 2020 2020 7061 7373 0a0a   """..    pass..
-000116d0: 0a63 6c61 7373 2055 6e69 636f 6465 5465  .class UnicodeTe
-000116e0: 7874 5465 7374 285f 556e 6963 6f64 6546  xtTest(_UnicodeF
-000116f0: 6978 7475 7265 2c20 5f55 6e69 636f 6465  ixture, _Unicode
-00011700: 5465 7874 5465 7374 293a 0a20 2020 2022  TextTest):.    "
-00011710: 2222 0a20 2020 2053 5041 4e4e 4552 204f  "".    SPANNER O
-00011720: 5645 5252 4944 453a 0a0a 2020 2020 556e  VERRIDE:..    Un
-00011730: 6963 6f64 6554 6578 7454 6573 7420 636c  icodeTextTest cl
-00011740: 6173 7320 696e 6865 7269 7473 2074 6865  ass inherits the
-00011750: 205f 5f55 6e69 636f 6465 4669 7874 7572   __UnicodeFixtur
-00011760: 6520 636c 6173 7327 7320 7465 7374 732c  e class's tests,
-00011770: 0a20 2020 2073 6f20 746f 2061 766f 6964  .    so to avoid
-00011780: 2074 686f 7365 2066 6169 6c75 7265 7320   those failures 
-00011790: 616e 6420 6d61 696e 7461 696e 2044 5259  and maintain DRY
-000117a0: 2063 6f6e 6365 7074 206a 7573 7420 696e   concept just in
-000117b0: 6865 7269 7420 7468 6520 636c 6173 7320  herit the class 
-000117c0: 746f 2072 756e 0a20 2020 2074 6573 7473  to run.    tests
-000117d0: 2073 7563 6365 7373 6675 6c6c 792e 0a20   successfully.. 
-000117e0: 2020 2022 2222 0a0a 2020 2020 7061 7373     """..    pass
-000117f0: 0a0a 0a63 6c61 7373 2052 6f77 4665 7463  ...class RowFetc
-00011800: 6854 6573 7428 5f52 6f77 4665 7463 6854  hTest(_RowFetchT
-00011810: 6573 7429 3a0a 2020 2020 6465 6620 7465  est):.    def te
-00011820: 7374 5f72 6f77 5f77 5f73 6361 6c61 725f  st_row_w_scalar_
-00011830: 7365 6c65 6374 2873 656c 662c 2063 6f6e  select(self, con
-00011840: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-00011850: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-00011860: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-00011870: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
-00011880: 7061 6e6e 6572 2072 6574 7572 6e73 2061  panner returns a
-00011890: 2044 6174 6574 696d 6557 6974 684e 616e   DatetimeWithNan
-000118a0: 6f73 6563 6f6e 6473 2829 2066 6f72 2064  oseconds() for d
-000118b0: 6174 650a 2020 2020 2020 2020 6461 7461  ate.        data
-000118c0: 2074 7970 6573 2e20 4f76 6572 7269 6469   types. Overridi
-000118d0: 6e67 2074 6865 2074 6573 7420 746f 2075  ng the test to u
-000118e0: 7365 2061 2044 6174 6574 696d 6557 6974  se a DatetimeWit
-000118f0: 684e 616e 6f73 6563 6f6e 6473 0a20 2020  hNanoseconds.   
-00011900: 2020 2020 2074 7970 6520 7661 6c75 6520       type value 
-00011910: 6173 2061 6e20 6578 7065 6374 6564 2072  as an expected r
-00011920: 6573 756c 742e 0a20 2020 2020 2020 202d  esult..        -
-00011930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20  -------------.. 
-00011940: 2020 2020 2020 2074 6573 7420 7468 6174         test that
-00011950: 2061 2073 6361 6c61 7220 7365 6c65 6374   a scalar select
-00011960: 2061 7320 6120 636f 6c75 6d6e 2069 7320   as a column is 
-00011970: 7265 7475 726e 6564 2061 7320 7375 6368  returned as such
-00011980: 0a20 2020 2020 2020 2061 6e64 2074 6861  .        and tha
-00011990: 7420 7479 7065 2063 6f6e 7665 7273 696f  t type conversio
-000119a0: 6e20 776f 726b 7320 4f4b 2e0a 0a20 2020  n works OK...   
-000119b0: 2020 2020 2028 7468 6973 2069 7320 6861       (this is ha
-000119c0: 6c66 2061 2053 514c 416c 6368 656d 7920  lf a SQLAlchemy 
-000119d0: 436f 7265 2074 6573 7420 616e 6420 6861  Core test and ha
-000119e0: 6c66 2074 6f20 6361 7463 6820 6461 7461  lf to catch data
-000119f0: 6261 7365 0a20 2020 2020 2020 2062 6163  base.        bac
-00011a00: 6b65 6e64 7320 7468 6174 206d 6179 2068  kends that may h
-00011a10: 6176 6520 756e 7573 7561 6c20 6265 6861  ave unusual beha
-00011a20: 7669 6f72 2077 6974 6820 7363 616c 6172  vior with scalar
-00011a30: 2073 656c 6563 7473 2e29 0a20 2020 2020   selects.).     
-00011a40: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-00011a50: 6174 6574 6162 6c65 203d 2073 656c 662e  atetable = self.
-00011a60: 7461 626c 6573 2e68 6173 5f64 6174 6573  tables.has_dates
-00011a70: 0a20 2020 2020 2020 2073 203d 2073 656c  .        s = sel
-00011a80: 6563 7428 6461 7465 7461 626c 652e 616c  ect(datetable.al
-00011a90: 6961 7328 2278 2229 2e63 2e74 6f64 6179  ias("x").c.today
-00011aa0: 292e 7363 616c 6172 5f73 7562 7175 6572  ).scalar_subquer
-00011ab0: 7928 290a 2020 2020 2020 2020 7332 203d  y().        s2 =
-00011ac0: 2073 656c 6563 7428 6461 7465 7461 626c   select(datetabl
-00011ad0: 652e 632e 6964 2c20 732e 6c61 6265 6c28  e.c.id, s.label(
-00011ae0: 2273 6f6d 656c 6162 656c 2229 290a 2020  "somelabel")).  
-00011af0: 2020 2020 2020 726f 7720 3d20 636f 6e6e        row = conn
-00011b00: 6563 7469 6f6e 2e65 7865 6375 7465 2873  ection.execute(s
-00011b10: 3229 2e66 6972 7374 2829 0a0a 2020 2020  2).first()..    
-00011b20: 2020 2020 6571 5f28 0a20 2020 2020 2020      eq_(.       
-00011b30: 2020 2020 2072 6f77 2e73 6f6d 656c 6162       row.somelab
-00011b40: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-00011b50: 4461 7465 7469 6d65 5769 7468 4e61 6e6f  DatetimeWithNano
-00011b60: 7365 636f 6e64 7328 3230 3036 2c20 352c  seconds(2006, 5,
-00011b70: 2031 322c 2031 322c 2030 2c20 302c 2074   12, 12, 0, 0, t
-00011b80: 7a69 6e66 6f3d 7469 6d65 7a6f 6e65 2e75  zinfo=timezone.u
-00011b90: 7463 292c 0a20 2020 2020 2020 2029 0a0a  tc),.        )..
-00011ba0: 0a63 6c61 7373 2049 6e73 6572 7442 6568  .class InsertBeh
-00011bb0: 6176 696f 7254 6573 7428 5f49 6e73 6572  aviorTest(_Inser
-00011bc0: 7442 6568 6176 696f 7254 6573 7429 3a0a  tBehaviorTest):.
-00011bd0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00011be0: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-00011bf0: 6f65 736e 2774 2073 7570 706f 7274 2065  oesn't support e
-00011c00: 6d70 7479 2069 6e73 6572 7473 2229 0a20  mpty inserts"). 
-00011c10: 2020 2064 6566 2074 6573 745f 656d 7074     def test_empt
-00011c20: 795f 696e 7365 7274 2873 656c 6629 3a0a  y_insert(self):.
-00011c30: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00011c40: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00011c50: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-00011c60: 736e 2774 2073 7570 706f 7274 2065 6d70  sn't support emp
-00011c70: 7479 2069 6e73 6572 7473 2229 0a20 2020  ty inserts").   
-00011c80: 2064 6566 2074 6573 745f 656d 7074 795f   def test_empty_
-00011c90: 696e 7365 7274 5f6d 756c 7469 706c 6528  insert_multiple(
-00011ca0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00011cb0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-00011cc0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-00011cd0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-00011ce0: 6f72 7420 6175 746f 2069 6e63 7265 6d65  ort auto increme
-00011cf0: 6e74 2229 0a20 2020 2064 6566 2074 6573  nt").    def tes
-00011d00: 745f 696e 7365 7274 5f66 726f 6d5f 7365  t_insert_from_se
-00011d10: 6c65 6374 5f61 7574 6f69 6e63 2873 656c  lect_autoinc(sel
-00011d20: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00011d30: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
-00011d40: 7574 6f63 6c6f 7365 5f6f 6e5f 696e 7365  utoclose_on_inse
-00011d50: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
-00011d60: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-00011d70: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-00011d80: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
-00011d90: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
-00011da0: 7570 706f 7274 2074 6162 6c65 7320 7769  upport tables wi
-00011db0: 7468 2061 6e20 6175 746f 2069 6e63 7265  th an auto incre
-00011dc0: 6d65 6e74 2070 7269 6d61 7279 206b 6579  ment primary key
-00011dd0: 2c0a 2020 2020 2020 2020 666f 6c6c 6f77  ,.        follow
-00011de0: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
-00011df0: 696c 6c20 6661 696c 2077 6974 6820 6034  ill fail with `4
-00011e00: 3030 2069 6420 6d75 7374 206e 6f74 2062  00 id must not b
-00011e10: 6520 4e55 4c4c 2069 6e20 7461 626c 650a  e NULL in table.
-00011e20: 2020 2020 2020 2020 6175 746f 696e 635f          autoinc_
-00011e30: 706b 602e 0a0a 2020 2020 2020 2020 4f76  pk`...        Ov
-00011e40: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
-00011e50: 7473 2061 6e64 2061 6464 696e 6720 6120  ts and adding a 
-00011e60: 6d61 6e75 616c 2070 7269 6d61 7279 206b  manual primary k
-00011e70: 6579 2076 616c 7565 2074 6f20 6176 6f69  ey value to avoi
-00011e80: 6420 7468 6520 7361 6d65 0a20 2020 2020  d the same.     
-00011e90: 2020 2066 6169 6c75 7265 732e 0a20 2020     failures..   
-00011ea0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011eb0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00011ec0: 2020 6861 7361 7474 7228 636f 6e66 6967    hasattr(config
-00011ed0: 2e72 6571 7569 7265 6d65 6e74 732c 2022  .requirements, "
-00011ee0: 7265 7475 726e 696e 6722 290a 2020 2020  returning").    
-00011ef0: 2020 2020 2020 2020 616e 6420 636f 6e66          and conf
-00011f00: 6967 2e72 6571 7569 7265 6d65 6e74 732e  ig.requirements.
-00011f10: 7265 7475 726e 696e 672e 656e 6162 6c65  returning.enable
-00011f20: 640a 2020 2020 2020 2020 293a 0a20 2020  d.        ):.   
-00011f30: 2020 2020 2020 2020 2065 6e67 696e 6520           engine 
-00011f40: 3d20 656e 6769 6e65 732e 7465 7374 696e  = engines.testin
-00011f50: 675f 656e 6769 6e65 286f 7074 696f 6e73  g_engine(options
-00011f60: 3d7b 2269 6d70 6c69 6369 745f 7265 7475  ={"implicit_retu
-00011f70: 726e 696e 6722 3a20 4661 6c73 657d 290a  rning": False}).
-00011f80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00011f90: 2020 2020 2020 2020 2020 656e 6769 6e65            engine
-00011fa0: 203d 2063 6f6e 6669 672e 6462 0a0a 2020   = config.db..  
-00011fb0: 2020 2020 2020 7769 7468 2065 6e67 696e        with engin
-00011fc0: 652e 6265 6769 6e28 2920 6173 2063 6f6e  e.begin() as con
-00011fd0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
-00011fe0: 203d 2063 6f6e 6e2e 6578 6563 7574 6528   = conn.execute(
-00011ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012000: 2073 656c 662e 7461 626c 6573 2e61 7574   self.tables.aut
-00012010: 6f69 6e63 5f70 6b2e 696e 7365 7274 2829  oinc_pk.insert()
-00012020: 2c20 6469 6374 2869 643d 312c 2064 6174  , dict(id=1, dat
-00012030: 613d 2273 6f6d 6520 6461 7461 2229 0a20  a="some data"). 
-00012040: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00012050: 2020 2020 2020 6173 7365 7274 2072 2e5f        assert r._
-00012060: 736f 6674 5f63 6c6f 7365 640a 2020 2020  soft_closed.    
-00012070: 2020 2020 6173 7365 7274 206e 6f74 2072      assert not r
-00012080: 2e63 6c6f 7365 640a 2020 2020 2020 2020  .closed.        
-00012090: 6173 7365 7274 2072 2e69 735f 696e 7365  assert r.is_inse
-000120a0: 7274 0a20 2020 2020 2020 2061 7373 6572  rt.        asser
-000120b0: 7420 6e6f 7420 722e 7265 7475 726e 735f  t not r.returns_
-000120c0: 726f 7773 0a0a 0a63 6c61 7373 2042 7974  rows...class Byt
-000120d0: 6573 5465 7374 285f 4c69 7465 7261 6c52  esTest(_LiteralR
-000120e0: 6f75 6e64 5472 6970 4669 7874 7572 652c  oundTripFixture,
-000120f0: 2066 6978 7475 7265 732e 5465 7374 4261   fixtures.TestBa
-00012100: 7365 293a 0a20 2020 205f 5f62 6163 6b65  se):.    __backe
-00012110: 6e64 5f5f 203d 2054 7275 650a 0a20 2020  nd__ = True..   
-00012120: 2064 6566 2074 6573 745f 6e6f 6c65 6e67   def test_noleng
-00012130: 7468 5f62 696e 6172 7928 7365 6c66 293a  th_binary(self):
-00012140: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00012150: 6120 3d20 4d65 7461 4461 7461 2829 0a20  a = MetaData(). 
-00012160: 2020 2020 2020 2066 6f6f 203d 2054 6162         foo = Tab
-00012170: 6c65 2822 666f 6f22 2c20 6d65 7461 6461  le("foo", metada
-00012180: 7461 2c20 436f 6c75 6d6e 2822 6f6e 6522  ta, Column("one"
-00012190: 2c20 4c61 7267 6542 696e 6172 7929 290a  , LargeBinary)).
-000121a0: 0a20 2020 2020 2020 2066 6f6f 2e63 7265  .        foo.cre
-000121b0: 6174 6528 636f 6e66 6967 2e64 6229 0a20  ate(config.db). 
-000121c0: 2020 2020 2020 2066 6f6f 2e64 726f 7028         foo.drop(
-000121d0: 636f 6e66 6967 2e64 6229 0a0a 0a63 6c61  config.db)...cla
-000121e0: 7373 2053 7472 696e 6754 6573 7428 5f53  ss StringTest(_S
-000121f0: 7472 696e 6754 6573 7429 3a0a 2020 2020  tringTest):.    
-00012200: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00012210: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
-00012220: 2774 2073 7570 706f 7274 206e 6f6e 2d61  't support non-a
-00012230: 7363 6969 2063 6861 7261 6374 6572 7322  scii characters"
-00012240: 290a 2020 2020 6465 6620 7465 7374 5f6c  ).    def test_l
-00012250: 6974 6572 616c 5f6e 6f6e 5f61 7363 6969  iteral_non_ascii
-00012260: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00012270: 7061 7373 0a0a 2020 2020 6465 6620 7465  pass..    def te
-00012280: 7374 5f64 6f6e 745f 7472 756e 6361 7465  st_dont_truncate
-00012290: 5f72 6967 6874 7369 6465 280a 2020 2020  _rightside(.    
-000122a0: 2020 2020 7365 6c66 2c20 6d65 7461 6461      self, metada
-000122b0: 7461 2c20 636f 6e6e 6563 7469 6f6e 2c20  ta, connection, 
-000122c0: 6578 7072 3d4e 6f6e 652c 2065 7870 6563  expr=None, expec
-000122d0: 7465 643d 4e6f 6e65 0a20 2020 2029 3a0a  ted=None.    ):.
-000122e0: 2020 2020 2020 2020 7420 3d20 5461 626c          t = Tabl
-000122f0: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00012300: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00012310: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00012320: 2020 2020 2020 436f 6c75 6d6e 2822 7822        Column("x"
-00012330: 2c20 5374 7269 6e67 2832 2929 2c0a 2020  , String(2)),.  
-00012340: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00012350: 2822 6964 222c 2049 6e74 6567 6572 2c20  ("id", Integer, 
-00012360: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00012370: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
-00012380: 2020 2020 2074 2e63 7265 6174 6528 636f       t.create(co
-00012390: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
-000123a0: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
-000123b0: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
-000123c0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-000123d0: 696f 6e2e 6578 6563 7574 6528 0a20 2020  ion.execute(.   
-000123e0: 2020 2020 2020 2020 2074 2e69 6e73 6572           t.inser
-000123f0: 7428 292c 0a20 2020 2020 2020 2020 2020  t(),.           
-00012400: 205b 7b22 7822 3a20 2241 4222 2c20 2269   [{"x": "AB", "i
-00012410: 6422 3a20 317d 2c20 7b22 7822 3a20 2242  d": 1}, {"x": "B
-00012420: 4322 2c20 2269 6422 3a20 327d 2c20 7b22  C", "id": 2}, {"
-00012430: 7822 3a20 2241 4322 2c20 2269 6422 3a20  x": "AC", "id": 
-00012440: 337d 5d2c 0a20 2020 2020 2020 2029 0a20  3}],.        ). 
-00012450: 2020 2020 2020 2063 6f6d 6269 6e61 7469         combinati
-00012460: 6f6e 7320 3d20 5b28 2225 4225 222c 205b  ons = [("%B%", [
-00012470: 2241 4222 2c20 2242 4322 5d29 2c20 2822  "AB", "BC"]), ("
-00012480: 4125 4322 2c20 5b22 4143 225d 292c 2028  A%C", ["AC"]), (
-00012490: 2241 2543 255a 222c 205b 5d29 5d0a 0a20  "A%C%Z", [])].. 
-000124a0: 2020 2020 2020 2066 6f72 2061 7267 7320         for args 
-000124b0: 696e 2063 6f6d 6269 6e61 7469 6f6e 733a  in combinations:
-000124c0: 0a20 2020 2020 2020 2020 2020 2065 715f  .            eq_
-000124d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000124e0: 2020 636f 6e6e 6563 7469 6f6e 2e73 6361    connection.sca
-000124f0: 6c61 7273 2873 656c 6563 7428 742e 632e  lars(select(t.c.
-00012500: 7829 2e77 6865 7265 2874 2e63 2e78 2e6c  x).where(t.c.x.l
-00012510: 696b 6528 6172 6773 5b30 5d29 2929 2e61  ike(args[0]))).a
-00012520: 6c6c 2829 2c0a 2020 2020 2020 2020 2020  ll(),.          
-00012530: 2020 2020 2020 6172 6773 5b31 5d2c 0a20        args[1],. 
-00012540: 2020 2020 2020 2020 2020 2029 0a0a 0a63             )...c
-00012550: 6c61 7373 2054 6578 7454 6573 7428 5f54  lass TextTest(_T
-00012560: 6578 7454 6573 7429 3a0a 2020 2020 4063  extTest):.    @c
-00012570: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00012580: 6566 2064 6566 696e 655f 7461 626c 6573  ef define_tables
-00012590: 2863 6c73 2c20 6d65 7461 6461 7461 293a  (cls, metadata):
-000125a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000125b0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-000125c0: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
-000125d0: 436c 6f75 6420 5370 616e 6e65 7220 646f  Cloud Spanner do
-000125e0: 6573 6e27 7420 7375 7070 6f72 7420 6175  esn't support au
-000125f0: 746f 2069 6e63 7265 6d65 6e74 696e 6720  to incrementing 
-00012600: 6964 7320 6665 6174 7572 652c 0a20 2020  ids feature,.   
-00012610: 2020 2020 2077 6869 6368 2069 7320 7573       which is us
-00012620: 6564 2062 7920 7468 6520 6f72 6967 696e  ed by the origin
-00012630: 616c 2074 6573 742e 204f 7665 7272 6964  al test. Overrid
-00012640: 696e 6720 7468 6520 7465 7374 2064 6174  ing the test dat
-00012650: 610a 2020 2020 2020 2020 6372 6561 7469  a.        creati
-00012660: 6f6e 206d 6574 686f 6420 746f 2064 6973  on method to dis
-00012670: 6162 6c65 2061 7574 6f69 6e63 7265 6d65  able autoincreme
-00012680: 6e74 2061 6e64 206d 616b 6520 6964 2063  nt and make id c
-00012690: 6f6c 756d 6e0a 2020 2020 2020 2020 6e75  olumn.        nu
-000126a0: 6c6c 6162 6c65 2e0a 2020 2020 2020 2020  llable..        
-000126b0: 2222 220a 2020 2020 2020 2020 5461 626c  """.        Tabl
-000126c0: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-000126d0: 7465 7874 5f74 6162 6c65 222c 0a20 2020  text_table",.   
-000126e0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-000126f0: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
-00012700: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
-00012710: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00012720: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
-00012730: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00012740: 2020 2043 6f6c 756d 6e28 2274 6578 745f     Column("text_
-00012750: 6461 7461 222c 2054 6578 7429 2c0a 2020  data", Text),.  
-00012760: 2020 2020 2020 290a 0a20 2020 2040 7079        )..    @py
-00012770: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00012780: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-00012790: 7375 7070 6f72 7420 6e6f 6e2d 6173 6369  support non-asci
-000127a0: 6920 6368 6172 6163 7465 7273 2229 0a20  i characters"). 
-000127b0: 2020 2064 6566 2074 6573 745f 6c69 7465     def test_lite
-000127c0: 7261 6c5f 6e6f 6e5f 6173 6369 6928 7365  ral_non_ascii(se
-000127d0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000127e0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
-000127f0: 6172 6b2e 736b 6970 2822 4e6f 7420 7375  ark.skip("Not su
-00012800: 7070 6f72 7465 6420 6279 2053 7061 6e6e  pported by Spann
-00012810: 6572 2229 0a20 2020 2064 6566 2074 6573  er").    def tes
-00012820: 745f 7465 7874 5f72 6f75 6e64 7472 6970  t_text_roundtrip
-00012830: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
-00012840: 6e29 3a0a 2020 2020 2020 2020 7061 7373  n):.        pass
-00012850: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00012860: 726b 2e73 6b69 7028 224e 6f74 2073 7570  rk.skip("Not sup
-00012870: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
-00012880: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
-00012890: 5f74 6578 745f 656d 7074 795f 7374 7269  _text_empty_stri
-000128a0: 6e67 7328 7365 6c66 2c20 636f 6e6e 6563  ngs(self, connec
-000128b0: 7469 6f6e 293a 0a20 2020 2020 2020 2070  tion):.        p
-000128c0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-000128d0: 2e6d 6172 6b2e 736b 6970 2822 4e6f 7420  .mark.skip("Not 
-000128e0: 7375 7070 6f72 7465 6420 6279 2053 7061  supported by Spa
-000128f0: 6e6e 6572 2229 0a20 2020 2064 6566 2074  nner").    def t
-00012900: 6573 745f 7465 7874 5f6e 756c 6c5f 7374  est_text_null_st
-00012910: 7269 6e67 7328 7365 6c66 2c20 636f 6e6e  rings(self, conn
-00012920: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
-00012930: 2070 6173 730a 0a0a 636c 6173 7320 4e75   pass...class Nu
-00012940: 6d65 7269 6354 6573 7428 5f4e 756d 6572  mericTest(_Numer
-00012950: 6963 5465 7374 293a 0a20 2020 2040 7465  icTest):.    @te
-00012960: 7374 696e 672e 6669 7874 7572 650a 2020  sting.fixture.  
-00012970: 2020 6465 6620 646f 5f6e 756d 6572 6963    def do_numeric
-00012980: 5f74 6573 7428 7365 6c66 2c20 6d65 7461  _test(self, meta
-00012990: 6461 7461 2c20 636f 6e6e 6563 7469 6f6e  data, connection
-000129a0: 293a 0a20 2020 2020 2020 2040 7465 7374  ):.        @test
-000129b0: 696e 672e 656d 6974 735f 7761 726e 696e  ing.emits_warnin
-000129c0: 6728 7222 2e2a 646f 6573 205c 2a6e 6f74  g(r".*does \*not
-000129d0: 5c2a 2073 7570 706f 7274 2044 6563 696d  \* support Decim
-000129e0: 616c 206f 626a 6563 7473 206e 6174 6976  al objects nativ
-000129f0: 656c 7922 290a 2020 2020 2020 2020 6465  ely").        de
-00012a00: 6620 7275 6e28 7479 7065 5f2c 2069 6e70  f run(type_, inp
-00012a10: 7574 5f2c 206f 7574 7075 742c 2066 696c  ut_, output, fil
-00012a20: 7465 725f 3d4e 6f6e 652c 2063 6865 636b  ter_=None, check
-00012a30: 5f73 6361 6c65 3d46 616c 7365 293a 0a20  _scale=False):. 
-00012a40: 2020 2020 2020 2020 2020 2074 203d 2054             t = T
-00012a50: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
-00012a60: 2020 2020 2020 2274 222c 0a20 2020 2020        "t",.     
-00012a70: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00012a80: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00012a90: 2020 2020 2043 6f6c 756d 6e28 2278 222c       Column("x",
-00012aa0: 2074 7970 655f 292c 0a20 2020 2020 2020   type_),.       
-00012ab0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00012ac0: 2269 6422 2c20 496e 7465 6765 722c 2070  "id", Integer, p
-00012ad0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-00012ae0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00012af0: 2020 2020 2020 2020 2020 2020 742e 6372              t.cr
-00012b00: 6561 7465 2863 6f6e 6e65 6374 696f 6e29  eate(connection)
-00012b10: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00012b20: 6e65 6374 696f 6e2e 636f 6e6e 6563 7469  nection.connecti
-00012b30: 6f6e 2e63 6f6d 6d69 7428 290a 2020 2020  on.commit().    
-00012b40: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
-00012b50: 6f6e 2e65 7865 6375 7465 280a 2020 2020  on.execute(.    
-00012b60: 2020 2020 2020 2020 2020 2020 742e 696e              t.in
-00012b70: 7365 7274 2829 2c20 5b7b 2278 223a 2078  sert(), [{"x": x
-00012b80: 2c20 2269 6422 3a20 697d 2066 6f72 2069  , "id": i} for i
-00012b90: 2c20 7820 696e 2065 6e75 6d65 7261 7465  , x in enumerate
-00012ba0: 2869 6e70 7574 5f29 5d0a 2020 2020 2020  (input_)].      
-00012bb0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00012bc0: 2020 2020 2072 6573 756c 7420 3d20 7b72       result = {r
-00012bd0: 6f77 5b30 5d20 666f 7220 726f 7720 696e  ow[0] for row in
-00012be0: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
-00012bf0: 7574 6528 742e 7365 6c65 6374 2829 297d  ute(t.select())}
-00012c00: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00012c10: 7075 7420 3d20 7365 7428 6f75 7470 7574  put = set(output
-00012c20: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00012c30: 2066 696c 7465 725f 3a0a 2020 2020 2020   filter_:.      
-00012c40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00012c50: 203d 2073 6574 2866 696c 7465 725f 2878   = set(filter_(x
-00012c60: 2920 666f 7220 7820 696e 2072 6573 756c  ) for x in resul
-00012c70: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00012c80: 2020 206f 7574 7075 7420 3d20 7365 7428     output = set(
-00012c90: 6669 6c74 6572 5f28 7829 2066 6f72 2078  filter_(x) for x
-00012ca0: 2069 6e20 6f75 7470 7574 290a 2020 2020   in output).    
-00012cb0: 2020 2020 2020 2020 6571 5f28 7265 7375          eq_(resu
-00012cc0: 6c74 2c20 6f75 7470 7574 290a 2020 2020  lt, output).    
-00012cd0: 2020 2020 2020 2020 6966 2063 6865 636b          if check
-00012ce0: 5f73 6361 6c65 3a0a 2020 2020 2020 2020  _scale:.        
-00012cf0: 2020 2020 2020 2020 6571 5f28 5b73 7472          eq_([str
-00012d00: 2878 2920 666f 7220 7820 696e 2072 6573  (x) for x in res
-00012d10: 756c 745d 2c20 5b73 7472 2878 2920 666f  ult], [str(x) fo
-00012d20: 7220 7820 696e 206f 7574 7075 745d 290a  r x in output]).
-00012d30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012d40: 7275 6e0a 0a20 2020 2040 656d 6974 735f  run..    @emits_
-00012d50: 7761 726e 696e 6728 7222 2e2a 646f 6573  warning(r".*does
-00012d60: 205c 2a6e 6f74 5c2a 2073 7570 706f 7274   \*not\* support
-00012d70: 2044 6563 696d 616c 206f 626a 6563 7473   Decimal objects
-00012d80: 206e 6174 6976 656c 7922 290a 2020 2020   natively").    
-00012d90: 6465 6620 7465 7374 5f72 656e 6465 725f  def test_render_
-00012da0: 6c69 7465 7261 6c5f 6e75 6d65 7269 6328  literal_numeric(
-00012db0: 7365 6c66 2c20 6c69 7465 7261 6c5f 726f  self, literal_ro
-00012dc0: 756e 645f 7472 6970 293a 0a20 2020 2020  und_trip):.     
-00012dd0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00012de0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-00012df0: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
-00012e00: 5370 616e 6e65 7220 7375 7070 6f72 7473  Spanner supports
-00012e10: 2074 6162 6c65 7320 7769 7468 2061 6e20   tables with an 
-00012e20: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
-00012e30: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
-00012e40: 6e6c 7920 6120 7369 6e67 6c65 2072 6f77  nly a single row
-00012e50: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
-00012e60: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
-00012e70: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
-00012e80: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
-00012e90: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
-00012ea0: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
-00012eb0: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
-00012ec0: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
-00012ed0: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
-00012ee0: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
-00012ef0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012f00: 2020 2020 206c 6974 6572 616c 5f72 6f75       literal_rou
-00012f10: 6e64 5f74 7269 7028 0a20 2020 2020 2020  nd_trip(.       
-00012f20: 2020 2020 204e 756d 6572 6963 2870 7265       Numeric(pre
-00012f30: 6369 7369 6f6e 3d38 2c20 7363 616c 653d  cision=8, scale=
-00012f40: 3429 2c0a 2020 2020 2020 2020 2020 2020  4),.            
-00012f50: 5b64 6563 696d 616c 2e44 6563 696d 616c  [decimal.Decimal
-00012f60: 2822 3135 2e37 3536 3322 295d 2c0a 2020  ("15.7563")],.  
-00012f70: 2020 2020 2020 2020 2020 5b64 6563 696d            [decim
-00012f80: 616c 2e44 6563 696d 616c 2822 3135 2e37  al.Decimal("15.7
-00012f90: 3536 3322 295d 2c0a 2020 2020 2020 2020  563")],.        
-00012fa0: 290a 0a20 2020 2040 656d 6974 735f 7761  )..    @emits_wa
-00012fb0: 726e 696e 6728 7222 2e2a 646f 6573 205c  rning(r".*does \
-00012fc0: 2a6e 6f74 5c2a 2073 7570 706f 7274 2044  *not\* support D
-00012fd0: 6563 696d 616c 206f 626a 6563 7473 206e  ecimal objects n
-00012fe0: 6174 6976 656c 7922 290a 2020 2020 6465  atively").    de
-00012ff0: 6620 7465 7374 5f72 656e 6465 725f 6c69  f test_render_li
-00013000: 7465 7261 6c5f 6e75 6d65 7269 635f 6173  teral_numeric_as
-00013010: 666c 6f61 7428 7365 6c66 2c20 6c69 7465  float(self, lite
-00013020: 7261 6c5f 726f 756e 645f 7472 6970 293a  ral_round_trip):
-00013030: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013040: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-00013050: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
-00013060: 436c 6f75 6420 5370 616e 6e65 7220 7375  Cloud Spanner su
-00013070: 7070 6f72 7473 2074 6162 6c65 7320 7769  pports tables wi
-00013080: 7468 2061 6e20 656d 7074 7920 7072 696d  th an empty prim
-00013090: 6172 7920 6b65 792c 2062 7574 0a20 2020  ary key, but.   
-000130a0: 2020 2020 206f 6e6c 7920 6120 7369 6e67       only a sing
-000130b0: 6c65 2072 6f77 2063 616e 2062 6520 696e  le row can be in
-000130c0: 7365 7274 6564 2069 6e74 6f20 7375 6368  serted into such
-000130d0: 2061 2074 6162 6c65 202d 0a20 2020 2020   a table -.     
-000130e0: 2020 2066 6f6c 6c6f 7769 6e67 2069 6e73     following ins
-000130f0: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
-00013100: 6c20 7769 7468 2060 526f 7720 5b5d 2061  l with `Row [] a
-00013110: 6c72 6561 6479 2065 7869 7374 7322 2e0a  lready exists"..
-00013120: 2020 2020 2020 2020 4f76 6572 7269 6469          Overridi
-00013130: 6e67 2074 6865 2074 6573 7420 746f 2061  ng the test to a
-00013140: 766f 6964 2074 6865 2073 616d 6520 6661  void the same fa
-00013150: 696c 7572 652e 0a20 2020 2020 2020 2022  ilure..        "
-00013160: 2222 0a20 2020 2020 2020 206c 6974 6572  "".        liter
-00013170: 616c 5f72 6f75 6e64 5f74 7269 7028 0a20  al_round_trip(. 
-00013180: 2020 2020 2020 2020 2020 204e 756d 6572             Numer
-00013190: 6963 2870 7265 6369 7369 6f6e 3d38 2c20  ic(precision=8, 
-000131a0: 7363 616c 653d 342c 2061 7364 6563 696d  scale=4, asdecim
-000131b0: 616c 3d46 616c 7365 292c 0a20 2020 2020  al=False),.     
-000131c0: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
-000131d0: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
-000131e0: 2229 5d2c 0a20 2020 2020 2020 2020 2020  ")],.           
-000131f0: 205b 3135 2e37 3536 335d 2c0a 2020 2020   [15.7563],.    
-00013200: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
-00013210: 6573 745f 7265 6e64 6572 5f6c 6974 6572  est_render_liter
-00013220: 616c 5f66 6c6f 6174 2873 656c 662c 206c  al_float(self, l
-00013230: 6974 6572 616c 5f72 6f75 6e64 5f74 7269  iteral_round_tri
-00013240: 7029 3a0a 2020 2020 2020 2020 2222 220a  p):.        """.
-00013250: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
-00013260: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-00013270: 2020 2043 6c6f 7564 2053 7061 6e6e 6572     Cloud Spanner
-00013280: 2073 7570 706f 7274 7320 7461 626c 6573   supports tables
-00013290: 2077 6974 6820 616e 2065 6d70 7479 2070   with an empty p
-000132a0: 7269 6d61 7279 206b 6579 2c20 6275 740a  rimary key, but.
-000132b0: 2020 2020 2020 2020 6f6e 6c79 2061 2073          only a s
-000132c0: 696e 676c 6520 726f 7720 6361 6e20 6265  ingle row can be
-000132d0: 2069 6e73 6572 7465 6420 696e 746f 2073   inserted into s
-000132e0: 7563 6820 6120 7461 626c 6520 2d0a 2020  uch a table -.  
-000132f0: 2020 2020 2020 666f 6c6c 6f77 696e 6720        following 
-00013300: 696e 7365 7274 696f 6e73 2077 696c 6c20  insertions will 
-00013310: 6661 696c 2077 6974 6820 6052 6f77 205b  fail with `Row [
-00013320: 5d20 616c 7265 6164 7920 6578 6973 7473  ] already exists
-00013330: 222e 0a20 2020 2020 2020 204f 7665 7272  "..        Overr
-00013340: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
-00013350: 6f20 6176 6f69 6420 7468 6520 7361 6d65  o avoid the same
-00013360: 2066 6169 6c75 7265 2e0a 2020 2020 2020   failure..      
-00013370: 2020 2222 220a 2020 2020 2020 2020 6c69    """.        li
-00013380: 7465 7261 6c5f 726f 756e 645f 7472 6970  teral_round_trip
-00013390: 280a 2020 2020 2020 2020 2020 2020 466c  (.            Fl
-000133a0: 6f61 7428 3429 2c0a 2020 2020 2020 2020  oat(4),.        
-000133b0: 2020 2020 5b64 6563 696d 616c 2e44 6563      [decimal.Dec
-000133c0: 696d 616c 2822 3135 2e37 3536 3322 295d  imal("15.7563")]
-000133d0: 2c0a 2020 2020 2020 2020 2020 2020 5b31  ,.            [1
-000133e0: 352e 3735 3633 5d2c 0a20 2020 2020 2020  5.7563],.       
-000133f0: 2020 2020 2066 696c 7465 725f 3d6c 616d       filter_=lam
-00013400: 6264 6120 6e3a 206e 2069 7320 6e6f 7420  bda n: n is not 
-00013410: 4e6f 6e65 2061 6e64 2072 6f75 6e64 286e  None and round(n
-00013420: 2c20 3529 206f 7220 4e6f 6e65 2c0a 2020  , 5) or None,.  
-00013430: 2020 2020 2020 290a 0a20 2020 2040 7265        )..    @re
-00013440: 7175 6972 6573 2e70 7265 6369 7369 6f6e  quires.precision
-00013450: 5f67 656e 6572 6963 5f66 6c6f 6174 5f74  _generic_float_t
-00013460: 7970 650a 2020 2020 6465 6620 7465 7374  ype.    def test
-00013470: 5f66 6c6f 6174 5f63 7573 746f 6d5f 7363  _float_custom_sc
-00013480: 616c 6528 7365 6c66 2c20 646f 5f6e 756d  ale(self, do_num
-00013490: 6572 6963 5f74 6573 7429 3a0a 2020 2020  eric_test):.    
-000134a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000134b0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
-000134c0: 3a0a 0a20 2020 2020 2020 2043 6c6f 7564  :..        Cloud
-000134d0: 2053 7061 6e6e 6572 2073 7570 706f 7274   Spanner support
-000134e0: 7320 7461 626c 6573 2077 6974 6820 616e  s tables with an
-000134f0: 2065 6d70 7479 2070 7269 6d61 7279 206b   empty primary k
-00013500: 6579 2c20 6275 740a 2020 2020 2020 2020  ey, but.        
-00013510: 6f6e 6c79 2061 2073 696e 676c 6520 726f  only a single ro
-00013520: 7720 6361 6e20 6265 2069 6e73 6572 7465  w can be inserte
-00013530: 6420 696e 746f 2073 7563 6820 6120 7461  d into such a ta
-00013540: 626c 6520 2d0a 2020 2020 2020 2020 666f  ble -.        fo
-00013550: 6c6c 6f77 696e 6720 696e 7365 7274 696f  llowing insertio
-00013560: 6e73 2077 696c 6c20 6661 696c 2077 6974  ns will fail wit
-00013570: 6820 6052 6f77 205b 5d20 616c 7265 6164  h `Row [] alread
-00013580: 7920 6578 6973 7473 222e 0a20 2020 2020  y exists"..     
-00013590: 2020 204f 7665 7272 6964 696e 6720 7468     Overriding th
-000135a0: 6520 7465 7374 2074 6f20 6176 6f69 6420  e test to avoid 
-000135b0: 7468 6520 7361 6d65 2066 6169 6c75 7265  the same failure
-000135c0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000135d0: 2020 2020 2020 646f 5f6e 756d 6572 6963        do_numeric
-000135e0: 5f74 6573 7428 0a20 2020 2020 2020 2020  _test(.         
-000135f0: 2020 2046 6c6f 6174 284e 6f6e 652c 2064     Float(None, d
-00013600: 6563 696d 616c 5f72 6574 7572 6e5f 7363  ecimal_return_sc
-00013610: 616c 653d 372c 2061 7364 6563 696d 616c  ale=7, asdecimal
-00013620: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00013630: 2020 2020 5b64 6563 696d 616c 2e44 6563      [decimal.Dec
-00013640: 696d 616c 2822 3135 2e37 3536 3338 3237  imal("15.7563827
-00013650: 2229 2c20 6465 6369 6d61 6c2e 4465 6369  "), decimal.Deci
-00013660: 6d61 6c28 2231 352e 3735 3633 3832 3722  mal("15.7563827"
-00013670: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
-00013680: 5b64 6563 696d 616c 2e44 6563 696d 616c  [decimal.Decimal
-00013690: 2822 3135 2e37 3536 3338 3237 2229 5d2c  ("15.7563827")],
-000136a0: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-000136b0: 636b 5f73 6361 6c65 3d54 7275 652c 0a20  ck_scale=True,. 
-000136c0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-000136d0: 6620 7465 7374 5f6e 756d 6572 6963 5f61  f test_numeric_a
-000136e0: 735f 6465 6369 6d61 6c28 7365 6c66 2c20  s_decimal(self, 
-000136f0: 646f 5f6e 756d 6572 6963 5f74 6573 7429  do_numeric_test)
-00013700: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013710: 2020 2020 2020 5350 414e 4e45 5220 4f56        SPANNER OV
-00013720: 4552 5249 4445 3a0a 0a20 2020 2020 2020  ERRIDE:..       
-00013730: 2053 7061 6e6e 6572 2074 6872 6f77 7320   Spanner throws 
-00013740: 616e 2065 7272 6f72 2034 3030 2056 616c  an error 400 Val
-00013750: 7565 2068 6173 2074 7970 6520 464c 4f41  ue has type FLOA
-00013760: 5436 3420 7768 6963 6820 6361 6e6e 6f74  T64 which cannot
-00013770: 2062 650a 2020 2020 2020 2020 696e 7365   be.        inse
-00013780: 7274 6564 2069 6e74 6f20 636f 6c75 6d6e  rted into column
-00013790: 2078 2c20 7768 6963 6820 6861 7320 7479   x, which has ty
-000137a0: 7065 204e 554d 4552 4943 2066 6f72 2076  pe NUMERIC for v
-000137b0: 616c 7565 2031 352e 3735 3633 2e0a 2020  alue 15.7563..  
-000137c0: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
-000137d0: 2074 6865 2074 6573 7420 746f 2072 656d   the test to rem
-000137e0: 6f76 6520 7468 6520 6661 696c 7572 6520  ove the failure 
-000137f0: 6361 7365 2e0a 2020 2020 2020 2020 2222  case..        ""
-00013800: 220a 2020 2020 2020 2020 646f 5f6e 756d  ".        do_num
-00013810: 6572 6963 5f74 6573 7428 0a20 2020 2020  eric_test(.     
-00013820: 2020 2020 2020 204e 756d 6572 6963 2870         Numeric(p
-00013830: 7265 6369 7369 6f6e 3d38 2c20 7363 616c  recision=8, scal
-00013840: 653d 3429 2c0a 2020 2020 2020 2020 2020  e=4),.          
-00013850: 2020 5b64 6563 696d 616c 2e44 6563 696d    [decimal.Decim
-00013860: 616c 2822 3135 2e37 3536 3322 292c 2064  al("15.7563"), d
-00013870: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-00013880: 3135 2e37 3536 3322 295d 2c0a 2020 2020  15.7563")],.    
-00013890: 2020 2020 2020 2020 5b64 6563 696d 616c          [decimal
-000138a0: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
-000138b0: 3322 295d 2c0a 2020 2020 2020 2020 290a  3")],.        ).
-000138c0: 0a20 2020 2064 6566 2074 6573 745f 6e75  .    def test_nu
-000138d0: 6d65 7269 635f 6173 5f66 6c6f 6174 2873  meric_as_float(s
-000138e0: 656c 662c 2064 6f5f 6e75 6d65 7269 635f  elf, do_numeric_
-000138f0: 7465 7374 293a 0a20 2020 2020 2020 2022  test):.        "
-00013900: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
-00013910: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
-00013920: 2020 2020 2020 5370 616e 6e65 7220 7468        Spanner th
-00013930: 726f 7773 2061 6e20 6572 726f 7220 3430  rows an error 40
-00013940: 3020 5661 6c75 6520 6861 7320 7479 7065  0 Value has type
-00013950: 2046 4c4f 4154 3634 2077 6869 6368 2063   FLOAT64 which c
-00013960: 616e 6e6f 7420 6265 0a20 2020 2020 2020  annot be.       
-00013970: 2069 6e73 6572 7465 6420 696e 746f 2063   inserted into c
-00013980: 6f6c 756d 6e20 782c 2077 6869 6368 2068  olumn x, which h
-00013990: 6173 2074 7970 6520 4e55 4d45 5249 4320  as type NUMERIC 
-000139a0: 666f 7220 7661 6c75 6520 3135 2e37 3536  for value 15.756
-000139b0: 332e 0a20 2020 2020 2020 204f 7665 7272  3..        Overr
-000139c0: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
-000139d0: 6f20 7265 6d6f 7665 2074 6865 2066 6169  o remove the fai
-000139e0: 6c75 7265 2063 6173 652e 0a20 2020 2020  lure case..     
-000139f0: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-00013a00: 6f5f 6e75 6d65 7269 635f 7465 7374 280a  o_numeric_test(.
-00013a10: 2020 2020 2020 2020 2020 2020 4e75 6d65              Nume
-00013a20: 7269 6328 7072 6563 6973 696f 6e3d 382c  ric(precision=8,
-00013a30: 2073 6361 6c65 3d34 2c20 6173 6465 6369   scale=4, asdeci
-00013a40: 6d61 6c3d 4661 6c73 6529 2c0a 2020 2020  mal=False),.    
-00013a50: 2020 2020 2020 2020 5b64 6563 696d 616c          [decimal
-00013a60: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
-00013a70: 3322 292c 2064 6563 696d 616c 2e44 6563  3"), decimal.Dec
-00013a80: 696d 616c 2822 3135 2e37 3536 3322 295d  imal("15.7563")]
-00013a90: 2c0a 2020 2020 2020 2020 2020 2020 5b31  ,.            [1
-00013aa0: 352e 3735 3633 5d2c 0a20 2020 2020 2020  5.7563],.       
-00013ab0: 2029 0a0a 2020 2020 4072 6571 7569 7265   )..    @require
-00013ac0: 732e 666c 6f61 7473 5f74 6f5f 666f 7572  s.floats_to_four
-00013ad0: 5f64 6563 696d 616c 730a 2020 2020 6465  _decimals.    de
-00013ae0: 6620 7465 7374 5f66 6c6f 6174 5f61 735f  f test_float_as_
-00013af0: 6465 6369 6d61 6c28 7365 6c66 2c20 646f  decimal(self, do
-00013b00: 5f6e 756d 6572 6963 5f74 6573 7429 3a0a  _numeric_test):.
-00013b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013b20: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-00013b30: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
-00013b40: 6c6f 7564 2053 7061 6e6e 6572 2073 7570  loud Spanner sup
-00013b50: 706f 7274 7320 7461 626c 6573 2077 6974  ports tables wit
-00013b60: 6820 616e 2065 6d70 7479 2070 7269 6d61  h an empty prima
-00013b70: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
-00013b80: 2020 2020 6f6e 6c79 2061 2073 696e 676c      only a singl
-00013b90: 6520 726f 7720 6361 6e20 6265 2069 6e73  e row can be ins
-00013ba0: 6572 7465 6420 696e 746f 2073 7563 6820  erted into such 
-00013bb0: 6120 7461 626c 6520 2d0a 2020 2020 2020  a table -.      
-00013bc0: 2020 666f 6c6c 6f77 696e 6720 696e 7365    following inse
-00013bd0: 7274 696f 6e73 2077 696c 6c20 6661 696c  rtions will fail
-00013be0: 2077 6974 6820 6052 6f77 205b 5d20 616c   with `Row [] al
-00013bf0: 7265 6164 7920 6578 6973 7473 222e 0a20  ready exists".. 
-00013c00: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
-00013c10: 6720 7468 6520 7465 7374 2074 6f20 6176  g the test to av
-00013c20: 6f69 6420 7468 6520 7361 6d65 2066 6169  oid the same fai
-00013c30: 6c75 7265 2e0a 2020 2020 2020 2020 2222  lure..        ""
-00013c40: 220a 2020 2020 2020 2020 646f 5f6e 756d  ".        do_num
-00013c50: 6572 6963 5f74 6573 7428 0a20 2020 2020  eric_test(.     
-00013c60: 2020 2020 2020 2046 6c6f 6174 2870 7265         Float(pre
-00013c70: 6369 7369 6f6e 3d38 2c20 6173 6465 6369  cision=8, asdeci
-00013c80: 6d61 6c3d 5472 7565 292c 0a20 2020 2020  mal=True),.     
-00013c90: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
-00013ca0: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
-00013cb0: 2229 2c20 6465 6369 6d61 6c2e 4465 6369  "), decimal.Deci
-00013cc0: 6d61 6c28 2231 352e 3735 3633 2229 2c20  mal("15.7563"), 
-00013cd0: 4e6f 6e65 5d2c 0a20 2020 2020 2020 2020  None],.         
-00013ce0: 2020 205b 6465 6369 6d61 6c2e 4465 6369     [decimal.Deci
-00013cf0: 6d61 6c28 2231 352e 3735 3633 2229 2c20  mal("15.7563"), 
-00013d00: 4e6f 6e65 5d2c 0a20 2020 2020 2020 2020  None],.         
-00013d10: 2020 2066 696c 7465 725f 3d6c 616d 6264     filter_=lambd
-00013d20: 6120 6e3a 206e 2069 7320 6e6f 7420 4e6f  a n: n is not No
-00013d30: 6e65 2061 6e64 2072 6f75 6e64 286e 2c20  ne and round(n, 
-00013d40: 3429 206f 7220 4e6f 6e65 2c0a 2020 2020  4) or None,.    
-00013d50: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
-00013d60: 6573 745f 666c 6f61 745f 6173 5f66 6c6f  est_float_as_flo
-00013d70: 6174 2873 656c 662c 2064 6f5f 6e75 6d65  at(self, do_nume
-00013d80: 7269 635f 7465 7374 293a 0a20 2020 2020  ric_test):.     
-00013d90: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00013da0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-00013db0: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
-00013dc0: 5370 616e 6e65 7220 7375 7070 6f72 7473  Spanner supports
-00013dd0: 2074 6162 6c65 7320 7769 7468 2061 6e20   tables with an 
-00013de0: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
-00013df0: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
-00013e00: 6e6c 7920 6120 7369 6e67 6c65 2072 6f77  nly a single row
-00013e10: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
-00013e20: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
-00013e30: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
-00013e40: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
-00013e50: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
-00013e60: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
-00013e70: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
-00013e80: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
-00013e90: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
-00013ea0: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
-00013eb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013ec0: 2020 2020 2064 6f5f 6e75 6d65 7269 635f       do_numeric_
-00013ed0: 7465 7374 280a 2020 2020 2020 2020 2020  test(.          
-00013ee0: 2020 466c 6f61 7428 7072 6563 6973 696f    Float(precisio
-00013ef0: 6e3d 3829 2c0a 2020 2020 2020 2020 2020  n=8),.          
-00013f00: 2020 5b64 6563 696d 616c 2e44 6563 696d    [decimal.Decim
-00013f10: 616c 2822 3135 2e37 3536 3322 292c 2064  al("15.7563"), d
-00013f20: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-00013f30: 3135 2e37 3536 3322 295d 2c0a 2020 2020  15.7563")],.    
-00013f40: 2020 2020 2020 2020 5b31 352e 3735 3633          [15.7563
-00013f50: 5d2c 0a20 2020 2020 2020 2020 2020 2066  ],.            f
-00013f60: 696c 7465 725f 3d6c 616d 6264 6120 6e3a  ilter_=lambda n:
-00013f70: 206e 2069 7320 6e6f 7420 4e6f 6e65 2061   n is not None a
-00013f80: 6e64 2072 6f75 6e64 286e 2c20 3529 206f  nd round(n, 5) o
-00013f90: 7220 4e6f 6e65 2c0a 2020 2020 2020 2020  r None,.        
-00013fa0: 290a 0a20 2020 2040 7265 7175 6972 6573  )..    @requires
-00013fb0: 2e70 7265 6369 7369 6f6e 5f6e 756d 6572  .precision_numer
-00013fc0: 6963 735f 6765 6e65 7261 6c0a 2020 2020  ics_general.    
-00013fd0: 6465 6620 7465 7374 5f70 7265 6369 7369  def test_precisi
-00013fe0: 6f6e 5f64 6563 696d 616c 2873 656c 662c  on_decimal(self,
-00013ff0: 2064 6f5f 6e75 6d65 7269 635f 7465 7374   do_numeric_test
-00014000: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00014010: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
-00014020: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
-00014030: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
-00014040: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
-00014050: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
-00014060: 696d 6172 7920 6b65 792c 2062 7574 0a20  imary key, but. 
-00014070: 2020 2020 2020 206f 6e6c 7920 6120 7369         only a si
-00014080: 6e67 6c65 2072 6f77 2063 616e 2062 6520  ngle row can be 
-00014090: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
-000140a0: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
-000140b0: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
-000140c0: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
-000140d0: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
-000140e0: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
-000140f0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
-00014100: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-00014110: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
-00014120: 6661 696c 7572 652e 0a0a 2020 2020 2020  failure...      
-00014130: 2020 5265 6d6f 7665 2061 6e20 6578 7472    Remove an extr
-00014140: 6120 6469 6769 7473 2061 6674 6572 2064  a digits after d
-00014150: 6563 696d 616c 2070 6f69 6e74 2061 7320  ecimal point as 
-00014160: 636c 6f75 6420 7370 616e 6e65 7220 6973  cloud spanner is
-00014170: 0a20 2020 2020 2020 2063 6170 6162 6c65  .        capable
-00014180: 206f 6620 7265 7072 6573 656e 7469 6e67   of representing
-00014190: 2061 6e20 6578 6163 7420 6e75 6d65 7269   an exact numeri
-000141a0: 6320 7661 6c75 6520 7769 7468 2061 2070  c value with a p
-000141b0: 7265 6369 7369 6f6e 0a20 2020 2020 2020  recision.       
-000141c0: 206f 6620 3338 2061 6e64 2073 6361 6c65   of 38 and scale
-000141d0: 206f 6620 392e 0a20 2020 2020 2020 2022   of 9..        "
-000141e0: 2222 0a20 2020 2020 2020 206e 756d 6265  "".        numbe
-000141f0: 7273 203d 2073 6574 280a 2020 2020 2020  rs = set(.      
-00014200: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00014210: 2020 2020 2020 2020 6465 6369 6d61 6c2e          decimal.
-00014220: 4465 6369 6d61 6c28 2235 342e 3234 3634  Decimal("54.2464
-00014230: 3531 3635 3022 292c 0a20 2020 2020 2020  51650"),.       
-00014240: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-00014250: 2e44 6563 696d 616c 2822 302e 3030 3433  .Decimal("0.0043
-00014260: 3534 2229 2c0a 2020 2020 2020 2020 2020  54"),.          
-00014270: 2020 2020 2020 6465 6369 6d61 6c2e 4465        decimal.De
-00014280: 6369 6d61 6c28 2239 3030 2e30 2229 2c0a  cimal("900.0"),.
-00014290: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-000142a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000142b0: 646f 5f6e 756d 6572 6963 5f74 6573 7428  do_numeric_test(
-000142c0: 4e75 6d65 7269 6328 7072 6563 6973 696f  Numeric(precisio
-000142d0: 6e3d 3138 2c20 7363 616c 653d 3929 2c20  n=18, scale=9), 
-000142e0: 6e75 6d62 6572 732c 206e 756d 6265 7273  numbers, numbers
-000142f0: 290a 0a20 2020 2040 7465 7374 696e 672e  )..    @testing.
-00014300: 7265 7175 6972 6573 2e70 7265 6369 7369  requires.precisi
-00014310: 6f6e 5f6e 756d 6572 6963 735f 656e 6f74  on_numerics_enot
-00014320: 6174 696f 6e5f 6c61 7267 650a 2020 2020  ation_large.    
-00014330: 6465 6620 7465 7374 5f65 6e6f 7461 7469  def test_enotati
-00014340: 6f6e 5f64 6563 696d 616c 5f6c 6172 6765  on_decimal_large
-00014350: 2873 656c 662c 2064 6f5f 6e75 6d65 7269  (self, do_numeri
-00014360: 635f 7465 7374 293a 0a20 2020 2020 2020  c_test):.       
-00014370: 2022 2222 7465 7374 2065 7863 6565 6469   """test exceedi
-00014380: 6e67 6c79 206c 6172 6765 2064 6563 696d  ngly large decim
-00014390: 616c 732e 0a0a 2020 2020 2020 2020 5350  als...        SP
-000143a0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-000143b0: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
-000143c0: 7061 6e6e 6572 2073 7570 706f 7274 7320  panner supports 
-000143d0: 7461 626c 6573 2077 6974 6820 616e 2065  tables with an e
-000143e0: 6d70 7479 2070 7269 6d61 7279 206b 6579  mpty primary key
-000143f0: 2c20 6275 740a 2020 2020 2020 2020 6f6e  , but.        on
-00014400: 6c79 2061 2073 696e 676c 6520 726f 7720  ly a single row 
-00014410: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
-00014420: 696e 746f 2073 7563 6820 6120 7461 626c  into such a tabl
-00014430: 6520 2d0a 2020 2020 2020 2020 666f 6c6c  e -.        foll
-00014440: 6f77 696e 6720 696e 7365 7274 696f 6e73  owing insertions
-00014450: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
-00014460: 6052 6f77 205b 5d20 616c 7265 6164 7920  `Row [] already 
-00014470: 6578 6973 7473 222e 0a20 2020 2020 2020  exists"..       
-00014480: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
-00014490: 7465 7374 2074 6f20 6176 6f69 6420 7468  test to avoid th
-000144a0: 6520 7361 6d65 2066 6169 6c75 7265 2e0a  e same failure..
-000144b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000144c0: 2020 2020 6e75 6d62 6572 7320 3d20 7365      numbers = se
-000144d0: 7428 0a20 2020 2020 2020 2020 2020 205b  t(.            [
-000144e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000144f0: 2064 6563 696d 616c 2e44 6563 696d 616c   decimal.Decimal
-00014500: 2822 3445 2b38 2229 2c0a 2020 2020 2020  ("4E+8"),.      
-00014510: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-00014520: 6c2e 4465 6369 6d61 6c28 2235 3734 3845  l.Decimal("5748E
-00014530: 2b31 3522 292c 0a20 2020 2020 2020 2020  +15"),.         
-00014540: 2020 2020 2020 2064 6563 696d 616c 2e44         decimal.D
-00014550: 6563 696d 616c 2822 312e 3532 3145 2b31  ecimal("1.521E+1
-00014560: 3522 292c 0a20 2020 2020 2020 2020 2020  5"),.           
-00014570: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
-00014580: 696d 616c 2822 3030 3030 3030 3030 302e  imal("000000000.
-00014590: 3145 2b39 2229 2c0a 2020 2020 2020 2020  1E+9"),.        
-000145a0: 2020 2020 5d0a 2020 2020 2020 2020 290a      ].        ).
-000145b0: 2020 2020 2020 2020 646f 5f6e 756d 6572          do_numer
-000145c0: 6963 5f74 6573 7428 4e75 6d65 7269 6328  ic_test(Numeric(
-000145d0: 7072 6563 6973 696f 6e3d 3235 2c20 7363  precision=25, sc
-000145e0: 616c 653d 3229 2c20 6e75 6d62 6572 732c  ale=2), numbers,
-000145f0: 206e 756d 6265 7273 290a 0a20 2020 2040   numbers)..    @
-00014600: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
-00014610: 2e70 7265 6369 7369 6f6e 5f6e 756d 6572  .precision_numer
-00014620: 6963 735f 656e 6f74 6174 696f 6e5f 6c61  ics_enotation_la
-00014630: 7267 650a 2020 2020 6465 6620 7465 7374  rge.    def test
-00014640: 5f65 6e6f 7461 7469 6f6e 5f64 6563 696d  _enotation_decim
-00014650: 616c 2873 656c 662c 2064 6f5f 6e75 6d65  al(self, do_nume
-00014660: 7269 635f 7465 7374 293a 0a20 2020 2020  ric_test):.     
-00014670: 2020 2022 2222 7465 7374 2065 7863 6565     """test excee
-00014680: 6469 6e67 6c79 2073 6d61 6c6c 2064 6563  dingly small dec
-00014690: 696d 616c 732e 0a0a 2020 2020 2020 2020  imals...        
-000146a0: 4465 6369 6d61 6c20 7265 706f 7274 7320  Decimal reports 
-000146b0: 7661 6c75 6573 2077 6974 6820 4520 6e6f  values with E no
-000146c0: 7461 7469 6f6e 2077 6865 6e20 7468 6520  tation when the 
-000146d0: 6578 706f 6e65 6e74 0a20 2020 2020 2020  exponent.       
-000146e0: 2069 7320 6772 6561 7465 7220 7468 616e   is greater than
-000146f0: 2036 2e0a 0a20 2020 2020 2020 2053 5041   6...        SPA
-00014700: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-00014710: 2020 2020 2020 2020 5265 6d6f 7665 2065          Remove e
-00014720: 7874 7261 2064 6967 6974 7320 6166 7465  xtra digits afte
-00014730: 7220 6465 6369 6d61 6c20 706f 696e 7420  r decimal point 
-00014740: 6173 2043 6c6f 7564 2053 7061 6e6e 6572  as Cloud Spanner
-00014750: 2069 730a 2020 2020 2020 2020 6361 7061   is.        capa
-00014760: 626c 6520 6f66 2072 6570 7265 7365 6e74  ble of represent
-00014770: 696e 6720 616e 2065 7861 6374 206e 756d  ing an exact num
-00014780: 6572 6963 2076 616c 7565 2077 6974 6820  eric value with 
-00014790: 6120 7072 6563 6973 696f 6e0a 2020 2020  a precision.    
-000147a0: 2020 2020 6f66 2033 3820 616e 6420 7363      of 38 and sc
-000147b0: 616c 6520 6f66 2039 2e0a 2020 2020 2020  ale of 9..      
-000147c0: 2020 2222 220a 2020 2020 2020 2020 6e75    """.        nu
-000147d0: 6d62 6572 7320 3d20 7365 7428 0a20 2020  mbers = set(.   
-000147e0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-000147f0: 2020 2020 2020 2020 2020 2064 6563 696d             decim
-00014800: 616c 2e44 6563 696d 616c 2822 3145 2d32  al.Decimal("1E-2
-00014810: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00014820: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-00014830: 6d61 6c28 2231 452d 3322 292c 0a20 2020  mal("1E-3"),.   
-00014840: 2020 2020 2020 2020 2020 2020 2064 6563               dec
-00014850: 696d 616c 2e44 6563 696d 616c 2822 3145  imal.Decimal("1E
-00014860: 2d34 2229 2c0a 2020 2020 2020 2020 2020  -4"),.          
-00014870: 2020 2020 2020 6465 6369 6d61 6c2e 4465        decimal.De
-00014880: 6369 6d61 6c28 2231 452d 3522 292c 0a20  cimal("1E-5"),. 
-00014890: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000148a0: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-000148b0: 3145 2d36 2229 2c0a 2020 2020 2020 2020  1E-6"),.        
-000148c0: 2020 2020 2020 2020 6465 6369 6d61 6c2e          decimal.
-000148d0: 4465 6369 6d61 6c28 2231 452d 3722 292c  Decimal("1E-7"),
-000148e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000148f0: 2064 6563 696d 616c 2e44 6563 696d 616c   decimal.Decimal
-00014900: 2822 3145 2d38 2229 2c0a 2020 2020 2020  ("1E-8"),.      
-00014910: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-00014920: 6c2e 4465 6369 6d61 6c28 2230 2e31 3035  l.Decimal("0.105
-00014930: 3934 3036 3936 2229 2c0a 2020 2020 2020  940696"),.      
-00014940: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-00014950: 6c2e 4465 6369 6d61 6c28 2230 2e30 3035  l.Decimal("0.005
-00014960: 3934 3036 3936 2229 2c0a 2020 2020 2020  940696"),.      
-00014970: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-00014980: 6c2e 4465 6369 6d61 6c28 2230 2e30 3030  l.Decimal("0.000
-00014990: 3030 3036 3936 2229 2c0a 2020 2020 2020  000696"),.      
-000149a0: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-000149b0: 6c2e 4465 6369 6d61 6c28 2230 2e37 3030  l.Decimal("0.700
-000149c0: 3030 3036 3936 2229 2c0a 2020 2020 2020  000696"),.      
-000149d0: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
-000149e0: 6c2e 4465 6369 6d61 6c28 2236 3936 452d  l.Decimal("696E-
-000149f0: 3922 292c 0a20 2020 2020 2020 2020 2020  9"),.           
-00014a00: 205d 0a20 2020 2020 2020 2029 0a20 2020   ].        ).   
-00014a10: 2020 2020 2064 6f5f 6e75 6d65 7269 635f       do_numeric_
-00014a20: 7465 7374 284e 756d 6572 6963 2870 7265  test(Numeric(pre
-00014a30: 6369 7369 6f6e 3d33 382c 2073 6361 6c65  cision=38, scale
-00014a40: 3d39 292c 206e 756d 6265 7273 2c20 6e75  =9), numbers, nu
-00014a50: 6d62 6572 7329 0a0a 0a63 6c61 7373 204c  mbers)...class L
-00014a60: 696b 6546 756e 6374 696f 6e73 5465 7374  ikeFunctionsTest
-00014a70: 285f 4c69 6b65 4675 6e63 7469 6f6e 7354  (_LikeFunctionsT
-00014a80: 6573 7429 3a0a 2020 2020 4070 7974 6573  est):.    @pytes
-00014a90: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
-00014aa0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-00014ab0: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
-00014ac0: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
-00014ad0: 6620 7465 7374 5f63 6f6e 7461 696e 735f  f test_contains_
-00014ae0: 6175 746f 6573 6361 7065 2873 656c 6629  autoescape(self)
-00014af0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00014b00: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00014b10: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-00014b20: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
-00014b30: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
-00014b40: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
-00014b50: 5f63 6f6e 7461 696e 735f 6175 746f 6573  _contains_autoes
-00014b60: 6361 7065 5f65 7363 6170 6528 7365 6c66  cape_escape(self
-00014b70: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00014b80: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00014b90: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-00014ba0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00014bb0: 4c49 4b45 2045 5343 4150 4520 636c 6175  LIKE ESCAPE clau
-00014bc0: 7365 2229 0a20 2020 2064 6566 2074 6573  se").    def tes
-00014bd0: 745f 636f 6e74 6169 6e73 5f65 7363 6170  t_contains_escap
-00014be0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00014bf0: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-00014c00: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-00014c10: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00014c20: 7070 6f72 7420 4c49 4b45 2045 5343 4150  pport LIKE ESCAP
-00014c30: 4520 636c 6175 7365 2229 0a20 2020 2064  E clause").    d
-00014c40: 6566 2074 6573 745f 656e 6473 7769 7468  ef test_endswith
-00014c50: 5f61 7574 6f65 7363 6170 6528 7365 6c66  _autoescape(self
-00014c60: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00014c70: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00014c80: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-00014c90: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00014ca0: 4c49 4b45 2045 5343 4150 4520 636c 6175  LIKE ESCAPE clau
-00014cb0: 7365 2229 0a20 2020 2064 6566 2074 6573  se").    def tes
-00014cc0: 745f 656e 6473 7769 7468 5f65 7363 6170  t_endswith_escap
-00014cd0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00014ce0: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-00014cf0: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-00014d00: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00014d10: 7070 6f72 7420 4c49 4b45 2045 5343 4150  pport LIKE ESCAP
-00014d20: 4520 636c 6175 7365 2229 0a20 2020 2064  E clause").    d
-00014d30: 6566 2074 6573 745f 656e 6473 7769 7468  ef test_endswith
-00014d40: 5f61 7574 6f65 7363 6170 655f 6573 6361  _autoescape_esca
-00014d50: 7065 2873 656c 6629 3a0a 2020 2020 2020  pe(self):.      
-00014d60: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
-00014d70: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
-00014d80: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
-00014d90: 7570 706f 7274 204c 494b 4520 4553 4341  upport LIKE ESCA
-00014da0: 5045 2063 6c61 7573 6522 290a 2020 2020  PE clause").    
-00014db0: 6465 6620 7465 7374 5f73 7461 7274 7377  def test_startsw
-00014dc0: 6974 685f 6175 746f 6573 6361 7065 2873  ith_autoescape(s
-00014dd0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-00014de0: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-00014df0: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
-00014e00: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
-00014e10: 7274 204c 494b 4520 4553 4341 5045 2063  rt LIKE ESCAPE c
-00014e20: 6c61 7573 6522 290a 2020 2020 6465 6620  lause").    def 
-00014e30: 7465 7374 5f73 7461 7274 7377 6974 685f  test_startswith_
-00014e40: 6573 6361 7065 2873 656c 6629 3a0a 2020  escape(self):.  
-00014e50: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00014e60: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00014e70: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
-00014e80: 2774 2073 7570 706f 7274 204c 494b 4520  't support LIKE 
-00014e90: 4553 4341 5045 2063 6c61 7573 6522 290a  ESCAPE clause").
-00014ea0: 2020 2020 6465 6620 7465 7374 5f73 7461      def test_sta
-00014eb0: 7274 7377 6974 685f 6175 746f 6573 6361  rtswith_autoesca
-00014ec0: 7065 5f65 7363 6170 6528 7365 6c66 293a  pe_escape(self):
-00014ed0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00014ee0: 2020 2064 6566 2074 6573 745f 6573 6361     def test_esca
-00014ef0: 7065 5f6b 6579 776f 7264 5f72 6169 7365  pe_keyword_raise
-00014f00: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00014f10: 2022 2222 4368 6563 6b20 7468 6174 2045   """Check that E
-00014f20: 5343 4150 4520 6b65 7977 6f72 6420 6361  SCAPE keyword ca
-00014f30: 7573 6573 2061 6e20 6578 6365 7074 696f  uses an exceptio
-00014f40: 6e20 7768 656e 2075 7365 642e 2222 220a  n when used.""".
-00014f50: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-00014f60: 6573 742e 7261 6973 6573 284e 6f74 496d  est.raises(NotIm
-00014f70: 706c 656d 656e 7465 6445 7272 6f72 293a  plementedError):
-00014f80: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00014f90: 203d 2073 656c 662e 7461 626c 6573 2e73   = self.tables.s
-00014fa0: 6f6d 655f 7461 626c 652e 632e 6461 7461  ome_table.c.data
-00014fb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014fc0: 662e 5f74 6573 7428 636f 6c2e 636f 6e74  f._test(col.cont
-00014fd0: 6169 6e73 2822 6223 2363 6465 222c 2065  ains("b##cde", e
-00014fe0: 7363 6170 653d 2223 2229 2c20 7b37 7d29  scape="#"), {7})
-00014ff0: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-00015000: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
-00015010: 6573 6e27 7420 7375 7070 6f72 7420 4953  esn't support IS
-00015020: 2044 4953 5449 4e43 5420 4652 4f4d 2063   DISTINCT FROM c
-00015030: 6c61 7573 6522 290a 636c 6173 7320 4973  lause").class Is
-00015040: 4f72 4973 4e6f 7444 6973 7469 6e63 7446  OrIsNotDistinctF
-00015050: 726f 6d54 6573 7428 5f49 734f 7249 734e  romTest(_IsOrIsN
-00015060: 6f74 4469 7374 696e 6374 4672 6f6d 5465  otDistinctFromTe
-00015070: 7374 293a 0a20 2020 2070 6173 730a 0a0a  st):.    pass...
-00015080: 636c 6173 7320 4f72 6465 7242 794c 6162  class OrderByLab
-00015090: 656c 5465 7374 285f 4f72 6465 7242 794c  elTest(_OrderByL
-000150a0: 6162 656c 5465 7374 293a 0a20 2020 2040  abelTest):.    @
-000150b0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-000150c0: 280a 2020 2020 2020 2020 2253 7061 6e6e  (.        "Spann
-000150d0: 6572 2072 6571 7569 7265 7320 616e 2061  er requires an a
-000150e0: 6c69 6173 2066 6f72 2074 6865 2047 524f  lias for the GRO
-000150f0: 5550 2042 5920 6c69 7374 2077 6865 6e20  UP BY list when 
-00015100: 7370 6563 6966 7969 6e67 2064 6572 6976  specifying deriv
-00015110: 6564 2022 0a20 2020 2020 2020 2022 636f  ed ".        "co
-00015120: 6c75 6d6e 7320 616c 736f 2075 7365 6420  lumns also used 
-00015130: 696e 2053 454c 4543 5422 0a20 2020 2029  in SELECT".    )
-00015140: 0a20 2020 2064 6566 2074 6573 745f 6772  .    def test_gr
-00015150: 6f75 705f 6279 5f63 6f6d 706f 7365 6428  oup_by_composed(
-00015160: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00015170: 6173 730a 0a0a 636c 6173 7320 436f 6d70  ass...class Comp
-00015180: 6f75 6e64 5365 6c65 6374 5465 7374 285f  oundSelectTest(_
-00015190: 436f 6d70 6f75 6e64 5365 6c65 6374 5465  CompoundSelectTe
-000151a0: 7374 293a 0a20 2020 2022 2222 0a20 2020  st):.    """.   
-000151b0: 2053 6565 3a20 6874 7470 733a 2f2f 6769   See: https://gi
-000151c0: 7468 7562 2e63 6f6d 2f67 6f6f 676c 6561  thub.com/googlea
-000151d0: 7069 732f 7079 7468 6f6e 2d73 7061 6e6e  pis/python-spann
-000151e0: 6572 2f69 7373 7565 732f 3334 370a 2020  er/issues/347.  
-000151f0: 2020 2222 220a 0a20 2020 2040 7079 7465    """..    @pyte
-00015200: 7374 2e6d 6172 6b2e 736b 6970 280a 2020  st.mark.skip(.  
-00015210: 2020 2020 2020 2253 7061 6e6e 6572 2044        "Spanner D
-00015220: 4241 5049 2069 6e63 6f72 7265 6374 6c79  BAPI incorrectly
-00015230: 2063 6c61 7373 6966 7920 7468 6520 7374   classify the st
-00015240: 6174 656d 656e 7420 7374 6172 7469 6e67  atement starting
-00015250: 2077 6974 6820 6272 6163 6b65 7473 2e22   with brackets."
-00015260: 0a20 2020 2029 0a20 2020 2064 6566 2074  .    ).    def t
-00015270: 6573 745f 6c69 6d69 745f 6f66 6673 6574  est_limit_offset
-00015280: 5f73 656c 6563 7461 626c 655f 696e 5f75  _selectable_in_u
-00015290: 6e69 6f6e 7328 7365 6c66 293a 0a20 2020  nions(self):.   
-000152a0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-000152b0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-000152c0: 280a 2020 2020 2020 2020 2253 7061 6e6e  (.        "Spann
-000152d0: 6572 2044 4241 5049 2069 6e63 6f72 7265  er DBAPI incorre
-000152e0: 6374 6c79 2063 6c61 7373 6966 7920 7468  ctly classify th
-000152f0: 6520 7374 6174 656d 656e 7420 7374 6172  e statement star
-00015300: 7469 6e67 2077 6974 6820 6272 6163 6b65  ting with bracke
-00015310: 7473 2e22 0a20 2020 2029 0a20 2020 2064  ts.".    ).    d
-00015320: 6566 2074 6573 745f 6f72 6465 725f 6279  ef test_order_by
-00015330: 5f73 656c 6563 7461 626c 655f 696e 5f75  _selectable_in_u
-00015340: 6e69 6f6e 7328 7365 6c66 293a 0a20 2020  nions(self):.   
-00015350: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
-00015360: 7320 5465 7374 5175 6572 7948 696e 7473  s TestQueryHints
-00015370: 2866 6978 7475 7265 732e 5461 626c 6573  (fixtures.Tables
-00015380: 5465 7374 293a 0a20 2020 2022 2222 0a20  Test):.    """. 
-00015390: 2020 2043 6f6d 7069 6c65 2061 2063 6f6d     Compile a com
-000153a0: 706c 6578 2071 7565 7279 2077 6974 6820  plex query with 
-000153b0: 4a4f 494e 2061 6e64 2063 6865 636b 2074  JOIN and check t
-000153c0: 6861 740a 2020 2020 7468 6520 7461 626c  hat.    the tabl
-000153d0: 6520 6869 6e74 2077 6173 2073 6574 2069  e hint was set i
-000153e0: 6e74 6f20 7468 6520 7269 6768 7420 706c  nto the right pl
-000153f0: 6163 652e 0a20 2020 2022 2222 0a0a 2020  ace..    """..  
-00015400: 2020 5f5f 6261 636b 656e 645f 5f20 3d20    __backend__ = 
-00015410: 5472 7565 0a0a 2020 2020 6465 6620 7465  True..    def te
-00015420: 7374 5f63 6f6d 706c 6578 5f71 7565 7279  st_complex_query
-00015430: 5f74 6162 6c65 5f68 696e 7473 2873 656c  _table_hints(sel
-00015440: 6629 3a0a 2020 2020 2020 2020 4558 5045  f):.        EXPE
-00015450: 4354 4544 5f51 5545 5259 203d 2028 0a20  CTED_QUERY = (. 
-00015460: 2020 2020 2020 2020 2020 2022 5345 4c45             "SELE
-00015470: 4354 2075 7365 7273 2e69 642c 2075 7365  CT users.id, use
-00015480: 7273 2e6e 616d 6520 5c6e 4652 4f4d 2075  rs.name \nFROM u
-00015490: 7365 7273 2040 7b46 4f52 4345 5f49 4e44  sers @{FORCE_IND
-000154a0: 4558 3d74 6162 6c65 5f31 5f62 795f 696e  EX=table_1_by_in
-000154b0: 745f 6964 787d 220a 2020 2020 2020 2020  t_idx}".        
-000154c0: 2020 2020 2220 4a4f 494e 2061 6464 7265      " JOIN addre
-000154d0: 7373 6573 204f 4e20 7573 6572 732e 6964  sses ON users.id
-000154e0: 203d 2061 6464 7265 7373 6573 2e75 7365   = addresses.use
-000154f0: 725f 6964 2022 0a20 2020 2020 2020 2020  r_id ".         
-00015500: 2020 2022 5c6e 5748 4552 4520 7573 6572     "\nWHERE user
-00015510: 732e 6e61 6d65 2049 4e20 285f 5f5b 504f  s.name IN (__[PO
-00015520: 5354 434f 4d50 494c 455f 6e61 6d65 5f31  STCOMPILE_name_1
-00015530: 5d29 220a 2020 2020 2020 2020 290a 0a20  ])".        ).. 
-00015540: 2020 2020 2020 2042 6173 6520 3d20 6465         Base = de
-00015550: 636c 6172 6174 6976 655f 6261 7365 2829  clarative_base()
-00015560: 0a20 2020 2020 2020 2065 6e67 696e 6520  .        engine 
-00015570: 3d20 6372 6561 7465 5f65 6e67 696e 6528  = create_engine(
-00015580: 0a20 2020 2020 2020 2020 2020 2022 7370  .            "sp
-00015590: 616e 6e65 723a 2f2f 2f70 726f 6a65 6374  anner:///project
-000155a0: 732f 7072 6f6a 6563 742d 6964 2f69 6e73  s/project-id/ins
-000155b0: 7461 6e63 6573 2f69 6e73 7461 6e63 652d  tances/instance-
-000155c0: 6964 2f64 6174 6162 6173 6573 2f64 6174  id/databases/dat
-000155d0: 6162 6173 652d 6964 220a 2020 2020 2020  abase-id".      
-000155e0: 2020 290a 0a20 2020 2020 2020 2063 6c61    )..        cla
-000155f0: 7373 2055 7365 7228 4261 7365 293a 0a20  ss User(Base):. 
-00015600: 2020 2020 2020 2020 2020 205f 5f74 6162             __tab
-00015610: 6c65 6e61 6d65 5f5f 203d 2022 7573 6572  lename__ = "user
-00015620: 7322 0a20 2020 2020 2020 2020 2020 2069  s".            i
-00015630: 6420 3d20 436f 6c75 6d6e 2849 6e74 6567  d = Column(Integ
-00015640: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
-00015650: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00015660: 2020 6e61 6d65 203d 2043 6f6c 756d 6e28    name = Column(
-00015670: 5374 7269 6e67 2835 3029 290a 2020 2020  String(50)).    
-00015680: 2020 2020 2020 2020 6164 6472 6573 7365          addresse
-00015690: 7320 3d20 7265 6c61 7469 6f6e 7368 6970  s = relationship
-000156a0: 2822 4164 6472 6573 7322 2c20 6261 636b  ("Address", back
-000156b0: 7265 663d 2275 7365 7222 290a 0a20 2020  ref="user")..   
-000156c0: 2020 2020 2063 6c61 7373 2041 6464 7265       class Addre
-000156d0: 7373 2842 6173 6529 3a0a 2020 2020 2020  ss(Base):.      
-000156e0: 2020 2020 2020 5f5f 7461 626c 656e 616d        __tablenam
-000156f0: 655f 5f20 3d20 2261 6464 7265 7373 6573  e__ = "addresses
-00015700: 220a 2020 2020 2020 2020 2020 2020 6964  ".            id
-00015710: 203d 2043 6f6c 756d 6e28 496e 7465 6765   = Column(Intege
-00015720: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-00015730: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00015740: 2065 6d61 696c 203d 2043 6f6c 756d 6e28   email = Column(
-00015750: 5374 7269 6e67 2835 3029 290a 2020 2020  String(50)).    
-00015760: 2020 2020 2020 2020 7573 6572 5f69 6420          user_id 
-00015770: 3d20 436f 6c75 6d6e 2849 6e74 6567 6572  = Column(Integer
-00015780: 2c20 466f 7265 6967 6e4b 6579 2822 7573  , ForeignKey("us
-00015790: 6572 732e 6964 2229 290a 0a20 2020 2020  ers.id"))..     
-000157a0: 2020 2073 6573 7369 6f6e 203d 2053 6573     session = Ses
-000157b0: 7369 6f6e 2865 6e67 696e 6529 0a0a 2020  sion(engine)..  
-000157c0: 2020 2020 2020 7175 6572 7920 3d20 7365        query = se
-000157d0: 7373 696f 6e2e 7175 6572 7928 5573 6572  ssion.query(User
-000157e0: 290a 2020 2020 2020 2020 7175 6572 7920  ).        query 
-000157f0: 3d20 7175 6572 792e 7769 7468 5f68 696e  = query.with_hin
-00015800: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
-00015810: 656c 6563 7461 626c 653d 5573 6572 2c20  electable=User, 
-00015820: 7465 7874 3d22 407b 464f 5243 455f 494e  text="@{FORCE_IN
-00015830: 4445 583d 7461 626c 655f 315f 6279 5f69  DEX=table_1_by_i
-00015840: 6e74 5f69 6478 7d22 0a20 2020 2020 2020  nt_idx}".       
-00015850: 2029 0a0a 2020 2020 2020 2020 7175 6572   )..        quer
-00015860: 7920 3d20 7175 6572 792e 6669 6c74 6572  y = query.filter
-00015870: 2855 7365 722e 6e61 6d65 2e69 6e5f 285b  (User.name.in_([
-00015880: 2276 616c 3122 2c20 2276 616c 3222 5d29  "val1", "val2"])
-00015890: 290a 2020 2020 2020 2020 7175 6572 7920  ).        query 
-000158a0: 3d20 7175 6572 792e 6a6f 696e 2841 6464  = query.join(Add
-000158b0: 7265 7373 290a 0a20 2020 2020 2020 2061  ress)..        a
-000158c0: 7373 6572 7420 7374 7228 7175 6572 792e  ssert str(query.
-000158d0: 7374 6174 656d 656e 742e 636f 6d70 696c  statement.compil
-000158e0: 6528 7365 7373 696f 6e2e 6269 6e64 2929  e(session.bind))
-000158f0: 203d 3d20 4558 5045 4354 4544 5f51 5545   == EXPECTED_QUE
-00015900: 5259 0a0a 0a63 6c61 7373 2049 6e74 6572  RY...class Inter
-00015910: 6c65 6176 6564 5461 626c 6573 5465 7374  leavedTablesTest
-00015920: 2866 6978 7475 7265 732e 5465 7374 4261  (fixtures.TestBa
-00015930: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
-00015940: 2043 6865 636b 2074 6861 7420 4352 4541   Check that CREA
-00015950: 5445 2054 4142 4c45 2073 7461 7465 6d65  TE TABLE stateme
-00015960: 6e74 7320 666f 7220 696e 7465 726c 6561  nts for interlea
-00015970: 7665 6420 7461 626c 6573 2061 7265 2063  ved tables are c
-00015980: 6f72 7265 6374 6c79 0a20 2020 2067 656e  orrectly.    gen
-00015990: 6572 6174 6564 2e0a 2020 2020 2222 220a  erated..    """.
-000159a0: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
-000159b0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-000159c0: 6c66 2e5f 656e 6769 6e65 203d 2063 7265  lf._engine = cre
-000159d0: 6174 655f 656e 6769 6e65 280a 2020 2020  ate_engine(.    
-000159e0: 2020 2020 2020 2020 2273 7061 6e6e 6572          "spanner
-000159f0: 3a2f 2f2f 7072 6f6a 6563 7473 2f61 7070  :///projects/app
-00015a00: 6465 762d 736f 6461 2d73 7061 6e6e 6572  dev-soda-spanner
-00015a10: 2d73 7461 6769 6e67 2f69 6e73 7461 6e63  -staging/instanc
-00015a20: 6573 2f22 0a20 2020 2020 2020 2020 2020  es/".           
-00015a30: 2022 7371 6c61 6c63 6865 6d79 2d64 6961   "sqlalchemy-dia
-00015a40: 6c65 6374 2d74 6573 742f 6461 7461 6261  lect-test/databa
-00015a50: 7365 732f 636f 6d70 6c69 616e 6365 2d74  ses/compliance-t
-00015a60: 6573 7422 0a20 2020 2020 2020 2029 0a20  est".        ). 
-00015a70: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
-00015a80: 6164 6174 6120 3d20 4d65 7461 4461 7461  adata = MetaData
-00015a90: 2829 0a0a 2020 2020 6465 6620 7465 7374  ()..    def test
-00015aa0: 5f69 6e74 6572 6c65 6176 6528 7365 6c66  _interleave(self
-00015ab0: 293a 0a20 2020 2020 2020 2045 5850 5f51  ):.        EXP_Q
-00015ac0: 5545 5259 203d 2028 0a20 2020 2020 2020  UERY = (.       
-00015ad0: 2020 2020 2022 5c6e 4352 4541 5445 2054       "\nCREATE T
-00015ae0: 4142 4c45 2063 6c69 656e 7420 285c 6e5c  ABLE client (\n\
-00015af0: 7474 6561 6d5f 6964 2049 4e54 3634 204e  tteam_id INT64 N
-00015b00: 4f54 204e 554c 4c2c 2022 0a20 2020 2020  OT NULL, ".     
-00015b10: 2020 2020 2020 2022 5c6e 5c74 636c 6965         "\n\tclie
-00015b20: 6e74 5f69 6420 494e 5436 3420 4e4f 5420  nt_id INT64 NOT 
-00015b30: 4e55 4c4c 2c20 220a 2020 2020 2020 2020  NULL, ".        
-00015b40: 2020 2020 225c 6e5c 7463 6c69 656e 745f      "\n\tclient_
-00015b50: 6e61 6d65 2053 5452 494e 4728 3136 2920  name STRING(16) 
-00015b60: 4e4f 5420 4e55 4c4c 220a 2020 2020 2020  NOT NULL".      
-00015b70: 2020 2020 2020 225c 6e29 2050 5249 4d41        "\n) PRIMA
-00015b80: 5259 204b 4559 2028 7465 616d 5f69 642c  RY KEY (team_id,
-00015b90: 2063 6c69 656e 745f 6964 292c 220a 2020   client_id),".  
-00015ba0: 2020 2020 2020 2020 2020 225c 6e49 4e54            "\nINT
-00015bb0: 4552 4c45 4156 4520 494e 2050 4152 454e  ERLEAVE IN PAREN
-00015bc0: 5420 7465 616d 5c6e 5c6e 220a 2020 2020  T team\n\n".    
-00015bd0: 2020 2020 290a 2020 2020 2020 2020 636c      ).        cl
-00015be0: 6965 6e74 203d 2054 6162 6c65 280a 2020  ient = Table(.  
-00015bf0: 2020 2020 2020 2020 2020 2263 6c69 656e            "clien
-00015c00: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00015c10: 7365 6c66 2e5f 6d65 7461 6461 7461 2c0a  self._metadata,.
-00015c20: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-00015c30: 6d6e 2822 7465 616d 5f69 6422 2c20 496e  mn("team_id", In
-00015c40: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
-00015c50: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
-00015c60: 2020 2020 2020 436f 6c75 6d6e 2822 636c        Column("cl
-00015c70: 6965 6e74 5f69 6422 2c20 496e 7465 6765  ient_id", Intege
-00015c80: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-00015c90: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-00015ca0: 2020 436f 6c75 6d6e 2822 636c 6965 6e74    Column("client
-00015cb0: 5f6e 616d 6522 2c20 5374 7269 6e67 2831  _name", String(1
-00015cc0: 3629 2c20 6e75 6c6c 6162 6c65 3d46 616c  6), nullable=Fal
-00015cd0: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
-00015ce0: 2073 7061 6e6e 6572 5f69 6e74 6572 6c65   spanner_interle
-00015cf0: 6176 655f 696e 3d22 7465 616d 222c 0a20  ave_in="team",. 
-00015d00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00015d10: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
-00015d20: 2822 676f 6f67 6c65 2e63 6c6f 7564 2e73  ("google.cloud.s
-00015d30: 7061 6e6e 6572 5f64 6261 7069 2e63 7572  panner_dbapi.cur
-00015d40: 736f 722e 4375 7273 6f72 2e65 7865 6375  sor.Cursor.execu
-00015d50: 7465 2229 2061 7320 6578 6563 7574 653a  te") as execute:
-00015d60: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00015d70: 656e 742e 6372 6561 7465 2873 656c 662e  ent.create(self.
-00015d80: 5f65 6e67 696e 6529 0a20 2020 2020 2020  _engine).       
-00015d90: 2020 2020 2065 7865 6375 7465 2e61 7373       execute.ass
-00015da0: 6572 745f 6361 6c6c 6564 5f6f 6e63 655f  ert_called_once_
-00015db0: 7769 7468 2845 5850 5f51 5545 5259 2c20  with(EXP_QUERY, 
-00015dc0: 5b5d 290a 0a20 2020 2064 6566 2074 6573  [])..    def tes
-00015dd0: 745f 696e 7465 726c 6561 7665 5f6f 6e5f  t_interleave_on_
-00015de0: 6465 6c65 7465 5f63 6173 6361 6465 2873  delete_cascade(s
-00015df0: 656c 6629 3a0a 2020 2020 2020 2020 4558  elf):.        EX
-00015e00: 505f 5155 4552 5920 3d20 280a 2020 2020  P_QUERY = (.    
-00015e10: 2020 2020 2020 2020 225c 6e43 5245 4154          "\nCREAT
-00015e20: 4520 5441 424c 4520 636c 6965 6e74 2028  E TABLE client (
-00015e30: 5c6e 5c74 7465 616d 5f69 6420 494e 5436  \n\tteam_id INT6
-00015e40: 3420 4e4f 5420 4e55 4c4c 2c20 220a 2020  4 NOT NULL, ".  
-00015e50: 2020 2020 2020 2020 2020 225c 6e5c 7463            "\n\tc
-00015e60: 6c69 656e 745f 6964 2049 4e54 3634 204e  lient_id INT64 N
-00015e70: 4f54 204e 554c 4c2c 2022 0a20 2020 2020  OT NULL, ".     
-00015e80: 2020 2020 2020 2022 5c6e 5c74 636c 6965         "\n\tclie
-00015e90: 6e74 5f6e 616d 6520 5354 5249 4e47 2831  nt_name STRING(1
-00015ea0: 3629 204e 4f54 204e 554c 4c22 0a20 2020  6) NOT NULL".   
-00015eb0: 2020 2020 2020 2020 2022 5c6e 2920 5052           "\n) PR
-00015ec0: 494d 4152 5920 4b45 5920 2874 6561 6d5f  IMARY KEY (team_
-00015ed0: 6964 2c20 636c 6965 6e74 5f69 6429 2c22  id, client_id),"
-00015ee0: 0a20 2020 2020 2020 2020 2020 2022 5c6e  .            "\n
-00015ef0: 494e 5445 524c 4541 5645 2049 4e20 5041  INTERLEAVE IN PA
-00015f00: 5245 4e54 2074 6561 6d20 4f4e 2044 454c  RENT team ON DEL
-00015f10: 4554 4520 4341 5343 4144 455c 6e5c 6e22  ETE CASCADE\n\n"
-00015f20: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00015f30: 2020 2063 6c69 656e 7420 3d20 5461 626c     client = Tabl
-00015f40: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00015f50: 636c 6965 6e74 222c 0a20 2020 2020 2020  client",.       
-00015f60: 2020 2020 2073 656c 662e 5f6d 6574 6164       self._metad
-00015f70: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00015f80: 2043 6f6c 756d 6e28 2274 6561 6d5f 6964   Column("team_id
-00015f90: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
-00015fa0: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
-00015fb0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00015fc0: 6e28 2263 6c69 656e 745f 6964 222c 2049  n("client_id", I
-00015fd0: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-00015fe0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
-00015ff0: 2020 2020 2020 2043 6f6c 756d 6e28 2263         Column("c
-00016000: 6c69 656e 745f 6e61 6d65 222c 2053 7472  lient_name", Str
-00016010: 696e 6728 3136 292c 206e 756c 6c61 626c  ing(16), nullabl
-00016020: 653d 4661 6c73 6529 2c0a 2020 2020 2020  e=False),.      
-00016030: 2020 2020 2020 7370 616e 6e65 725f 696e        spanner_in
-00016040: 7465 726c 6561 7665 5f69 6e3d 2274 6561  terleave_in="tea
-00016050: 6d22 2c0a 2020 2020 2020 2020 2020 2020  m",.            
-00016060: 7370 616e 6e65 725f 696e 7465 726c 6561  spanner_interlea
-00016070: 7665 5f6f 6e5f 6465 6c65 7465 5f63 6173  ve_on_delete_cas
-00016080: 6361 6465 3d54 7275 652c 0a20 2020 2020  cade=True,.     
-00016090: 2020 2029 0a20 2020 2020 2020 2077 6974     ).        wit
-000160a0: 6820 6d6f 636b 2e70 6174 6368 2822 676f  h mock.patch("go
-000160b0: 6f67 6c65 2e63 6c6f 7564 2e73 7061 6e6e  ogle.cloud.spann
-000160c0: 6572 5f64 6261 7069 2e63 7572 736f 722e  er_dbapi.cursor.
-000160d0: 4375 7273 6f72 2e65 7865 6375 7465 2229  Cursor.execute")
-000160e0: 2061 7320 6578 6563 7574 653a 0a20 2020   as execute:.   
-000160f0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-00016100: 6372 6561 7465 2873 656c 662e 5f65 6e67  create(self._eng
-00016110: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
-00016120: 2065 7865 6375 7465 2e61 7373 6572 745f   execute.assert_
-00016130: 6361 6c6c 6564 5f6f 6e63 655f 7769 7468  called_once_with
-00016140: 2845 5850 5f51 5545 5259 2c20 5b5d 290a  (EXP_QUERY, []).
-00016150: 0a0a 636c 6173 7320 5573 6572 4167 656e  ..class UserAgen
-00016160: 7454 6573 7428 6669 7874 7572 6573 2e54  tTest(fixtures.T
-00016170: 6573 7442 6173 6529 3a0a 2020 2020 2222  estBase):.    ""
-00016180: 2243 6865 636b 2074 6861 7420 5351 4c41  "Check that SQLA
-00016190: 6c63 6865 6d79 2064 6961 6c65 6374 2075  lchemy dialect u
-000161a0: 7365 7320 636f 7272 6563 7420 7573 6572  ses correct user
-000161b0: 2061 6765 6e74 2e22 2222 0a0a 2020 2020   agent."""..    
-000161c0: 6465 6620 7365 7455 7028 7365 6c66 293a  def setUp(self):
-000161d0: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-000161e0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
-000161f0: 6e67 696e 6528 0a20 2020 2020 2020 2020  ngine(.         
-00016200: 2020 2022 7370 616e 6e65 723a 2f2f 2f70     "spanner:///p
-00016210: 726f 6a65 6374 732f 6170 7064 6576 2d73  rojects/appdev-s
-00016220: 6f64 612d 7370 616e 6e65 722d 7374 6167  oda-spanner-stag
-00016230: 696e 672f 696e 7374 616e 6365 732f 220a  ing/instances/".
-00016240: 2020 2020 2020 2020 2020 2020 2273 716c              "sql
-00016250: 616c 6368 656d 792d 6469 616c 6563 742d  alchemy-dialect-
-00016260: 7465 7374 2f64 6174 6162 6173 6573 2f63  test/databases/c
-00016270: 6f6d 706c 6961 6e63 652d 7465 7374 220a  ompliance-test".
-00016280: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00016290: 2020 7365 6c66 2e5f 6d65 7461 6461 7461    self._metadata
-000162a0: 203d 204d 6574 6144 6174 6128 290a 0a20   = MetaData().. 
-000162b0: 2020 2064 6566 2074 6573 745f 7573 6572     def test_user
-000162c0: 5f61 6765 6e74 2873 656c 6629 3a0a 2020  _agent(self):.  
-000162d0: 2020 2020 2020 6469 7374 203d 2070 6b67        dist = pkg
-000162e0: 5f72 6573 6f75 7263 6573 2e67 6574 5f64  _resources.get_d
-000162f0: 6973 7472 6962 7574 696f 6e28 2273 716c  istribution("sql
-00016300: 616c 6368 656d 792d 7370 616e 6e65 7222  alchemy-spanner"
-00016310: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00016320: 7365 6c66 2e5f 656e 6769 6e65 2e63 6f6e  self._engine.con
-00016330: 6e65 6374 2829 2061 7320 636f 6e6e 6563  nect() as connec
-00016340: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00016350: 2020 6173 7365 7274 2028 0a20 2020 2020    assert (.     
-00016360: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-00016370: 6374 696f 6e2e 636f 6e6e 6563 7469 6f6e  ction.connection
-00016380: 2e69 6e73 7461 6e63 652e 5f63 6c69 656e  .instance._clien
-00016390: 742e 5f63 6c69 656e 745f 696e 666f 2e75  t._client_info.u
-000163a0: 7365 725f 6167 656e 740a 2020 2020 2020  ser_agent.      
-000163b0: 2020 2020 2020 2020 2020 3d3d 2022 676c            == "gl
-000163c0: 2d22 202b 2064 6973 742e 7072 6f6a 6563  -" + dist.projec
-000163d0: 745f 6e61 6d65 202b 2022 2f22 202b 2064  t_name + "/" + d
-000163e0: 6973 742e 7665 7273 696f 6e0a 2020 2020  ist.version.    
-000163f0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-00016400: 7320 5369 6d70 6c65 5570 6461 7465 4465  s SimpleUpdateDe
-00016410: 6c65 7465 5465 7374 285f 5369 6d70 6c65  leteTest(_Simple
-00016420: 5570 6461 7465 4465 6c65 7465 5465 7374  UpdateDeleteTest
-00016430: 293a 0a20 2020 2022 2222 0a20 2020 2053  ):.    """.    S
-00016440: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-00016450: 0a0a 2020 2020 5370 616e 6e65 7220 646f  ..    Spanner do
-00016460: 6573 6e27 7420 7375 7070 6f72 7420 6072  esn't support `r
-00016470: 6f77 636f 756e 7460 2070 726f 7065 7274  owcount` propert
-00016480: 792e 2054 6865 7365 0a20 2020 2074 6573  y. These.    tes
-00016490: 7420 6361 7365 7320 6f76 6572 7269 6465  t cases override
-000164a0: 7320 6f6d 6974 2060 726f 7763 6f75 6e74  s omit `rowcount
-000164b0: 6020 6368 6563 6b73 2e0a 2020 2020 2222  ` checks..    ""
-000164c0: 220a 0a20 2020 2064 6566 2074 6573 745f  "..    def test_
-000164d0: 6465 6c65 7465 2873 656c 662c 2063 6f6e  delete(self, con
-000164e0: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-000164f0: 2020 7420 3d20 7365 6c66 2e74 6162 6c65    t = self.table
-00016500: 732e 706c 6169 6e5f 706b 0a20 2020 2020  s.plain_pk.     
-00016510: 2020 2072 203d 2063 6f6e 6e65 6374 696f     r = connectio
-00016520: 6e2e 6578 6563 7574 6528 742e 6465 6c65  n.execute(t.dele
-00016530: 7465 2829 2e77 6865 7265 2874 2e63 2e69  te().where(t.c.i
-00016540: 6420 3d3d 2032 2929 0a20 2020 2020 2020  d == 2)).       
-00016550: 2061 7373 6572 7420 6e6f 7420 722e 6973   assert not r.is
-00016560: 5f69 6e73 6572 740a 2020 2020 2020 2020  _insert.        
-00016570: 6173 7365 7274 206e 6f74 2072 2e72 6574  assert not r.ret
-00016580: 7572 6e73 5f72 6f77 730a 2020 2020 2020  urns_rows.      
-00016590: 2020 6571 5f28 0a20 2020 2020 2020 2020    eq_(.         
-000165a0: 2020 2063 6f6e 6e65 6374 696f 6e2e 6578     connection.ex
-000165b0: 6563 7574 6528 742e 7365 6c65 6374 2829  ecute(t.select()
-000165c0: 2e6f 7264 6572 5f62 7928 742e 632e 6964  .order_by(t.c.id
-000165d0: 2929 2e66 6574 6368 616c 6c28 292c 0a20  )).fetchall(),. 
-000165e0: 2020 2020 2020 2020 2020 205b 2831 2c20             [(1, 
-000165f0: 2264 3122 292c 2028 332c 2022 6433 2229  "d1"), (3, "d3")
-00016600: 5d2c 0a20 2020 2020 2020 2029 0a0a 2020  ],.        )..  
-00016610: 2020 6465 6620 7465 7374 5f75 7064 6174    def test_updat
-00016620: 6528 7365 6c66 2c20 636f 6e6e 6563 7469  e(self, connecti
-00016630: 6f6e 293a 0a20 2020 2020 2020 2074 203d  on):.        t =
-00016640: 2073 656c 662e 7461 626c 6573 2e70 6c61   self.tables.pla
-00016650: 696e 5f70 6b0a 2020 2020 2020 2020 7220  in_pk.        r 
-00016660: 3d20 636f 6e6e 6563 7469 6f6e 2e65 7865  = connection.exe
-00016670: 6375 7465 2874 2e75 7064 6174 6528 292e  cute(t.update().
-00016680: 7768 6572 6528 742e 632e 6964 203d 3d20  where(t.c.id == 
-00016690: 3229 2c20 6469 6374 2864 6174 613d 2264  2), dict(data="d
-000166a0: 325f 6e65 7722 2929 0a20 2020 2020 2020  2_new")).       
-000166b0: 2061 7373 6572 7420 6e6f 7420 722e 6973   assert not r.is
-000166c0: 5f69 6e73 6572 740a 2020 2020 2020 2020  _insert.        
-000166d0: 6173 7365 7274 206e 6f74 2072 2e72 6574  assert not r.ret
-000166e0: 7572 6e73 5f72 6f77 730a 0a20 2020 2020  urns_rows..     
-000166f0: 2020 2065 715f 280a 2020 2020 2020 2020     eq_(.        
-00016700: 2020 2020 636f 6e6e 6563 7469 6f6e 2e65      connection.e
-00016710: 7865 6375 7465 2874 2e73 656c 6563 7428  xecute(t.select(
-00016720: 292e 6f72 6465 725f 6279 2874 2e63 2e69  ).order_by(t.c.i
-00016730: 6429 292e 6665 7463 6861 6c6c 2829 2c0a  d)).fetchall(),.
-00016740: 2020 2020 2020 2020 2020 2020 5b28 312c              [(1,
-00016750: 2022 6431 2229 2c20 2832 2c20 2264 325f   "d1"), (2, "d2_
-00016760: 6e65 7722 292c 2028 332c 2022 6433 2229  new"), (3, "d3")
-00016770: 5d2c 0a20 2020 2020 2020 2029 0a0a 0a63  ],.        )...c
-00016780: 6c61 7373 2048 6173 496e 6465 7854 6573  lass HasIndexTes
-00016790: 7428 5f48 6173 496e 6465 7854 6573 7429  t(_HasIndexTest)
-000167a0: 3a0a 2020 2020 5f5f 6261 636b 656e 645f  :.    __backend_
-000167b0: 5f20 3d20 5472 7565 0a20 2020 206b 696e  _ = True.    kin
-000167c0: 6420 3d20 7465 7374 696e 672e 636f 6d62  d = testing.comb
-000167d0: 696e 6174 696f 6e73 2822 6469 616c 6563  inations("dialec
-000167e0: 7422 2c20 2269 6e73 7065 6374 6f72 222c  t", "inspector",
-000167f0: 2061 7267 6e61 6d65 733d 226b 696e 6422   argnames="kind"
-00016800: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-00016810: 686f 640a 2020 2020 6465 6620 6465 6669  hod.    def defi
-00016820: 6e65 5f74 6162 6c65 7328 636c 732c 206d  ne_tables(cls, m
-00016830: 6574 6164 6174 6129 3a0a 2020 2020 2020  etadata):.      
-00016840: 2020 7474 203d 2054 6162 6c65 280a 2020    tt = Table(.  
-00016850: 2020 2020 2020 2020 2020 2274 6573 745f            "test_
-00016860: 7461 626c 6522 2c0a 2020 2020 2020 2020  table",.        
-00016870: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00016880: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00016890: 2822 6964 222c 2049 6e74 6567 6572 2c20  ("id", Integer, 
-000168a0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-000168b0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-000168c0: 6f6c 756d 6e28 2264 6174 6122 2c20 5374  olumn("data", St
-000168d0: 7269 6e67 2835 3029 292c 0a20 2020 2020  ring(50)),.     
-000168e0: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
-000168f0: 6174 6132 222c 2053 7472 696e 6728 3530  ata2", String(50
-00016900: 2929 2c0a 2020 2020 2020 2020 290a 2020  )),.        ).  
-00016910: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-00016920: 2e49 6e64 6578 2822 6d79 5f69 6478 222c  .Index("my_idx",
-00016930: 2074 742e 632e 6461 7461 290a 0a20 2020   tt.c.data)..   
-00016940: 2040 6b69 6e64 0a20 2020 2064 6566 2074   @kind.    def t
-00016950: 6573 745f 6861 735f 696e 6465 7828 7365  est_has_index(se
-00016960: 6c66 2c20 6b69 6e64 2c20 636f 6e6e 6563  lf, kind, connec
-00016970: 7469 6f6e 2c20 6d65 7461 6461 7461 293a  tion, metadata):
-00016980: 0a20 2020 2020 2020 206d 6574 6820 3d20  .        meth = 
-00016990: 7365 6c66 2e5f 6861 735f 696e 6465 7828  self._has_index(
-000169a0: 6b69 6e64 2c20 636f 6e6e 6563 7469 6f6e  kind, connection
-000169b0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-000169c0: 206d 6574 6828 2274 6573 745f 7461 626c   meth("test_tabl
-000169d0: 6522 2c20 226d 795f 6964 7822 290a 2020  e", "my_idx").  
-000169e0: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
-000169f0: 206d 6574 6828 2274 6573 745f 7461 626c   meth("test_tabl
-00016a00: 6522 2c20 226d 795f 6964 785f 7322 290a  e", "my_idx_s").
-00016a10: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-00016a20: 6f74 206d 6574 6828 226e 6f6e 6578 6973  ot meth("nonexis
-00016a30: 7465 6e74 5f74 6162 6c65 222c 2022 6d79  tent_table", "my
-00016a40: 5f69 6478 2229 0a20 2020 2020 2020 2061  _idx").        a
-00016a50: 7373 6572 7420 6e6f 7420 6d65 7468 2822  ssert not meth("
-00016a60: 7465 7374 5f74 6162 6c65 222c 2022 6e6f  test_table", "no
-00016a70: 6e65 7869 7374 656e 745f 6964 7822 290a  nexistent_idx").
-00016a80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00016a90: 6e6f 7420 6d65 7468 2822 7465 7374 5f74  not meth("test_t
-00016aa0: 6162 6c65 222c 2022 6d79 5f69 6478 5f32  able", "my_idx_2
-00016ab0: 2229 0a20 2020 2020 2020 2061 7373 6572  ").        asser
-00016ac0: 7420 6e6f 7420 6d65 7468 2822 7465 7374  t not meth("test
-00016ad0: 5f74 6162 6c65 5f32 222c 2022 6d79 5f69  _table_2", "my_i
-00016ae0: 6478 5f33 2229 0a20 2020 2020 2020 2069  dx_3").        i
-00016af0: 6478 203d 2049 6e64 6578 2822 6d79 5f69  dx = Index("my_i
-00016b00: 6478 5f32 222c 2073 656c 662e 7461 626c  dx_2", self.tabl
-00016b10: 6573 2e74 6573 745f 7461 626c 652e 632e  es.test_table.c.
-00016b20: 6461 7461 3229 0a20 2020 2020 2020 2074  data2).        t
-00016b30: 626c 203d 2054 6162 6c65 280a 2020 2020  bl = Table(.    
-00016b40: 2020 2020 2020 2020 2274 6573 745f 7461          "test_ta
-00016b50: 626c 655f 3222 2c0a 2020 2020 2020 2020  ble_2",.        
-00016b60: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00016b70: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00016b80: 2822 666f 6f22 2c20 496e 7465 6765 722c  ("foo", Integer,
-00016b90: 2070 7269 6d61 7279 5f6b 6579 3d54 7275   primary_key=Tru
-00016ba0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00016bb0: 496e 6465 7828 226d 795f 6964 785f 3322  Index("my_idx_3"
-00016bc0: 2c20 2266 6f6f 2229 2c0a 2020 2020 2020  , "foo"),.      
-00016bd0: 2020 290a 2020 2020 2020 2020 6964 782e    ).        idx.
-00016be0: 6372 6561 7465 2863 6f6e 6e65 6374 696f  create(connectio
-00016bf0: 6e29 0a20 2020 2020 2020 2074 626c 2e63  n).        tbl.c
-00016c00: 7265 6174 6528 636f 6e6e 6563 7469 6f6e  reate(connection
-00016c10: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
-00016c20: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00016c30: 696e 6420 3d3d 2022 696e 7370 6563 746f  ind == "inspecto
-00016c40: 7222 3a0a 2020 2020 2020 2020 2020 2020  r":.            
-00016c50: 2020 2020 6173 7365 7274 206e 6f74 206d      assert not m
-00016c60: 6574 6828 2274 6573 745f 7461 626c 6522  eth("test_table"
-00016c70: 2c20 226d 795f 6964 785f 3222 290a 2020  , "my_idx_2").  
-00016c80: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00016c90: 7365 7274 206e 6f74 206d 6574 6828 2274  sert not meth("t
-00016ca0: 6573 745f 7461 626c 655f 3222 2c20 226d  est_table_2", "m
-00016cb0: 795f 6964 785f 3322 290a 2020 2020 2020  y_idx_3").      
-00016cc0: 2020 2020 2020 2020 2020 6d65 7468 2e5f            meth._
-00016cd0: 5f73 656c 665f 5f2e 636c 6561 725f 6361  _self__.clear_ca
-00016ce0: 6368 6528 290a 2020 2020 2020 2020 2020  che().          
-00016cf0: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
-00016d00: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
-00016d10: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00016d20: 6572 7420 6d65 7468 2822 7465 7374 5f74  ert meth("test_t
-00016d30: 6162 6c65 222c 2022 6d79 5f69 6478 5f32  able", "my_idx_2
-00016d40: 2229 2069 7320 5472 7565 0a20 2020 2020  ") is True.     
-00016d50: 2020 2020 2020 2061 7373 6572 7420 6d65         assert me
-00016d60: 7468 2822 7465 7374 5f74 6162 6c65 5f32  th("test_table_2
-00016d70: 222c 2022 6d79 5f69 6478 5f33 2229 2069  ", "my_idx_3") i
-00016d80: 7320 5472 7565 0a20 2020 2020 2020 2066  s True.        f
-00016d90: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-00016da0: 2020 2020 7462 6c2e 6472 6f70 2863 6f6e      tbl.drop(con
-00016db0: 6e65 6374 696f 6e29 0a20 2020 2020 2020  nection).       
-00016dc0: 2020 2020 2069 6478 2e64 726f 7028 636f       idx.drop(co
-00016dd0: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
-00016de0: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-00016df0: 2e63 6f6e 6e65 6374 696f 6e2e 636f 6d6d  .connection.comm
-00016e00: 6974 2829 0a20 2020 2020 2020 2020 2020  it().           
-00016e10: 2073 656c 662e 7461 626c 6573 5b22 7465   self.tables["te
-00016e20: 7374 5f74 6162 6c65 225d 2e69 6e64 6578  st_table"].index
-00016e30: 6573 2e72 656d 6f76 6528 6964 7829 0a0a  es.remove(idx)..
-00016e40: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00016e50: 2e73 6b69 7028 224e 6f74 2073 7570 706f  .skip("Not suppo
-00016e60: 7274 6564 2062 7920 436c 6f75 6420 5370  rted by Cloud Sp
-00016e70: 616e 6e65 7222 290a 2020 2020 406b 696e  anner").    @kin
-00016e80: 640a 2020 2020 6465 6620 7465 7374 5f68  d.    def test_h
-00016e90: 6173 5f69 6e64 6578 5f73 6368 656d 6128  as_index_schema(
-00016ea0: 7365 6c66 2c20 6b69 6e64 2c20 636f 6e6e  self, kind, conn
-00016eb0: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
-00016ec0: 2070 6173 730a 0a0a 636c 6173 7320 4861   pass...class Ha
-00016ed0: 7354 6162 6c65 5465 7374 285f 4861 7354  sTableTest(_HasT
-00016ee0: 6162 6c65 5465 7374 293a 0a20 2020 2040  ableTest):.    @
-00016ef0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00016f00: 6465 6620 6465 6669 6e65 5f74 6162 6c65  def define_table
-00016f10: 7328 636c 732c 206d 6574 6164 6174 6129  s(cls, metadata)
-00016f20: 3a0a 2020 2020 2020 2020 5461 626c 6528  :.        Table(
-00016f30: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
-00016f40: 7374 5f74 6162 6c65 222c 0a20 2020 2020  st_table",.     
-00016f50: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
-00016f60: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-00016f70: 756d 6e28 2269 6422 2c20 496e 7465 6765  umn("id", Intege
-00016f80: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-00016f90: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-00016fa0: 2020 436f 6c75 6d6e 2822 6461 7461 222c    Column("data",
-00016fb0: 2053 7472 696e 6728 3530 2929 2c0a 2020   String(50)),.  
-00016fc0: 2020 2020 2020 290a 0a20 2020 2040 7079        )..    @py
-00016fd0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00016fe0: 4e6f 7420 7375 7070 6f72 7465 6420 6279  Not supported by
-00016ff0: 2043 6c6f 7564 2053 7061 6e6e 6572 2229   Cloud Spanner")
-00017000: 0a20 2020 2064 6566 2074 6573 745f 6861  .    def test_ha
-00017010: 735f 7461 626c 655f 6e6f 6e65 7869 7374  s_table_nonexist
-00017020: 656e 745f 7363 6865 6d61 2873 656c 6629  ent_schema(self)
-00017030: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00017040: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00017050: 2e73 6b69 7028 224e 6f74 2073 7570 706f  .skip("Not suppo
-00017060: 7274 6564 2062 7920 436c 6f75 6420 5370  rted by Cloud Sp
-00017070: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
-00017080: 7465 7374 5f68 6173 5f74 6162 6c65 5f73  test_has_table_s
-00017090: 6368 656d 6128 7365 6c66 293a 0a20 2020  chema(self):.   
-000170a0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-000170b0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-000170c0: 2822 4e6f 7420 7375 7070 6f72 7465 6420  ("Not supported 
-000170d0: 6279 2043 6c6f 7564 2053 7061 6e6e 6572  by Cloud Spanner
-000170e0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-000170f0: 6861 735f 7461 626c 655f 6361 6368 6528  has_table_cache(
-00017100: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00017110: 6173 730a 0a20 2020 2040 7465 7374 696e  ass..    @testin
-00017120: 672e 7265 7175 6972 6573 2e76 6965 7773  g.requires.views
-00017130: 0a20 2020 2064 6566 2074 6573 745f 6861  .    def test_ha
-00017140: 735f 7461 626c 655f 7669 6577 2873 656c  s_table_view(sel
-00017150: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
-00017160: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00017170: 2020 4074 6573 7469 6e67 2e72 6571 7569    @testing.requi
-00017180: 7265 732e 7669 6577 730a 2020 2020 6465  res.views.    de
-00017190: 6620 7465 7374 5f68 6173 5f74 6162 6c65  f test_has_table
-000171a0: 5f76 6965 775f 7363 6865 6d61 2873 656c  _view_schema(sel
-000171b0: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
-000171c0: 2020 2020 2020 2020 7061 7373 0a0a 0a63          pass...c
-000171d0: 6c61 7373 2050 6f73 7443 6f6d 7069 6c65  lass PostCompile
-000171e0: 5061 7261 6d73 5465 7374 285f 506f 7374  ParamsTest(_Post
-000171f0: 436f 6d70 696c 6550 6172 616d 7354 6573  CompileParamsTes
-00017200: 7429 3a0a 2020 2020 6465 6620 7465 7374  t):.    def test
-00017210: 5f65 7865 6375 7465 2873 656c 6629 3a0a  _execute(self):.
-00017220: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-00017230: 7365 6c66 2e74 6162 6c65 732e 736f 6d65  self.tables.some
-00017240: 5f74 6162 6c65 0a0a 2020 2020 2020 2020  _table..        
-00017250: 7374 6d74 203d 2073 656c 6563 7428 7461  stmt = select(ta
-00017260: 626c 652e 632e 6964 292e 7768 6572 6528  ble.c.id).where(
-00017270: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00017280: 6c65 2e63 2e78 203d 3d20 7371 6c61 6c63  le.c.x == sqlalc
-00017290: 6865 6d79 2e62 696e 6470 6172 616d 2822  hemy.bindparam("
-000172a0: 7122 2c20 6c69 7465 7261 6c5f 6578 6563  q", literal_exec
-000172b0: 7574 653d 5472 7565 290a 2020 2020 2020  ute=True).      
-000172c0: 2020 290a 0a20 2020 2020 2020 2077 6974    )..        wit
-000172d0: 6820 7365 6c66 2e73 716c 5f65 7865 6375  h self.sql_execu
-000172e0: 7469 6f6e 5f61 7373 6572 7465 7228 2920  tion_asserter() 
-000172f0: 6173 2061 7373 6572 7465 723a 0a20 2020  as asserter:.   
-00017300: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-00017310: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
-00017320: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
-00017330: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
-00017340: 6578 6563 7574 6528 7374 6d74 2c20 6469  execute(stmt, di
-00017350: 6374 2871 3d31 3029 290a 0a20 2020 2020  ct(q=10))..     
-00017360: 2020 2061 7373 6572 7465 722e 6173 7365     asserter.asse
-00017370: 7274 5f28 0a20 2020 2020 2020 2020 2020  rt_(.           
-00017380: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-00017390: 696e 672e 6173 7365 7274 7371 6c2e 4375  ing.assertsql.Cu
-000173a0: 7273 6f72 5351 4c28 0a20 2020 2020 2020  rsorSQL(.       
-000173b0: 2020 2020 2020 2020 2022 5345 4c45 4354           "SELECT
-000173c0: 2073 6f6d 655f 7461 626c 652e 6964 205c   some_table.id \
-000173d0: 6e46 524f 4d20 736f 6d65 5f74 6162 6c65  nFROM some_table
-000173e0: 2022 2022 5c6e 5748 4552 4520 736f 6d65   " "\nWHERE some
-000173f0: 5f74 6162 6c65 2e78 203d 2031 3022 2c0a  _table.x = 10",.
-00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017410: 5b5d 2069 6620 636f 6e66 6967 2e64 622e  [] if config.db.
-00017420: 6469 616c 6563 742e 706f 7369 7469 6f6e  dialect.position
-00017430: 616c 2065 6c73 6520 7b7d 2c0a 2020 2020  al else {},.    
-00017440: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017450: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
-00017460: 745f 6578 6563 7574 655f 6578 7061 6e64  t_execute_expand
-00017470: 696e 675f 706c 7573 5f6c 6974 6572 616c  ing_plus_literal
-00017480: 5f65 7865 6375 7465 2873 656c 6629 3a0a  _execute(self):.
-00017490: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-000174a0: 7365 6c66 2e74 6162 6c65 732e 736f 6d65  self.tables.some
-000174b0: 5f74 6162 6c65 0a0a 2020 2020 2020 2020  _table..        
-000174c0: 7374 6d74 203d 2073 656c 6563 7428 7461  stmt = select(ta
-000174d0: 626c 652e 632e 6964 292e 7768 6572 6528  ble.c.id).where(
-000174e0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-000174f0: 6c65 2e63 2e78 2e69 6e5f 280a 2020 2020  le.c.x.in_(.    
-00017500: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-00017510: 6c63 6865 6d79 2e62 696e 6470 6172 616d  lchemy.bindparam
-00017520: 2822 7122 2c20 6578 7061 6e64 696e 673d  ("q", expanding=
-00017530: 5472 7565 2c20 6c69 7465 7261 6c5f 6578  True, literal_ex
-00017540: 6563 7574 653d 5472 7565 290a 2020 2020  ecute=True).    
-00017550: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017560: 2020 290a 0a20 2020 2020 2020 2077 6974    )..        wit
-00017570: 6820 7365 6c66 2e73 716c 5f65 7865 6375  h self.sql_execu
-00017580: 7469 6f6e 5f61 7373 6572 7465 7228 2920  tion_asserter() 
-00017590: 6173 2061 7373 6572 7465 723a 0a20 2020  as asserter:.   
-000175a0: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-000175b0: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
-000175c0: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
-000175d0: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
-000175e0: 6578 6563 7574 6528 7374 6d74 2c20 6469  execute(stmt, di
-000175f0: 6374 2871 3d5b 352c 2036 2c20 375d 2929  ct(q=[5, 6, 7]))
-00017600: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00017610: 6572 2e61 7373 6572 745f 280a 2020 2020  er.assert_(.    
-00017620: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
-00017630: 6d79 2e74 6573 7469 6e67 2e61 7373 6572  my.testing.asser
-00017640: 7473 716c 2e43 7572 736f 7253 514c 280a  tsql.CursorSQL(.
-00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017660: 2253 454c 4543 5420 736f 6d65 5f74 6162  "SELECT some_tab
-00017670: 6c65 2e69 6420 5c6e 4652 4f4d 2073 6f6d  le.id \nFROM som
-00017680: 655f 7461 626c 6520 220a 2020 2020 2020  e_table ".      
-00017690: 2020 2020 2020 2020 2020 225c 6e57 4845            "\nWHE
-000176a0: 5245 2073 6f6d 655f 7461 626c 652e 7820  RE some_table.x 
-000176b0: 494e 2028 352c 2036 2c20 3729 222c 0a20  IN (5, 6, 7)",. 
-000176c0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000176d0: 5d20 6966 2063 6f6e 6669 672e 6462 2e64  ] if config.db.d
-000176e0: 6961 6c65 6374 2e70 6f73 6974 696f 6e61  ialect.positiona
-000176f0: 6c20 656c 7365 207b 7d2c 0a20 2020 2020  l else {},.     
-00017700: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00017710: 2029 0a0a 2020 2020 4074 6573 7469 6e67   )..    @testing
-00017720: 2e72 6571 7569 7265 732e 7475 706c 655f  .requires.tuple_
-00017730: 696e 0a20 2020 2064 6566 2074 6573 745f  in.    def test_
-00017740: 6578 6563 7574 655f 7475 706c 655f 6578  execute_tuple_ex
-00017750: 7061 6e64 696e 675f 706c 7573 5f6c 6974  panding_plus_lit
-00017760: 6572 616c 5f65 7865 6375 7465 2873 656c  eral_execute(sel
-00017770: 6629 3a0a 2020 2020 2020 2020 7461 626c  f):.        tabl
-00017780: 6520 3d20 7365 6c66 2e74 6162 6c65 732e  e = self.tables.
-00017790: 736f 6d65 5f74 6162 6c65 0a0a 2020 2020  some_table..    
-000177a0: 2020 2020 7374 6d74 203d 2073 656c 6563      stmt = selec
-000177b0: 7428 7461 626c 652e 632e 6964 292e 7768  t(table.c.id).wh
-000177c0: 6572 6528 0a20 2020 2020 2020 2020 2020  ere(.           
-000177d0: 2073 716c 616c 6368 656d 792e 7475 706c   sqlalchemy.tupl
-000177e0: 655f 2874 6162 6c65 2e63 2e78 2c20 7461  e_(table.c.x, ta
-000177f0: 626c 652e 632e 7929 2e69 6e5f 280a 2020  ble.c.y).in_(.  
-00017800: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-00017810: 6c61 6c63 6865 6d79 2e62 696e 6470 6172  lalchemy.bindpar
-00017820: 616d 2822 7122 2c20 6578 7061 6e64 696e  am("q", expandin
-00017830: 673d 5472 7565 2c20 6c69 7465 7261 6c5f  g=True, literal_
-00017840: 6578 6563 7574 653d 5472 7565 290a 2020  execute=True).  
-00017850: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00017860: 2020 2020 290a 0a20 2020 2020 2020 2077      )..        w
-00017870: 6974 6820 7365 6c66 2e73 716c 5f65 7865  ith self.sql_exe
-00017880: 6375 7469 6f6e 5f61 7373 6572 7465 7228  cution_asserter(
-00017890: 2920 6173 2061 7373 6572 7465 723a 0a20  ) as asserter:. 
-000178a0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-000178b0: 636f 6e66 6967 2e64 622e 636f 6e6e 6563  config.db.connec
-000178c0: 7428 2920 6173 2063 6f6e 6e3a 0a20 2020  t() as conn:.   
-000178d0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000178e0: 6e2e 6578 6563 7574 6528 7374 6d74 2c20  n.execute(stmt, 
-000178f0: 6469 6374 2871 3d5b 2835 2c20 3130 292c  dict(q=[(5, 10),
-00017900: 2028 3132 2c20 3138 295d 2929 0a0a 2020   (12, 18)]))..  
-00017910: 2020 2020 2020 6173 7365 7274 6572 2e61        asserter.a
-00017920: 7373 6572 745f 280a 2020 2020 2020 2020  ssert_(.        
-00017930: 2020 2020 7371 6c61 6c63 6865 6d79 2e74      sqlalchemy.t
-00017940: 6573 7469 6e67 2e61 7373 6572 7473 716c  esting.assertsql
-00017950: 2e43 7572 736f 7253 514c 280a 2020 2020  .CursorSQL(.    
-00017960: 2020 2020 2020 2020 2020 2020 2253 454c              "SEL
-00017970: 4543 5420 736f 6d65 5f74 6162 6c65 2e69  ECT some_table.i
-00017980: 6420 5c6e 4652 4f4d 2073 6f6d 655f 7461  d \nFROM some_ta
-00017990: 626c 6520 220a 2020 2020 2020 2020 2020  ble ".          
-000179a0: 2020 2020 2020 225c 6e57 4845 5245 2028        "\nWHERE (
-000179b0: 736f 6d65 5f74 6162 6c65 2e78 2c20 736f  some_table.x, so
-000179c0: 6d65 5f74 6162 6c65 2e79 2920 220a 2020  me_table.y) ".  
-000179d0: 2020 2020 2020 2020 2020 2020 2020 2249                "I
-000179e0: 4e20 2825 7328 352c 2031 3029 2c20 2831  N (%s(5, 10), (1
-000179f0: 322c 2031 3829 2922 0a20 2020 2020 2020  2, 18))".       
-00017a00: 2020 2020 2020 2020 2025 2028 2256 414c           % ("VAL
-00017a10: 5545 5320 2220 6966 2063 6f6e 6669 672e  UES " if config.
-00017a20: 6462 2e64 6961 6c65 6374 2e74 7570 6c65  db.dialect.tuple
-00017a30: 5f69 6e5f 7661 6c75 6573 2065 6c73 6520  _in_values else 
-00017a40: 2222 292c 0a20 2020 2020 2020 2020 2020  ""),.           
-00017a50: 2020 2020 2028 2920 6966 2063 6f6e 6669       () if confi
-00017a60: 672e 6462 2e64 6961 6c65 6374 2e70 6f73  g.db.dialect.pos
-00017a70: 6974 696f 6e61 6c20 656c 7365 207b 7d2c  itional else {},
-00017a80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00017a90: 2020 2020 2020 2029 0a0a 2020 2020 4074         )..    @t
-00017aa0: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00017ab0: 7475 706c 655f 696e 0a20 2020 2064 6566  tuple_in.    def
-00017ac0: 2074 6573 745f 6578 6563 7574 655f 7475   test_execute_tu
-00017ad0: 706c 655f 6578 7061 6e64 696e 675f 706c  ple_expanding_pl
-00017ae0: 7573 5f6c 6974 6572 616c 5f68 6574 6572  us_literal_heter
-00017af0: 6f67 656e 656f 7573 5f65 7865 6375 7465  ogeneous_execute
-00017b00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00017b10: 7461 626c 6520 3d20 7365 6c66 2e74 6162  table = self.tab
-00017b20: 6c65 732e 736f 6d65 5f74 6162 6c65 0a0a  les.some_table..
-00017b30: 2020 2020 2020 2020 7374 6d74 203d 2073          stmt = s
-00017b40: 656c 6563 7428 7461 626c 652e 632e 6964  elect(table.c.id
-00017b50: 292e 7768 6572 6528 0a20 2020 2020 2020  ).where(.       
-00017b60: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
-00017b70: 7475 706c 655f 2874 6162 6c65 2e63 2e78  tuple_(table.c.x
-00017b80: 2c20 7461 626c 652e 632e 7a29 2e69 6e5f  , table.c.z).in_
-00017b90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00017ba0: 2020 7371 6c61 6c63 6865 6d79 2e62 696e    sqlalchemy.bin
-00017bb0: 6470 6172 616d 2822 7122 2c20 6578 7061  dparam("q", expa
-00017bc0: 6e64 696e 673d 5472 7565 2c20 6c69 7465  nding=True, lite
-00017bd0: 7261 6c5f 6578 6563 7574 653d 5472 7565  ral_execute=True
-00017be0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00017bf0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00017c00: 2020 2077 6974 6820 7365 6c66 2e73 716c     with self.sql
-00017c10: 5f65 7865 6375 7469 6f6e 5f61 7373 6572  _execution_asser
-00017c20: 7465 7228 2920 6173 2061 7373 6572 7465  ter() as asserte
-00017c30: 723a 0a20 2020 2020 2020 2020 2020 2077  r:.            w
-00017c40: 6974 6820 636f 6e66 6967 2e64 622e 636f  ith config.db.co
-00017c50: 6e6e 6563 7428 2920 6173 2063 6f6e 6e3a  nnect() as conn:
-00017c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c70: 2063 6f6e 6e2e 6578 6563 7574 6528 7374   conn.execute(st
-00017c80: 6d74 2c20 6469 6374 2871 3d5b 2835 2c20  mt, dict(q=[(5, 
-00017c90: 227a 3122 292c 2028 3132 2c20 227a 3322  "z1"), (12, "z3"
-00017ca0: 295d 2929 0a0a 2020 2020 2020 2020 6173  )]))..        as
-00017cb0: 7365 7274 6572 2e61 7373 6572 745f 280a  serter.assert_(.
-00017cc0: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-00017cd0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e61  lchemy.testing.a
-00017ce0: 7373 6572 7473 716c 2e43 7572 736f 7253  ssertsql.CursorS
-00017cf0: 514c 280a 2020 2020 2020 2020 2020 2020  QL(.            
-00017d00: 2020 2020 2253 454c 4543 5420 736f 6d65      "SELECT some
-00017d10: 5f74 6162 6c65 2e69 6420 5c6e 4652 4f4d  _table.id \nFROM
-00017d20: 2073 6f6d 655f 7461 626c 6520 220a 2020   some_table ".  
-00017d30: 2020 2020 2020 2020 2020 2020 2020 225c                "\
-00017d40: 6e57 4845 5245 2028 736f 6d65 5f74 6162  nWHERE (some_tab
-00017d50: 6c65 2e78 2c20 736f 6d65 5f74 6162 6c65  le.x, some_table
-00017d60: 2e7a 2920 220a 2020 2020 2020 2020 2020  .z) ".          
-00017d70: 2020 2020 2020 2249 4e20 2825 7328 352c        "IN (%s(5,
-00017d80: 2027 7a31 2729 2c20 2831 322c 2027 7a33   'z1'), (12, 'z3
-00017d90: 2729 2922 0a20 2020 2020 2020 2020 2020  '))".           
-00017da0: 2020 2020 2025 2028 2256 414c 5545 5320       % ("VALUES 
-00017db0: 2220 6966 2063 6f6e 6669 672e 6462 2e64  " if config.db.d
-00017dc0: 6961 6c65 6374 2e74 7570 6c65 5f69 6e5f  ialect.tuple_in_
-00017dd0: 7661 6c75 6573 2065 6c73 6520 2222 292c  values else ""),
-00017de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017df0: 2028 2920 6966 2063 6f6e 6669 672e 6462   () if config.db
-00017e00: 2e64 6961 6c65 6374 2e70 6f73 6974 696f  .dialect.positio
-00017e10: 6e61 6c20 656c 7365 207b 7d2c 0a20 2020  nal else {},.   
-00017e20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00017e30: 2020 2029 0a0a 0a40 7079 7465 7374 2e6d     )...@pytest.m
-00017e40: 6172 6b2e 736b 6970 6966 280a 2020 2020  ark.skipif(.    
-00017e50: 626f 6f6c 286f 732e 656e 7669 726f 6e2e  bool(os.environ.
-00017e60: 6765 7428 2253 5041 4e4e 4552 5f45 4d55  get("SPANNER_EMU
-00017e70: 4c41 544f 525f 484f 5354 2229 292c 2072  LATOR_HOST")), r
-00017e80: 6561 736f 6e3d 2253 6b69 7070 6564 206f  eason="Skipped o
-00017e90: 6e20 656d 756c 6174 6f72 220a 290a 636c  n emulator".).cl
-00017ea0: 6173 7320 4a53 4f4e 5465 7374 285f 4a53  ass JSONTest(_JS
-00017eb0: 4f4e 5465 7374 293a 0a20 2020 2040 7079  ONTest):.    @py
-00017ec0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00017ed0: 5661 6c75 6573 2077 6974 686f 7574 206b  Values without k
-00017ee0: 6579 7320 6172 6520 6e6f 7420 7375 7070  eys are not supp
-00017ef0: 6f72 7465 642e 2229 0a20 2020 2064 6566  orted.").    def
-00017f00: 2074 6573 745f 7369 6e67 6c65 5f65 6c65   test_single_ele
-00017f10: 6d65 6e74 5f72 6f75 6e64 5f74 7269 7028  ment_round_trip(
-00017f20: 7365 6c66 2c20 656c 656d 656e 7429 3a0a  self, element):.
-00017f30: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00017f40: 2020 6465 6620 5f74 6573 745f 726f 756e    def _test_roun
-00017f50: 645f 7472 6970 2873 656c 662c 2064 6174  d_trip(self, dat
-00017f60: 615f 656c 656d 656e 742c 2063 6f6e 6e65  a_element, conne
-00017f70: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-00017f80: 6461 7461 5f74 6162 6c65 203d 2073 656c  data_table = sel
-00017f90: 662e 7461 626c 6573 2e64 6174 615f 7461  f.tables.data_ta
-00017fa0: 626c 650a 0a20 2020 2020 2020 2063 6f6e  ble..        con
-00017fb0: 6e65 6374 696f 6e2e 6578 6563 7574 6528  nection.execute(
-00017fc0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00017fd0: 615f 7461 626c 652e 696e 7365 7274 2829  a_table.insert()
-00017fe0: 2c0a 2020 2020 2020 2020 2020 2020 7b22  ,.            {"
-00017ff0: 6964 223a 2072 616e 646f 6d2e 7261 6e64  id": random.rand
-00018000: 696e 7428 312c 2031 3030 3030 3030 3030  int(1, 100000000
-00018010: 292c 2022 6e61 6d65 223a 2022 726f 7731  ), "name": "row1
-00018020: 222c 2022 6461 7461 223a 2064 6174 615f  ", "data": data_
-00018030: 656c 656d 656e 747d 2c0a 2020 2020 2020  element},.      
-00018040: 2020 290a 0a20 2020 2020 2020 2072 6f77    )..        row
-00018050: 203d 2063 6f6e 6e65 6374 696f 6e2e 6578   = connection.ex
-00018060: 6563 7574 6528 7365 6c65 6374 2864 6174  ecute(select(dat
-00018070: 615f 7461 626c 652e 632e 6461 7461 2929  a_table.c.data))
-00018080: 2e66 6972 7374 2829 0a0a 2020 2020 2020  .first()..      
-00018090: 2020 6571 5f28 726f 772c 2028 6461 7461    eq_(row, (data
-000180a0: 5f65 6c65 6d65 6e74 2c29 290a 0a20 2020  _element,))..   
-000180b0: 2064 6566 2074 6573 745f 756e 6963 6f64   def test_unicod
-000180c0: 655f 726f 756e 645f 7472 6970 2873 656c  e_round_trip(sel
-000180d0: 6629 3a0a 2020 2020 2020 2020 2320 6e6f  f):.        # no
-000180e0: 7465 2077 6520 696e 636c 7564 6520 556e  te we include Un
-000180f0: 6963 6f64 6520 7375 7070 6c65 6d65 6e74  icode supplement
-00018100: 6172 7920 6368 6172 6163 7465 7273 2061  ary characters a
-00018110: 7320 7765 6c6c 0a20 2020 2020 2020 2077  s well.        w
-00018120: 6974 6820 636f 6e66 6967 2e64 622e 636f  ith config.db.co
-00018130: 6e6e 6563 7428 2920 6173 2063 6f6e 6e3a  nnect() as conn:
-00018140: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00018150: 6e2e 6578 6563 7574 6528 0a20 2020 2020  n.execute(.     
-00018160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018170: 7461 626c 6573 2e64 6174 615f 7461 626c  tables.data_tabl
-00018180: 652e 696e 7365 7274 2829 2c0a 2020 2020  e.insert(),.    
-00018190: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181b0: 2020 2269 6422 3a20 7261 6e64 6f6d 2e72    "id": random.r
-000181c0: 616e 6469 6e74 2831 2c20 3130 3030 3030  andint(1, 100000
-000181d0: 3030 3029 2c0a 2020 2020 2020 2020 2020  000),.          
-000181e0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-000181f0: 3a20 2272 3122 2c0a 2020 2020 2020 2020  : "r1",.        
-00018200: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-00018210: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00018220: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00018230: c3a9 7665 f09f 908d 2069 6c6c c3a9 223a  ..ve.... ill..":
-00018240: 2022 72c3 a976 65f0 9f90 8d20 696c 6cc3   "r..ve.... ill.
-00018250: a922 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00018260: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-00018270: 6122 3a20 7b22 6b31 223a 2022 6472 c3b4  a": {"k1": "dr..
-00018280: 6cf0 9f90 8d65 227d 2c0a 2020 2020 2020  l....e"},.      
-00018290: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000182a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000182b0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000182c0: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
-000182d0: 715f 280a 2020 2020 2020 2020 2020 2020  q_(.            
-000182e0: 2020 2020 636f 6e6e 2e73 6361 6c61 7228      conn.scalar(
-000182f0: 7365 6c65 6374 2873 656c 662e 7461 626c  select(self.tabl
-00018300: 6573 2e64 6174 615f 7461 626c 652e 632e  es.data_table.c.
-00018310: 6461 7461 2929 2c0a 2020 2020 2020 2020  data)),.        
-00018320: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00018330: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00018340: c3a9 7665 f09f 908d 2069 6c6c c3a9 223a  ..ve.... ill..":
-00018350: 2022 72c3 a976 65f0 9f90 8d20 696c 6cc3   "r..ve.... ill.
-00018360: a922 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00018370: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
-00018380: 7b22 6b31 223a 2022 6472 c3b4 6cf0 9f90  {"k1": "dr..l...
-00018390: 8d65 227d 2c0a 2020 2020 2020 2020 2020  .e"},.          
-000183a0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000183b0: 2020 2020 2029 0a0a 2020 2020 4070 7974       )..    @pyt
-000183c0: 6573 742e 6d61 726b 2e73 6b69 7028 2250  est.mark.skip("P
-000183d0: 6172 616d 6574 6572 697a 6564 2074 7970  arameterized typ
-000183e0: 6573 2061 7265 206e 6f74 2073 7570 706f  es are not suppo
-000183f0: 7274 6564 2e22 290a 2020 2020 6465 6620  rted.").    def 
-00018400: 7465 7374 5f65 7661 6c5f 6e6f 6e65 5f66  test_eval_none_f
-00018410: 6c61 675f 6f72 6d28 7365 6c66 293a 0a20  lag_orm(self):. 
-00018420: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00018430: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
-00018440: 6970 280a 2020 2020 2020 2020 2253 7061  ip(.        "Spa
-00018450: 6e6e 6572 204a 534f 4e5f 5641 4c55 4528  nner JSON_VALUE(
-00018460: 2920 616c 7761 7973 2072 6574 7572 6e73  ) always returns
-00018470: 2053 5452 494e 472c 220a 2020 2020 2020   STRING,".      
-00018480: 2020 2274 6875 732c 2074 6869 7320 7465    "thus, this te
-00018490: 7374 2063 6173 6520 6361 6e27 7420 6265  st case can't be
-000184a0: 2065 7865 6375 7465 642e 220a 2020 2020   executed.".    
-000184b0: 290a 2020 2020 6465 6620 7465 7374 5f69  ).    def test_i
-000184c0: 6e64 6578 5f74 7970 6564 5f63 6f6d 7061  ndex_typed_compa
-000184d0: 7269 736f 6e28 7365 6c66 293a 0a20 2020  rison(self):.   
-000184e0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-000184f0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-00018500: 280a 2020 2020 2020 2020 2253 7061 6e6e  (.        "Spann
-00018510: 6572 204a 534f 4e5f 5641 4c55 4528 2920  er JSON_VALUE() 
-00018520: 616c 7761 7973 2072 6574 7572 6e73 2053  always returns S
-00018530: 5452 494e 472c 220a 2020 2020 2020 2020  TRING,".        
-00018540: 2274 6875 732c 2074 6869 7320 7465 7374  "thus, this test
-00018550: 2063 6173 6520 6361 6e27 7420 6265 2065   case can't be e
-00018560: 7865 6375 7465 642e 220a 2020 2020 290a  xecuted.".    ).
-00018570: 2020 2020 6465 6620 7465 7374 5f70 6174      def test_pat
-00018580: 685f 7479 7065 645f 636f 6d70 6172 6973  h_typed_comparis
-00018590: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
-000185a0: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
-000185b0: 6573 742e 6d61 726b 2e73 6b69 7028 2243  est.mark.skip("C
-000185c0: 7573 746f 6d20 4a53 4f4e 2064 652d 2f73  ustom JSON de-/s
-000185d0: 6572 6961 6c69 7a65 7273 2061 7265 206e  erializers are n
-000185e0: 6f74 2073 7570 706f 7274 6564 2e22 290a  ot supported.").
-000185f0: 2020 2020 6465 6620 7465 7374 5f72 6f75      def test_rou
-00018600: 6e64 5f74 7269 705f 6375 7374 6f6d 5f6a  nd_trip_custom_j
-00018610: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
-00018620: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00018630: 205f 696e 6465 785f 6669 7874 7572 6573   _index_fixtures
-00018640: 2866 6e29 3a0a 2020 2020 2020 2020 666e  (fn):.        fn
-00018650: 203d 2074 6573 7469 6e67 2e63 6f6d 6269   = testing.combi
-00018660: 6e61 7469 6f6e 7328 0a20 2020 2020 2020  nations(.       
-00018670: 2020 2020 2028 2262 6f6f 6c65 616e 222c       ("boolean",
-00018680: 2054 7275 6529 2c0a 2020 2020 2020 2020   True),.        
-00018690: 2020 2020 2822 626f 6f6c 6561 6e22 2c20      ("boolean", 
-000186a0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-000186b0: 2020 2020 2822 626f 6f6c 6561 6e22 2c20      ("boolean", 
-000186c0: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
-000186d0: 2020 2028 2273 7472 696e 6722 2c20 2273     ("string", "s
-000186e0: 6f6d 6520 7374 7269 6e67 2229 2c0a 2020  ome string"),.  
-000186f0: 2020 2020 2020 2020 2020 2822 7374 7269            ("stri
-00018700: 6e67 222c 204e 6f6e 6529 2c0a 2020 2020  ng", None),.    
-00018710: 2020 2020 2020 2020 2822 696e 7465 6765          ("intege
-00018720: 7222 2c20 3135 292c 0a20 2020 2020 2020  r", 15),.       
-00018730: 2020 2020 2028 2269 6e74 6567 6572 222c       ("integer",
-00018740: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
-00018750: 2028 2269 6e74 6567 6572 222c 2030 292c   ("integer", 0),
-00018760: 0a20 2020 2020 2020 2020 2020 2028 2269  .            ("i
-00018770: 6e74 6567 6572 222c 204e 6f6e 6529 2c0a  nteger", None),.
-00018780: 2020 2020 2020 2020 2020 2020 2822 666c              ("fl
-00018790: 6f61 7422 2c20 3238 2e35 292c 0a20 2020  oat", 28.5),.   
-000187a0: 2020 2020 2020 2020 2028 2266 6c6f 6174           ("float
-000187b0: 222c 204e 6f6e 6529 2c0a 2020 2020 2020  ", None),.      
-000187c0: 2020 2020 2020 6964 5f3d 2273 6122 2c0a        id_="sa",.
-000187d0: 2020 2020 2020 2020 2928 666e 290a 2020          )(fn).  
-000187e0: 2020 2020 2020 7265 7475 726e 2066 6e0a        return fn.
-000187f0: 0a20 2020 2040 5f69 6e64 6578 5f66 6978  .    @_index_fix
-00018800: 7475 7265 730a 2020 2020 6465 6620 7465  tures.    def te
-00018810: 7374 5f69 6e64 6578 5f74 7970 6564 5f61  st_index_typed_a
-00018820: 6363 6573 7328 7365 6c66 2c20 6461 7461  ccess(self, data
-00018830: 7479 7065 2c20 7661 6c75 6529 3a0a 2020  type, value):.  
-00018840: 2020 2020 2020 6461 7461 5f74 6162 6c65        data_table
-00018850: 203d 2073 656c 662e 7461 626c 6573 2e64   = self.tables.d
-00018860: 6174 615f 7461 626c 650a 2020 2020 2020  ata_table.      
-00018870: 2020 6461 7461 5f65 6c65 6d65 6e74 203d    data_element =
-00018880: 207b 226b 6579 3122 3a20 7661 6c75 657d   {"key1": value}
-00018890: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
-000188a0: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
-000188b0: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
-000188c0: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
-000188d0: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
-000188e0: 2020 2020 2064 6174 615f 7461 626c 652e       data_table.
-000188f0: 696e 7365 7274 2829 2c0a 2020 2020 2020  insert(),.      
-00018900: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00018910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018920: 2269 6422 3a20 7261 6e64 6f6d 2e72 616e  "id": random.ran
-00018930: 6469 6e74 2831 2c20 3130 3030 3030 3030  dint(1, 10000000
-00018940: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-00018950: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-00018960: 2272 6f77 3122 2c0a 2020 2020 2020 2020  "row1",.        
-00018970: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-00018980: 6122 3a20 6461 7461 5f65 6c65 6d65 6e74  a": data_element
-00018990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000189a0: 2020 2020 2020 226e 756c 6c64 6174 6122        "nulldata"
-000189b0: 3a20 6461 7461 5f65 6c65 6d65 6e74 2c0a  : data_element,.
-000189c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189d0: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
-000189e0: 0a0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-000189f0: 7072 203d 2064 6174 615f 7461 626c 652e  pr = data_table.
-00018a00: 632e 6461 7461 5b22 6b65 7931 225d 0a20  c.data["key1"]. 
-00018a10: 2020 2020 2020 2020 2020 2065 7870 7220             expr 
-00018a20: 3d20 6765 7461 7474 7228 6578 7072 2c20  = getattr(expr, 
-00018a30: 2261 735f 2573 2220 2520 6461 7461 7479  "as_%s" % dataty
-00018a40: 7065 2928 290a 0a20 2020 2020 2020 2020  pe)()..         
-00018a50: 2020 2072 6f75 6e64 7472 6970 203d 2063     roundtrip = c
-00018a60: 6f6e 6e2e 7363 616c 6172 2873 656c 6563  onn.scalar(selec
-00018a70: 7428 6578 7072 2929 0a20 2020 2020 2020  t(expr)).       
-00018a80: 2020 2020 2069 6620 726f 756e 6474 7269       if roundtri
-00018a90: 7020 696e 2028 2274 7275 6522 2c20 2266  p in ("true", "f
-00018aa0: 616c 7365 222c 204e 6f6e 6529 3a0a 2020  alse", None):.  
-00018ab0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00018ac0: 756e 6474 7269 7020 3d20 7374 7228 726f  undtrip = str(ro
-00018ad0: 756e 6474 7269 7029 2e63 6170 6974 616c  undtrip).capital
-00018ae0: 697a 6528 290a 0a20 2020 2020 2020 2020  ize()..         
-00018af0: 2020 2065 715f 2873 7472 2872 6f75 6e64     eq_(str(round
-00018b00: 7472 6970 292c 2073 7472 2876 616c 7565  trip), str(value
-00018b10: 2929 0a0a 2020 2020 4070 7974 6573 742e  ))..    @pytest.
-00018b20: 6d61 726b 2e73 6b69 7028 0a20 2020 2020  mark.skip(.     
-00018b30: 2020 2022 5370 616e 6e65 7220 646f 6573     "Spanner does
-00018b40: 6e27 7420 7375 7070 6f72 7420 7479 7065  n't support type
-00018b50: 2063 6173 7473 2069 6e73 6964 6520 4a53   casts inside JS
-00018b60: 4f4e 5f56 414c 5545 2829 2066 756e 6374  ON_VALUE() funct
-00018b70: 696f 6e2e 220a 2020 2020 290a 2020 2020  ion.".    ).    
-00018b80: 6465 6620 7465 7374 5f72 6f75 6e64 5f74  def test_round_t
-00018b90: 7269 705f 6a73 6f6e 5f6e 756c 6c5f 6173  rip_json_null_as
-00018ba0: 5f6a 736f 6e5f 6e75 6c6c 2873 656c 6629  _json_null(self)
-00018bb0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00018bc0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00018bd0: 2e73 6b69 7028 0a20 2020 2020 2020 2022  .skip(.        "
-00018be0: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-00018bf0: 7375 7070 6f72 7420 7479 7065 2063 6173  support type cas
-00018c00: 7473 2069 6e73 6964 6520 4a53 4f4e 5f56  ts inside JSON_V
-00018c10: 414c 5545 2829 2066 756e 6374 696f 6e2e  ALUE() function.
-00018c20: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
-00018c30: 7465 7374 5f72 6f75 6e64 5f74 7269 705f  test_round_trip_
-00018c40: 6e6f 6e65 5f61 735f 6a73 6f6e 5f6e 756c  none_as_json_nul
-00018c50: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-00018c60: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-00018c70: 7374 2e6d 6172 6b2e 736b 6970 280a 2020  st.mark.skip(.  
-00018c80: 2020 2020 2020 2253 7061 6e6e 6572 2064        "Spanner d
-00018c90: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-00018ca0: 7970 6520 6361 7374 7320 696e 7369 6465  ype casts inside
-00018cb0: 204a 534f 4e5f 5641 4c55 4528 2920 6675   JSON_VALUE() fu
-00018cc0: 6e63 7469 6f6e 2e22 0a20 2020 2029 0a20  nction.".    ). 
-00018cd0: 2020 2064 6566 2074 6573 745f 726f 756e     def test_roun
-00018ce0: 645f 7472 6970 5f6e 6f6e 655f 6173 5f73  d_trip_none_as_s
-00018cf0: 716c 5f6e 756c 6c28 7365 6c66 293a 0a20  ql_null(self):. 
-00018d00: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
-00018d10: 6173 7320 4578 6563 7574 696f 6e4f 7074  ass ExecutionOpt
-00018d20: 696f 6e73 5265 7175 6573 7450 7269 6f72  ionsRequestPrior
-00018d30: 6f74 7954 6573 7428 6669 7874 7572 6573  otyTest(fixtures
-00018d40: 2e54 6573 7442 6173 6529 3a0a 2020 2020  .TestBase):.    
-00018d50: 6465 6620 7365 7455 7028 7365 6c66 293a  def setUp(self):
-00018d60: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-00018d70: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
-00018d80: 6e67 696e 6528 6765 745f 6462 5f75 726c  ngine(get_db_url
-00018d90: 2829 2c20 706f 6f6c 5f73 697a 653d 3129  (), pool_size=1)
-00018da0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00018db0: 6120 3d20 4d65 7461 4461 7461 2829 0a0a  a = MetaData()..
-00018dc0: 2020 2020 2020 2020 7365 6c66 2e5f 7461          self._ta
-00018dd0: 626c 6520 3d20 5461 626c 6528 0a20 2020  ble = Table(.   
-00018de0: 2020 2020 2020 2020 2022 6578 6563 7574           "execut
-00018df0: 696f 6e5f 6f70 7469 6f6e 7332 222c 0a20  ion_options2",. 
-00018e00: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00018e10: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00018e20: 2043 6f6c 756d 6e28 226f 7074 5f69 6422   Column("opt_id"
-00018e30: 2c20 496e 7465 6765 722c 2070 7269 6d61  , Integer, prima
-00018e40: 7279 5f6b 6579 3d54 7275 6529 2c0a 2020  ry_key=True),.  
-00018e50: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00018e60: 2822 6f70 745f 6e61 6d65 222c 2053 7472  ("opt_name", Str
-00018e70: 696e 6728 3136 292c 206e 756c 6c61 626c  ing(16), nullabl
-00018e80: 653d 4661 6c73 6529 2c0a 2020 2020 2020  e=False),.      
-00018e90: 2020 290a 0a20 2020 2020 2020 206d 6574    )..        met
-00018ea0: 6164 6174 612e 6372 6561 7465 5f61 6c6c  adata.create_all
-00018eb0: 2873 656c 662e 5f65 6e67 696e 6529 0a20  (self._engine). 
-00018ec0: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00018ed0: 7028 3129 0a0a 2020 2020 6465 6620 7465  p(1)..    def te
-00018ee0: 7374 5f72 6571 7565 7374 5f70 7269 6f72  st_request_prior
-00018ef0: 6974 7928 7365 6c66 293a 0a20 2020 2020  ity(self):.     
-00018f00: 2020 2050 5249 4f52 4954 5920 3d20 5265     PRIORITY = Re
-00018f10: 7175 6573 744f 7074 696f 6e73 2e50 7269  questOptions.Pri
-00018f20: 6f72 6974 792e 5052 494f 5249 5459 5f4d  ority.PRIORITY_M
-00018f30: 4544 4955 4d0a 2020 2020 2020 2020 7769  EDIUM.        wi
-00018f40: 7468 2073 656c 662e 5f65 6e67 696e 652e  th self._engine.
-00018f50: 636f 6e6e 6563 7428 292e 6578 6563 7574  connect().execut
-00018f60: 696f 6e5f 6f70 7469 6f6e 7328 0a20 2020  ion_options(.   
-00018f70: 2020 2020 2020 2020 2072 6571 7565 7374           request
-00018f80: 5f70 7269 6f72 6974 793d 5052 494f 5249  _priority=PRIORI
-00018f90: 5459 0a20 2020 2020 2020 2029 2061 7320  TY.        ) as 
-00018fa0: 636f 6e6e 6563 7469 6f6e 3a0a 2020 2020  connection:.    
-00018fb0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
-00018fc0: 6f6e 2e65 7865 6375 7465 2873 656c 6563  on.execute(selec
-00018fd0: 7428 7365 6c66 2e5f 7461 626c 6529 292e  t(self._table)).
-00018fe0: 6665 7463 6861 6c6c 2829 0a0a 2020 2020  fetchall()..    
-00018ff0: 2020 2020 7769 7468 2073 656c 662e 5f65      with self._e
-00019000: 6e67 696e 652e 636f 6e6e 6563 7428 2920  ngine.connect() 
-00019010: 6173 2063 6f6e 6e65 6374 696f 6e3a 0a20  as connection:. 
-00019020: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00019030: 7420 636f 6e6e 6563 7469 6f6e 2e63 6f6e  t connection.con
-00019040: 6e65 6374 696f 6e2e 7265 7175 6573 745f  nection.request_
-00019050: 7072 696f 7269 7479 2069 7320 4e6f 6e65  priority is None
-00019060: 0a0a 2020 2020 2020 2020 656e 6769 6e65  ..        engine
-00019070: 203d 2063 7265 6174 655f 656e 6769 6e65   = create_engine
-00019080: 2822 7371 6c69 7465 3a2f 2f2f 6461 7461  ("sqlite:///data
-00019090: 6261 7365 2229 0a20 2020 2020 2020 2077  base").        w
-000190a0: 6974 6820 656e 6769 6e65 2e63 6f6e 6e65  ith engine.conne
-000190b0: 6374 2829 2061 7320 636f 6e6e 6563 7469  ct() as connecti
-000190c0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000190d0: 7061 7373 0a                             pass.
+00005c00: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00005c10: 2020 2020 2020 2020 3e20 302c 0a20 2020          > 0,.   
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2022 2573 2825 7329 2c20 2573 2825 7329   "%s(%s), %s(%s)
+00005c40: 2220 2520 2863 6f6c 2e6e 616d 652c 2063  " % (col.name, c
+00005c50: 6f6c 2e74 7970 652c 2063 6f6c 735b 695d  ol.type, cols[i]
+00005c60: 5b22 6e61 6d65 225d 2c20 6374 7970 6529  ["name"], ctype)
+00005c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005c80: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00005c90: 2020 2020 2069 6620 6e6f 7420 636f 6c2e       if not col.
+00005ca0: 7072 696d 6172 795f 6b65 793a 0a20 2020  primary_key:.   
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2061 7373 6572 7420 636f 6c73 5b69 5d5b   assert cols[i][
+00005cd0: 2264 6566 6175 6c74 225d 2069 7320 4e6f  "default"] is No
+00005ce0: 6e65 0a0a 2020 2020 4070 7974 6573 742e  ne..    @pytest.
+00005cf0: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
+00005d00: 2020 2020 2062 6f6f 6c28 6f73 2e65 6e76       bool(os.env
+00005d10: 6972 6f6e 2e67 6574 2822 5350 414e 4e45  iron.get("SPANNE
+00005d20: 525f 454d 554c 4154 4f52 5f48 4f53 5422  R_EMULATOR_HOST"
+00005d30: 2929 2c20 7265 6173 6f6e 3d22 536b 6970  )), reason="Skip
+00005d40: 7065 6420 6f6e 2065 6d75 6c61 746f 7222  ped on emulator"
+00005d50: 0a20 2020 2029 0a20 2020 2040 7465 7374  .    ).    @test
+00005d60: 696e 672e 7265 7175 6972 6573 2e76 6965  ing.requires.vie
+00005d70: 775f 7265 666c 6563 7469 6f6e 0a20 2020  w_reflection.   
+00005d80: 2064 6566 2074 6573 745f 6765 745f 7669   def test_get_vi
+00005d90: 6577 5f64 6566 696e 6974 696f 6e28 0a20  ew_definition(. 
+00005da0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00005db0: 2020 2020 2063 6f6e 6e65 6374 696f 6e2c       connection,
+00005dc0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00005dd0: 7363 6865 6d61 203d 204e 6f6e 650a 2020  schema = None.  
+00005de0: 2020 2020 2020 696e 7370 203d 2069 6e73        insp = ins
+00005df0: 7065 6374 2863 6f6e 6e65 6374 696f 6e29  pect(connection)
+00005e00: 0a20 2020 2020 2020 2066 6f72 2076 6965  .        for vie
+00005e10: 7720 696e 205b 2275 7365 7273 5f76 222c  w in ["users_v",
+00005e20: 2022 656d 6169 6c5f 6164 6472 6573 7365   "email_addresse
+00005e30: 735f 7622 2c20 2264 696e 6761 6c69 6e67  s_v", "dingaling
+00005e40: 735f 7622 5d3a 0a20 2020 2020 2020 2020  s_v"]:.         
+00005e50: 2020 2076 203d 2069 6e73 702e 6765 745f     v = insp.get_
+00005e60: 7669 6577 5f64 6566 696e 6974 696f 6e28  view_definition(
+00005e70: 7669 6577 2c20 7363 6865 6d61 3d73 6368  view, schema=sch
+00005e80: 656d 6129 0a20 2020 2020 2020 2020 2020  ema).           
+00005e90: 2069 735f 7472 7565 2862 6f6f 6c28 7629   is_true(bool(v)
+00005ea0: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+00005eb0: 6172 6b2e 736b 6970 6966 280a 2020 2020  ark.skipif(.    
+00005ec0: 2020 2020 626f 6f6c 286f 732e 656e 7669      bool(os.envi
+00005ed0: 726f 6e2e 6765 7428 2253 5041 4e4e 4552  ron.get("SPANNER
+00005ee0: 5f45 4d55 4c41 544f 525f 484f 5354 2229  _EMULATOR_HOST")
+00005ef0: 292c 2072 6561 736f 6e3d 2253 6b69 7070  ), reason="Skipp
+00005f00: 6564 206f 6e20 656d 756c 6174 6f72 220a  ed on emulator".
+00005f10: 2020 2020 290a 2020 2020 4074 6573 7469      ).    @testi
+00005f20: 6e67 2e72 6571 7569 7265 732e 7669 6577  ng.requires.view
+00005f30: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
+00005f40: 6465 6620 7465 7374 5f67 6574 5f76 6965  def test_get_vie
+00005f50: 775f 6465 6669 6e69 7469 6f6e 5f64 6f65  w_definition_doe
+00005f60: 735f 6e6f 745f 6578 6973 7428 7365 6c66  s_not_exist(self
+00005f70: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00005f80: 2020 2020 2020 2073 7570 6572 2829 2e74         super().t
+00005f90: 6573 745f 6765 745f 7669 6577 5f64 6566  est_get_view_def
+00005fa0: 696e 6974 696f 6e5f 646f 6573 5f6e 6f74  inition_does_not
+00005fb0: 5f65 7869 7374 2863 6f6e 6e65 6374 696f  _exist(connectio
+00005fc0: 6e29 0a0a 2020 2020 6465 6620 6669 6c74  n)..    def filt
+00005fd0: 6572 5f6e 616d 655f 7661 6c75 6573 2829  er_name_values()
+00005fe0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00005ff0: 2074 6573 7469 6e67 2e63 6f6d 6269 6e61   testing.combina
+00006000: 7469 6f6e 7328 5472 7565 2c20 4661 6c73  tions(True, Fals
+00006010: 652c 2061 7267 6e61 6d65 733d 2275 7365  e, argnames="use
+00006020: 5f66 696c 7465 7222 290a 0a20 2020 2040  _filter")..    @
+00006030: 6669 6c74 6572 5f6e 616d 655f 7661 6c75  filter_name_valu
+00006040: 6573 2829 0a20 2020 2040 7465 7374 696e  es().    @testin
+00006050: 672e 7265 7175 6972 6573 2e69 6e64 6578  g.requires.index
+00006060: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
+00006070: 6465 6620 7465 7374 5f67 6574 5f6d 756c  def test_get_mul
+00006080: 7469 5f69 6e64 6578 6573 280a 2020 2020  ti_indexes(.    
+00006090: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000060a0: 2020 6765 745f 6d75 6c74 695f 6578 702c    get_multi_exp,
+000060b0: 0a20 2020 2020 2020 2075 7365 5f66 696c  .        use_fil
+000060c0: 7465 722c 0a20 2020 2020 2020 2073 6368  ter,.        sch
+000060d0: 656d 613d 4e6f 6e65 2c0a 2020 2020 2020  ema=None,.      
+000060e0: 2020 7363 6f70 653d 4f62 6a65 6374 5363    scope=ObjectSc
+000060f0: 6f70 652e 4445 4641 554c 542c 0a20 2020  ope.DEFAULT,.   
+00006100: 2020 2020 206b 696e 643d 4f62 6a65 6374       kind=Object
+00006110: 4b69 6e64 2e54 4142 4c45 2c0a 2020 2020  Kind.TABLE,.    
+00006120: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00006130: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
+00006140: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
+00006150: 2020 5370 616e 6e65 7220 646f 6573 6e27    Spanner doesn'
+00006160: 7420 7375 7070 6f72 7420 696e 6465 7865  t support indexe
+00006170: 7320 6f6e 2076 6965 7773 2061 6e64 0a20  s on views and. 
+00006180: 2020 2020 2020 2064 6f65 736e 2774 2073         doesn't s
+00006190: 7570 706f 7274 2074 656d 706f 7261 7279  upport temporary
+000061a0: 2074 6162 6c65 732c 2073 6f20 7265 616c   tables, so real
+000061b0: 2074 6162 6c65 7320 6172 650a 2020 2020   tables are.    
+000061c0: 2020 2020 7573 6564 2066 6f72 2074 6573      used for tes
+000061d0: 7469 6e67 2e20 4173 2074 6865 206f 7269  ting. As the ori
+000061e0: 6769 6e61 6c20 7465 7374 2065 7870 6563  ginal test expec
+000061f0: 7473 206f 6e6c 7920 7265 616c 0a20 2020  ts only real.   
+00006200: 2020 2020 2074 6162 6c65 7320 746f 2062       tables to b
+00006210: 6520 7265 6164 2c20 616e 6420 696e 2053  e read, and in S
+00006220: 7061 6e6e 6572 2061 6c6c 2074 6865 2074  panner all the t
+00006230: 6162 6c65 7320 6172 6520 7265 616c 2c0a  ables are real,.
+00006240: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00006250: 2072 6573 756c 7473 206f 7665 7272 6964   results overrid
+00006260: 6520 6973 2072 6571 7569 7265 642e 0a20  e is required.. 
+00006270: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006280: 2020 2069 6e73 702c 206b 7773 2c20 6578     insp, kws, ex
+00006290: 7020 3d20 6765 745f 6d75 6c74 695f 6578  p = get_multi_ex
+000062a0: 7028 0a20 2020 2020 2020 2020 2020 2073  p(.            s
+000062b0: 6368 656d 612c 0a20 2020 2020 2020 2020  chema,.         
+000062c0: 2020 2073 636f 7065 2c0a 2020 2020 2020     scope,.      
+000062d0: 2020 2020 2020 6b69 6e64 2c0a 2020 2020        kind,.    
+000062e0: 2020 2020 2020 2020 7573 655f 6669 6c74          use_filt
+000062f0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00006300: 496e 7370 6563 746f 722e 6765 745f 696e  Inspector.get_in
+00006310: 6465 7865 732c 0a20 2020 2020 2020 2020  dexes,.         
+00006320: 2020 2073 656c 662e 6578 705f 696e 6465     self.exp_inde
+00006330: 7865 732c 0a20 2020 2020 2020 2029 0a20  xes,.        ). 
+00006340: 2020 2020 2020 205f 6967 6e6f 7265 5f74         _ignore_t
+00006350: 6162 6c65 7320 3d20 5b0a 2020 2020 2020  ables = [.      
+00006360: 2020 2020 2020 284e 6f6e 652c 2022 636f        (None, "co
+00006370: 6d6d 656e 745f 7465 7374 2229 2c0a 2020  mment_test"),.  
+00006380: 2020 2020 2020 2020 2020 284e 6f6e 652c            (None,
+00006390: 2022 6469 6e67 616c 696e 6773 2229 2c0a   "dingalings"),.
+000063a0: 2020 2020 2020 2020 2020 2020 284e 6f6e              (Non
+000063b0: 652c 2022 656d 6169 6c5f 6164 6472 6573  e, "email_addres
+000063c0: 7365 7322 292c 0a20 2020 2020 2020 2020  ses"),.         
+000063d0: 2020 2028 4e6f 6e65 2c20 226e 6f5f 636f     (None, "no_co
+000063e0: 6e73 7472 6169 6e74 7322 292c 0a20 2020  nstraints"),.   
+000063f0: 2020 2020 205d 0a20 2020 2020 2020 2065       ].        e
+00006400: 7870 203d 207b 6b3a 2076 2066 6f72 206b  xp = {k: v for k
+00006410: 2c20 7620 696e 2065 7870 2e69 7465 6d73  , v in exp.items
+00006420: 2829 2069 6620 6b20 6e6f 7420 696e 205f  () if k not in _
+00006430: 6967 6e6f 7265 5f74 6162 6c65 737d 0a0a  ignore_tables}..
+00006440: 2020 2020 2020 2020 666f 7220 6b77 2069          for kw i
+00006450: 6e20 6b77 733a 0a20 2020 2020 2020 2020  n kws:.         
+00006460: 2020 2069 6e73 702e 636c 6561 725f 6361     insp.clear_ca
+00006470: 6368 6528 290a 2020 2020 2020 2020 2020  che().          
+00006480: 2020 7265 7375 6c74 203d 2069 6e73 702e    result = insp.
+00006490: 6765 745f 6d75 6c74 695f 696e 6465 7865  get_multi_indexe
+000064a0: 7328 2a2a 6b77 290a 2020 2020 2020 2020  s(**kw).        
+000064b0: 2020 2020 7365 6c66 2e5f 6368 6563 6b5f      self._check_
+000064c0: 7461 626c 655f 6469 6374 2872 6573 756c  table_dict(resul
+000064d0: 742c 2065 7870 2c20 7365 6c66 2e5f 7265  t, exp, self._re
+000064e0: 7175 6972 6564 5f69 6e64 6578 5f6b 6579  quired_index_key
+000064f0: 7329 0a0a 2020 2020 6465 6620 6578 705f  s)..    def exp_
+00006500: 706b 7328 0a20 2020 2020 2020 2073 656c  pks(.        sel
+00006510: 662c 0a20 2020 2020 2020 2073 6368 656d  f,.        schem
+00006520: 613d 4e6f 6e65 2c0a 2020 2020 2020 2020  a=None,.        
+00006530: 7363 6f70 653d 4f62 6a65 6374 5363 6f70  scope=ObjectScop
+00006540: 652e 414e 592c 0a20 2020 2020 2020 206b  e.ANY,.        k
+00006550: 696e 643d 4f62 6a65 6374 4b69 6e64 2e41  ind=ObjectKind.A
+00006560: 4e59 2c0a 2020 2020 2020 2020 6669 6c74  NY,.        filt
+00006570: 6572 5f6e 616d 6573 3d4e 6f6e 652c 0a20  er_names=None,. 
+00006580: 2020 2029 3a0a 2020 2020 2020 2020 6465     ):.        de
+00006590: 6620 706b 282a 636f 6c73 2c20 6e61 6d65  f pk(*cols, name
+000065a0: 3d6d 6f63 6b2e 414e 592c 2063 6f6d 6d65  =mock.ANY, comme
+000065b0: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
+000065c0: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000065e0: 636f 6e73 7472 6169 6e65 645f 636f 6c75  constrained_colu
+000065f0: 6d6e 7322 3a20 6c69 7374 2863 6f6c 7329  mns": list(cols)
+00006600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006610: 2020 226e 616d 6522 3a20 6e61 6d65 2c0a    "name": name,.
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2263 6f6d 6d65 6e74 223a 2063 6f6d 6d65  "comment": comme
+00006640: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00006650: 7d0a 0a20 2020 2020 2020 2065 6d70 7479  }..        empty
+00006660: 203d 2070 6b28 6e61 6d65 3d4e 6f6e 6529   = pk(name=None)
+00006670: 0a20 2020 2020 2020 2069 6620 7465 7374  .        if test
+00006680: 696e 672e 7265 7175 6972 6573 2e6d 6174  ing.requires.mat
+00006690: 6572 6961 6c69 7a65 645f 7669 6577 735f  erialized_views_
+000066a0: 7265 666c 6563 745f 706b 2e65 6e61 626c  reflect_pk.enabl
+000066b0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+000066c0: 6d61 7465 7269 616c 697a 6564 203d 207b  materialized = {
+000066d0: 2873 6368 656d 612c 2022 6469 6e67 616c  (schema, "dingal
+000066e0: 696e 6773 5f76 2229 3a20 706b 2822 6469  ings_v"): pk("di
+000066f0: 6e67 616c 696e 675f 6964 2229 7d0a 2020  ngaling_id")}.  
+00006700: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006710: 2020 2020 2020 2020 6d61 7465 7269 616c          material
+00006720: 697a 6564 203d 207b 2873 6368 656d 612c  ized = {(schema,
+00006730: 2022 6469 6e67 616c 696e 6773 5f76 2229   "dingalings_v")
+00006740: 3a20 656d 7074 797d 0a20 2020 2020 2020  : empty}.       
+00006750: 2076 6965 7773 203d 207b 0a20 2020 2020   views = {.     
+00006760: 2020 2020 2020 2028 7363 6865 6d61 2c20         (schema, 
+00006770: 2265 6d61 696c 5f61 6464 7265 7373 6573  "email_addresses
+00006780: 5f76 2229 3a20 656d 7074 792c 0a20 2020  _v"): empty,.   
+00006790: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
+000067a0: 2c20 2275 7365 7273 5f76 2229 3a20 656d  , "users_v"): em
+000067b0: 7074 792c 0a20 2020 2020 2020 2020 2020  pty,.           
+000067c0: 2028 7363 6865 6d61 2c20 2275 7365 725f   (schema, "user_
+000067d0: 746d 705f 7622 293a 2065 6d70 7479 2c0a  tmp_v"): empty,.
+000067e0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000067f0: 2020 7365 6c66 2e5f 7265 736f 6c76 655f    self._resolve_
+00006800: 7669 6577 7328 7669 6577 732c 206d 6174  views(views, mat
+00006810: 6572 6961 6c69 7a65 6429 0a20 2020 2020  erialized).     
+00006820: 2020 2074 6162 6c65 7320 3d20 7b0a 2020     tables = {.  
+00006830: 2020 2020 2020 2020 2020 2873 6368 656d            (schem
+00006840: 612c 2022 7573 6572 7322 293a 2070 6b28  a, "users"): pk(
+00006850: 2275 7365 725f 6964 2229 2c0a 2020 2020  "user_id"),.    
+00006860: 2020 2020 2020 2020 2873 6368 656d 612c          (schema,
+00006870: 2022 6469 6e67 616c 696e 6773 2229 3a20   "dingalings"): 
+00006880: 706b 2822 6469 6e67 616c 696e 675f 6964  pk("dingaling_id
+00006890: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+000068a0: 2873 6368 656d 612c 2022 656d 6169 6c5f  (schema, "email_
+000068b0: 6164 6472 6573 7365 7322 293a 2070 6b28  addresses"): pk(
+000068c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000068d0: 2022 6164 6472 6573 735f 6964 222c 206e   "address_id", n
+000068e0: 616d 653d 2265 6d61 696c 5f61 645f 706b  ame="email_ad_pk
+000068f0: 222c 2063 6f6d 6d65 6e74 3d22 6561 2070  ", comment="ea p
+00006900: 6b20 636f 6d6d 656e 7422 0a20 2020 2020  k comment".     
+00006910: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00006920: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
+00006930: 636f 6d6d 656e 745f 7465 7374 2229 3a20  comment_test"): 
+00006940: 706b 2822 6964 2229 2c0a 2020 2020 2020  pk("id"),.      
+00006950: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
+00006960: 6e6f 5f63 6f6e 7374 7261 696e 7473 2229  no_constraints")
+00006970: 3a20 656d 7074 792c 0a20 2020 2020 2020  : empty,.       
+00006980: 2020 2020 2028 7363 6865 6d61 2c20 226c       (schema, "l
+00006990: 6f63 616c 5f74 6162 6c65 2229 3a20 706b  ocal_table"): pk
+000069a0: 2822 6964 2229 2c0a 2020 2020 2020 2020  ("id"),.        
+000069b0: 2020 2020 2873 6368 656d 612c 2022 7265      (schema, "re
+000069c0: 6d6f 7465 5f74 6162 6c65 2229 3a20 706b  mote_table"): pk
+000069d0: 2822 6964 2229 2c0a 2020 2020 2020 2020  ("id"),.        
+000069e0: 2020 2020 2873 6368 656d 612c 2022 7265      (schema, "re
+000069f0: 6d6f 7465 5f74 6162 6c65 5f32 2229 3a20  mote_table_2"): 
+00006a00: 706b 2822 6964 2229 2c0a 2020 2020 2020  pk("id"),.      
+00006a10: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
+00006a20: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
+00006a30: 6e6f 706b 2229 3a20 706b 2822 6964 2229  nopk"): pk("id")
+00006a40: 2c0a 2020 2020 2020 2020 2020 2020 2873  ,.            (s
+00006a50: 6368 656d 612c 2022 6e6f 6e63 6f6c 5f69  chema, "noncol_i
+00006a60: 6478 5f74 6573 745f 706b 2229 3a20 706b  dx_test_pk"): pk
+00006a70: 2822 6964 2229 2c0a 2020 2020 2020 2020  ("id"),.        
+00006a80: 2020 2020 2873 6368 656d 612c 2073 656c      (schema, sel
+00006a90: 662e 7465 6d70 5f74 6162 6c65 5f6e 616d  f.temp_table_nam
+00006aa0: 6528 2929 3a20 706b 2822 6964 2229 2c0a  e()): pk("id"),.
+00006ab0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00006ac0: 2020 6966 206e 6f74 2074 6573 7469 6e67    if not testing
+00006ad0: 2e72 6571 7569 7265 732e 7265 666c 6563  .requires.reflec
+00006ae0: 7473 5f70 6b5f 6e61 6d65 732e 656e 6162  ts_pk_names.enab
+00006af0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+00006b00: 2066 6f72 2076 616c 2069 6e20 7461 626c   for val in tabl
+00006b10: 6573 2e76 616c 7565 7328 293a 0a20 2020  es.values():.   
+00006b20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006b30: 7661 6c5b 226e 616d 6522 5d20 6973 206e  val["name"] is n
+00006b40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00006b50: 2020 2020 2020 2020 2020 2020 2076 616c               val
+00006b60: 5b22 6e61 6d65 225d 203d 206d 6f63 6b2e  ["name"] = mock.
+00006b70: 414e 590a 2020 2020 2020 2020 7265 7320  ANY.        res 
+00006b80: 3d20 7365 6c66 2e5f 7265 736f 6c76 655f  = self._resolve_
+00006b90: 6b69 6e64 286b 696e 642c 2074 6162 6c65  kind(kind, table
+00006ba0: 732c 2076 6965 7773 2c20 6d61 7465 7269  s, views, materi
+00006bb0: 616c 697a 6564 290a 2020 2020 2020 2020  alized).        
+00006bc0: 7265 7320 3d20 7365 6c66 2e5f 7265 736f  res = self._reso
+00006bd0: 6c76 655f 6e61 6d65 7328 7363 6865 6d61  lve_names(schema
+00006be0: 2c20 7363 6f70 652c 2066 696c 7465 725f  , scope, filter_
+00006bf0: 6e61 6d65 732c 2072 6573 290a 2020 2020  names, res).    
+00006c00: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+00006c10: 2020 2020 4066 696c 7465 725f 6e61 6d65      @filter_name
+00006c20: 5f76 616c 7565 7328 290a 2020 2020 4074  _values().    @t
+00006c30: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00006c40: 7072 696d 6172 795f 6b65 795f 636f 6e73  primary_key_cons
+00006c50: 7472 6169 6e74 5f72 6566 6c65 6374 696f  traint_reflectio
+00006c60: 6e0a 2020 2020 6465 6620 7465 7374 5f67  n.    def test_g
+00006c70: 6574 5f6d 756c 7469 5f70 6b5f 636f 6e73  et_multi_pk_cons
+00006c80: 7472 6169 6e74 280a 2020 2020 2020 2020  traint(.        
+00006c90: 7365 6c66 2c0a 2020 2020 2020 2020 6765  self,.        ge
+00006ca0: 745f 6d75 6c74 695f 6578 702c 0a20 2020  t_multi_exp,.   
+00006cb0: 2020 2020 2075 7365 5f66 696c 7465 722c       use_filter,
+00006cc0: 0a20 2020 2020 2020 2073 6368 656d 613d  .        schema=
+00006cd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7363  None,.        sc
+00006ce0: 6f70 653d 4f62 6a65 6374 5363 6f70 652e  ope=ObjectScope.
+00006cf0: 4445 4641 554c 542c 0a20 2020 2020 2020  DEFAULT,.       
+00006d00: 206b 696e 643d 4f62 6a65 6374 4b69 6e64   kind=ObjectKind
+00006d10: 2e54 4142 4c45 2c0a 2020 2020 293a 0a20  .TABLE,.    ):. 
+00006d20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006d30: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+00006d40: 4944 453a 0a0a 2020 2020 2020 2020 5370  IDE:..        Sp
+00006d50: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+00006d60: 7070 6f72 7420 7465 6d70 6f72 6172 7920  pport temporary 
+00006d70: 7461 626c 6573 2c20 736f 2072 6561 6c20  tables, so real 
+00006d80: 7461 626c 6573 2061 7265 0a20 2020 2020  tables are.     
+00006d90: 2020 2075 7365 6420 666f 7220 7465 7374     used for test
+00006da0: 696e 672e 2041 7320 7468 6520 6f72 6967  ing. As the orig
+00006db0: 696e 616c 2074 6573 7420 6578 7065 6374  inal test expect
+00006dc0: 7320 6f6e 6c79 2072 6561 6c0a 2020 2020  s only real.    
+00006dd0: 2020 2020 7461 626c 6573 2074 6f20 6265      tables to be
+00006de0: 2072 6561 642c 2061 6e64 2069 6e20 5370   read, and in Sp
+00006df0: 616e 6e65 7220 616c 6c20 7468 6520 7461  anner all the ta
+00006e00: 626c 6573 2061 7265 2072 6561 6c2c 0a20  bles are real,. 
+00006e10: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
+00006e20: 7265 7375 6c74 7320 6f76 6572 7269 6465  results override
+00006e30: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
+00006e40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006e50: 2020 696e 7370 2c20 6b77 732c 2065 7870    insp, kws, exp
+00006e60: 203d 2067 6574 5f6d 756c 7469 5f65 7870   = get_multi_exp
+00006e70: 280a 2020 2020 2020 2020 2020 2020 7363  (.            sc
+00006e80: 6865 6d61 2c0a 2020 2020 2020 2020 2020  hema,.          
+00006e90: 2020 7363 6f70 652c 0a20 2020 2020 2020    scope,.       
+00006ea0: 2020 2020 206b 696e 642c 0a20 2020 2020       kind,.     
+00006eb0: 2020 2020 2020 2075 7365 5f66 696c 7465         use_filte
+00006ec0: 722c 0a20 2020 2020 2020 2020 2020 2049  r,.            I
+00006ed0: 6e73 7065 6374 6f72 2e67 6574 5f70 6b5f  nspector.get_pk_
+00006ee0: 636f 6e73 7472 6169 6e74 2c0a 2020 2020  constraint,.    
+00006ef0: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
+00006f00: 5f70 6b73 2c0a 2020 2020 2020 2020 290a  _pks,.        ).
+00006f10: 2020 2020 2020 2020 5f69 676e 6f72 655f          _ignore_
+00006f20: 7461 626c 6573 203d 205b 284e 6f6e 652c  tables = [(None,
+00006f30: 2022 6e6f 5f63 6f6e 7374 7261 696e 7473   "no_constraints
+00006f40: 2229 5d0a 2020 2020 2020 2020 6578 7020  ")].        exp 
+00006f50: 3d20 7b6b 3a20 7620 666f 7220 6b2c 2076  = {k: v for k, v
+00006f60: 2069 6e20 6578 702e 6974 656d 7328 2920   in exp.items() 
+00006f70: 6966 206b 206e 6f74 2069 6e20 5f69 676e  if k not in _ign
+00006f80: 6f72 655f 7461 626c 6573 7d0a 0a20 2020  ore_tables}..   
+00006f90: 2020 2020 2066 6f72 206b 7720 696e 206b       for kw in k
+00006fa0: 7773 3a0a 2020 2020 2020 2020 2020 2020  ws:.            
+00006fb0: 696e 7370 2e63 6c65 6172 5f63 6163 6865  insp.clear_cache
+00006fc0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+00006fd0: 6573 756c 7420 3d20 696e 7370 2e67 6574  esult = insp.get
+00006fe0: 5f6d 756c 7469 5f70 6b5f 636f 6e73 7472  _multi_pk_constr
+00006ff0: 6169 6e74 282a 2a6b 7729 0a20 2020 2020  aint(**kw).     
+00007000: 2020 2020 2020 2073 656c 662e 5f63 6865         self._che
+00007010: 636b 5f74 6162 6c65 5f64 6963 7428 7265  ck_table_dict(re
+00007020: 7375 6c74 2c20 6578 702c 2073 656c 662e  sult, exp, self.
+00007030: 5f72 6571 7569 7265 645f 706b 5f6b 6579  _required_pk_key
+00007040: 732c 206d 616b 655f 6c69 7374 733d 5472  s, make_lists=Tr
+00007050: 7565 290a 0a20 2020 2064 6566 2065 7870  ue)..    def exp
+00007060: 5f66 6b73 280a 2020 2020 2020 2020 7365  _fks(.        se
+00007070: 6c66 2c0a 2020 2020 2020 2020 7363 6865  lf,.        sche
+00007080: 6d61 3d4e 6f6e 652c 0a20 2020 2020 2020  ma=None,.       
+00007090: 2073 636f 7065 3d4f 626a 6563 7453 636f   scope=ObjectSco
+000070a0: 7065 2e41 4e59 2c0a 2020 2020 2020 2020  pe.ANY,.        
+000070b0: 6b69 6e64 3d4f 626a 6563 744b 696e 642e  kind=ObjectKind.
+000070c0: 414e 592c 0a20 2020 2020 2020 2066 696c  ANY,.        fil
+000070d0: 7465 725f 6e61 6d65 733d 4e6f 6e65 2c0a  ter_names=None,.
+000070e0: 2020 2020 293a 0a20 2020 2020 2020 2063      ):.        c
+000070f0: 6c61 7373 2074 743a 0a20 2020 2020 2020  lass tt:.       
+00007100: 2020 2020 2064 6566 205f 5f65 715f 5f28       def __eq__(
+00007110: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+00007120: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00007130: 7475 726e 206f 7468 6572 2069 7320 4e6f  turn other is No
+00007140: 6e65 206f 7220 636f 6e66 6967 2e64 622e  ne or config.db.
+00007150: 6469 616c 6563 742e 6465 6661 756c 745f  dialect.default_
+00007160: 7363 6865 6d61 5f6e 616d 6520 3d3d 206f  schema_name == o
+00007170: 7468 6572 0a0a 2020 2020 2020 2020 6465  ther..        de
+00007180: 6620 666b 280a 2020 2020 2020 2020 2020  f fk(.          
+00007190: 2020 636f 6c73 2c0a 2020 2020 2020 2020    cols,.        
+000071a0: 2020 2020 7265 665f 636f 6c2c 0a20 2020      ref_col,.   
+000071b0: 2020 2020 2020 2020 2072 6566 5f74 6162           ref_tab
+000071c0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+000071d0: 7265 665f 7363 6865 6d61 3d73 6368 656d  ref_schema=schem
+000071e0: 612c 0a20 2020 2020 2020 2020 2020 206e  a,.            n
+000071f0: 616d 653d 6d6f 636b 2e41 4e59 2c0a 2020  ame=mock.ANY,.  
+00007200: 2020 2020 2020 2020 2020 636f 6d6d 656e            commen
+00007210: 743d 4e6f 6e65 2c0a 2020 2020 2020 2020  t=None,.        
+00007220: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00007230: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+00007240: 2020 2020 2020 2020 2263 6f6e 7374 7261          "constra
+00007250: 696e 6564 5f63 6f6c 756d 6e73 223a 2063  ined_columns": c
+00007260: 6f6c 732c 0a20 2020 2020 2020 2020 2020  ols,.           
+00007270: 2020 2020 2022 7265 6665 7272 6564 5f63       "referred_c
+00007280: 6f6c 756d 6e73 223a 2072 6566 5f63 6f6c  olumns": ref_col
+00007290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000072a0: 2020 226e 616d 6522 3a20 6e61 6d65 2c0a    "name": name,.
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072c0: 226f 7074 696f 6e73 223a 206d 6f63 6b2e  "options": mock.
+000072d0: 414e 592c 0a20 2020 2020 2020 2020 2020  ANY,.           
+000072e0: 2020 2020 2022 7265 6665 7272 6564 5f73       "referred_s
+000072f0: 6368 656d 6122 3a20 7265 665f 7363 6865  chema": ref_sche
+00007300: 6d61 2069 6620 7265 665f 7363 6865 6d61  ma if ref_schema
+00007310: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+00007320: 6520 7474 2829 2c0a 2020 2020 2020 2020  e tt(),.        
+00007330: 2020 2020 2020 2020 2272 6566 6572 7265          "referre
+00007340: 645f 7461 626c 6522 3a20 7265 665f 7461  d_table": ref_ta
+00007350: 626c 652c 0a20 2020 2020 2020 2020 2020  ble,.           
+00007360: 2020 2020 2022 636f 6d6d 656e 7422 3a20       "comment": 
+00007370: 636f 6d6d 656e 742c 0a20 2020 2020 2020  comment,.       
+00007380: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00007390: 6d61 7465 7269 616c 697a 6564 203d 207b  materialized = {
+000073a0: 7d0a 2020 2020 2020 2020 7669 6577 7320  }.        views 
+000073b0: 3d20 7b7d 0a20 2020 2020 2020 2073 656c  = {}.        sel
+000073c0: 662e 5f72 6573 6f6c 7665 5f76 6965 7773  f._resolve_views
+000073d0: 2876 6965 7773 2c20 6d61 7465 7269 616c  (views, material
+000073e0: 697a 6564 290a 2020 2020 2020 2020 7461  ized).        ta
+000073f0: 626c 6573 203d 207b 0a20 2020 2020 2020  bles = {.       
+00007400: 2020 2020 2028 7363 6865 6d61 2c20 2275       (schema, "u
+00007410: 7365 7273 2229 3a20 5b0a 2020 2020 2020  sers"): [.      
+00007420: 2020 2020 2020 2020 2020 666b 285b 2270            fk(["p
+00007430: 6172 656e 745f 7573 6572 5f69 6422 5d2c  arent_user_id"],
+00007440: 205b 2275 7365 725f 6964 225d 2c20 2275   ["user_id"], "u
+00007450: 7365 7273 222c 206e 616d 653d 2275 7365  sers", name="use
+00007460: 725f 6964 5f66 6b22 290a 2020 2020 2020  r_id_fk").      
+00007470: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00007480: 2020 2020 2028 7363 6865 6d61 2c20 2264       (schema, "d
+00007490: 696e 6761 6c69 6e67 7322 293a 205b 0a20  ingalings"): [. 
+000074a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000074b0: 6b28 5b22 6164 6472 6573 735f 6964 225d  k(["address_id"]
+000074c0: 2c20 5b22 6164 6472 6573 735f 6964 225d  , ["address_id"]
+000074d0: 2c20 2265 6d61 696c 5f61 6464 7265 7373  , "email_address
+000074e0: 6573 2229 2c0a 2020 2020 2020 2020 2020  es"),.          
+000074f0: 2020 2020 2020 666b 285b 2269 645f 7573        fk(["id_us
+00007500: 6572 225d 2c20 5b22 7573 6572 5f69 6422  er"], ["user_id"
+00007510: 5d2c 2022 7573 6572 7322 292c 0a20 2020  ], "users"),.   
+00007520: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00007530: 2020 2020 2020 2020 2873 6368 656d 612c          (schema,
+00007540: 2022 656d 6169 6c5f 6164 6472 6573 7365   "email_addresse
+00007550: 7322 293a 205b 666b 285b 2272 656d 6f74  s"): [fk(["remot
+00007560: 655f 7573 6572 5f69 6422 5d2c 205b 2275  e_user_id"], ["u
+00007570: 7365 725f 6964 225d 2c20 2275 7365 7273  ser_id"], "users
+00007580: 2229 5d2c 0a20 2020 2020 2020 2020 2020  ")],.           
+00007590: 2028 7363 6865 6d61 2c20 226c 6f63 616c   (schema, "local
+000075a0: 5f74 6162 6c65 2229 3a20 5b0a 2020 2020  _table"): [.    
+000075b0: 2020 2020 2020 2020 2020 2020 666b 280a              fk(.
+000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075d0: 2020 2020 5b22 7265 6d6f 7465 5f69 6422      ["remote_id"
+000075e0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000075f0: 2020 2020 2020 205b 2269 6422 5d2c 0a20         ["id"],. 
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 2020 2022 7265 6d6f 7465 5f74 6162 6c65     "remote_table
+00007620: 5f32 222c 0a20 2020 2020 2020 2020 2020  _2",.           
+00007630: 2020 2020 2020 2020 2072 6566 5f73 6368           ref_sch
+00007640: 656d 613d 636f 6e66 6967 2e74 6573 745f  ema=config.test_
+00007650: 7363 6865 6d61 2c0a 2020 2020 2020 2020  schema,.        
+00007660: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00007670: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00007680: 2020 2020 2028 7363 6865 6d61 2c20 2272       (schema, "r
+00007690: 656d 6f74 655f 7461 626c 6522 293a 205b  emote_table"): [
+000076a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000076b0: 2066 6b28 5b22 6c6f 6361 6c5f 6964 225d   fk(["local_id"]
+000076c0: 2c20 5b22 6964 225d 2c20 226c 6f63 616c  , ["id"], "local
+000076d0: 5f74 6162 6c65 222c 2072 6566 5f73 6368  _table", ref_sch
+000076e0: 656d 613d 4e6f 6e65 290a 2020 2020 2020  ema=None).      
+000076f0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00007700: 207d 0a20 2020 2020 2020 2069 6620 6e6f   }.        if no
+00007710: 7420 7465 7374 696e 672e 7265 7175 6972  t testing.requir
+00007720: 6573 2e73 656c 665f 7265 6665 7265 6e74  es.self_referent
+00007730: 6961 6c5f 666f 7265 6967 6e5f 6b65 7973  ial_foreign_keys
+00007740: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
+00007750: 2020 2020 2020 7461 626c 6573 5b28 7363        tables[(sc
+00007760: 6865 6d61 2c20 2275 7365 7273 2229 5d2e  hema, "users")].
+00007770: 636c 6561 7228 290a 2020 2020 2020 2020  clear().        
+00007780: 6966 206e 6f74 2074 6573 7469 6e67 2e72  if not testing.r
+00007790: 6571 7569 7265 732e 6e61 6d65 645f 636f  equires.named_co
+000077a0: 6e73 7472 6169 6e74 732e 656e 6162 6c65  nstraints.enable
+000077b0: 643a 0a20 2020 2020 2020 2020 2020 2066  d:.            f
+000077c0: 6f72 2076 616c 7320 696e 2074 6162 6c65  or vals in table
+000077d0: 732e 7661 6c75 6573 2829 3a0a 2020 2020  s.values():.    
+000077e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000077f0: 7661 6c20 696e 2076 616c 733a 0a20 2020  val in vals:.   
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007810: 2069 6620 7661 6c5b 226e 616d 6522 5d20   if val["name"] 
+00007820: 6973 206e 6f74 206d 6f63 6b2e 414e 593a  is not mock.ANY:
+00007830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007840: 2020 2020 2020 2020 2076 616c 5b22 6e61           val["na
+00007850: 6d65 225d 203d 206d 6f63 6b2e 414e 590a  me"] = mock.ANY.
+00007860: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
+00007870: 656c 662e 5f72 6573 6f6c 7665 5f6b 696e  elf._resolve_kin
+00007880: 6428 6b69 6e64 2c20 7461 626c 6573 2c20  d(kind, tables, 
+00007890: 7669 6577 732c 206d 6174 6572 6961 6c69  views, materiali
+000078a0: 7a65 6429 0a20 2020 2020 2020 2072 6573  zed).        res
+000078b0: 203d 2073 656c 662e 5f72 6573 6f6c 7665   = self._resolve
+000078c0: 5f6e 616d 6573 2873 6368 656d 612c 2073  _names(schema, s
+000078d0: 636f 7065 2c20 6669 6c74 6572 5f6e 616d  cope, filter_nam
+000078e0: 6573 2c20 7265 7329 0a20 2020 2020 2020  es, res).       
+000078f0: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
+00007900: 2040 6669 6c74 6572 5f6e 616d 655f 7661   @filter_name_va
+00007910: 6c75 6573 2829 0a20 2020 2040 7465 7374  lues().    @test
+00007920: 696e 672e 7265 7175 6972 6573 2e66 6f72  ing.requires.for
+00007930: 6569 676e 5f6b 6579 5f63 6f6e 7374 7261  eign_key_constra
+00007940: 696e 745f 7265 666c 6563 7469 6f6e 0a20  int_reflection. 
+00007950: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
+00007960: 6d75 6c74 695f 666f 7265 6967 6e5f 6b65  multi_foreign_ke
+00007970: 7973 280a 2020 2020 2020 2020 7365 6c66  ys(.        self
+00007980: 2c0a 2020 2020 2020 2020 6765 745f 6d75  ,.        get_mu
+00007990: 6c74 695f 6578 702c 0a20 2020 2020 2020  lti_exp,.       
+000079a0: 2075 7365 5f66 696c 7465 722c 0a20 2020   use_filter,.   
+000079b0: 2020 2020 2073 6368 656d 613d 4e6f 6e65       schema=None
+000079c0: 2c0a 2020 2020 2020 2020 7363 6f70 653d  ,.        scope=
+000079d0: 4f62 6a65 6374 5363 6f70 652e 4445 4641  ObjectScope.DEFA
+000079e0: 554c 542c 0a20 2020 2020 2020 206b 696e  ULT,.        kin
+000079f0: 643d 4f62 6a65 6374 4b69 6e64 2e54 4142  d=ObjectKind.TAB
+00007a00: 4c45 2c0a 2020 2020 293a 0a0a 2020 2020  LE,.    ):..    
+00007a10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007a20: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+00007a30: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
+00007a40: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+00007a50: 7274 2074 656d 706f 7261 7279 2074 6162  rt temporary tab
+00007a60: 6c65 732c 2073 6f20 7265 616c 2074 6162  les, so real tab
+00007a70: 6c65 7320 6172 650a 2020 2020 2020 2020  les are.        
+00007a80: 7573 6564 2066 6f72 2074 6573 7469 6e67  used for testing
+00007a90: 2e20 4173 2074 6865 206f 7269 6769 6e61  . As the origina
+00007aa0: 6c20 7465 7374 2065 7870 6563 7473 206f  l test expects o
+00007ab0: 6e6c 7920 7265 616c 0a20 2020 2020 2020  nly real.       
+00007ac0: 2074 6162 6c65 7320 746f 2062 6520 7265   tables to be re
+00007ad0: 6164 2c20 616e 6420 696e 2053 7061 6e6e  ad, and in Spann
+00007ae0: 6572 2061 6c6c 2074 6865 2074 6162 6c65  er all the table
+00007af0: 7320 6172 6520 7265 616c 2c0a 2020 2020  s are real,.    
+00007b00: 2020 2020 6578 7065 6374 6564 2072 6573      expected res
+00007b10: 756c 7473 206f 7665 7272 6964 6520 6973  ults override is
+00007b20: 2072 6571 7569 7265 642e 0a20 2020 2020   required..     
+00007b30: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00007b40: 6e73 702c 206b 7773 2c20 6578 7020 3d20  nsp, kws, exp = 
+00007b50: 6765 745f 6d75 6c74 695f 6578 7028 0a20  get_multi_exp(. 
+00007b60: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+00007b70: 612c 0a20 2020 2020 2020 2020 2020 2073  a,.            s
+00007b80: 636f 7065 2c0a 2020 2020 2020 2020 2020  cope,.          
+00007b90: 2020 6b69 6e64 2c0a 2020 2020 2020 2020    kind,.        
+00007ba0: 2020 2020 7573 655f 6669 6c74 6572 2c0a      use_filter,.
+00007bb0: 2020 2020 2020 2020 2020 2020 496e 7370              Insp
+00007bc0: 6563 746f 722e 6765 745f 666f 7265 6967  ector.get_foreig
+00007bd0: 6e5f 6b65 7973 2c0a 2020 2020 2020 2020  n_keys,.        
+00007be0: 2020 2020 7365 6c66 2e65 7870 5f66 6b73      self.exp_fks
+00007bf0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00007c00: 2020 2020 666f 7220 6b77 2069 6e20 6b77      for kw in kw
+00007c10: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00007c20: 6e73 702e 636c 6561 725f 6361 6368 6528  nsp.clear_cache(
+00007c30: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007c40: 7375 6c74 203d 2069 6e73 702e 6765 745f  sult = insp.get_
+00007c50: 6d75 6c74 695f 666f 7265 6967 6e5f 6b65  multi_foreign_ke
+00007c60: 7973 282a 2a6b 7729 0a20 2020 2020 2020  ys(**kw).       
+00007c70: 2020 2020 2073 656c 662e 5f61 646a 7573       self._adjus
+00007c80: 745f 736f 7274 2872 6573 756c 742c 2065  t_sort(result, e
+00007c90: 7870 2c20 6c61 6d62 6461 2064 3a20 7475  xp, lambda d: tu
+00007ca0: 706c 6528 645b 2263 6f6e 7374 7261 696e  ple(d["constrain
+00007cb0: 6564 5f63 6f6c 756d 6e73 225d 2929 0a20  ed_columns"])). 
+00007cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007cd0: 5f63 6865 636b 5f74 6162 6c65 5f64 6963  _check_table_dic
+00007ce0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00007cf0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00007d00: 2020 2020 2020 2020 206b 6579 3a20 736f           key: so
+00007d10: 7274 6564 2876 616c 7565 2c20 6b65 793d  rted(value, key=
+00007d20: 6c61 6d62 6461 2078 3a20 785b 2263 6f6e  lambda x: x["con
+00007d30: 7374 7261 696e 6564 5f63 6f6c 756d 6e73  strained_columns
+00007d40: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
+00007d50: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
+00007d60: 2076 616c 7565 2069 6e20 7265 7375 6c74   value in result
+00007d70: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
+00007d80: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00007d90: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007db0: 2020 6b65 793a 2073 6f72 7465 6428 7661    key: sorted(va
+00007dc0: 6c75 652c 206b 6579 3d6c 616d 6264 6120  lue, key=lambda 
+00007dd0: 783a 2078 5b22 636f 6e73 7472 6169 6e65  x: x["constraine
+00007de0: 645f 636f 6c75 6d6e 7322 5d29 0a20 2020  d_columns"]).   
+00007df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e00: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00007e10: 696e 2065 7870 2e69 7465 6d73 2829 0a20  in exp.items(). 
+00007e20: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00007e30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007e40: 2020 7365 6c66 2e5f 7265 7175 6972 6564    self._required
+00007e50: 5f66 6b5f 6b65 7973 2c0a 2020 2020 2020  _fk_keys,.      
+00007e60: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00007e70: 2065 7870 5f63 6f6c 756d 6e73 280a 2020   exp_columns(.  
+00007e80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00007e90: 2020 2020 7363 6865 6d61 3d4e 6f6e 652c      schema=None,
+00007ea0: 0a20 2020 2020 2020 2073 636f 7065 3d4f  .        scope=O
+00007eb0: 626a 6563 7453 636f 7065 2e41 4e59 2c0a  bjectScope.ANY,.
+00007ec0: 2020 2020 2020 2020 6b69 6e64 3d4f 626a          kind=Obj
+00007ed0: 6563 744b 696e 642e 414e 592c 0a20 2020  ectKind.ANY,.   
+00007ee0: 2020 2020 2066 696c 7465 725f 6e61 6d65       filter_name
+00007ef0: 733d 4e6f 6e65 2c0a 2020 2020 293a 0a20  s=None,.    ):. 
+00007f00: 2020 2020 2020 2064 6566 2063 6f6c 286e         def col(n
+00007f10: 616d 652c 2061 7574 6f3d 4661 6c73 652c  ame, auto=False,
+00007f20: 2064 6566 6175 6c74 3d6d 6f63 6b2e 414e   default=mock.AN
+00007f30: 592c 2063 6f6d 6d65 6e74 3d4e 6f6e 652c  Y, comment=None,
+00007f40: 206e 756c 6c61 626c 653d 5472 7565 293a   nullable=True):
+00007f50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00007f60: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00007f70: 2020 2020 2022 6e61 6d65 223a 206e 616d       "name": nam
+00007f80: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00007f90: 2020 2022 6175 746f 696e 6372 656d 656e     "autoincremen
+00007fa0: 7422 3a20 6175 746f 2c0a 2020 2020 2020  t": auto,.      
+00007fb0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00007fc0: 3a20 6d6f 636b 2e41 4e59 2c0a 2020 2020  : mock.ANY,.    
+00007fd0: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+00007fe0: 6175 6c74 223a 2064 6566 6175 6c74 2c0a  ault": default,.
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008000: 2263 6f6d 6d65 6e74 223a 2063 6f6d 6d65  "comment": comme
+00008010: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00008020: 2020 2020 226e 756c 6c61 626c 6522 3a20      "nullable": 
+00008030: 6e75 6c6c 6162 6c65 2c0a 2020 2020 2020  nullable,.      
+00008040: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00008050: 2020 2020 6966 2061 7574 6f20 3d3d 2022      if auto == "
+00008060: 6f6d 6974 223a 0a20 2020 2020 2020 2020  omit":.         
+00008070: 2020 2020 2020 2072 6573 2e70 6f70 2822         res.pop("
+00008080: 6175 746f 696e 6372 656d 656e 7422 290a  autoincrement").
+00008090: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000080a0: 726e 2072 6573 0a0a 2020 2020 2020 2020  rn res..        
+000080b0: 6465 6620 706b 286e 616d 652c 202a 2a6b  def pk(name, **k
+000080c0: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
+000080d0: 6b77 203d 207b 2261 7574 6f22 3a20 5472  kw = {"auto": Tr
+000080e0: 7565 2c20 2264 6566 6175 6c74 223a 206d  ue, "default": m
+000080f0: 6f63 6b2e 414e 592c 2022 6e75 6c6c 6162  ock.ANY, "nullab
+00008100: 6c65 223a 2046 616c 7365 2c20 2a2a 6b77  le": False, **kw
+00008110: 7d0a 2020 2020 2020 2020 2020 2020 7265  }.            re
+00008120: 7475 726e 2063 6f6c 286e 616d 652c 202a  turn col(name, *
+00008130: 2a6b 7729 0a0a 2020 2020 2020 2020 6d61  *kw)..        ma
+00008140: 7465 7269 616c 697a 6564 203d 207b 0a20  terialized = {. 
+00008150: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
+00008160: 6d61 2c20 2264 696e 6761 6c69 6e67 735f  ma, "dingalings_
+00008170: 7622 293a 205b 0a20 2020 2020 2020 2020  v"): [.         
+00008180: 2020 2020 2020 2063 6f6c 2822 6469 6e67         col("ding
+00008190: 616c 696e 675f 6964 222c 2061 7574 6f3d  aling_id", auto=
+000081a0: 226f 6d69 7422 2c20 6e75 6c6c 6162 6c65  "omit", nullable
+000081b0: 3d6d 6f63 6b2e 414e 5929 2c0a 2020 2020  =mock.ANY),.    
+000081c0: 2020 2020 2020 2020 2020 2020 636f 6c28              col(
+000081d0: 2261 6464 7265 7373 5f69 6422 292c 0a20  "address_id"),. 
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000081f0: 6f6c 2822 6964 5f75 7365 7222 292c 0a20  ol("id_user"),. 
+00008200: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008210: 6f6c 2822 6461 7461 2229 2c0a 2020 2020  ol("data"),.    
+00008220: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00008230: 2020 7d0a 2020 2020 2020 2020 7669 6577    }.        view
+00008240: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+00008250: 2020 2873 6368 656d 612c 2022 656d 6169    (schema, "emai
+00008260: 6c5f 6164 6472 6573 7365 735f 7622 293a  l_addresses_v"):
+00008270: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00008280: 2020 2063 6f6c 2822 6164 6472 6573 735f     col("address_
+00008290: 6964 222c 2061 7574 6f3d 226f 6d69 7422  id", auto="omit"
+000082a0: 2c20 6e75 6c6c 6162 6c65 3d6d 6f63 6b2e  , nullable=mock.
+000082b0: 414e 5929 2c0a 2020 2020 2020 2020 2020  ANY),.          
+000082c0: 2020 2020 2020 636f 6c28 2272 656d 6f74        col("remot
+000082d0: 655f 7573 6572 5f69 6422 292c 0a20 2020  e_user_id"),.   
+000082e0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+000082f0: 2822 656d 6169 6c5f 6164 6472 6573 7322  ("email_address"
+00008300: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
+00008310: 2c0a 2020 2020 2020 2020 2020 2020 2873  ,.            (s
+00008320: 6368 656d 612c 2022 7573 6572 735f 7622  chema, "users_v"
+00008330: 293a 205b 0a20 2020 2020 2020 2020 2020  ): [.           
+00008340: 2020 2020 2063 6f6c 2822 7573 6572 5f69       col("user_i
+00008350: 6422 2c20 6175 746f 3d22 6f6d 6974 222c  d", auto="omit",
+00008360: 206e 756c 6c61 626c 653d 6d6f 636b 2e41   nullable=mock.A
+00008370: 4e59 292c 0a20 2020 2020 2020 2020 2020  NY),.           
+00008380: 2020 2020 2063 6f6c 2822 7465 7374 3122       col("test1"
+00008390: 2c20 6e75 6c6c 6162 6c65 3d6d 6f63 6b2e  , nullable=mock.
+000083a0: 414e 5929 2c0a 2020 2020 2020 2020 2020  ANY),.          
+000083b0: 2020 2020 2020 636f 6c28 2274 6573 7432        col("test2
+000083c0: 222c 206e 756c 6c61 626c 653d 6d6f 636b  ", nullable=mock
+000083d0: 2e41 4e59 292c 0a20 2020 2020 2020 2020  .ANY),.         
+000083e0: 2020 2020 2020 2063 6f6c 2822 7061 7265         col("pare
+000083f0: 6e74 5f75 7365 725f 6964 2229 2c0a 2020  nt_user_id"),.  
+00008400: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00008410: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
+00008420: 2c20 2275 7365 725f 746d 705f 7622 293a  , "user_tmp_v"):
+00008430: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00008440: 2020 2063 6f6c 2822 6964 222c 2061 7574     col("id", aut
+00008450: 6f3d 226f 6d69 7422 2c20 6e75 6c6c 6162  o="omit", nullab
+00008460: 6c65 3d6d 6f63 6b2e 414e 5929 2c0a 2020  le=mock.ANY),.  
+00008470: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00008480: 6c28 226e 616d 6522 292c 0a20 2020 2020  l("name"),.     
+00008490: 2020 2020 2020 2020 2020 2063 6f6c 2822             col("
+000084a0: 666f 6f22 292c 0a20 2020 2020 2020 2020  foo"),.         
+000084b0: 2020 205d 2c0a 2020 2020 2020 2020 7d0a     ],.        }.
+000084c0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+000084d0: 736f 6c76 655f 7669 6577 7328 7669 6577  solve_views(view
+000084e0: 732c 206d 6174 6572 6961 6c69 7a65 6429  s, materialized)
+000084f0: 0a20 2020 2020 2020 2074 6162 6c65 7320  .        tables 
+00008500: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00008510: 2873 6368 656d 612c 2022 7573 6572 7322  (schema, "users"
+00008520: 293a 205b 0a20 2020 2020 2020 2020 2020  ): [.           
+00008530: 2020 2020 2070 6b28 2275 7365 725f 6964       pk("user_id
+00008540: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00008550: 2020 2020 636f 6c28 2274 6573 7431 222c      col("test1",
+00008560: 206e 756c 6c61 626c 653d 4661 6c73 6529   nullable=False)
+00008570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008580: 2020 636f 6c28 2274 6573 7432 222c 206e    col("test2", n
+00008590: 756c 6c61 626c 653d 4661 6c73 6529 2c0a  ullable=False),.
+000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085b0: 636f 6c28 2270 6172 656e 745f 7573 6572  col("parent_user
+000085c0: 5f69 6422 292c 0a20 2020 2020 2020 2020  _id"),.         
+000085d0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+000085e0: 2020 2873 6368 656d 612c 2022 6469 6e67    (schema, "ding
+000085f0: 616c 696e 6773 2229 3a20 5b0a 2020 2020  alings"): [.    
+00008600: 2020 2020 2020 2020 2020 2020 706b 2822              pk("
+00008610: 6469 6e67 616c 696e 675f 6964 2229 2c0a  dingaling_id"),.
+00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008630: 636f 6c28 2261 6464 7265 7373 5f69 6422  col("address_id"
+00008640: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008650: 2020 2063 6f6c 2822 6964 5f75 7365 7222     col("id_user"
+00008660: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008670: 2020 2063 6f6c 2822 6461 7461 2229 2c0a     col("data"),.
+00008680: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00008690: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
+000086a0: 6d61 2c20 2265 6d61 696c 5f61 6464 7265  ma, "email_addre
+000086b0: 7373 6573 2229 3a20 5b0a 2020 2020 2020  sses"): [.      
+000086c0: 2020 2020 2020 2020 2020 706b 2822 6164            pk("ad
+000086d0: 6472 6573 735f 6964 2229 2c0a 2020 2020  dress_id"),.    
+000086e0: 2020 2020 2020 2020 2020 2020 636f 6c28              col(
+000086f0: 2272 656d 6f74 655f 7573 6572 5f69 6422  "remote_user_id"
+00008700: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008710: 2020 2063 6f6c 2822 656d 6169 6c5f 6164     col("email_ad
+00008720: 6472 6573 7322 292c 0a20 2020 2020 2020  dress"),.       
+00008730: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00008740: 2020 2020 2873 6368 656d 612c 2022 636f      (schema, "co
+00008750: 6d6d 656e 745f 7465 7374 2229 3a20 5b0a  mment_test"): [.
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 706b 2822 6964 222c 2063 6f6d 6d65 6e74  pk("id", comment
+00008780: 3d22 6964 2063 6f6d 6d65 6e74 2229 2c0a  ="id comment"),.
+00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087a0: 636f 6c28 2264 6174 6122 2c20 636f 6d6d  col("data", comm
+000087b0: 656e 743d 2264 6174 6120 2520 636f 6d6d  ent="data % comm
+000087c0: 656e 7422 292c 0a20 2020 2020 2020 2020  ent"),.         
+000087d0: 2020 2020 2020 2063 6f6c 280a 2020 2020         col(.    
+000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087f0: 2264 3222 2c0a 2020 2020 2020 2020 2020  "d2",.          
+00008800: 2020 2020 2020 2020 2020 636f 6d6d 656e            commen
+00008810: 743d 7222 2222 436f 6d6d 656e 7420 7479  t=r"""Comment ty
+00008820: 7065 7320 7479 7065 2073 7065 6564 696c  pes type speedil
+00008830: 7920 2720 2220 5c20 2727 2046 756e 2122  y ' " \ '' Fun!"
+00008840: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00008850: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00008860: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+00008870: 2020 2873 6368 656d 612c 2022 6e6f 5f63    (schema, "no_c
+00008880: 6f6e 7374 7261 696e 7473 2229 3a20 5b63  onstraints"): [c
+00008890: 6f6c 2822 6461 7461 2229 5d2c 0a20 2020  ol("data")],.   
+000088a0: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
+000088b0: 2c20 226c 6f63 616c 5f74 6162 6c65 2229  , "local_table")
+000088c0: 3a20 5b70 6b28 2269 6422 292c 2063 6f6c  : [pk("id"), col
+000088d0: 2822 6461 7461 2229 2c20 636f 6c28 2272  ("data"), col("r
+000088e0: 656d 6f74 655f 6964 2229 5d2c 0a20 2020  emote_id")],.   
+000088f0: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
+00008900: 2c20 2272 656d 6f74 655f 7461 626c 6522  , "remote_table"
+00008910: 293a 205b 706b 2822 6964 2229 2c20 636f  ): [pk("id"), co
+00008920: 6c28 226c 6f63 616c 5f69 6422 292c 2063  l("local_id"), c
+00008930: 6f6c 2822 6461 7461 2229 5d2c 0a20 2020  ol("data")],.   
+00008940: 2020 2020 2020 2020 2028 7363 6865 6d61           (schema
+00008950: 2c20 2272 656d 6f74 655f 7461 626c 655f  , "remote_table_
+00008960: 3222 293a 205b 706b 2822 6964 2229 2c20  2"): [pk("id"), 
+00008970: 636f 6c28 2264 6174 6122 295d 2c0a 2020  col("data")],.  
+00008980: 2020 2020 2020 2020 2020 2873 6368 656d            (schem
+00008990: 612c 2022 6e6f 6e63 6f6c 5f69 6478 5f74  a, "noncol_idx_t
+000089a0: 6573 745f 6e6f 706b 2229 3a20 5b70 6b28  est_nopk"): [pk(
+000089b0: 2269 6422 292c 2063 6f6c 2822 7122 295d  "id"), col("q")]
+000089c0: 2c0a 2020 2020 2020 2020 2020 2020 2873  ,.            (s
+000089d0: 6368 656d 612c 2022 6e6f 6e63 6f6c 5f69  chema, "noncol_i
+000089e0: 6478 5f74 6573 745f 706b 2229 3a20 5b70  dx_test_pk"): [p
+000089f0: 6b28 2269 6422 292c 2063 6f6c 2822 7122  k("id"), col("q"
+00008a00: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+00008a10: 2873 6368 656d 612c 2073 656c 662e 7465  (schema, self.te
+00008a20: 6d70 5f74 6162 6c65 5f6e 616d 6528 2929  mp_table_name())
+00008a30: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00008a40: 2020 2020 706b 2822 6964 2229 2c0a 2020      pk("id"),.  
+00008a50: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00008a60: 6c28 226e 616d 6522 292c 0a20 2020 2020  l("name"),.     
+00008a70: 2020 2020 2020 2020 2020 2063 6f6c 2822             col("
+00008a80: 666f 6f22 292c 0a20 2020 2020 2020 2020  foo"),.         
+00008a90: 2020 205d 2c0a 2020 2020 2020 2020 7d0a     ],.        }.
+00008aa0: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+00008ab0: 6c66 2e5f 7265 736f 6c76 655f 6b69 6e64  lf._resolve_kind
+00008ac0: 286b 696e 642c 2074 6162 6c65 732c 2076  (kind, tables, v
+00008ad0: 6965 7773 2c20 6d61 7465 7269 616c 697a  iews, materializ
+00008ae0: 6564 290a 2020 2020 2020 2020 7265 7320  ed).        res 
+00008af0: 3d20 7365 6c66 2e5f 7265 736f 6c76 655f  = self._resolve_
+00008b00: 6e61 6d65 7328 7363 6865 6d61 2c20 7363  names(schema, sc
+00008b10: 6f70 652c 2066 696c 7465 725f 6e61 6d65  ope, filter_name
+00008b20: 732c 2072 6573 290a 2020 2020 2020 2020  s, res).        
+00008b30: 7265 7475 726e 2072 6573 0a0a 2020 2020  return res..    
+00008b40: 4066 696c 7465 725f 6e61 6d65 5f76 616c  @filter_name_val
+00008b50: 7565 7328 290a 2020 2020 6465 6620 7465  ues().    def te
+00008b60: 7374 5f67 6574 5f6d 756c 7469 5f63 6f6c  st_get_multi_col
+00008b70: 756d 6e73 280a 2020 2020 2020 2020 7365  umns(.        se
+00008b80: 6c66 2c0a 2020 2020 2020 2020 6765 745f  lf,.        get_
+00008b90: 6d75 6c74 695f 6578 702c 0a20 2020 2020  multi_exp,.     
+00008ba0: 2020 2075 7365 5f66 696c 7465 722c 0a20     use_filter,. 
+00008bb0: 2020 2020 2020 2073 6368 656d 613d 4e6f         schema=No
+00008bc0: 6e65 2c0a 2020 2020 2020 2020 7363 6f70  ne,.        scop
+00008bd0: 653d 4f62 6a65 6374 5363 6f70 652e 4445  e=ObjectScope.DE
+00008be0: 4641 554c 542c 0a20 2020 2020 2020 206b  FAULT,.        k
+00008bf0: 696e 643d 4f62 6a65 6374 4b69 6e64 2e54  ind=ObjectKind.T
+00008c00: 4142 4c45 2c0a 2020 2020 293a 0a20 2020  ABLE,.    ):.   
+00008c10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00008c20: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+00008c30: 453a 0a0a 2020 2020 2020 2020 5370 616e  E:..        Span
+00008c40: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+00008c50: 6f72 7420 7465 6d70 6f72 6172 7920 7461  ort temporary ta
+00008c60: 626c 6573 2c20 736f 2072 6561 6c20 7461  bles, so real ta
+00008c70: 626c 6573 2061 7265 0a20 2020 2020 2020  bles are.       
+00008c80: 2075 7365 6420 666f 7220 7465 7374 696e   used for testin
+00008c90: 672e 2041 7320 7468 6520 6f72 6967 696e  g. As the origin
+00008ca0: 616c 2074 6573 7420 6578 7065 6374 7320  al test expects 
+00008cb0: 6f6e 6c79 2072 6561 6c0a 2020 2020 2020  only real.      
+00008cc0: 2020 7461 626c 6573 2074 6f20 6265 2072    tables to be r
+00008cd0: 6561 642c 2061 6e64 2069 6e20 5370 616e  ead, and in Span
+00008ce0: 6e65 7220 616c 6c20 7468 6520 7461 626c  ner all the tabl
+00008cf0: 6573 2061 7265 2072 6561 6c2c 0a20 2020  es are real,.   
+00008d00: 2020 2020 2065 7870 6563 7465 6420 7265       expected re
+00008d10: 7375 6c74 7320 6f76 6572 7269 6465 2069  sults override i
+00008d20: 7320 7265 7175 6972 6564 2e0a 2020 2020  s required..    
+00008d30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008d40: 696e 7370 2c20 6b77 732c 2065 7870 203d  insp, kws, exp =
+00008d50: 2067 6574 5f6d 756c 7469 5f65 7870 280a   get_multi_exp(.
+00008d60: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00008d70: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
+00008d80: 7363 6f70 652c 0a20 2020 2020 2020 2020  scope,.         
+00008d90: 2020 206b 696e 642c 0a20 2020 2020 2020     kind,.       
+00008da0: 2020 2020 2075 7365 5f66 696c 7465 722c       use_filter,
+00008db0: 0a20 2020 2020 2020 2020 2020 2049 6e73  .            Ins
+00008dc0: 7065 6374 6f72 2e67 6574 5f63 6f6c 756d  pector.get_colum
+00008dd0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00008de0: 7365 6c66 2e65 7870 5f63 6f6c 756d 6e73  self.exp_columns
+00008df0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00008e00: 2020 2020 2066 6f72 206b 7720 696e 206b       for kw in k
+00008e10: 7773 3a0a 2020 2020 2020 2020 2020 2020  ws:.            
+00008e20: 696e 7370 2e63 6c65 6172 5f63 6163 6865  insp.clear_cache
+00008e30: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+00008e40: 6573 756c 7420 3d20 696e 7370 2e67 6574  esult = insp.get
+00008e50: 5f6d 756c 7469 5f63 6f6c 756d 6e73 282a  _multi_columns(*
+00008e60: 2a6b 7729 0a20 2020 2020 2020 2020 2020  *kw).           
+00008e70: 2073 656c 662e 5f63 6865 636b 5f74 6162   self._check_tab
+00008e80: 6c65 5f64 6963 7428 7265 7375 6c74 2c20  le_dict(result, 
+00008e90: 6578 702c 2073 656c 662e 5f72 6571 7569  exp, self._requi
+00008ea0: 7265 645f 636f 6c75 6d6e 5f6b 6579 7329  red_column_keys)
+00008eb0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+00008ec0: 726b 2e73 6b69 7028 0a20 2020 2020 2020  rk.skip(.       
+00008ed0: 2022 5265 7175 6972 6573 2061 6e20 696e   "Requires an in
+00008ee0: 7472 6f73 7065 6374 696f 6e20 6d65 7468  trospection meth
+00008ef0: 6f64 2074 6f20 6265 2069 6d70 6c65 6d65  od to be impleme
+00008f00: 6e74 6564 2069 6e20 5351 4c41 6c63 6865  nted in SQLAlche
+00008f10: 6d79 2066 6972 7374 220a 2020 2020 290a  my first".    ).
+00008f20: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
+00008f30: 5f6d 756c 7469 5f75 6e69 7175 655f 636f  _multi_unique_co
+00008f40: 6e73 7472 6169 6e74 7328 293a 0a20 2020  nstraints():.   
+00008f50: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+00008f60: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+00008f70: 280a 2020 2020 2020 2020 2252 6571 7569  (.        "Requi
+00008f80: 7265 7320 616e 2069 6e74 726f 7370 6563  res an introspec
+00008f90: 7469 6f6e 206d 6574 686f 6420 746f 2062  tion method to b
+00008fa0: 6520 696d 706c 656d 656e 7465 6420 696e  e implemented in
+00008fb0: 2053 514c 416c 6368 656d 7920 6669 7273   SQLAlchemy firs
+00008fc0: 7422 0a20 2020 2029 0a20 2020 2064 6566  t".    ).    def
+00008fd0: 2074 6573 745f 6765 745f 6d75 6c74 695f   test_get_multi_
+00008fe0: 6368 6563 6b5f 636f 6e73 7472 6169 6e74  check_constraint
+00008ff0: 7328 293a 0a20 2020 2020 2020 2070 6173  s():.        pas
+00009000: 730a 0a20 2020 2040 7465 7374 696e 672e  s..    @testing.
+00009010: 636f 6d62 696e 6174 696f 6e73 2828 4661  combinations((Fa
+00009020: 6c73 652c 292c 2061 7267 6e61 6d65 733d  lse,), argnames=
+00009030: 2275 7365 5f73 6368 656d 6122 290a 2020  "use_schema").  
+00009040: 2020 4074 6573 7469 6e67 2e72 6571 7569    @testing.requi
+00009050: 7265 732e 666f 7265 6967 6e5f 6b65 795f  res.foreign_key_
+00009060: 636f 6e73 7472 6169 6e74 5f72 6566 6c65  constraint_refle
+00009070: 6374 696f 6e0a 2020 2020 6465 6620 7465  ction.    def te
+00009080: 7374 5f67 6574 5f66 6f72 6569 676e 5f6b  st_get_foreign_k
+00009090: 6579 7328 7365 6c66 2c20 636f 6e6e 6563  eys(self, connec
+000090a0: 7469 6f6e 2c20 7573 655f 7363 6865 6d61  tion, use_schema
+000090b0: 293a 0a20 2020 2020 2020 2069 6620 7573  ):.        if us
+000090c0: 655f 7363 6865 6d61 3a0a 2020 2020 2020  e_schema:.      
+000090d0: 2020 2020 2020 7363 6865 6d61 203d 2063        schema = c
+000090e0: 6f6e 6669 672e 7465 7374 5f73 6368 656d  onfig.test_schem
+000090f0: 610a 2020 2020 2020 2020 656c 7365 3a0a  a.        else:.
+00009100: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00009110: 6d61 203d 204e 6f6e 650a 0a20 2020 2020  ma = None..     
+00009120: 2020 2075 7365 7273 2c20 6164 6472 6573     users, addres
+00009130: 7365 7320 3d20 2873 656c 662e 7461 626c  ses = (self.tabl
+00009140: 6573 2e75 7365 7273 2c20 7365 6c66 2e74  es.users, self.t
+00009150: 6162 6c65 732e 656d 6169 6c5f 6164 6472  ables.email_addr
+00009160: 6573 7365 7329 0a20 2020 2020 2020 2069  esses).        i
+00009170: 6e73 7020 3d20 696e 7370 6563 7428 636f  nsp = inspect(co
+00009180: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
+00009190: 2020 6578 7065 6374 6564 5f73 6368 656d    expected_schem
+000091a0: 6120 3d20 7363 6865 6d61 0a20 2020 2020  a = schema.     
+000091b0: 2020 2023 2075 7365 7273 0a0a 2020 2020     # users..    
+000091c0: 2020 2020 6966 2074 6573 7469 6e67 2e72      if testing.r
+000091d0: 6571 7569 7265 732e 7365 6c66 5f72 6566  equires.self_ref
+000091e0: 6572 656e 7469 616c 5f66 6f72 6569 676e  erential_foreign
+000091f0: 5f6b 6579 732e 656e 6162 6c65 643a 0a20  _keys.enabled:. 
+00009200: 2020 2020 2020 2020 2020 2075 7365 7273             users
+00009210: 5f66 6b65 7973 203d 2069 6e73 702e 6765  _fkeys = insp.ge
+00009220: 745f 666f 7265 6967 6e5f 6b65 7973 2875  t_foreign_keys(u
+00009230: 7365 7273 2e6e 616d 652c 2073 6368 656d  sers.name, schem
+00009240: 613d 7363 6865 6d61 290a 2020 2020 2020  a=schema).      
+00009250: 2020 2020 2020 666b 6579 3120 3d20 7573        fkey1 = us
+00009260: 6572 735f 666b 6579 735b 305d 0a0a 2020  ers_fkeys[0]..  
+00009270: 2020 2020 2020 2020 2020 7769 7468 2074            with t
+00009280: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00009290: 6e61 6d65 645f 636f 6e73 7472 6169 6e74  named_constraint
+000092a0: 732e 6661 696c 5f69 6628 293a 0a20 2020  s.fail_if():.   
+000092b0: 2020 2020 2020 2020 2020 2020 2065 715f               eq_
+000092c0: 2866 6b65 7931 5b22 6e61 6d65 225d 2c20  (fkey1["name"], 
+000092d0: 2275 7365 725f 6964 5f66 6b22 290a 0a20  "user_id_fk").. 
+000092e0: 2020 2020 2020 2020 2020 2065 715f 2866             eq_(f
+000092f0: 6b65 7931 5b22 7265 6665 7272 6564 5f73  key1["referred_s
+00009300: 6368 656d 6122 5d2c 2065 7870 6563 7465  chema"], expecte
+00009310: 645f 7363 6865 6d61 290a 2020 2020 2020  d_schema).      
+00009320: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
+00009330: 2272 6566 6572 7265 645f 7461 626c 6522  "referred_table"
+00009340: 5d2c 2075 7365 7273 2e6e 616d 6529 0a20  ], users.name). 
+00009350: 2020 2020 2020 2020 2020 2065 715f 2866             eq_(f
+00009360: 6b65 7931 5b22 7265 6665 7272 6564 5f63  key1["referred_c
+00009370: 6f6c 756d 6e73 225d 2c20 5b22 7573 6572  olumns"], ["user
+00009380: 5f69 6422 5d29 0a20 2020 2020 2020 2020  _id"]).         
+00009390: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
+000093a0: 7175 6972 6573 2e73 656c 665f 7265 6665  quires.self_refe
+000093b0: 7265 6e74 6961 6c5f 666f 7265 6967 6e5f  rential_foreign_
+000093c0: 6b65 7973 2e65 6e61 626c 6564 3a0a 2020  keys.enabled:.  
+000093d0: 2020 2020 2020 2020 2020 2020 2020 6571                eq
+000093e0: 5f28 666b 6579 315b 2263 6f6e 7374 7261  _(fkey1["constra
+000093f0: 696e 6564 5f63 6f6c 756d 6e73 225d 2c20  ined_columns"], 
+00009400: 5b22 7061 7265 6e74 5f75 7365 725f 6964  ["parent_user_id
+00009410: 225d 290a 0a20 2020 2020 2020 2023 2061  "])..        # a
+00009420: 6464 7265 7373 6573 0a20 2020 2020 2020  ddresses.       
+00009430: 2061 6464 725f 666b 6579 7320 3d20 696e   addr_fkeys = in
+00009440: 7370 2e67 6574 5f66 6f72 6569 676e 5f6b  sp.get_foreign_k
+00009450: 6579 7328 6164 6472 6573 7365 732e 6e61  eys(addresses.na
+00009460: 6d65 2c20 7363 6865 6d61 3d73 6368 656d  me, schema=schem
+00009470: 6129 0a20 2020 2020 2020 2066 6b65 7931  a).        fkey1
+00009480: 203d 2061 6464 725f 666b 6579 735b 305d   = addr_fkeys[0]
+00009490: 0a0a 2020 2020 2020 2020 7769 7468 2074  ..        with t
+000094a0: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+000094b0: 696d 706c 6963 6974 6c79 5f6e 616d 6564  implicitly_named
+000094c0: 5f63 6f6e 7374 7261 696e 7473 2e66 6169  _constraints.fai
+000094d0: 6c5f 6966 2829 3a0a 2020 2020 2020 2020  l_if():.        
+000094e0: 2020 2020 7365 6c66 2e61 7373 6572 745f      self.assert_
+000094f0: 2866 6b65 7931 5b22 6e61 6d65 225d 2069  (fkey1["name"] i
+00009500: 7320 6e6f 7420 4e6f 6e65 290a 0a20 2020  s not None)..   
+00009510: 2020 2020 2065 715f 2866 6b65 7931 5b22       eq_(fkey1["
+00009520: 7265 6665 7272 6564 5f73 6368 656d 6122  referred_schema"
+00009530: 5d2c 2065 7870 6563 7465 645f 7363 6865  ], expected_sche
+00009540: 6d61 290a 2020 2020 2020 2020 6571 5f28  ma).        eq_(
+00009550: 666b 6579 315b 2272 6566 6572 7265 645f  fkey1["referred_
+00009560: 7461 626c 6522 5d2c 2075 7365 7273 2e6e  table"], users.n
+00009570: 616d 6529 0a20 2020 2020 2020 2065 715f  ame).        eq_
+00009580: 2866 6b65 7931 5b22 7265 6665 7272 6564  (fkey1["referred
+00009590: 5f63 6f6c 756d 6e73 225d 2c20 5b22 7573  _columns"], ["us
+000095a0: 6572 5f69 6422 5d29 0a20 2020 2020 2020  er_id"]).       
+000095b0: 2065 715f 2866 6b65 7931 5b22 636f 6e73   eq_(fkey1["cons
+000095c0: 7472 6169 6e65 645f 636f 6c75 6d6e 7322  trained_columns"
+000095d0: 5d2c 205b 2272 656d 6f74 655f 7573 6572  ], ["remote_user
+000095e0: 5f69 6422 5d29 0a0a 2020 2020 4074 6573  _id"])..    @tes
+000095f0: 7469 6e67 2e63 6f6d 6269 6e61 7469 6f6e  ting.combination
+00009600: 7328 0a20 2020 2020 2020 204e 6f6e 652c  s(.        None,
+00009610: 0a20 2020 2020 2020 2028 2266 6f72 6569  .        ("forei
+00009620: 676e 5f6b 6579 222c 2074 6573 7469 6e67  gn_key", testing
+00009630: 2e72 6571 7569 7265 732e 666f 7265 6967  .requires.foreig
+00009640: 6e5f 6b65 795f 636f 6e73 7472 6169 6e74  n_key_constraint
+00009650: 5f72 6566 6c65 6374 696f 6e29 2c0a 2020  _reflection),.  
+00009660: 2020 2020 2020 6172 676e 616d 6573 3d22        argnames="
+00009670: 6f72 6465 725f 6279 222c 0a20 2020 2029  order_by",.    )
+00009680: 0a20 2020 2040 7465 7374 696e 672e 636f  .    @testing.co
+00009690: 6d62 696e 6174 696f 6e73 280a 2020 2020  mbinations(.    
+000096a0: 2020 2020 2854 7275 652c 2074 6573 7469      (True, testi
+000096b0: 6e67 2e72 6571 7569 7265 732e 7363 6865  ng.requires.sche
+000096c0: 6d61 7329 2c20 4661 6c73 652c 2061 7267  mas), False, arg
+000096d0: 6e61 6d65 733d 2275 7365 5f73 6368 656d  names="use_schem
+000096e0: 6122 0a20 2020 2029 0a20 2020 2064 6566  a".    ).    def
+000096f0: 2074 6573 745f 6765 745f 7461 626c 655f   test_get_table_
+00009700: 6e61 6d65 7328 7365 6c66 2c20 636f 6e6e  names(self, conn
+00009710: 6563 7469 6f6e 2c20 6f72 6465 725f 6279  ection, order_by
+00009720: 2c20 7573 655f 7363 6865 6d61 293a 0a0a  , use_schema):..
+00009730: 2020 2020 2020 2020 7363 6865 6d61 203d          schema =
+00009740: 204e 6f6e 650a 0a20 2020 2020 2020 205f   None..        _
+00009750: 6967 6e6f 7265 5f74 6162 6c65 7320 3d20  ignore_tables = 
+00009760: 5b0a 2020 2020 2020 2020 2020 2020 2261  [.            "a
+00009770: 6363 6f75 6e74 222c 0a20 2020 2020 2020  ccount",.       
+00009780: 2020 2020 2022 616c 656d 6269 635f 7665       "alembic_ve
+00009790: 7273 696f 6e22 2c0a 2020 2020 2020 2020  rsion",.        
+000097a0: 2020 2020 2262 7974 6573 5f74 6162 6c65      "bytes_table
+000097b0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000097c0: 636f 6d6d 656e 745f 7465 7374 222c 0a20  comment_test",. 
+000097d0: 2020 2020 2020 2020 2020 2022 6461 7465             "date
+000097e0: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+000097f0: 2020 2020 2022 6e6f 6e63 6f6c 5f69 6478       "noncol_idx
+00009800: 5f74 6573 745f 706b 222c 0a20 2020 2020  _test_pk",.     
+00009810: 2020 2020 2020 2022 6e6f 6e63 6f6c 5f69         "noncol_i
+00009820: 6478 5f74 6573 745f 6e6f 706b 222c 0a20  dx_test_nopk",. 
+00009830: 2020 2020 2020 2020 2020 2022 6c6f 6361             "loca
+00009840: 6c5f 7461 626c 6522 2c0a 2020 2020 2020  l_table",.      
+00009850: 2020 2020 2020 2272 656d 6f74 655f 7461        "remote_ta
+00009860: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
+00009870: 2020 2272 656d 6f74 655f 7461 626c 655f    "remote_table_
+00009880: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+00009890: 2274 6578 745f 7461 626c 6522 2c0a 2020  "text_table",.  
+000098a0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+000098b0: 746d 7022 2c0a 2020 2020 2020 2020 2020  tmp",.          
+000098c0: 2020 226e 6f5f 636f 6e73 7472 6169 6e74    "no_constraint
+000098d0: 7322 2c0a 2020 2020 2020 2020 5d0a 0a20  s",.        ].. 
+000098e0: 2020 2020 2020 2069 6e73 7020 3d20 696e         insp = in
+000098f0: 7370 6563 7428 636f 6e6e 6563 7469 6f6e  spect(connection
+00009900: 290a 0a20 2020 2020 2020 2069 6620 6f72  )..        if or
+00009910: 6465 725f 6279 3a0a 2020 2020 2020 2020  der_by:.        
+00009920: 2020 2020 7461 626c 6573 203d 205b 0a20      tables = [. 
+00009930: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009940: 6563 5b30 5d20 666f 7220 7265 6320 696e  ec[0] for rec in
+00009950: 2069 6e73 702e 6765 745f 736f 7274 6564   insp.get_sorted
+00009960: 5f74 6162 6c65 5f61 6e64 5f66 6b63 5f6e  _table_and_fkc_n
+00009970: 616d 6573 2873 6368 656d 6129 2069 6620  ames(schema) if 
+00009980: 7265 635b 305d 0a20 2020 2020 2020 2020  rec[0].         
+00009990: 2020 205d 0a20 2020 2020 2020 2065 6c73     ].        els
+000099a0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+000099b0: 6162 6c65 7320 3d20 696e 7370 2e67 6574  ables = insp.get
+000099c0: 5f74 6162 6c65 5f6e 616d 6573 2873 6368  _table_names(sch
+000099d0: 656d 6129 0a20 2020 2020 2020 2074 6162  ema).        tab
+000099e0: 6c65 5f6e 616d 6573 203d 205b 7420 666f  le_names = [t fo
+000099f0: 7220 7420 696e 2074 6162 6c65 7320 6966  r t in tables if
+00009a00: 2074 206e 6f74 2069 6e20 5f69 676e 6f72   t not in _ignor
+00009a10: 655f 7461 626c 6573 5d0a 0a20 2020 2020  e_tables]..     
+00009a20: 2020 2069 6620 6f72 6465 725f 6279 203d     if order_by =
+00009a30: 3d20 2266 6f72 6569 676e 5f6b 6579 223a  = "foreign_key":
+00009a40: 0a20 2020 2020 2020 2020 2020 2061 6e73  .            ans
+00009a50: 7765 7220 3d20 5b22 7573 6572 7322 2c20  wer = ["users", 
+00009a60: 2265 6d61 696c 5f61 6464 7265 7373 6573  "email_addresses
+00009a70: 222c 2022 6469 6e67 616c 696e 6773 225d  ", "dingalings"]
+00009a80: 0a20 2020 2020 2020 2020 2020 2065 715f  .            eq_
+00009a90: 2874 6162 6c65 5f6e 616d 6573 2c20 616e  (table_names, an
+00009aa0: 7377 6572 290a 2020 2020 2020 2020 656c  swer).        el
+00009ab0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009ac0: 616e 7377 6572 203d 205b 2264 696e 6761  answer = ["dinga
+00009ad0: 6c69 6e67 7322 2c20 2265 6d61 696c 5f61  lings", "email_a
+00009ae0: 6464 7265 7373 6573 222c 2022 7573 6572  ddresses", "user
+00009af0: 7322 5d0a 2020 2020 2020 2020 2020 2020  s"].            
+00009b00: 6571 5f28 736f 7274 6564 2874 6162 6c65  eq_(sorted(table
+00009b10: 5f6e 616d 6573 292c 2061 6e73 7765 7229  _names), answer)
+00009b20: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00009b30: 6f64 0a20 2020 2064 6566 2064 6566 696e  od.    def defin
+00009b40: 655f 7465 6d70 5f74 6162 6c65 7328 636c  e_temp_tables(cl
+00009b50: 732c 206d 6574 6164 6174 6129 3a0a 2020  s, metadata):.  
+00009b60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009b70: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+00009b80: 4445 3a0a 0a20 2020 2020 2020 2049 6e20  DE:..        In 
+00009b90: 436c 6f75 6420 5370 616e 6e65 7220 756e  Cloud Spanner un
+00009ba0: 6971 7565 2069 6e64 6578 6573 2061 7265  ique indexes are
+00009bb0: 2075 7365 6420 696e 7374 6561 6420 6f66   used instead of
+00009bc0: 2064 6972 6563 746c 790a 2020 2020 2020   directly.      
+00009bd0: 2020 6372 6561 7469 6e67 2075 6e69 7175    creating uniqu
+00009be0: 6520 636f 6e73 7472 6169 6e74 732e 204f  e constraints. O
+00009bf0: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+00009c00: 7374 2074 6f20 7265 706c 6163 650a 2020  st to replace.  
+00009c10: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
+00009c20: 7320 7769 7468 2069 6e64 6578 6573 2069  s with indexes i
+00009c30: 6e20 7465 7374 696e 6720 6461 7461 2e0a  n testing data..
+00009c40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009c50: 2020 2020 6b77 203d 2074 656d 705f 7461      kw = temp_ta
+00009c60: 626c 655f 6b65 7977 6f72 645f 6172 6773  ble_keyword_args
+00009c70: 2863 6f6e 6669 672c 2063 6f6e 6669 672e  (config, config.
+00009c80: 6462 290a 2020 2020 2020 2020 7573 6572  db).        user
+00009c90: 5f74 6d70 203d 2054 6162 6c65 280a 2020  _tmp = Table(.  
+00009ca0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+00009cb0: 746d 7022 2c0a 2020 2020 2020 2020 2020  tmp",.          
+00009cc0: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
+00009cd0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00009ce0: 6964 222c 2073 716c 616c 6368 656d 792e  id", sqlalchemy.
+00009cf0: 494e 542c 2070 7269 6d61 7279 5f6b 6579  INT, primary_key
+00009d00: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00009d10: 2020 2020 436f 6c75 6d6e 2822 6e61 6d65      Column("name
+00009d20: 222c 2073 716c 616c 6368 656d 792e 5641  ", sqlalchemy.VA
+00009d30: 5243 4841 5228 3530 2929 2c0a 2020 2020  RCHAR(50)),.    
+00009d40: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00009d50: 666f 6f22 2c20 7371 6c61 6c63 6865 6d79  foo", sqlalchemy
+00009d60: 2e49 4e54 292c 0a20 2020 2020 2020 2020  .INT),.         
+00009d70: 2020 2073 716c 616c 6368 656d 792e 496e     sqlalchemy.In
+00009d80: 6465 7828 2275 7365 725f 746d 705f 7571  dex("user_tmp_uq
+00009d90: 222c 2022 6e61 6d65 222c 2075 6e69 7175  ", "name", uniqu
+00009da0: 653d 5472 7565 292c 0a20 2020 2020 2020  e=True),.       
+00009db0: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+00009dc0: 496e 6465 7828 2275 7365 725f 746d 705f  Index("user_tmp_
+00009dd0: 6978 222c 2022 666f 6f22 292c 0a20 2020  ix", "foo"),.   
+00009de0: 2020 2020 2020 2020 2065 7874 656e 645f           extend_
+00009df0: 6578 6973 7469 6e67 3d54 7275 652c 0a20  existing=True,. 
+00009e00: 2020 2020 2020 2020 2020 202a 2a6b 772c             **kw,
+00009e10: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00009e20: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00009e30: 2020 2020 7465 7374 696e 672e 7265 7175      testing.requ
+00009e40: 6972 6573 2e76 6965 775f 7265 666c 6563  ires.view_reflec
+00009e50: 7469 6f6e 2e65 6e61 626c 6564 0a20 2020  tion.enabled.   
+00009e60: 2020 2020 2020 2020 2061 6e64 2074 6573           and tes
+00009e70: 7469 6e67 2e72 6571 7569 7265 732e 7465  ting.requires.te
+00009e80: 6d70 6f72 6172 795f 7669 6577 732e 656e  mporary_views.en
+00009e90: 6162 6c65 640a 2020 2020 2020 2020 293a  abled.        ):
+00009ea0: 0a20 2020 2020 2020 2020 2020 2065 7665  .            eve
+00009eb0: 6e74 2e6c 6973 7465 6e28 0a20 2020 2020  nt.listen(.     
+00009ec0: 2020 2020 2020 2020 2020 2075 7365 725f             user_
+00009ed0: 746d 702c 0a20 2020 2020 2020 2020 2020  tmp,.           
+00009ee0: 2020 2020 2022 6166 7465 725f 6372 6561       "after_crea
+00009ef0: 7465 222c 0a20 2020 2020 2020 2020 2020  te",.           
+00009f00: 2020 2020 2044 444c 2822 6372 6561 7465       DDL("create
+00009f10: 2074 656d 706f 7261 7279 2076 6965 7720   temporary view 
+00009f20: 7573 6572 5f74 6d70 5f76 2061 7320 2220  user_tmp_v as " 
+00009f30: 2273 656c 6563 7420 2a20 6672 6f6d 2075  "select * from u
+00009f40: 7365 725f 746d 7022 292c 0a20 2020 2020  ser_tmp"),.     
+00009f50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00009f60: 2020 2020 2065 7665 6e74 2e6c 6973 7465       event.liste
+00009f70: 6e28 7573 6572 5f74 6d70 2c20 2262 6566  n(user_tmp, "bef
+00009f80: 6f72 655f 6472 6f70 222c 2044 444c 2822  ore_drop", DDL("
+00009f90: 6472 6f70 2076 6965 7720 7573 6572 5f74  drop view user_t
+00009fa0: 6d70 5f76 2229 290a 0a20 2020 2040 7465  mp_v"))..    @te
+00009fb0: 7374 696e 672e 7072 6f76 6964 655f 6d65  sting.provide_me
+00009fc0: 7461 6461 7461 0a20 2020 2064 6566 2074  tadata.    def t
+00009fd0: 6573 745f 7265 666c 6563 745f 7374 7269  est_reflect_stri
+00009fe0: 6e67 5f63 6f6c 756d 6e5f 6d61 785f 6c65  ng_column_max_le
+00009ff0: 6e28 7365 6c66 2c20 636f 6e6e 6563 7469  n(self, connecti
+0000a000: 6f6e 293a 0a20 2020 2020 2020 2022 2222  on):.        """
+0000a010: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+0000a020: 2053 5045 4349 4649 4320 5445 5354 3a0a   SPECIFIC TEST:.
+0000a030: 0a20 2020 2020 2020 2049 6e20 5370 616e  .        In Span
+0000a040: 6e65 7220 636f 6c75 6d6e 206f 6620 7468  ner column of th
+0000a050: 6520 5354 5249 4e47 2074 7970 6520 6361  e STRING type ca
+0000a060: 6e20 6265 0a20 2020 2020 2020 2063 7265  n be.        cre
+0000a070: 6174 6564 2077 6974 6820 7369 7a65 2064  ated with size d
+0000a080: 6566 696e 6564 2061 7320 4d41 582e 2054  efined as MAX. T
+0000a090: 6865 2074 6573 740a 2020 2020 2020 2020  he test.        
+0000a0a0: 6368 6563 6b73 2074 6861 7420 7375 6368  checks that such
+0000a0b0: 2061 2063 6f6c 756d 6e20 6973 2063 6f72   a column is cor
+0000a0c0: 7265 6374 6c79 2072 6566 6c65 6374 6564  rectly reflected
+0000a0d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000a0e0: 2020 2020 2020 6d65 7461 6461 7461 203d        metadata =
+0000a0f0: 204d 6574 6144 6174 6128 290a 2020 2020   MetaData().    
+0000a100: 2020 2020 5461 626c 6528 2274 6578 745f      Table("text_
+0000a110: 7461 626c 6522 2c20 6d65 7461 6461 7461  table", metadata
+0000a120: 2c20 436f 6c75 6d6e 2822 5465 7374 436f  , Column("TestCo
+0000a130: 6c75 6d6e 222c 2054 6578 742c 206e 756c  lumn", Text, nul
+0000a140: 6c61 626c 653d 4661 6c73 6529 290a 2020  lable=False)).  
+0000a150: 2020 2020 2020 6d65 7461 6461 7461 2e63        metadata.c
+0000a160: 7265 6174 655f 616c 6c28 636f 6e6e 6563  reate_all(connec
+0000a170: 7469 6f6e 290a 0a20 2020 2020 2020 2054  tion)..        T
+0000a180: 6162 6c65 2822 7465 7874 5f74 6162 6c65  able("text_table
+0000a190: 222c 206d 6574 6164 6174 612c 2061 7574  ", metadata, aut
+0000a1a0: 6f6c 6f61 643d 5472 7565 290a 0a20 2020  oload=True)..   
+0000a1b0: 2064 6566 2074 6573 745f 7265 666c 6563   def test_reflec
+0000a1c0: 745f 6279 7465 735f 636f 6c75 6d6e 5f6d  t_bytes_column_m
+0000a1d0: 6178 5f6c 656e 2873 656c 662c 2063 6f6e  ax_len(self, con
+0000a1e0: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+0000a1f0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+0000a200: 414e 4e45 5220 5350 4543 4946 4943 2054  ANNER SPECIFIC T
+0000a210: 4553 543a 0a0a 2020 2020 2020 2020 496e  EST:..        In
+0000a220: 2053 7061 6e6e 6572 2063 6f6c 756d 6e20   Spanner column 
+0000a230: 6f66 2074 6865 2042 5954 4553 2074 7970  of the BYTES typ
+0000a240: 6520 6361 6e20 6265 0a20 2020 2020 2020  e can be.       
+0000a250: 2063 7265 6174 6564 2077 6974 6820 7369   created with si
+0000a260: 7a65 2064 6566 696e 6564 2061 7320 4d41  ze defined as MA
+0000a270: 582e 2054 6865 2074 6573 740a 2020 2020  X. The test.    
+0000a280: 2020 2020 6368 6563 6b73 2074 6861 7420      checks that 
+0000a290: 7375 6368 2061 2063 6f6c 756d 6e20 6973  such a column is
+0000a2a0: 2063 6f72 7265 6374 6c79 2072 6566 6c65   correctly refle
+0000a2b0: 6374 6564 2e0a 2020 2020 2020 2020 2222  cted..        ""
+0000a2c0: 220a 2020 2020 2020 2020 6d65 7461 6461  ".        metada
+0000a2d0: 7461 203d 204d 6574 6144 6174 6128 290a  ta = MetaData().
+0000a2e0: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+0000a2f0: 2020 2020 2020 2020 2020 2022 6279 7465             "byte
+0000a300: 735f 7461 626c 6522 2c0a 2020 2020 2020  s_table",.      
+0000a310: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
+0000a320: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+0000a330: 6d6e 2822 5465 7374 436f 6c75 6d6e 222c  mn("TestColumn",
+0000a340: 204c 6172 6765 4269 6e61 7279 2c20 6e75   LargeBinary, nu
+0000a350: 6c6c 6162 6c65 3d46 616c 7365 292c 0a20  llable=False),. 
+0000a360: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000a370: 206d 6574 6164 6174 612e 6372 6561 7465   metadata.create
+0000a380: 5f61 6c6c 2863 6f6e 6e65 6374 696f 6e29  _all(connection)
+0000a390: 0a0a 2020 2020 2020 2020 5461 626c 6528  ..        Table(
+0000a3a0: 2262 7974 6573 5f74 6162 6c65 222c 206d  "bytes_table", m
+0000a3b0: 6574 6164 6174 612c 2061 7574 6f6c 6f61  etadata, autoloa
+0000a3c0: 643d 5472 7565 290a 0a20 2020 2040 7465  d=True)..    @te
+0000a3d0: 7374 696e 672e 7265 7175 6972 6573 2e75  sting.requires.u
+0000a3e0: 6e69 7175 655f 636f 6e73 7472 6169 6e74  nique_constraint
+0000a3f0: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
+0000a400: 6465 6620 7465 7374 5f67 6574 5f75 6e69  def test_get_uni
+0000a410: 7175 655f 636f 6e73 7472 6169 6e74 7328  que_constraints(
+0000a420: 7365 6c66 2c20 6d65 7461 6461 7461 2c20  self, metadata, 
+0000a430: 636f 6e6e 6563 7469 6f6e 2c20 7573 655f  connection, use_
+0000a440: 7363 6865 6d61 3d46 616c 7365 293a 0a20  schema=False):. 
+0000a450: 2020 2020 2020 2023 2053 514c 6974 6520         # SQLite 
+0000a460: 6469 616c 6563 7420 6e65 6564 7320 746f  dialect needs to
+0000a470: 2070 6172 7365 2074 6865 206e 616d 6573   parse the names
+0000a480: 206f 6620 7468 6520 636f 6e73 7472 6169   of the constrai
+0000a490: 6e74 730a 2020 2020 2020 2020 2320 7365  nts.        # se
+0000a4a0: 7061 7261 7465 6c79 2066 726f 6d20 7768  parately from wh
+0000a4b0: 6174 2069 7420 6765 7473 2066 726f 6d20  at it gets from 
+0000a4c0: 5052 4147 4d41 2069 6e64 6578 5f6c 6973  PRAGMA index_lis
+0000a4d0: 7428 292c 2061 6e64 0a20 2020 2020 2020  t(), and.       
+0000a4e0: 2023 2074 6865 6e20 6d61 7463 6865 7320   # then matches 
+0000a4f0: 7468 656d 2075 702e 2020 736f 2073 616d  them up.  so sam
+0000a500: 6520 7365 7420 6f66 2063 6f6c 756d 6e5f  e set of column_
+0000a510: 6e61 6d65 7320 696e 2074 776f 0a20 2020  names in two.   
+0000a520: 2020 2020 2023 2063 6f6e 7374 7261 696e       # constrain
+0000a530: 7473 2077 696c 6c20 636f 6e66 7573 6520  ts will confuse 
+0000a540: 6974 2e20 2020 2050 6572 6861 7073 2077  it.    Perhaps w
+0000a550: 6520 7368 6f75 6c64 206e 6f20 6c6f 6e67  e should no long
+0000a560: 6572 0a20 2020 2020 2020 2023 2062 6f74  er.        # bot
+0000a570: 6865 7220 7769 7468 2069 6e64 6578 5f6c  her with index_l
+0000a580: 6973 7428 2920 6865 7265 2073 696e 6365  ist() here since
+0000a590: 2077 6520 6861 7665 2074 6865 2077 686f   we have the who
+0000a5a0: 6c65 0a20 2020 2020 2020 2023 2043 5245  le.        # CRE
+0000a5b0: 4154 4520 5441 424c 453f 0a0a 2020 2020  ATE TABLE?..    
+0000a5c0: 2020 2020 6966 2075 7365 5f73 6368 656d      if use_schem
+0000a5d0: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
+0000a5e0: 6368 656d 6120 3d20 636f 6e66 6967 2e74  chema = config.t
+0000a5f0: 6573 745f 7363 6865 6d61 0a20 2020 2020  est_schema.     
+0000a600: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a610: 2020 2020 2073 6368 656d 6120 3d20 4e6f       schema = No
+0000a620: 6e65 0a20 2020 2020 2020 2075 6e69 7175  ne.        uniqu
+0000a630: 6573 203d 2073 6f72 7465 6428 0a20 2020  es = sorted(.   
+0000a640: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
+0000a650: 2020 2020 2020 2020 2020 207b 226e 616d             {"nam
+0000a660: 6522 3a20 2275 6e69 7175 655f 6122 2c20  e": "unique_a", 
+0000a670: 2263 6f6c 756d 6e5f 6e61 6d65 7322 3a20  "column_names": 
+0000a680: 5b22 6122 5d7d 2c0a 2020 2020 2020 2020  ["a"]},.        
+0000a690: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+0000a6a0: 2022 756e 6971 7565 5f61 5f62 5f63 222c   "unique_a_b_c",
+0000a6b0: 2022 636f 6c75 6d6e 5f6e 616d 6573 223a   "column_names":
+0000a6c0: 205b 2261 222c 2022 6222 2c20 2263 225d   ["a", "b", "c"]
+0000a6d0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+0000a6e0: 2020 207b 226e 616d 6522 3a20 2275 6e69     {"name": "uni
+0000a6f0: 7175 655f 635f 615f 6222 2c20 2263 6f6c  que_c_a_b", "col
+0000a700: 756d 6e5f 6e61 6d65 7322 3a20 5b22 6322  umn_names": ["c"
+0000a710: 2c20 2261 222c 2022 6222 5d7d 2c0a 2020  , "a", "b"]},.  
+0000a720: 2020 2020 2020 2020 2020 2020 2020 7b22                {"
+0000a730: 6e61 6d65 223a 2022 756e 6971 7565 5f61  name": "unique_a
+0000a740: 7363 5f6b 6579 222c 2022 636f 6c75 6d6e  sc_key", "column
+0000a750: 5f6e 616d 6573 223a 205b 2261 7363 222c  _names": ["asc",
+0000a760: 2022 6b65 7922 5d7d 2c0a 2020 2020 2020   "key"]},.      
+0000a770: 2020 2020 2020 2020 2020 7b22 6e61 6d65            {"name
+0000a780: 223a 2022 692e 6861 7665 2e64 6f74 7322  ": "i.have.dots"
+0000a790: 2c20 2263 6f6c 756d 6e5f 6e61 6d65 7322  , "column_names"
+0000a7a0: 3a20 5b22 6222 5d7d 2c0a 2020 2020 2020  : ["b"]},.      
+0000a7b0: 2020 2020 2020 2020 2020 7b22 6e61 6d65            {"name
+0000a7c0: 223a 2022 6920 6861 7665 2073 7061 6365  ": "i have space
+0000a7d0: 7322 2c20 2263 6f6c 756d 6e5f 6e61 6d65  s", "column_name
+0000a7e0: 7322 3a20 5b22 6322 5d7d 2c0a 2020 2020  s": ["c"]},.    
+0000a7f0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000a800: 2020 2020 2020 206b 6579 3d6f 7065 7261         key=opera
+0000a810: 746f 722e 6974 656d 6765 7474 6572 2822  tor.itemgetter("
+0000a820: 6e61 6d65 2229 2c0a 2020 2020 2020 2020  name"),.        
+0000a830: 290a 2020 2020 2020 2020 7461 626c 6520  ).        table 
+0000a840: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
+0000a850: 2020 2020 2022 7465 7374 7462 6c22 2c0a       "testtbl",.
+0000a860: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+0000a870: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+0000a880: 2020 436f 6c75 6d6e 2822 6964 222c 2073    Column("id", s
+0000a890: 716c 616c 6368 656d 792e 494e 542c 2070  qlalchemy.INT, p
+0000a8a0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+0000a8b0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+0000a8c0: 6c75 6d6e 2822 6122 2c20 5374 7269 6e67  lumn("a", String
+0000a8d0: 2832 3029 292c 0a20 2020 2020 2020 2020  (20)),.         
+0000a8e0: 2020 2043 6f6c 756d 6e28 2262 222c 2053     Column("b", S
+0000a8f0: 7472 696e 6728 3330 2929 2c0a 2020 2020  tring(30)),.    
+0000a900: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+0000a910: 6322 2c20 496e 7465 6765 7229 2c0a 2020  c", Integer),.  
+0000a920: 2020 2020 2020 2020 2020 2320 7265 7365            # rese
+0000a930: 7276 6564 2069 6465 6e74 6966 6965 7273  rved identifiers
+0000a940: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+0000a950: 756d 6e28 2261 7363 222c 2053 7472 696e  umn("asc", Strin
+0000a960: 6728 3330 2929 2c0a 2020 2020 2020 2020  g(30)),.        
+0000a970: 2020 2020 436f 6c75 6d6e 2822 6b65 7922      Column("key"
+0000a980: 2c20 5374 7269 6e67 2833 3029 292c 0a20  , String(30)),. 
+0000a990: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
+0000a9a0: 6368 656d 792e 496e 6465 7828 2275 6e69  chemy.Index("uni
+0000a9b0: 7175 655f 6122 2c20 2261 222c 2075 6e69  que_a", "a", uni
+0000a9c0: 7175 653d 5472 7565 292c 0a20 2020 2020  que=True),.     
+0000a9d0: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
+0000a9e0: 792e 496e 6465 7828 2275 6e69 7175 655f  y.Index("unique_
+0000a9f0: 615f 625f 6322 2c20 2261 222c 2022 6222  a_b_c", "a", "b"
+0000aa00: 2c20 2263 222c 2075 6e69 7175 653d 5472  , "c", unique=Tr
+0000aa10: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
+0000aa20: 2073 716c 616c 6368 656d 792e 496e 6465   sqlalchemy.Inde
+0000aa30: 7828 2275 6e69 7175 655f 635f 615f 6222  x("unique_c_a_b"
+0000aa40: 2c20 2263 222c 2022 6122 2c20 2262 222c  , "c", "a", "b",
+0000aa50: 2075 6e69 7175 653d 5472 7565 292c 0a20   unique=True),. 
+0000aa60: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
+0000aa70: 6368 656d 792e 496e 6465 7828 2275 6e69  chemy.Index("uni
+0000aa80: 7175 655f 6173 635f 6b65 7922 2c20 2261  que_asc_key", "a
+0000aa90: 7363 222c 2022 6b65 7922 2c20 756e 6971  sc", "key", uniq
+0000aaa0: 7565 3d54 7275 6529 2c0a 2020 2020 2020  ue=True),.      
+0000aab0: 2020 2020 2020 7363 6865 6d61 3d73 6368        schema=sch
+0000aac0: 656d 612c 0a20 2020 2020 2020 2029 0a20  ema,.        ). 
+0000aad0: 2020 2020 2020 2074 6162 6c65 2e63 7265         table.cre
+0000aae0: 6174 6528 636f 6e6e 6563 7469 6f6e 290a  ate(connection).
+0000aaf0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+0000ab00: 6f6e 2e63 6f6e 6e65 6374 696f 6e2e 636f  on.connection.co
+0000ab10: 6d6d 6974 2829 0a0a 2020 2020 2020 2020  mmit()..        
+0000ab20: 696e 7370 6563 746f 7220 3d20 696e 7370  inspector = insp
+0000ab30: 6563 7428 636f 6e6e 6563 7469 6f6e 290a  ect(connection).
+0000ab40: 2020 2020 2020 2020 7265 666c 6563 7465          reflecte
+0000ab50: 6420 3d20 736f 7274 6564 280a 2020 2020  d = sorted(.    
+0000ab60: 2020 2020 2020 2020 696e 7370 6563 746f          inspecto
+0000ab70: 722e 6765 745f 756e 6971 7565 5f63 6f6e  r.get_unique_con
+0000ab80: 7374 7261 696e 7473 2822 7465 7374 7462  straints("testtb
+0000ab90: 6c22 2c20 7363 6865 6d61 3d73 6368 656d  l", schema=schem
+0000aba0: 6129 2c0a 2020 2020 2020 2020 2020 2020  a),.            
+0000abb0: 6b65 793d 6f70 6572 6174 6f72 2e69 7465  key=operator.ite
+0000abc0: 6d67 6574 7465 7228 226e 616d 6522 292c  mgetter("name"),
+0000abd0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000abe0: 2020 2020 6e61 6d65 735f 7468 6174 5f64      names_that_d
+0000abf0: 7570 6c69 6361 7465 5f69 6e64 6578 203d  uplicate_index =
+0000ac00: 2073 6574 2829 0a0a 2020 2020 2020 2020   set()..        
+0000ac10: 666f 7220 6f72 6967 2c20 7265 666c 2069  for orig, refl i
+0000ac20: 6e20 7a69 7028 756e 6971 7565 732c 2072  n zip(uniques, r
+0000ac30: 6566 6c65 6374 6564 293a 0a20 2020 2020  eflected):.     
+0000ac40: 2020 2020 2020 2023 2044 6966 6665 7265         # Differe
+0000ac50: 6e74 2064 6961 6c65 6374 7320 6861 6e64  nt dialects hand
+0000ac60: 6c65 2064 7570 6c69 6361 7465 2069 6e64  le duplicate ind
+0000ac70: 6578 2061 6e64 2063 6f6e 7374 7261 696e  ex and constrain
+0000ac80: 7473 0a20 2020 2020 2020 2020 2020 2023  ts.            #
+0000ac90: 2064 6966 6665 7265 6e74 6c79 2c20 736f   differently, so
+0000aca0: 2069 676e 6f72 6520 7468 6973 2066 6c61   ignore this fla
+0000acb0: 670a 2020 2020 2020 2020 2020 2020 6475  g.            du
+0000acc0: 7065 203d 2072 6566 6c2e 706f 7028 2264  pe = refl.pop("d
+0000acd0: 7570 6c69 6361 7465 735f 696e 6465 7822  uplicates_index"
+0000ace0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+0000acf0: 2020 2020 6966 2064 7570 653a 0a20 2020      if dupe:.   
+0000ad00: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0000ad10: 6573 5f74 6861 745f 6475 706c 6963 6174  es_that_duplicat
+0000ad20: 655f 696e 6465 782e 6164 6428 6475 7065  e_index.add(dupe
+0000ad30: 290a 2020 2020 2020 2020 2020 2020 6571  ).            eq
+0000ad40: 5f28 6f72 6967 2c20 7265 666c 290a 0a20  _(orig, refl).. 
+0000ad50: 2020 2020 2020 2072 6566 6c65 6374 6564         reflected
+0000ad60: 5f6d 6574 6164 6174 6120 3d20 4d65 7461  _metadata = Meta
+0000ad70: 4461 7461 2829 0a20 2020 2020 2020 2072  Data().        r
+0000ad80: 6566 6c65 6374 6564 203d 2054 6162 6c65  eflected = Table
+0000ad90: 280a 2020 2020 2020 2020 2020 2020 2274  (.            "t
+0000ada0: 6573 7474 626c 222c 0a20 2020 2020 2020  esttbl",.       
+0000adb0: 2020 2020 2072 6566 6c65 6374 6564 5f6d       reflected_m
+0000adc0: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
+0000add0: 2020 2020 2061 7574 6f6c 6f61 645f 7769       autoload_wi
+0000ade0: 7468 3d63 6f6e 6e65 6374 696f 6e2c 0a20  th=connection,. 
+0000adf0: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+0000ae00: 613d 7363 6865 6d61 2c0a 2020 2020 2020  a=schema,.      
+0000ae10: 2020 290a 0a20 2020 2020 2020 2023 2074    )..        # t
+0000ae20: 6573 7420 2264 6564 7570 6c69 6361 7465  est "deduplicate
+0000ae30: 7320 666f 7220 696e 6465 7822 206c 6f67  s for index" log
+0000ae40: 6963 2e20 2020 4d79 5351 4c20 616e 6420  ic.   MySQL and 
+0000ae50: 4f72 6163 6c65 0a20 2020 2020 2020 2023  Oracle.        #
+0000ae60: 2022 756e 6971 7565 2063 6f6e 7374 7261   "unique constra
+0000ae70: 696e 7473 2220 6172 6520 6163 7475 616c  ints" are actual
+0000ae80: 6c79 2075 6e69 7175 6520 696e 6465 7865  ly unique indexe
+0000ae90: 7320 2877 6974 6820 706f 7373 6962 6c65  s (with possible
+0000aea0: 0a20 2020 2020 2020 2023 2065 7863 6570  .        # excep
+0000aeb0: 7469 6f6e 206f 6620 6120 756e 6971 7565  tion of a unique
+0000aec0: 2074 6861 7420 6973 2061 2064 7570 6520   that is a dupe 
+0000aed0: 6f66 2061 6e6f 7468 6572 206f 6e65 2069  of another one i
+0000aee0: 6e20 7468 6520 6361 7365 0a20 2020 2020  n the case.     
+0000aef0: 2020 2023 206f 6620 4f72 6163 6c65 292e     # of Oracle).
+0000af00: 2020 6d61 6b65 2073 7572 6520 2320 7468    make sure # th
+0000af10: 6579 2061 7265 6e27 7420 6475 706c 6963  ey aren't duplic
+0000af20: 6174 6564 2e0a 2020 2020 2020 2020 6964  ated..        id
+0000af30: 785f 6e61 6d65 7320 3d20 7365 7428 5b69  x_names = set([i
+0000af40: 6478 2e6e 616d 6520 666f 7220 6964 7820  dx.name for idx 
+0000af50: 696e 2072 6566 6c65 6374 6564 2e69 6e64  in reflected.ind
+0000af60: 6578 6573 5d29 0a20 2020 2020 2020 2075  exes]).        u
+0000af70: 715f 6e61 6d65 7320 3d20 7365 7428 0a20  q_names = set(. 
+0000af80: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+0000af90: 2020 2020 2020 2020 2020 2020 2075 712e               uq.
+0000afa0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+0000afb0: 2020 2020 2066 6f72 2075 7120 696e 2072       for uq in r
+0000afc0: 6566 6c65 6374 6564 2e63 6f6e 7374 7261  eflected.constra
+0000afd0: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
+0000afe0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0000aff0: 6365 2875 712c 2073 716c 616c 6368 656d  ce(uq, sqlalchem
+0000b000: 792e 556e 6971 7565 436f 6e73 7472 6169  y.UniqueConstrai
+0000b010: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+0000b020: 5d0a 2020 2020 2020 2020 292e 6469 6666  ].        ).diff
+0000b030: 6572 656e 6365 285b 2275 6e69 7175 655f  erence(["unique_
+0000b040: 635f 615f 6222 5d29 0a0a 2020 2020 2020  c_a_b"])..      
+0000b050: 2020 6173 7365 7274 206e 6f74 2069 6478    assert not idx
+0000b060: 5f6e 616d 6573 2e69 6e74 6572 7365 6374  _names.intersect
+0000b070: 696f 6e28 7571 5f6e 616d 6573 290a 2020  ion(uq_names).  
+0000b080: 2020 2020 2020 6966 206e 616d 6573 5f74        if names_t
+0000b090: 6861 745f 6475 706c 6963 6174 655f 696e  hat_duplicate_in
+0000b0a0: 6465 783a 0a20 2020 2020 2020 2020 2020  dex:.           
+0000b0b0: 2065 715f 286e 616d 6573 5f74 6861 745f   eq_(names_that_
+0000b0c0: 6475 706c 6963 6174 655f 696e 6465 782c  duplicate_index,
+0000b0d0: 2069 6478 5f6e 616d 6573 290a 2020 2020   idx_names).    
+0000b0e0: 2020 2020 2020 2020 6571 5f28 7571 5f6e          eq_(uq_n
+0000b0f0: 616d 6573 2c20 7365 7428 2929 0a0a 2020  ames, set())..  
+0000b100: 2020 4074 6573 7469 6e67 2e70 726f 7669    @testing.provi
+0000b110: 6465 5f6d 6574 6164 6174 610a 2020 2020  de_metadata.    
+0000b120: 6465 6620 7465 7374 5f75 6e69 7175 655f  def test_unique_
+0000b130: 636f 6e73 7472 6169 6e74 5f72 6169 7365  constraint_raise
+0000b140: 7328 7365 6c66 2c20 636f 6e6e 6563 7469  s(self, connecti
+0000b150: 6f6e 293a 0a20 2020 2020 2020 2022 2222  on):.        """
+0000b160: 0a20 2020 2020 2020 2043 6865 636b 696e  .        Checkin
+0000b170: 6720 7468 6174 2075 6e69 7175 6520 636f  g that unique co
+0000b180: 6e73 7472 6169 6e74 2063 7265 6174 696f  nstraint creatio
+0000b190: 6e0a 2020 2020 2020 2020 6661 696c 7320  n.        fails 
+0000b1a0: 6475 6520 746f 2061 2050 726f 6772 616d  due to a Program
+0000b1b0: 6d69 6e67 4572 726f 722e 0a20 2020 2020  mingError..     
+0000b1c0: 2020 2022 2222 0a20 2020 2020 2020 206d     """.        m
+0000b1d0: 6574 6164 6174 6120 3d20 4d65 7461 4461  etadata = MetaDa
+0000b1e0: 7461 2829 0a20 2020 2020 2020 2054 6162  ta().        Tab
+0000b1f0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+0000b200: 2275 7365 725f 746d 705f 6661 696c 7572  "user_tmp_failur
+0000b210: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+0000b220: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+0000b230: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+0000b240: 222c 2073 716c 616c 6368 656d 792e 494e  ", sqlalchemy.IN
+0000b250: 542c 2070 7269 6d61 7279 5f6b 6579 3d54  T, primary_key=T
+0000b260: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+0000b270: 2020 436f 6c75 6d6e 2822 6e61 6d65 222c    Column("name",
+0000b280: 2073 716c 616c 6368 656d 792e 5641 5243   sqlalchemy.VARC
+0000b290: 4841 5228 3530 2929 2c0a 2020 2020 2020  HAR(50)),.      
+0000b2a0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+0000b2b0: 2e55 6e69 7175 6543 6f6e 7374 7261 696e  .UniqueConstrain
+0000b2c0: 7428 226e 616d 6522 2c20 6e61 6d65 3d22  t("name", name="
+0000b2d0: 7573 6572 5f74 6d70 5f75 7122 292c 0a20  user_tmp_uq"),. 
+0000b2e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000b2f0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+0000b300: 6973 6573 2873 7061 6e6e 6572 5f64 6261  ises(spanner_dba
+0000b310: 7069 2e65 7863 6570 7469 6f6e 732e 5072  pi.exceptions.Pr
+0000b320: 6f67 7261 6d6d 696e 6745 7272 6f72 293a  ogrammingError):
+0000b330: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0000b340: 6164 6174 612e 6372 6561 7465 5f61 6c6c  adata.create_all
+0000b350: 2863 6f6e 6e65 6374 696f 6e29 0a0a 2020  (connection)..  
+0000b360: 2020 4074 6573 7469 6e67 2e70 726f 7669    @testing.provi
+0000b370: 6465 5f6d 6574 6164 6174 610a 2020 2020  de_metadata.    
+0000b380: 6465 6620 5f74 6573 745f 6765 745f 7461  def _test_get_ta
+0000b390: 626c 655f 6e61 6d65 7328 7365 6c66 2c20  ble_names(self, 
+0000b3a0: 7363 6865 6d61 3d4e 6f6e 652c 2074 6162  schema=None, tab
+0000b3b0: 6c65 5f74 7970 653d 2274 6162 6c65 222c  le_type="table",
+0000b3c0: 206f 7264 6572 5f62 793d 4e6f 6e65 293a   order_by=None):
+0000b3d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000b3e0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
+0000b3f0: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
+0000b400: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
+0000b410: 7375 7070 6f72 7420 7465 6d70 6f72 6172  support temporar
+0000b420: 7920 7461 626c 6573 2c20 736f 2072 6561  y tables, so rea
+0000b430: 6c20 7461 626c 6573 2061 7265 0a20 2020  l tables are.   
+0000b440: 2020 2020 2075 7365 6420 666f 7220 7465       used for te
+0000b450: 7374 696e 672e 2041 7320 7468 6520 6f72  sting. As the or
+0000b460: 6967 696e 616c 2074 6573 7420 6578 7065  iginal test expe
+0000b470: 6374 7320 6f6e 6c79 2072 6561 6c0a 2020  cts only real.  
+0000b480: 2020 2020 2020 7461 626c 6573 2074 6f20        tables to 
+0000b490: 6265 2072 6561 642c 2061 6e64 2069 6e20  be read, and in 
+0000b4a0: 5370 616e 6e65 7220 616c 6c20 7468 6520  Spanner all the 
+0000b4b0: 7461 626c 6573 2061 7265 2072 6561 6c2c  tables are real,
+0000b4c0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+0000b4d0: 6420 7265 7375 6c74 7320 6f76 6572 7269  d results overri
+0000b4e0: 6465 2069 7320 7265 7175 6972 6564 2e0a  de is required..
+0000b4f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b500: 2020 2020 5f69 676e 6f72 655f 7461 626c      _ignore_tabl
+0000b510: 6573 203d 205b 0a20 2020 2020 2020 2020  es = [.         
+0000b520: 2020 2022 636f 6d6d 656e 745f 7465 7374     "comment_test
+0000b530: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000b540: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
+0000b550: 706b 222c 0a20 2020 2020 2020 2020 2020  pk",.           
+0000b560: 2022 6e6f 6e63 6f6c 5f69 6478 5f74 6573   "noncol_idx_tes
+0000b570: 745f 6e6f 706b 222c 0a20 2020 2020 2020  t_nopk",.       
+0000b580: 2020 2020 2022 6c6f 6361 6c5f 7461 626c       "local_tabl
+0000b590: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+0000b5a0: 2272 656d 6f74 655f 7461 626c 6522 2c0a  "remote_table",.
+0000b5b0: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
+0000b5c0: 6f74 655f 7461 626c 655f 3222 2c0a 2020  ote_table_2",.  
+0000b5d0: 2020 2020 2020 2020 2020 226e 6f5f 636f            "no_co
+0000b5e0: 6e73 7472 6169 6e74 7322 2c0a 2020 2020  nstraints",.    
+0000b5f0: 2020 2020 5d0a 2020 2020 2020 2020 6d65      ].        me
+0000b600: 7461 203d 2073 656c 662e 6d65 7461 6461  ta = self.metada
+0000b610: 7461 0a0a 2020 2020 2020 2020 696e 7370  ta..        insp
+0000b620: 203d 2069 6e73 7065 6374 286d 6574 612e   = inspect(meta.
+0000b630: 6269 6e64 290a 0a20 2020 2020 2020 2069  bind)..        i
+0000b640: 6620 7461 626c 655f 7479 7065 203d 3d20  f table_type == 
+0000b650: 2276 6965 7722 2061 6e64 206e 6f74 2062  "view" and not b
+0000b660: 6f6f 6c28 6f73 2e65 6e76 6972 6f6e 2e67  ool(os.environ.g
+0000b670: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
+0000b680: 4154 4f52 5f48 4f53 5422 2929 3a0a 2020  ATOR_HOST")):.  
+0000b690: 2020 2020 2020 2020 2020 7461 626c 655f            table_
+0000b6a0: 6e61 6d65 7320 3d20 696e 7370 2e67 6574  names = insp.get
+0000b6b0: 5f76 6965 775f 6e61 6d65 7328 7363 6865  _view_names(sche
+0000b6c0: 6d61 290a 2020 2020 2020 2020 2020 2020  ma).            
+0000b6d0: 7461 626c 655f 6e61 6d65 732e 736f 7274  table_names.sort
+0000b6e0: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
+0000b6f0: 6e73 7765 7220 3d20 5b22 656d 6169 6c5f  nswer = ["email_
+0000b700: 6164 6472 6573 7365 735f 7622 2c20 2275  addresses_v", "u
+0000b710: 7365 7273 5f76 225d 0a20 2020 2020 2020  sers_v"].       
+0000b720: 2020 2020 2065 715f 2873 6f72 7465 6428       eq_(sorted(
+0000b730: 7461 626c 655f 6e61 6d65 7329 2c20 616e  table_names), an
+0000b740: 7377 6572 290a 2020 2020 2020 2020 656c  swer).        el
+0000b750: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000b760: 6966 206f 7264 6572 5f62 793a 0a20 2020  if order_by:.   
+0000b770: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+0000b780: 6c65 7320 3d20 5b0a 2020 2020 2020 2020  les = [.        
+0000b790: 2020 2020 2020 2020 2020 2020 7265 635b              rec[
+0000b7a0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0000b7b0: 2020 2020 2020 2066 6f72 2072 6563 2069         for rec i
+0000b7c0: 6e20 696e 7370 2e67 6574 5f73 6f72 7465  n insp.get_sorte
+0000b7d0: 645f 7461 626c 655f 616e 645f 666b 635f  d_table_and_fkc_
+0000b7e0: 6e61 6d65 7328 7363 6865 6d61 290a 2020  names(schema).  
+0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b800: 2020 6966 2072 6563 5b30 5d0a 2020 2020    if rec[0].    
+0000b810: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+0000b820: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b840: 7461 626c 6573 203d 2069 6e73 702e 6765  tables = insp.ge
+0000b850: 745f 7461 626c 655f 6e61 6d65 7328 7363  t_table_names(sc
+0000b860: 6865 6d61 290a 2020 2020 2020 2020 2020  hema).          
+0000b870: 2020 7461 626c 655f 6e61 6d65 7320 3d20    table_names = 
+0000b880: 5b74 2066 6f72 2074 2069 6e20 7461 626c  [t for t in tabl
+0000b890: 6573 2069 6620 7420 6e6f 7420 696e 205f  es if t not in _
+0000b8a0: 6967 6e6f 7265 5f74 6162 6c65 735d 0a0a  ignore_tables]..
+0000b8b0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+0000b8c0: 7264 6572 5f62 7920 3d3d 2022 666f 7265  rder_by == "fore
+0000b8d0: 6967 6e5f 6b65 7922 3a0a 2020 2020 2020  ign_key":.      
+0000b8e0: 2020 2020 2020 2020 2020 616e 7377 6572            answer
+0000b8f0: 203d 207b 2264 696e 6761 6c69 6e67 7322   = {"dingalings"
+0000b900: 2c20 2265 6d61 696c 5f61 6464 7265 7373  , "email_address
+0000b910: 6573 222c 2022 7573 6572 5f74 6d70 222c  es", "user_tmp",
+0000b920: 2022 7573 6572 7322 7d0a 2020 2020 2020   "users"}.      
+0000b930: 2020 2020 2020 2020 2020 6571 5f28 7365            eq_(se
+0000b940: 7428 7461 626c 655f 6e61 6d65 7329 2c20  t(table_names), 
+0000b950: 616e 7377 6572 290a 2020 2020 2020 2020  answer).        
+0000b960: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000b970: 2020 2020 2020 2020 2020 616e 7377 6572            answer
+0000b980: 203d 205b 2264 696e 6761 6c69 6e67 7322   = ["dingalings"
+0000b990: 2c20 2265 6d61 696c 5f61 6464 7265 7373  , "email_address
+0000b9a0: 6573 222c 2022 7573 6572 5f74 6d70 222c  es", "user_tmp",
+0000b9b0: 2022 7573 6572 7322 5d0a 2020 2020 2020   "users"].      
+0000b9c0: 2020 2020 2020 2020 2020 6571 5f28 736f            eq_(so
+0000b9d0: 7274 6564 2874 6162 6c65 5f6e 616d 6573  rted(table_names
+0000b9e0: 292c 2061 6e73 7765 7229 0a0a 2020 2020  ), answer)..    
+0000b9f0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000ba00: 7069 6628 0a20 2020 2020 2020 2062 6f6f  pif(.        boo
+0000ba10: 6c28 6f73 2e65 6e76 6972 6f6e 2e67 6574  l(os.environ.get
+0000ba20: 2822 5350 414e 4e45 525f 454d 554c 4154  ("SPANNER_EMULAT
+0000ba30: 4f52 5f48 4f53 5422 2929 2c20 7265 6173  OR_HOST")), reas
+0000ba40: 6f6e 3d22 536b 6970 7065 6420 6f6e 2065  on="Skipped on e
+0000ba50: 6d75 6c61 746f 7222 0a20 2020 2029 0a20  mulator".    ). 
+0000ba60: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
+0000ba70: 7669 6577 5f6e 616d 6573 2873 656c 662c  view_names(self,
+0000ba80: 2063 6f6e 6e65 6374 696f 6e2c 2075 7365   connection, use
+0000ba90: 5f73 6368 656d 613d 4661 6c73 6529 3a0a  _schema=False):.
+0000baa0: 2020 2020 2020 2020 696e 7370 203d 2069          insp = i
+0000bab0: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
+0000bac0: 6e29 0a20 2020 2020 2020 2073 6368 656d  n).        schem
+0000bad0: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
+0000bae0: 2074 6162 6c65 5f6e 616d 6573 203d 2069   table_names = i
+0000baf0: 6e73 702e 6765 745f 7669 6577 5f6e 616d  nsp.get_view_nam
+0000bb00: 6573 2873 6368 656d 6129 0a20 2020 2020  es(schema).     
+0000bb10: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
+0000bb20: 7175 6972 6573 2e6d 6174 6572 6961 6c69  quires.materiali
+0000bb30: 7a65 645f 7669 6577 732e 656e 6162 6c65  zed_views.enable
+0000bb40: 643a 0a20 2020 2020 2020 2020 2020 2065  d:.            e
+0000bb50: 715f 2873 6f72 7465 6428 7461 626c 655f  q_(sorted(table_
+0000bb60: 6e61 6d65 7329 2c20 5b22 656d 6169 6c5f  names), ["email_
+0000bb70: 6164 6472 6573 7365 735f 7622 2c20 2275  addresses_v", "u
+0000bb80: 7365 7273 5f76 225d 290a 2020 2020 2020  sers_v"]).      
+0000bb90: 2020 2020 2020 6571 5f28 696e 7370 2e67        eq_(insp.g
+0000bba0: 6574 5f6d 6174 6572 6961 6c69 7a65 645f  et_materialized_
+0000bbb0: 7669 6577 5f6e 616d 6573 2873 6368 656d  view_names(schem
+0000bbc0: 6129 2c20 5b22 6469 6e67 616c 696e 6773  a), ["dingalings
+0000bbd0: 5f76 225d 290a 2020 2020 2020 2020 656c  _v"]).        el
+0000bbe0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000bbf0: 616e 7377 6572 203d 205b 2264 696e 6761  answer = ["dinga
+0000bc00: 6c69 6e67 735f 7622 2c20 2265 6d61 696c  lings_v", "email
+0000bc10: 5f61 6464 7265 7373 6573 5f76 222c 2022  _addresses_v", "
+0000bc20: 7573 6572 735f 7622 5d0a 2020 2020 2020  users_v"].      
+0000bc30: 2020 2020 2020 6571 5f28 736f 7274 6564        eq_(sorted
+0000bc40: 2874 6162 6c65 5f6e 616d 6573 292c 2061  (table_names), a
+0000bc50: 6e73 7765 7229 0a0a 2020 2020 4070 7974  nswer)..    @pyt
+0000bc60: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
+0000bc70: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
+0000bc80: 7570 706f 7274 2074 656d 706f 7261 7279  upport temporary
+0000bc90: 2074 6162 6c65 7322 290a 2020 2020 6465   tables").    de
+0000bca0: 6620 7465 7374 5f67 6574 5f74 656d 705f  f test_get_temp_
+0000bcb0: 7461 626c 655f 696e 6465 7865 7328 7365  table_indexes(se
+0000bcc0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0000bcd0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+0000bce0: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+0000bcf0: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000bd00: 7420 7465 6d70 6f72 6172 7920 7461 626c  t temporary tabl
+0000bd10: 6573 2229 0a20 2020 2064 6566 2074 6573  es").    def tes
+0000bd20: 745f 6765 745f 7465 6d70 5f74 6162 6c65  t_get_temp_table
+0000bd30: 5f75 6e69 7175 655f 636f 6e73 7472 6169  _unique_constrai
+0000bd40: 6e74 7328 7365 6c66 293a 0a20 2020 2020  nts(self):.     
+0000bd50: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
+0000bd60: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
+0000bd70: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
+0000bd80: 7375 7070 6f72 7420 7465 6d70 6f72 6172  support temporar
+0000bd90: 7920 7461 626c 6573 2229 0a20 2020 2064  y tables").    d
+0000bda0: 6566 2074 6573 745f 6765 745f 7465 6d70  ef test_get_temp
+0000bdb0: 5f74 6162 6c65 5f63 6f6c 756d 6e73 2873  _table_columns(s
+0000bdc0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0000bdd0: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+0000bde0: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
+0000bdf0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+0000be00: 7274 2074 656d 706f 7261 7279 2074 6162  rt temporary tab
+0000be10: 6c65 7322 290a 2020 2020 6465 6620 7465  les").    def te
+0000be20: 7374 5f72 6566 6c65 6374 5f74 6162 6c65  st_reflect_table
+0000be30: 5f74 656d 705f 7461 626c 6528 7365 6c66  _temp_table(self
+0000be40: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+0000be50: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000be60: 2064 6566 2065 7870 5f69 6e64 6578 6573   def exp_indexes
+0000be70: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000be80: 2020 2020 2020 2020 7363 6865 6d61 3d4e          schema=N
+0000be90: 6f6e 652c 0a20 2020 2020 2020 2073 636f  one,.        sco
+0000bea0: 7065 3d4f 626a 6563 7453 636f 7065 2e41  pe=ObjectScope.A
+0000beb0: 4e59 2c0a 2020 2020 2020 2020 6b69 6e64  NY,.        kind
+0000bec0: 3d4f 626a 6563 744b 696e 642e 414e 592c  =ObjectKind.ANY,
+0000bed0: 0a20 2020 2020 2020 2066 696c 7465 725f  .        filter_
+0000bee0: 6e61 6d65 733d 4e6f 6e65 2c0a 2020 2020  names=None,.    
+0000bef0: 293a 0a20 2020 2020 2020 2064 6566 2069  ):.        def i
+0000bf00: 6478 280a 2020 2020 2020 2020 2020 2020  dx(.            
+0000bf10: 2a63 6f6c 732c 0a20 2020 2020 2020 2020  *cols,.         
+0000bf20: 2020 206e 616d 652c 0a20 2020 2020 2020     name,.       
+0000bf30: 2020 2020 2075 6e69 7175 653d 4661 6c73       unique=Fals
+0000bf40: 652c 0a20 2020 2020 2020 2020 2020 2063  e,.            c
+0000bf50: 6f6c 756d 6e5f 736f 7274 696e 673d 4e6f  olumn_sorting=No
+0000bf60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000bf70: 6475 706c 6963 6174 6573 3d46 616c 7365  duplicates=False
+0000bf80: 2c0a 2020 2020 2020 2020 2020 2020 666b  ,.            fk
+0000bf90: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000bfa0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+0000bfb0: 6b5f 7265 7120 3d20 7465 7374 696e 672e  k_req = testing.
+0000bfc0: 7265 7175 6972 6573 2e66 6f72 6569 676e  requires.foreign
+0000bfd0: 5f6b 6579 735f 7265 666c 6563 745f 6173  _keys_reflect_as
+0000bfe0: 5f69 6e64 6578 0a20 2020 2020 2020 2020  _index.         
+0000bff0: 2020 2064 7570 5f72 6571 203d 2074 6573     dup_req = tes
+0000c000: 7469 6e67 2e72 6571 7569 7265 732e 756e  ting.requires.un
+0000c010: 6971 7565 5f63 6f6e 7374 7261 696e 7473  ique_constraints
+0000c020: 5f72 6566 6c65 6374 5f61 735f 696e 6465  _reflect_as_inde
+0000c030: 780a 2020 2020 2020 2020 2020 2020 6966  x.            if
+0000c040: 2028 666b 2061 6e64 206e 6f74 2066 6b5f   (fk and not fk_
+0000c050: 7265 712e 656e 6162 6c65 6429 206f 7220  req.enabled) or 
+0000c060: 2864 7570 6c69 6361 7465 7320 616e 6420  (duplicates and 
+0000c070: 6e6f 7420 6475 705f 7265 712e 656e 6162  not dup_req.enab
+0000c080: 6c65 6429 3a0a 2020 2020 2020 2020 2020  led):.          
+0000c090: 2020 2020 2020 7265 7475 726e 2028 290a        return ().
+0000c0a0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+0000c0b0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0000c0c0: 2020 2020 2275 6e69 7175 6522 3a20 756e      "unique": un
+0000c0d0: 6971 7565 2c0a 2020 2020 2020 2020 2020  ique,.          
+0000c0e0: 2020 2020 2020 2263 6f6c 756d 6e5f 6e61        "column_na
+0000c0f0: 6d65 7322 3a20 6c69 7374 2863 6f6c 7329  mes": list(cols)
+0000c100: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c110: 2020 226e 616d 6522 3a20 6e61 6d65 2c0a    "name": name,.
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 2264 6961 6c65 6374 5f6f 7074 696f 6e73  "dialect_options
+0000c140: 223a 206d 6f63 6b2e 414e 592c 0a20 2020  ": mock.ANY,.   
+0000c150: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+0000c160: 636c 7564 655f 636f 6c75 6d6e 7322 3a20  clude_columns": 
+0000c170: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+0000c180: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+0000c190: 2063 6f6c 756d 6e5f 736f 7274 696e 673a   column_sorting:
+0000c1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1b0: 2072 6573 5b22 636f 6c75 6d6e 5f73 6f72   res["column_sor
+0000c1c0: 7469 6e67 225d 203d 207b 2271 223a 2022  ting"] = {"q": "
+0000c1d0: 4445 5343 227d 0a20 2020 2020 2020 2020  DESC"}.         
+0000c1e0: 2020 2069 6620 6475 706c 6963 6174 6573     if duplicates
+0000c1f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c200: 2020 7265 735b 2264 7570 6c69 6361 7465    res["duplicate
+0000c210: 735f 636f 6e73 7472 6169 6e74 225d 203d  s_constraint"] =
+0000c220: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+0000c230: 2020 7265 7475 726e 205b 7265 735d 0a0a    return [res]..
+0000c240: 2020 2020 2020 2020 6d61 7465 7269 616c          material
+0000c250: 697a 6564 203d 207b 2873 6368 656d 612c  ized = {(schema,
+0000c260: 2022 6469 6e67 616c 696e 6773 5f76 2229   "dingalings_v")
+0000c270: 3a20 5b5d 7d0a 2020 2020 2020 2020 7669  : []}.        vi
+0000c280: 6577 7320 3d20 7b0a 2020 2020 2020 2020  ews = {.        
+0000c290: 2020 2020 2873 6368 656d 612c 2022 656d      (schema, "em
+0000c2a0: 6169 6c5f 6164 6472 6573 7365 735f 7622  ail_addresses_v"
+0000c2b0: 293a 205b 5d2c 0a20 2020 2020 2020 2020  ): [],.         
+0000c2c0: 2020 2028 7363 6865 6d61 2c20 2275 7365     (schema, "use
+0000c2d0: 7273 5f76 2229 3a20 5b5d 2c0a 2020 2020  rs_v"): [],.    
+0000c2e0: 2020 2020 2020 2020 2873 6368 656d 612c          (schema,
+0000c2f0: 2022 7573 6572 5f74 6d70 5f76 2229 3a20   "user_tmp_v"): 
+0000c300: 5b5d 2c0a 2020 2020 2020 2020 7d0a 2020  [],.        }.  
+0000c310: 2020 2020 2020 7365 6c66 2e5f 7265 736f        self._reso
+0000c320: 6c76 655f 7669 6577 7328 7669 6577 732c  lve_views(views,
+0000c330: 206d 6174 6572 6961 6c69 7a65 6429 0a20   materialized). 
+0000c340: 2020 2020 2020 2069 6620 6d61 7465 7269         if materi
+0000c350: 616c 697a 6564 3a0a 2020 2020 2020 2020  alized:.        
+0000c360: 2020 2020 6d61 7465 7269 616c 697a 6564      materialized
+0000c370: 5b28 7363 6865 6d61 2c20 2264 696e 6761  [(schema, "dinga
+0000c380: 6c69 6e67 735f 7622 295d 2e65 7874 656e  lings_v")].exten
+0000c390: 6428 6964 7828 2264 6174 6122 2c20 6e61  d(idx("data", na
+0000c3a0: 6d65 3d22 6d61 745f 696e 6465 7822 2929  me="mat_index"))
+0000c3b0: 0a20 2020 2020 2020 2074 6162 6c65 7320  .        tables 
+0000c3c0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0000c3d0: 2873 6368 656d 612c 2022 7573 6572 7322  (schema, "users"
+0000c3e0: 293a 205b 0a20 2020 2020 2020 2020 2020  ): [.           
+0000c3f0: 2020 2020 202a 6964 7828 2270 6172 656e       *idx("paren
+0000c400: 745f 7573 6572 5f69 6422 2c20 6e61 6d65  t_user_id", name
+0000c410: 3d22 7573 6572 5f69 645f 666b 222c 2066  ="user_id_fk", f
+0000c420: 6b3d 5472 7565 292c 0a20 2020 2020 2020  k=True),.       
+0000c430: 2020 2020 2020 2020 202a 6964 7828 2275           *idx("u
+0000c440: 7365 725f 6964 222c 2022 7465 7374 3222  ser_id", "test2"
+0000c450: 2c20 2274 6573 7431 222c 206e 616d 653d  , "test1", name=
+0000c460: 2275 7365 7273 5f61 6c6c 5f69 6478 2229  "users_all_idx")
+0000c470: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c480: 2020 2a69 6478 2822 7465 7374 3122 2c20    *idx("test1", 
+0000c490: 2274 6573 7432 222c 206e 616d 653d 2275  "test2", name="u
+0000c4a0: 7365 7273 5f74 5f69 6478 222c 2075 6e69  sers_t_idx", uni
+0000c4b0: 7175 653d 5472 7565 292c 0a20 2020 2020  que=True),.     
+0000c4c0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+0000c4d0: 2020 2020 2020 2873 6368 656d 612c 2022        (schema, "
+0000c4e0: 6469 6e67 616c 696e 6773 2229 3a20 5b0a  dingalings"): [.
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c500: 2a69 6478 2822 6461 7461 222c 206e 616d  *idx("data", nam
+0000c510: 653d 6d6f 636b 2e41 4e59 2c20 756e 6971  e=mock.ANY, uniq
+0000c520: 7565 3d54 7275 652c 2064 7570 6c69 6361  ue=True, duplica
+0000c530: 7465 733d 5472 7565 292c 0a20 2020 2020  tes=True),.     
+0000c540: 2020 2020 2020 2020 2020 202a 6964 7828             *idx(
+0000c550: 2269 645f 7573 6572 222c 206e 616d 653d  "id_user", name=
+0000c560: 6d6f 636b 2e41 4e59 2c20 666b 3d54 7275  mock.ANY, fk=Tru
+0000c570: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000c580: 2020 2020 2a69 6478 280a 2020 2020 2020      *idx(.      
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+0000c5a0: 6464 7265 7373 5f69 6422 2c0a 2020 2020  ddress_id",.    
+0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5c0: 2264 696e 6761 6c69 6e67 5f69 6422 2c0a  "dingaling_id",.
+0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 2020 2020 6e61 6d65 3d22 7a7a 5f64 696e      name="zz_din
+0000c5f0: 6761 6c69 6e67 735f 6d75 6c74 6970 6c65  galings_multiple
+0000c600: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000c610: 2020 2020 2020 2075 6e69 7175 653d 5472         unique=Tr
+0000c620: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000c630: 2020 2020 2020 2020 6475 706c 6963 6174          duplicat
+0000c640: 6573 3d54 7275 652c 0a20 2020 2020 2020  es=True,.       
+0000c650: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+0000c660: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000c670: 2020 2020 2020 2028 7363 6865 6d61 2c20         (schema, 
+0000c680: 2265 6d61 696c 5f61 6464 7265 7373 6573  "email_addresses
+0000c690: 2229 3a20 5b0a 2020 2020 2020 2020 2020  "): [.          
+0000c6a0: 2020 2020 2020 2a69 6478 2822 656d 6169        *idx("emai
+0000c6b0: 6c5f 6164 6472 6573 7322 2c20 6e61 6d65  l_address", name
+0000c6c0: 3d6d 6f63 6b2e 414e 5929 2c0a 2020 2020  =mock.ANY),.    
+0000c6d0: 2020 2020 2020 2020 2020 2020 2a69 6478              *idx
+0000c6e0: 2822 7265 6d6f 7465 5f75 7365 725f 6964  ("remote_user_id
+0000c6f0: 222c 206e 616d 653d 6d6f 636b 2e41 4e59  ", name=mock.ANY
+0000c700: 2c20 666b 3d54 7275 6529 2c0a 2020 2020  , fk=True),.    
+0000c710: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000c720: 2020 2020 2020 2028 7363 6865 6d61 2c20         (schema, 
+0000c730: 2263 6f6d 6d65 6e74 5f74 6573 7422 293a  "comment_test"):
+0000c740: 205b 5d2c 0a20 2020 2020 2020 2020 2020   [],.           
+0000c750: 2028 7363 6865 6d61 2c20 226e 6f5f 636f   (schema, "no_co
+0000c760: 6e73 7472 6169 6e74 7322 293a 205b 5d2c  nstraints"): [],
+0000c770: 0a20 2020 2020 2020 2020 2020 2028 7363  .            (sc
+0000c780: 6865 6d61 2c20 226c 6f63 616c 5f74 6162  hema, "local_tab
+0000c790: 6c65 2229 3a20 5b2a 6964 7828 2272 656d  le"): [*idx("rem
+0000c7a0: 6f74 655f 6964 222c 206e 616d 653d 6d6f  ote_id", name=mo
+0000c7b0: 636b 2e41 4e59 2c20 666b 3d54 7275 6529  ck.ANY, fk=True)
+0000c7c0: 5d2c 0a20 2020 2020 2020 2020 2020 2028  ],.            (
+0000c7d0: 7363 6865 6d61 2c20 2272 656d 6f74 655f  schema, "remote_
+0000c7e0: 7461 626c 6522 293a 205b 2a69 6478 2822  table"): [*idx("
+0000c7f0: 6c6f 6361 6c5f 6964 222c 206e 616d 653d  local_id", name=
+0000c800: 6d6f 636b 2e41 4e59 2c20 666b 3d54 7275  mock.ANY, fk=Tru
+0000c810: 6529 5d2c 0a20 2020 2020 2020 2020 2020  e)],.           
+0000c820: 2028 7363 6865 6d61 2c20 2272 656d 6f74   (schema, "remot
+0000c830: 655f 7461 626c 655f 3222 293a 205b 5d2c  e_table_2"): [],
+0000c840: 0a20 2020 2020 2020 2020 2020 2028 7363  .            (sc
+0000c850: 6865 6d61 2c20 226e 6f6e 636f 6c5f 6964  hema, "noncol_id
+0000c860: 785f 7465 7374 5f6e 6f70 6b22 293a 205b  x_test_nopk"): [
+0000c870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c880: 202a 6964 7828 0a20 2020 2020 2020 2020   *idx(.         
+0000c890: 2020 2020 2020 2020 2020 2022 7122 2c0a             "q",.
+0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8b0: 2020 2020 6e61 6d65 3d22 6e6f 6e63 6f6c      name="noncol
+0000c8c0: 5f69 6478 5f6e 6f70 6b22 2c0a 2020 2020  _idx_nopk",.    
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 636f 6c75 6d6e 5f73 6f72 7469 6e67 3d7b  column_sorting={
+0000c8f0: 2271 223a 2022 4445 5343 227d 2c0a 2020  "q": "DESC"},.  
+0000c900: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000c910: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+0000c920: 2020 2020 2020 2020 2020 2028 7363 6865             (sche
+0000c930: 6d61 2c20 226e 6f6e 636f 6c5f 6964 785f  ma, "noncol_idx_
+0000c940: 7465 7374 5f70 6b22 293a 205b 0a20 2020  test_pk"): [.   
+0000c950: 2020 2020 2020 2020 2020 2020 202a 6964               *id
+0000c960: 7828 2271 222c 206e 616d 653d 226e 6f6e  x("q", name="non
+0000c970: 636f 6c5f 6964 785f 706b 222c 2063 6f6c  col_idx_pk", col
+0000c980: 756d 6e5f 736f 7274 696e 673d 7b22 7122  umn_sorting={"q"
+0000c990: 3a20 2244 4553 4322 7d29 0a20 2020 2020  : "DESC"}).     
+0000c9a0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+0000c9b0: 2020 2020 2020 2873 6368 656d 612c 2073        (schema, s
+0000c9c0: 656c 662e 7465 6d70 5f74 6162 6c65 5f6e  elf.temp_table_n
+0000c9d0: 616d 6528 2929 3a20 5b0a 2020 2020 2020  ame()): [.      
+0000c9e0: 2020 2020 2020 2020 2020 2a69 6478 2822            *idx("
+0000c9f0: 666f 6f22 2c20 6e61 6d65 3d22 7573 6572  foo", name="user
+0000ca00: 5f74 6d70 5f69 7822 292c 0a20 2020 2020  _tmp_ix"),.     
+0000ca10: 2020 2020 2020 2020 2020 202a 6964 7828             *idx(
+0000ca20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca30: 2020 2020 2022 6e61 6d65 222c 0a20 2020       "name",.   
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca50: 206e 616d 653d 6622 7573 6572 5f74 6d70   name=f"user_tmp
+0000ca60: 5f75 715f 7b63 6f6e 6669 672e 6964 656e  _uq_{config.iden
+0000ca70: 747d 222c 0a20 2020 2020 2020 2020 2020  t}",.           
+0000ca80: 2020 2020 2020 2020 2064 7570 6c69 6361           duplica
+0000ca90: 7465 733d 5472 7565 2c0a 2020 2020 2020  tes=True,.      
+0000caa0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+0000cab0: 6971 7565 3d54 7275 652c 0a20 2020 2020  ique=True,.     
+0000cac0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+0000cad0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+0000cae0: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
+0000caf0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+0000cb00: 6e6f 7420 7465 7374 696e 672e 7265 7175  not testing.requ
+0000cb10: 6972 6573 2e69 6e64 6578 6573 5f77 6974  ires.indexes_wit
+0000cb20: 685f 6173 6364 6573 632e 656e 6162 6c65  h_ascdesc.enable
+0000cb30: 640a 2020 2020 2020 2020 2020 2020 6f72  d.            or
+0000cb40: 206e 6f74 2074 6573 7469 6e67 2e72 6571   not testing.req
+0000cb50: 7569 7265 732e 7265 666c 6563 745f 696e  uires.reflect_in
+0000cb60: 6465 7865 735f 7769 7468 5f61 7363 6465  dexes_with_ascde
+0000cb70: 7363 2e65 6e61 626c 6564 0a20 2020 2020  sc.enabled.     
+0000cb80: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0000cb90: 2020 7461 626c 6573 5b28 7363 6865 6d61    tables[(schema
+0000cba0: 2c20 226e 6f6e 636f 6c5f 6964 785f 7465  , "noncol_idx_te
+0000cbb0: 7374 5f6e 6f70 6b22 295d 2e63 6c65 6172  st_nopk")].clear
+0000cbc0: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
+0000cbd0: 6162 6c65 735b 2873 6368 656d 612c 2022  ables[(schema, "
+0000cbe0: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
+0000cbf0: 706b 2229 5d2e 636c 6561 7228 290a 2020  pk")].clear().  
+0000cc00: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+0000cc10: 2e5f 7265 736f 6c76 655f 6b69 6e64 286b  ._resolve_kind(k
+0000cc20: 696e 642c 2074 6162 6c65 732c 2076 6965  ind, tables, vie
+0000cc30: 7773 2c20 6d61 7465 7269 616c 697a 6564  ws, materialized
+0000cc40: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
+0000cc50: 7365 6c66 2e5f 7265 736f 6c76 655f 6e61  self._resolve_na
+0000cc60: 6d65 7328 7363 6865 6d61 2c20 7363 6f70  mes(schema, scop
+0000cc70: 652c 2066 696c 7465 725f 6e61 6d65 732c  e, filter_names,
+0000cc80: 2072 6573 290a 2020 2020 2020 2020 7265   res).        re
+0000cc90: 7475 726e 2072 6573 0a0a 2020 2020 6465  turn res..    de
+0000cca0: 6620 5f63 6865 636b 5f6c 6973 7428 7365  f _check_list(se
+0000ccb0: 6c66 2c20 7265 7375 6c74 2c20 6578 702c  lf, result, exp,
+0000ccc0: 2072 6571 5f6b 6579 733d 4e6f 6e65 2c20   req_keys=None, 
+0000ccd0: 6d73 673d 4e6f 6e65 293a 0a20 2020 2020  msg=None):.     
+0000cce0: 2020 2069 6620 7265 715f 6b65 7973 2069     if req_keys i
+0000ccf0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000cd00: 2020 2020 6571 5f28 7265 7375 6c74 2c20      eq_(result, 
+0000cd10: 6578 702c 206d 7367 290a 2020 2020 2020  exp, msg).      
+0000cd20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000cd30: 2020 2020 6571 5f28 6c65 6e28 7265 7375      eq_(len(resu
+0000cd40: 6c74 292c 206c 656e 2865 7870 292c 206d  lt), len(exp), m
+0000cd50: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
+0000cd60: 666f 7220 722c 2065 2069 6e20 7a69 7028  for r, e in zip(
+0000cd70: 7265 7375 6c74 2c20 6578 7029 3a0a 2020  result, exp):.  
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000cd90: 7220 6b20 696e 2073 6574 2872 2920 7c20  r k in set(r) | 
+0000cda0: 7365 7428 6529 3a0a 2020 2020 2020 2020  set(e):.        
+0000cdb0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0000cdc0: 6b20 696e 2072 6571 5f6b 6579 7320 616e  k in req_keys an
+0000cdd0: 6420 286b 2069 6e20 7220 616e 6420 6b20  d (k in r and k 
+0000cde0: 696e 2065 2929 206f 7220 286b 2069 6e20  in e)) or (k in 
+0000cdf0: 7220 616e 6420 6b20 696e 2065 293a 0a20  r and k in e):. 
+0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce10: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000ce20: 616e 6365 2872 5b6b 5d2c 206c 6973 7429  ance(r[k], list)
+0000ce30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ce40: 2020 2020 2020 2020 2020 2020 2020 725b                r[
+0000ce50: 6b5d 2e73 6f72 7428 290a 2020 2020 2020  k].sort().      
+0000ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce70: 2020 2020 2020 655b 6b5d 2e73 6f72 7428        e[k].sort(
+0000ce80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ce90: 2020 2020 2020 2020 2020 6571 5f28 725b            eq_(r[
+0000cea0: 6b5d 2c20 655b 6b5d 2c20 6622 7b6d 7367  k], e[k], f"{msg
+0000ceb0: 7d20 2d20 7b6b 7d20 2d20 7b72 7d22 290a  } - {k} - {r}").
+0000cec0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0000ced0: 6b2e 736b 6970 6966 280a 2020 2020 2020  k.skipif(.      
+0000cee0: 2020 626f 6f6c 286f 732e 656e 7669 726f    bool(os.enviro
+0000cef0: 6e2e 6765 7428 2253 5041 4e4e 4552 5f45  n.get("SPANNER_E
+0000cf00: 4d55 4c41 544f 525f 484f 5354 2229 292c  MULATOR_HOST")),
+0000cf10: 2072 6561 736f 6e3d 2253 6b69 7070 6564   reason="Skipped
+0000cf20: 206f 6e20 656d 756c 6174 6f72 220a 2020   on emulator".  
+0000cf30: 2020 290a 2020 2020 4074 6573 7469 6e67    ).    @testing
+0000cf40: 2e63 6f6d 6269 6e61 7469 6f6e 7328 5472  .combinations(Tr
+0000cf50: 7565 2c20 4661 6c73 652c 2061 7267 6e61  ue, False, argna
+0000cf60: 6d65 733d 2275 7365 5f73 6368 656d 6122  mes="use_schema"
+0000cf70: 290a 2020 2020 4074 6573 7469 6e67 2e63  ).    @testing.c
+0000cf80: 6f6d 6269 6e61 7469 6f6e 7328 2854 7275  ombinations((Tru
+0000cf90: 652c 2074 6573 7469 6e67 2e72 6571 7569  e, testing.requi
+0000cfa0: 7265 732e 7669 6577 7329 2c20 4661 6c73  res.views), Fals
+0000cfb0: 652c 2061 7267 6e61 6d65 733d 2276 6965  e, argnames="vie
+0000cfc0: 7773 2229 0a20 2020 2064 6566 2074 6573  ws").    def tes
+0000cfd0: 745f 6d65 7461 6461 7461 2873 656c 662c  t_metadata(self,
+0000cfe0: 2063 6f6e 6e65 6374 696f 6e2c 2075 7365   connection, use
+0000cff0: 5f73 6368 656d 612c 2076 6965 7773 293a  _schema, views):
+0000d000: 0a20 2020 2020 2020 206d 203d 204d 6574  .        m = Met
+0000d010: 6144 6174 6128 290a 2020 2020 2020 2020  aData().        
+0000d020: 7363 6865 6d61 203d 204e 6f6e 650a 2020  schema = None.  
+0000d030: 2020 2020 2020 6d2e 7265 666c 6563 7428        m.reflect(
+0000d040: 636f 6e6e 6563 7469 6f6e 2c20 7363 6865  connection, sche
+0000d050: 6d61 3d73 6368 656d 612c 2076 6965 7773  ma=schema, views
+0000d060: 3d76 6965 7773 2c20 7265 736f 6c76 655f  =views, resolve_
+0000d070: 666b 733d 4661 6c73 6529 0a0a 2020 2020  fks=False)..    
+0000d080: 2020 2020 696e 7370 203d 2069 6e73 7065      insp = inspe
+0000d090: 6374 2863 6f6e 6e65 6374 696f 6e29 0a20  ct(connection). 
+0000d0a0: 2020 2020 2020 2074 6162 6c65 7320 3d20         tables = 
+0000d0b0: 696e 7370 2e67 6574 5f74 6162 6c65 5f6e  insp.get_table_n
+0000d0c0: 616d 6573 2873 6368 656d 6129 0a20 2020  ames(schema).   
+0000d0d0: 2020 2020 2069 6620 7669 6577 733a 0a20       if views:. 
+0000d0e0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0000d0f0: 7320 2b3d 2069 6e73 702e 6765 745f 7669  s += insp.get_vi
+0000d100: 6577 5f6e 616d 6573 2873 6368 656d 6129  ew_names(schema)
+0000d110: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+0000d120: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d130: 2020 7461 626c 6573 202b 3d20 696e 7370    tables += insp
+0000d140: 2e67 6574 5f6d 6174 6572 6961 6c69 7a65  .get_materialize
+0000d150: 645f 7669 6577 5f6e 616d 6573 2873 6368  d_view_names(sch
+0000d160: 656d 6129 0a20 2020 2020 2020 2020 2020  ema).           
+0000d170: 2065 7863 6570 7420 4e6f 7449 6d70 6c65   except NotImple
+0000d180: 6d65 6e74 6564 4572 726f 723a 0a20 2020  mentedError:.   
+0000d190: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+0000d1a0: 730a 2020 2020 2020 2020 6966 2073 6368  s.        if sch
+0000d1b0: 656d 6120 6973 206e 6f74 204e 6f6e 653a  ema is not None:
+0000d1c0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+0000d1d0: 6c65 7320 3d20 5b66 227b 7363 6865 6d61  les = [f"{schema
+0000d1e0: 7d2e 7b74 7d22 2066 6f72 2074 2069 6e20  }.{t}" for t in 
+0000d1f0: 7461 626c 6573 5d0a 2020 2020 2020 2020  tables].        
+0000d200: 6571 5f28 736f 7274 6564 286d 2e74 6162  eq_(sorted(m.tab
+0000d210: 6c65 7329 2c20 736f 7274 6564 2874 6162  les), sorted(tab
+0000d220: 6c65 7329 290a 0a0a 636c 6173 7320 436f  les))...class Co
+0000d230: 6d70 6f73 6974 654b 6579 5265 666c 6563  mpositeKeyReflec
+0000d240: 7469 6f6e 5465 7374 285f 436f 6d70 6f73  tionTest(_Compos
+0000d250: 6974 654b 6579 5265 666c 6563 7469 6f6e  iteKeyReflection
+0000d260: 5465 7374 293a 0a20 2020 2040 7465 7374  Test):.    @test
+0000d270: 696e 672e 7265 7175 6972 6573 2e66 6f72  ing.requires.for
+0000d280: 6569 676e 5f6b 6579 5f63 6f6e 7374 7261  eign_key_constra
+0000d290: 696e 745f 7265 666c 6563 7469 6f6e 0a20  int_reflection. 
+0000d2a0: 2020 2064 6566 2074 6573 745f 666b 5f63     def test_fk_c
+0000d2b0: 6f6c 756d 6e5f 6f72 6465 7228 7365 6c66  olumn_order(self
+0000d2c0: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+0000d2d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d2e0: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+0000d2f0: 4944 453a 0a0a 2020 2020 2020 2020 5370  IDE:..        Sp
+0000d300: 616e 6e65 7220 636f 6c75 6d6e 2075 7361  anner column usa
+0000d310: 6765 2072 6566 6c65 6374 696f 6e20 646f  ge reflection do
+0000d320: 6573 6e27 7420 7375 7070 6f72 7420 6465  esn't support de
+0000d330: 7465 726d 656e 6973 7469 630a 2020 2020  termenistic.    
+0000d340: 2020 2020 6f72 6465 7269 6e67 2e20 4f76      ordering. Ov
+0000d350: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
+0000d360: 7420 746f 2063 6865 636b 2074 6861 7420  t to check that 
+0000d370: 636f 6c75 6d6e 7320 6172 650a 2020 2020  columns are.    
+0000d380: 2020 2020 7265 666c 6563 7465 6420 636f      reflected co
+0000d390: 7272 6563 746c 792c 2077 6974 686f 7574  rrectly, without
+0000d3a0: 2063 6f6e 7369 6465 7269 6e67 2074 6865   considering the
+0000d3b0: 6972 206f 7264 6572 2e0a 2020 2020 2020  ir order..      
+0000d3c0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+0000d3d0: 7465 7374 2066 6f72 2069 7373 7565 2023  test for issue #
+0000d3e0: 3536 3631 0a20 2020 2020 2020 2069 6e73  5661.        ins
+0000d3f0: 7020 3d20 696e 7370 6563 7428 636f 6e6e  p = inspect(conn
+0000d400: 6563 7469 6f6e 290a 2020 2020 2020 2020  ection).        
+0000d410: 666f 7265 6967 6e5f 6b65 7973 203d 2069  foreign_keys = i
+0000d420: 6e73 702e 6765 745f 666f 7265 6967 6e5f  nsp.get_foreign_
+0000d430: 6b65 7973 2873 656c 662e 7461 626c 6573  keys(self.tables
+0000d440: 2e74 6232 2e6e 616d 6529 0a20 2020 2020  .tb2.name).     
+0000d450: 2020 2065 715f 286c 656e 2866 6f72 6569     eq_(len(forei
+0000d460: 676e 5f6b 6579 7329 2c20 3129 0a20 2020  gn_keys), 1).   
+0000d470: 2020 2020 2066 6b65 7931 203d 2066 6f72       fkey1 = for
+0000d480: 6569 676e 5f6b 6579 735b 305d 0a20 2020  eign_keys[0].   
+0000d490: 2020 2020 2065 715f 2873 6574 2866 6b65       eq_(set(fke
+0000d4a0: 7931 2e67 6574 2822 7265 6665 7272 6564  y1.get("referred
+0000d4b0: 5f63 6f6c 756d 6e73 2229 292c 207b 226e  _columns")), {"n
+0000d4c0: 616d 6522 2c20 2269 6422 2c20 2261 7474  ame", "id", "att
+0000d4d0: 7222 7d29 0a20 2020 2020 2020 2065 715f  r"}).        eq_
+0000d4e0: 2873 6574 2866 6b65 7931 2e67 6574 2822  (set(fkey1.get("
+0000d4f0: 636f 6e73 7472 6169 6e65 645f 636f 6c75  constrained_colu
+0000d500: 6d6e 7322 2929 2c20 7b22 706e 616d 6522  mns")), {"pname"
+0000d510: 2c20 2270 6964 222c 2022 7061 7474 7222  , "pid", "pattr"
+0000d520: 7d29 0a0a 2020 2020 4074 6573 7469 6e67  })..    @testing
+0000d530: 2e72 6571 7569 7265 732e 7072 696d 6172  .requires.primar
+0000d540: 795f 6b65 795f 636f 6e73 7472 6169 6e74  y_key_constraint
+0000d550: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
+0000d560: 6465 6620 7465 7374 5f70 6b5f 636f 6c75  def test_pk_colu
+0000d570: 6d6e 5f6f 7264 6572 2873 656c 662c 2063  mn_order(self, c
+0000d580: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+0000d590: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d5a0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+0000d5b0: 3a0a 2020 2020 2020 2020 456d 756c 746f  :.        Emulto
+0000d5c0: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000d5d0: 7420 7265 7475 726e 696e 6720 706b 2073  t returning pk s
+0000d5e0: 6f72 7465 6420 6279 206f 7264 696e 616c  orted by ordinal
+0000d5f0: 2076 616c 7565 0a20 2020 2020 2020 206f   value.        o
+0000d600: 6620 636f 6c75 6d6e 732e 0a20 2020 2020  f columns..     
+0000d610: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000d620: 6e73 7020 3d20 696e 7370 6563 7428 636f  nsp = inspect(co
+0000d630: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
+0000d640: 2020 7072 696d 6172 795f 6b65 7920 3d20    primary_key = 
+0000d650: 696e 7370 2e67 6574 5f70 6b5f 636f 6e73  insp.get_pk_cons
+0000d660: 7472 6169 6e74 2873 656c 662e 7461 626c  traint(self.tabl
+0000d670: 6573 2e74 6231 2e6e 616d 6529 0a20 2020  es.tb1.name).   
+0000d680: 2020 2020 2065 7870 203d 2028 0a20 2020       exp = (.   
+0000d690: 2020 2020 2020 2020 205b 2269 6422 2c20           ["id", 
+0000d6a0: 226e 616d 6522 2c20 2261 7474 7222 5d0a  "name", "attr"].
+0000d6b0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
+0000d6c0: 6f6f 6c28 6f73 2e65 6e76 6972 6f6e 2e67  ool(os.environ.g
+0000d6d0: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
+0000d6e0: 4154 4f52 5f48 4f53 5422 2929 0a20 2020  ATOR_HOST")).   
+0000d6f0: 2020 2020 2020 2020 2065 6c73 6520 5b22           else ["
+0000d700: 6e61 6d65 222c 2022 6964 222c 2022 6174  name", "id", "at
+0000d710: 7472 225d 0a20 2020 2020 2020 2029 0a20  tr"].        ). 
+0000d720: 2020 2020 2020 2065 715f 2870 7269 6d61         eq_(prima
+0000d730: 7279 5f6b 6579 2e67 6574 2822 636f 6e73  ry_key.get("cons
+0000d740: 7472 6169 6e65 645f 636f 6c75 6d6e 7322  trained_columns"
+0000d750: 292c 2065 7870 290a 0a0a 4070 7974 6573  ), exp)...@pytes
+0000d760: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+0000d770: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+0000d780: 706f 7274 2071 756f 7465 7320 696e 2074  port quotes in t
+0000d790: 6162 6c65 206e 616d 6573 2e22 290a 636c  able names.").cl
+0000d7a0: 6173 7320 5175 6f74 6564 4e61 6d65 4172  ass QuotedNameAr
+0000d7b0: 6775 6d65 6e74 5465 7374 285f 5175 6f74  gumentTest(_Quot
+0000d7c0: 6564 4e61 6d65 4172 6775 6d65 6e74 5465  edNameArgumentTe
+0000d7d0: 7374 293a 0a20 2020 2070 6173 730a 0a0a  st):.    pass...
+0000d7e0: 636c 6173 7320 5f44 6174 6546 6978 7475  class _DateFixtu
+0000d7f0: 7265 285f 5f44 6174 6546 6978 7475 7265  re(__DateFixture
+0000d800: 293a 0a20 2020 2063 6f6d 7061 7265 203d  ):.    compare =
+0000d810: 204e 6f6e 650a 0a20 2020 2040 636c 6173   None..    @clas
+0000d820: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+0000d830: 6465 6669 6e65 5f74 6162 6c65 7328 636c  define_tables(cl
+0000d840: 732c 206d 6574 6164 6174 6129 3a0a 2020  s, metadata):.  
+0000d850: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d860: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+0000d870: 4445 3a0a 0a20 2020 2020 2020 2043 6c6f  DE:..        Clo
+0000d880: 7564 2053 7061 6e6e 6572 2064 6f65 736e  ud Spanner doesn
+0000d890: 2774 2073 7570 706f 7274 2061 7574 6f20  't support auto 
+0000d8a0: 696e 6372 656d 656e 7469 6e67 2069 6473  incrementing ids
+0000d8b0: 2066 6561 7475 7265 2c0a 2020 2020 2020   feature,.      
+0000d8c0: 2020 7768 6963 6820 6973 2075 7365 6420    which is used 
+0000d8d0: 6279 2074 6865 206f 7269 6769 6e61 6c20  by the original 
+0000d8e0: 7465 7374 2e20 4f76 6572 7269 6469 6e67  test. Overriding
+0000d8f0: 2074 6865 2074 6573 7420 6461 7461 0a20   the test data. 
+0000d900: 2020 2020 2020 2063 7265 6174 696f 6e20         creation 
+0000d910: 6d65 7468 6f64 2074 6f20 6469 7361 626c  method to disabl
+0000d920: 6520 6175 746f 696e 6372 656d 656e 7420  e autoincrement 
+0000d930: 616e 6420 6d61 6b65 2069 6420 636f 6c75  and make id colu
+0000d940: 6d6e 0a20 2020 2020 2020 206e 756c 6c61  mn.        nulla
+0000d950: 626c 652e 0a20 2020 2020 2020 2022 2222  ble..        """
+0000d960: 0a0a 2020 2020 2020 2020 636c 6173 7320  ..        class 
+0000d970: 4465 636f 7261 7465 6428 7371 6c61 6c63  Decorated(sqlalc
+0000d980: 6865 6d79 2e54 7970 6544 6563 6f72 6174  hemy.TypeDecorat
+0000d990: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0000d9a0: 2069 6d70 6c20 3d20 636c 732e 6461 7461   impl = cls.data
+0000d9b0: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
+0000d9c0: 2063 6163 6865 5f6f 6b20 3d20 5472 7565   cache_ok = True
+0000d9d0: 0a0a 2020 2020 2020 2020 5461 626c 6528  ..        Table(
+0000d9e0: 0a20 2020 2020 2020 2020 2020 2022 6461  .            "da
+0000d9f0: 7465 5f74 6162 6c65 222c 0a20 2020 2020  te_table",.     
+0000da00: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
+0000da10: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+0000da20: 756d 6e28 2269 6422 2c20 496e 7465 6765  umn("id", Intege
+0000da30: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+0000da40: 7275 652c 206e 756c 6c61 626c 653d 5472  rue, nullable=Tr
+0000da50: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
+0000da60: 2043 6f6c 756d 6e28 2264 6174 655f 6461   Column("date_da
+0000da70: 7461 222c 2063 6c73 2e64 6174 6174 7970  ta", cls.datatyp
+0000da80: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000da90: 436f 6c75 6d6e 2822 6465 636f 7261 7465  Column("decorate
+0000daa0: 645f 6461 7465 5f64 6174 6122 2c20 4465  d_date_data", De
+0000dab0: 636f 7261 7465 6429 2c0a 2020 2020 2020  corated),.      
+0000dac0: 2020 290a 0a0a 636c 6173 7320 4461 7465    )...class Date
+0000dad0: 5465 7374 285f 4461 7465 5465 7374 293a  Test(_DateTest):
+0000dae0: 0a20 2020 2022 2222 0a20 2020 2053 5041  .    """.    SPA
+0000daf0: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+0000db00: 2020 2020 4461 7465 5465 7374 2074 6573      DateTest tes
+0000db10: 7473 2075 7365 6420 7361 6d65 2063 6c61  ts used same cla
+0000db20: 7373 206d 6574 686f 6420 746f 2063 7265  ss method to cre
+0000db30: 6174 6520 7461 626c 652c 2073 6f20 746f  ate table, so to
+0000db40: 2061 766f 6964 2074 686f 7365 2066 6169   avoid those fai
+0000db50: 6c75 7265 730a 2020 2020 616e 6420 6d61  lures.    and ma
+0000db60: 696e 7461 696e 2044 5259 2063 6f6e 6365  intain DRY conce
+0000db70: 7074 206a 7573 7420 696e 6865 7269 7420  pt just inherit 
+0000db80: 7468 6520 636c 6173 7320 746f 2072 756e  the class to run
+0000db90: 2074 6573 7473 2073 7563 6365 7373 6675   tests successfu
+0000dba0: 6c6c 792e 0a20 2020 2022 2222 0a0a 2020  lly..    """..  
+0000dbb0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+0000dbc0: 6b69 7069 6628 0a20 2020 2020 2020 2062  kipif(.        b
+0000dbd0: 6f6f 6c28 6f73 2e65 6e76 6972 6f6e 2e67  ool(os.environ.g
+0000dbe0: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
+0000dbf0: 4154 4f52 5f48 4f53 5422 2929 2c20 7265  ATOR_HOST")), re
+0000dc00: 6173 6f6e 3d22 536b 6970 7065 6420 6f6e  ason="Skipped on
+0000dc10: 2065 6d75 6c61 746f 7222 0a20 2020 2029   emulator".    )
+0000dc20: 0a20 2020 2064 6566 2074 6573 745f 6e75  .    def test_nu
+0000dc30: 6c6c 5f62 6f75 6e64 5f63 6f6d 7061 7269  ll_bound_compari
+0000dc40: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
+0000dc50: 2020 2073 7570 6572 2829 2e74 6573 745f     super().test_
+0000dc60: 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d 7061  null_bound_compa
+0000dc70: 7269 736f 6e28 290a 0a20 2020 2040 7079  rison()..    @py
+0000dc80: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
+0000dc90: 280a 2020 2020 2020 2020 626f 6f6c 286f  (.        bool(o
+0000dca0: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
+0000dcb0: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
+0000dcc0: 484f 5354 2229 292c 2072 6561 736f 6e3d  HOST")), reason=
+0000dcd0: 2253 6b69 7070 6564 206f 6e20 656d 756c  "Skipped on emul
+0000dce0: 6174 6f72 220a 2020 2020 290a 2020 2020  ator".    ).    
+0000dcf0: 6465 6620 7465 7374 5f6e 756c 6c28 7365  def test_null(se
+0000dd00: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
+0000dd10: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0000dd20: 2e74 6573 745f 6e75 6c6c 2863 6f6e 6e65  .test_null(conne
+0000dd30: 6374 696f 6e29 0a0a 0a63 6c61 7373 2043  ction)...class C
+0000dd40: 5445 5465 7374 285f 4354 4554 6573 7429  TETest(_CTETest)
+0000dd50: 3a0a 2020 2020 4063 6c61 7373 6d65 7468  :.    @classmeth
+0000dd60: 6f64 0a20 2020 2064 6566 2064 6566 696e  od.    def defin
+0000dd70: 655f 7461 626c 6573 2863 6c73 2c20 6d65  e_tables(cls, me
+0000dd80: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
+0000dd90: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
+0000dda0: 206f 7269 6769 6e61 6c20 6d65 7468 6f64   original method
+0000ddb0: 2063 7265 6174 6573 2061 2066 6f72 6569   creates a forei
+0000ddc0: 676e 206b 6579 2077 6974 686f 7574 2061  gn key without a
+0000ddd0: 206e 616d 652c 0a20 2020 2020 2020 2077   name,.        w
+0000dde0: 6869 6368 2063 6175 7365 7320 7472 6f75  hich causes trou
+0000ddf0: 626c 6573 206f 6e20 7465 7374 2063 6c65  bles on test cle
+0000de00: 616e 7570 2e20 4f76 6572 7269 6469 6e67  anup. Overriding
+0000de10: 2074 6865 0a20 2020 2020 2020 206d 6574   the.        met
+0000de20: 686f 6420 746f 2065 7870 6c69 6369 746c  hod to explicitl
+0000de30: 7920 7365 7420 6120 666f 7265 6967 6e20  y set a foreign 
+0000de40: 6b65 7920 6e61 6d65 2e0a 2020 2020 2020  key name..      
+0000de50: 2020 2222 220a 2020 2020 2020 2020 5461    """.        Ta
+0000de60: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+0000de70: 2022 736f 6d65 5f74 6162 6c65 222c 0a20   "some_table",. 
+0000de80: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+0000de90: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+0000dea0: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
+0000deb0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+0000dec0: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
+0000ded0: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
+0000dee0: 7461 222c 2053 7472 696e 6728 3530 2929  ta", String(50))
+0000def0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+0000df00: 6c75 6d6e 2822 7061 7265 6e74 5f69 6422  lumn("parent_id"
+0000df10: 2c20 466f 7265 6967 6e4b 6579 2822 736f  , ForeignKey("so
+0000df20: 6d65 5f74 6162 6c65 2e69 6422 2c20 6e61  me_table.id", na
+0000df30: 6d65 3d22 666b 5f73 6f6d 655f 7461 626c  me="fk_some_tabl
+0000df40: 6522 2929 2c0a 2020 2020 2020 2020 290a  e")),.        ).
+0000df50: 0a20 2020 2020 2020 2054 6162 6c65 280a  .        Table(.
+0000df60: 2020 2020 2020 2020 2020 2020 2273 6f6d              "som
+0000df70: 655f 6f74 6865 725f 7461 626c 6522 2c0a  e_other_table",.
+0000df80: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+0000df90: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+0000dfa0: 2020 436f 6c75 6d6e 2822 6964 222c 2049    Column("id", I
+0000dfb0: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+0000dfc0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+0000dfd0: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
+0000dfe0: 6174 6122 2c20 5374 7269 6e67 2835 3029  ata", String(50)
+0000dff0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+0000e000: 6f6c 756d 6e28 2270 6172 656e 745f 6964  olumn("parent_id
+0000e010: 222c 2049 6e74 6567 6572 292c 0a20 2020  ", Integer),.   
+0000e020: 2020 2020 2029 0a0a 2020 2020 4070 7974       )..    @pyt
+0000e030: 6573 742e 6d61 726b 2e73 6b69 7028 2249  est.mark.skip("I
+0000e040: 4e53 4552 5420 6672 6f6d 2057 4954 4820  NSERT from WITH 
+0000e050: 7375 6271 7565 7279 2069 7320 6e6f 7420  subquery is not 
+0000e060: 7375 7070 6f72 7465 6422 290a 2020 2020  supported").    
+0000e070: 6465 6620 7465 7374 5f69 6e73 6572 745f  def test_insert_
+0000e080: 6672 6f6d 5f73 656c 6563 745f 726f 756e  from_select_roun
+0000e090: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
+0000e0a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e0b0: 2020 5468 6520 7465 7374 2063 6865 636b    The test check
+0000e0c0: 7320 6966 2061 6e20 494e 5345 5254 2063  s if an INSERT c
+0000e0d0: 616e 2062 6520 646f 6e65 2066 726f 6d20  an be done from 
+0000e0e0: 6120 6374 652c 206c 696b 653a 0a0a 2020  a cte, like:..  
+0000e0f0: 2020 2020 2020 5749 5448 2073 6f6d 655f        WITH some_
+0000e100: 6374 6520 4153 2028 2e2e 2e29 0a20 2020  cte AS (...).   
+0000e110: 2020 2020 2049 4e53 4552 5420 494e 544f       INSERT INTO
+0000e120: 2073 6f6d 655f 6f74 6865 725f 7461 626c   some_other_tabl
+0000e130: 6520 282e 2e2e 2053 454c 4543 5420 2a20  e (... SELECT * 
+0000e140: 4652 4f4d 2073 6f6d 655f 6374 6529 0a0a  FROM some_cte)..
+0000e150: 2020 2020 2020 2020 5375 6368 2071 7565          Such que
+0000e160: 7269 6573 2061 7265 206e 6f74 2073 7570  ries are not sup
+0000e170: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
+0000e180: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+0000e190: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000e1a0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+0000e1b0: 6970 2822 4445 4c45 5445 2066 726f 6d20  ip("DELETE from 
+0000e1c0: 5749 5448 2073 7562 7175 6572 7920 6973  WITH subquery is
+0000e1d0: 206e 6f74 2073 7570 706f 7274 6564 2229   not supported")
+0000e1e0: 0a20 2020 2064 6566 2074 6573 745f 6465  .    def test_de
+0000e1f0: 6c65 7465 5f73 6361 6c61 725f 7375 6271  lete_scalar_subq
+0000e200: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
+0000e210: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000e220: 2020 2020 2020 2054 6865 2074 6573 7420         The test 
+0000e230: 6368 6563 6b73 2069 6620 6120 4445 4c45  checks if a DELE
+0000e240: 5445 2063 616e 2062 6520 646f 6e65 2066  TE can be done f
+0000e250: 726f 6d20 6120 6374 652c 206c 696b 653a  rom a cte, like:
+0000e260: 0a0a 2020 2020 2020 2020 5749 5448 2073  ..        WITH s
+0000e270: 6f6d 655f 6374 6520 4153 2028 2e2e 2e29  ome_cte AS (...)
+0000e280: 0a20 2020 2020 2020 2044 454c 4554 4520  .        DELETE 
+0000e290: 4652 4f4d 2073 6f6d 655f 6f74 6865 725f  FROM some_other_
+0000e2a0: 7461 626c 6520 282e 2e2e 2053 454c 4543  table (... SELEC
+0000e2b0: 5420 2a20 4652 4f4d 2073 6f6d 655f 6374  T * FROM some_ct
+0000e2c0: 6529 0a0a 2020 2020 2020 2020 5375 6368  e)..        Such
+0000e2d0: 2071 7565 7269 6573 2061 7265 206e 6f74   queries are not
+0000e2e0: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
+0000e2f0: 616e 6e65 722e 0a20 2020 2020 2020 2022  anner..        "
+0000e300: 2222 0a20 2020 2020 2020 2070 6173 730a  "".        pass.
+0000e310: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0000e320: 6b2e 736b 6970 2822 4445 4c45 5445 2066  k.skip("DELETE f
+0000e330: 726f 6d20 5749 5448 2073 7562 7175 6572  rom WITH subquer
+0000e340: 7920 6973 206e 6f74 2073 7570 706f 7274  y is not support
+0000e350: 6564 2229 0a20 2020 2064 6566 2074 6573  ed").    def tes
+0000e360: 745f 6465 6c65 7465 5f66 726f 6d5f 726f  t_delete_from_ro
+0000e370: 756e 645f 7472 6970 2873 656c 6629 3a0a  und_trip(self):.
+0000e380: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000e390: 2020 2020 5468 6520 7465 7374 2063 6865      The test che
+0000e3a0: 636b 7320 6966 2061 2044 454c 4554 4520  cks if a DELETE 
+0000e3b0: 6361 6e20 6265 2064 6f6e 6520 6672 6f6d  can be done from
+0000e3c0: 2061 2063 7465 2c20 6c69 6b65 3a0a 0a20   a cte, like:.. 
+0000e3d0: 2020 2020 2020 2057 4954 4820 736f 6d65         WITH some
+0000e3e0: 5f63 7465 2041 5320 282e 2e2e 290a 2020  _cte AS (...).  
+0000e3f0: 2020 2020 2020 4445 4c45 5445 2046 524f        DELETE FRO
+0000e400: 4d20 736f 6d65 5f6f 7468 6572 5f74 6162  M some_other_tab
+0000e410: 6c65 2028 2e2e 2e20 5345 4c45 4354 202a  le (... SELECT *
+0000e420: 2046 524f 4d20 736f 6d65 5f63 7465 290a   FROM some_cte).
+0000e430: 0a20 2020 2020 2020 2053 7563 6820 7175  .        Such qu
+0000e440: 6572 6965 7320 6172 6520 6e6f 7420 7375  eries are not su
+0000e450: 7070 6f72 7465 6420 6279 2053 7061 6e6e  pported by Spann
+0000e460: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
+0000e470: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000e480: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+0000e490: 6b69 7028 2255 5044 4154 4520 6672 6f6d  kip("UPDATE from
+0000e4a0: 2057 4954 4820 7375 6271 7565 7279 2069   WITH subquery i
+0000e4b0: 7320 6e6f 7420 7375 7070 6f72 7465 6422  s not supported"
+0000e4c0: 290a 2020 2020 6465 6620 7465 7374 5f75  ).    def test_u
+0000e4d0: 7064 6174 655f 6672 6f6d 5f72 6f75 6e64  pdate_from_round
+0000e4e0: 5f74 7269 7028 7365 6c66 293a 0a20 2020  _trip(self):.   
+0000e4f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000e500: 2054 6865 2074 6573 7420 6368 6563 6b73   The test checks
+0000e510: 2069 6620 616e 2055 5044 4154 4520 6361   if an UPDATE ca
+0000e520: 6e20 6265 2064 6f6e 6520 6672 6f6d 2061  n be done from a
+0000e530: 2063 7465 2c20 6c69 6b65 3a0a 0a20 2020   cte, like:..   
+0000e540: 2020 2020 2057 4954 4820 736f 6d65 5f63       WITH some_c
+0000e550: 7465 2041 5320 282e 2e2e 290a 2020 2020  te AS (...).    
+0000e560: 2020 2020 5550 4441 5445 2073 6f6d 655f      UPDATE some_
+0000e570: 6f74 6865 725f 7461 626c 650a 2020 2020  other_table.    
+0000e580: 2020 2020 5345 5420 282e 2e2e 2053 454c      SET (... SEL
+0000e590: 4543 5420 2a20 4652 4f4d 2073 6f6d 655f  ECT * FROM some_
+0000e5a0: 6374 6529 0a0a 2020 2020 2020 2020 5375  cte)..        Su
+0000e5b0: 6368 2071 7565 7269 6573 2061 7265 206e  ch queries are n
+0000e5c0: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
+0000e5d0: 5370 616e 6e65 722e 0a20 2020 2020 2020  Spanner..       
+0000e5e0: 2022 2222 0a20 2020 2020 2020 2070 6173   """.        pas
+0000e5f0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+0000e600: 6172 6b2e 736b 6970 2822 5749 5448 2052  ark.skip("WITH R
+0000e610: 4543 5552 5349 5645 2073 7562 7175 6572  ECURSIVE subquer
+0000e620: 6965 7320 6172 6520 6e6f 7420 7375 7070  ies are not supp
+0000e630: 6f72 7465 6422 290a 2020 2020 6465 6620  orted").    def 
+0000e640: 7465 7374 5f73 656c 6563 745f 7265 6375  test_select_recu
+0000e650: 7273 6976 655f 726f 756e 645f 7472 6970  rsive_round_trip
+0000e660: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e670: 7061 7373 0a0a 0a63 6c61 7373 2044 6174  pass...class Dat
+0000e680: 6554 696d 654d 6963 726f 7365 636f 6e64  eTimeMicrosecond
+0000e690: 7354 6573 7428 5f44 6174 6554 696d 654d  sTest(_DateTimeM
+0000e6a0: 6963 726f 7365 636f 6e64 7354 6573 742c  icrosecondsTest,
+0000e6b0: 2044 6174 6554 6573 7429 3a0a 2020 2020   DateTest):.    
+0000e6c0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000e6d0: 7028 2253 7061 6e6e 6572 2064 6174 6573  p("Spanner dates
+0000e6e0: 2061 7265 2074 696d 6520 7a6f 6e65 2069   are time zone i
+0000e6f0: 6e64 6570 656e 6465 6e74 2229 0a20 2020  ndependent").   
+0000e700: 2064 6566 2074 6573 745f 7365 6c65 6374   def test_select
+0000e710: 5f64 6972 6563 7428 7365 6c66 293a 0a20  _direct(self):. 
+0000e720: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000e730: 2064 6566 2074 6573 745f 726f 756e 645f   def test_round_
+0000e740: 7472 6970 2873 656c 6629 3a0a 2020 2020  trip(self):.    
+0000e750: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000e760: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+0000e770: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
+0000e780: 6572 2063 6f6e 7665 7274 7320 7469 6d65  er converts time
+0000e790: 7374 616d 7020 696e 746f 2060 2559 2d25  stamp into `%Y-%
+0000e7a0: 6d2d 2564 5425 483a 254d 3a25 532e 2566  m-%dT%H:%M:%S.%f
+0000e7b0: 5a60 2066 6f72 6d61 742c 2073 6f20 746f  Z` format, so to
+0000e7c0: 2061 766f 6964 0a20 2020 2020 2020 2061   avoid.        a
+0000e7d0: 7373 6572 7420 6661 696c 7572 6573 2063  ssert failures c
+0000e7e0: 6f6e 7665 7274 2064 6174 6574 696d 6520  onvert datetime 
+0000e7f0: 696e 7075 7420 746f 2074 6865 2064 6573  input to the des
+0000e800: 6972 6520 7469 6d65 7374 616d 7020 666f  ire timestamp fo
+0000e810: 726d 6174 2e0a 2020 2020 2020 2020 2222  rmat..        ""
+0000e820: 220a 2020 2020 2020 2020 6461 7465 5f74  ".        date_t
+0000e830: 6162 6c65 203d 2073 656c 662e 7461 626c  able = self.tabl
+0000e840: 6573 2e64 6174 655f 7461 626c 650a 0a20  es.date_table.. 
+0000e850: 2020 2020 2020 2077 6974 6820 636f 6e66         with conf
+0000e860: 6967 2e64 622e 636f 6e6e 6563 7428 2920  ig.db.connect() 
+0000e870: 6173 2063 6f6e 6e65 6374 696f 6e3a 0a20  as connection:. 
+0000e880: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+0000e890: 6374 696f 6e2e 6578 6563 7574 6528 6461  ction.execute(da
+0000e8a0: 7465 5f74 6162 6c65 2e69 6e73 6572 7428  te_table.insert(
+0000e8b0: 292c 207b 2264 6174 655f 6461 7461 223a  ), {"date_data":
+0000e8c0: 2073 656c 662e 6461 7461 2c20 2269 6422   self.data, "id"
+0000e8d0: 3a20 3235 307d 290a 2020 2020 2020 2020  : 250}).        
+0000e8e0: 2020 2020 726f 7720 3d20 636f 6e6e 6563      row = connec
+0000e8f0: 7469 6f6e 2e65 7865 6375 7465 2873 656c  tion.execute(sel
+0000e900: 6563 7428 6461 7465 5f74 6162 6c65 2e63  ect(date_table.c
+0000e910: 2e64 6174 655f 6461 7461 2929 2e66 6972  .date_data)).fir
+0000e920: 7374 2829 0a0a 2020 2020 2020 2020 636f  st()..        co
+0000e930: 6d70 6172 6520 3d20 7365 6c66 2e63 6f6d  mpare = self.com
+0000e940: 7061 7265 206f 7220 7365 6c66 2e64 6174  pare or self.dat
+0000e950: 610a 2020 2020 2020 2020 636f 6d70 6172  a.        compar
+0000e960: 6520 3d20 636f 6d70 6172 652e 7374 7266  e = compare.strf
+0000e970: 7469 6d65 2822 2559 2d25 6d2d 2564 5425  time("%Y-%m-%dT%
+0000e980: 483a 254d 3a25 532e 2566 5a22 290a 2020  H:%M:%S.%fZ").  
+0000e990: 2020 2020 2020 6571 5f28 726f 775b 305d        eq_(row[0]
+0000e9a0: 2e72 6663 3333 3339 2829 2c20 636f 6d70  .rfc3339(), comp
+0000e9b0: 6172 6529 0a20 2020 2020 2020 2061 7373  are).        ass
+0000e9c0: 6572 7420 6973 696e 7374 616e 6365 2872  ert isinstance(r
+0000e9d0: 6f77 5b30 5d2c 2044 6174 6574 696d 6557  ow[0], DatetimeW
+0000e9e0: 6974 684e 616e 6f73 6563 6f6e 6473 290a  ithNanoseconds).
+0000e9f0: 0a20 2020 2064 6566 2074 6573 745f 726f  .    def test_ro
+0000ea00: 756e 645f 7472 6970 5f64 6563 6f72 6174  und_trip_decorat
+0000ea10: 6564 2873 656c 662c 2063 6f6e 6e65 6374  ed(self, connect
+0000ea20: 696f 6e29 3a0a 2020 2020 2020 2020 2222  ion):.        ""
+0000ea30: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
+0000ea40: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
+0000ea50: 2020 2020 2053 7061 6e6e 6572 2063 6f6e       Spanner con
+0000ea60: 7665 7274 7320 7469 6d65 7374 616d 7020  verts timestamp 
+0000ea70: 696e 746f 2060 2559 2d25 6d2d 2564 5425  into `%Y-%m-%dT%
+0000ea80: 483a 254d 3a25 532e 2566 5a60 2066 6f72  H:%M:%S.%fZ` for
+0000ea90: 6d61 742c 2073 6f20 746f 2061 766f 6964  mat, so to avoid
+0000eaa0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000eab0: 6661 696c 7572 6573 2063 6f6e 7665 7274  failures convert
+0000eac0: 2064 6174 6574 696d 6520 696e 7075 7420   datetime input 
+0000ead0: 746f 2074 6865 2064 6573 6972 6520 7469  to the desire ti
+0000eae0: 6d65 7374 616d 7020 666f 726d 6174 2e0a  mestamp format..
+0000eaf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000eb00: 2020 2020 6461 7465 5f74 6162 6c65 203d      date_table =
+0000eb10: 2073 656c 662e 7461 626c 6573 2e64 6174   self.tables.dat
+0000eb20: 655f 7461 626c 650a 0a20 2020 2020 2020  e_table..       
+0000eb30: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
+0000eb40: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
+0000eb50: 2064 6174 655f 7461 626c 652e 696e 7365   date_table.inse
+0000eb60: 7274 2829 2c20 7b22 6964 223a 2031 2c20  rt(), {"id": 1, 
+0000eb70: 2264 6563 6f72 6174 6564 5f64 6174 655f  "decorated_date_
+0000eb80: 6461 7461 223a 2073 656c 662e 6461 7461  data": self.data
+0000eb90: 7d0a 2020 2020 2020 2020 290a 0a20 2020  }.        )..   
+0000eba0: 2020 2020 2072 6f77 203d 2063 6f6e 6e65       row = conne
+0000ebb0: 6374 696f 6e2e 6578 6563 7574 6528 7365  ction.execute(se
+0000ebc0: 6c65 6374 2864 6174 655f 7461 626c 652e  lect(date_table.
+0000ebd0: 632e 6465 636f 7261 7465 645f 6461 7465  c.decorated_date
+0000ebe0: 5f64 6174 6129 292e 6669 7273 7428 290a  _data)).first().
+0000ebf0: 0a20 2020 2020 2020 2063 6f6d 7061 7265  .        compare
+0000ec00: 203d 2073 656c 662e 636f 6d70 6172 6520   = self.compare 
+0000ec10: 6f72 2073 656c 662e 6461 7461 0a20 2020  or self.data.   
+0000ec20: 2020 2020 2063 6f6d 7061 7265 203d 2063       compare = c
+0000ec30: 6f6d 7061 7265 2e73 7472 6674 696d 6528  ompare.strftime(
+0000ec40: 2225 592d 256d 2d25 6454 2548 3a25 4d3a  "%Y-%m-%dT%H:%M:
+0000ec50: 2553 2e25 665a 2229 0a20 2020 2020 2020  %S.%fZ").       
+0000ec60: 2065 715f 2872 6f77 5b30 5d2e 7266 6333   eq_(row[0].rfc3
+0000ec70: 3333 3928 292c 2063 6f6d 7061 7265 290a  339(), compare).
+0000ec80: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+0000ec90: 7369 6e73 7461 6e63 6528 726f 775b 305d  sinstance(row[0]
+0000eca0: 2c20 4461 7465 7469 6d65 5769 7468 4e61  , DatetimeWithNa
+0000ecb0: 6e6f 7365 636f 6e64 7329 0a0a 2020 2020  noseconds)..    
+0000ecc0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000ecd0: 7069 6628 0a20 2020 2020 2020 2062 6f6f  pif(.        boo
+0000ece0: 6c28 6f73 2e65 6e76 6972 6f6e 2e67 6574  l(os.environ.get
+0000ecf0: 2822 5350 414e 4e45 525f 454d 554c 4154  ("SPANNER_EMULAT
+0000ed00: 4f52 5f48 4f53 5422 2929 2c20 7265 6173  OR_HOST")), reas
+0000ed10: 6f6e 3d22 536b 6970 7065 6420 6f6e 2065  on="Skipped on e
+0000ed20: 6d75 6c61 746f 7222 0a20 2020 2029 0a20  mulator".    ). 
+0000ed30: 2020 2064 6566 2074 6573 745f 6e75 6c6c     def test_null
+0000ed40: 5f62 6f75 6e64 5f63 6f6d 7061 7269 736f  _bound_compariso
+0000ed50: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+0000ed60: 2073 7570 6572 2829 2e74 6573 745f 6e75   super().test_nu
+0000ed70: 6c6c 5f62 6f75 6e64 5f63 6f6d 7061 7269  ll_bound_compari
+0000ed80: 736f 6e28 290a 0a20 2020 2040 7079 7465  son()..    @pyte
+0000ed90: 7374 2e6d 6172 6b2e 736b 6970 6966 280a  st.mark.skipif(.
+0000eda0: 2020 2020 2020 2020 626f 6f6c 286f 732e          bool(os.
+0000edb0: 656e 7669 726f 6e2e 6765 7428 2253 5041  environ.get("SPA
+0000edc0: 4e4e 4552 5f45 4d55 4c41 544f 525f 484f  NNER_EMULATOR_HO
+0000edd0: 5354 2229 292c 2072 6561 736f 6e3d 2253  ST")), reason="S
+0000ede0: 6b69 7070 6564 206f 6e20 656d 756c 6174  kipped on emulat
+0000edf0: 6f72 220a 2020 2020 290a 2020 2020 6465  or".    ).    de
+0000ee00: 6620 7465 7374 5f6e 756c 6c28 7365 6c66  f test_null(self
+0000ee10: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+0000ee20: 2020 2020 2020 2073 7570 6572 2829 2e74         super().t
+0000ee30: 6573 745f 6e75 6c6c 2863 6f6e 6e65 6374  est_null(connect
+0000ee40: 696f 6e29 0a0a 0a63 6c61 7373 2044 6174  ion)...class Dat
+0000ee50: 6554 696d 6554 6573 7428 5f44 6174 6554  eTimeTest(_DateT
+0000ee60: 696d 6554 6573 742c 2044 6174 6554 696d  imeTest, DateTim
+0000ee70: 654d 6963 726f 7365 636f 6e64 7354 6573  eMicrosecondsTes
+0000ee80: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
+0000ee90: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+0000eea0: 3a0a 0a20 2020 2044 6174 6554 696d 6554  :..    DateTimeT
+0000eeb0: 6573 7420 7465 7374 7320 6861 7665 2074  est tests have t
+0000eec0: 6865 2073 616d 6520 6661 696c 7572 6573  he same failures
+0000eed0: 2073 616d 6520 6173 2044 6174 6554 696d   same as DateTim
+0000eee0: 654d 6963 726f 7365 636f 6e64 7354 6573  eMicrosecondsTes
+0000eef0: 7420 7465 7374 732c 0a20 2020 2073 6f20  t tests,.    so 
+0000ef00: 746f 2061 766f 6964 2074 686f 7365 2066  to avoid those f
+0000ef10: 6169 6c75 7265 7320 616e 6420 6d61 696e  ailures and main
+0000ef20: 7461 696e 2044 5259 2063 6f6e 6365 7074  tain DRY concept
+0000ef30: 206a 7573 7420 696e 6865 7269 7420 7468   just inherit th
+0000ef40: 6520 636c 6173 7320 746f 2072 756e 0a20  e class to run. 
+0000ef50: 2020 2074 6573 7473 2073 7563 6365 7373     tests success
+0000ef60: 6675 6c6c 792e 0a20 2020 2022 2222 0a0a  fully..    """..
+0000ef70: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000ef80: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
+0000ef90: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
+0000efa0: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
+0000efb0: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
+0000efc0: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
+0000efd0: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
+0000efe0: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
+0000eff0: 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d 7061  null_bound_compa
+0000f000: 7269 736f 6e28 7365 6c66 293a 0a20 2020  rison(self):.   
+0000f010: 2020 2020 2073 7570 6572 2829 2e74 6573       super().tes
+0000f020: 745f 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d  t_null_bound_com
+0000f030: 7061 7269 736f 6e28 290a 0a20 2020 2040  parison()..    @
+0000f040: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+0000f050: 6966 280a 2020 2020 2020 2020 626f 6f6c  if(.        bool
+0000f060: 286f 732e 656e 7669 726f 6e2e 6765 7428  (os.environ.get(
+0000f070: 2253 5041 4e4e 4552 5f45 4d55 4c41 544f  "SPANNER_EMULATO
+0000f080: 525f 484f 5354 2229 292c 2072 6561 736f  R_HOST")), reaso
+0000f090: 6e3d 2253 6b69 7070 6564 206f 6e20 656d  n="Skipped on em
+0000f0a0: 756c 6174 6f72 220a 2020 2020 290a 2020  ulator".    ).  
+0000f0b0: 2020 6465 6620 7465 7374 5f6e 756c 6c28    def test_null(
+0000f0c0: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
+0000f0d0: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+0000f0e0: 2829 2e74 6573 745f 6e75 6c6c 2863 6f6e  ().test_null(con
+0000f0f0: 6e65 6374 696f 6e29 0a0a 2020 2020 4070  nection)..    @p
+0000f100: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000f110: 2253 7061 6e6e 6572 2064 6174 6573 2061  "Spanner dates a
+0000f120: 7265 2074 696d 6520 7a6f 6e65 2069 6e64  re time zone ind
+0000f130: 6570 656e 6465 6e74 2229 0a20 2020 2064  ependent").    d
+0000f140: 6566 2074 6573 745f 7365 6c65 6374 5f64  ef test_select_d
+0000f150: 6972 6563 7428 7365 6c66 293a 0a20 2020  irect(self):.   
+0000f160: 2020 2020 2070 6173 730a 0a0a 4070 7974       pass...@pyt
+0000f170: 6573 742e 6d61 726b 2e73 6b69 7028 224e  est.mark.skip("N
+0000f180: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
+0000f190: 5370 616e 6e65 7222 290a 636c 6173 7320  Spanner").class 
+0000f1a0: 4469 6666 6963 756c 7450 6172 616d 6574  DifficultParamet
+0000f1b0: 6572 7354 6573 7428 5f44 6966 6669 6375  ersTest(_Difficu
+0000f1c0: 6c74 5061 7261 6d65 7465 7273 5465 7374  ltParametersTest
+0000f1d0: 293a 0a20 2020 2070 6173 730a 0a0a 636c  ):.    pass...cl
+0000f1e0: 6173 7320 4665 7463 684c 696d 6974 4f66  ass FetchLimitOf
+0000f1f0: 6673 6574 5465 7374 285f 4665 7463 684c  fsetTest(_FetchL
+0000f200: 696d 6974 4f66 6673 6574 5465 7374 293a  imitOffsetTest):
+0000f210: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0000f220: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
+0000f230: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+0000f240: 636f 6d70 6f73 6974 6520 4c49 4d49 5420  composite LIMIT 
+0000f250: 616e 6420 4f46 4653 4554 2063 6c61 7573  and OFFSET claus
+0000f260: 6573 2229 0a20 2020 2064 6566 2074 6573  es").    def tes
+0000f270: 745f 6578 7072 5f6c 696d 6974 2873 656c  t_expr_limit(sel
+0000f280: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
+0000f290: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000f2a0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+0000f2b0: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
+0000f2c0: 736e 2774 2073 7570 706f 7274 2063 6f6d  sn't support com
+0000f2d0: 706f 7369 7465 204c 494d 4954 2061 6e64  posite LIMIT and
+0000f2e0: 204f 4646 5345 5420 636c 6175 7365 7322   OFFSET clauses"
+0000f2f0: 290a 2020 2020 6465 6620 7465 7374 5f65  ).    def test_e
+0000f300: 7870 725f 6f66 6673 6574 2873 656c 662c  xpr_offset(self,
+0000f310: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
+0000f320: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0000f330: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000f340: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+0000f350: 2774 2073 7570 706f 7274 2063 6f6d 706f  't support compo
+0000f360: 7369 7465 204c 494d 4954 2061 6e64 204f  site LIMIT and O
+0000f370: 4646 5345 5420 636c 6175 7365 7322 290a  FFSET clauses").
+0000f380: 2020 2020 6465 6620 7465 7374 5f65 7870      def test_exp
+0000f390: 725f 6c69 6d69 745f 6f66 6673 6574 2873  r_limit_offset(s
+0000f3a0: 656c 662c 2063 6f6e 6e65 6374 696f 6e29  elf, connection)
+0000f3b0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000f3c0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000f3d0: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+0000f3e0: 6f65 736e 2774 2073 7570 706f 7274 2063  oesn't support c
+0000f3f0: 6f6d 706f 7369 7465 204c 494d 4954 2061  omposite LIMIT a
+0000f400: 6e64 204f 4646 5345 5420 636c 6175 7365  nd OFFSET clause
+0000f410: 7322 290a 2020 2020 6465 6620 7465 7374  s").    def test
+0000f420: 5f65 7870 725f 6c69 6d69 745f 7369 6d70  _expr_limit_simp
+0000f430: 6c65 5f6f 6666 7365 7428 7365 6c66 2c20  le_offset(self, 
+0000f440: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
+0000f450: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+0000f460: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+0000f470: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
+0000f480: 7420 7375 7070 6f72 7420 636f 6d70 6f73  t support compos
+0000f490: 6974 6520 4c49 4d49 5420 616e 6420 4f46  ite LIMIT and OF
+0000f4a0: 4653 4554 2063 6c61 7573 6573 2229 0a20  FSET clauses"). 
+0000f4b0: 2020 2064 6566 2074 6573 745f 7369 6d70     def test_simp
+0000f4c0: 6c65 5f6c 696d 6974 5f65 7870 725f 6f66  le_limit_expr_of
+0000f4d0: 6673 6574 2873 656c 662c 2063 6f6e 6e65  fset(self, conne
+0000f4e0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+0000f4f0: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+0000f500: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+0000f510: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+0000f520: 706f 7274 2063 6f6d 706f 7369 7465 204c  port composite L
+0000f530: 494d 4954 2061 6e64 204f 4646 5345 5420  IMIT and OFFSET 
+0000f540: 636c 6175 7365 7322 290a 2020 2020 6465  clauses").    de
+0000f550: 6620 7465 7374 5f62 6f75 6e64 5f6f 6666  f test_bound_off
+0000f560: 7365 7428 7365 6c66 2c20 636f 6e6e 6563  set(self, connec
+0000f570: 7469 6f6e 293a 0a20 2020 2020 2020 2070  tion):.        p
+0000f580: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+0000f590: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
+0000f5a0: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
+0000f5b0: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
+0000f5c0: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
+0000f5d0: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
+0000f5e0: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
+0000f5f0: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
+0000f600: 7465 7374 5f6c 696d 6974 5f72 656e 6465  test_limit_rende
+0000f610: 725f 6d75 6c74 6970 6c65 5f74 696d 6573  r_multiple_times
+0000f620: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+0000f630: 6e29 3a0a 2020 2020 2020 2020 7461 626c  n):.        tabl
+0000f640: 6520 3d20 7365 6c66 2e74 6162 6c65 732e  e = self.tables.
+0000f650: 736f 6d65 5f74 6162 6c65 0a20 2020 2020  some_table.     
+0000f660: 2020 2073 746d 7420 3d20 7365 6c65 6374     stmt = select
+0000f670: 2874 6162 6c65 2e63 2e69 6429 2e6c 696d  (table.c.id).lim
+0000f680: 6974 2831 292e 7363 616c 6172 5f73 7562  it(1).scalar_sub
+0000f690: 7175 6572 7928 290a 0a20 2020 2020 2020  query()..       
+0000f6a0: 2075 203d 2075 6e69 6f6e 2873 656c 6563   u = union(selec
+0000f6b0: 7428 7374 6d74 292c 2073 656c 6563 7428  t(stmt), select(
+0000f6c0: 7374 6d74 2929 2e73 7562 7175 6572 7928  stmt)).subquery(
+0000f6d0: 292e 7365 6c65 6374 2829 0a0a 2020 2020  ).select()..    
+0000f6e0: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
+0000f6f0: 5f72 6573 756c 7428 0a20 2020 2020 2020  _result(.       
+0000f700: 2020 2020 2063 6f6e 6e65 6374 696f 6e2c       connection,
+0000f710: 0a20 2020 2020 2020 2020 2020 2075 2c0a  .            u,.
+0000f720: 2020 2020 2020 2020 2020 2020 5b28 312c              [(1,
+0000f730: 295d 2c0a 2020 2020 2020 2020 290a 0a20  )],.        ).. 
+0000f740: 2020 2040 7465 7374 696e 672e 7265 7175     @testing.requ
+0000f750: 6972 6573 2e6f 6666 7365 740a 2020 2020  ires.offset.    
+0000f760: 6465 6620 7465 7374 5f73 696d 706c 655f  def test_simple_
+0000f770: 6f66 6673 6574 2873 656c 662c 2063 6f6e  offset(self, con
+0000f780: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+0000f790: 2020 7461 626c 6520 3d20 7365 6c66 2e74    table = self.t
+0000f7a0: 6162 6c65 732e 736f 6d65 5f74 6162 6c65  ables.some_table
+0000f7b0: 0a20 2020 2020 2020 2073 656c 662e 5f61  .        self._a
+0000f7c0: 7373 6572 745f 7265 7375 6c74 280a 2020  ssert_result(.  
+0000f7d0: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
+0000f7e0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0000f7f0: 2020 7365 6c65 6374 2874 6162 6c65 292e    select(table).
+0000f800: 6f72 6465 725f 6279 2874 6162 6c65 2e63  order_by(table.c
+0000f810: 2e69 6429 2e6f 6666 7365 7428 3229 2c0a  .id).offset(2),.
+0000f820: 2020 2020 2020 2020 2020 2020 5b28 332c              [(3,
+0000f830: 2033 2c20 3429 2c20 2834 2c20 342c 2035   3, 4), (4, 4, 5
+0000f840: 292c 2028 352c 2034 2c20 3629 5d2c 0a20  ), (5, 4, 6)],. 
+0000f850: 2020 2020 2020 2029 0a0a 0a40 7079 7465         )...@pyte
+0000f860: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+0000f870: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+0000f880: 7070 6f72 7420 6175 746f 696e 6372 656d  pport autoincrem
+0000f890: 656e 7422 290a 636c 6173 7320 4964 656e  ent").class Iden
+0000f8a0: 7469 7479 4175 746f 696e 6372 656d 656e  tityAutoincremen
+0000f8b0: 7454 6573 7428 5f49 6465 6e74 6974 7941  tTest(_IdentityA
+0000f8c0: 7574 6f69 6e63 7265 6d65 6e74 5465 7374  utoincrementTest
+0000f8d0: 293a 0a20 2020 2070 6173 730a 0a0a 4070  ):.    pass...@p
+0000f8e0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000f8f0: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
+0000f900: 2073 7570 706f 7274 2072 6574 7572 6e69   support returni
+0000f910: 6e67 2229 0a63 6c61 7373 2052 6574 7572  ng").class Retur
+0000f920: 6e69 6e67 4775 6172 6473 5465 7374 285f  ningGuardsTest(_
+0000f930: 5265 7475 726e 696e 6747 7561 7264 7354  ReturningGuardsT
+0000f940: 6573 7429 3a0a 2020 2020 7061 7373 0a0a  est):.    pass..
+0000f950: 0a40 7079 7465 7374 2e6d 6172 6b2e 736b  .@pytest.mark.sk
+0000f960: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
+0000f970: 6e27 7420 7375 7070 6f72 7420 7573 6572  n't support user
+0000f980: 206d 6164 6520 7363 6865 6d61 7322 290a   made schemas").
+0000f990: 636c 6173 7320 5361 6d65 4e61 6d65 6453  class SameNamedS
+0000f9a0: 6368 656d 6154 6162 6c65 5465 7374 285f  chemaTableTest(_
+0000f9b0: 5361 6d65 4e61 6d65 6453 6368 656d 6154  SameNamedSchemaT
+0000f9c0: 6162 6c65 5465 7374 293a 0a20 2020 2070  ableTest):.    p
+0000f9d0: 6173 730a 0a0a 636c 6173 7320 4573 6361  ass...class Esca
+0000f9e0: 7069 6e67 5465 7374 285f 4573 6361 7069  pingTest(_Escapi
+0000f9f0: 6e67 5465 7374 293a 0a20 2020 2040 7072  ngTest):.    @pr
+0000fa00: 6f76 6964 655f 6d65 7461 6461 7461 0a20  ovide_metadata. 
+0000fa10: 2020 2064 6566 2074 6573 745f 7065 7263     def test_perc
+0000fa20: 656e 745f 7369 676e 5f72 6f75 6e64 5f74  ent_sign_round_t
+0000fa30: 7269 7028 7365 6c66 293a 0a20 2020 2020  rip(self):.     
+0000fa40: 2020 2022 2222 5465 7374 2074 6861 7420     """Test that 
+0000fa50: 7468 6520 4442 4150 4920 6163 636f 6d6d  the DBAPI accomm
+0000fa60: 6f64 6174 6573 2066 6f72 2065 7363 6170  odates for escap
+0000fa70: 6564 202f 206e 6f6e 6573 6361 7065 640a  ed / nonescaped.
+0000fa80: 2020 2020 2020 2020 7065 7263 656e 7420          percent 
+0000fa90: 7369 676e 7320 696e 2061 2077 6179 2074  signs in a way t
+0000faa0: 6861 7420 6d61 7463 6865 7320 7468 6520  hat matches the 
+0000fab0: 636f 6d70 696c 6572 0a0a 2020 2020 2020  compiler..      
+0000fac0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+0000fad0: 4445 0a20 2020 2020 2020 2043 6c6f 7564  DE.        Cloud
+0000fae0: 2053 7061 6e6e 6572 2073 7570 706f 7274   Spanner support
+0000faf0: 7320 7461 626c 6573 2077 6974 6820 656d  s tables with em
+0000fb00: 7074 7920 7072 696d 6172 7920 6b65 792c  pty primary key,
+0000fb10: 2062 7574 0a20 2020 2020 2020 206f 6e6c   but.        onl
+0000fb20: 7920 7369 6e67 6c65 206f 6e65 2072 6f77  y single one row
+0000fb30: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
+0000fb40: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
+0000fb50: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
+0000fb60: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
+0000fb70: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
+0000fb80: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
+0000fb90: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
+0000fba0: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
+0000fbb0: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
+0000fbc0: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
+0000fbd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fbe0: 2020 2020 206d 203d 2073 656c 662e 6d65       m = self.me
+0000fbf0: 7461 6461 7461 0a20 2020 2020 2020 2074  tadata.        t
+0000fc00: 203d 2054 6162 6c65 2822 7422 2c20 6d2c   = Table("t", m,
+0000fc10: 2043 6f6c 756d 6e28 2264 6174 6122 2c20   Column("data", 
+0000fc20: 5374 7269 6e67 2835 3029 2929 0a20 2020  String(50))).   
+0000fc30: 2020 2020 2074 2e63 7265 6174 6528 636f       t.create(co
+0000fc40: 6e66 6967 2e64 6229 0a20 2020 2020 2020  nfig.db).       
+0000fc50: 2077 6974 6820 636f 6e66 6967 2e64 622e   with config.db.
+0000fc60: 6265 6769 6e28 2920 6173 2063 6f6e 6e3a  begin() as conn:
+0000fc70: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000fc80: 6e2e 6578 6563 7574 6528 742e 696e 7365  n.execute(t.inse
+0000fc90: 7274 2829 2c20 6469 6374 2864 6174 613d  rt(), dict(data=
+0000fca0: 2273 6f6d 6520 2520 7661 6c75 6522 2929  "some % value"))
+0000fcb0: 0a0a 2020 2020 2020 2020 2020 2020 6571  ..            eq
+0000fcc0: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
+0000fcd0: 2020 2063 6f6e 6e2e 7363 616c 6172 280a     conn.scalar(.
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 2020 2020 7365 6c65 6374 2874 2e63 2e64      select(t.c.d
+0000fd00: 6174 6129 2e77 6865 7265 2874 2e63 2e64  ata).where(t.c.d
+0000fd10: 6174 6120 3d3d 206c 6974 6572 616c 5f63  ata == literal_c
+0000fd20: 6f6c 756d 6e28 2227 736f 6d65 2025 2076  olumn("'some % v
+0000fd30: 616c 7565 2722 2929 0a20 2020 2020 2020  alue'")).       
+0000fd40: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+0000fd50: 2020 2020 2020 2020 2020 2020 2273 6f6d              "som
+0000fd60: 6520 2520 7661 6c75 6522 2c0a 2020 2020  e % value",.    
+0000fd70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000fd80: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
+0000fd90: 7574 6528 742e 6465 6c65 7465 2829 290a  ute(t.delete()).
+0000fda0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+0000fdb0: 2e65 7865 6375 7465 2874 2e69 6e73 6572  .execute(t.inser
+0000fdc0: 7428 292c 2064 6963 7428 6461 7461 3d22  t(), dict(data="
+0000fdd0: 736f 6d65 2025 2520 6f74 6865 7220 7661  some %% other va
+0000fde0: 6c75 6522 2929 0a20 2020 2020 2020 2020  lue")).         
+0000fdf0: 2020 2065 715f 280a 2020 2020 2020 2020     eq_(.        
+0000fe00: 2020 2020 2020 2020 636f 6e6e 2e73 6361          conn.sca
+0000fe10: 6c61 7228 0a20 2020 2020 2020 2020 2020  lar(.           
+0000fe20: 2020 2020 2020 2020 2073 656c 6563 7428           select(
+0000fe30: 742e 632e 6461 7461 292e 7768 6572 6528  t.c.data).where(
+0000fe40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fe50: 2020 2020 2020 2020 2074 2e63 2e64 6174           t.c.dat
+0000fe60: 6120 3d3d 206c 6974 6572 616c 5f63 6f6c  a == literal_col
+0000fe70: 756d 6e28 2227 736f 6d65 2025 2520 6f74  umn("'some %% ot
+0000fe80: 6865 7220 7661 6c75 6527 2229 0a20 2020  her value'").   
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000feb0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+0000fec0: 2020 2020 2020 2273 6f6d 6520 2525 206f        "some %% o
+0000fed0: 7468 6572 2076 616c 7565 222c 0a20 2020  ther value",.   
+0000fee0: 2020 2020 2020 2020 2029 0a0a 0a63 6c61           )...cla
+0000fef0: 7373 2045 7869 7374 7354 6573 7428 5f45  ss ExistsTest(_E
+0000ff00: 7869 7374 7354 6573 7429 3a0a 2020 2020  xistsTest):.    
+0000ff10: 6465 6620 7465 7374 5f73 656c 6563 745f  def test_select_
+0000ff20: 6578 6973 7473 2873 656c 662c 2063 6f6e  exists(self, con
+0000ff30: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+0000ff40: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+0000ff50: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+0000ff60: 0a20 2020 2020 2020 2054 6865 206f 7269  .        The ori
+0000ff70: 6769 6e61 6c20 7465 7374 2069 7320 7472  ginal test is tr
+0000ff80: 7969 6e67 2074 6f20 6578 6563 7574 6520  ying to execute 
+0000ff90: 6120 7175 6572 7920 6c69 6b65 3a0a 0a20  a query like:.. 
+0000ffa0: 2020 2020 2020 2053 454c 4543 5420 2e2e         SELECT ..
+0000ffb0: 2e0a 2020 2020 2020 2020 5748 4552 4520  ..        WHERE 
+0000ffc0: 4558 4953 5453 2028 5345 4c45 4354 202e  EXISTS (SELECT .
+0000ffd0: 2e2e 290a 0a20 2020 2020 2020 2053 454c  ..)..        SEL
+0000ffe0: 4543 5420 5748 4552 4520 7769 7468 6f75  ECT WHERE withou
+0000fff0: 7420 4652 4f4d 2063 6c61 7573 6520 6973  t FROM clause is
+00010000: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
+00010010: 7920 5370 616e 6e65 722e 0a20 2020 2020  y Spanner..     
+00010020: 2020 2052 6577 7269 7469 6e67 2074 6865     Rewriting the
+00010030: 2074 6573 7420 746f 2066 6f72 6365 2069   test to force i
+00010040: 7420 746f 2067 656e 6572 6174 6520 6120  t to generate a 
+00010050: 7175 6572 7920 6c69 6b65 3a0a 0a20 2020  query like:..   
+00010060: 2020 2020 2053 454c 4543 5420 4558 4953       SELECT EXIS
+00010070: 5453 2028 5345 4c45 4354 202e 2e2e 290a  TS (SELECT ...).
+00010080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010090: 2020 2020 7374 7566 6620 3d20 7365 6c66      stuff = self
+000100a0: 2e74 6162 6c65 732e 7374 7566 660a 2020  .tables.stuff.  
+000100b0: 2020 2020 2020 6571 5f28 0a20 2020 2020        eq_(.     
+000100c0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+000100d0: 6e2e 6578 6563 7574 6528 0a20 2020 2020  n.execute(.     
+000100e0: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+000100f0: 7428 6578 6973 7473 2829 2e77 6865 7265  t(exists().where
+00010100: 2873 7475 6666 2e63 2e64 6174 6120 3d3d  (stuff.c.data ==
+00010110: 2022 736f 6d65 2064 6174 6122 2929 0a20   "some data")). 
+00010120: 2020 2020 2020 2020 2020 2029 2e66 6574             ).fet
+00010130: 6368 616c 6c28 292c 0a20 2020 2020 2020  chall(),.       
+00010140: 2020 2020 205b 2854 7275 652c 295d 2c0a       [(True,)],.
+00010150: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00010160: 6566 2074 6573 745f 7365 6c65 6374 5f65  ef test_select_e
+00010170: 7869 7374 735f 6661 6c73 6528 7365 6c66  xists_false(self
+00010180: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00010190: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000101a0: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+000101b0: 4944 453a 0a0a 2020 2020 2020 2020 5468  IDE:..        Th
+000101c0: 6520 6f72 6967 696e 616c 2074 6573 7420  e original test 
+000101d0: 6973 2074 7279 696e 6720 746f 2065 7865  is trying to exe
+000101e0: 6375 7465 2061 2071 7565 7279 206c 696b  cute a query lik
+000101f0: 653a 0a0a 2020 2020 2020 2020 5345 4c45  e:..        SELE
+00010200: 4354 202e 2e2e 0a20 2020 2020 2020 2057  CT ....        W
+00010210: 4845 5245 2045 5849 5354 5320 2853 454c  HERE EXISTS (SEL
+00010220: 4543 5420 2e2e 2e29 0a0a 2020 2020 2020  ECT ...)..      
+00010230: 2020 5345 4c45 4354 2057 4845 5245 2077    SELECT WHERE w
+00010240: 6974 686f 7574 2046 524f 4d20 636c 6175  ithout FROM clau
+00010250: 7365 2069 7320 6e6f 7420 7375 7070 6f72  se is not suppor
+00010260: 7465 6420 6279 2053 7061 6e6e 6572 2e0a  ted by Spanner..
+00010270: 2020 2020 2020 2020 5265 7772 6974 696e          Rewritin
+00010280: 6720 7468 6520 7465 7374 2074 6f20 666f  g the test to fo
+00010290: 7263 6520 6974 2074 6f20 6765 6e65 7261  rce it to genera
+000102a0: 7465 2061 2071 7565 7279 206c 696b 653a  te a query like:
+000102b0: 0a0a 2020 2020 2020 2020 5345 4c45 4354  ..        SELECT
+000102c0: 2045 5849 5354 5320 2853 454c 4543 5420   EXISTS (SELECT 
+000102d0: 2e2e 2e29 0a20 2020 2020 2020 2022 2222  ...).        """
+000102e0: 0a20 2020 2020 2020 2073 7475 6666 203d  .        stuff =
+000102f0: 2073 656c 662e 7461 626c 6573 2e73 7475   self.tables.stu
+00010300: 6666 0a20 2020 2020 2020 2065 715f 280a  ff.        eq_(.
+00010310: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+00010320: 6563 7469 6f6e 2e65 7865 6375 7465 280a  ection.execute(.
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 7365 6c65 6374 2865 7869 7374 7328 292e  select(exists().
+00010350: 7768 6572 6528 7374 7566 662e 632e 6461  where(stuff.c.da
+00010360: 7461 203d 3d20 226e 6f20 6461 7461 2229  ta == "no data")
+00010370: 290a 2020 2020 2020 2020 2020 2020 292e  ).            ).
+00010380: 6665 7463 6861 6c6c 2829 2c0a 2020 2020  fetchall(),.    
+00010390: 2020 2020 2020 2020 5b28 4661 6c73 652c          [(False,
+000103a0: 295d 2c0a 2020 2020 2020 2020 290a 0a0a  )],.        )...
+000103b0: 636c 6173 7320 5461 626c 6544 444c 5465  class TableDDLTe
+000103c0: 7374 285f 5461 626c 6544 444c 5465 7374  st(_TableDDLTest
+000103d0: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
+000103e0: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
+000103f0: 2020 2253 7061 6e6e 6572 2074 6162 6c65    "Spanner table
+00010400: 206e 616d 6520 6d75 7374 2073 7461 7274   name must start
+00010410: 2077 6974 6820 616e 2075 7070 6572 6361   with an upperca
+00010420: 7365 206f 7220 6c6f 7765 7263 6173 6520  se or lowercase 
+00010430: 6c65 7474 6572 220a 2020 2020 290a 2020  letter".    ).  
+00010440: 2020 6465 6620 7465 7374 5f75 6e64 6572    def test_under
+00010450: 7363 6f72 655f 6e61 6d65 7328 7365 6c66  score_names(self
+00010460: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00010470: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00010480: 6b2e 736b 6970 2822 5461 626c 6520 6e61  k.skip("Table na
+00010490: 6d65 7320 696e 6375 6469 6e67 2073 6368  mes incuding sch
+000104a0: 656d 6173 2061 7265 206e 6f74 2073 7570  emas are not sup
+000104b0: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
+000104c0: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
+000104d0: 5f63 7265 6174 655f 7461 626c 655f 7363  _create_table_sc
+000104e0: 6865 6d61 2873 656c 6629 3a0a 2020 2020  hema(self):.    
+000104f0: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+00010500: 2046 7574 7572 6554 6162 6c65 4444 4c54   FutureTableDDLT
+00010510: 6573 7428 5f46 7574 7572 6554 6162 6c65  est(_FutureTable
+00010520: 4444 4c54 6573 7429 3a0a 2020 2020 4070  DDLTest):.    @p
+00010530: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+00010540: 2254 6162 6c65 206e 616d 6573 2069 6e63  "Table names inc
+00010550: 7564 696e 6720 7363 6865 6d61 7320 6172  uding schemas ar
+00010560: 6520 6e6f 7420 7375 7070 6f72 7465 6420  e not supported 
+00010570: 6279 2053 7061 6e6e 6572 2229 0a20 2020  by Spanner").   
+00010580: 2064 6566 2074 6573 745f 6372 6561 7465   def test_create
+00010590: 5f74 6162 6c65 5f73 6368 656d 6128 7365  _table_schema(se
+000105a0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000105b0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+000105c0: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
+000105d0: 2020 2253 7061 6e6e 6572 2074 6162 6c65    "Spanner table
+000105e0: 206e 616d 6520 6d75 7374 2073 7461 7274   name must start
+000105f0: 2077 6974 6820 616e 2075 7070 6572 6361   with an upperca
+00010600: 7365 206f 7220 6c6f 7765 7263 6173 6520  se or lowercase 
+00010610: 6c65 7474 6572 220a 2020 2020 290a 2020  letter".    ).  
+00010620: 2020 6465 6620 7465 7374 5f75 6e64 6572    def test_under
+00010630: 7363 6f72 655f 6e61 6d65 7328 7365 6c66  score_names(self
+00010640: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00010650: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
+00010660: 6b69 7028 224d 6178 2069 6465 6e74 6966  kip("Max identif
+00010670: 6965 7220 6c65 6e67 7468 2069 6e20 5370  ier length in Sp
+00010680: 616e 6e65 7220 6973 2031 3238 2229 0a63  anner is 128").c
+00010690: 6c61 7373 204c 6f6e 674e 616d 6542 6c6f  lass LongNameBlo
+000106a0: 776f 7574 5465 7374 285f 4c6f 6e67 4e61  woutTest(_LongNa
+000106b0: 6d65 426c 6f77 6f75 7454 6573 7429 3a0a  meBlowoutTest):.
+000106c0: 2020 2020 7061 7373 0a0a 0a40 7079 7465      pass...@pyte
+000106d0: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+000106e0: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+000106f0: 7070 6f72 7420 5469 6d65 2064 6174 6120  pport Time data 
+00010700: 7479 7065 2e22 290a 636c 6173 7320 5469  type.").class Ti
+00010710: 6d65 5465 7374 7328 5f54 696d 654d 6963  meTests(_TimeMic
+00010720: 726f 7365 636f 6e64 7354 6573 742c 205f  rosecondsTest, _
+00010730: 5469 6d65 5465 7374 293a 0a20 2020 2070  TimeTest):.    p
+00010740: 6173 730a 0a0a 4070 7974 6573 742e 6d61  ass...@pytest.ma
+00010750: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
+00010760: 2064 6f65 736e 2774 2063 6f65 7263 6520   doesn't coerce 
+00010770: 6461 7465 7320 6672 6f6d 2064 6174 6574  dates from datet
+00010780: 696d 652e 2229 0a63 6c61 7373 2044 6174  ime.").class Dat
+00010790: 6554 696d 6543 6f65 7263 6564 546f 4461  eTimeCoercedToDa
+000107a0: 7465 5469 6d65 5465 7374 285f 4461 7465  teTimeTest(_Date
+000107b0: 5469 6d65 436f 6572 6365 6454 6f44 6174  TimeCoercedToDat
+000107c0: 6554 696d 6554 6573 7429 3a0a 2020 2020  eTimeTest):.    
+000107d0: 7061 7373 0a0a 0a63 6c61 7373 2049 6e74  pass...class Int
+000107e0: 6567 6572 5465 7374 285f 496e 7465 6765  egerTest(_Intege
+000107f0: 7254 6573 7429 3a0a 2020 2020 4070 726f  rTest):.    @pro
+00010800: 7669 6465 5f6d 6574 6164 6174 610a 2020  vide_metadata.  
+00010810: 2020 6465 6620 5f72 6f75 6e64 5f74 7269    def _round_tri
+00010820: 7028 7365 6c66 2c20 6461 7461 7479 7065  p(self, datatype
+00010830: 2c20 6461 7461 293a 0a20 2020 2020 2020  , data):.       
+00010840: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
+00010850: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+00010860: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+00010870: 7468 6520 6865 6c70 6572 206d 6574 686f  the helper metho
+00010880: 6420 666f 7220 696e 7465 6765 7220 636c  d for integer cl
+00010890: 6173 7320 7465 7374 7320 7768 6963 6820  ass tests which 
+000108a0: 6372 6561 7465 7320 6120 7461 626c 6520  creates a table 
+000108b0: 616e 640a 2020 2020 2020 2020 7065 7266  and.        perf
+000108c0: 6f72 6d73 2061 6e20 696e 7365 7274 206f  orms an insert o
+000108d0: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
+000108e0: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
+000108f0: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
+00010900: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
+00010910: 696d 6172 7920 6b65 792c 2062 7574 206f  imary key, but o
+00010920: 6e6c 7920 6f6e 650a 2020 2020 2020 2020  nly one.        
+00010930: 726f 7720 6361 6e20 6265 2069 6e73 6572  row can be inser
+00010940: 7465 6420 696e 746f 2073 7563 6820 6120  ted into such a 
+00010950: 7461 626c 6520 2d20 666f 6c6c 6f77 696e  table - followin
+00010960: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
+00010970: 6c20 6661 696c 2077 6974 680a 2020 2020  l fail with.    
+00010980: 2020 2020 6034 3030 2069 6420 6d75 7374      `400 id must
+00010990: 206e 6f74 2062 6520 4e55 4c4c 2069 6e20   not be NULL in 
+000109a0: 7461 626c 6520 6461 7465 5f74 6162 6c65  table date_table
+000109b0: 602e 0a20 2020 2020 2020 204f 7665 7272  `..        Overr
+000109c0: 6964 696e 6720 7468 6520 7465 7374 7320  iding the tests 
+000109d0: 616e 6420 6164 6469 6e67 2061 206d 616e  and adding a man
+000109e0: 7561 6c20 7072 696d 6172 7920 6b65 7920  ual primary key 
+000109f0: 7661 6c75 6520 746f 2061 766f 6964 2074  value to avoid t
+00010a00: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
+00010a10: 6661 696c 7572 6573 2e0a 2020 2020 2020  failures..      
+00010a20: 2020 2222 220a 2020 2020 2020 2020 6d65    """.        me
+00010a30: 7461 6461 7461 203d 2073 656c 662e 6d65  tadata = self.me
+00010a40: 7461 6461 7461 0a20 2020 2020 2020 2069  tadata.        i
+00010a50: 6e74 5f74 6162 6c65 203d 2054 6162 6c65  nt_table = Table
+00010a60: 280a 2020 2020 2020 2020 2020 2020 2269  (.            "i
+00010a70: 6e74 6567 6572 5f74 6162 6c65 222c 0a20  nteger_table",. 
+00010a80: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+00010a90: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00010aa0: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
+00010ab0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+00010ac0: 6579 3d54 7275 652c 2074 6573 745f 6e65  ey=True, test_ne
+00010ad0: 6564 735f 6175 746f 696e 6372 656d 656e  eds_autoincremen
+00010ae0: 743d 5472 7565 292c 0a20 2020 2020 2020  t=True),.       
+00010af0: 2020 2020 2043 6f6c 756d 6e28 2269 6e74       Column("int
+00010b00: 6567 6572 5f64 6174 6122 2c20 6461 7461  eger_data", data
+00010b10: 7479 7065 292c 0a20 2020 2020 2020 2029  type),.        )
+00010b20: 0a0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
+00010b30: 7461 2e63 7265 6174 655f 616c 6c28 636f  ta.create_all(co
+00010b40: 6e66 6967 2e64 6229 0a0a 2020 2020 2020  nfig.db)..      
+00010b50: 2020 636f 6e66 6967 2e64 622e 6578 6563    config.db.exec
+00010b60: 7574 6528 696e 745f 7461 626c 652e 696e  ute(int_table.in
+00010b70: 7365 7274 2829 2c20 7b22 6964 223a 2031  sert(), {"id": 1
+00010b80: 2c20 2269 6e74 6567 6572 5f64 6174 6122  , "integer_data"
+00010b90: 3a20 6461 7461 7d29 0a0a 2020 2020 2020  : data})..      
+00010ba0: 2020 726f 7720 3d20 636f 6e66 6967 2e64    row = config.d
+00010bb0: 622e 6578 6563 7574 6528 7365 6c65 6374  b.execute(select
+00010bc0: 2869 6e74 5f74 6162 6c65 2e63 2e69 6e74  (int_table.c.int
+00010bd0: 6567 6572 5f64 6174 6129 292e 6669 7273  eger_data)).firs
+00010be0: 7428 290a 0a20 2020 2020 2020 2065 715f  t()..        eq_
+00010bf0: 2872 6f77 2c20 2864 6174 612c 2929 0a0a  (row, (data,))..
+00010c00: 2020 2020 2020 2020 6966 2075 7469 6c2e          if util.
+00010c10: 7079 336b 3a0a 2020 2020 2020 2020 2020  py3k:.          
+00010c20: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00010c30: 6e63 6528 726f 775b 305d 2c20 696e 7429  nce(row[0], int)
+00010c40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00010c50: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00010c60: 7420 6973 696e 7374 616e 6365 2872 6f77  t isinstance(row
+00010c70: 5b30 5d2c 2028 6c6f 6e67 2c20 696e 7429  [0], (long, int)
+00010c80: 2920 2023 206e 6f71 610a 0a20 2020 2064  )  # noqa..    d
+00010c90: 6566 205f 6875 6765 5f69 6e74 7328 293a  ef _huge_ints():
+00010ca0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00010cb0: 2074 6573 7469 6e67 2e63 6f6d 6269 6e61   testing.combina
+00010cc0: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
+00010cd0: 2020 2032 3134 3734 3833 3634 392c 2020     2147483649,  
+00010ce0: 2320 3332 2062 6974 730a 2020 2020 2020  # 32 bits.      
+00010cf0: 2020 2020 2020 3231 3437 3438 3336 3438        2147483648
+00010d00: 2c20 2023 2033 3220 6269 7473 0a20 2020  ,  # 32 bits.   
+00010d10: 2020 2020 2020 2020 2032 3134 3734 3833           2147483
+00010d20: 3634 372c 2020 2320 3331 2062 6974 730a  647,  # 31 bits.
+00010d30: 2020 2020 2020 2020 2020 2020 3231 3437              2147
+00010d40: 3438 3336 3436 2c20 2023 2033 3120 6269  483646,  # 31 bi
+00010d50: 7473 0a20 2020 2020 2020 2020 2020 202d  ts.            -
+00010d60: 3231 3437 3438 3336 3439 2c20 2023 2033  2147483649,  # 3
+00010d70: 3220 6269 7473 0a20 2020 2020 2020 2020  2 bits.         
+00010d80: 2020 202d 3231 3437 3438 3336 3438 2c20     -2147483648, 
+00010d90: 2023 2033 3220 696e 7465 7265 7374 696e   # 32 interestin
+00010da0: 676c 792c 2061 7379 6e63 7067 2061 6363  gly, asyncpg acc
+00010db0: 6570 7473 2074 6869 7320 6f6e 6520 6173  epts this one as
+00010dc0: 2069 6e74 3332 0a20 2020 2020 2020 2020   int32.         
+00010dd0: 2020 202d 3231 3437 3438 3336 3437 2c20     -2147483647, 
+00010de0: 2023 2033 310a 2020 2020 2020 2020 2020   # 31.          
+00010df0: 2020 2d32 3134 3734 3833 3634 362c 2020    -2147483646,  
+00010e00: 2320 3331 0a20 2020 2020 2020 2020 2020  # 31.           
+00010e10: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+00010e20: 3133 3736 3533 3730 3138 3336 3831 3237  1376537018368127
+00010e30: 2c0a 2020 2020 2020 2020 2020 2020 2d31  ,.            -1
+00010e40: 3337 3635 3337 3031 3833 3638 3132 372c  376537018368127,
+00010e50: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00010e60: 6e61 6d65 733d 2269 6e74 7661 6c75 6522  names="intvalue"
+00010e70: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00010e80: 2040 5f68 7567 655f 696e 7473 2829 0a20   @_huge_ints(). 
+00010e90: 2020 2064 6566 2074 6573 745f 6875 6765     def test_huge
+00010ea0: 5f69 6e74 5f61 7574 6f5f 6163 636f 6d6d  _int_auto_accomm
+00010eb0: 6f64 6174 696f 6e28 7365 6c66 2c20 636f  odation(self, co
+00010ec0: 6e6e 6563 7469 6f6e 2c20 696e 7476 616c  nnection, intval
+00010ed0: 7565 293a 0a20 2020 2020 2020 2022 2222  ue):.        """
+00010ee0: 0a20 2020 2020 2020 2053 7061 6e6e 6572  .        Spanner
+00010ef0: 2064 6f65 7320 6e6f 7420 616c 6c6f 7720   does not allow 
+00010f00: 7175 6572 7920 746f 2068 6176 6520 4652  query to have FR
+00010f10: 4f4d 2063 6c61 7573 6520 7769 7468 6f75  OM clause withou
+00010f20: 7420 6120 5748 4552 4520 636c 6175 7365  t a WHERE clause
+00010f30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010f40: 2020 2020 2065 715f 280a 2020 2020 2020       eq_(.      
+00010f50: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+00010f60: 2e73 6361 6c61 7228 7365 6c65 6374 2869  .scalar(select(i
+00010f70: 6e74 7661 6c75 6529 292c 0a20 2020 2020  ntvalue)),.     
+00010f80: 2020 2020 2020 2069 6e74 7661 6c75 652c         intvalue,
+00010f90: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00010fa0: 7373 205f 556e 6963 6f64 6546 6978 7475  ss _UnicodeFixtu
+00010fb0: 7265 285f 5f55 6e69 636f 6465 4669 7874  re(__UnicodeFixt
+00010fc0: 7572 6529 3a0a 2020 2020 4063 6c61 7373  ure):.    @class
+00010fd0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+00010fe0: 6566 696e 655f 7461 626c 6573 2863 6c73  efine_tables(cls
+00010ff0: 2c20 6d65 7461 6461 7461 293a 0a20 2020  , metadata):.   
+00011000: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011010: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+00011020: 453a 0a0a 2020 2020 2020 2020 436c 6f75  E:..        Clou
+00011030: 6420 5370 616e 6e65 7220 646f 6573 6e27  d Spanner doesn'
+00011040: 7420 7375 7070 6f72 7420 6175 746f 2069  t support auto i
+00011050: 6e63 7265 6d65 6e74 696e 6720 6964 7320  ncrementing ids 
+00011060: 6665 6174 7572 652c 0a20 2020 2020 2020  feature,.       
+00011070: 2077 6869 6368 2069 7320 7573 6564 2062   which is used b
+00011080: 7920 7468 6520 6f72 6967 696e 616c 2074  y the original t
+00011090: 6573 742e 204f 7665 7272 6964 696e 6720  est. Overriding 
+000110a0: 7468 6520 7465 7374 2064 6174 610a 2020  the test data.  
+000110b0: 2020 2020 2020 6372 6561 7469 6f6e 206d        creation m
+000110c0: 6574 686f 6420 746f 2064 6973 6162 6c65  ethod to disable
+000110d0: 2061 7574 6f69 6e63 7265 6d65 6e74 2061   autoincrement a
+000110e0: 6e64 206d 616b 6520 6964 2063 6f6c 756d  nd make id colum
+000110f0: 6e0a 2020 2020 2020 2020 6e75 6c6c 6162  n.        nullab
+00011100: 6c65 2e0a 2020 2020 2020 2020 2222 220a  le..        """.
+00011110: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+00011120: 2020 2020 2020 2020 2020 2022 756e 6963             "unic
+00011130: 6f64 655f 7461 626c 6522 2c0a 2020 2020  ode_table",.    
+00011140: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+00011150: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+00011160: 6c75 6d6e 2822 6964 222c 2049 6e74 6567  lumn("id", Integ
+00011170: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+00011180: 5472 7565 2c20 6e75 6c6c 6162 6c65 3d54  True, nullable=T
+00011190: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+000111a0: 2020 436f 6c75 6d6e 2822 756e 6963 6f64    Column("unicod
+000111b0: 655f 6461 7461 222c 2063 6c73 2e64 6174  e_data", cls.dat
+000111c0: 6174 7970 6529 2c0a 2020 2020 2020 2020  atype),.        
+000111d0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000111e0: 726f 756e 645f 7472 6970 5f65 7865 6375  round_trip_execu
+000111f0: 7465 6d61 6e79 2873 656c 662c 2063 6f6e  temany(self, con
+00011200: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+00011210: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00011220: 414e 4e45 5220 4f56 4552 5249 4445 0a0a  ANNER OVERRIDE..
+00011230: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
+00011240: 616e 6e65 7220 7375 7070 6f72 7473 2074  anner supports t
+00011250: 6162 6c65 7320 7769 7468 2065 6d70 7479  ables with empty
+00011260: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
+00011270: 740a 2020 2020 2020 2020 6f6e 6c79 2073  t.        only s
+00011280: 696e 676c 6520 6f6e 6520 726f 7720 6361  ingle one row ca
+00011290: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
+000112a0: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
+000112b0: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
+000112c0: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
+000112d0: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
+000112e0: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
+000112f0: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
+00011300: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+00011310: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
+00011320: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
+00011330: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011340: 2020 756e 6963 6f64 655f 7461 626c 6520    unicode_table 
+00011350: 3d20 7365 6c66 2e74 6162 6c65 732e 756e  = self.tables.un
+00011360: 6963 6f64 655f 7461 626c 650a 0a20 2020  icode_table..   
+00011370: 2020 2020 2063 6f6e 6e65 6374 696f 6e2e       connection.
+00011380: 6578 6563 7574 6528 0a20 2020 2020 2020  execute(.       
+00011390: 2020 2020 2075 6e69 636f 6465 5f74 6162       unicode_tab
+000113a0: 6c65 2e69 6e73 6572 7428 292c 0a20 2020  le.insert(),.   
+000113b0: 2020 2020 2020 2020 205b 7b22 6964 223a           [{"id":
+000113c0: 2069 2c20 2275 6e69 636f 6465 5f64 6174   i, "unicode_dat
+000113d0: 6122 3a20 7365 6c66 2e64 6174 617d 2066  a": self.data} f
+000113e0: 6f72 2069 2069 6e20 7261 6e67 6528 312c  or i in range(1,
+000113f0: 2034 295d 2c0a 2020 2020 2020 2020 290a   4)],.        ).
+00011400: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
+00011410: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
+00011420: 7465 2873 656c 6563 7428 756e 6963 6f64  te(select(unicod
+00011430: 655f 7461 626c 652e 632e 756e 6963 6f64  e_table.c.unicod
+00011440: 655f 6461 7461 2929 2e66 6574 6368 616c  e_data)).fetchal
+00011450: 6c28 290a 2020 2020 2020 2020 6571 5f28  l().        eq_(
+00011460: 726f 7773 2c20 5b28 7365 6c66 2e64 6174  rows, [(self.dat
+00011470: 612c 2920 666f 7220 6920 696e 2072 616e  a,) for i in ran
+00011480: 6765 2831 2c20 3429 5d29 0a20 2020 2020  ge(1, 4)]).     
+00011490: 2020 2066 6f72 2072 6f77 2069 6e20 726f     for row in ro
+000114a0: 7773 3a0a 2020 2020 2020 2020 2020 2020  ws:.            
+000114b0: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+000114c0: 6528 726f 775b 305d 2c20 7374 7229 0a0a  e(row[0], str)..
+000114d0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+000114e0: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+000114f0: 6f65 736e 2774 2073 7570 706f 7274 206e  oesn't support n
+00011500: 6f6e 2d61 7363 6969 2063 6861 7261 6374  on-ascii charact
+00011510: 6572 7322 290a 2020 2020 6465 6620 7465  ers").    def te
+00011520: 7374 5f6c 6974 6572 616c 2873 656c 6629  st_literal(self)
+00011530: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00011540: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00011550: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+00011560: 6f65 736e 2774 2073 7570 706f 7274 206e  oesn't support n
+00011570: 6f6e 2d61 7363 6969 2063 6861 7261 6374  on-ascii charact
+00011580: 6572 7322 290a 2020 2020 6465 6620 7465  ers").    def te
+00011590: 7374 5f6c 6974 6572 616c 5f6e 6f6e 5f61  st_literal_non_a
+000115a0: 7363 6969 2873 656c 6629 3a0a 2020 2020  scii(self):.    
+000115b0: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+000115c0: 2055 6e69 636f 6465 5661 7263 6861 7254   UnicodeVarcharT
+000115d0: 6573 7428 5f55 6e69 636f 6465 4669 7874  est(_UnicodeFixt
+000115e0: 7572 652c 205f 556e 6963 6f64 6556 6172  ure, _UnicodeVar
+000115f0: 6368 6172 5465 7374 293a 0a20 2020 2022  charTest):.    "
+00011600: 2222 0a20 2020 2053 5041 4e4e 4552 204f  "".    SPANNER O
+00011610: 5645 5252 4944 453a 0a0a 2020 2020 556e  VERRIDE:..    Un
+00011620: 6963 6f64 6556 6172 6368 6172 5465 7374  icodeVarcharTest
+00011630: 2063 6c61 7373 2069 6e68 6572 6974 7320   class inherits 
+00011640: 7468 6520 5f5f 556e 6963 6f64 6546 6978  the __UnicodeFix
+00011650: 7475 7265 2063 6c61 7373 2773 2074 6573  ture class's tes
+00011660: 7473 2c0a 2020 2020 736f 2074 6f20 6176  ts,.    so to av
+00011670: 6f69 6420 7468 6f73 6520 6661 696c 7572  oid those failur
+00011680: 6573 2061 6e64 206d 6169 6e74 6169 6e20  es and maintain 
+00011690: 4452 5920 636f 6e63 6570 7420 6a75 7374  DRY concept just
+000116a0: 2069 6e68 6572 6974 2074 6865 2063 6c61   inherit the cla
+000116b0: 7373 2074 6f20 7275 6e0a 2020 2020 7465  ss to run.    te
+000116c0: 7374 7320 7375 6363 6573 7366 756c 6c79  sts successfully
+000116d0: 2e0a 2020 2020 2222 220a 0a20 2020 2070  ..    """..    p
+000116e0: 6173 730a 0a0a 636c 6173 7320 556e 6963  ass...class Unic
+000116f0: 6f64 6554 6578 7454 6573 7428 5f55 6e69  odeTextTest(_Uni
+00011700: 636f 6465 4669 7874 7572 652c 205f 556e  codeFixture, _Un
+00011710: 6963 6f64 6554 6578 7454 6573 7429 3a0a  icodeTextTest):.
+00011720: 2020 2020 2222 220a 2020 2020 5350 414e      """.    SPAN
+00011730: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+00011740: 2020 2055 6e69 636f 6465 5465 7874 5465     UnicodeTextTe
+00011750: 7374 2063 6c61 7373 2069 6e68 6572 6974  st class inherit
+00011760: 7320 7468 6520 5f5f 556e 6963 6f64 6546  s the __UnicodeF
+00011770: 6978 7475 7265 2063 6c61 7373 2773 2074  ixture class's t
+00011780: 6573 7473 2c0a 2020 2020 736f 2074 6f20  ests,.    so to 
+00011790: 6176 6f69 6420 7468 6f73 6520 6661 696c  avoid those fail
+000117a0: 7572 6573 2061 6e64 206d 6169 6e74 6169  ures and maintai
+000117b0: 6e20 4452 5920 636f 6e63 6570 7420 6a75  n DRY concept ju
+000117c0: 7374 2069 6e68 6572 6974 2074 6865 2063  st inherit the c
+000117d0: 6c61 7373 2074 6f20 7275 6e0a 2020 2020  lass to run.    
+000117e0: 7465 7374 7320 7375 6363 6573 7366 756c  tests successful
+000117f0: 6c79 2e0a 2020 2020 2222 220a 0a20 2020  ly..    """..   
+00011800: 2070 6173 730a 0a0a 636c 6173 7320 526f   pass...class Ro
+00011810: 7746 6574 6368 5465 7374 285f 526f 7746  wFetchTest(_RowF
+00011820: 6574 6368 5465 7374 293a 0a20 2020 2064  etchTest):.    d
+00011830: 6566 2074 6573 745f 726f 775f 775f 7363  ef test_row_w_sc
+00011840: 616c 6172 5f73 656c 6563 7428 7365 6c66  alar_select(self
+00011850: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00011860: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011870: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+00011880: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
+00011890: 6f75 6420 5370 616e 6e65 7220 7265 7475  oud Spanner retu
+000118a0: 726e 7320 6120 4461 7465 7469 6d65 5769  rns a DatetimeWi
+000118b0: 7468 4e61 6e6f 7365 636f 6e64 7328 2920  thNanoseconds() 
+000118c0: 666f 7220 6461 7465 0a20 2020 2020 2020  for date.       
+000118d0: 2064 6174 6120 7479 7065 732e 204f 7665   data types. Ove
+000118e0: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
+000118f0: 2074 6f20 7573 6520 6120 4461 7465 7469   to use a Dateti
+00011900: 6d65 5769 7468 4e61 6e6f 7365 636f 6e64  meWithNanosecond
+00011910: 730a 2020 2020 2020 2020 7479 7065 2076  s.        type v
+00011920: 616c 7565 2061 7320 616e 2065 7870 6563  alue as an expec
+00011930: 7465 6420 7265 7375 6c74 2e0a 2020 2020  ted result..    
+00011940: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00011950: 2d2d 0a0a 2020 2020 2020 2020 7465 7374  --..        test
+00011960: 2074 6861 7420 6120 7363 616c 6172 2073   that a scalar s
+00011970: 656c 6563 7420 6173 2061 2063 6f6c 756d  elect as a colum
+00011980: 6e20 6973 2072 6574 7572 6e65 6420 6173  n is returned as
+00011990: 2073 7563 680a 2020 2020 2020 2020 616e   such.        an
+000119a0: 6420 7468 6174 2074 7970 6520 636f 6e76  d that type conv
+000119b0: 6572 7369 6f6e 2077 6f72 6b73 204f 4b2e  ersion works OK.
+000119c0: 0a0a 2020 2020 2020 2020 2874 6869 7320  ..        (this 
+000119d0: 6973 2068 616c 6620 6120 5351 4c41 6c63  is half a SQLAlc
+000119e0: 6865 6d79 2043 6f72 6520 7465 7374 2061  hemy Core test a
+000119f0: 6e64 2068 616c 6620 746f 2063 6174 6368  nd half to catch
+00011a00: 2064 6174 6162 6173 650a 2020 2020 2020   database.      
+00011a10: 2020 6261 636b 656e 6473 2074 6861 7420    backends that 
+00011a20: 6d61 7920 6861 7665 2075 6e75 7375 616c  may have unusual
+00011a30: 2062 6568 6176 696f 7220 7769 7468 2073   behavior with s
+00011a40: 6361 6c61 7220 7365 6c65 6374 732e 290a  calar selects.).
+00011a50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011a60: 2020 2020 6461 7465 7461 626c 6520 3d20      datetable = 
+00011a70: 7365 6c66 2e74 6162 6c65 732e 6861 735f  self.tables.has_
+00011a80: 6461 7465 730a 2020 2020 2020 2020 7320  dates.        s 
+00011a90: 3d20 7365 6c65 6374 2864 6174 6574 6162  = select(datetab
+00011aa0: 6c65 2e61 6c69 6173 2822 7822 292e 632e  le.alias("x").c.
+00011ab0: 746f 6461 7929 2e73 6361 6c61 725f 7375  today).scalar_su
+00011ac0: 6271 7565 7279 2829 0a20 2020 2020 2020  bquery().       
+00011ad0: 2073 3220 3d20 7365 6c65 6374 2864 6174   s2 = select(dat
+00011ae0: 6574 6162 6c65 2e63 2e69 642c 2073 2e6c  etable.c.id, s.l
+00011af0: 6162 656c 2822 736f 6d65 6c61 6265 6c22  abel("somelabel"
+00011b00: 2929 0a20 2020 2020 2020 2072 6f77 203d  )).        row =
+00011b10: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
+00011b20: 7574 6528 7332 292e 6669 7273 7428 290a  ute(s2).first().
+00011b30: 0a20 2020 2020 2020 2065 715f 280a 2020  .        eq_(.  
+00011b40: 2020 2020 2020 2020 2020 726f 772e 736f            row.so
+00011b50: 6d65 6c61 6265 6c2c 0a20 2020 2020 2020  melabel,.       
+00011b60: 2020 2020 2044 6174 6574 696d 6557 6974       DatetimeWit
+00011b70: 684e 616e 6f73 6563 6f6e 6473 2832 3030  hNanoseconds(200
+00011b80: 362c 2035 2c20 3132 2c20 3132 2c20 302c  6, 5, 12, 12, 0,
+00011b90: 2030 2c20 747a 696e 666f 3d74 696d 657a   0, tzinfo=timez
+00011ba0: 6f6e 652e 7574 6329 2c0a 2020 2020 2020  one.utc),.      
+00011bb0: 2020 290a 0a0a 636c 6173 7320 496e 7365    )...class Inse
+00011bc0: 7274 4265 6861 7669 6f72 5465 7374 285f  rtBehaviorTest(_
+00011bd0: 496e 7365 7274 4265 6861 7669 6f72 5465  InsertBehaviorTe
+00011be0: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
+00011bf0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+00011c00: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+00011c10: 6f72 7420 656d 7074 7920 696e 7365 7274  ort empty insert
+00011c20: 7322 290a 2020 2020 6465 6620 7465 7374  s").    def test
+00011c30: 5f65 6d70 7479 5f69 6e73 6572 7428 7365  _empty_insert(se
+00011c40: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00011c50: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+00011c60: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+00011c70: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+00011c80: 7420 656d 7074 7920 696e 7365 7274 7322  t empty inserts"
+00011c90: 290a 2020 2020 6465 6620 7465 7374 5f65  ).    def test_e
+00011ca0: 6d70 7479 5f69 6e73 6572 745f 6d75 6c74  mpty_insert_mult
+00011cb0: 6970 6c65 2873 656c 6629 3a0a 2020 2020  iple(self):.    
+00011cc0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+00011cd0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+00011ce0: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
+00011cf0: 2073 7570 706f 7274 2061 7574 6f20 696e   support auto in
+00011d00: 6372 656d 656e 7422 290a 2020 2020 6465  crement").    de
+00011d10: 6620 7465 7374 5f69 6e73 6572 745f 6672  f test_insert_fr
+00011d20: 6f6d 5f73 656c 6563 745f 6175 746f 696e  om_select_autoin
+00011d30: 6328 7365 6c66 293a 0a20 2020 2020 2020  c(self):.       
+00011d40: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00011d50: 6573 745f 6175 746f 636c 6f73 655f 6f6e  est_autoclose_on
+00011d60: 5f69 6e73 6572 7428 7365 6c66 293a 0a20  _insert(self):. 
+00011d70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011d80: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+00011d90: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
+00011da0: 6f75 6420 5370 616e 6e65 7220 646f 6573  oud Spanner does
+00011db0: 6e27 7420 7375 7070 6f72 7420 7461 626c  n't support tabl
+00011dc0: 6573 2077 6974 6820 616e 2061 7574 6f20  es with an auto 
+00011dd0: 696e 6372 656d 656e 7420 7072 696d 6172  increment primar
+00011de0: 7920 6b65 792c 0a20 2020 2020 2020 2066  y key,.        f
+00011df0: 6f6c 6c6f 7769 6e67 2069 6e73 6572 7469  ollowing inserti
+00011e00: 6f6e 7320 7769 6c6c 2066 6169 6c20 7769  ons will fail wi
+00011e10: 7468 2060 3430 3020 6964 206d 7573 7420  th `400 id must 
+00011e20: 6e6f 7420 6265 204e 554c 4c20 696e 2074  not be NULL in t
+00011e30: 6162 6c65 0a20 2020 2020 2020 2061 7574  able.        aut
+00011e40: 6f69 6e63 5f70 6b60 2e0a 0a20 2020 2020  oinc_pk`...     
+00011e50: 2020 204f 7665 7272 6964 696e 6720 7468     Overriding th
+00011e60: 6520 7465 7374 7320 616e 6420 6164 6469  e tests and addi
+00011e70: 6e67 2061 206d 616e 7561 6c20 7072 696d  ng a manual prim
+00011e80: 6172 7920 6b65 7920 7661 6c75 6520 746f  ary key value to
+00011e90: 2061 766f 6964 2074 6865 2073 616d 650a   avoid the same.
+00011ea0: 2020 2020 2020 2020 6661 696c 7572 6573          failures
+00011eb0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00011ec0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+00011ed0: 2020 2020 2020 2068 6173 6174 7472 2863         hasattr(c
+00011ee0: 6f6e 6669 672e 7265 7175 6972 656d 656e  onfig.requiremen
+00011ef0: 7473 2c20 2272 6574 7572 6e69 6e67 2229  ts, "returning")
+00011f00: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00011f10: 2063 6f6e 6669 672e 7265 7175 6972 656d   config.requirem
+00011f20: 656e 7473 2e72 6574 7572 6e69 6e67 2e65  ents.returning.e
+00011f30: 6e61 626c 6564 0a20 2020 2020 2020 2029  nabled.        )
+00011f40: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
+00011f50: 6769 6e65 203d 2065 6e67 696e 6573 2e74  gine = engines.t
+00011f60: 6573 7469 6e67 5f65 6e67 696e 6528 6f70  esting_engine(op
+00011f70: 7469 6f6e 733d 7b22 696d 706c 6963 6974  tions={"implicit
+00011f80: 5f72 6574 7572 6e69 6e67 223a 2046 616c  _returning": Fal
+00011f90: 7365 7d29 0a20 2020 2020 2020 2065 6c73  se}).        els
+00011fa0: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+00011fb0: 6e67 696e 6520 3d20 636f 6e66 6967 2e64  ngine = config.d
+00011fc0: 620a 0a20 2020 2020 2020 2077 6974 6820  b..        with 
+00011fd0: 656e 6769 6e65 2e62 6567 696e 2829 2061  engine.begin() a
+00011fe0: 7320 636f 6e6e 3a0a 2020 2020 2020 2020  s conn:.        
+00011ff0: 2020 2020 7220 3d20 636f 6e6e 2e65 7865      r = conn.exe
+00012000: 6375 7465 280a 2020 2020 2020 2020 2020  cute(.          
+00012010: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
+00012020: 732e 6175 746f 696e 635f 706b 2e69 6e73  s.autoinc_pk.ins
+00012030: 6572 7428 292c 2064 6963 7428 6964 3d31  ert(), dict(id=1
+00012040: 2c20 6461 7461 3d22 736f 6d65 2064 6174  , data="some dat
+00012050: 6122 290a 2020 2020 2020 2020 2020 2020  a").            
+00012060: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00012070: 7420 722e 5f73 6f66 745f 636c 6f73 6564  t r._soft_closed
+00012080: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00012090: 6e6f 7420 722e 636c 6f73 6564 0a20 2020  not r.closed.   
+000120a0: 2020 2020 2061 7373 6572 7420 722e 6973       assert r.is
+000120b0: 5f69 6e73 6572 740a 2020 2020 2020 2020  _insert.        
+000120c0: 6173 7365 7274 206e 6f74 2072 2e72 6574  assert not r.ret
+000120d0: 7572 6e73 5f72 6f77 730a 0a0a 636c 6173  urns_rows...clas
+000120e0: 7320 4279 7465 7354 6573 7428 5f4c 6974  s BytesTest(_Lit
+000120f0: 6572 616c 526f 756e 6454 7269 7046 6978  eralRoundTripFix
+00012100: 7475 7265 2c20 6669 7874 7572 6573 2e54  ture, fixtures.T
+00012110: 6573 7442 6173 6529 3a0a 2020 2020 5f5f  estBase):.    __
+00012120: 6261 636b 656e 645f 5f20 3d20 5472 7565  backend__ = True
+00012130: 0a0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
+00012140: 6f6c 656e 6774 685f 6269 6e61 7279 2873  olength_binary(s
+00012150: 656c 6629 3a0a 2020 2020 2020 2020 6d65  elf):.        me
+00012160: 7461 6461 7461 203d 204d 6574 6144 6174  tadata = MetaDat
+00012170: 6128 290a 2020 2020 2020 2020 666f 6f20  a().        foo 
+00012180: 3d20 5461 626c 6528 2266 6f6f 222c 206d  = Table("foo", m
+00012190: 6574 6164 6174 612c 2043 6f6c 756d 6e28  etadata, Column(
+000121a0: 226f 6e65 222c 204c 6172 6765 4269 6e61  "one", LargeBina
+000121b0: 7279 2929 0a0a 2020 2020 2020 2020 666f  ry))..        fo
+000121c0: 6f2e 6372 6561 7465 2863 6f6e 6669 672e  o.create(config.
+000121d0: 6462 290a 2020 2020 2020 2020 666f 6f2e  db).        foo.
+000121e0: 6472 6f70 2863 6f6e 6669 672e 6462 290a  drop(config.db).
+000121f0: 0a0a 636c 6173 7320 5374 7269 6e67 5465  ..class StringTe
+00012200: 7374 285f 5374 7269 6e67 5465 7374 293a  st(_StringTest):
+00012210: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00012220: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
+00012230: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+00012240: 6e6f 6e2d 6173 6369 6920 6368 6172 6163  non-ascii charac
+00012250: 7465 7273 2229 0a20 2020 2064 6566 2074  ters").    def t
+00012260: 6573 745f 6c69 7465 7261 6c5f 6e6f 6e5f  est_literal_non_
+00012270: 6173 6369 6928 7365 6c66 293a 0a20 2020  ascii(self):.   
+00012280: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00012290: 6566 2074 6573 745f 646f 6e74 5f74 7275  ef test_dont_tru
+000122a0: 6e63 6174 655f 7269 6768 7473 6964 6528  ncate_rightside(
+000122b0: 0a20 2020 2020 2020 2073 656c 662c 206d  .        self, m
+000122c0: 6574 6164 6174 612c 2063 6f6e 6e65 6374  etadata, connect
+000122d0: 696f 6e2c 2065 7870 723d 4e6f 6e65 2c20  ion, expr=None, 
+000122e0: 6578 7065 6374 6564 3d4e 6f6e 650a 2020  expected=None.  
+000122f0: 2020 293a 0a20 2020 2020 2020 2074 203d    ):.        t =
+00012300: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00012310: 2020 2020 2274 222c 0a20 2020 2020 2020      "t",.       
+00012320: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00012330: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00012340: 6e28 2278 222c 2053 7472 696e 6728 3229  n("x", String(2)
+00012350: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+00012360: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
+00012370: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+00012380: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00012390: 290a 2020 2020 2020 2020 742e 6372 6561  ).        t.crea
+000123a0: 7465 2863 6f6e 6e65 6374 696f 6e29 0a20  te(connection). 
+000123b0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+000123c0: 6e2e 636f 6e6e 6563 7469 6f6e 2e63 6f6d  n.connection.com
+000123d0: 6d69 7428 290a 2020 2020 2020 2020 636f  mit().        co
+000123e0: 6e6e 6563 7469 6f6e 2e65 7865 6375 7465  nnection.execute
+000123f0: 280a 2020 2020 2020 2020 2020 2020 742e  (.            t.
+00012400: 696e 7365 7274 2829 2c0a 2020 2020 2020  insert(),.      
+00012410: 2020 2020 2020 5b7b 2278 223a 2022 4142        [{"x": "AB
+00012420: 222c 2022 6964 223a 2031 7d2c 207b 2278  ", "id": 1}, {"x
+00012430: 223a 2022 4243 222c 2022 6964 223a 2032  ": "BC", "id": 2
+00012440: 7d2c 207b 2278 223a 2022 4143 222c 2022  }, {"x": "AC", "
+00012450: 6964 223a 2033 7d5d 2c0a 2020 2020 2020  id": 3}],.      
+00012460: 2020 290a 2020 2020 2020 2020 636f 6d62    ).        comb
+00012470: 696e 6174 696f 6e73 203d 205b 2822 2542  inations = [("%B
+00012480: 2522 2c20 5b22 4142 222c 2022 4243 225d  %", ["AB", "BC"]
+00012490: 292c 2028 2241 2543 222c 205b 2241 4322  ), ("A%C", ["AC"
+000124a0: 5d29 2c20 2822 4125 4325 5a22 2c20 5b5d  ]), ("A%C%Z", []
+000124b0: 295d 0a0a 2020 2020 2020 2020 666f 7220  )]..        for 
+000124c0: 6172 6773 2069 6e20 636f 6d62 696e 6174  args in combinat
+000124d0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+000124e0: 2020 6571 5f28 0a20 2020 2020 2020 2020    eq_(.         
+000124f0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+00012500: 6e2e 7363 616c 6172 7328 7365 6c65 6374  n.scalars(select
+00012510: 2874 2e63 2e78 292e 7768 6572 6528 742e  (t.c.x).where(t.
+00012520: 632e 782e 6c69 6b65 2861 7267 735b 305d  c.x.like(args[0]
+00012530: 2929 292e 616c 6c28 292c 0a20 2020 2020  ))).all(),.     
+00012540: 2020 2020 2020 2020 2020 2061 7267 735b             args[
+00012550: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00012560: 290a 0a0a 636c 6173 7320 5465 7874 5465  )...class TextTe
+00012570: 7374 285f 5465 7874 5465 7374 293a 0a20  st(_TextTest):. 
+00012580: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00012590: 2020 2020 6465 6620 6465 6669 6e65 5f74      def define_t
+000125a0: 6162 6c65 7328 636c 732c 206d 6574 6164  ables(cls, metad
+000125b0: 6174 6129 3a0a 2020 2020 2020 2020 2222  ata):.        ""
+000125c0: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
+000125d0: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
+000125e0: 2020 2020 2043 6c6f 7564 2053 7061 6e6e       Cloud Spann
+000125f0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+00012600: 7274 2061 7574 6f20 696e 6372 656d 656e  rt auto incremen
+00012610: 7469 6e67 2069 6473 2066 6561 7475 7265  ting ids feature
+00012620: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
+00012630: 6973 2075 7365 6420 6279 2074 6865 206f  is used by the o
+00012640: 7269 6769 6e61 6c20 7465 7374 2e20 4f76  riginal test. Ov
+00012650: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
+00012660: 7420 6461 7461 0a20 2020 2020 2020 2063  t data.        c
+00012670: 7265 6174 696f 6e20 6d65 7468 6f64 2074  reation method t
+00012680: 6f20 6469 7361 626c 6520 6175 746f 696e  o disable autoin
+00012690: 6372 656d 656e 7420 616e 6420 6d61 6b65  crement and make
+000126a0: 2069 6420 636f 6c75 6d6e 0a20 2020 2020   id column.     
+000126b0: 2020 206e 756c 6c61 626c 652e 0a20 2020     nullable..   
+000126c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000126d0: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+000126e0: 2020 2020 2274 6578 745f 7461 626c 6522      "text_table"
+000126f0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00012700: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
+00012710: 2020 2020 436f 6c75 6d6e 2822 6964 222c      Column("id",
+00012720: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
+00012730: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
+00012740: 6162 6c65 3d54 7275 6529 2c0a 2020 2020  able=True),.    
+00012750: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00012760: 7465 7874 5f64 6174 6122 2c20 5465 7874  text_data", Text
+00012770: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00012780: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00012790: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
+000127a0: 736e 2774 2073 7570 706f 7274 206e 6f6e  sn't support non
+000127b0: 2d61 7363 6969 2063 6861 7261 6374 6572  -ascii character
+000127c0: 7322 290a 2020 2020 6465 6620 7465 7374  s").    def test
+000127d0: 5f6c 6974 6572 616c 5f6e 6f6e 5f61 7363  _literal_non_asc
+000127e0: 6969 2873 656c 6629 3a0a 2020 2020 2020  ii(self):.      
+000127f0: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
+00012800: 6573 742e 6d61 726b 2e73 6b69 7028 224e  est.mark.skip("N
+00012810: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
+00012820: 5370 616e 6e65 7222 290a 2020 2020 6465  Spanner").    de
+00012830: 6620 7465 7374 5f74 6578 745f 726f 756e  f test_text_roun
+00012840: 6474 7269 7028 7365 6c66 2c20 636f 6e6e  dtrip(self, conn
+00012850: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
+00012860: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
+00012870: 7374 2e6d 6172 6b2e 736b 6970 2822 4e6f  st.mark.skip("No
+00012880: 7420 7375 7070 6f72 7465 6420 6279 2053  t supported by S
+00012890: 7061 6e6e 6572 2229 0a20 2020 2064 6566  panner").    def
+000128a0: 2074 6573 745f 7465 7874 5f65 6d70 7479   test_text_empty
+000128b0: 5f73 7472 696e 6773 2873 656c 662c 2063  _strings(self, c
+000128c0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+000128d0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+000128e0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+000128f0: 224e 6f74 2073 7570 706f 7274 6564 2062  "Not supported b
+00012900: 7920 5370 616e 6e65 7222 290a 2020 2020  y Spanner").    
+00012910: 6465 6620 7465 7374 5f74 6578 745f 6e75  def test_text_nu
+00012920: 6c6c 5f73 7472 696e 6773 2873 656c 662c  ll_strings(self,
+00012930: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
+00012940: 2020 2020 2020 7061 7373 0a0a 0a63 6c61        pass...cla
+00012950: 7373 204e 756d 6572 6963 5465 7374 285f  ss NumericTest(_
+00012960: 4e75 6d65 7269 6354 6573 7429 3a0a 2020  NumericTest):.  
+00012970: 2020 4074 6573 7469 6e67 2e66 6978 7475    @testing.fixtu
+00012980: 7265 0a20 2020 2064 6566 2064 6f5f 6e75  re.    def do_nu
+00012990: 6d65 7269 635f 7465 7374 2873 656c 662c  meric_test(self,
+000129a0: 206d 6574 6164 6174 612c 2063 6f6e 6e65   metadata, conne
+000129b0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+000129c0: 4074 6573 7469 6e67 2e65 6d69 7473 5f77  @testing.emits_w
+000129d0: 6172 6e69 6e67 2872 222e 2a64 6f65 7320  arning(r".*does 
+000129e0: 5c2a 6e6f 745c 2a20 7375 7070 6f72 7420  \*not\* support 
+000129f0: 4465 6369 6d61 6c20 6f62 6a65 6374 7320  Decimal objects 
+00012a00: 6e61 7469 7665 6c79 2229 0a20 2020 2020  natively").     
+00012a10: 2020 2064 6566 2072 756e 2874 7970 655f     def run(type_
+00012a20: 2c20 696e 7075 745f 2c20 6f75 7470 7574  , input_, output
+00012a30: 2c20 6669 6c74 6572 5f3d 4e6f 6e65 2c20  , filter_=None, 
+00012a40: 6368 6563 6b5f 7363 616c 653d 4661 6c73  check_scale=Fals
+00012a50: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00012a60: 7420 3d20 5461 626c 6528 0a20 2020 2020  t = Table(.     
+00012a70: 2020 2020 2020 2020 2020 2022 7422 2c0a             "t",.
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a90: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00012aa0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+00012ab0: 2822 7822 2c20 7479 7065 5f29 2c0a 2020  ("x", type_),.  
+00012ac0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00012ad0: 6c75 6d6e 2822 6964 222c 2049 6e74 6567  lumn("id", Integ
+00012ae0: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+00012af0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+00012b00: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00012b10: 2074 2e63 7265 6174 6528 636f 6e6e 6563   t.create(connec
+00012b20: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
+00012b30: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
+00012b40: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
+00012b50: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00012b60: 6e65 6374 696f 6e2e 6578 6563 7574 6528  nection.execute(
+00012b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b80: 2074 2e69 6e73 6572 7428 292c 205b 7b22   t.insert(), [{"
+00012b90: 7822 3a20 782c 2022 6964 223a 2069 7d20  x": x, "id": i} 
+00012ba0: 666f 7220 692c 2078 2069 6e20 656e 756d  for i, x in enum
+00012bb0: 6572 6174 6528 696e 7075 745f 295d 0a20  erate(input_)]. 
+00012bc0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00012bd0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00012be0: 203d 207b 726f 775b 305d 2066 6f72 2072   = {row[0] for r
+00012bf0: 6f77 2069 6e20 636f 6e6e 6563 7469 6f6e  ow in connection
+00012c00: 2e65 7865 6375 7465 2874 2e73 656c 6563  .execute(t.selec
+00012c10: 7428 2929 7d0a 2020 2020 2020 2020 2020  t())}.          
+00012c20: 2020 6f75 7470 7574 203d 2073 6574 286f    output = set(o
+00012c30: 7574 7075 7429 0a20 2020 2020 2020 2020  utput).         
+00012c40: 2020 2069 6620 6669 6c74 6572 5f3a 0a20     if filter_:. 
+00012c50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012c60: 6573 756c 7420 3d20 7365 7428 6669 6c74  esult = set(filt
+00012c70: 6572 5f28 7829 2066 6f72 2078 2069 6e20  er_(x) for x in 
+00012c80: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
+00012c90: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+00012ca0: 2073 6574 2866 696c 7465 725f 2878 2920   set(filter_(x) 
+00012cb0: 666f 7220 7820 696e 206f 7574 7075 7429  for x in output)
+00012cc0: 0a20 2020 2020 2020 2020 2020 2065 715f  .            eq_
+00012cd0: 2872 6573 756c 742c 206f 7574 7075 7429  (result, output)
+00012ce0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00012cf0: 6368 6563 6b5f 7363 616c 653a 0a20 2020  check_scale:.   
+00012d00: 2020 2020 2020 2020 2020 2020 2065 715f               eq_
+00012d10: 285b 7374 7228 7829 2066 6f72 2078 2069  ([str(x) for x i
+00012d20: 6e20 7265 7375 6c74 5d2c 205b 7374 7228  n result], [str(
+00012d30: 7829 2066 6f72 2078 2069 6e20 6f75 7470  x) for x in outp
+00012d40: 7574 5d29 0a0a 2020 2020 2020 2020 7265  ut])..        re
+00012d50: 7475 726e 2072 756e 0a0a 2020 2020 4065  turn run..    @e
+00012d60: 6d69 7473 5f77 6172 6e69 6e67 2872 222e  mits_warning(r".
+00012d70: 2a64 6f65 7320 5c2a 6e6f 745c 2a20 7375  *does \*not\* su
+00012d80: 7070 6f72 7420 4465 6369 6d61 6c20 6f62  pport Decimal ob
+00012d90: 6a65 6374 7320 6e61 7469 7665 6c79 2229  jects natively")
+00012da0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+00012db0: 6e64 6572 5f6c 6974 6572 616c 5f6e 756d  nder_literal_num
+00012dc0: 6572 6963 2873 656c 662c 206c 6974 6572  eric(self, liter
+00012dd0: 616c 5f72 6f75 6e64 5f74 7269 7029 3a0a  al_round_trip):.
+00012de0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012df0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+00012e00: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
+00012e10: 6c6f 7564 2053 7061 6e6e 6572 2073 7570  loud Spanner sup
+00012e20: 706f 7274 7320 7461 626c 6573 2077 6974  ports tables wit
+00012e30: 6820 616e 2065 6d70 7479 2070 7269 6d61  h an empty prima
+00012e40: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
+00012e50: 2020 2020 6f6e 6c79 2061 2073 696e 676c      only a singl
+00012e60: 6520 726f 7720 6361 6e20 6265 2069 6e73  e row can be ins
+00012e70: 6572 7465 6420 696e 746f 2073 7563 6820  erted into such 
+00012e80: 6120 7461 626c 6520 2d0a 2020 2020 2020  a table -.      
+00012e90: 2020 666f 6c6c 6f77 696e 6720 696e 7365    following inse
+00012ea0: 7274 696f 6e73 2077 696c 6c20 6661 696c  rtions will fail
+00012eb0: 2077 6974 6820 6052 6f77 205b 5d20 616c   with `Row [] al
+00012ec0: 7265 6164 7920 6578 6973 7473 222e 0a20  ready exists".. 
+00012ed0: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
+00012ee0: 6720 7468 6520 7465 7374 2074 6f20 6176  g the test to av
+00012ef0: 6f69 6420 7468 6520 7361 6d65 2066 6169  oid the same fai
+00012f00: 6c75 7265 2e0a 2020 2020 2020 2020 2222  lure..        ""
+00012f10: 220a 2020 2020 2020 2020 6c69 7465 7261  ".        litera
+00012f20: 6c5f 726f 756e 645f 7472 6970 280a 2020  l_round_trip(.  
+00012f30: 2020 2020 2020 2020 2020 4e75 6d65 7269            Numeri
+00012f40: 6328 7072 6563 6973 696f 6e3d 382c 2073  c(precision=8, s
+00012f50: 6361 6c65 3d34 292c 0a20 2020 2020 2020  cale=4),.       
+00012f60: 2020 2020 205b 6465 6369 6d61 6c2e 4465       [decimal.De
+00012f70: 6369 6d61 6c28 2231 352e 3735 3633 2229  cimal("15.7563")
+00012f80: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00012f90: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
+00012fa0: 2231 352e 3735 3633 2229 5d2c 0a20 2020  "15.7563")],.   
+00012fb0: 2020 2020 2029 0a0a 2020 2020 4065 6d69       )..    @emi
+00012fc0: 7473 5f77 6172 6e69 6e67 2872 222e 2a64  ts_warning(r".*d
+00012fd0: 6f65 7320 5c2a 6e6f 745c 2a20 7375 7070  oes \*not\* supp
+00012fe0: 6f72 7420 4465 6369 6d61 6c20 6f62 6a65  ort Decimal obje
+00012ff0: 6374 7320 6e61 7469 7665 6c79 2229 0a20  cts natively"). 
+00013000: 2020 2064 6566 2074 6573 745f 7265 6e64     def test_rend
+00013010: 6572 5f6c 6974 6572 616c 5f6e 756d 6572  er_literal_numer
+00013020: 6963 5f61 7366 6c6f 6174 2873 656c 662c  ic_asfloat(self,
+00013030: 206c 6974 6572 616c 5f72 6f75 6e64 5f74   literal_round_t
+00013040: 7269 7029 3a0a 2020 2020 2020 2020 2222  rip):.        ""
+00013050: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
+00013060: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
+00013070: 2020 2020 2043 6c6f 7564 2053 7061 6e6e       Cloud Spann
+00013080: 6572 2073 7570 706f 7274 7320 7461 626c  er supports tabl
+00013090: 6573 2077 6974 6820 616e 2065 6d70 7479  es with an empty
+000130a0: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
+000130b0: 740a 2020 2020 2020 2020 6f6e 6c79 2061  t.        only a
+000130c0: 2073 696e 676c 6520 726f 7720 6361 6e20   single row can 
+000130d0: 6265 2069 6e73 6572 7465 6420 696e 746f  be inserted into
+000130e0: 2073 7563 6820 6120 7461 626c 6520 2d0a   such a table -.
+000130f0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
+00013100: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
+00013110: 6c20 6661 696c 2077 6974 6820 6052 6f77  l fail with `Row
+00013120: 205b 5d20 616c 7265 6164 7920 6578 6973   [] already exis
+00013130: 7473 222e 0a20 2020 2020 2020 204f 7665  ts"..        Ove
+00013140: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
+00013150: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
+00013160: 6d65 2066 6169 6c75 7265 2e0a 2020 2020  me failure..    
+00013170: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013180: 6c69 7465 7261 6c5f 726f 756e 645f 7472  literal_round_tr
+00013190: 6970 280a 2020 2020 2020 2020 2020 2020  ip(.            
+000131a0: 4e75 6d65 7269 6328 7072 6563 6973 696f  Numeric(precisio
+000131b0: 6e3d 382c 2073 6361 6c65 3d34 2c20 6173  n=8, scale=4, as
+000131c0: 6465 6369 6d61 6c3d 4661 6c73 6529 2c0a  decimal=False),.
+000131d0: 2020 2020 2020 2020 2020 2020 5b64 6563              [dec
+000131e0: 696d 616c 2e44 6563 696d 616c 2822 3135  imal.Decimal("15
+000131f0: 2e37 3536 3322 295d 2c0a 2020 2020 2020  .7563")],.      
+00013200: 2020 2020 2020 5b31 352e 3735 3633 5d2c        [15.7563],
+00013210: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00013220: 6465 6620 7465 7374 5f72 656e 6465 725f  def test_render_
+00013230: 6c69 7465 7261 6c5f 666c 6f61 7428 7365  literal_float(se
+00013240: 6c66 2c20 6c69 7465 7261 6c5f 726f 756e  lf, literal_roun
+00013250: 645f 7472 6970 293a 0a20 2020 2020 2020  d_trip):.       
+00013260: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
+00013270: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+00013280: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
+00013290: 616e 6e65 7220 7375 7070 6f72 7473 2074  anner supports t
+000132a0: 6162 6c65 7320 7769 7468 2061 6e20 656d  ables with an em
+000132b0: 7074 7920 7072 696d 6172 7920 6b65 792c  pty primary key,
+000132c0: 2062 7574 0a20 2020 2020 2020 206f 6e6c   but.        onl
+000132d0: 7920 6120 7369 6e67 6c65 2072 6f77 2063  y a single row c
+000132e0: 616e 2062 6520 696e 7365 7274 6564 2069  an be inserted i
+000132f0: 6e74 6f20 7375 6368 2061 2074 6162 6c65  nto such a table
+00013300: 202d 0a20 2020 2020 2020 2066 6f6c 6c6f   -.        follo
+00013310: 7769 6e67 2069 6e73 6572 7469 6f6e 7320  wing insertions 
+00013320: 7769 6c6c 2066 6169 6c20 7769 7468 2060  will fail with `
+00013330: 526f 7720 5b5d 2061 6c72 6561 6479 2065  Row [] already e
+00013340: 7869 7374 7322 2e0a 2020 2020 2020 2020  xists"..        
+00013350: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
+00013360: 6573 7420 746f 2061 766f 6964 2074 6865  est to avoid the
+00013370: 2073 616d 6520 6661 696c 7572 652e 0a20   same failure.. 
+00013380: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013390: 2020 206c 6974 6572 616c 5f72 6f75 6e64     literal_round
+000133a0: 5f74 7269 7028 0a20 2020 2020 2020 2020  _trip(.         
+000133b0: 2020 2046 6c6f 6174 2834 292c 0a20 2020     Float(4),.   
+000133c0: 2020 2020 2020 2020 205b 6465 6369 6d61           [decima
+000133d0: 6c2e 4465 6369 6d61 6c28 2231 352e 3735  l.Decimal("15.75
+000133e0: 3633 2229 5d2c 0a20 2020 2020 2020 2020  63")],.         
+000133f0: 2020 205b 3135 2e37 3536 335d 2c0a 2020     [15.7563],.  
+00013400: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00013410: 5f3d 6c61 6d62 6461 206e 3a20 6e20 6973  _=lambda n: n is
+00013420: 206e 6f74 204e 6f6e 6520 616e 6420 726f   not None and ro
+00013430: 756e 6428 6e2c 2035 2920 6f72 204e 6f6e  und(n, 5) or Non
+00013440: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+00013450: 2020 4072 6571 7569 7265 732e 7072 6563    @requires.prec
+00013460: 6973 696f 6e5f 6765 6e65 7269 635f 666c  ision_generic_fl
+00013470: 6f61 745f 7479 7065 0a20 2020 2064 6566  oat_type.    def
+00013480: 2074 6573 745f 666c 6f61 745f 6375 7374   test_float_cust
+00013490: 6f6d 5f73 6361 6c65 2873 656c 662c 2064  om_scale(self, d
+000134a0: 6f5f 6e75 6d65 7269 635f 7465 7374 293a  o_numeric_test):
+000134b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000134c0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
+000134d0: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
+000134e0: 436c 6f75 6420 5370 616e 6e65 7220 7375  Cloud Spanner su
+000134f0: 7070 6f72 7473 2074 6162 6c65 7320 7769  pports tables wi
+00013500: 7468 2061 6e20 656d 7074 7920 7072 696d  th an empty prim
+00013510: 6172 7920 6b65 792c 2062 7574 0a20 2020  ary key, but.   
+00013520: 2020 2020 206f 6e6c 7920 6120 7369 6e67       only a sing
+00013530: 6c65 2072 6f77 2063 616e 2062 6520 696e  le row can be in
+00013540: 7365 7274 6564 2069 6e74 6f20 7375 6368  serted into such
+00013550: 2061 2074 6162 6c65 202d 0a20 2020 2020   a table -.     
+00013560: 2020 2066 6f6c 6c6f 7769 6e67 2069 6e73     following ins
+00013570: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
+00013580: 6c20 7769 7468 2060 526f 7720 5b5d 2061  l with `Row [] a
+00013590: 6c72 6561 6479 2065 7869 7374 7322 2e0a  lready exists"..
+000135a0: 2020 2020 2020 2020 4f76 6572 7269 6469          Overridi
+000135b0: 6e67 2074 6865 2074 6573 7420 746f 2061  ng the test to a
+000135c0: 766f 6964 2074 6865 2073 616d 6520 6661  void the same fa
+000135d0: 696c 7572 652e 0a20 2020 2020 2020 2022  ilure..        "
+000135e0: 2222 0a20 2020 2020 2020 2064 6f5f 6e75  "".        do_nu
+000135f0: 6d65 7269 635f 7465 7374 280a 2020 2020  meric_test(.    
+00013600: 2020 2020 2020 2020 466c 6f61 7428 4e6f          Float(No
+00013610: 6e65 2c20 6465 6369 6d61 6c5f 7265 7475  ne, decimal_retu
+00013620: 726e 5f73 6361 6c65 3d37 2c20 6173 6465  rn_scale=7, asde
+00013630: 6369 6d61 6c3d 5472 7565 292c 0a20 2020  cimal=True),.   
+00013640: 2020 2020 2020 2020 205b 6465 6369 6d61           [decima
+00013650: 6c2e 4465 6369 6d61 6c28 2231 352e 3735  l.Decimal("15.75
+00013660: 3633 3832 3722 292c 2064 6563 696d 616c  63827"), decimal
+00013670: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
+00013680: 3338 3237 2229 5d2c 0a20 2020 2020 2020  3827")],.       
+00013690: 2020 2020 205b 6465 6369 6d61 6c2e 4465       [decimal.De
+000136a0: 6369 6d61 6c28 2231 352e 3735 3633 3832  cimal("15.756382
+000136b0: 3722 295d 2c0a 2020 2020 2020 2020 2020  7")],.          
+000136c0: 2020 6368 6563 6b5f 7363 616c 653d 5472    check_scale=Tr
+000136d0: 7565 2c0a 2020 2020 2020 2020 290a 0a20  ue,.        ).. 
+000136e0: 2020 2064 6566 2074 6573 745f 6e75 6d65     def test_nume
+000136f0: 7269 635f 6173 5f64 6563 696d 616c 2873  ric_as_decimal(s
+00013700: 656c 662c 2064 6f5f 6e75 6d65 7269 635f  elf, do_numeric_
+00013710: 7465 7374 293a 0a20 2020 2020 2020 2022  test):.        "
+00013720: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
+00013730: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
+00013740: 2020 2020 2020 5370 616e 6e65 7220 7468        Spanner th
+00013750: 726f 7773 2061 6e20 6572 726f 7220 3430  rows an error 40
+00013760: 3020 5661 6c75 6520 6861 7320 7479 7065  0 Value has type
+00013770: 2046 4c4f 4154 3634 2077 6869 6368 2063   FLOAT64 which c
+00013780: 616e 6e6f 7420 6265 0a20 2020 2020 2020  annot be.       
+00013790: 2069 6e73 6572 7465 6420 696e 746f 2063   inserted into c
+000137a0: 6f6c 756d 6e20 782c 2077 6869 6368 2068  olumn x, which h
+000137b0: 6173 2074 7970 6520 4e55 4d45 5249 4320  as type NUMERIC 
+000137c0: 666f 7220 7661 6c75 6520 3135 2e37 3536  for value 15.756
+000137d0: 332e 0a20 2020 2020 2020 204f 7665 7272  3..        Overr
+000137e0: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
+000137f0: 6f20 7265 6d6f 7665 2074 6865 2066 6169  o remove the fai
+00013800: 6c75 7265 2063 6173 652e 0a20 2020 2020  lure case..     
+00013810: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+00013820: 6f5f 6e75 6d65 7269 635f 7465 7374 280a  o_numeric_test(.
+00013830: 2020 2020 2020 2020 2020 2020 4e75 6d65              Nume
+00013840: 7269 6328 7072 6563 6973 696f 6e3d 382c  ric(precision=8,
+00013850: 2073 6361 6c65 3d34 292c 0a20 2020 2020   scale=4),.     
+00013860: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
+00013870: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+00013880: 2229 2c20 6465 6369 6d61 6c2e 4465 6369  "), decimal.Deci
+00013890: 6d61 6c28 2231 352e 3735 3633 2229 5d2c  mal("15.7563")],
+000138a0: 0a20 2020 2020 2020 2020 2020 205b 6465  .            [de
+000138b0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
+000138c0: 352e 3735 3633 2229 5d2c 0a20 2020 2020  5.7563")],.     
+000138d0: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
+000138e0: 7374 5f6e 756d 6572 6963 5f61 735f 666c  st_numeric_as_fl
+000138f0: 6f61 7428 7365 6c66 2c20 646f 5f6e 756d  oat(self, do_num
+00013900: 6572 6963 5f74 6573 7429 3a0a 2020 2020  eric_test):.    
+00013910: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013920: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+00013930: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
+00013940: 6572 2074 6872 6f77 7320 616e 2065 7272  er throws an err
+00013950: 6f72 2034 3030 2056 616c 7565 2068 6173  or 400 Value has
+00013960: 2074 7970 6520 464c 4f41 5436 3420 7768   type FLOAT64 wh
+00013970: 6963 6820 6361 6e6e 6f74 2062 650a 2020  ich cannot be.  
+00013980: 2020 2020 2020 696e 7365 7274 6564 2069        inserted i
+00013990: 6e74 6f20 636f 6c75 6d6e 2078 2c20 7768  nto column x, wh
+000139a0: 6963 6820 6861 7320 7479 7065 204e 554d  ich has type NUM
+000139b0: 4552 4943 2066 6f72 2076 616c 7565 2031  ERIC for value 1
+000139c0: 352e 3735 3633 2e0a 2020 2020 2020 2020  5.7563..        
+000139d0: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
+000139e0: 6573 7420 746f 2072 656d 6f76 6520 7468  est to remove th
+000139f0: 6520 6661 696c 7572 6520 6361 7365 2e0a  e failure case..
+00013a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013a10: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
+00013a20: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+00013a30: 204e 756d 6572 6963 2870 7265 6369 7369   Numeric(precisi
+00013a40: 6f6e 3d38 2c20 7363 616c 653d 342c 2061  on=8, scale=4, a
+00013a50: 7364 6563 696d 616c 3d46 616c 7365 292c  sdecimal=False),
+00013a60: 0a20 2020 2020 2020 2020 2020 205b 6465  .            [de
+00013a70: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
+00013a80: 352e 3735 3633 2229 2c20 6465 6369 6d61  5.7563"), decima
+00013a90: 6c2e 4465 6369 6d61 6c28 2231 352e 3735  l.Decimal("15.75
+00013aa0: 3633 2229 5d2c 0a20 2020 2020 2020 2020  63")],.         
+00013ab0: 2020 205b 3135 2e37 3536 335d 2c0a 2020     [15.7563],.  
+00013ac0: 2020 2020 2020 290a 0a20 2020 2040 7265        )..    @re
+00013ad0: 7175 6972 6573 2e66 6c6f 6174 735f 746f  quires.floats_to
+00013ae0: 5f66 6f75 725f 6465 6369 6d61 6c73 0a20  _four_decimals. 
+00013af0: 2020 2064 6566 2074 6573 745f 666c 6f61     def test_floa
+00013b00: 745f 6173 5f64 6563 696d 616c 2873 656c  t_as_decimal(sel
+00013b10: 662c 2064 6f5f 6e75 6d65 7269 635f 7465  f, do_numeric_te
+00013b20: 7374 293a 0a20 2020 2020 2020 2022 2222  st):.        """
+00013b30: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+00013b40: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
+00013b50: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
+00013b60: 7220 7375 7070 6f72 7473 2074 6162 6c65  r supports table
+00013b70: 7320 7769 7468 2061 6e20 656d 7074 7920  s with an empty 
+00013b80: 7072 696d 6172 7920 6b65 792c 2062 7574  primary key, but
+00013b90: 0a20 2020 2020 2020 206f 6e6c 7920 6120  .        only a 
+00013ba0: 7369 6e67 6c65 2072 6f77 2063 616e 2062  single row can b
+00013bb0: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
+00013bc0: 7375 6368 2061 2074 6162 6c65 202d 0a20  such a table -. 
+00013bd0: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
+00013be0: 2069 6e73 6572 7469 6f6e 7320 7769 6c6c   insertions will
+00013bf0: 2066 6169 6c20 7769 7468 2060 526f 7720   fail with `Row 
+00013c00: 5b5d 2061 6c72 6561 6479 2065 7869 7374  [] already exist
+00013c10: 7322 2e0a 2020 2020 2020 2020 4f76 6572  s"..        Over
+00013c20: 7269 6469 6e67 2074 6865 2074 6573 7420  riding the test 
+00013c30: 746f 2061 766f 6964 2074 6865 2073 616d  to avoid the sam
+00013c40: 6520 6661 696c 7572 652e 0a20 2020 2020  e failure..     
+00013c50: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+00013c60: 6f5f 6e75 6d65 7269 635f 7465 7374 280a  o_numeric_test(.
+00013c70: 2020 2020 2020 2020 2020 2020 466c 6f61              Floa
+00013c80: 7428 7072 6563 6973 696f 6e3d 382c 2061  t(precision=8, a
+00013c90: 7364 6563 696d 616c 3d54 7275 6529 2c0a  sdecimal=True),.
+00013ca0: 2020 2020 2020 2020 2020 2020 5b64 6563              [dec
+00013cb0: 696d 616c 2e44 6563 696d 616c 2822 3135  imal.Decimal("15
+00013cc0: 2e37 3536 3322 292c 2064 6563 696d 616c  .7563"), decimal
+00013cd0: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
+00013ce0: 3322 292c 204e 6f6e 655d 2c0a 2020 2020  3"), None],.    
+00013cf0: 2020 2020 2020 2020 5b64 6563 696d 616c          [decimal
+00013d00: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
+00013d10: 3322 292c 204e 6f6e 655d 2c0a 2020 2020  3"), None],.    
+00013d20: 2020 2020 2020 2020 6669 6c74 6572 5f3d          filter_=
+00013d30: 6c61 6d62 6461 206e 3a20 6e20 6973 206e  lambda n: n is n
+00013d40: 6f74 204e 6f6e 6520 616e 6420 726f 756e  ot None and roun
+00013d50: 6428 6e2c 2034 2920 6f72 204e 6f6e 652c  d(n, 4) or None,
+00013d60: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00013d70: 6465 6620 7465 7374 5f66 6c6f 6174 5f61  def test_float_a
+00013d80: 735f 666c 6f61 7428 7365 6c66 2c20 646f  s_float(self, do
+00013d90: 5f6e 756d 6572 6963 5f74 6573 7429 3a0a  _numeric_test):.
+00013da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013db0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+00013dc0: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
+00013dd0: 6c6f 7564 2053 7061 6e6e 6572 2073 7570  loud Spanner sup
+00013de0: 706f 7274 7320 7461 626c 6573 2077 6974  ports tables wit
+00013df0: 6820 616e 2065 6d70 7479 2070 7269 6d61  h an empty prima
+00013e00: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
+00013e10: 2020 2020 6f6e 6c79 2061 2073 696e 676c      only a singl
+00013e20: 6520 726f 7720 6361 6e20 6265 2069 6e73  e row can be ins
+00013e30: 6572 7465 6420 696e 746f 2073 7563 6820  erted into such 
+00013e40: 6120 7461 626c 6520 2d0a 2020 2020 2020  a table -.      
+00013e50: 2020 666f 6c6c 6f77 696e 6720 696e 7365    following inse
+00013e60: 7274 696f 6e73 2077 696c 6c20 6661 696c  rtions will fail
+00013e70: 2077 6974 6820 6052 6f77 205b 5d20 616c   with `Row [] al
+00013e80: 7265 6164 7920 6578 6973 7473 222e 0a20  ready exists".. 
+00013e90: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
+00013ea0: 6720 7468 6520 7465 7374 2074 6f20 6176  g the test to av
+00013eb0: 6f69 6420 7468 6520 7361 6d65 2066 6169  oid the same fai
+00013ec0: 6c75 7265 2e0a 2020 2020 2020 2020 2222  lure..        ""
+00013ed0: 220a 2020 2020 2020 2020 646f 5f6e 756d  ".        do_num
+00013ee0: 6572 6963 5f74 6573 7428 0a20 2020 2020  eric_test(.     
+00013ef0: 2020 2020 2020 2046 6c6f 6174 2870 7265         Float(pre
+00013f00: 6369 7369 6f6e 3d38 292c 0a20 2020 2020  cision=8),.     
+00013f10: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
+00013f20: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+00013f30: 2229 2c20 6465 6369 6d61 6c2e 4465 6369  "), decimal.Deci
+00013f40: 6d61 6c28 2231 352e 3735 3633 2229 5d2c  mal("15.7563")],
+00013f50: 0a20 2020 2020 2020 2020 2020 205b 3135  .            [15
+00013f60: 2e37 3536 335d 2c0a 2020 2020 2020 2020  .7563],.        
+00013f70: 2020 2020 6669 6c74 6572 5f3d 6c61 6d62      filter_=lamb
+00013f80: 6461 206e 3a20 6e20 6973 206e 6f74 204e  da n: n is not N
+00013f90: 6f6e 6520 616e 6420 726f 756e 6428 6e2c  one and round(n,
+00013fa0: 2035 2920 6f72 204e 6f6e 652c 0a20 2020   5) or None,.   
+00013fb0: 2020 2020 2029 0a0a 2020 2020 4072 6571       )..    @req
+00013fc0: 7569 7265 732e 7072 6563 6973 696f 6e5f  uires.precision_
+00013fd0: 6e75 6d65 7269 6373 5f67 656e 6572 616c  numerics_general
+00013fe0: 0a20 2020 2064 6566 2074 6573 745f 7072  .    def test_pr
+00013ff0: 6563 6973 696f 6e5f 6465 6369 6d61 6c28  ecision_decimal(
+00014000: 7365 6c66 2c20 646f 5f6e 756d 6572 6963  self, do_numeric
+00014010: 5f74 6573 7429 3a0a 2020 2020 2020 2020  _test):.        
+00014020: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
+00014030: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+00014040: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
+00014050: 6e6e 6572 2073 7570 706f 7274 7320 7461  nner supports ta
+00014060: 626c 6573 2077 6974 6820 616e 2065 6d70  bles with an emp
+00014070: 7479 2070 7269 6d61 7279 206b 6579 2c20  ty primary key, 
+00014080: 6275 740a 2020 2020 2020 2020 6f6e 6c79  but.        only
+00014090: 2061 2073 696e 676c 6520 726f 7720 6361   a single row ca
+000140a0: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
+000140b0: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
+000140c0: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
+000140d0: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
+000140e0: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
+000140f0: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
+00014100: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
+00014110: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+00014120: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
+00014130: 7361 6d65 2066 6169 6c75 7265 2e0a 0a20  same failure... 
+00014140: 2020 2020 2020 2052 656d 6f76 6520 616e         Remove an
+00014150: 2065 7874 7261 2064 6967 6974 7320 6166   extra digits af
+00014160: 7465 7220 6465 6369 6d61 6c20 706f 696e  ter decimal poin
+00014170: 7420 6173 2063 6c6f 7564 2073 7061 6e6e  t as cloud spann
+00014180: 6572 2069 730a 2020 2020 2020 2020 6361  er is.        ca
+00014190: 7061 626c 6520 6f66 2072 6570 7265 7365  pable of represe
+000141a0: 6e74 696e 6720 616e 2065 7861 6374 206e  nting an exact n
+000141b0: 756d 6572 6963 2076 616c 7565 2077 6974  umeric value wit
+000141c0: 6820 6120 7072 6563 6973 696f 6e0a 2020  h a precision.  
+000141d0: 2020 2020 2020 6f66 2033 3820 616e 6420        of 38 and 
+000141e0: 7363 616c 6520 6f66 2039 2e0a 2020 2020  scale of 9..    
+000141f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014200: 6e75 6d62 6572 7320 3d20 7365 7428 0a20  numbers = set(. 
+00014210: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00014220: 2020 2020 2020 2020 2020 2020 2064 6563               dec
+00014230: 696d 616c 2e44 6563 696d 616c 2822 3534  imal.Decimal("54
+00014240: 2e32 3436 3435 3136 3530 2229 2c0a 2020  .246451650"),.  
+00014250: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00014260: 6369 6d61 6c2e 4465 6369 6d61 6c28 2230  cimal.Decimal("0
+00014270: 2e30 3034 3335 3422 292c 0a20 2020 2020  .004354"),.     
+00014280: 2020 2020 2020 2020 2020 2064 6563 696d             decim
+00014290: 616c 2e44 6563 696d 616c 2822 3930 302e  al.Decimal("900.
+000142a0: 3022 292c 0a20 2020 2020 2020 2020 2020  0"),.           
+000142b0: 205d 0a20 2020 2020 2020 2029 0a20 2020   ].        ).   
+000142c0: 2020 2020 2064 6f5f 6e75 6d65 7269 635f       do_numeric_
+000142d0: 7465 7374 284e 756d 6572 6963 2870 7265  test(Numeric(pre
+000142e0: 6369 7369 6f6e 3d31 382c 2073 6361 6c65  cision=18, scale
+000142f0: 3d39 292c 206e 756d 6265 7273 2c20 6e75  =9), numbers, nu
+00014300: 6d62 6572 7329 0a0a 2020 2020 4074 6573  mbers)..    @tes
+00014310: 7469 6e67 2e72 6571 7569 7265 732e 7072  ting.requires.pr
+00014320: 6563 6973 696f 6e5f 6e75 6d65 7269 6373  ecision_numerics
+00014330: 5f65 6e6f 7461 7469 6f6e 5f6c 6172 6765  _enotation_large
+00014340: 0a20 2020 2064 6566 2074 6573 745f 656e  .    def test_en
+00014350: 6f74 6174 696f 6e5f 6465 6369 6d61 6c5f  otation_decimal_
+00014360: 6c61 7267 6528 7365 6c66 2c20 646f 5f6e  large(self, do_n
+00014370: 756d 6572 6963 5f74 6573 7429 3a0a 2020  umeric_test):.  
+00014380: 2020 2020 2020 2222 2274 6573 7420 6578        """test ex
+00014390: 6365 6564 696e 676c 7920 6c61 7267 6520  ceedingly large 
+000143a0: 6465 6369 6d61 6c73 2e0a 0a20 2020 2020  decimals...     
+000143b0: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+000143c0: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
+000143d0: 6f75 6420 5370 616e 6e65 7220 7375 7070  oud Spanner supp
+000143e0: 6f72 7473 2074 6162 6c65 7320 7769 7468  orts tables with
+000143f0: 2061 6e20 656d 7074 7920 7072 696d 6172   an empty primar
+00014400: 7920 6b65 792c 2062 7574 0a20 2020 2020  y key, but.     
+00014410: 2020 206f 6e6c 7920 6120 7369 6e67 6c65     only a single
+00014420: 2072 6f77 2063 616e 2062 6520 696e 7365   row can be inse
+00014430: 7274 6564 2069 6e74 6f20 7375 6368 2061  rted into such a
+00014440: 2074 6162 6c65 202d 0a20 2020 2020 2020   table -.       
+00014450: 2066 6f6c 6c6f 7769 6e67 2069 6e73 6572   following inser
+00014460: 7469 6f6e 7320 7769 6c6c 2066 6169 6c20  tions will fail 
+00014470: 7769 7468 2060 526f 7720 5b5d 2061 6c72  with `Row [] alr
+00014480: 6561 6479 2065 7869 7374 7322 2e0a 2020  eady exists"..  
+00014490: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
+000144a0: 2074 6865 2074 6573 7420 746f 2061 766f   the test to avo
+000144b0: 6964 2074 6865 2073 616d 6520 6661 696c  id the same fail
+000144c0: 7572 652e 0a20 2020 2020 2020 2022 2222  ure..        """
+000144d0: 0a20 2020 2020 2020 206e 756d 6265 7273  .        numbers
+000144e0: 203d 2073 6574 280a 2020 2020 2020 2020   = set(.        
+000144f0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00014500: 2020 2020 2020 6465 6369 6d61 6c2e 4465        decimal.De
+00014510: 6369 6d61 6c28 2234 452b 3822 292c 0a20  cimal("4E+8"),. 
+00014520: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00014530: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+00014540: 3537 3438 452b 3135 2229 2c0a 2020 2020  5748E+15"),.    
+00014550: 2020 2020 2020 2020 2020 2020 6465 6369              deci
+00014560: 6d61 6c2e 4465 6369 6d61 6c28 2231 2e35  mal.Decimal("1.5
+00014570: 3231 452b 3135 2229 2c0a 2020 2020 2020  21E+15"),.      
+00014580: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
+00014590: 6c2e 4465 6369 6d61 6c28 2230 3030 3030  l.Decimal("00000
+000145a0: 3030 3030 2e31 452b 3922 292c 0a20 2020  0000.1E+9"),.   
+000145b0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+000145c0: 2020 2029 0a20 2020 2020 2020 2064 6f5f     ).        do_
+000145d0: 6e75 6d65 7269 635f 7465 7374 284e 756d  numeric_test(Num
+000145e0: 6572 6963 2870 7265 6369 7369 6f6e 3d32  eric(precision=2
+000145f0: 352c 2073 6361 6c65 3d32 292c 206e 756d  5, scale=2), num
+00014600: 6265 7273 2c20 6e75 6d62 6572 7329 0a0a  bers, numbers)..
+00014610: 2020 2020 4074 6573 7469 6e67 2e72 6571      @testing.req
+00014620: 7569 7265 732e 7072 6563 6973 696f 6e5f  uires.precision_
+00014630: 6e75 6d65 7269 6373 5f65 6e6f 7461 7469  numerics_enotati
+00014640: 6f6e 5f6c 6172 6765 0a20 2020 2064 6566  on_large.    def
+00014650: 2074 6573 745f 656e 6f74 6174 696f 6e5f   test_enotation_
+00014660: 6465 6369 6d61 6c28 7365 6c66 2c20 646f  decimal(self, do
+00014670: 5f6e 756d 6572 6963 5f74 6573 7429 3a0a  _numeric_test):.
+00014680: 2020 2020 2020 2020 2222 2274 6573 7420          """test 
+00014690: 6578 6365 6564 696e 676c 7920 736d 616c  exceedingly smal
+000146a0: 6c20 6465 6369 6d61 6c73 2e0a 0a20 2020  l decimals...   
+000146b0: 2020 2020 2044 6563 696d 616c 2072 6570       Decimal rep
+000146c0: 6f72 7473 2076 616c 7565 7320 7769 7468  orts values with
+000146d0: 2045 206e 6f74 6174 696f 6e20 7768 656e   E notation when
+000146e0: 2074 6865 2065 7870 6f6e 656e 740a 2020   the exponent.  
+000146f0: 2020 2020 2020 6973 2067 7265 6174 6572        is greater
+00014700: 2074 6861 6e20 362e 0a0a 2020 2020 2020   than 6...      
+00014710: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+00014720: 4445 3a0a 0a20 2020 2020 2020 2052 656d  DE:..        Rem
+00014730: 6f76 6520 6578 7472 6120 6469 6769 7473  ove extra digits
+00014740: 2061 6674 6572 2064 6563 696d 616c 2070   after decimal p
+00014750: 6f69 6e74 2061 7320 436c 6f75 6420 5370  oint as Cloud Sp
+00014760: 616e 6e65 7220 6973 0a20 2020 2020 2020  anner is.       
+00014770: 2063 6170 6162 6c65 206f 6620 7265 7072   capable of repr
+00014780: 6573 656e 7469 6e67 2061 6e20 6578 6163  esenting an exac
+00014790: 7420 6e75 6d65 7269 6320 7661 6c75 6520  t numeric value 
+000147a0: 7769 7468 2061 2070 7265 6369 7369 6f6e  with a precision
+000147b0: 0a20 2020 2020 2020 206f 6620 3338 2061  .        of 38 a
+000147c0: 6e64 2073 6361 6c65 206f 6620 392e 0a20  nd scale of 9.. 
+000147d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000147e0: 2020 206e 756d 6265 7273 203d 2073 6574     numbers = set
+000147f0: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
+00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014810: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
+00014820: 2231 452d 3222 292c 0a20 2020 2020 2020  "1E-2"),.       
+00014830: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+00014840: 2e44 6563 696d 616c 2822 3145 2d33 2229  .Decimal("1E-3")
+00014850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014860: 2020 6465 6369 6d61 6c2e 4465 6369 6d61    decimal.Decima
+00014870: 6c28 2231 452d 3422 292c 0a20 2020 2020  l("1E-4"),.     
+00014880: 2020 2020 2020 2020 2020 2064 6563 696d             decim
+00014890: 616c 2e44 6563 696d 616c 2822 3145 2d35  al.Decimal("1E-5
+000148a0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+000148b0: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
+000148c0: 6d61 6c28 2231 452d 3622 292c 0a20 2020  mal("1E-6"),.   
+000148d0: 2020 2020 2020 2020 2020 2020 2064 6563               dec
+000148e0: 696d 616c 2e44 6563 696d 616c 2822 3145  imal.Decimal("1E
+000148f0: 2d37 2229 2c0a 2020 2020 2020 2020 2020  -7"),.          
+00014900: 2020 2020 2020 6465 6369 6d61 6c2e 4465        decimal.De
+00014910: 6369 6d61 6c28 2231 452d 3822 292c 0a20  cimal("1E-8"),. 
+00014920: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00014930: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+00014940: 302e 3130 3539 3430 3639 3622 292c 0a20  0.105940696"),. 
+00014950: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00014960: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+00014970: 302e 3030 3539 3430 3639 3622 292c 0a20  0.005940696"),. 
+00014980: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00014990: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+000149a0: 302e 3030 3030 3030 3639 3622 292c 0a20  0.000000696"),. 
+000149b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000149c0: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+000149d0: 302e 3730 3030 3030 3639 3622 292c 0a20  0.700000696"),. 
+000149e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000149f0: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
+00014a00: 3639 3645 2d39 2229 2c0a 2020 2020 2020  696E-9"),.      
+00014a10: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00014a20: 290a 2020 2020 2020 2020 646f 5f6e 756d  ).        do_num
+00014a30: 6572 6963 5f74 6573 7428 4e75 6d65 7269  eric_test(Numeri
+00014a40: 6328 7072 6563 6973 696f 6e3d 3338 2c20  c(precision=38, 
+00014a50: 7363 616c 653d 3929 2c20 6e75 6d62 6572  scale=9), number
+00014a60: 732c 206e 756d 6265 7273 290a 0a0a 636c  s, numbers)...cl
+00014a70: 6173 7320 4c69 6b65 4675 6e63 7469 6f6e  ass LikeFunction
+00014a80: 7354 6573 7428 5f4c 696b 6546 756e 6374  sTest(_LikeFunct
+00014a90: 696f 6e73 5465 7374 293a 0a20 2020 2040  ionsTest):.    @
+00014aa0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+00014ab0: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
+00014ac0: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
+00014ad0: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
+00014ae0: 2020 2064 6566 2074 6573 745f 636f 6e74     def test_cont
+00014af0: 6169 6e73 5f61 7574 6f65 7363 6170 6528  ains_autoescape(
+00014b00: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00014b10: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+00014b20: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+00014b30: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+00014b40: 6f72 7420 4c49 4b45 2045 5343 4150 4520  ort LIKE ESCAPE 
+00014b50: 636c 6175 7365 2229 0a20 2020 2064 6566  clause").    def
+00014b60: 2074 6573 745f 636f 6e74 6169 6e73 5f61   test_contains_a
+00014b70: 7574 6f65 7363 6170 655f 6573 6361 7065  utoescape_escape
+00014b80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00014b90: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+00014ba0: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+00014bb0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+00014bc0: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
+00014bd0: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
+00014be0: 6620 7465 7374 5f63 6f6e 7461 696e 735f  f test_contains_
+00014bf0: 6573 6361 7065 2873 656c 6629 3a0a 2020  escape(self):.  
+00014c00: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00014c10: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00014c20: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+00014c30: 2774 2073 7570 706f 7274 204c 494b 4520  't support LIKE 
+00014c40: 4553 4341 5045 2063 6c61 7573 6522 290a  ESCAPE clause").
+00014c50: 2020 2020 6465 6620 7465 7374 5f65 6e64      def test_end
+00014c60: 7377 6974 685f 6175 746f 6573 6361 7065  swith_autoescape
+00014c70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00014c80: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+00014c90: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+00014ca0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+00014cb0: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
+00014cc0: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
+00014cd0: 6620 7465 7374 5f65 6e64 7377 6974 685f  f test_endswith_
+00014ce0: 6573 6361 7065 2873 656c 6629 3a0a 2020  escape(self):.  
+00014cf0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00014d00: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00014d10: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+00014d20: 2774 2073 7570 706f 7274 204c 494b 4520  't support LIKE 
+00014d30: 4553 4341 5045 2063 6c61 7573 6522 290a  ESCAPE clause").
+00014d40: 2020 2020 6465 6620 7465 7374 5f65 6e64      def test_end
+00014d50: 7377 6974 685f 6175 746f 6573 6361 7065  swith_autoescape
+00014d60: 5f65 7363 6170 6528 7365 6c66 293a 0a20  _escape(self):. 
+00014d70: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00014d80: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+00014d90: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
+00014da0: 6e27 7420 7375 7070 6f72 7420 4c49 4b45  n't support LIKE
+00014db0: 2045 5343 4150 4520 636c 6175 7365 2229   ESCAPE clause")
+00014dc0: 0a20 2020 2064 6566 2074 6573 745f 7374  .    def test_st
+00014dd0: 6172 7473 7769 7468 5f61 7574 6f65 7363  artswith_autoesc
+00014de0: 6170 6528 7365 6c66 293a 0a20 2020 2020  ape(self):.     
+00014df0: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
+00014e00: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
+00014e10: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
+00014e20: 7375 7070 6f72 7420 4c49 4b45 2045 5343  support LIKE ESC
+00014e30: 4150 4520 636c 6175 7365 2229 0a20 2020  APE clause").   
+00014e40: 2064 6566 2074 6573 745f 7374 6172 7473   def test_starts
+00014e50: 7769 7468 5f65 7363 6170 6528 7365 6c66  with_escape(self
+00014e60: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00014e70: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00014e80: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
+00014e90: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+00014ea0: 4c49 4b45 2045 5343 4150 4520 636c 6175  LIKE ESCAPE clau
+00014eb0: 7365 2229 0a20 2020 2064 6566 2074 6573  se").    def tes
+00014ec0: 745f 7374 6172 7473 7769 7468 5f61 7574  t_startswith_aut
+00014ed0: 6f65 7363 6170 655f 6573 6361 7065 2873  oescape_escape(s
+00014ee0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00014ef0: 7373 0a0a 2020 2020 6465 6620 7465 7374  ss..    def test
+00014f00: 5f65 7363 6170 655f 6b65 7977 6f72 645f  _escape_keyword_
+00014f10: 7261 6973 6573 2873 656c 6629 3a0a 2020  raises(self):.  
+00014f20: 2020 2020 2020 2222 2243 6865 636b 2074        """Check t
+00014f30: 6861 7420 4553 4341 5045 206b 6579 776f  hat ESCAPE keywo
+00014f40: 7264 2063 6175 7365 7320 616e 2065 7863  rd causes an exc
+00014f50: 6570 7469 6f6e 2077 6865 6e20 7573 6564  eption when used
+00014f60: 2e22 2222 0a20 2020 2020 2020 2077 6974  .""".        wit
+00014f70: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
+00014f80: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00014f90: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00014fa0: 2020 636f 6c20 3d20 7365 6c66 2e74 6162    col = self.tab
+00014fb0: 6c65 732e 736f 6d65 5f74 6162 6c65 2e63  les.some_table.c
+00014fc0: 2e64 6174 610a 2020 2020 2020 2020 2020  .data.          
+00014fd0: 2020 7365 6c66 2e5f 7465 7374 2863 6f6c    self._test(col
+00014fe0: 2e63 6f6e 7461 696e 7328 2262 2323 6364  .contains("b##cd
+00014ff0: 6522 2c20 6573 6361 7065 3d22 2322 292c  e", escape="#"),
+00015000: 207b 377d 290a 0a0a 4070 7974 6573 742e   {7})...@pytest.
+00015010: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
+00015020: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+00015030: 7274 2049 5320 4449 5354 494e 4354 2046  rt IS DISTINCT F
+00015040: 524f 4d20 636c 6175 7365 2229 0a63 6c61  ROM clause").cla
+00015050: 7373 2049 734f 7249 734e 6f74 4469 7374  ss IsOrIsNotDist
+00015060: 696e 6374 4672 6f6d 5465 7374 285f 4973  inctFromTest(_Is
+00015070: 4f72 4973 4e6f 7444 6973 7469 6e63 7446  OrIsNotDistinctF
+00015080: 726f 6d54 6573 7429 3a0a 2020 2020 7061  romTest):.    pa
+00015090: 7373 0a0a 0a63 6c61 7373 204f 7264 6572  ss...class Order
+000150a0: 4279 4c61 6265 6c54 6573 7428 5f4f 7264  ByLabelTest(_Ord
+000150b0: 6572 4279 4c61 6265 6c54 6573 7429 3a0a  erByLabelTest):.
+000150c0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+000150d0: 2e73 6b69 7028 0a20 2020 2020 2020 2022  .skip(.        "
+000150e0: 5370 616e 6e65 7220 7265 7175 6972 6573  Spanner requires
+000150f0: 2061 6e20 616c 6961 7320 666f 7220 7468   an alias for th
+00015100: 6520 4752 4f55 5020 4259 206c 6973 7420  e GROUP BY list 
+00015110: 7768 656e 2073 7065 6369 6679 696e 6720  when specifying 
+00015120: 6465 7269 7665 6420 220a 2020 2020 2020  derived ".      
+00015130: 2020 2263 6f6c 756d 6e73 2061 6c73 6f20    "columns also 
+00015140: 7573 6564 2069 6e20 5345 4c45 4354 220a  used in SELECT".
+00015150: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
+00015160: 7374 5f67 726f 7570 5f62 795f 636f 6d70  st_group_by_comp
+00015170: 6f73 6564 2873 656c 6629 3a0a 2020 2020  osed(self):.    
+00015180: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+00015190: 2043 6f6d 706f 756e 6453 656c 6563 7454   CompoundSelectT
+000151a0: 6573 7428 5f43 6f6d 706f 756e 6453 656c  est(_CompoundSel
+000151b0: 6563 7454 6573 7429 3a0a 2020 2020 2222  ectTest):.    ""
+000151c0: 220a 2020 2020 5365 653a 2068 7474 7073  ".    See: https
+000151d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
+000151e0: 6f67 6c65 6170 6973 2f70 7974 686f 6e2d  ogleapis/python-
+000151f0: 7370 616e 6e65 722f 6973 7375 6573 2f33  spanner/issues/3
+00015200: 3437 0a20 2020 2022 2222 0a0a 2020 2020  47.    """..    
+00015210: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00015220: 7028 0a20 2020 2020 2020 2022 5370 616e  p(.        "Span
+00015230: 6e65 7220 4442 4150 4920 696e 636f 7272  ner DBAPI incorr
+00015240: 6563 746c 7920 636c 6173 7369 6679 2074  ectly classify t
+00015250: 6865 2073 7461 7465 6d65 6e74 2073 7461  he statement sta
+00015260: 7274 696e 6720 7769 7468 2062 7261 636b  rting with brack
+00015270: 6574 732e 220a 2020 2020 290a 2020 2020  ets.".    ).    
+00015280: 6465 6620 7465 7374 5f6c 696d 6974 5f6f  def test_limit_o
+00015290: 6666 7365 745f 7365 6c65 6374 6162 6c65  ffset_selectable
+000152a0: 5f69 6e5f 756e 696f 6e73 2873 656c 6629  _in_unions(self)
+000152b0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000152c0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+000152d0: 2e73 6b69 7028 0a20 2020 2020 2020 2022  .skip(.        "
+000152e0: 5370 616e 6e65 7220 4442 4150 4920 696e  Spanner DBAPI in
+000152f0: 636f 7272 6563 746c 7920 636c 6173 7369  correctly classi
+00015300: 6679 2074 6865 2073 7461 7465 6d65 6e74  fy the statement
+00015310: 2073 7461 7274 696e 6720 7769 7468 2062   starting with b
+00015320: 7261 636b 6574 732e 220a 2020 2020 290a  rackets.".    ).
+00015330: 2020 2020 6465 6620 7465 7374 5f6f 7264      def test_ord
+00015340: 6572 5f62 795f 7365 6c65 6374 6162 6c65  er_by_selectable
+00015350: 5f69 6e5f 756e 696f 6e73 2873 656c 6629  _in_unions(self)
+00015360: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00015370: 0a63 6c61 7373 2054 6573 7451 7565 7279  .class TestQuery
+00015380: 4869 6e74 7328 6669 7874 7572 6573 2e54  Hints(fixtures.T
+00015390: 6162 6c65 7354 6573 7429 3a0a 2020 2020  ablesTest):.    
+000153a0: 2222 220a 2020 2020 436f 6d70 696c 6520  """.    Compile 
+000153b0: 6120 636f 6d70 6c65 7820 7175 6572 7920  a complex query 
+000153c0: 7769 7468 204a 4f49 4e20 616e 6420 6368  with JOIN and ch
+000153d0: 6563 6b20 7468 6174 0a20 2020 2074 6865  eck that.    the
+000153e0: 2074 6162 6c65 2068 696e 7420 7761 7320   table hint was 
+000153f0: 7365 7420 696e 746f 2074 6865 2072 6967  set into the rig
+00015400: 6874 2070 6c61 6365 2e0a 2020 2020 2222  ht place..    ""
+00015410: 220a 0a20 2020 205f 5f62 6163 6b65 6e64  "..    __backend
+00015420: 5f5f 203d 2054 7275 650a 0a20 2020 2064  __ = True..    d
+00015430: 6566 2074 6573 745f 636f 6d70 6c65 785f  ef test_complex_
+00015440: 7175 6572 795f 7461 626c 655f 6869 6e74  query_table_hint
+00015450: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00015460: 2045 5850 4543 5445 445f 5155 4552 5920   EXPECTED_QUERY 
+00015470: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00015480: 2253 454c 4543 5420 7573 6572 732e 6964  "SELECT users.id
+00015490: 2c20 7573 6572 732e 6e61 6d65 205c 6e46  , users.name \nF
+000154a0: 524f 4d20 7573 6572 7320 407b 464f 5243  ROM users @{FORC
+000154b0: 455f 494e 4445 583d 7461 626c 655f 315f  E_INDEX=table_1_
+000154c0: 6279 5f69 6e74 5f69 6478 7d22 0a20 2020  by_int_idx}".   
+000154d0: 2020 2020 2020 2020 2022 204a 4f49 4e20           " JOIN 
+000154e0: 6164 6472 6573 7365 7320 4f4e 2075 7365  addresses ON use
+000154f0: 7273 2e69 6420 3d20 6164 6472 6573 7365  rs.id = addresse
+00015500: 732e 7573 6572 5f69 6420 220a 2020 2020  s.user_id ".    
+00015510: 2020 2020 2020 2020 225c 6e57 4845 5245          "\nWHERE
+00015520: 2075 7365 7273 2e6e 616d 6520 494e 2028   users.name IN (
+00015530: 5f5f 5b50 4f53 5443 4f4d 5049 4c45 5f6e  __[POSTCOMPILE_n
+00015540: 616d 655f 315d 2922 0a20 2020 2020 2020  ame_1])".       
+00015550: 2029 0a0a 2020 2020 2020 2020 4261 7365   )..        Base
+00015560: 203d 2064 6563 6c61 7261 7469 7665 5f62   = declarative_b
+00015570: 6173 6528 290a 2020 2020 2020 2020 656e  ase().        en
+00015580: 6769 6e65 203d 2063 7265 6174 655f 656e  gine = create_en
+00015590: 6769 6e65 280a 2020 2020 2020 2020 2020  gine(.          
+000155a0: 2020 2273 7061 6e6e 6572 3a2f 2f2f 7072    "spanner:///pr
+000155b0: 6f6a 6563 7473 2f70 726f 6a65 6374 2d69  ojects/project-i
+000155c0: 642f 696e 7374 616e 6365 732f 696e 7374  d/instances/inst
+000155d0: 616e 6365 2d69 642f 6461 7461 6261 7365  ance-id/database
+000155e0: 732f 6461 7461 6261 7365 2d69 6422 0a20  s/database-id". 
+000155f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00015600: 2020 636c 6173 7320 5573 6572 2842 6173    class User(Bas
+00015610: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00015620: 5f5f 7461 626c 656e 616d 655f 5f20 3d20  __tablename__ = 
+00015630: 2275 7365 7273 220a 2020 2020 2020 2020  "users".        
+00015640: 2020 2020 6964 203d 2043 6f6c 756d 6e28      id = Column(
+00015650: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
+00015660: 5f6b 6579 3d54 7275 6529 0a20 2020 2020  _key=True).     
+00015670: 2020 2020 2020 206e 616d 6520 3d20 436f         name = Co
+00015680: 6c75 6d6e 2853 7472 696e 6728 3530 2929  lumn(String(50))
+00015690: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+000156a0: 7265 7373 6573 203d 2072 656c 6174 696f  resses = relatio
+000156b0: 6e73 6869 7028 2241 6464 7265 7373 222c  nship("Address",
+000156c0: 2062 6163 6b72 6566 3d22 7573 6572 2229   backref="user")
+000156d0: 0a0a 2020 2020 2020 2020 636c 6173 7320  ..        class 
+000156e0: 4164 6472 6573 7328 4261 7365 293a 0a20  Address(Base):. 
+000156f0: 2020 2020 2020 2020 2020 205f 5f74 6162             __tab
+00015700: 6c65 6e61 6d65 5f5f 203d 2022 6164 6472  lename__ = "addr
+00015710: 6573 7365 7322 0a20 2020 2020 2020 2020  esses".         
+00015720: 2020 2069 6420 3d20 436f 6c75 6d6e 2849     id = Column(I
+00015730: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+00015740: 6b65 793d 5472 7565 290a 2020 2020 2020  key=True).      
+00015750: 2020 2020 2020 656d 6169 6c20 3d20 436f        email = Co
+00015760: 6c75 6d6e 2853 7472 696e 6728 3530 2929  lumn(String(50))
+00015770: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00015780: 725f 6964 203d 2043 6f6c 756d 6e28 496e  r_id = Column(In
+00015790: 7465 6765 722c 2046 6f72 6569 676e 4b65  teger, ForeignKe
+000157a0: 7928 2275 7365 7273 2e69 6422 2929 0a0a  y("users.id"))..
+000157b0: 2020 2020 2020 2020 7365 7373 696f 6e20          session 
+000157c0: 3d20 5365 7373 696f 6e28 656e 6769 6e65  = Session(engine
+000157d0: 290a 0a20 2020 2020 2020 2071 7565 7279  )..        query
+000157e0: 203d 2073 6573 7369 6f6e 2e71 7565 7279   = session.query
+000157f0: 2855 7365 7229 0a20 2020 2020 2020 2071  (User).        q
+00015800: 7565 7279 203d 2071 7565 7279 2e77 6974  uery = query.wit
+00015810: 685f 6869 6e74 280a 2020 2020 2020 2020  h_hint(.        
+00015820: 2020 2020 7365 6c65 6374 6162 6c65 3d55      selectable=U
+00015830: 7365 722c 2074 6578 743d 2240 7b46 4f52  ser, text="@{FOR
+00015840: 4345 5f49 4e44 4558 3d74 6162 6c65 5f31  CE_INDEX=table_1
+00015850: 5f62 795f 696e 745f 6964 787d 220a 2020  _by_int_idx}".  
+00015860: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00015870: 2071 7565 7279 203d 2071 7565 7279 2e66   query = query.f
+00015880: 696c 7465 7228 5573 6572 2e6e 616d 652e  ilter(User.name.
+00015890: 696e 5f28 5b22 7661 6c31 222c 2022 7661  in_(["val1", "va
+000158a0: 6c32 225d 2929 0a20 2020 2020 2020 2071  l2"])).        q
+000158b0: 7565 7279 203d 2071 7565 7279 2e6a 6f69  uery = query.joi
+000158c0: 6e28 4164 6472 6573 7329 0a0a 2020 2020  n(Address)..    
+000158d0: 2020 2020 6173 7365 7274 2073 7472 2871      assert str(q
+000158e0: 7565 7279 2e73 7461 7465 6d65 6e74 2e63  uery.statement.c
+000158f0: 6f6d 7069 6c65 2873 6573 7369 6f6e 2e62  ompile(session.b
+00015900: 696e 6429 2920 3d3d 2045 5850 4543 5445  ind)) == EXPECTE
+00015910: 445f 5155 4552 590a 0a0a 636c 6173 7320  D_QUERY...class 
+00015920: 496e 7465 726c 6561 7665 6454 6162 6c65  InterleavedTable
+00015930: 7354 6573 7428 6669 7874 7572 6573 2e54  sTest(fixtures.T
+00015940: 6573 7442 6173 6529 3a0a 2020 2020 2222  estBase):.    ""
+00015950: 220a 2020 2020 4368 6563 6b20 7468 6174  ".    Check that
+00015960: 2043 5245 4154 4520 5441 424c 4520 7374   CREATE TABLE st
+00015970: 6174 656d 656e 7473 2066 6f72 2069 6e74  atements for int
+00015980: 6572 6c65 6176 6564 2074 6162 6c65 7320  erleaved tables 
+00015990: 6172 6520 636f 7272 6563 746c 790a 2020  are correctly.  
+000159a0: 2020 6765 6e65 7261 7465 642e 0a20 2020    generated..   
+000159b0: 2022 2222 0a0a 2020 2020 6465 6620 7365   """..    def se
+000159c0: 7455 7028 7365 6c66 293a 0a20 2020 2020  tUp(self):.     
+000159d0: 2020 2073 656c 662e 5f65 6e67 696e 6520     self._engine 
+000159e0: 3d20 6372 6561 7465 5f65 6e67 696e 6528  = create_engine(
+000159f0: 0a20 2020 2020 2020 2020 2020 2022 7370  .            "sp
+00015a00: 616e 6e65 723a 2f2f 2f70 726f 6a65 6374  anner:///project
+00015a10: 732f 6170 7064 6576 2d73 6f64 612d 7370  s/appdev-soda-sp
+00015a20: 616e 6e65 722d 7374 6167 696e 672f 696e  anner-staging/in
+00015a30: 7374 616e 6365 732f 220a 2020 2020 2020  stances/".      
+00015a40: 2020 2020 2020 2273 716c 616c 6368 656d        "sqlalchem
+00015a50: 792d 6469 616c 6563 742d 7465 7374 2f64  y-dialect-test/d
+00015a60: 6174 6162 6173 6573 2f63 6f6d 706c 6961  atabases/complia
+00015a70: 6e63 652d 7465 7374 220a 2020 2020 2020  nce-test".      
+00015a80: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+00015a90: 2e5f 6d65 7461 6461 7461 203d 204d 6574  ._metadata = Met
+00015aa0: 6144 6174 6128 290a 0a20 2020 2064 6566  aData()..    def
+00015ab0: 2074 6573 745f 696e 7465 726c 6561 7665   test_interleave
+00015ac0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00015ad0: 4558 505f 5155 4552 5920 3d20 280a 2020  EXP_QUERY = (.  
+00015ae0: 2020 2020 2020 2020 2020 225c 6e43 5245            "\nCRE
+00015af0: 4154 4520 5441 424c 4520 636c 6965 6e74  ATE TABLE client
+00015b00: 2028 5c6e 5c74 7465 616d 5f69 6420 494e   (\n\tteam_id IN
+00015b10: 5436 3420 4e4f 5420 4e55 4c4c 2c20 220a  T64 NOT NULL, ".
+00015b20: 2020 2020 2020 2020 2020 2020 225c 6e5c              "\n\
+00015b30: 7463 6c69 656e 745f 6964 2049 4e54 3634  tclient_id INT64
+00015b40: 204e 4f54 204e 554c 4c2c 2022 0a20 2020   NOT NULL, ".   
+00015b50: 2020 2020 2020 2020 2022 5c6e 5c74 636c           "\n\tcl
+00015b60: 6965 6e74 5f6e 616d 6520 5354 5249 4e47  ient_name STRING
+00015b70: 2831 3629 204e 4f54 204e 554c 4c22 0a20  (16) NOT NULL". 
+00015b80: 2020 2020 2020 2020 2020 2022 5c6e 2920             "\n) 
+00015b90: 5052 494d 4152 5920 4b45 5920 2874 6561  PRIMARY KEY (tea
+00015ba0: 6d5f 6964 2c20 636c 6965 6e74 5f69 6429  m_id, client_id)
+00015bb0: 2c22 0a20 2020 2020 2020 2020 2020 2022  ,".            "
+00015bc0: 5c6e 494e 5445 524c 4541 5645 2049 4e20  \nINTERLEAVE IN 
+00015bd0: 5041 5245 4e54 2074 6561 6d5c 6e5c 6e22  PARENT team\n\n"
+00015be0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00015bf0: 2020 2063 6c69 656e 7420 3d20 5461 626c     client = Tabl
+00015c00: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
+00015c10: 636c 6965 6e74 222c 0a20 2020 2020 2020  client",.       
+00015c20: 2020 2020 2073 656c 662e 5f6d 6574 6164       self._metad
+00015c30: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00015c40: 2043 6f6c 756d 6e28 2274 6561 6d5f 6964   Column("team_id
+00015c50: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
+00015c60: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
+00015c70: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00015c80: 6e28 2263 6c69 656e 745f 6964 222c 2049  n("client_id", I
+00015c90: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+00015ca0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+00015cb0: 2020 2020 2020 2043 6f6c 756d 6e28 2263         Column("c
+00015cc0: 6c69 656e 745f 6e61 6d65 222c 2053 7472  lient_name", Str
+00015cd0: 696e 6728 3136 292c 206e 756c 6c61 626c  ing(16), nullabl
+00015ce0: 653d 4661 6c73 6529 2c0a 2020 2020 2020  e=False),.      
+00015cf0: 2020 2020 2020 7370 616e 6e65 725f 696e        spanner_in
+00015d00: 7465 726c 6561 7665 5f69 6e3d 2274 6561  terleave_in="tea
+00015d10: 6d22 2c0a 2020 2020 2020 2020 290a 2020  m",.        ).  
+00015d20: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
+00015d30: 7061 7463 6828 2267 6f6f 676c 652e 636c  patch("google.cl
+00015d40: 6f75 642e 7370 616e 6e65 725f 6462 6170  oud.spanner_dbap
+00015d50: 692e 6375 7273 6f72 2e43 7572 736f 722e  i.cursor.Cursor.
+00015d60: 6578 6563 7574 6522 2920 6173 2065 7865  execute") as exe
+00015d70: 6375 7465 3a0a 2020 2020 2020 2020 2020  cute:.          
+00015d80: 2020 636c 6965 6e74 2e63 7265 6174 6528    client.create(
+00015d90: 7365 6c66 2e5f 656e 6769 6e65 290a 2020  self._engine).  
+00015da0: 2020 2020 2020 2020 2020 6578 6563 7574            execut
+00015db0: 652e 6173 7365 7274 5f63 616c 6c65 645f  e.assert_called_
+00015dc0: 6f6e 6365 5f77 6974 6828 4558 505f 5155  once_with(EXP_QU
+00015dd0: 4552 592c 205b 5d29 0a0a 2020 2020 6465  ERY, [])..    de
+00015de0: 6620 7465 7374 5f69 6e74 6572 6c65 6176  f test_interleav
+00015df0: 655f 6f6e 5f64 656c 6574 655f 6361 7363  e_on_delete_casc
+00015e00: 6164 6528 7365 6c66 293a 0a20 2020 2020  ade(self):.     
+00015e10: 2020 2045 5850 5f51 5545 5259 203d 2028     EXP_QUERY = (
+00015e20: 0a20 2020 2020 2020 2020 2020 2022 5c6e  .            "\n
+00015e30: 4352 4541 5445 2054 4142 4c45 2063 6c69  CREATE TABLE cli
+00015e40: 656e 7420 285c 6e5c 7474 6561 6d5f 6964  ent (\n\tteam_id
+00015e50: 2049 4e54 3634 204e 4f54 204e 554c 4c2c   INT64 NOT NULL,
+00015e60: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+00015e70: 5c6e 5c74 636c 6965 6e74 5f69 6420 494e  \n\tclient_id IN
+00015e80: 5436 3420 4e4f 5420 4e55 4c4c 2c20 220a  T64 NOT NULL, ".
+00015e90: 2020 2020 2020 2020 2020 2020 225c 6e5c              "\n\
+00015ea0: 7463 6c69 656e 745f 6e61 6d65 2053 5452  tclient_name STR
+00015eb0: 494e 4728 3136 2920 4e4f 5420 4e55 4c4c  ING(16) NOT NULL
+00015ec0: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
+00015ed0: 6e29 2050 5249 4d41 5259 204b 4559 2028  n) PRIMARY KEY (
+00015ee0: 7465 616d 5f69 642c 2063 6c69 656e 745f  team_id, client_
+00015ef0: 6964 292c 220a 2020 2020 2020 2020 2020  id),".          
+00015f00: 2020 225c 6e49 4e54 4552 4c45 4156 4520    "\nINTERLEAVE 
+00015f10: 494e 2050 4152 454e 5420 7465 616d 204f  IN PARENT team O
+00015f20: 4e20 4445 4c45 5445 2043 4153 4341 4445  N DELETE CASCADE
+00015f30: 5c6e 5c6e 220a 2020 2020 2020 2020 290a  \n\n".        ).
+00015f40: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
+00015f50: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00015f60: 2020 2020 2263 6c69 656e 7422 2c0a 2020      "client",.  
+00015f70: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00015f80: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00015f90: 2020 2020 2020 436f 6c75 6d6e 2822 7465        Column("te
+00015fa0: 616d 5f69 6422 2c20 496e 7465 6765 722c  am_id", Integer,
+00015fb0: 2070 7269 6d61 7279 5f6b 6579 3d54 7275   primary_key=Tru
+00015fc0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00015fd0: 436f 6c75 6d6e 2822 636c 6965 6e74 5f69  Column("client_i
+00015fe0: 6422 2c20 496e 7465 6765 722c 2070 7269  d", Integer, pri
+00015ff0: 6d61 7279 5f6b 6579 3d54 7275 6529 2c0a  mary_key=True),.
+00016000: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00016010: 6d6e 2822 636c 6965 6e74 5f6e 616d 6522  mn("client_name"
+00016020: 2c20 5374 7269 6e67 2831 3629 2c20 6e75  , String(16), nu
+00016030: 6c6c 6162 6c65 3d46 616c 7365 292c 0a20  llable=False),. 
+00016040: 2020 2020 2020 2020 2020 2073 7061 6e6e             spann
+00016050: 6572 5f69 6e74 6572 6c65 6176 655f 696e  er_interleave_in
+00016060: 3d22 7465 616d 222c 0a20 2020 2020 2020  ="team",.       
+00016070: 2020 2020 2073 7061 6e6e 6572 5f69 6e74       spanner_int
+00016080: 6572 6c65 6176 655f 6f6e 5f64 656c 6574  erleave_on_delet
+00016090: 655f 6361 7363 6164 653d 5472 7565 2c0a  e_cascade=True,.
+000160a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000160b0: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
+000160c0: 6828 2267 6f6f 676c 652e 636c 6f75 642e  h("google.cloud.
+000160d0: 7370 616e 6e65 725f 6462 6170 692e 6375  spanner_dbapi.cu
+000160e0: 7273 6f72 2e43 7572 736f 722e 6578 6563  rsor.Cursor.exec
+000160f0: 7574 6522 2920 6173 2065 7865 6375 7465  ute") as execute
+00016100: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+00016110: 6965 6e74 2e63 7265 6174 6528 7365 6c66  ient.create(self
+00016120: 2e5f 656e 6769 6e65 290a 2020 2020 2020  ._engine).      
+00016130: 2020 2020 2020 6578 6563 7574 652e 6173        execute.as
+00016140: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+00016150: 5f77 6974 6828 4558 505f 5155 4552 592c  _with(EXP_QUERY,
+00016160: 205b 5d29 0a0a 0a63 6c61 7373 2055 7365   [])...class Use
+00016170: 7241 6765 6e74 5465 7374 2866 6978 7475  rAgentTest(fixtu
+00016180: 7265 732e 5465 7374 4261 7365 293a 0a20  res.TestBase):. 
+00016190: 2020 2022 2222 4368 6563 6b20 7468 6174     """Check that
+000161a0: 2053 514c 416c 6368 656d 7920 6469 616c   SQLAlchemy dial
+000161b0: 6563 7420 7573 6573 2063 6f72 7265 6374  ect uses correct
+000161c0: 2075 7365 7220 6167 656e 742e 2222 220a   user agent.""".
+000161d0: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
+000161e0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+000161f0: 6c66 2e5f 656e 6769 6e65 203d 2063 7265  lf._engine = cre
+00016200: 6174 655f 656e 6769 6e65 280a 2020 2020  ate_engine(.    
+00016210: 2020 2020 2020 2020 2273 7061 6e6e 6572          "spanner
+00016220: 3a2f 2f2f 7072 6f6a 6563 7473 2f61 7070  :///projects/app
+00016230: 6465 762d 736f 6461 2d73 7061 6e6e 6572  dev-soda-spanner
+00016240: 2d73 7461 6769 6e67 2f69 6e73 7461 6e63  -staging/instanc
+00016250: 6573 2f22 0a20 2020 2020 2020 2020 2020  es/".           
+00016260: 2022 7371 6c61 6c63 6865 6d79 2d64 6961   "sqlalchemy-dia
+00016270: 6c65 6374 2d74 6573 742f 6461 7461 6261  lect-test/databa
+00016280: 7365 732f 636f 6d70 6c69 616e 6365 2d74  ses/compliance-t
+00016290: 6573 7422 0a20 2020 2020 2020 2029 0a20  est".        ). 
+000162a0: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
+000162b0: 6164 6174 6120 3d20 4d65 7461 4461 7461  adata = MetaData
+000162c0: 2829 0a0a 2020 2020 6465 6620 7465 7374  ()..    def test
+000162d0: 5f75 7365 725f 6167 656e 7428 7365 6c66  _user_agent(self
+000162e0: 293a 0a20 2020 2020 2020 2064 6973 7420  ):.        dist 
+000162f0: 3d20 706b 675f 7265 736f 7572 6365 732e  = pkg_resources.
+00016300: 6765 745f 6469 7374 7269 6275 7469 6f6e  get_distribution
+00016310: 2822 7371 6c61 6c63 6865 6d79 2d73 7061  ("sqlalchemy-spa
+00016320: 6e6e 6572 2229 0a0a 2020 2020 2020 2020  nner")..        
+00016330: 7769 7468 2073 656c 662e 5f65 6e67 696e  with self._engin
+00016340: 652e 636f 6e6e 6563 7428 2920 6173 2063  e.connect() as c
+00016350: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
+00016360: 2020 2020 2020 2061 7373 6572 7420 280a         assert (.
+00016370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016380: 636f 6e6e 6563 7469 6f6e 2e63 6f6e 6e65  connection.conne
+00016390: 6374 696f 6e2e 696e 7374 616e 6365 2e5f  ction.instance._
+000163a0: 636c 6965 6e74 2e5f 636c 6965 6e74 5f69  client._client_i
+000163b0: 6e66 6f2e 7573 6572 5f61 6765 6e74 0a20  nfo.user_agent. 
+000163c0: 2020 2020 2020 2020 2020 2020 2020 203d                 =
+000163d0: 3d20 2267 6c2d 2220 2b20 6469 7374 2e70  = "gl-" + dist.p
+000163e0: 726f 6a65 6374 5f6e 616d 6520 2b20 222f  roject_name + "/
+000163f0: 2220 2b20 6469 7374 2e76 6572 7369 6f6e  " + dist.version
+00016400: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00016410: 0a63 6c61 7373 2053 696d 706c 6555 7064  .class SimpleUpd
+00016420: 6174 6544 656c 6574 6554 6573 7428 5f53  ateDeleteTest(_S
+00016430: 696d 706c 6555 7064 6174 6544 656c 6574  impleUpdateDelet
+00016440: 6554 6573 7429 3a0a 2020 2020 2222 220a  eTest):.    """.
+00016450: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+00016460: 5249 4445 3a0a 0a20 2020 2053 7061 6e6e  RIDE:..    Spann
+00016470: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+00016480: 7274 2060 726f 7763 6f75 6e74 6020 7072  rt `rowcount` pr
+00016490: 6f70 6572 7479 2e20 5468 6573 650a 2020  operty. These.  
+000164a0: 2020 7465 7374 2063 6173 6573 206f 7665    test cases ove
+000164b0: 7272 6964 6573 206f 6d69 7420 6072 6f77  rrides omit `row
+000164c0: 636f 756e 7460 2063 6865 636b 732e 0a20  count` checks.. 
+000164d0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+000164e0: 7465 7374 5f64 656c 6574 6528 7365 6c66  test_delete(self
+000164f0: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00016500: 2020 2020 2020 2074 203d 2073 656c 662e         t = self.
+00016510: 7461 626c 6573 2e70 6c61 696e 5f70 6b0a  tables.plain_pk.
+00016520: 2020 2020 2020 2020 7220 3d20 636f 6e6e          r = conn
+00016530: 6563 7469 6f6e 2e65 7865 6375 7465 2874  ection.execute(t
+00016540: 2e64 656c 6574 6528 292e 7768 6572 6528  .delete().where(
+00016550: 742e 632e 6964 203d 3d20 3229 290a 2020  t.c.id == 2)).  
+00016560: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
+00016570: 2072 2e69 735f 696e 7365 7274 0a20 2020   r.is_insert.   
+00016580: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
+00016590: 722e 7265 7475 726e 735f 726f 7773 0a20  r.returns_rows. 
+000165a0: 2020 2020 2020 2065 715f 280a 2020 2020         eq_(.    
+000165b0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+000165c0: 6f6e 2e65 7865 6375 7465 2874 2e73 656c  on.execute(t.sel
+000165d0: 6563 7428 292e 6f72 6465 725f 6279 2874  ect().order_by(t
+000165e0: 2e63 2e69 6429 292e 6665 7463 6861 6c6c  .c.id)).fetchall
+000165f0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00016600: 5b28 312c 2022 6431 2229 2c20 2833 2c20  [(1, "d1"), (3, 
+00016610: 2264 3322 295d 2c0a 2020 2020 2020 2020  "d3")],.        
+00016620: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00016630: 7570 6461 7465 2873 656c 662c 2063 6f6e  update(self, con
+00016640: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
+00016650: 2020 7420 3d20 7365 6c66 2e74 6162 6c65    t = self.table
+00016660: 732e 706c 6169 6e5f 706b 0a20 2020 2020  s.plain_pk.     
+00016670: 2020 2072 203d 2063 6f6e 6e65 6374 696f     r = connectio
+00016680: 6e2e 6578 6563 7574 6528 742e 7570 6461  n.execute(t.upda
+00016690: 7465 2829 2e77 6865 7265 2874 2e63 2e69  te().where(t.c.i
+000166a0: 6420 3d3d 2032 292c 2064 6963 7428 6461  d == 2), dict(da
+000166b0: 7461 3d22 6432 5f6e 6577 2229 290a 2020  ta="d2_new")).  
+000166c0: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
+000166d0: 2072 2e69 735f 696e 7365 7274 0a20 2020   r.is_insert.   
+000166e0: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
+000166f0: 722e 7265 7475 726e 735f 726f 7773 0a0a  r.returns_rows..
+00016700: 2020 2020 2020 2020 6571 5f28 0a20 2020          eq_(.   
+00016710: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+00016720: 696f 6e2e 6578 6563 7574 6528 742e 7365  ion.execute(t.se
+00016730: 6c65 6374 2829 2e6f 7264 6572 5f62 7928  lect().order_by(
+00016740: 742e 632e 6964 2929 2e66 6574 6368 616c  t.c.id)).fetchal
+00016750: 6c28 292c 0a20 2020 2020 2020 2020 2020  l(),.           
+00016760: 205b 2831 2c20 2264 3122 292c 2028 322c   [(1, "d1"), (2,
+00016770: 2022 6432 5f6e 6577 2229 2c20 2833 2c20   "d2_new"), (3, 
+00016780: 2264 3322 295d 2c0a 2020 2020 2020 2020  "d3")],.        
+00016790: 290a 0a0a 636c 6173 7320 4861 7349 6e64  )...class HasInd
+000167a0: 6578 5465 7374 285f 4861 7349 6e64 6578  exTest(_HasIndex
+000167b0: 5465 7374 293a 0a20 2020 205f 5f62 6163  Test):.    __bac
+000167c0: 6b65 6e64 5f5f 203d 2054 7275 650a 2020  kend__ = True.  
+000167d0: 2020 6b69 6e64 203d 2074 6573 7469 6e67    kind = testing
+000167e0: 2e63 6f6d 6269 6e61 7469 6f6e 7328 2264  .combinations("d
+000167f0: 6961 6c65 6374 222c 2022 696e 7370 6563  ialect", "inspec
+00016800: 746f 7222 2c20 6172 676e 616d 6573 3d22  tor", argnames="
+00016810: 6b69 6e64 2229 0a0a 2020 2020 4063 6c61  kind")..    @cla
+00016820: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00016830: 2064 6566 696e 655f 7461 626c 6573 2863   define_tables(c
+00016840: 6c73 2c20 6d65 7461 6461 7461 293a 0a20  ls, metadata):. 
+00016850: 2020 2020 2020 2074 7420 3d20 5461 626c         tt = Tabl
+00016860: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
+00016870: 7465 7374 5f74 6162 6c65 222c 0a20 2020  test_table",.   
+00016880: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00016890: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
+000168a0: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
+000168b0: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+000168c0: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+000168d0: 2020 2020 436f 6c75 6d6e 2822 6461 7461      Column("data
+000168e0: 222c 2053 7472 696e 6728 3530 2929 2c0a  ", String(50)),.
+000168f0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00016900: 6d6e 2822 6461 7461 3222 2c20 5374 7269  mn("data2", Stri
+00016910: 6e67 2835 3029 292c 0a20 2020 2020 2020  ng(50)),.       
+00016920: 2029 0a20 2020 2020 2020 2073 716c 616c   ).        sqlal
+00016930: 6368 656d 792e 496e 6465 7828 226d 795f  chemy.Index("my_
+00016940: 6964 7822 2c20 7474 2e63 2e64 6174 6129  idx", tt.c.data)
+00016950: 0a0a 2020 2020 406b 696e 640a 2020 2020  ..    @kind.    
+00016960: 6465 6620 7465 7374 5f68 6173 5f69 6e64  def test_has_ind
+00016970: 6578 2873 656c 662c 206b 696e 642c 2063  ex(self, kind, c
+00016980: 6f6e 6e65 6374 696f 6e2c 206d 6574 6164  onnection, metad
+00016990: 6174 6129 3a0a 2020 2020 2020 2020 6d65  ata):.        me
+000169a0: 7468 203d 2073 656c 662e 5f68 6173 5f69  th = self._has_i
+000169b0: 6e64 6578 286b 696e 642c 2063 6f6e 6e65  ndex(kind, conne
+000169c0: 6374 696f 6e29 0a20 2020 2020 2020 2061  ction).        a
+000169d0: 7373 6572 7420 6d65 7468 2822 7465 7374  ssert meth("test
+000169e0: 5f74 6162 6c65 222c 2022 6d79 5f69 6478  _table", "my_idx
+000169f0: 2229 0a20 2020 2020 2020 2061 7373 6572  ").        asser
+00016a00: 7420 6e6f 7420 6d65 7468 2822 7465 7374  t not meth("test
+00016a10: 5f74 6162 6c65 222c 2022 6d79 5f69 6478  _table", "my_idx
+00016a20: 5f73 2229 0a20 2020 2020 2020 2061 7373  _s").        ass
+00016a30: 6572 7420 6e6f 7420 6d65 7468 2822 6e6f  ert not meth("no
+00016a40: 6e65 7869 7374 656e 745f 7461 626c 6522  nexistent_table"
+00016a50: 2c20 226d 795f 6964 7822 290a 2020 2020  , "my_idx").    
+00016a60: 2020 2020 6173 7365 7274 206e 6f74 206d      assert not m
+00016a70: 6574 6828 2274 6573 745f 7461 626c 6522  eth("test_table"
+00016a80: 2c20 226e 6f6e 6578 6973 7465 6e74 5f69  , "nonexistent_i
+00016a90: 6478 2229 0a0a 2020 2020 2020 2020 6173  dx")..        as
+00016aa0: 7365 7274 206e 6f74 206d 6574 6828 2274  sert not meth("t
+00016ab0: 6573 745f 7461 626c 6522 2c20 226d 795f  est_table", "my_
+00016ac0: 6964 785f 3222 290a 2020 2020 2020 2020  idx_2").        
+00016ad0: 6173 7365 7274 206e 6f74 206d 6574 6828  assert not meth(
+00016ae0: 2274 6573 745f 7461 626c 655f 3222 2c20  "test_table_2", 
+00016af0: 226d 795f 6964 785f 3322 290a 2020 2020  "my_idx_3").    
+00016b00: 2020 2020 6964 7820 3d20 496e 6465 7828      idx = Index(
+00016b10: 226d 795f 6964 785f 3222 2c20 7365 6c66  "my_idx_2", self
+00016b20: 2e74 6162 6c65 732e 7465 7374 5f74 6162  .tables.test_tab
+00016b30: 6c65 2e63 2e64 6174 6132 290a 2020 2020  le.c.data2).    
+00016b40: 2020 2020 7462 6c20 3d20 5461 626c 6528      tbl = Table(
+00016b50: 0a20 2020 2020 2020 2020 2020 2022 7465  .            "te
+00016b60: 7374 5f74 6162 6c65 5f32 222c 0a20 2020  st_table_2",.   
+00016b70: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00016b80: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
+00016b90: 6f6c 756d 6e28 2266 6f6f 222c 2049 6e74  olumn("foo", Int
+00016ba0: 6567 6572 2c20 7072 696d 6172 795f 6b65  eger, primary_ke
+00016bb0: 793d 5472 7565 292c 0a20 2020 2020 2020  y=True),.       
+00016bc0: 2020 2020 2049 6e64 6578 2822 6d79 5f69       Index("my_i
+00016bd0: 6478 5f33 222c 2022 666f 6f22 292c 0a20  dx_3", "foo"),. 
+00016be0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00016bf0: 2069 6478 2e63 7265 6174 6528 636f 6e6e   idx.create(conn
+00016c00: 6563 7469 6f6e 290a 2020 2020 2020 2020  ection).        
+00016c10: 7462 6c2e 6372 6561 7465 2863 6f6e 6e65  tbl.create(conne
+00016c20: 6374 696f 6e29 0a0a 2020 2020 2020 2020  ction)..        
+00016c30: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00016c40: 2069 6620 6b69 6e64 203d 3d20 2269 6e73   if kind == "ins
+00016c50: 7065 6374 6f72 223a 0a20 2020 2020 2020  pector":.       
+00016c60: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00016c70: 6e6f 7420 6d65 7468 2822 7465 7374 5f74  not meth("test_t
+00016c80: 6162 6c65 222c 2022 6d79 5f69 6478 5f32  able", "my_idx_2
+00016c90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00016ca0: 2020 2061 7373 6572 7420 6e6f 7420 6d65     assert not me
+00016cb0: 7468 2822 7465 7374 5f74 6162 6c65 5f32  th("test_table_2
+00016cc0: 222c 2022 6d79 5f69 6478 5f33 2229 0a20  ", "my_idx_3"). 
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016ce0: 6574 682e 5f5f 7365 6c66 5f5f 2e63 6c65  eth.__self__.cle
+00016cf0: 6172 5f63 6163 6865 2829 0a20 2020 2020  ar_cache().     
+00016d00: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+00016d10: 6e2e 636f 6e6e 6563 7469 6f6e 2e63 6f6d  n.connection.com
+00016d20: 6d69 7428 290a 2020 2020 2020 2020 2020  mit().          
+00016d30: 2020 6173 7365 7274 206d 6574 6828 2274    assert meth("t
+00016d40: 6573 745f 7461 626c 6522 2c20 226d 795f  est_table", "my_
+00016d50: 6964 785f 3222 2920 6973 2054 7275 650a  idx_2") is True.
+00016d60: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00016d70: 7274 206d 6574 6828 2274 6573 745f 7461  rt meth("test_ta
+00016d80: 626c 655f 3222 2c20 226d 795f 6964 785f  ble_2", "my_idx_
+00016d90: 3322 2920 6973 2054 7275 650a 2020 2020  3") is True.    
+00016da0: 2020 2020 6669 6e61 6c6c 793a 0a20 2020      finally:.   
+00016db0: 2020 2020 2020 2020 2074 626c 2e64 726f           tbl.dro
+00016dc0: 7028 636f 6e6e 6563 7469 6f6e 290a 2020  p(connection).  
+00016dd0: 2020 2020 2020 2020 2020 6964 782e 6472            idx.dr
+00016de0: 6f70 2863 6f6e 6e65 6374 696f 6e29 0a20  op(connection). 
+00016df0: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+00016e00: 6374 696f 6e2e 636f 6e6e 6563 7469 6f6e  ction.connection
+00016e10: 2e63 6f6d 6d69 7428 290a 2020 2020 2020  .commit().      
+00016e20: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
+00016e30: 735b 2274 6573 745f 7461 626c 6522 5d2e  s["test_table"].
+00016e40: 696e 6465 7865 732e 7265 6d6f 7665 2869  indexes.remove(i
+00016e50: 6478 290a 0a20 2020 2040 7079 7465 7374  dx)..    @pytest
+00016e60: 2e6d 6172 6b2e 736b 6970 2822 4e6f 7420  .mark.skip("Not 
+00016e70: 7375 7070 6f72 7465 6420 6279 2043 6c6f  supported by Clo
+00016e80: 7564 2053 7061 6e6e 6572 2229 0a20 2020  ud Spanner").   
+00016e90: 2040 6b69 6e64 0a20 2020 2064 6566 2074   @kind.    def t
+00016ea0: 6573 745f 6861 735f 696e 6465 785f 7363  est_has_index_sc
+00016eb0: 6865 6d61 2873 656c 662c 206b 696e 642c  hema(self, kind,
+00016ec0: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
+00016ed0: 2020 2020 2020 7061 7373 0a0a 0a63 6c61        pass...cla
+00016ee0: 7373 2048 6173 5461 626c 6554 6573 7428  ss HasTableTest(
+00016ef0: 5f48 6173 5461 626c 6554 6573 7429 3a0a  _HasTableTest):.
+00016f00: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00016f10: 0a20 2020 2064 6566 2064 6566 696e 655f  .    def define_
+00016f20: 7461 626c 6573 2863 6c73 2c20 6d65 7461  tables(cls, meta
+00016f30: 6461 7461 293a 0a20 2020 2020 2020 2054  data):.        T
+00016f40: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+00016f50: 2020 2274 6573 745f 7461 626c 6522 2c0a    "test_table",.
+00016f60: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00016f70: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+00016f80: 2020 436f 6c75 6d6e 2822 6964 222c 2049    Column("id", I
+00016f90: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+00016fa0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+00016fb0: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
+00016fc0: 6174 6122 2c20 5374 7269 6e67 2835 3029  ata", String(50)
+00016fd0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00016fe0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00016ff0: 6b69 7028 224e 6f74 2073 7570 706f 7274  kip("Not support
+00017000: 6564 2062 7920 436c 6f75 6420 5370 616e  ed by Cloud Span
+00017010: 6e65 7222 290a 2020 2020 6465 6620 7465  ner").    def te
+00017020: 7374 5f68 6173 5f74 6162 6c65 5f6e 6f6e  st_has_table_non
+00017030: 6578 6973 7465 6e74 5f73 6368 656d 6128  existent_schema(
+00017040: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00017050: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+00017060: 2e6d 6172 6b2e 736b 6970 2822 4e6f 7420  .mark.skip("Not 
+00017070: 7375 7070 6f72 7465 6420 6279 2043 6c6f  supported by Clo
+00017080: 7564 2053 7061 6e6e 6572 2229 0a20 2020  ud Spanner").   
+00017090: 2064 6566 2074 6573 745f 6861 735f 7461   def test_has_ta
+000170a0: 626c 655f 7363 6865 6d61 2873 656c 6629  ble_schema(self)
+000170b0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000170c0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+000170d0: 2e73 6b69 7028 224e 6f74 2073 7570 706f  .skip("Not suppo
+000170e0: 7274 6564 2062 7920 436c 6f75 6420 5370  rted by Cloud Sp
+000170f0: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
+00017100: 7465 7374 5f68 6173 5f74 6162 6c65 5f63  test_has_table_c
+00017110: 6163 6865 2873 656c 6629 3a0a 2020 2020  ache(self):.    
+00017120: 2020 2020 7061 7373 0a0a 2020 2020 4074      pass..    @t
+00017130: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00017140: 7669 6577 730a 2020 2020 6465 6620 7465  views.    def te
+00017150: 7374 5f68 6173 5f74 6162 6c65 5f76 6965  st_has_table_vie
+00017160: 7728 7365 6c66 2c20 636f 6e6e 6563 7469  w(self, connecti
+00017170: 6f6e 293a 0a20 2020 2020 2020 2070 6173  on):.        pas
+00017180: 730a 0a20 2020 2040 7465 7374 696e 672e  s..    @testing.
+00017190: 7265 7175 6972 6573 2e76 6965 7773 0a20  requires.views. 
+000171a0: 2020 2064 6566 2074 6573 745f 6861 735f     def test_has_
+000171b0: 7461 626c 655f 7669 6577 5f73 6368 656d  table_view_schem
+000171c0: 6128 7365 6c66 2c20 636f 6e6e 6563 7469  a(self, connecti
+000171d0: 6f6e 293a 0a20 2020 2020 2020 2070 6173  on):.        pas
+000171e0: 730a 0a0a 636c 6173 7320 506f 7374 436f  s...class PostCo
+000171f0: 6d70 696c 6550 6172 616d 7354 6573 7428  mpileParamsTest(
+00017200: 5f50 6f73 7443 6f6d 7069 6c65 5061 7261  _PostCompilePara
+00017210: 6d73 5465 7374 293a 0a20 2020 2064 6566  msTest):.    def
+00017220: 2074 6573 745f 6578 6563 7574 6528 7365   test_execute(se
+00017230: 6c66 293a 0a20 2020 2020 2020 2074 6162  lf):.        tab
+00017240: 6c65 203d 2073 656c 662e 7461 626c 6573  le = self.tables
+00017250: 2e73 6f6d 655f 7461 626c 650a 0a20 2020  .some_table..   
+00017260: 2020 2020 2073 746d 7420 3d20 7365 6c65       stmt = sele
+00017270: 6374 2874 6162 6c65 2e63 2e69 6429 2e77  ct(table.c.id).w
+00017280: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
+00017290: 2020 7461 626c 652e 632e 7820 3d3d 2073    table.c.x == s
+000172a0: 716c 616c 6368 656d 792e 6269 6e64 7061  qlalchemy.bindpa
+000172b0: 7261 6d28 2271 222c 206c 6974 6572 616c  ram("q", literal
+000172c0: 5f65 7865 6375 7465 3d54 7275 6529 0a20  _execute=True). 
+000172d0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000172e0: 2020 7769 7468 2073 656c 662e 7371 6c5f    with self.sql_
+000172f0: 6578 6563 7574 696f 6e5f 6173 7365 7274  execution_assert
+00017300: 6572 2829 2061 7320 6173 7365 7274 6572  er() as asserter
+00017310: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00017320: 7468 2063 6f6e 6669 672e 6462 2e63 6f6e  th config.db.con
+00017330: 6e65 6374 2829 2061 7320 636f 6e6e 3a0a  nect() as conn:.
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 636f 6e6e 2e65 7865 6375 7465 2873 746d  conn.execute(stm
+00017360: 742c 2064 6963 7428 713d 3130 2929 0a0a  t, dict(q=10))..
+00017370: 2020 2020 2020 2020 6173 7365 7274 6572          asserter
+00017380: 2e61 7373 6572 745f 280a 2020 2020 2020  .assert_(.      
+00017390: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+000173a0: 2e74 6573 7469 6e67 2e61 7373 6572 7473  .testing.asserts
+000173b0: 716c 2e43 7572 736f 7253 514c 280a 2020  ql.CursorSQL(.  
+000173c0: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+000173d0: 454c 4543 5420 736f 6d65 5f74 6162 6c65  ELECT some_table
+000173e0: 2e69 6420 5c6e 4652 4f4d 2073 6f6d 655f  .id \nFROM some_
+000173f0: 7461 626c 6520 2220 225c 6e57 4845 5245  table " "\nWHERE
+00017400: 2073 6f6d 655f 7461 626c 652e 7820 3d20   some_table.x = 
+00017410: 3130 222c 0a20 2020 2020 2020 2020 2020  10",.           
+00017420: 2020 2020 205b 5d20 6966 2063 6f6e 6669       [] if confi
+00017430: 672e 6462 2e64 6961 6c65 6374 2e70 6f73  g.db.dialect.pos
+00017440: 6974 696f 6e61 6c20 656c 7365 207b 7d2c  itional else {},
+00017450: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00017460: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00017470: 6620 7465 7374 5f65 7865 6375 7465 5f65  f test_execute_e
+00017480: 7870 616e 6469 6e67 5f70 6c75 735f 6c69  xpanding_plus_li
+00017490: 7465 7261 6c5f 6578 6563 7574 6528 7365  teral_execute(se
+000174a0: 6c66 293a 0a20 2020 2020 2020 2074 6162  lf):.        tab
+000174b0: 6c65 203d 2073 656c 662e 7461 626c 6573  le = self.tables
+000174c0: 2e73 6f6d 655f 7461 626c 650a 0a20 2020  .some_table..   
+000174d0: 2020 2020 2073 746d 7420 3d20 7365 6c65       stmt = sele
+000174e0: 6374 2874 6162 6c65 2e63 2e69 6429 2e77  ct(table.c.id).w
+000174f0: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
+00017500: 2020 7461 626c 652e 632e 782e 696e 5f28    table.c.x.in_(
+00017510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017520: 2073 716c 616c 6368 656d 792e 6269 6e64   sqlalchemy.bind
+00017530: 7061 7261 6d28 2271 222c 2065 7870 616e  param("q", expan
+00017540: 6469 6e67 3d54 7275 652c 206c 6974 6572  ding=True, liter
+00017550: 616c 5f65 7865 6375 7465 3d54 7275 6529  al_execute=True)
+00017560: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00017570: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00017580: 2020 7769 7468 2073 656c 662e 7371 6c5f    with self.sql_
+00017590: 6578 6563 7574 696f 6e5f 6173 7365 7274  execution_assert
+000175a0: 6572 2829 2061 7320 6173 7365 7274 6572  er() as asserter
+000175b0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+000175c0: 7468 2063 6f6e 6669 672e 6462 2e63 6f6e  th config.db.con
+000175d0: 6e65 6374 2829 2061 7320 636f 6e6e 3a0a  nect() as conn:.
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 636f 6e6e 2e65 7865 6375 7465 2873 746d  conn.execute(stm
+00017600: 742c 2064 6963 7428 713d 5b35 2c20 362c  t, dict(q=[5, 6,
+00017610: 2037 5d29 290a 0a20 2020 2020 2020 2061   7]))..        a
+00017620: 7373 6572 7465 722e 6173 7365 7274 5f28  sserter.assert_(
+00017630: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
+00017640: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
+00017650: 6173 7365 7274 7371 6c2e 4375 7273 6f72  assertsql.Cursor
+00017660: 5351 4c28 0a20 2020 2020 2020 2020 2020  SQL(.           
+00017670: 2020 2020 2022 5345 4c45 4354 2073 6f6d       "SELECT som
+00017680: 655f 7461 626c 652e 6964 205c 6e46 524f  e_table.id \nFRO
+00017690: 4d20 736f 6d65 5f74 6162 6c65 2022 0a20  M some_table ". 
+000176a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000176b0: 5c6e 5748 4552 4520 736f 6d65 5f74 6162  \nWHERE some_tab
+000176c0: 6c65 2e78 2049 4e20 2835 2c20 362c 2037  le.x IN (5, 6, 7
+000176d0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+000176e0: 2020 2020 5b5d 2069 6620 636f 6e66 6967      [] if config
+000176f0: 2e64 622e 6469 616c 6563 742e 706f 7369  .db.dialect.posi
+00017700: 7469 6f6e 616c 2065 6c73 6520 7b7d 2c0a  tional else {},.
+00017710: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00017720: 2020 2020 2020 290a 0a20 2020 2040 7465        )..    @te
+00017730: 7374 696e 672e 7265 7175 6972 6573 2e74  sting.requires.t
+00017740: 7570 6c65 5f69 6e0a 2020 2020 6465 6620  uple_in.    def 
+00017750: 7465 7374 5f65 7865 6375 7465 5f74 7570  test_execute_tup
+00017760: 6c65 5f65 7870 616e 6469 6e67 5f70 6c75  le_expanding_plu
+00017770: 735f 6c69 7465 7261 6c5f 6578 6563 7574  s_literal_execut
+00017780: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00017790: 2074 6162 6c65 203d 2073 656c 662e 7461   table = self.ta
+000177a0: 626c 6573 2e73 6f6d 655f 7461 626c 650a  bles.some_table.
+000177b0: 0a20 2020 2020 2020 2073 746d 7420 3d20  .        stmt = 
+000177c0: 7365 6c65 6374 2874 6162 6c65 2e63 2e69  select(table.c.i
+000177d0: 6429 2e77 6865 7265 280a 2020 2020 2020  d).where(.      
+000177e0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+000177f0: 2e74 7570 6c65 5f28 7461 626c 652e 632e  .tuple_(table.c.
+00017800: 782c 2074 6162 6c65 2e63 2e79 292e 696e  x, table.c.y).in
+00017810: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
+00017820: 2020 2073 716c 616c 6368 656d 792e 6269     sqlalchemy.bi
+00017830: 6e64 7061 7261 6d28 2271 222c 2065 7870  ndparam("q", exp
+00017840: 616e 6469 6e67 3d54 7275 652c 206c 6974  anding=True, lit
+00017850: 6572 616c 5f65 7865 6375 7465 3d54 7275  eral_execute=Tru
+00017860: 6529 0a20 2020 2020 2020 2020 2020 2029  e).            )
+00017870: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00017880: 2020 2020 7769 7468 2073 656c 662e 7371      with self.sq
+00017890: 6c5f 6578 6563 7574 696f 6e5f 6173 7365  l_execution_asse
+000178a0: 7274 6572 2829 2061 7320 6173 7365 7274  rter() as assert
+000178b0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000178c0: 7769 7468 2063 6f6e 6669 672e 6462 2e63  with config.db.c
+000178d0: 6f6e 6e65 6374 2829 2061 7320 636f 6e6e  onnect() as conn
+000178e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000178f0: 2020 636f 6e6e 2e65 7865 6375 7465 2873    conn.execute(s
+00017900: 746d 742c 2064 6963 7428 713d 5b28 352c  tmt, dict(q=[(5,
+00017910: 2031 3029 2c20 2831 322c 2031 3829 5d29   10), (12, 18)])
+00017920: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00017930: 7465 722e 6173 7365 7274 5f28 0a20 2020  ter.assert_(.   
+00017940: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
+00017950: 656d 792e 7465 7374 696e 672e 6173 7365  emy.testing.asse
+00017960: 7274 7371 6c2e 4375 7273 6f72 5351 4c28  rtsql.CursorSQL(
+00017970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017980: 2022 5345 4c45 4354 2073 6f6d 655f 7461   "SELECT some_ta
+00017990: 626c 652e 6964 205c 6e46 524f 4d20 736f  ble.id \nFROM so
+000179a0: 6d65 5f74 6162 6c65 2022 0a20 2020 2020  me_table ".     
+000179b0: 2020 2020 2020 2020 2020 2022 5c6e 5748             "\nWH
+000179c0: 4552 4520 2873 6f6d 655f 7461 626c 652e  ERE (some_table.
+000179d0: 782c 2073 6f6d 655f 7461 626c 652e 7929  x, some_table.y)
+000179e0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+000179f0: 2020 2022 494e 2028 2573 2835 2c20 3130     "IN (%s(5, 10
+00017a00: 292c 2028 3132 2c20 3138 2929 220a 2020  ), (12, 18))".  
+00017a10: 2020 2020 2020 2020 2020 2020 2020 2520                % 
+00017a20: 2822 5641 4c55 4553 2022 2069 6620 636f  ("VALUES " if co
+00017a30: 6e66 6967 2e64 622e 6469 616c 6563 742e  nfig.db.dialect.
+00017a40: 7475 706c 655f 696e 5f76 616c 7565 7320  tuple_in_values 
+00017a50: 656c 7365 2022 2229 2c0a 2020 2020 2020  else ""),.      
+00017a60: 2020 2020 2020 2020 2020 2829 2069 6620            () if 
+00017a70: 636f 6e66 6967 2e64 622e 6469 616c 6563  config.db.dialec
+00017a80: 742e 706f 7369 7469 6f6e 616c 2065 6c73  t.positional els
+00017a90: 6520 7b7d 2c0a 2020 2020 2020 2020 2020  e {},.          
+00017aa0: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+00017ab0: 2020 2040 7465 7374 696e 672e 7265 7175     @testing.requ
+00017ac0: 6972 6573 2e74 7570 6c65 5f69 6e0a 2020  ires.tuple_in.  
+00017ad0: 2020 6465 6620 7465 7374 5f65 7865 6375    def test_execu
+00017ae0: 7465 5f74 7570 6c65 5f65 7870 616e 6469  te_tuple_expandi
+00017af0: 6e67 5f70 6c75 735f 6c69 7465 7261 6c5f  ng_plus_literal_
+00017b00: 6865 7465 726f 6765 6e65 6f75 735f 6578  heterogeneous_ex
+00017b10: 6563 7574 6528 7365 6c66 293a 0a20 2020  ecute(self):.   
+00017b20: 2020 2020 2074 6162 6c65 203d 2073 656c       table = sel
+00017b30: 662e 7461 626c 6573 2e73 6f6d 655f 7461  f.tables.some_ta
+00017b40: 626c 650a 0a20 2020 2020 2020 2073 746d  ble..        stm
+00017b50: 7420 3d20 7365 6c65 6374 2874 6162 6c65  t = select(table
+00017b60: 2e63 2e69 6429 2e77 6865 7265 280a 2020  .c.id).where(.  
+00017b70: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
+00017b80: 6865 6d79 2e74 7570 6c65 5f28 7461 626c  hemy.tuple_(tabl
+00017b90: 652e 632e 782c 2074 6162 6c65 2e63 2e7a  e.c.x, table.c.z
+00017ba0: 292e 696e 5f28 0a20 2020 2020 2020 2020  ).in_(.         
+00017bb0: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
+00017bc0: 792e 6269 6e64 7061 7261 6d28 2271 222c  y.bindparam("q",
+00017bd0: 2065 7870 616e 6469 6e67 3d54 7275 652c   expanding=True,
+00017be0: 206c 6974 6572 616c 5f65 7865 6375 7465   literal_execute
+00017bf0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00017c00: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
+00017c10: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00017c20: 662e 7371 6c5f 6578 6563 7574 696f 6e5f  f.sql_execution_
+00017c30: 6173 7365 7274 6572 2829 2061 7320 6173  asserter() as as
+00017c40: 7365 7274 6572 3a0a 2020 2020 2020 2020  serter:.        
+00017c50: 2020 2020 7769 7468 2063 6f6e 6669 672e      with config.
+00017c60: 6462 2e63 6f6e 6e65 6374 2829 2061 7320  db.connect() as 
+00017c70: 636f 6e6e 3a0a 2020 2020 2020 2020 2020  conn:.          
+00017c80: 2020 2020 2020 636f 6e6e 2e65 7865 6375        conn.execu
+00017c90: 7465 2873 746d 742c 2064 6963 7428 713d  te(stmt, dict(q=
+00017ca0: 5b28 352c 2022 7a31 2229 2c20 2831 322c  [(5, "z1"), (12,
+00017cb0: 2022 7a33 2229 5d29 290a 0a20 2020 2020   "z3")]))..     
+00017cc0: 2020 2061 7373 6572 7465 722e 6173 7365     asserter.asse
+00017cd0: 7274 5f28 0a20 2020 2020 2020 2020 2020  rt_(.           
+00017ce0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00017cf0: 696e 672e 6173 7365 7274 7371 6c2e 4375  ing.assertsql.Cu
+00017d00: 7273 6f72 5351 4c28 0a20 2020 2020 2020  rsorSQL(.       
+00017d10: 2020 2020 2020 2020 2022 5345 4c45 4354           "SELECT
+00017d20: 2073 6f6d 655f 7461 626c 652e 6964 205c   some_table.id \
+00017d30: 6e46 524f 4d20 736f 6d65 5f74 6162 6c65  nFROM some_table
+00017d40: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00017d50: 2020 2022 5c6e 5748 4552 4520 2873 6f6d     "\nWHERE (som
+00017d60: 655f 7461 626c 652e 782c 2073 6f6d 655f  e_table.x, some_
+00017d70: 7461 626c 652e 7a29 2022 0a20 2020 2020  table.z) ".     
+00017d80: 2020 2020 2020 2020 2020 2022 494e 2028             "IN (
+00017d90: 2573 2835 2c20 277a 3127 292c 2028 3132  %s(5, 'z1'), (12
+00017da0: 2c20 277a 3327 2929 220a 2020 2020 2020  , 'z3'))".      
+00017db0: 2020 2020 2020 2020 2020 2520 2822 5641            % ("VA
+00017dc0: 4c55 4553 2022 2069 6620 636f 6e66 6967  LUES " if config
+00017dd0: 2e64 622e 6469 616c 6563 742e 7475 706c  .db.dialect.tupl
+00017de0: 655f 696e 5f76 616c 7565 7320 656c 7365  e_in_values else
+00017df0: 2022 2229 2c0a 2020 2020 2020 2020 2020   ""),.          
+00017e00: 2020 2020 2020 2829 2069 6620 636f 6e66        () if conf
+00017e10: 6967 2e64 622e 6469 616c 6563 742e 706f  ig.db.dialect.po
+00017e20: 7369 7469 6f6e 616c 2065 6c73 6520 7b7d  sitional else {}
+00017e30: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00017e40: 2020 2020 2020 2020 290a 0a0a 4070 7974          )...@pyt
+00017e50: 6573 742e 6d61 726b 2e73 6b69 7069 6628  est.mark.skipif(
+00017e60: 0a20 2020 2062 6f6f 6c28 6f73 2e65 6e76  .    bool(os.env
+00017e70: 6972 6f6e 2e67 6574 2822 5350 414e 4e45  iron.get("SPANNE
+00017e80: 525f 454d 554c 4154 4f52 5f48 4f53 5422  R_EMULATOR_HOST"
+00017e90: 2929 2c20 7265 6173 6f6e 3d22 536b 6970  )), reason="Skip
+00017ea0: 7065 6420 6f6e 2065 6d75 6c61 746f 7222  ped on emulator"
+00017eb0: 0a29 0a63 6c61 7373 204a 534f 4e54 6573  .).class JSONTes
+00017ec0: 7428 5f4a 534f 4e54 6573 7429 3a0a 2020  t(_JSONTest):.  
+00017ed0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00017ee0: 6b69 7028 2256 616c 7565 7320 7769 7468  kip("Values with
+00017ef0: 6f75 7420 6b65 7973 2061 7265 206e 6f74  out keys are not
+00017f00: 2073 7570 706f 7274 6564 2e22 290a 2020   supported.").  
+00017f10: 2020 6465 6620 7465 7374 5f73 696e 676c    def test_singl
+00017f20: 655f 656c 656d 656e 745f 726f 756e 645f  e_element_round_
+00017f30: 7472 6970 2873 656c 662c 2065 6c65 6d65  trip(self, eleme
+00017f40: 6e74 293a 0a20 2020 2020 2020 2070 6173  nt):.        pas
+00017f50: 730a 0a20 2020 2064 6566 205f 7465 7374  s..    def _test
+00017f60: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
+00017f70: 2c20 6461 7461 5f65 6c65 6d65 6e74 2c20  , data_element, 
+00017f80: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
+00017f90: 2020 2020 2064 6174 615f 7461 626c 6520       data_table 
+00017fa0: 3d20 7365 6c66 2e74 6162 6c65 732e 6461  = self.tables.da
+00017fb0: 7461 5f74 6162 6c65 0a0a 2020 2020 2020  ta_table..      
+00017fc0: 2020 636f 6e6e 6563 7469 6f6e 2e65 7865    connection.exe
+00017fd0: 6375 7465 280a 2020 2020 2020 2020 2020  cute(.          
+00017fe0: 2020 6461 7461 5f74 6162 6c65 2e69 6e73    data_table.ins
+00017ff0: 6572 7428 292c 0a20 2020 2020 2020 2020  ert(),.         
+00018000: 2020 207b 2269 6422 3a20 7261 6e64 6f6d     {"id": random
+00018010: 2e72 616e 6469 6e74 2831 2c20 3130 3030  .randint(1, 1000
+00018020: 3030 3030 3029 2c20 226e 616d 6522 3a20  00000), "name": 
+00018030: 2272 6f77 3122 2c20 2264 6174 6122 3a20  "row1", "data": 
+00018040: 6461 7461 5f65 6c65 6d65 6e74 7d2c 0a20  data_element},. 
+00018050: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00018060: 2020 726f 7720 3d20 636f 6e6e 6563 7469    row = connecti
+00018070: 6f6e 2e65 7865 6375 7465 2873 656c 6563  on.execute(selec
+00018080: 7428 6461 7461 5f74 6162 6c65 2e63 2e64  t(data_table.c.d
+00018090: 6174 6129 292e 6669 7273 7428 290a 0a20  ata)).first().. 
+000180a0: 2020 2020 2020 2065 715f 2872 6f77 2c20         eq_(row, 
+000180b0: 2864 6174 615f 656c 656d 656e 742c 2929  (data_element,))
+000180c0: 0a0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
+000180d0: 6e69 636f 6465 5f72 6f75 6e64 5f74 7269  nicode_round_tri
+000180e0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000180f0: 2023 206e 6f74 6520 7765 2069 6e63 6c75   # note we inclu
+00018100: 6465 2055 6e69 636f 6465 2073 7570 706c  de Unicode suppl
+00018110: 656d 656e 7461 7279 2063 6861 7261 6374  ementary charact
+00018120: 6572 7320 6173 2077 656c 6c0a 2020 2020  ers as well.    
+00018130: 2020 2020 7769 7468 2063 6f6e 6669 672e      with config.
+00018140: 6462 2e63 6f6e 6e65 6374 2829 2061 7320  db.connect() as 
+00018150: 636f 6e6e 3a0a 2020 2020 2020 2020 2020  conn:.          
+00018160: 2020 636f 6e6e 2e65 7865 6375 7465 280a    conn.execute(.
+00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018180: 7365 6c66 2e74 6162 6c65 732e 6461 7461  self.tables.data
+00018190: 5f74 6162 6c65 2e69 6e73 6572 7428 292c  _table.insert(),
+000181a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000181b0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000181c0: 2020 2020 2020 2022 6964 223a 2072 616e         "id": ran
+000181d0: 646f 6d2e 7261 6e64 696e 7428 312c 2031  dom.randint(1, 1
+000181e0: 3030 3030 3030 3030 292c 0a20 2020 2020  00000000),.     
+000181f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00018200: 6e61 6d65 223a 2022 7231 222c 0a20 2020  name": "r1",.   
+00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018220: 2022 6461 7461 223a 207b 0a20 2020 2020   "data": {.     
+00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018240: 2020 2022 72c3 a976 65f0 9f90 8d20 696c     "r..ve.... il
+00018250: 6cc3 a922 3a20 2272 c3a9 7665 f09f 908d  l..": "r..ve....
+00018260: 2069 6c6c c3a9 222c 0a20 2020 2020 2020   ill..",.       
+00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018280: 2022 6461 7461 223a 207b 226b 3122 3a20   "data": {"k1": 
+00018290: 2264 72c3 b46c f09f 908d 6522 7d2c 0a20  "dr..l....e"},. 
+000182a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182b0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+000182c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000182d0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000182e0: 2020 2020 6571 5f28 0a20 2020 2020 2020      eq_(.       
+000182f0: 2020 2020 2020 2020 2063 6f6e 6e2e 7363           conn.sc
+00018300: 616c 6172 2873 656c 6563 7428 7365 6c66  alar(select(self
+00018310: 2e74 6162 6c65 732e 6461 7461 5f74 6162  .tables.data_tab
+00018320: 6c65 2e63 2e64 6174 6129 292c 0a20 2020  le.c.data)),.   
+00018330: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018350: 2020 2022 72c3 a976 65f0 9f90 8d20 696c     "r..ve.... il
+00018360: 6cc3 a922 3a20 2272 c3a9 7665 f09f 908d  l..": "r..ve....
+00018370: 2069 6c6c c3a9 222c 0a20 2020 2020 2020   ill..",.       
+00018380: 2020 2020 2020 2020 2020 2020 2022 6461               "da
+00018390: 7461 223a 207b 226b 3122 3a20 2264 72c3  ta": {"k1": "dr.
+000183a0: b46c f09f 908d 6522 7d2c 0a20 2020 2020  .l....e"},.     
+000183b0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000183c0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000183d0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+000183e0: 6970 2822 5061 7261 6d65 7465 7269 7a65  ip("Parameterize
+000183f0: 6420 7479 7065 7320 6172 6520 6e6f 7420  d types are not 
+00018400: 7375 7070 6f72 7465 642e 2229 0a20 2020  supported.").   
+00018410: 2064 6566 2074 6573 745f 6576 616c 5f6e   def test_eval_n
+00018420: 6f6e 655f 666c 6167 5f6f 726d 2873 656c  one_flag_orm(sel
+00018430: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00018440: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+00018450: 726b 2e73 6b69 7028 0a20 2020 2020 2020  rk.skip(.       
+00018460: 2022 5370 616e 6e65 7220 4a53 4f4e 5f56   "Spanner JSON_V
+00018470: 414c 5545 2829 2061 6c77 6179 7320 7265  ALUE() always re
+00018480: 7475 726e 7320 5354 5249 4e47 2c22 0a20  turns STRING,". 
+00018490: 2020 2020 2020 2022 7468 7573 2c20 7468         "thus, th
+000184a0: 6973 2074 6573 7420 6361 7365 2063 616e  is test case can
+000184b0: 2774 2062 6520 6578 6563 7574 6564 2e22  't be executed."
+000184c0: 0a20 2020 2029 0a20 2020 2064 6566 2074  .    ).    def t
+000184d0: 6573 745f 696e 6465 785f 7479 7065 645f  est_index_typed_
+000184e0: 636f 6d70 6172 6973 6f6e 2873 656c 6629  comparison(self)
+000184f0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00018500: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00018510: 2e73 6b69 7028 0a20 2020 2020 2020 2022  .skip(.        "
+00018520: 5370 616e 6e65 7220 4a53 4f4e 5f56 414c  Spanner JSON_VAL
+00018530: 5545 2829 2061 6c77 6179 7320 7265 7475  UE() always retu
+00018540: 726e 7320 5354 5249 4e47 2c22 0a20 2020  rns STRING,".   
+00018550: 2020 2020 2022 7468 7573 2c20 7468 6973       "thus, this
+00018560: 2074 6573 7420 6361 7365 2063 616e 2774   test case can't
+00018570: 2062 6520 6578 6563 7574 6564 2e22 0a20   be executed.". 
+00018580: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
+00018590: 745f 7061 7468 5f74 7970 6564 5f63 6f6d  t_path_typed_com
+000185a0: 7061 7269 736f 6e28 7365 6c66 293a 0a20  parison(self):. 
+000185b0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000185c0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+000185d0: 6970 2822 4375 7374 6f6d 204a 534f 4e20  ip("Custom JSON 
+000185e0: 6465 2d2f 7365 7269 616c 697a 6572 7320  de-/serializers 
+000185f0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
+00018600: 642e 2229 0a20 2020 2064 6566 2074 6573  d.").    def tes
+00018610: 745f 726f 756e 645f 7472 6970 5f63 7573  t_round_trip_cus
+00018620: 746f 6d5f 6a73 6f6e 2873 656c 6629 3a0a  tom_json(self):.
+00018630: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00018640: 2020 6465 6620 5f69 6e64 6578 5f66 6978    def _index_fix
+00018650: 7475 7265 7328 666e 293a 0a20 2020 2020  tures(fn):.     
+00018660: 2020 2066 6e20 3d20 7465 7374 696e 672e     fn = testing.
+00018670: 636f 6d62 696e 6174 696f 6e73 280a 2020  combinations(.  
+00018680: 2020 2020 2020 2020 2020 2822 626f 6f6c            ("bool
+00018690: 6561 6e22 2c20 5472 7565 292c 0a20 2020  ean", True),.   
+000186a0: 2020 2020 2020 2020 2028 2262 6f6f 6c65           ("boole
+000186b0: 616e 222c 2046 616c 7365 292c 0a20 2020  an", False),.   
+000186c0: 2020 2020 2020 2020 2028 2262 6f6f 6c65           ("boole
+000186d0: 616e 222c 204e 6f6e 6529 2c0a 2020 2020  an", None),.    
+000186e0: 2020 2020 2020 2020 2822 7374 7269 6e67          ("string
+000186f0: 222c 2022 736f 6d65 2073 7472 696e 6722  ", "some string"
+00018700: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00018710: 2273 7472 696e 6722 2c20 4e6f 6e65 292c  "string", None),
+00018720: 0a20 2020 2020 2020 2020 2020 2028 2269  .            ("i
+00018730: 6e74 6567 6572 222c 2031 3529 2c0a 2020  nteger", 15),.  
+00018740: 2020 2020 2020 2020 2020 2822 696e 7465            ("inte
+00018750: 6765 7222 2c20 3129 2c0a 2020 2020 2020  ger", 1),.      
+00018760: 2020 2020 2020 2822 696e 7465 6765 7222        ("integer"
+00018770: 2c20 3029 2c0a 2020 2020 2020 2020 2020  , 0),.          
+00018780: 2020 2822 696e 7465 6765 7222 2c20 4e6f    ("integer", No
+00018790: 6e65 292c 0a20 2020 2020 2020 2020 2020  ne),.           
+000187a0: 2028 2266 6c6f 6174 222c 2032 382e 3529   ("float", 28.5)
+000187b0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+000187c0: 666c 6f61 7422 2c20 4e6f 6e65 292c 0a20  float", None),. 
+000187d0: 2020 2020 2020 2020 2020 2069 645f 3d22             id_="
+000187e0: 7361 222c 0a20 2020 2020 2020 2029 2866  sa",.        )(f
+000187f0: 6e29 0a20 2020 2020 2020 2072 6574 7572  n).        retur
+00018800: 6e20 666e 0a0a 2020 2020 405f 696e 6465  n fn..    @_inde
+00018810: 785f 6669 7874 7572 6573 0a20 2020 2064  x_fixtures.    d
+00018820: 6566 2074 6573 745f 696e 6465 785f 7479  ef test_index_ty
+00018830: 7065 645f 6163 6365 7373 2873 656c 662c  ped_access(self,
+00018840: 2064 6174 6174 7970 652c 2076 616c 7565   datatype, value
+00018850: 293a 0a20 2020 2020 2020 2064 6174 615f  ):.        data_
+00018860: 7461 626c 6520 3d20 7365 6c66 2e74 6162  table = self.tab
+00018870: 6c65 732e 6461 7461 5f74 6162 6c65 0a20  les.data_table. 
+00018880: 2020 2020 2020 2064 6174 615f 656c 656d         data_elem
+00018890: 656e 7420 3d20 7b22 6b65 7931 223a 2076  ent = {"key1": v
+000188a0: 616c 7565 7d0a 2020 2020 2020 2020 7769  alue}.        wi
+000188b0: 7468 2063 6f6e 6669 672e 6462 2e63 6f6e  th config.db.con
+000188c0: 6e65 6374 2829 2061 7320 636f 6e6e 3a0a  nect() as conn:.
+000188d0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+000188e0: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
+000188f0: 2020 2020 2020 2020 2020 6461 7461 5f74            data_t
+00018900: 6162 6c65 2e69 6e73 6572 7428 292c 0a20  able.insert(),. 
+00018910: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00018920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018930: 2020 2020 2022 6964 223a 2072 616e 646f       "id": rando
+00018940: 6d2e 7261 6e64 696e 7428 312c 2031 3030  m.randint(1, 100
+00018950: 3030 3030 3030 292c 0a20 2020 2020 2020  000000),.       
+00018960: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+00018970: 6d65 223a 2022 726f 7731 222c 0a20 2020  me": "row1",.   
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 2022 6461 7461 223a 2064 6174 615f 656c   "data": data_el
+000189a0: 656d 656e 742c 0a20 2020 2020 2020 2020  ement,.         
+000189b0: 2020 2020 2020 2020 2020 2022 6e75 6c6c             "null
+000189c0: 6461 7461 223a 2064 6174 615f 656c 656d  data": data_elem
+000189d0: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
+000189e0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000189f0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00018a00: 2020 2065 7870 7220 3d20 6461 7461 5f74     expr = data_t
+00018a10: 6162 6c65 2e63 2e64 6174 615b 226b 6579  able.c.data["key
+00018a20: 3122 5d0a 2020 2020 2020 2020 2020 2020  1"].            
+00018a30: 6578 7072 203d 2067 6574 6174 7472 2865  expr = getattr(e
+00018a40: 7870 722c 2022 6173 5f25 7322 2025 2064  xpr, "as_%s" % d
+00018a50: 6174 6174 7970 6529 2829 0a0a 2020 2020  atatype)()..    
+00018a60: 2020 2020 2020 2020 726f 756e 6474 7269          roundtri
+00018a70: 7020 3d20 636f 6e6e 2e73 6361 6c61 7228  p = conn.scalar(
+00018a80: 7365 6c65 6374 2865 7870 7229 290a 2020  select(expr)).  
+00018a90: 2020 2020 2020 2020 2020 6966 2072 6f75            if rou
+00018aa0: 6e64 7472 6970 2069 6e20 2822 7472 7565  ndtrip in ("true
+00018ab0: 222c 2022 6661 6c73 6522 2c20 4e6f 6e65  ", "false", None
+00018ac0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00018ad0: 2020 2072 6f75 6e64 7472 6970 203d 2073     roundtrip = s
+00018ae0: 7472 2872 6f75 6e64 7472 6970 292e 6361  tr(roundtrip).ca
+00018af0: 7069 7461 6c69 7a65 2829 0a0a 2020 2020  pitalize()..    
+00018b00: 2020 2020 2020 2020 6571 5f28 7374 7228          eq_(str(
+00018b10: 726f 756e 6474 7269 7029 2c20 7374 7228  roundtrip), str(
+00018b20: 7661 6c75 6529 290a 0a20 2020 2040 7079  value))..    @py
+00018b30: 7465 7374 2e6d 6172 6b2e 736b 6970 280a  test.mark.skip(.
+00018b40: 2020 2020 2020 2020 2253 7061 6e6e 6572          "Spanner
+00018b50: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
+00018b60: 2074 7970 6520 6361 7374 7320 696e 7369   type casts insi
+00018b70: 6465 204a 534f 4e5f 5641 4c55 4528 2920  de JSON_VALUE() 
+00018b80: 6675 6e63 7469 6f6e 2e22 0a20 2020 2029  function.".    )
+00018b90: 0a20 2020 2064 6566 2074 6573 745f 726f  .    def test_ro
+00018ba0: 756e 645f 7472 6970 5f6a 736f 6e5f 6e75  und_trip_json_nu
+00018bb0: 6c6c 5f61 735f 6a73 6f6e 5f6e 756c 6c28  ll_as_json_null(
+00018bc0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00018bd0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+00018be0: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
+00018bf0: 2020 2020 2253 7061 6e6e 6572 2064 6f65      "Spanner doe
+00018c00: 736e 2774 2073 7570 706f 7274 2074 7970  sn't support typ
+00018c10: 6520 6361 7374 7320 696e 7369 6465 204a  e casts inside J
+00018c20: 534f 4e5f 5641 4c55 4528 2920 6675 6e63  SON_VALUE() func
+00018c30: 7469 6f6e 2e22 0a20 2020 2029 0a20 2020  tion.".    ).   
+00018c40: 2064 6566 2074 6573 745f 726f 756e 645f   def test_round_
+00018c50: 7472 6970 5f6e 6f6e 655f 6173 5f6a 736f  trip_none_as_jso
+00018c60: 6e5f 6e75 6c6c 2873 656c 6629 3a0a 2020  n_null(self):.  
+00018c70: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00018c80: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00018c90: 7028 0a20 2020 2020 2020 2022 5370 616e  p(.        "Span
+00018ca0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+00018cb0: 6f72 7420 7479 7065 2063 6173 7473 2069  ort type casts i
+00018cc0: 6e73 6964 6520 4a53 4f4e 5f56 414c 5545  nside JSON_VALUE
+00018cd0: 2829 2066 756e 6374 696f 6e2e 220a 2020  () function.".  
+00018ce0: 2020 290a 2020 2020 6465 6620 7465 7374    ).    def test
+00018cf0: 5f72 6f75 6e64 5f74 7269 705f 6e6f 6e65  _round_trip_none
+00018d00: 5f61 735f 7371 6c5f 6e75 6c6c 2873 656c  _as_sql_null(sel
+00018d10: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00018d20: 0a0a 0a63 6c61 7373 2045 7865 6375 7469  ...class Executi
+00018d30: 6f6e 4f70 7469 6f6e 7352 6571 7565 7374  onOptionsRequest
+00018d40: 5072 696f 726f 7479 5465 7374 2866 6978  PriorotyTest(fix
+00018d50: 7475 7265 732e 5465 7374 4261 7365 293a  tures.TestBase):
+00018d60: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
+00018d70: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00018d80: 6c66 2e5f 656e 6769 6e65 203d 2063 7265  lf._engine = cre
+00018d90: 6174 655f 656e 6769 6e65 2867 6574 5f64  ate_engine(get_d
+00018da0: 625f 7572 6c28 292c 2070 6f6f 6c5f 7369  b_url(), pool_si
+00018db0: 7a65 3d31 290a 2020 2020 2020 2020 6d65  ze=1).        me
+00018dc0: 7461 6461 7461 203d 204d 6574 6144 6174  tadata = MetaDat
+00018dd0: 6128 290a 0a20 2020 2020 2020 2073 656c  a()..        sel
+00018de0: 662e 5f74 6162 6c65 203d 2054 6162 6c65  f._table = Table
+00018df0: 280a 2020 2020 2020 2020 2020 2020 2265  (.            "e
+00018e00: 7865 6375 7469 6f6e 5f6f 7074 696f 6e73  xecution_options
+00018e10: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+00018e20: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00018e30: 2020 2020 2020 436f 6c75 6d6e 2822 6f70        Column("op
+00018e40: 745f 6964 222c 2049 6e74 6567 6572 2c20  t_id", Integer, 
+00018e50: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
+00018e60: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+00018e70: 6f6c 756d 6e28 226f 7074 5f6e 616d 6522  olumn("opt_name"
+00018e80: 2c20 5374 7269 6e67 2831 3629 2c20 6e75  , String(16), nu
+00018e90: 6c6c 6162 6c65 3d46 616c 7365 292c 0a20  llable=False),. 
+00018ea0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00018eb0: 2020 6d65 7461 6461 7461 2e63 7265 6174    metadata.creat
+00018ec0: 655f 616c 6c28 7365 6c66 2e5f 656e 6769  e_all(self._engi
+00018ed0: 6e65 290a 2020 2020 2020 2020 7469 6d65  ne).        time
+00018ee0: 2e73 6c65 6570 2831 290a 0a20 2020 2064  .sleep(1)..    d
+00018ef0: 6566 2074 6573 745f 7265 7175 6573 745f  ef test_request_
+00018f00: 7072 696f 7269 7479 2873 656c 6629 3a0a  priority(self):.
+00018f10: 2020 2020 2020 2020 5052 494f 5249 5459          PRIORITY
+00018f20: 203d 2052 6571 7565 7374 4f70 7469 6f6e   = RequestOption
+00018f30: 732e 5072 696f 7269 7479 2e50 5249 4f52  s.Priority.PRIOR
+00018f40: 4954 595f 4d45 4449 554d 0a20 2020 2020  ITY_MEDIUM.     
+00018f50: 2020 2077 6974 6820 7365 6c66 2e5f 656e     with self._en
+00018f60: 6769 6e65 2e63 6f6e 6e65 6374 2829 2e65  gine.connect().e
+00018f70: 7865 6375 7469 6f6e 5f6f 7074 696f 6e73  xecution_options
+00018f80: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+00018f90: 7175 6573 745f 7072 696f 7269 7479 3d50  quest_priority=P
+00018fa0: 5249 4f52 4954 590a 2020 2020 2020 2020  RIORITY.        
+00018fb0: 2920 6173 2063 6f6e 6e65 6374 696f 6e3a  ) as connection:
+00018fc0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00018fd0: 6e65 6374 696f 6e2e 6578 6563 7574 6528  nection.execute(
+00018fe0: 7365 6c65 6374 2873 656c 662e 5f74 6162  select(self._tab
+00018ff0: 6c65 2929 2e66 6574 6368 616c 6c28 290a  le)).fetchall().
+00019000: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00019010: 6c66 2e5f 656e 6769 6e65 2e63 6f6e 6e65  lf._engine.conne
+00019020: 6374 2829 2061 7320 636f 6e6e 6563 7469  ct() as connecti
+00019030: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00019040: 6173 7365 7274 2063 6f6e 6e65 6374 696f  assert connectio
+00019050: 6e2e 636f 6e6e 6563 7469 6f6e 2e72 6571  n.connection.req
+00019060: 7565 7374 5f70 7269 6f72 6974 7920 6973  uest_priority is
+00019070: 204e 6f6e 650a 0a20 2020 2020 2020 2065   None..        e
+00019080: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
+00019090: 6e67 696e 6528 2273 716c 6974 653a 2f2f  ngine("sqlite://
+000190a0: 2f64 6174 6162 6173 6522 290a 2020 2020  /database").    
+000190b0: 2020 2020 7769 7468 2065 6e67 696e 652e      with engine.
+000190c0: 636f 6e6e 6563 7428 2920 6173 2063 6f6e  connect() as con
+000190d0: 6e65 6374 696f 6e3a 0a20 2020 2020 2020  nection:.       
+000190e0: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
+000190f0: 7320 4372 6561 7465 456e 6769 6e65 5769  s CreateEngineWi
+00019100: 7468 436c 6965 6e74 4f62 6a65 6374 5465  thClientObjectTe
+00019110: 7374 2866 6978 7475 7265 732e 5465 7374  st(fixtures.Test
+00019120: 4261 7365 293a 0a20 2020 2064 6566 2074  Base):.    def t
+00019130: 6573 745f 6372 6561 7465 5f65 6e67 696e  est_create_engin
+00019140: 655f 775f 7661 6c69 645f 636c 6965 6e74  e_w_valid_client
+00019150: 5f6f 626a 6563 7428 7365 6c66 293a 0a20  _object(self):. 
+00019160: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00019170: 2020 2053 5041 4e4e 4552 2054 4553 543a     SPANNER TEST:
+00019180: 0a0a 2020 2020 2020 2020 4368 6563 6b20  ..        Check 
+00019190: 7468 6174 2077 6520 6361 6e20 636f 6e6e  that we can conn
+000191a0: 6563 7420 746f 2053 716c 416c 6368 656d  ect to SqlAlchem
+000191b0: 790a 2020 2020 2020 2020 6279 2070 6173  y.        by pas
+000191c0: 7369 6e67 2063 7573 746f 6d20 436c 6965  sing custom Clie
+000191d0: 6e74 206f 626a 6563 742e 0a20 2020 2020  nt object..     
+000191e0: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
+000191f0: 6c69 656e 7420 3d20 436c 6965 6e74 2870  lient = Client(p
+00019200: 726f 6a65 6374 3d67 6574 5f70 726f 6a65  roject=get_proje
+00019210: 6374 2829 290a 2020 2020 2020 2020 656e  ct()).        en
+00019220: 6769 6e65 203d 2063 7265 6174 655f 656e  gine = create_en
+00019230: 6769 6e65 2867 6574 5f64 625f 7572 6c28  gine(get_db_url(
+00019240: 292c 2063 6f6e 6e65 6374 5f61 7267 733d  ), connect_args=
+00019250: 7b22 636c 6965 6e74 223a 2063 6c69 656e  {"client": clien
+00019260: 747d 290a 2020 2020 2020 2020 7769 7468  t}).        with
+00019270: 2065 6e67 696e 652e 636f 6e6e 6563 7428   engine.connect(
+00019280: 2920 6173 2063 6f6e 6e65 6374 696f 6e3a  ) as connection:
+00019290: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+000192a0: 6572 7420 636f 6e6e 6563 7469 6f6e 2e63  ert connection.c
+000192b0: 6f6e 6e65 6374 696f 6e2e 696e 7374 616e  onnection.instan
+000192c0: 6365 2e5f 636c 6965 6e74 203d 3d20 636c  ce._client == cl
+000192d0: 6965 6e74 0a0a 2020 2020 6465 6620 7465  ient..    def te
+000192e0: 7374 5f63 7265 6174 655f 656e 6769 6e65  st_create_engine
+000192f0: 5f77 5f69 6e76 616c 6964 5f63 6c69 656e  _w_invalid_clien
+00019300: 745f 6f62 6a65 6374 2873 656c 6629 3a0a  t_object(self):.
+00019310: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00019320: 2020 2020 5350 414e 4e45 5220 5445 5354      SPANNER TEST
+00019330: 3a0a 0a20 2020 2020 2020 2043 6865 636b  :..        Check
+00019340: 2074 6861 7420 6966 2070 726f 6a65 6374   that if project
+00019350: 2069 6420 696e 2075 726c 2061 6e64 2063   id in url and c
+00019360: 7573 746f 6d20 436c 6965 6e74 0a20 2020  ustom Client.   
+00019370: 2020 2020 204f 626a 6563 7420 7061 7373       Object pass
+00019380: 6564 2074 6f20 656e 6769 6e65 7220 6d69  ed to enginer mi
+00019390: 736d 6174 6368 2c20 6572 726f 7220 6973  smatch, error is
+000193a0: 2074 6872 6f77 6e2e 0a20 2020 2020 2020   thrown..       
+000193b0: 2022 2222 0a20 2020 2020 2020 2063 6c69   """.        cli
+000193c0: 656e 7420 3d20 436c 6965 6e74 2870 726f  ent = Client(pro
+000193d0: 6a65 6374 3d22 7072 6f6a 6563 745f 6964  ject="project_id
+000193e0: 2229 0a20 2020 2020 2020 2065 6e67 696e  ").        engin
+000193f0: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
+00019400: 6528 6765 745f 6462 5f75 726c 2829 2c20  e(get_db_url(), 
+00019410: 636f 6e6e 6563 745f 6172 6773 3d7b 2263  connect_args={"c
+00019420: 6c69 656e 7422 3a20 636c 6965 6e74 7d29  lient": client})
+00019430: 0a0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
+00019440: 7974 6573 742e 7261 6973 6573 2856 616c  ytest.raises(Val
+00019450: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
+00019460: 2020 2020 2020 656e 6769 6e65 2e63 6f6e        engine.con
+00019470: 6e65 6374 2829 0a0a 0a63 6c61 7373 2043  nect()...class C
+00019480: 7265 6174 6545 6e67 696e 6557 6974 686f  reateEngineWitho
+00019490: 7574 4461 7461 6261 7365 5465 7374 2866  utDatabaseTest(f
+000194a0: 6978 7475 7265 732e 5465 7374 4261 7365  ixtures.TestBase
+000194b0: 293a 0a20 2020 2064 6566 2074 6573 745f  ):.    def test_
+000194c0: 6372 6561 7465 5f65 6e67 696e 655f 776f  create_engine_wo
+000194d0: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
+000194e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000194f0: 2020 2020 2053 5041 4e4e 4552 2054 4553       SPANNER TES
+00019500: 543a 0a0a 2020 2020 2020 2020 4368 6563  T:..        Chec
+00019510: 6b20 7468 6174 2077 6520 6361 6e20 636f  k that we can co
+00019520: 6e6e 6563 7420 746f 2053 716c 416c 6368  nnect to SqlAlch
+00019530: 656d 790a 2020 2020 2020 2020 7769 7468  emy.        with
+00019540: 6f75 7420 7061 7373 696e 6720 6461 7461  out passing data
+00019550: 6261 7365 2069 6420 696e 2074 6865 0a20  base id in the. 
+00019560: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+00019570: 6e20 5552 4c2e 0a20 2020 2020 2020 2022  n URL..        "
+00019580: 2222 0a20 2020 2020 2020 2065 6e67 696e  "".        engin
+00019590: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
+000195a0: 6528 6765 745f 6462 5f75 726c 2829 2e73  e(get_db_url().s
+000195b0: 706c 6974 2822 2f64 6174 6162 6173 6522  plit("/database"
+000195c0: 295b 305d 290a 2020 2020 2020 2020 7769  )[0]).        wi
+000195d0: 7468 2065 6e67 696e 652e 636f 6e6e 6563  th engine.connec
+000195e0: 7428 2920 6173 2063 6f6e 6e65 6374 696f  t() as connectio
+000195f0: 6e3a 0a20 2020 2020 2020 2020 2020 2061  n:.            a
+00019600: 7373 6572 7420 636f 6e6e 6563 7469 6f6e  ssert connection
+00019610: 2e63 6f6e 6e65 6374 696f 6e2e 6461 7461  .connection.data
+00019620: 6261 7365 2069 7320 4e6f 6e65 0a         base is None.
```

