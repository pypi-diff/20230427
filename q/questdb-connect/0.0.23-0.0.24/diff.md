# Comparing `tmp/questdb-connect-0.0.23.tar.gz` & `tmp/questdb-connect-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.23.tar", last modified: Thu Apr 27 10:13:52 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.24.tar", last modified: Thu Apr 27 10:40:34 2023, max compression
```

## Comparing `questdb-connect-0.0.23.tar` & `questdb-connect-0.0.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.269573 questdb-connect-0.0.23/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.23/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 10:13:52.269387 questdb-connect-0.0.23/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.23/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2446 2023-04-27 10:13:29.000000 questdb-connect-0.0.23/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-27 10:13:52.269622 questdb-connect-0.0.23/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.259447 questdb-connect-0.0.23/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.261652 questdb-connect-0.0.23/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.23/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     9841 2023-04-27 09:01:14.000000 questdb-connect-0.0.23/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.23/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     9816 2023-04-27 10:07:30.000000 questdb-connect-0.0.23/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.23/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.267125 questdb-connect-0.0.23/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.268805 questdb-connect-0.0.23/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.23/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.23/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.23/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:40:34.698472 questdb-connect-0.0.24/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.24/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 10:40:34.698341 questdb-connect-0.0.24/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.24/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2446 2023-04-27 10:40:23.000000 questdb-connect-0.0.24/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-27 10:40:34.698513 questdb-connect-0.0.24/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:40:34.694607 questdb-connect-0.0.24/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:40:34.696497 questdb-connect-0.0.24/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.24/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10187 2023-04-27 10:40:05.000000 questdb-connect-0.0.24/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.24/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9816 2023-04-27 10:07:30.000000 questdb-connect-0.0.24/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.24/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:40:34.697431 questdb-connect-0.0.24/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 10:40:34.000000 questdb-connect-0.0.24/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-04-27 10:40:34.000000 questdb-connect-0.0.24/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-27 10:40:34.000000 questdb-connect-0.0.24/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-27 10:40:34.000000 questdb-connect-0.0.24/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-27 10:40:34.000000 questdb-connect-0.0.24/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-27 10:40:34.000000 questdb-connect-0.0.24/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:40:34.698070 questdb-connect-0.0.24/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.24/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.24/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.24/tests/test_types.py
```

### Comparing `questdb-connect-0.0.23/LICENSE` & `questdb-connect-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/PKG-INFO` & `questdb-connect-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.23
+Version: 0.0.24
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.23/README.md` & `questdb-connect-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/pyproject.toml` & `questdb-connect-0.0.24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.23"
+version = "0.0.24"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.23/src/questdb_connect/__init__.py` & `questdb-connect-0.0.24/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/src/questdb_connect/dialect.py` & `questdb-connect-0.0.24/src/questdb_connect/dialect.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,23 +91,37 @@
 def _none(_ignore):
     return None
 
 
 class QDBIdentifierPreparer(IdentifierPreparer, abc.ABC):
     schema_for_object = staticmethod(_none)
 
+    def __init__(
+            self,
+            dialect,
+            initial_quote='"',
+            final_quote=None,
+            escape_quote='"',
+            quote_case_sensitive_collations=True,
+            omit_schema=False,
+    ):
+        super().__init__(
+            dialect,
+            "'",
+            final_quote,
+            "'",
+            quote_case_sensitive_collations,
+            True)
+
     def quote_identifier(self, value):
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
         return True
 
-    def schema_for_object(self, _obj):
-        return None
-
 
 class QDBDDLCompiler(DDLCompiler, abc.ABC):
     def visit_create_schema(self, create, **kw):
         raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
 
     def visit_drop_schema(self, drop, **kw):
         raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
```

### Comparing `questdb-connect-0.0.23/src/questdb_connect/function_names.py` & `questdb-connect-0.0.24/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.24/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/src/questdb_connect/types.py` & `questdb-connect-0.0.24/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.24/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.23
+Version: 0.0.24
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.23/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.24/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/tests/test_dialect.py` & `questdb-connect-0.0.24/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/tests/test_superset.py` & `questdb-connect-0.0.24/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.23/tests/test_types.py` & `questdb-connect-0.0.24/tests/test_types.py`

 * *Files identical despite different names*

