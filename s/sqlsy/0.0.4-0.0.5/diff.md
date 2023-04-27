# Comparing `tmp/sqlsy-0.0.4.tar.gz` & `tmp/sqlsy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsy-0.0.4.tar", last modified: Fri Apr  7 17:09:31 2023, max compression
+gzip compressed data, was "sqlsy-0.0.5.tar", last modified: Thu Apr 27 11:49:44 2023, max compression
```

## Comparing `sqlsy-0.0.4.tar` & `sqlsy-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/
--rw-r--r--   0 logic     (1000) logic     (1000)     3040 2023-04-07 17:09:31.160633 sqlsy-0.0.4/PKG-INFO
--rw-r--r--   0 logic     (1000) logic     (1000)     2549 2023-04-06 01:38:15.000000 sqlsy-0.0.4/README.md
--rw-r--r--   0 logic     (1000) logic     (1000)      739 2023-04-07 17:09:25.000000 sqlsy-0.0.4/pyproject.toml
--rw-r--r--   0 logic     (1000) logic     (1000)       38 2023-04-07 17:09:31.160633 sqlsy-0.0.4/setup.cfg
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.156633 sqlsy-0.0.4/src/
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/src/sqlsy/
--rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-05 00:55:42.000000 sqlsy-0.0.4/src/sqlsy/__init__.py
--rw-r--r--   0 logic     (1000) logic     (1000)       98 2023-04-05 00:56:42.000000 sqlsy-0.0.4/src/sqlsy/__main__.py
--rwxrwxr--   0 logic     (1000) logic     (1000)     5338 2023-04-07 16:59:04.000000 sqlsy-0.0.4/src/sqlsy/engine.py
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/src/sqlsy/utils/
--rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-03 17:18:12.000000 sqlsy-0.0.4/src/sqlsy/utils/__init__.py
--rw-r--r--   0 logic     (1000) logic     (1000)      846 2023-04-07 17:07:57.000000 sqlsy-0.0.4/src/sqlsy/utils/custom_callbacks.py
--rwxrwxr--   0 logic     (1000) logic     (1000)     1257 2023-04-07 17:08:20.000000 sqlsy-0.0.4/src/sqlsy/utils/mapping.py
--rwxrwxr--   0 logic     (1000) logic     (1000)     1948 2023-04-07 16:47:15.000000 sqlsy-0.0.4/src/sqlsy/utils/schema.py
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/src/sqlsy.egg-info/
--rw-r--r--   0 logic     (1000) logic     (1000)     3040 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/PKG-INFO
--rw-r--r--   0 logic     (1000) logic     (1000)      405 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/SOURCES.txt
--rw-r--r--   0 logic     (1000) logic     (1000)        1 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/dependency_links.txt
--rw-r--r--   0 logic     (1000) logic     (1000)       46 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/entry_points.txt
--rw-r--r--   0 logic     (1000) logic     (1000)       50 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/requires.txt
--rw-r--r--   0 logic     (1000) logic     (1000)        6 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/top_level.txt
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3783 2023-04-27 11:49:44.645915 sqlsy-0.0.5/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)     3292 2023-04-27 10:52:45.000000 sqlsy-0.0.5/README.md
+-rw-r--r--   0 logic     (1000) logic     (1000)      742 2023-04-27 10:59:30.000000 sqlsy-0.0.5/pyproject.toml
+-rw-r--r--   0 logic     (1000) logic     (1000)       38 2023-04-27 11:49:44.645915 sqlsy-0.0.5/setup.cfg
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/sqlsy/
+-rw-r--r--   0 logic     (1000) logic     (1000)      105 2023-04-27 11:33:51.000000 sqlsy-0.0.5/src/sqlsy/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)       93 2023-04-07 17:15:46.000000 sqlsy-0.0.5/src/sqlsy/__main__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5733 2023-04-27 11:48:18.000000 sqlsy-0.0.5/src/sqlsy/engine.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     1954 2023-04-27 11:07:07.000000 sqlsy-0.0.5/src/sqlsy/schema.py
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/sqlsy/utils/
+-rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-07 17:13:55.000000 sqlsy-0.0.5/src/sqlsy/utils/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)      846 2023-04-26 14:54:18.000000 sqlsy-0.0.5/src/sqlsy/utils/custom_callbacks.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     1257 2023-04-07 17:14:55.000000 sqlsy-0.0.5/src/sqlsy/utils/mapping.py
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/sqlsy.egg-info/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3783 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)      399 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/SOURCES.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)        1 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/dependency_links.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)       49 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/entry_points.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)       50 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/requires.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)        6 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/top_level.txt
```

### Comparing `sqlsy-0.0.4/PKG-INFO` & `sqlsy-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,115 @@
-Metadata-Version: 2.1
-Name: sqlsy
-Version: 0.0.4
-Summary: Fill your database Quickly with dummy data
-Author-email: shoaib wani <shoaibwani010@gmail.com>
-Project-URL: Homepage, https://github.com/pyloris/sqlsy
-Keywords: sql,sql dummy data,fake data
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # sqlsy
-### Install
+![badge1](https://img.shields.io/static/v1?label=python%203&message=SQL&color=blue)
+![badge2](https://img.shields.io/static/v1?label=easy&message=install&color=green)
+
+A simple Python Module to easy fill your sql tables with data.
+
+## Install
 ```bash
 pip install sqlsy
 ```
 
 A python module to easy filling in dummy data insde mysql databases.
 
 ```python
 from sqlsy.engine import Engine
 from sqlsy.utils.schema import Int, VarChar      # sql datatypes to define schema
 
 # config for mysql connection : uses mysql api inside
 config = {
   'user':'username',
   'password':'pas@word',
-  'host':'localhost',
-  'database':'db_name'
+  'host':'localhost'
 }
 
 # define the schema of the table to fill
 
 # hook specifies what data to generate
 schema = {
-  'id':Int('id', hook='seq_choice', args=[0,100]),     # generates numbers 0 - 100 inclu
-  'name':VarChar('name', hook='name'),        # here generate fake names
-  'job':VarChar('job', hook='job')           # here generate fake jobs
+  'id':Int(hook='sequence', args=[0,30]),     # generates numbers 0 - 30 including 30
+  'name':VarChar(hook='name'),        # here generate fake names
+  'job':VarChar(hook='job')           # here generate fake jobs
 }
 
 
 # create engine instance
 engine = Engine(config)
 
+# create a database to store above table, if not already created
+engine.create_db('employee')
+
+# create the table with above schema
+engine.create_table('person', schema)
+
 # call the method to fill in the table
-# 101 rows as id can take values from 0 to 100 = 101
-engine.fill_table("table_name", schema, 101)       # give it tablename, schema of table and no of rows.
+# 101 rows as id can take values from 0 to 30 = 31
+engine.fill_table("person", schema, 31)       # give it tablename, schema of table and no of rows.
 
 # print the table if you want
 engine.print_table("table_name")
 
 # delete all the data added to the table
 engine.clear_table("table_name")
 
-# Thats IT :)
+# drop the database if you want to
+engine.drop_db("employee")
 ```
 
+![image](https://user-images.githubusercontent.com/76217003/230254219-aafe049f-93cd-45ff-ab97-22d960785add.png)
+
 
 # Schema Functions to specify datatypes
 `Int` - means "INT" of SQL.
 
-`Char` - means "CHAR" of SQL.
+`Float` - means "Float" of SQL. Doesnt support size and pricision as recommended by the Mysql docs.
 
-`VarChar` - means "VARCHAR" of SQL. # does not take size like in SQL.
+`Char` - means "CHAR" of SQL. By default of size 255.
+
+`VarChar` - means "VARCHAR" of SQL. By default of size 255 # does not take size like in SQL.
 
 `Date` - means DATE of sql, `DateTime`, `Time` and `Timestamp`
 
 
 # Hooks
-### Int
+### Int/Float
 `random_int` : generates random integers
 
 `random_digits` : generates random 0-9 digit.
 
-`seq_choice` : generates sequenctial numbers from the range given using `args`.
+`random_float` : generates random float value in the range given in args.
+
+```python
+schema = {
+  'id':Float(hook='random_float', args=[50,200])
+}
+```
+
+`sequence` : generates sequenctial numbers from the range given using `args`.
+
+```python
+schema = {
+  'id':Int(hook='sequence', args=[50,100])
+}
+```
 
+`random_choice` : Randomly chooses values from a given list
 ```python
 schema = {
-  'id':Int('id', hook='seq_choice', args=[50,100])
+  'stream':VarChar(hook='random_choice', args=[['bca', 'btech', 'commerce', 'mtech']])
 }
 ```
 
 ### VarChar/Char
 `name` : generates full names
 
 `first_name` : generates first names
 
+`email` : generates emails
+
 `last_name` : generates last names
 
 `address` : generates fake addresses
 
 `male_name` : generates male names
 
 `female_name` : generates female names
@@ -111,16 +129,8 @@
 
 `past_date` : generates a past date
 
 `time` : generates time value HH:MM:SS
 
 `date`: generates date value
 
-
-### Choose randomly from a list
-For example if we want to choose values from a provided list at random we can use the hook `random_choice`.
-```python
-schema = {
-  'stream':VarChar('stream', hook='random_choice', args=[['Science', 'BCA', 'BTech']])
-}
-# stream will contain values from the given list in `args` at random.
-```
+`date_of_birth` : generates dob's in YYYY-MM-DD format
```

### Comparing `sqlsy-0.0.4/pyproject.toml` & `sqlsy-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlsy"
-version = "0.0.4"
+version = "0.0.5"
 description = "Fill your database Quickly with dummy data"
 readme = "README.md"
 authors = [{ name="shoaib wani", email="shoaibwani010@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["sql", "sql dummy data", "fake data"]
 requires-python = ">=3.9"
 classifiers = [
@@ -25,8 +25,8 @@
 	"numpy"
 ]
 
 [project.urls]
 Homepage = "https://github.com/pyloris/sqlsy"
 
 [project.scripts]
-sqlsy = "sqlsy.__main__:main"
+sqlsy = "sqlsy.__main__:welcome"
```

### Comparing `sqlsy-0.0.4/src/sqlsy/engine.py` & `sqlsy-0.0.5/src/sqlsy/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 			return conn
 		except mysql.connector.Error as err:
 			cprint("[x] Error : {}".format(err), "red")
 			exit(1)
 
 
 	# fetch data
-	def fetch(self, query):
+	def fetch(self, tb_name: str, cols:list):
+		query = f'select {",".join(cols)} from {tb_name}'
 		self.cursor.execute(query)
-		return cursor.fetchall()
+		return self.cursor.fetchall()
 
 
 	# Create a database
 	def create_db(self, db_name:str):
 
 		try:
 			cprint(f"[+] Creating Database {db_name}..", "blue")
@@ -173,15 +174,18 @@
 				self.cursor.execute(query % tuple(data))
 
 				# commit the data
 				self.conn.commit()
 			except mysql.connector.Error as err:
 				cprint("[x] Error : {}".format(err), "red")
 				exit(1)
-
+			except Exception as err:
+				self.clear_table(table_name)
+				cprint("[x] Error: {}".format(err), 'red')
+				exit(1)
 
 
 
 	# delete everything from the database
 	def clear_table(self, table_name):
 
 		cprint("[+] Clearing the table ...", 'blue')
@@ -208,14 +212,21 @@
 		for row in data:
 			row = list(map(str, row))
 			table.add_row(*row)
 
 		# print the table
 		console.print(table)
 
+	def close(self):
+		try:
+			self.conn.close()
+		except mysql.connector.Error as err:
+			cprint('[x] Couldnt close the connection : {}'.format(err), "red")
+
 
 	def __del__(self):
 		try:
-			self.conn.close()
-			cprint("[+] Closed the connection to mysql", "green")
+			if self.conn.is_connected():
+				self.conn.close()
+				cprint("[+] Closed the connection to mysql", "green")
 		except mysql.connector.Error as err:	
 			cprint("[x] Couldn't close connection : {}".format(err), "red")
```

### Comparing `sqlsy-0.0.4/src/sqlsy/utils/custom_callbacks.py` & `sqlsy-0.0.5/src/sqlsy/utils/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `sqlsy-0.0.4/src/sqlsy/utils/mapping.py` & `sqlsy-0.0.5/src/sqlsy/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `sqlsy-0.0.4/src/sqlsy/utils/schema.py` & `sqlsy-0.0.5/src/sqlsy/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####
 # This file defines functions related to datatypes in mysql
 # we define schema using these functions
 ####
 
 from termcolor import cprint
-from .mapping import mapping
+from .utils.mapping import mapping
 
 
 #  Sql datatypes
 def datatype(func):
 	def sql_dtype(*, hook=None, custom_func=None, args:list = None, constraints:list=None):
 
 		mini_scheme = {}
```

### Comparing `sqlsy-0.0.4/src/sqlsy.egg-info/PKG-INFO` & `sqlsy-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,129 @@
 Metadata-Version: 2.1
 Name: sqlsy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fill your database Quickly with dummy data
 Author-email: shoaib wani <shoaibwani010@gmail.com>
 Project-URL: Homepage, https://github.com/pyloris/sqlsy
 Keywords: sql,sql dummy data,fake data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # sqlsy
-### Install
+![badge1](https://img.shields.io/static/v1?label=python%203&message=SQL&color=blue)
+![badge2](https://img.shields.io/static/v1?label=easy&message=install&color=green)
+
+A simple Python Module to easy fill your sql tables with data.
+
+## Install
 ```bash
 pip install sqlsy
 ```
 
 A python module to easy filling in dummy data insde mysql databases.
 
 ```python
 from sqlsy.engine import Engine
 from sqlsy.utils.schema import Int, VarChar      # sql datatypes to define schema
 
 # config for mysql connection : uses mysql api inside
 config = {
   'user':'username',
   'password':'pas@word',
-  'host':'localhost',
-  'database':'db_name'
+  'host':'localhost'
 }
 
 # define the schema of the table to fill
 
 # hook specifies what data to generate
 schema = {
-  'id':Int('id', hook='seq_choice', args=[0,100]),     # generates numbers 0 - 100 inclu
-  'name':VarChar('name', hook='name'),        # here generate fake names
-  'job':VarChar('job', hook='job')           # here generate fake jobs
+  'id':Int(hook='sequence', args=[0,30]),     # generates numbers 0 - 30 including 30
+  'name':VarChar(hook='name'),        # here generate fake names
+  'job':VarChar(hook='job')           # here generate fake jobs
 }
 
 
 # create engine instance
 engine = Engine(config)
 
+# create a database to store above table, if not already created
+engine.create_db('employee')
+
+# create the table with above schema
+engine.create_table('person', schema)
+
 # call the method to fill in the table
-# 101 rows as id can take values from 0 to 100 = 101
-engine.fill_table("table_name", schema, 101)       # give it tablename, schema of table and no of rows.
+# 101 rows as id can take values from 0 to 30 = 31
+engine.fill_table("person", schema, 31)       # give it tablename, schema of table and no of rows.
 
 # print the table if you want
 engine.print_table("table_name")
 
 # delete all the data added to the table
 engine.clear_table("table_name")
 
-# Thats IT :)
+# drop the database if you want to
+engine.drop_db("employee")
 ```
 
+![image](https://user-images.githubusercontent.com/76217003/230254219-aafe049f-93cd-45ff-ab97-22d960785add.png)
+
 
 # Schema Functions to specify datatypes
 `Int` - means "INT" of SQL.
 
-`Char` - means "CHAR" of SQL.
+`Float` - means "Float" of SQL. Doesnt support size and pricision as recommended by the Mysql docs.
+
+`Char` - means "CHAR" of SQL. By default of size 255.
 
-`VarChar` - means "VARCHAR" of SQL. # does not take size like in SQL.
+`VarChar` - means "VARCHAR" of SQL. By default of size 255 # does not take size like in SQL.
 
 `Date` - means DATE of sql, `DateTime`, `Time` and `Timestamp`
 
 
 # Hooks
-### Int
+### Int/Float
 `random_int` : generates random integers
 
 `random_digits` : generates random 0-9 digit.
 
-`seq_choice` : generates sequenctial numbers from the range given using `args`.
+`random_float` : generates random float value in the range given in args.
+
+```python
+schema = {
+  'id':Float(hook='random_float', args=[50,200])
+}
+```
+
+`sequence` : generates sequenctial numbers from the range given using `args`.
 
 ```python
 schema = {
-  'id':Int('id', hook='seq_choice', args=[50,100])
+  'id':Int(hook='sequence', args=[50,100])
+}
+```
+
+`random_choice` : Randomly chooses values from a given list
+```python
+schema = {
+  'stream':VarChar(hook='random_choice', args=[['bca', 'btech', 'commerce', 'mtech']])
 }
 ```
 
 ### VarChar/Char
 `name` : generates full names
 
 `first_name` : generates first names
 
+`email` : generates emails
+
 `last_name` : generates last names
 
 `address` : generates fake addresses
 
 `male_name` : generates male names
 
 `female_name` : generates female names
@@ -111,16 +143,8 @@
 
 `past_date` : generates a past date
 
 `time` : generates time value HH:MM:SS
 
 `date`: generates date value
 
-
-### Choose randomly from a list
-For example if we want to choose values from a provided list at random we can use the hook `random_choice`.
-```python
-schema = {
-  'stream':VarChar('stream', hook='random_choice', args=[['Science', 'BCA', 'BTech']])
-}
-# stream will contain values from the given list in `args` at random.
-```
+`date_of_birth` : generates dob's in YYYY-MM-DD format
```

