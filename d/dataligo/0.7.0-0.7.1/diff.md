# Comparing `tmp/dataligo-0.7.0.tar.gz` & `tmp/dataligo-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-gjxd9htl/dataligo-0.7.0.tar", last modified: Sun Apr 23 15:51:45 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-aw1ywe4y/dataligo-0.7.1.tar", last modified: Thu Apr 27 13:10:06 2023, max compression
```

## Comparing `dataligo-0.7.0.tar` & `dataligo-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,31 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-23 15:51:45.000000 dataligo-0.7.0/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.7.0/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19511 2023-04-23 15:51:45.000000 dataligo-0.7.0/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5936 2023-04-23 15:20:00.000000 dataligo-0.7.0/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19511 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      191 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      358 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-23 15:51:45.000000 dataligo-0.7.0/dataligo.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1714 2023-04-23 15:51:16.000000 dataligo-0.7.0/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-23 15:51:45.000000 dataligo-0.7.0/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.7.1/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19517 2023-04-27 13:10:06.000000 dataligo-0.7.1/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5942 2023-04-26 05:05:28.000000 dataligo-0.7.1/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      189 2023-04-27 13:09:30.000000 dataligo-0.7.1/dataligo/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     3565 2023-04-15 19:19:37.000000 dataligo-0.7.1/dataligo/core.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo/databases/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.1/dataligo/databases/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11633 2023-04-22 06:58:51.000000 dataligo-0.7.1/dataligo/databases/database.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo/datalakes/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.1/dataligo/datalakes/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    20814 2023-04-26 05:01:07.000000 dataligo-0.7.1/dataligo/datalakes/datalake.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    10320 2023-04-22 09:57:28.000000 dataligo-0.7.1/dataligo/datalakes/utils.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo/datawarehouses/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.1/dataligo/datawarehouses/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    12643 2023-04-23 15:01:59.000000 dataligo-0.7.1/dataligo/datawarehouses/datawarehouse.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1796 2023-04-18 17:25:36.000000 dataligo-0.7.1/dataligo/datawarehouses/utils.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      544 2023-04-22 06:09:11.000000 dataligo-0.7.1/dataligo/exceptions.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo/nosql/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.1/dataligo/nosql/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     8175 2023-04-22 12:10:42.000000 dataligo-0.7.1/dataligo/nosql/nosql.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      249 2023-04-21 06:38:04.000000 dataligo-0.7.1/dataligo/utils.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19517 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      583 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      358 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-27 13:10:06.000000 dataligo-0.7.1/dataligo.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1718 2023-04-27 13:09:30.000000 dataligo-0.7.1/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-27 13:10:06.000000 dataligo-0.7.1/setup.cfg
```

### Comparing `dataligo-0.7.0/LICENSE` & `dataligo-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.0/PKG-INFO` & `dataligo-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -314,15 +314,15 @@
 |MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 |ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 |DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Redis| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Redis(beta)| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 
 
 ## Acknowledgement
 
 Some functionalities of DataLigo are inspired by the following packages.
 
 - [ConnectorX](https://github.com/sfu-db/connector-x)
```

### Comparing `dataligo-0.7.0/README.md` & `dataligo-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 |MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 |ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 |DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Redis| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Redis(beta)| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 
 
 ## Acknowledgement
 
 Some functionalities of DataLigo are inspired by the following packages.
 
 - [ConnectorX](https://github.com/sfu-db/connector-x)
```

### Comparing `dataligo-0.7.0/dataligo.egg-info/PKG-INFO` & `dataligo-0.7.1/dataligo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -314,15 +314,15 @@
 |MariaDB| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |MsSQL| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |Oracle| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |SQLite| database | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[x] read</li><li>[ ] write</li></ul> |
 |MongoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 |ElasticSearch| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 |DynamoDB| nosql | <ul><li>[x] read</li><li>[x] write</li></ul>   | <ul><li>[x] read</li><li>[x] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
-|Redis| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
+|Redis(beta)| nosql | <ul><li>[x] read</li><li>[ ] write</li></ul>   | <ul><li>[ ] read</li><li>[ ] write</li></ul> | <ul><li>[ ] read</li><li>[ ] write</li></ul> |
 
 
 ## Acknowledgement
 
 Some functionalities of DataLigo are inspired by the following packages.
 
 - [ConnectorX](https://github.com/sfu-db/connector-x)
```

### Comparing `dataligo-0.7.0/pyproject.toml` & `dataligo-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataligo"
-version = "0.7.0"
+version = "0.7.1"
 description = "A library to accelerate ML and ETL pipeline by connecting all data sources"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -39,19 +39,19 @@
 [project.optional-dependencies]
 polars = ["polars"]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/dataligo"
 
-[tool.setuptools]
-py-modules = ["dataligo"]
+# [tool.setuptools]
+# py-modules = ["dataligo"]
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.7.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

