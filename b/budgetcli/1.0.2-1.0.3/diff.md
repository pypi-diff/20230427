# Comparing `tmp/budgetcli-1.0.2.tar.gz` & `tmp/budgetcli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.0.2.tar", last modified: Wed Apr 26 06:40:56 2023, max compression
+gzip compressed data, was "budgetcli-1.0.3.tar", last modified: Thu Apr 27 19:26:17 2023, max compression
```

## Comparing `budgetcli-1.0.2.tar` & `budgetcli-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:56.667640 budgetcli-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-26 06:40:29.000000 budgetcli-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-26 06:40:56.667640 budgetcli-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 06:40:29.000000 budgetcli-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 06:40:29.000000 budgetcli-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 06:40:56.667640 budgetcli-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:56.663640 budgetcli-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:56.663640 budgetcli-1.0.2/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:56.667640 budgetcli-1.0.2/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:56.667640 budgetcli-1.0.2/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 06:40:29.000000 budgetcli-1.0.2/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:40:56.667640 budgetcli-1.0.2/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-26 06:40:56.000000 budgetcli-1.0.2/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 06:40:56.000000 budgetcli-1.0.2/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:40:56.000000 budgetcli-1.0.2/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 06:40:56.000000 budgetcli-1.0.2/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 06:40:56.000000 budgetcli-1.0.2/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 06:40:56.000000 budgetcli-1.0.2/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 19:25:52.000000 budgetcli-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 19:26:17.646772 budgetcli-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 19:25:52.000000 budgetcli-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 19:25:52.000000 budgetcli-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-27 19:26:17.646772 budgetcli-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.642773 budgetcli-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.0.2/LICENSE` & `budgetcli-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/PKG-INFO` & `budgetcli-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -37,34 +37,49 @@
 **Provide the google spreadsheet id**
 ```
 budgetcli config spreadsheet-id ID
 ```
 
 **Copy the client_secret_XXX.json to app config**
 ```
-budgetcli config credentials-path /path/to/client_secret.json
+budgetcli config credentials-file-path /path/to/client_secret.json
 ```
 
 **Authorize the app access to spreadsheet data**
 ```
 budgetcli auth
 ```
 
 **Init sheet tables headers**
 ```
 budgetcli init
 ```
 
 ## Usage
 
+The commands follow the below structure.
+```
+budgetcli <VERB> <OBJECT> <OPTIONS>
+```
+
 **Add an income**
 ```
 budgetcli add income 2023-03-20 salary "short description" 4000
 ```
-![income](./images/income.gif)
-
 **Add an outcome**
 ```
 budgetcli add outcome 2023-03-20 rent "short description" 400
 ```
-![outcome](./images/outcome.gif)
+**List transactions. Default first 100 rows**
+```
+budgetcli list transactions 
+```
+**List only first 10 transactions**
 
+```
+budgetcli list transactions --rows=10 
+```
+
+**List transactions for a specific month**
+```
+budgetcli list transactions --month=April 
+```
```

### Comparing `budgetcli-1.0.2/README.md` & `budgetcli-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,34 +22,49 @@
 **Provide the google spreadsheet id**
 ```
 budgetcli config spreadsheet-id ID
 ```
 
 **Copy the client_secret_XXX.json to app config**
 ```
-budgetcli config credentials-path /path/to/client_secret.json
+budgetcli config credentials-file-path /path/to/client_secret.json
 ```
 
 **Authorize the app access to spreadsheet data**
 ```
 budgetcli auth
 ```
 
 **Init sheet tables headers**
 ```
 budgetcli init
 ```
 
 ## Usage
 
+The commands follow the below structure.
+```
+budgetcli <VERB> <OBJECT> <OPTIONS>
+```
+
 **Add an income**
 ```
 budgetcli add income 2023-03-20 salary "short description" 4000
 ```
-![income](./images/income.gif)
-
 **Add an outcome**
 ```
 budgetcli add outcome 2023-03-20 rent "short description" 400
 ```
-![outcome](./images/outcome.gif)
+**List transactions. Default first 100 rows**
+```
+budgetcli list transactions 
+```
+**List only first 10 transactions**
 
+```
+budgetcli list transactions --rows=10 
+```
+
+**List transactions for a specific month**
+```
+budgetcli list transactions --month=April 
+```
```

### Comparing `budgetcli-1.0.2/setup.cfg` & `budgetcli-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.0.2
+version = 1.0.3
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.0.2/src/budgetcli/auth.py` & `budgetcli-1.0.3/src/budgetcli/auth.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/cli/add.py` & `budgetcli-1.0.3/src/budgetcli/cli/add.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/cli/config.py` & `budgetcli-1.0.3/src/budgetcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/cli/display.py` & `budgetcli-1.0.3/src/budgetcli/cli/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/commands.py` & `budgetcli-1.0.3/src/budgetcli/commands.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/data_manager.py` & `budgetcli-1.0.3/src/budgetcli/data_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,22 +133,22 @@
         self, month: int
     ) -> list[list[str]] | None:
         """Query the transactions for current month"""
         month = month - 1  # month query starts from 0 to 11
         query = f"select A,B,C,D,E where month(A)={month}"
         transactions = []
         rows = await self._query(query)
+        pprint(rows, expand_all=True)
         if rows:
             for row in rows:
                 transaction = []
                 for cel in row.get("c", []):
                     if "Date(" in str(cel.get("v")):
-                        clean_date = cel.get("v").replace("Date(", "")[:-1]
-                        clean_date = clean_date.replace(",", "-")
-                        transaction.append(clean_date)
+                        date = cel.get("f")
+                        transaction.append(date)
                     else:
                         transaction.append(cel.get("v"))
                 transactions.append(transaction)
         return transactions
 
     async def add_transaction(self, row: list) -> None:
         """Add a transaction to the spreadsheet"""
```

### Comparing `budgetcli-1.0.2/src/budgetcli/main.py` & `budgetcli-1.0.3/src/budgetcli/main.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/models.py` & `budgetcli-1.0.3/src/budgetcli/models.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/settings.py` & `budgetcli-1.0.3/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/utils/config.py` & `budgetcli-1.0.3/src/budgetcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/utils/dates.py` & `budgetcli-1.0.3/src/budgetcli/utils/dates.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.2/src/budgetcli/utils/display.py` & `budgetcli-1.0.3/src/budgetcli/utils/display.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from contextlib import contextmanager
 
+from rich import box, print
 from rich.table import Table
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 
 @contextmanager
 def task_progress(description: str):
     """An utility function to display a progress spinner"""
@@ -19,14 +20,14 @@
         end_time = time.time()
         elapsed_time = end_time - start_time
         print(f":sparkles: Completed in {elapsed_time:.2f} seconds")
 
 
 def get_transaction_table() -> Table:
     """Return table to display the transaction date"""
-    table = Table(show_edge=False, header_style="blue")
+    table = Table(header_style="blue", box=box.HORIZONTALS)
     table.add_column("Date", justify="left", no_wrap=True)
     table.add_column("Category", justify="left", no_wrap=True)
     table.add_column("Description", justify="left", no_wrap=True)
     table.add_column("Income", justify="left", no_wrap=True, style="green")
     table.add_column("Outcome", justify="left", no_wrap=True, style="red")
     return table
```

### Comparing `budgetcli-1.0.2/src/budgetcli.egg-info/PKG-INFO` & `budgetcli-1.0.3/src/budgetcli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -37,34 +37,49 @@
 **Provide the google spreadsheet id**
 ```
 budgetcli config spreadsheet-id ID
 ```
 
 **Copy the client_secret_XXX.json to app config**
 ```
-budgetcli config credentials-path /path/to/client_secret.json
+budgetcli config credentials-file-path /path/to/client_secret.json
 ```
 
 **Authorize the app access to spreadsheet data**
 ```
 budgetcli auth
 ```
 
 **Init sheet tables headers**
 ```
 budgetcli init
 ```
 
 ## Usage
 
+The commands follow the below structure.
+```
+budgetcli <VERB> <OBJECT> <OPTIONS>
+```
+
 **Add an income**
 ```
 budgetcli add income 2023-03-20 salary "short description" 4000
 ```
-![income](./images/income.gif)
-
 **Add an outcome**
 ```
 budgetcli add outcome 2023-03-20 rent "short description" 400
 ```
-![outcome](./images/outcome.gif)
+**List transactions. Default first 100 rows**
+```
+budgetcli list transactions 
+```
+**List only first 10 transactions**
 
+```
+budgetcli list transactions --rows=10 
+```
+
+**List transactions for a specific month**
+```
+budgetcli list transactions --month=April 
+```
```

### Comparing `budgetcli-1.0.2/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-1.0.3/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

