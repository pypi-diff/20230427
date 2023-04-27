# Comparing `tmp/questdb-connect-0.0.22.tar.gz` & `tmp/questdb-connect-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.22.tar", last modified: Wed Apr 26 18:19:41 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.23.tar", last modified: Thu Apr 27 10:13:52 2023, max compression
```

## Comparing `questdb-connect-0.0.22.tar` & `questdb-connect-0.0.23.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.824389 questdb-connect-0.0.22/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.22/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 18:19:41.824229 questdb-connect-0.0.22/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.22/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2432 2023-04-26 18:19:28.000000 questdb-connect-0.0.22/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-26 18:19:41.824430 questdb-connect-0.0.22/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.820330 questdb-connect-0.0.22/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.822026 questdb-connect-0.0.22/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.22/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     9849 2023-04-26 18:19:28.000000 questdb-connect-0.0.22/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     8316 2023-04-26 17:38:03.000000 questdb-connect-0.0.22/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.22/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.823027 questdb-connect-0.0.22/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      488 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.823818 questdb-connect-0.0.22/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.22/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.22/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.22/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.269573 questdb-connect-0.0.23/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.23/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 10:13:52.269387 questdb-connect-0.0.23/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.23/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2446 2023-04-27 10:13:29.000000 questdb-connect-0.0.23/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-27 10:13:52.269622 questdb-connect-0.0.23/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.259447 questdb-connect-0.0.23/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.261652 questdb-connect-0.0.23/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.23/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9841 2023-04-27 09:01:14.000000 questdb-connect-0.0.23/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.23/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9816 2023-04-27 10:07:30.000000 questdb-connect-0.0.23/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.23/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.267125 questdb-connect-0.0.23/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-27 10:13:52.000000 questdb-connect-0.0.23/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-27 10:13:52.268805 questdb-connect-0.0.23/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.23/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.23/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.23/tests/test_types.py
```

### Comparing `questdb-connect-0.0.22/LICENSE` & `questdb-connect-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.22/PKG-INFO` & `questdb-connect-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.22
+Version: 0.0.23
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.22/README.md` & `questdb-connect-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.22/pyproject.toml` & `questdb-connect-0.0.23/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.22"
+version = "0.0.23"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -70,12 +70,13 @@
     ".ruff_cache",
     "venv",
     "questdb_connect.egg-info",
 ]
 
 [tool.ruff.pylint]
 max-branches = 20
+max-args = 10
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
```

### Comparing `questdb-connect-0.0.22/src/questdb_connect/__init__.py` & `questdb-connect-0.0.23/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.22/src/questdb_connect/dialect.py` & `questdb-connect-0.0.23/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from questdb_connect.types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
-
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
@@ -48,15 +47,15 @@
 
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
             table_name: str,
-            ts_col_name: str = None,
+            ts_col_name: str,
             partition_by: PartitionBy = PartitionBy.DAY,
             is_wal: bool = True
     ):
         Traversible.__init__(self)
         self.name = table_name
         self.ts_col_name = ts_col_name
         self.partition_by = partition_by
```

### Comparing `questdb-connect-0.0.22/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.23/src/questdb_connect/superset_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
 from questdb_connect import types
+from questdb_connect.function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
@@ -42,14 +43,15 @@
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
     time_secondary_columns = True
     max_column_name_length = 120
+    try_remove_schema_from_table_name = True
     _time_grain_expressions = {
         None: '{col}',
         'PT1S': "date_trunc('second', {col})",
         'PT5S': "date_trunc('second', {col}) + 5000000",
         'PT30S': "date_trunc('second', {col}) + 30000000",
         'PT1M': "date_trunc('minute', {col})",
         'PT5M': "date_trunc('minute', {col}) + 300000000",
@@ -105,15 +107,14 @@
         return '{col} * 1000000'
 
     @classmethod
     def convert_dttm(cls, target_type: str, dttm: datetime, *_args, **_kwargs) -> Optional[str]:
         """Convert a Python `datetime` object to a SQL expression.
         :param target_type: The target type of expression
         :param dttm: The datetime object
-        :param db_extra: The database extra object
         :return: The SQL expression
         """
         type_u = target_type.upper()
         if type_u == 'DATE':
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if type_u in ('DATETIME', 'TIMESTAMP'):
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
@@ -181,7 +182,43 @@
         elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
             generic_type = GenericDataType.STRING
         return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
 
     @classmethod
     def column_datatype_to_string(cls, sqla_column_type: TypeEngine, *_args):
         return sqla_column_type.__visit_name__
+
+    @classmethod
+    def select_star(
+            cls,
+            database,
+            table_name: str,
+            engine,
+            schema: Optional[str] = None,
+            limit: int = 100,
+            show_cols: bool = False,
+            indent: bool = True,
+            latest_partition: bool = True,
+            cols: Optional[List[Dict[str, Any]]] = None,
+    ) -> str:
+        """Generate a "SELECT * from table_name" query with appropriate limit.
+        :param database: Database instance
+        :param table_name: Table name, unquoted
+        :param engine: SqlAlchemy Engine instance
+        :param schema: Schema, unquoted
+        :param limit: limit to impose on query
+        :param show_cols: Show columns in query; otherwise use "*"
+        :param indent: Add indentation to query
+        :param latest_partition: Only query the latest partition
+        :param cols: Columns to include in query
+        :return: SQL query
+        """
+        return super().select_star(database, table_name, engine, None, limit, show_cols, indent, latest_partition, cols)
+
+    @classmethod
+    def get_function_names(cls, database) -> List[str]:
+        """Get a list of function names that are able to be called on the database.
+        Used for SQL Lab autocomplete.
+        :param database: The database to get functions for
+        :return: A list of function names usable in the database
+        """
+        return FUNCTION_NAMES
```

### Comparing `questdb-connect-0.0.22/src/questdb_connect/types.py` & `questdb-connect-0.0.23/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.22/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.23/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.22
+Version: 0.0.23
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.22/tests/test_dialect.py` & `questdb-connect-0.0.23/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.22/tests/test_superset.py` & `questdb-connect-0.0.23/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.22/tests/test_types.py` & `questdb-connect-0.0.23/tests/test_types.py`

 * *Files identical despite different names*

