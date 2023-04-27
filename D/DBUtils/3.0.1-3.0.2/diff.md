# Comparing `tmp/DBUtils-3.0.1.tar.gz` & `tmp/DBUtils-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBUtils-3.0.1.tar", last modified: Wed Dec 22 17:21:10 2021, max compression
+gzip compressed data, was "DBUtils-3.0.2.tar", last modified: Fri Jan 14 21:03:04 2022, max compression
```

## Comparing `DBUtils-3.0.1.tar` & `DBUtils-3.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 17:21:10.100237 DBUtils-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-12-22 17:21:07.000000 DBUtils-3.0.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-12-22 17:21:07.000000 DBUtils-3.0.1/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-22 17:21:07.000000 DBUtils-3.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 17:21:10.096237 DBUtils-3.0.1/DBUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-12-22 17:21:10.000000 DBUtils-3.0.1/DBUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-12-22 17:21:10.000000 DBUtils-3.0.1/DBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-22 17:21:10.000000 DBUtils-3.0.1/DBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-12-22 17:21:10.000000 DBUtils-3.0.1/DBUtils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2021-12-22 17:21:07.000000 DBUtils-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-12-22 17:21:07.000000 DBUtils-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-12-22 17:21:10.100237 DBUtils-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-12-22 17:21:07.000000 DBUtils-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 17:21:10.096237 DBUtils-3.0.1/dbutils/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/persistent_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     7034 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/persistent_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)    21165 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/pooled_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    11261 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/pooled_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)     8220 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/simple_pooled_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     4575 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/simple_pooled_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)    26527 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/steady_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    10953 2021-12-22 17:21:07.000000 DBUtils-3.0.1/dbutils/steady_pg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 17:21:10.096237 DBUtils-3.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    11009 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/changelog.html
--rw-r--r--   0 runner    (1001) docker     (121)     7403 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4541 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/dependencies_db.png
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/dependencies_pg.png
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/doc.css
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/docutils.css
--rw-r--r--   0 runner    (1001) docker     (121)    36415 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/main.de.html
--rw-r--r--   0 runner    (1001) docker     (121)    26062 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/main.de.rst
--rw-r--r--   0 runner    (1001) docker     (121)    31825 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/main.html
--rw-r--r--   0 runner    (1001) docker     (121)    22324 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/main.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1019 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/make.py
--rw-r--r--   0 runner    (1001) docker     (121)     7038 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/persistent.png
--rw-r--r--   0 runner    (1001) docker     (121)    12053 2021-12-22 17:21:07.000000 DBUtils-3.0.1/docs/pooled.png
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-22 17:21:10.100237 DBUtils-3.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2059 2021-12-22 17:21:07.000000 DBUtils-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 17:21:10.100237 DBUtils-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/mock_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/mock_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)    10442 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_persistent_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     6999 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_persistent_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)    53549 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_pooled_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    11996 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_pooled_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_simple_pooled_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     3793 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_simple_pooled_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)    25968 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_steady_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    12742 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_steady_pg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tests/test_threading_local.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-12-22 17:21:07.000000 DBUtils-3.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 21:03:04.016974 DBUtils-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-01-14 21:03:02.000000 DBUtils-3.0.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-01-14 21:03:02.000000 DBUtils-3.0.2/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-14 21:03:02.000000 DBUtils-3.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 21:03:04.012974 DBUtils-3.0.2/DBUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-01-14 21:03:03.000000 DBUtils-3.0.2/DBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-01-14 21:03:03.000000 DBUtils-3.0.2/DBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 21:03:03.000000 DBUtils-3.0.2/DBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-14 21:03:03.000000 DBUtils-3.0.2/DBUtils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-01-14 21:03:02.000000 DBUtils-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-01-14 21:03:02.000000 DBUtils-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-01-14 21:03:04.016974 DBUtils-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-01-14 21:03:02.000000 DBUtils-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 21:03:04.012974 DBUtils-3.0.2/dbutils/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/persistent_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7034 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/persistent_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21165 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/pooled_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11261 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/pooled_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8220 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/simple_pooled_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/simple_pooled_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26843 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/steady_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10953 2022-01-14 21:03:02.000000 DBUtils-3.0.2/dbutils/steady_pg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 21:03:04.016974 DBUtils-3.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)    11187 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/changelog.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7529 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4541 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/dependencies_db.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4305 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/dependencies_pg.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/doc.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/docutils.css
+-rw-r--r--   0 runner    (1001) docker     (121)    36415 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/main.de.html
+-rw-r--r--   0 runner    (1001) docker     (121)    26062 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/main.de.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    31825 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/main.html
+-rw-r--r--   0 runner    (1001) docker     (121)    22324 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/main.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1019 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/make.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7038 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/persistent.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12053 2022-01-14 21:03:02.000000 DBUtils-3.0.2/docs/pooled.png
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-14 21:03:04.016974 DBUtils-3.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2059 2022-01-14 21:03:02.000000 DBUtils-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 21:03:04.016974 DBUtils-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/mock_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/mock_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10442 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_persistent_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6999 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_persistent_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53549 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_pooled_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11996 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_pooled_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_simple_pooled_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3793 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_simple_pooled_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27100 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_steady_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12742 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_steady_pg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tests/test_threading_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-14 21:03:02.000000 DBUtils-3.0.2/tox.ini
```

### Comparing `DBUtils-3.0.1/.bumpversion.cfg` & `DBUtils-3.0.2/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.0.1
+current_version = 3.0.2
 
 [bumpversion:file:setup.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
 [bumpversion:file:dbutils/__init__.py]
 search = __version__ = '{current_version}'
```

### Comparing `DBUtils-3.0.1/DBUtils.egg-info/PKG-INFO` & `DBUtils-3.0.2/DBUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBUtils
-Version: 3.0.1
+Version: 3.0.2
 Summary: Database connections for multi-threaded environments.
 Home-page: https://webwareforpython.github.io/DBUtils/
 Author: Christoph Zwerschke
 Author-email: cito@online.de
 License: MIT License
 Download-URL: https://pypi.org/project/DBUtils/
 Project-URL: Documentation, https://webwareforpython.github.io/DBUtils/main.html
@@ -35,14 +35,14 @@
 
 DBUtils is a suite of tools providing solid, persistent and pooled connections
 to a database that can be used in all kinds of multi-threaded environments.
 
 The suite supports DB-API 2 compliant database interfaces
 and the classic PyGreSQL interface.
 
-The current version 3.0.1 of DBUtils supports Python versions 3.6 to 3.10.
+The current version 3.0.2 of DBUtils supports Python versions 3.6 to 3.10.
 
 **Please have a look at the [changelog](https://webwareforpython.github.io/DBUtils/changelog.html), because there were some breaking changes in version 2.0.**
 
 The DBUtils home page can be found at https://webwareforpython.github.io/DBUtils/
```

### Comparing `DBUtils-3.0.1/DBUtils.egg-info/SOURCES.txt` & `DBUtils-3.0.2/DBUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/LICENSE` & `DBUtils-3.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Christoph Zwerschke
+Copyright (c) 2022 Christoph Zwerschke
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `DBUtils-3.0.1/PKG-INFO` & `DBUtils-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBUtils
-Version: 3.0.1
+Version: 3.0.2
 Summary: Database connections for multi-threaded environments.
 Home-page: https://webwareforpython.github.io/DBUtils/
 Author: Christoph Zwerschke
 Author-email: cito@online.de
 License: MIT License
 Download-URL: https://pypi.org/project/DBUtils/
 Project-URL: Documentation, https://webwareforpython.github.io/DBUtils/main.html
@@ -35,14 +35,14 @@
 
 DBUtils is a suite of tools providing solid, persistent and pooled connections
 to a database that can be used in all kinds of multi-threaded environments.
 
 The suite supports DB-API 2 compliant database interfaces
 and the classic PyGreSQL interface.
 
-The current version 3.0.1 of DBUtils supports Python versions 3.6 to 3.10.
+The current version 3.0.2 of DBUtils supports Python versions 3.6 to 3.10.
 
 **Please have a look at the [changelog](https://webwareforpython.github.io/DBUtils/changelog.html), because there were some breaking changes in version 2.0.**
 
 The DBUtils home page can be found at https://webwareforpython.github.io/DBUtils/
```

### Comparing `DBUtils-3.0.1/README.md` & `DBUtils-3.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 
 DBUtils is a suite of tools providing solid, persistent and pooled connections
 to a database that can be used in all kinds of multi-threaded environments.
 
 The suite supports DB-API 2 compliant database interfaces
 and the classic PyGreSQL interface.
 
-The current version 3.0.1 of DBUtils supports Python versions 3.6 to 3.10.
+The current version 3.0.2 of DBUtils supports Python versions 3.6 to 3.10.
 
 **Please have a look at the [changelog](https://webwareforpython.github.io/DBUtils/changelog.html), because there were some breaking changes in version 2.0.**
 
 The DBUtils home page can be found at https://webwareforpython.github.io/DBUtils/
```

### Comparing `DBUtils-3.0.1/dbutils/persistent_db.py` & `DBUtils-3.0.2/dbutils/persistent_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/dbutils/persistent_pg.py` & `DBUtils-3.0.2/dbutils/persistent_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/dbutils/pooled_db.py` & `DBUtils-3.0.2/dbutils/pooled_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/dbutils/pooled_pg.py` & `DBUtils-3.0.2/dbutils/pooled_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/dbutils/simple_pooled_db.py` & `DBUtils-3.0.2/dbutils/simple_pooled_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/dbutils/simple_pooled_pg.py` & `DBUtils-3.0.2/dbutils/simple_pooled_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/dbutils/steady_db.py` & `DBUtils-3.0.2/dbutils/steady_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,22 @@
         """Enter the runtime context for the cursor object."""
         return self
 
     def __exit__(self, *exc):
         """Exit the runtime context for the cursor object."""
         self.close()
 
+    def __iter__(self):
+        """Make cursor compatible to the iteration protocol."""
+        cursor = self._cursor
+        try:  # use iterator provided by original cursor
+            return iter(cursor)
+        except TypeError:  # create iterator if not provided
+            return iter(cursor.fetchone, None)
+
     def setinputsizes(self, sizes):
         """Store input sizes in case cursor needs to be reopened."""
         self._inputsizes = sizes
 
     def setoutputsize(self, size, column=None):
         """Store output sizes in case cursor needs to be reopened."""
         self._outputsizes[column] = size
```

### Comparing `DBUtils-3.0.1/dbutils/steady_pg.py` & `DBUtils-3.0.2/dbutils/steady_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/changelog.html` & `DBUtils-3.0.2/docs/changelog.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,54 +8,59 @@
 <link rel="stylesheet" href="doc.css" type="text/css" />
 </head>
 <body>
 <main id="changelog-for-dbutils">
 <h1 class="title">Changelog for DBUtils</h1>
 
 <section id="section-1">
+<h2>3.0.2</h2>
+<p>DBUtils 3.0.2 was released on January 14, 2022.</p>
+<p>The the optional iterator protocol on cursors is now supported.</p>
+</section>
+<section id="section-2">
 <h2>3.0.1</h2>
 <p>DBUtils 3.0.1 was released on December 22, 2021.</p>
 <p>It includes <span class="docutils literal">InterfaceError</span> to the default list of exceptions
 for which the connection failover mechanism is applied.
 You can override this with the <span class="docutils literal">failures</span> parameter.</p>
 </section>
-<section id="section-2">
+<section id="section-3">
 <h2>3.0.0</h2>
 <p>DBUtils 3.0.0 was released on November 26, 2021.</p>
 <p>It is intended to be used with Python versions 3.6 to 3.10.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Cease support for Python 2 and 3.5, minor optimizations.</p></li>
 </ul>
 </section>
-<section id="section-3">
+<section id="section-4">
 <h2>2.0.3</h2>
 <p>DBUtils 2.0.3 was released on November 26, 2021.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Support Python version 3.10.</p></li>
 </ul>
 </section>
-<section id="section-4">
+<section id="section-5">
 <h2>2.0.2</h2>
 <p>DBUtils 2.0.2 was released on June 8, 2021.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Allow using context managers for pooled connections.</p></li>
 </ul>
 </section>
-<section id="section-5">
+<section id="section-6">
 <h2>2.0.1</h2>
 <p>DBUtils 2.0.1 was released on April 8, 2021.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Avoid &quot;name Exception is not defined&quot; when exiting.</p></li>
 </ul>
 </section>
-<section id="section-6">
+<section id="section-7">
 <h2>2.0</h2>
 <p>DBUtils 2.0 was released on September 26, 2020.</p>
 <p>It is intended to be used with Python versions 2.7 and 3.5 to 3.9.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>DBUtils does not act as a Webware plugin anymore, it is now just an ordinary
 Python package (of course it could be used as such also before).</p></li>
@@ -63,54 +68,54 @@
 <li><p>Folders, packages and modules have been renamed to lower-case.
 Particularly, you need to import <span class="docutils literal">dbutils</span> instead of <span class="docutils literal">DBUtils</span> now.</p></li>
 <li><p>The internal naming conventions have also been changed to comply with PEP8.</p></li>
 <li><p>The documentation has been adapted to reflect the changes in this version.</p></li>
 <li><p>This changelog has been compiled from the former release notes.</p></li>
 </ul>
 </section>
-<section id="section-7">
+<section id="section-8">
 <h2>1.4</h2>
 <p>DBUtils 1.4 was released on September 26, 2020.</p>
 <p>It is intended to be used with Python versions 2.7 and 3.5 to 3.9.</p>
 <p>Improvements:</p>
 <ul class="simple">
 <li><p>The <span class="docutils literal">SteadyDB</span> and <span class="docutils literal">SteadyPg</span> classes only reconnect after the
 <span class="docutils literal">maxusage</span> limit has been reached when the connection is not currently
 inside a transaction.</p></li>
 </ul>
 </section>
-<section id="section-8">
+<section id="section-9">
 <h2>1.3</h2>
 <p>DBUtils 1.3 was released on March 3, 2018.</p>
 <p>It is intended to be used with Python versions 2.6, 2.7 and 3.4 to 3.7.</p>
 <p>Improvements:</p>
 <ul class="simple">
 <li><p>This version now supports context handlers for connections and cursors.</p></li>
 </ul>
 </section>
-<section id="section-9">
+<section id="section-10">
 <h2>1.2</h2>
 <p>DBUtils 1.2 was released on February 5, 2017.</p>
 <p>It is intended to be used with Python versions 2.6, 2.7 and 3.0 to 3.6.</p>
 </section>
-<section id="section-10">
+<section id="section-11">
 <h2>1.1.1</h2>
 <p>DBUtils 1.1.1 was released on February 4, 2017.</p>
 <p>It is intended to be used with Python versions 2.3 to 2.7.</p>
 <p>Improvements:</p>
 <ul class="simple">
 <li><p>Reopen <span class="docutils literal">SteadyDB</span> connections when commit or rollback fails
 (suggested by Ben Hoyt).</p></li>
 </ul>
 <p>Bugfixes:</p>
 <ul class="simple">
 <li><p>Fixed a problem when running under Jython (reported by Vitaly Kruglikov).</p></li>
 </ul>
 </section>
-<section id="section-11">
+<section id="section-12">
 <h2>1.1</h2>
 <p>DBUtils 1.1 was released on August 14, 2011.</p>
 <p>Improvements:</p>
 <ul class="simple">
 <li><p>The transparent reopening of connections is actually an undesired behavior
 if it happens during database transactions. In these cases, the transaction
 should fail and the error be reported back to the application instead of the
@@ -131,15 +136,15 @@
 <p>Bugfixes:</p>
 <ul class="simple">
 <li><p>Fixed propagation of error messages when the connection was lost.</p></li>
 <li><p>Fixed an issue with the <span class="docutils literal">setoutputsize()</span>  cursor method.</p></li>
 <li><p>Fixed some minor issues with the <span class="docutils literal">DBUtilsExample</span> for Webware.</p></li>
 </ul>
 </section>
-<section id="section-12">
+<section id="section-13">
 <h2>1.0</h2>
 <p>DBUtils 1.0 was released on November 29, 2008.</p>
 <p>It is intended to be used with Python versions 2.2 to 2.6.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Added a <span class="docutils literal">failures</span> parameter for configuring the exception classes for
 which the failover mechanisms is applied (as suggested by Matthew Harriger).</p></li>
@@ -164,63 +169,63 @@
 were already destroyed, finalizers could throw exceptions or create infinite
 recursion (problem reported by Gregory Pinero and Jehiah Czebotar).</p></li>
 <li><p>DBUtils now tries harder to find the underlying DB-API 2 module if only a
 connection creator function is specified. This had not worked before with
 the MySQLdb module (problem reported by Gregory Pinero).</p></li>
 </ul>
 </section>
-<section id="section-13">
+<section id="section-14">
 <h2>0.9.4</h2>
 <p>DBUtils 0.9.4 was released on July 7, 2007.</p>
 <p>This release fixes a problem in the destructor code and has been supplemented
 with a German User's Guide.</p>
 <p>Again, please note that the <span class="docutils literal">dbapi</span> parameter has been renamed to <span class="docutils literal">creator</span>
 in the last release, since you can now pass custom creator functions
 for database connections instead of DB-API 2 modules.</p>
 </section>
-<section id="section-14">
+<section id="section-15">
 <h2>0.9.3</h2>
 <p>DBUtils 0.9.3 was released on May 21, 2007.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Support custom creator functions for database connections.
 These can now be used as the first parameter instead of an DB-API module
 (suggested by Ezio Vernacotola).</p></li>
 <li><p>Added destructor for steady connections.</p></li>
 <li><p>Use <a class="reference external" href="https://github.com/pypa/setuptools">setuptools</a> if available.</p></li>
 <li><p>Some code cleanup.</p></li>
 <li><p>Some fixes in the documentation.
 Added Chinese translation of the User's Guide, kindly contributed by gashero.</p></li>
 </ul>
 </section>
-<section id="section-15">
+<section id="section-16">
 <h2>0.9.2</h2>
 <p>DBUtils 0.9.2 was released on September 22, 2006.</p>
 <p>It is intended to be used with Python versions 2.2 to 2.5.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Renamed <span class="docutils literal">SolidDB</span> to <span class="docutils literal">SteadyDB</span> to avoid confusion with the &quot;solidDB&quot;
 storage engine. Accordingly, renamed <span class="docutils literal">SolidPg</span> to <span class="docutils literal">SteadyPg</span>.</p></li>
 </ul>
 </section>
-<section id="section-16">
+<section id="section-17">
 <h2>0.9.1</h2>
 <p>DBUtils 0.9.1 was released on May 8, 2006.</p>
 <p>It is intended to be used with Python versions 2.2 to 2.4.</p>
 <p>Changes:</p>
 <ul class="simple">
 <li><p>Added <span class="docutils literal">_closeable</span> attribute and made persistent connections not closeable
 by default. This allows <span class="docutils literal">PersistentDB</span>  to be used in the same way as you
 would use <span class="docutils literal">PooledDB</span>.</p></li>
 <li><p>Allowed arguments in the DB-API 2 <span class="docutils literal">cursor()</span> method. MySQLdb is using this
 to specify cursor classes. (Suggested by Michael Palmer.)</p></li>
 <li><p>Improved the documentation and added a User's Guide.</p></li>
 </ul>
 </section>
-<section id="section-17">
+<section id="section-18">
 <h2>0.8.1 - 2005-09-13</h2>
 <p>DBUtils 0.8.1 was released on September 13, 2005.</p>
 <p>It is intended to be used with Python versions 2.0 to 2.4.</p>
 <p>This is the first public release of DBUtils.</p>
 </section>
 </main>
 </body>
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
 
 
 ****** Changelog for DBUtils ******
+***** 3.0.2 *****
+DBUtils 3.0.2 was released on January 14, 2022.
+The the optional iterator protocol on cursors is now supported.
+
 ***** 3.0.1 *****
 DBUtils 3.0.1 was released on December 22, 2021.
 It includes InterfaceError to the default list of exceptions for which the
 connection failover mechanism is applied. You can override this with the
 failures parameter.
 
 ***** 3.0.0 *****
```

### Comparing `DBUtils-3.0.1/docs/changelog.rst` & `DBUtils-3.0.2/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 ﻿Changelog for DBUtils
 +++++++++++++++++++++
 
+3.0.2
+=====
+
+DBUtils 3.0.2 was released on January 14, 2022.
+
+The the optional iterator protocol on cursors is now supported.
 
 3.0.1
 =====
 
 DBUtils 3.0.1 was released on December 22, 2021.
 
 It includes ``InterfaceError`` to the default list of exceptions
```

### Comparing `DBUtils-3.0.1/docs/dependencies_db.png` & `DBUtils-3.0.2/docs/dependencies_db.png`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/dependencies_pg.png` & `DBUtils-3.0.2/docs/dependencies_pg.png`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/doc.css` & `DBUtils-3.0.2/docs/doc.css`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/docutils.css` & `DBUtils-3.0.2/docs/docutils.css`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/main.de.html` & `DBUtils-3.0.2/docs/main.de.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <link rel="stylesheet" href="doc.css" type="text/css" />
 </head>
 <body class="with-toc">
 <main id="benutzeranleitung-fur-dbutils">
 <h1 class="title">Benutzeranleitung für DBUtils</h1>
 <dl class="docinfo simple">
 <dt class="version">Version<span class="colon">:</span></dt>
-<dd class="version">3.0.1</dd>
+<dd class="version">3.0.2</dd>
 <dt class="translations">Translations<span class="colon">:</span></dt>
 <dd class="translations"><p><a class="reference external" href="main.html">English</a> | German</p>
 </dd>
 </dl>
 <nav class="contents" id="inhalt" role="doc-toc">
 <p class="topic-title">Inhalt</p>
 <ul class="simple">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
 
 ****** Benutzeranleitung fÃ¼r DBUtils ******
   Version:
-      3.0.1
+      3.0.2
   Translations:
       English | German
 Inhalt
     * Zusammenfassung
     * Module
     * Download
     * Installation
```

### Comparing `DBUtils-3.0.1/docs/main.de.rst` & `DBUtils-3.0.2/docs/main.de.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿Benutzeranleitung für DBUtils
 +++++++++++++++++++++++++++++
 
-:Version: 3.0.1
+:Version: 3.0.2
 :Translations: English_ | German
 
 .. _English: main.html
 
 .. contents:: Inhalt
```

### Comparing `DBUtils-3.0.1/docs/main.html` & `DBUtils-3.0.2/docs/main.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <link rel="stylesheet" href="doc.css" type="text/css" />
 </head>
 <body class="with-toc">
 <main id="dbutils-user-s-guide">
 <h1 class="title">DBUtils User's Guide</h1>
 <dl class="docinfo simple">
 <dt class="version">Version<span class="colon">:</span></dt>
-<dd class="version">3.0.1</dd>
+<dd class="version">3.0.2</dd>
 <dt class="translations">Translations<span class="colon">:</span></dt>
 <dd class="translations"><p>English | <a class="reference external" href="main.de.html">German</a></p>
 </dd>
 </dl>
 <nav class="contents" id="contents" role="doc-toc">
 <p class="topic-title">Contents</p>
 <ul class="simple">
@@ -469,15 +469,15 @@
 Warren Smith (DbConnectionPool), Ezio Vernacotola, Jehiah Czebotar,
 Matthew Harriger, Gregory Piñero and Josef van Eenbergen.</p>
 </dd>
 </dl>
 </section>
 <section id="copyright-and-license">
 <h2>Copyright and License</h2>
-<p>Copyright © 2005-2021 by Christoph Zwerschke.
+<p>Copyright © 2005-2022 by Christoph Zwerschke.
 All Rights Reserved.</p>
 <p>DBUtils is free and open source software,
 licensed under the <a class="reference external" href="https://opensource.org/licenses/MIT">MIT license</a>.</p>
 </section>
 </main>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
 
 ****** DBUtils User's Guide ******
   Version:
-      3.0.1
+      3.0.2
   Translations:
       English | German
 Contents
     * Synopsis
     * Modules
     * Download
     * Installation
@@ -374,10 +374,10 @@
       DBUtils uses code, input and suggestions made by Ian Bicking, Chuck
       Esterbrook (Webware for Python), Dan Green (DBTools), Jay Love, Michael
       Palmer, Tom Schwaller, Geoffrey Talvola, Warren Smith (DbConnectionPool),
       Ezio Vernacotola, Jehiah Czebotar, Matthew Harriger, Gregory PiÃ±ero and
       Josef van Eenbergen.
 
 ***** Copyright and License *****
-Copyright Â© 2005-2021 by Christoph Zwerschke. All Rights Reserved.
+Copyright Â© 2005-2022 by Christoph Zwerschke. All Rights Reserved.
 DBUtils is free and open source software, licensed under the MIT_license.
```

### Comparing `DBUtils-3.0.1/docs/main.rst` & `DBUtils-3.0.2/docs/main.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿DBUtils User's Guide
 ++++++++++++++++++++
 
-:Version: 3.0.1
+:Version: 3.0.2
 :Translations: English | German_
 
 .. _German: main.de.html
 
 .. contents:: Contents
 
 
@@ -517,14 +517,14 @@
 
 .. _Christoph Zwerschke: https://github.com/Cito
 
 
 Copyright and License
 =====================
 
-Copyright © 2005-2021 by Christoph Zwerschke.
+Copyright © 2005-2022 by Christoph Zwerschke.
 All Rights Reserved.
 
 DBUtils is free and open source software,
 licensed under the `MIT license`__.
 
 __ https://opensource.org/licenses/MIT
```

### Comparing `DBUtils-3.0.1/docs/make.py` & `DBUtils-3.0.2/docs/make.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/persistent.png` & `DBUtils-3.0.2/docs/persistent.png`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/docs/pooled.png` & `DBUtils-3.0.2/docs/pooled.png`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/setup.py` & `DBUtils-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 py_version = version_info[:2]
 if not (3, 6) <= py_version < (4, 0):
     raise ImportError(
         'Python {}.{} is not supported by DBUtils.'.format(*py_version))
 
 warnings.filterwarnings('ignore', 'Unknown distribution option')
 
-__version__ = '3.0.1'
+__version__ = '3.0.2'
 
 readme = open('README.md').read()
 
 setup(
     name='DBUtils',
     version=__version__,
     description='Database connections for multi-threaded environments.',
```

### Comparing `DBUtils-3.0.1/tests/mock_db.py` & `DBUtils-3.0.2/tests/mock_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/mock_pg.py` & `DBUtils-3.0.2/tests/mock_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_persistent_db.py` & `DBUtils-3.0.2/tests/test_persistent_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_persistent_pg.py` & `DBUtils-3.0.2/tests/test_persistent_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_pooled_db.py` & `DBUtils-3.0.2/tests/test_pooled_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_pooled_pg.py` & `DBUtils-3.0.2/tests/test_pooled_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_simple_pooled_db.py` & `DBUtils-3.0.2/tests/test_simple_pooled_db.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_simple_pooled_pg.py` & `DBUtils-3.0.2/tests/test_simple_pooled_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_steady_db.py` & `DBUtils-3.0.2/tests/test_steady_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,44 @@
         self.assertEqual(db._con.open_cursors, 0)
         with db.cursor() as cursor:
             self.assertEqual(db._con.open_cursors, 1)
             cursor.execute('select test')
             self.assertEqual(cursor.fetchone(), 'test')
         self.assertEqual(db._con.open_cursors, 0)
 
+    def test_cursor_as_iterator_provided(self):
+        db = SteadyDBconnect(
+            dbapi, 0, None, None, None, True,
+            'SteadyDBTestDB', user='SteadyDBTestUser')
+        self.assertEqual(db._con.open_cursors, 0)
+        cursor = db.cursor()
+        self.assertEqual(db._con.open_cursors, 1)
+        cursor.execute('select test')
+        _cursor = cursor._cursor
+        try:
+            assert not hasattr(_cursor, 'iter')
+            _cursor.__iter__ = lambda: ['test-iter']
+            assert list(iter(cursor)) == ['test']
+        finally:
+            del _cursor.__iter__
+        cursor.close()
+        self.assertEqual(db._con.open_cursors, 0)
+
+    def test_cursor_as_iterator_created(self):
+        db = SteadyDBconnect(
+            dbapi, 0, None, None, None, True,
+            'SteadyDBTestDB', user='SteadyDBTestUser')
+        self.assertEqual(db._con.open_cursors, 0)
+        cursor = db.cursor()
+        self.assertEqual(db._con.open_cursors, 1)
+        cursor.execute('select test')
+        assert list(iter(cursor)) == ['test']
+        cursor.close()
+        self.assertEqual(db._con.open_cursors, 0)
+
     def test_connection_creator_function(self):
         db1 = SteadyDBconnect(
             dbapi, 0, None, None, None, True,
             'SteadyDBTestDB', user='SteadyDBTestUser')
         db2 = SteadyDBconnect(
             dbapi.connect, 0, None, None, None, True,
             'SteadyDBTestDB', user='SteadyDBTestUser')
```

### Comparing `DBUtils-3.0.1/tests/test_steady_pg.py` & `DBUtils-3.0.2/tests/test_steady_pg.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tests/test_threading_local.py` & `DBUtils-3.0.2/tests/test_threading_local.py`

 * *Files identical despite different names*

### Comparing `DBUtils-3.0.1/tox.ini` & `DBUtils-3.0.2/tox.ini`

 * *Files identical despite different names*

