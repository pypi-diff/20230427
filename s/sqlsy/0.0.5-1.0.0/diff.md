# Comparing `tmp/sqlsy-0.0.5.tar.gz` & `tmp/sqlsy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsy-0.0.5.tar", last modified: Thu Apr 27 11:49:44 2023, max compression
+gzip compressed data, was "sqlsy-1.0.0.tar", last modified: Thu Apr 27 13:26:33 2023, max compression
```

## Comparing `sqlsy-0.0.5.tar` & `sqlsy-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/
--rw-r--r--   0 logic     (1000) logic     (1000)     3783 2023-04-27 11:49:44.645915 sqlsy-0.0.5/PKG-INFO
--rw-r--r--   0 logic     (1000) logic     (1000)     3292 2023-04-27 10:52:45.000000 sqlsy-0.0.5/README.md
--rw-r--r--   0 logic     (1000) logic     (1000)      742 2023-04-27 10:59:30.000000 sqlsy-0.0.5/pyproject.toml
--rw-r--r--   0 logic     (1000) logic     (1000)       38 2023-04-27 11:49:44.645915 sqlsy-0.0.5/setup.cfg
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/sqlsy/
--rw-r--r--   0 logic     (1000) logic     (1000)      105 2023-04-27 11:33:51.000000 sqlsy-0.0.5/src/sqlsy/__init__.py
--rw-r--r--   0 logic     (1000) logic     (1000)       93 2023-04-07 17:15:46.000000 sqlsy-0.0.5/src/sqlsy/__main__.py
--rw-r--r--   0 logic     (1000) logic     (1000)     5733 2023-04-27 11:48:18.000000 sqlsy-0.0.5/src/sqlsy/engine.py
--rw-r--r--   0 logic     (1000) logic     (1000)     1954 2023-04-27 11:07:07.000000 sqlsy-0.0.5/src/sqlsy/schema.py
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/sqlsy/utils/
--rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-07 17:13:55.000000 sqlsy-0.0.5/src/sqlsy/utils/__init__.py
--rw-r--r--   0 logic     (1000) logic     (1000)      846 2023-04-26 14:54:18.000000 sqlsy-0.0.5/src/sqlsy/utils/custom_callbacks.py
--rw-r--r--   0 logic     (1000) logic     (1000)     1257 2023-04-07 17:14:55.000000 sqlsy-0.0.5/src/sqlsy/utils/mapping.py
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 11:49:44.645915 sqlsy-0.0.5/src/sqlsy.egg-info/
--rw-r--r--   0 logic     (1000) logic     (1000)     3783 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/PKG-INFO
--rw-r--r--   0 logic     (1000) logic     (1000)      399 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/SOURCES.txt
--rw-r--r--   0 logic     (1000) logic     (1000)        1 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/dependency_links.txt
--rw-r--r--   0 logic     (1000) logic     (1000)       49 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/entry_points.txt
--rw-r--r--   0 logic     (1000) logic     (1000)       50 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/requires.txt
--rw-r--r--   0 logic     (1000) logic     (1000)        6 2023-04-27 11:49:44.000000 sqlsy-0.0.5/src/sqlsy.egg-info/top_level.txt
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 13:26:33.705108 sqlsy-1.0.0/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3867 2023-04-27 13:26:33.705108 sqlsy-1.0.0/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)     3376 2023-04-27 11:53:03.000000 sqlsy-1.0.0/README.md
+-rw-r--r--   0 logic     (1000) logic     (1000)      742 2023-04-27 12:55:45.000000 sqlsy-1.0.0/pyproject.toml
+-rw-r--r--   0 logic     (1000) logic     (1000)       38 2023-04-27 13:26:33.705108 sqlsy-1.0.0/setup.cfg
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 13:26:33.701108 sqlsy-1.0.0/src/
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 13:26:33.705108 sqlsy-1.0.0/src/sqlsy/
+-rw-r--r--   0 logic     (1000) logic     (1000)      105 2023-04-27 11:33:51.000000 sqlsy-1.0.0/src/sqlsy/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)       93 2023-04-07 17:15:46.000000 sqlsy-1.0.0/src/sqlsy/__main__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6033 2023-04-27 13:25:22.000000 sqlsy-1.0.0/src/sqlsy/engine.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2162 2023-04-27 13:24:20.000000 sqlsy-1.0.0/src/sqlsy/schema.py
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 13:26:33.705108 sqlsy-1.0.0/src/sqlsy/utils/
+-rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-07 17:13:55.000000 sqlsy-1.0.0/src/sqlsy/utils/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)      846 2023-04-26 14:54:18.000000 sqlsy-1.0.0/src/sqlsy/utils/custom_callbacks.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     1257 2023-04-07 17:14:55.000000 sqlsy-1.0.0/src/sqlsy/utils/mapping.py
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-27 13:26:33.705108 sqlsy-1.0.0/src/sqlsy.egg-info/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3867 2023-04-27 13:26:33.000000 sqlsy-1.0.0/src/sqlsy.egg-info/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)      399 2023-04-27 13:26:33.000000 sqlsy-1.0.0/src/sqlsy.egg-info/SOURCES.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)        1 2023-04-27 13:26:33.000000 sqlsy-1.0.0/src/sqlsy.egg-info/dependency_links.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)       49 2023-04-27 13:26:33.000000 sqlsy-1.0.0/src/sqlsy.egg-info/entry_points.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)       50 2023-04-27 13:26:33.000000 sqlsy-1.0.0/src/sqlsy.egg-info/requires.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)        6 2023-04-27 13:26:33.000000 sqlsy-1.0.0/src/sqlsy.egg-info/top_level.txt
```

### Comparing `sqlsy-0.0.5/PKG-INFO` & `sqlsy-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-Metadata-Version: 2.1
-Name: sqlsy
-Version: 0.0.5
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
 ![badge1](https://img.shields.io/static/v1?label=python%203&message=SQL&color=blue)
 ![badge2](https://img.shields.io/static/v1?label=easy&message=install&color=green)
 
 A simple Python Module to easy fill your sql tables with data.
 
 ## Install
 ```bash
 pip install sqlsy
 ```
 
 A python module to easy filling in dummy data insde mysql databases.
 
 ```python
-from sqlsy.engine import Engine
-from sqlsy.utils.schema import Int, VarChar      # sql datatypes to define schema
+from sqlsy import Engine
+from sqlsy import Int, VarChar      # sql datatypes to define schema
 
 # config for mysql connection : uses mysql api inside
 config = {
   'user':'username',
   'password':'pas@word',
   'host':'localhost'
 }
@@ -82,15 +68,20 @@
 `VarChar` - means "VARCHAR" of SQL. By default of size 255 # does not take size like in SQL.
 
 `Date` - means DATE of sql, `DateTime`, `Time` and `Timestamp`
 
 
 # Hooks
 ### Int/Float
-`random_int` : generates random integers
+`random_int` : generates random integers - provide range with arguments
+```python
+tb_name = {
+  'age':Int(hook='random_int', args=[10,50])
+}
+```
 
 `random_digits` : generates random 0-9 digit.
 
 `random_float` : generates random float value in the range given in args.
 
 ```python
 schema = {
```

### Comparing `sqlsy-0.0.5/README.md` & `sqlsy-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,37 @@
+Metadata-Version: 2.1
+Name: sqlsy
+Version: 1.0.0
+Summary: Fill your database Quickly with dummy data
+Author-email: shoaib wani <shoaibwani010@gmail.com>
+Project-URL: Homepage, https://github.com/pyloris/sqlsy
+Keywords: sql,sql dummy data,fake data
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # sqlsy
 ![badge1](https://img.shields.io/static/v1?label=python%203&message=SQL&color=blue)
 ![badge2](https://img.shields.io/static/v1?label=easy&message=install&color=green)
 
 A simple Python Module to easy fill your sql tables with data.
 
 ## Install
 ```bash
 pip install sqlsy
 ```
 
 A python module to easy filling in dummy data insde mysql databases.
 
 ```python
-from sqlsy.engine import Engine
-from sqlsy.utils.schema import Int, VarChar      # sql datatypes to define schema
+from sqlsy import Engine
+from sqlsy import Int, VarChar      # sql datatypes to define schema
 
 # config for mysql connection : uses mysql api inside
 config = {
   'user':'username',
   'password':'pas@word',
   'host':'localhost'
 }
@@ -68,15 +82,20 @@
 `VarChar` - means "VARCHAR" of SQL. By default of size 255 # does not take size like in SQL.
 
 `Date` - means DATE of sql, `DateTime`, `Time` and `Timestamp`
 
 
 # Hooks
 ### Int/Float
-`random_int` : generates random integers
+`random_int` : generates random integers - provide range with arguments
+```python
+tb_name = {
+  'age':Int(hook='random_int', args=[10,50])
+}
+```
 
 `random_digits` : generates random 0-9 digit.
 
 `random_float` : generates random float value in the range given in args.
 
 ```python
 schema = {
```

### Comparing `sqlsy-0.0.5/pyproject.toml` & `sqlsy-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlsy"
-version = "0.0.5"
+version = "1.0.0"
 description = "Fill your database Quickly with dummy data"
 readme = "README.md"
 authors = [{ name="shoaib wani", email="shoaibwani010@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["sql", "sql dummy data", "fake data"]
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sqlsy-0.0.5/src/sqlsy/engine.py` & `sqlsy-1.0.0/src/sqlsy/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 
 	# current column being filled
 	current_col = ""
 
 	def __init__(self, config: dir):
 		self.config = config
 		self.conn = self.connect_db()
-
-		# cursor
 		self.cursor = self.conn.cursor()
 		
 
 	# connect to the database
 	def connect_db(self):
 		try:
 			conn = mysql.connector.connect(**self.config)
@@ -156,23 +154,28 @@
 		query = self.parse_schema(schema, table_name)
 
 		# store generated data for insertion into table
 		data = []
 
 		for i in track(range(n), description=colored(f"[+] Working on {table_name}: ", 'blue')):
 			data.clear()
-
-			for col,attr in zip(schema.keys(),schema.values()):
-				self.set_col(col)
-				if attr['args'] == None:
-					data.append(attr['callback']())
-				else:
-					# pass the arguments in
-					data.append(attr['callback'](*attr['args']))
-
+			try:
+				for col,attr in zip(schema.keys(),schema.values()):
+					self.set_col(col)
+					if 'custom_flag' in attr.keys():
+						data.append(next(attr['callback']))
+					elif attr['args'] == None:
+						data.append(attr['callback']())
+					else:
+						# pass the arguments in
+						data.append(attr['callback'](*attr['args']))
+			except StopIteration:
+				cprint("[x] The custom function generated less data then target rows!", "red")
+				self.clear_table(table_name)
+				exit(0)
 			try:
 				# add the data
 				self.cursor.execute(query % tuple(data))
 
 				# commit the data
 				self.conn.commit()
 			except mysql.connector.Error as err:
@@ -215,14 +218,15 @@
 
 		# print the table
 		console.print(table)
 
 	def close(self):
 		try:
 			self.conn.close()
+			cprint("[+] Closed the Connection to database", "green")
 		except mysql.connector.Error as err:
 			cprint('[x] Couldnt close the connection : {}'.format(err), "red")
 
 
 	def __del__(self):
 		try:
 			if self.conn.is_connected():
```

### Comparing `sqlsy-0.0.5/src/sqlsy/schema.py` & `sqlsy-1.0.0/src/sqlsy/schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,81 +5,89 @@
 
 from termcolor import cprint
 from .utils.mapping import mapping
 
 
 #  Sql datatypes
 def datatype(func):
-	def sql_dtype(*, hook=None, custom_func=None, args:list = None, constraints:list=None):
+	def sql_dtype(hook=None, custom_func=None, args:tuple = None, constraints:list=None):
 
 		mini_scheme = {}
 
 		# store the args
-		mini_scheme['args'] = args
+		if args and isinstance(args, tuple):
+			mini_scheme['args'] = args
+		elif args:
+			cprint("[x] Provide Arugments in a Tuple", 'red')
+			exit(1)
+		else:
+			mini_scheme['args'] = args
 		mini_scheme['constraints'] = constraints
 
 		# check for data generator
 		if not hook and not custom_func:
 			cprint("[x] Neither Hook nor custom function is provided", "red")
 			throw()
 
 		elif custom_func:
+			# set flag for custom function
+			mini_scheme['custom_flag'] = True
 			mini_scheme['callback'] = custom_func
 
 		elif hook:
 			mini_scheme['callback'] = mapping[hook]
 
 
 		# call datatype specific function to return scheme
 		return func(hook=hook, custom_func=custom_func, args=args, this=mini_scheme)
 
 	return sql_dtype
 
 
 @datatype
-def Int(*, hook=None, custom_func=None, args:list=None, this=None):
+def Int(hook=None, custom_func=None, args:list=None, this=None):
 	# used in dynamic query building
 	this['type'] = 'int'
 	return this
 
 
 @datatype
-def Float(*, hook=None, custom_func=None, args:list=None, this=None):
+def Float(hook=None, custom_func=None, args:list=None, this=None):
 	# store the float type
 	this['type'] = 'float'
 	return this
 
 
 @datatype
-def Char(*, hook=None, custom_func=None, args:list=None, this=None):
+def Char(hook=None, custom_func=None, args:list=None, this=None):
 	this['type'] = 'char(255)'
 	return this
 
 
 @datatype
-def VarChar(*, hook=None, custom_func=None, args:list = None, this=None):
+def VarChar(hook=None, custom_func=None, args:list = None, this=None):
 	this['type'] = 'varchar(255)'
 	return this
 
 
 @datatype
-def Date(*, hook=None, custom_func=None, args:list = None, this=None):
+def Date(hook=None, custom_func=None, args:list = None, this=None):
 	this['type'] = 'date'
 	return this
 
 
 @datatype
-def Time(*, hook=None, custom_func=None, args:list = None, this=None):
+def Time(hook=None, custom_func=None, args:list = None, this=None):
 	this['type'] = 'time'
 	return this
 
 
 @datatype
-def DateTime(*, hook=None, custom_func=None, args:list = None, this=None):
+def DateTime(hook=None, custom_func=None, args:list = None, this=None):
 	this['type'] = 'datetime'
 	return this
 
 
 @datatype
-def Timestamp(*, hook=None, custom_func=None, args:list = None, this=None):
+def Timestamp(hook=None, custom_func=None, args:list = None, this=None):
 	this['type'] = 'timestamp'
 	return this
```

### Comparing `sqlsy-0.0.5/src/sqlsy/utils/custom_callbacks.py` & `sqlsy-1.0.0/src/sqlsy/utils/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `sqlsy-0.0.5/src/sqlsy/utils/mapping.py` & `sqlsy-1.0.0/src/sqlsy/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `sqlsy-0.0.5/src/sqlsy.egg-info/PKG-INFO` & `sqlsy-1.0.0/src/sqlsy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsy
-Version: 0.0.5
+Version: 1.0.0
 Summary: Fill your database Quickly with dummy data
 Author-email: shoaib wani <shoaibwani010@gmail.com>
 Project-URL: Homepage, https://github.com/pyloris/sqlsy
 Keywords: sql,sql dummy data,fake data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
@@ -22,16 +22,16 @@
 ```bash
 pip install sqlsy
 ```
 
 A python module to easy filling in dummy data insde mysql databases.
 
 ```python
-from sqlsy.engine import Engine
-from sqlsy.utils.schema import Int, VarChar      # sql datatypes to define schema
+from sqlsy import Engine
+from sqlsy import Int, VarChar      # sql datatypes to define schema
 
 # config for mysql connection : uses mysql api inside
 config = {
   'user':'username',
   'password':'pas@word',
   'host':'localhost'
 }
@@ -82,15 +82,20 @@
 `VarChar` - means "VARCHAR" of SQL. By default of size 255 # does not take size like in SQL.
 
 `Date` - means DATE of sql, `DateTime`, `Time` and `Timestamp`
 
 
 # Hooks
 ### Int/Float
-`random_int` : generates random integers
+`random_int` : generates random integers - provide range with arguments
+```python
+tb_name = {
+  'age':Int(hook='random_int', args=[10,50])
+}
+```
 
 `random_digits` : generates random 0-9 digit.
 
 `random_float` : generates random float value in the range given in args.
 
 ```python
 schema = {
```

