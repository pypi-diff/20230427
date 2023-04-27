# Comparing `tmp/gulistandb-0.0.5.tar.gz` & `tmp/gulistandb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulistandb-0.0.5.tar", last modified: Wed Apr 26 14:08:26 2023, max compression
+gzip compressed data, was "gulistandb-0.0.6.tar", last modified: Thu Apr 27 05:52:13 2023, max compression
```

## Comparing `gulistandb-0.0.5.tar` & `gulistandb-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 14:08:26.559048 gulistandb-0.0.5/
--rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.5/License
--rw-rw-rw-   0        0        0     2760 2023-04-26 14:08:26.556040 gulistandb-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4086 2023-04-26 13:39:56.000000 gulistandb-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 14:08:26.561036 gulistandb-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-04-26 14:00:02.000000 gulistandb-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:08:26.509067 gulistandb-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.5/src/__init__.py
--rw-rw-rw-   0        0        0     1065 2023-04-26 11:40:19.000000 gulistandb-0.0.5/src/editor.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:08:26.551041 gulistandb-0.0.5/src/gulistandb.egg-info/
--rw-rw-rw-   0        0        0     2760 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6013 2023-04-26 13:13:08.000000 gulistandb-0.0.5/src/gulistandb.py
--rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.5/src/reader.py
--rw-rw-rw-   0        0        0     1750 2023-04-26 11:37:12.000000 gulistandb-0.0.5/src/writter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:52:13.699483 gulistandb-0.0.6/
+-rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.6/License
+-rw-rw-rw-   0        0        0     6646 2023-04-27 05:52:13.695485 gulistandb-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11850 2023-04-27 05:46:19.000000 gulistandb-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:52:13.699483 gulistandb-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-04-27 05:46:56.000000 gulistandb-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:52:13.548548 gulistandb-0.0.6/src/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.6/src/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-04-27 04:58:22.000000 gulistandb-0.0.6/src/editor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:52:13.692488 gulistandb-0.0.6/src/gulistandb.egg-info/
+-rw-rw-rw-   0        0        0     6646 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6270 2023-04-27 05:01:44.000000 gulistandb-0.0.6/src/gulistandb.py
+-rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.6/src/reader.py
+-rw-rw-rw-   0        0        0     1766 2023-04-27 04:59:45.000000 gulistandb-0.0.6/src/writter.py
```

### Comparing `gulistandb-0.0.5/License` & `gulistandb-0.0.6/License`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.5/setup.py` & `gulistandb-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-16') as f:
     long_description = f.read()
 
 setup(
     name='gulistandb',
-    version='0.0.5',
+    version='0.0.6',
     install_requires=[
         'pandas',
         # add more dependencies as needed
     ],
     package_dir={'': 'src'},
 
     # metadata
```

### Comparing `gulistandb-0.0.5/src/editor.py` & `gulistandb-0.0.6/src/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def fileInit(file_type: str, file_path: str, columns: list):
+def fileInit(file_type: str, file_path: str, columns: tuple):
     """ 
         Create a new file of the specified type if it doesn't exist, and write a header row if the file is a CSV.
 
     Args:
         file_type: A string representing the type of file to create. Valid options are 'json' and 'csv'.
         file_path: A string representing the path to the file to create.
         columns: A list of strings representing the CSV column names to write to the file.
@@ -13,21 +13,21 @@
     Raises:
         None.
 
     Example usage:
         fileInit('csv', 'data.csv', ['Name', 'Email', 'Phone'])
     """
     if file_type == 'json':
-        with open(file_path, 'x', encoding='utf-8') as f:
+        with open(file_path, 'w', encoding='utf-8') as f:
             f.write('[]')
 
     elif file_type == 'xlsv':
         pass
     else:
-        with open(file_path, 'x', encoding='utf-8') as f:
+        with open(file_path, 'w', encoding='utf-8') as f:
             for i, key in enumerate(columns):
                 f.write(key)
                 if i == len(columns)-1:
                     break
 
                 else:
                     f.write(',')
```

### Comparing `gulistandb-0.0.5/src/gulistandb.py` & `gulistandb-0.0.6/src/gulistandb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from editor import fileInit
 from reader import reader
 from writter import writter
 
 
-SUPPORTED_DATA_TYPES = ['csv', 'txt', 'json']
+SUPPORTED_DATA_TYPES = ['csv',   'json']
 
 
 class Table:
 
-    def __init__(self, tableName: str, *column, **fileType) -> None:
+    def __init__(self, tableName: str, *column, **fileType: str) -> None:
         """
     Initialize a new table with the specified name, columns and file type.
 
     Args:
         tableName: A string representing the name of the table to create.
         column: A variable-length argument list of strings representing the names of the columns to create.
         fileType: Keyword arguments specifying the file type to use and any other options. Valid options are 'csv'.
@@ -26,25 +26,29 @@
 
     Example usage:
         t = Table('users', 'id', 'name', 'email', fileType='csv')
     """
 
         self.TableName = tableName
         self.column = column
+        self.__isCalled = False
         # File Type, Default File Type Csv
         self.fileType = fileType.get('fileType', 'csv').lower() if fileType.get(
             'fileType', 'csv') in SUPPORTED_DATA_TYPES else 'csv'
 
         self.folder_path = os.path.join(
             os.getcwd(), "Data")
         self.file_path = f'{os.path.join(os.getcwd(), "Data")}/{self.TableName}.{self.fileType}'
 
         print(
             f"GulistanDB:\t\033[1;32mTable initialized successfully!\n{self.file_path}\033[0m")
-        self.__commit()
+        if not os.path.exists(self.folder_path):
+            self.__commit()
+            return None
+        print("ReInitilized")
 
     def __commit(self):
         self.file_path = f'{os.path.join(os.getcwd(), "Data")}/{self.TableName}.{self.fileType}'
         try:
             if not os.path.exists(self.folder_path):
                 os.makedirs(self.folder_path)
             fileInit(self.fileType, self.file_path, self.column)
@@ -52,15 +56,15 @@
             print(
                 f"GulistanDB:\t\033[1;31mThis file name already exists. Please try a different name.\033[0m")
             return -1
 
         print(
             f"GulistanDB:\t\033[1;33m{self.TableName} created successfully!\n{self.file_path}\033[0m")
 
-    def rename(self, newName, **fileType):
+    def rename(self, newName: str, **fileType: str):
         """
     Rename the table to a new name and/or a new file type.
 
     Args:
         newName: A string representing the new name of the table.
         fileType: Keyword arguments specifying the file type to use and any other options. Valid options are 'csv'.
 
@@ -145,14 +149,18 @@
         data = t.get()
     """
 
         with open(self.file_path, 'r') as file:
             data = file.read()
             return (data)
 
+    def clear(self):
+        fileInit(self.fileType, self.file_path, self.column)
+        return 0
+
     def insert(self, *datas):
         """
     Inserts new data into the table file.
 
     Args:
         *datas: Variable-length argument list of data rows to insert. Each row should be provided as a tuple of values.
```

### Comparing `gulistandb-0.0.5/src/reader.py` & `gulistandb-0.0.6/src/reader.py`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.5/src/writter.py` & `gulistandb-0.0.6/src/writter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import pandas as pd
 
 
-def writter(file_path, fileType, datas):
+def writter(file_path: str, fileType: str, datas: list):
     """
     Writes the provided data to the specified file in either JSON or CSV format.
 
     Args:
         file_path (str): The path to the file to be written to.
         fileType (str): The type of file to write. Must be either "json" or "csv".
         datas (list): The data to be written to the file. Must be a list of dictionaries.
```

