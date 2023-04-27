# Comparing `tmp/dbbot-sql-0.1.tar.gz` & `tmp/dbbot-sql-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbbot-sql-0.1.tar", last modified: Thu Sep 15 15:11:06 2022, max compression
+gzip compressed data, was "dbbot-sql-0.2.tar", last modified: Thu Apr 27 10:17:05 2023, max compression
```

## Comparing `dbbot-sql-0.1.tar` & `dbbot-sql-0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2022-09-15 15:11:06.240082 dbbot-sql-0.1/
--rw-r--r--   0 irfanmaulana   (501) staff       (20)    11358 2022-09-15 15:06:04.000000 dbbot-sql-0.1/LICENSE.txt
--rw-r--r--   0 irfanmaulana   (501) staff       (20)       31 2022-09-15 15:06:04.000000 dbbot-sql-0.1/MANIFEST.in
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     6912 2022-09-15 15:11:06.239941 dbbot-sql-0.1/PKG-INFO
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     6192 2022-09-15 15:06:04.000000 dbbot-sql-0.1/README.rst
-drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2022-09-15 15:11:06.238118 dbbot-sql-0.1/dbbot/
--rw-r--r--   0 irfanmaulana   (501) staff       (20)      656 2022-09-15 15:06:58.000000 dbbot-sql-0.1/dbbot/__init__.py
--rw-r--r--   0 irfanmaulana   (501) staff       (20)      650 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/__main__.py
--rw-r--r--   0 irfanmaulana   (501) staff       (20)      866 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/logger.py
-drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2022-09-15 15:11:06.238970 dbbot-sql-0.1/dbbot/reader/
--rw-r--r--   0 irfanmaulana   (501) staff       (20)      746 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/reader/__init__.py
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     9240 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/reader/database_writer.py
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     3476 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/reader/reader_options.py
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     9598 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/reader/robot_results_parser.py
--rwxr-xr-x   0 irfanmaulana   (501) staff       (20)     1811 2022-09-15 15:05:32.000000 dbbot-sql-0.1/dbbot/run.py
-drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2022-09-15 15:11:06.239747 dbbot-sql-0.1/dbbot_sql.egg-info/
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     6912 2022-09-15 15:11:06.000000 dbbot-sql-0.1/dbbot_sql.egg-info/PKG-INFO
--rw-r--r--   0 irfanmaulana   (501) staff       (20)      397 2022-09-15 15:11:06.000000 dbbot-sql-0.1/dbbot_sql.egg-info/SOURCES.txt
--rw-r--r--   0 irfanmaulana   (501) staff       (20)        1 2022-09-15 15:11:06.000000 dbbot-sql-0.1/dbbot_sql.egg-info/dependency_links.txt
--rw-r--r--   0 irfanmaulana   (501) staff       (20)       26 2022-09-15 15:11:06.000000 dbbot-sql-0.1/dbbot_sql.egg-info/requires.txt
--rw-r--r--   0 irfanmaulana   (501) staff       (20)        6 2022-09-15 15:11:06.000000 dbbot-sql-0.1/dbbot_sql.egg-info/top_level.txt
--rw-r--r--   0 irfanmaulana   (501) staff       (20)       38 2022-09-15 15:11:06.240135 dbbot-sql-0.1/setup.cfg
--rw-r--r--   0 irfanmaulana   (501) staff       (20)     1374 2022-09-15 15:06:53.000000 dbbot-sql-0.1/setup.py
+drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2023-04-27 10:17:05.901260 dbbot-sql-0.2/
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)    11358 2022-09-15 15:06:04.000000 dbbot-sql-0.2/LICENSE.txt
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)       31 2022-09-15 15:06:04.000000 dbbot-sql-0.2/MANIFEST.in
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     6912 2023-04-27 10:17:05.901128 dbbot-sql-0.2/PKG-INFO
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     6192 2022-09-15 15:06:04.000000 dbbot-sql-0.2/README.rst
+drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2023-04-27 10:17:05.899043 dbbot-sql-0.2/dbbot/
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)      656 2023-04-27 10:16:42.000000 dbbot-sql-0.2/dbbot/__init__.py
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)      650 2022-09-15 15:05:32.000000 dbbot-sql-0.2/dbbot/__main__.py
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)      866 2022-09-15 15:05:32.000000 dbbot-sql-0.2/dbbot/logger.py
+drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2023-04-27 10:17:05.900032 dbbot-sql-0.2/dbbot/reader/
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)      746 2022-09-15 15:05:32.000000 dbbot-sql-0.2/dbbot/reader/__init__.py
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     9272 2023-04-27 09:58:55.000000 dbbot-sql-0.2/dbbot/reader/database_writer.py
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     3476 2022-09-15 15:05:32.000000 dbbot-sql-0.2/dbbot/reader/reader_options.py
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     9598 2023-04-27 08:57:16.000000 dbbot-sql-0.2/dbbot/reader/robot_results_parser.py
+-rwxr-xr-x   0 irfanmaulana   (501) staff       (20)     1811 2023-04-27 08:01:14.000000 dbbot-sql-0.2/dbbot/run.py
+drwxr-xr-x   0 irfanmaulana   (501) staff       (20)        0 2023-04-27 10:17:05.900945 dbbot-sql-0.2/dbbot_sql.egg-info/
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     6912 2023-04-27 10:17:05.000000 dbbot-sql-0.2/dbbot_sql.egg-info/PKG-INFO
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)      397 2023-04-27 10:17:05.000000 dbbot-sql-0.2/dbbot_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)        1 2023-04-27 10:17:05.000000 dbbot-sql-0.2/dbbot_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)       26 2023-04-27 10:17:05.000000 dbbot-sql-0.2/dbbot_sql.egg-info/requires.txt
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)        6 2023-04-27 10:17:05.000000 dbbot-sql-0.2/dbbot_sql.egg-info/top_level.txt
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)       38 2023-04-27 10:17:05.901300 dbbot-sql-0.2/setup.cfg
+-rw-r--r--   0 irfanmaulana   (501) staff       (20)     1374 2022-09-15 15:06:53.000000 dbbot-sql-0.2/setup.py
```

### Comparing `dbbot-sql-0.1/LICENSE.txt` & `dbbot-sql-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/PKG-INFO` & `dbbot-sql-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbbot-sql
-Version: 0.1
+Version: 0.2
 Summary: A tool for inserting Robot Framework test run results into SQL database using SQLAlchemy.
 Home-page: https://github.com/pbylicki/DbBot-SQLAlchemy
 Download-URL: https://pypi.python.org/pypi/dbbot-sql
 Author: Robot Framework Developers, Pawel Bylicki
 Author-email: robotframework@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation atdd
```

### Comparing `dbbot-sql-0.1/README.rst` & `dbbot-sql-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot/__init__.py` & `dbbot-sql-0.2/dbbot/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = '0.1'
+__version__ = '0.2'
 
 from .logger import Logger
```

### Comparing `dbbot-sql-0.1/dbbot/__main__.py` & `dbbot-sql-0.2/dbbot/__main__.py`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot/logger.py` & `dbbot-sql-0.2/dbbot/logger.py`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot/reader/__init__.py` & `dbbot-sql-0.2/dbbot/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot/reader/database_writer.py` & `dbbot-sql-0.2/dbbot/reader/database_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
         if not result:
             raise Exception('Query did not yield id, even though it should have.'
                             '\nSQL statement was:\n%s\nArguments were:\n%s' % (sql_statement, list(criteria.values())))
         return result['id']
 
     def insert(self, table_name, criteria):
         sql_statement = getattr(self, table_name).insert()
-        result = self._connection.execute(sql_statement, **criteria)
+        result = self._connection.execute(sql_statement, criteria)
+        self._connection.commit()
         return result.inserted_primary_key[0]
 
     def insert_or_ignore(self, table_name, criteria):
         try:
             self.insert(table_name, criteria)
         except IntegrityError:
             self._verbose('Failed insert to {table} with values {values}'.format(table=table_name,
```

### Comparing `dbbot-sql-0.1/dbbot/reader/reader_options.py` & `dbbot-sql-0.2/dbbot/reader/reader_options.py`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot/reader/robot_results_parser.py` & `dbbot-sql-0.2/dbbot/reader/robot_results_parser.py`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot/run.py` & `dbbot-sql-0.2/dbbot/run.py`

 * *Files identical despite different names*

### Comparing `dbbot-sql-0.1/dbbot_sql.egg-info/PKG-INFO` & `dbbot-sql-0.2/dbbot_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbbot-sql
-Version: 0.1
+Version: 0.2
 Summary: A tool for inserting Robot Framework test run results into SQL database using SQLAlchemy.
 Home-page: https://github.com/pbylicki/DbBot-SQLAlchemy
 Download-URL: https://pypi.python.org/pypi/dbbot-sql
 Author: Robot Framework Developers, Pawel Bylicki
 Author-email: robotframework@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation atdd
```

### Comparing `dbbot-sql-0.1/setup.py` & `dbbot-sql-0.2/setup.py`

 * *Files identical despite different names*

