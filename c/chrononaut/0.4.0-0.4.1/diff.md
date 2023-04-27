# Comparing `tmp/chrononaut-0.4.0.tar.gz` & `tmp/chrononaut-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrononaut-0.4.0.tar", last modified: Tue Oct 11 13:31:14 2022, max compression
+gzip compressed data, was "chrononaut-0.4.1.tar", last modified: Thu Apr 27 13:52:38 2023, max compression
```

## Comparing `chrononaut-0.4.0.tar` & `chrononaut-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2022-10-11 13:31:14.829794 chrononaut-0.4.0/
--rw-r--r--   0 pawel      (501) staff       (20)     1096 2022-10-06 12:08:48.000000 chrononaut-0.4.0/LICENSE
--rw-r--r--   0 pawel      (501) staff       (20)     1038 2022-10-11 13:31:14.829905 chrononaut-0.4.0/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)     2359 2022-10-06 12:08:48.000000 chrononaut-0.4.0/README.md
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2022-10-11 13:31:14.828133 chrononaut-0.4.0/chrononaut/
--rw-r--r--   0 pawel      (501) staff       (20)     4912 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/__init__.py
--rw-r--r--   0 pawel      (501) staff       (20)     4581 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/change_info.py
--rw-r--r--   0 pawel      (501) staff       (20)     2880 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/context_managers.py
--rw-r--r--   0 pawel      (501) staff       (20)    14835 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/data_converters.py
--rw-r--r--   0 pawel      (501) staff       (20)      337 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/exceptions.py
--rw-r--r--   0 pawel      (501) staff       (20)     7597 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/flask_versioning.py
--rw-r--r--   0 pawel      (501) staff       (20)      444 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/history_mapper.py
--rw-r--r--   0 pawel      (501) staff       (20)     4332 2022-10-11 12:54:46.000000 chrononaut-0.4.0/chrononaut/models.py
--rw-r--r--   0 pawel      (501) staff       (20)     1455 2022-10-06 12:08:48.000000 chrononaut-0.4.0/chrononaut/unsafe.py
--rw-r--r--   0 pawel      (501) staff       (20)    11216 2022-10-11 12:54:46.000000 chrononaut-0.4.0/chrononaut/versioned.py
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2022-10-11 13:31:14.829608 chrononaut-0.4.0/chrononaut.egg-info/
--rw-r--r--   0 pawel      (501) staff       (20)     1038 2022-10-11 13:31:14.000000 chrononaut-0.4.0/chrononaut.egg-info/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      499 2022-10-11 13:31:14.000000 chrononaut-0.4.0/chrononaut.egg-info/SOURCES.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2022-10-11 13:31:14.000000 chrononaut-0.4.0/chrononaut.egg-info/dependency_links.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2022-10-11 13:28:51.000000 chrononaut-0.4.0/chrononaut.egg-info/not-zip-safe
--rw-r--r--   0 pawel      (501) staff       (20)      103 2022-10-11 13:31:14.000000 chrononaut-0.4.0/chrononaut.egg-info/requires.txt
--rw-r--r--   0 pawel      (501) staff       (20)       11 2022-10-11 13:31:14.000000 chrononaut-0.4.0/chrononaut.egg-info/top_level.txt
--rw-r--r--   0 pawel      (501) staff       (20)      167 2022-10-11 13:31:14.830560 chrononaut-0.4.0/setup.cfg
--rwxr-xr-x   0 pawel      (501) staff       (20)     1725 2022-10-11 13:26:02.000000 chrononaut-0.4.0/setup.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-04-27 13:52:38.538173 chrononaut-0.4.1/
+-rw-r--r--   0 pawel      (501) staff       (20)     1096 2022-10-06 12:08:48.000000 chrononaut-0.4.1/LICENSE
+-rw-r--r--   0 pawel      (501) staff       (20)     1075 2023-04-27 13:52:38.538290 chrononaut-0.4.1/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)     2916 2023-04-27 13:46:57.000000 chrononaut-0.4.1/README.md
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-04-27 13:52:38.535781 chrononaut-0.4.1/chrononaut/
+-rw-r--r--   0 pawel      (501) staff       (20)     4912 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/__init__.py
+-rw-r--r--   0 pawel      (501) staff       (20)     4581 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/change_info.py
+-rw-r--r--   0 pawel      (501) staff       (20)     2880 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/context_managers.py
+-rw-r--r--   0 pawel      (501) staff       (20)    14835 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/data_converters.py
+-rw-r--r--   0 pawel      (501) staff       (20)      337 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/exceptions.py
+-rw-r--r--   0 pawel      (501) staff       (20)     7597 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/flask_versioning.py
+-rw-r--r--   0 pawel      (501) staff       (20)      444 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/history_mapper.py
+-rw-r--r--   0 pawel      (501) staff       (20)     4335 2023-04-27 13:46:57.000000 chrononaut-0.4.1/chrononaut/models.py
+-rw-r--r--   0 pawel      (501) staff       (20)     1455 2022-10-06 12:08:48.000000 chrononaut-0.4.1/chrononaut/unsafe.py
+-rw-r--r--   0 pawel      (501) staff       (20)    11216 2022-10-11 12:54:46.000000 chrononaut-0.4.1/chrononaut/versioned.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-04-27 13:52:38.537949 chrononaut-0.4.1/chrononaut.egg-info/
+-rw-r--r--   0 pawel      (501) staff       (20)     1075 2023-04-27 13:52:38.000000 chrononaut-0.4.1/chrononaut.egg-info/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      499 2023-04-27 13:52:38.000000 chrononaut-0.4.1/chrononaut.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-04-27 13:52:38.000000 chrononaut-0.4.1/chrononaut.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2022-10-11 13:28:51.000000 chrononaut-0.4.1/chrononaut.egg-info/not-zip-safe
+-rw-r--r--   0 pawel      (501) staff       (20)      103 2023-04-27 13:52:38.000000 chrononaut-0.4.1/chrononaut.egg-info/requires.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       11 2023-04-27 13:52:38.000000 chrononaut-0.4.1/chrononaut.egg-info/top_level.txt
+-rw-r--r--   0 pawel      (501) staff       (20)      167 2023-04-27 13:52:38.539315 chrononaut-0.4.1/setup.cfg
+-rwxr-xr-x   0 pawel      (501) staff       (20)     1725 2023-04-27 13:52:36.000000 chrononaut-0.4.1/setup.py
```

### Comparing `chrononaut-0.4.0/LICENSE` & `chrononaut-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/PKG-INFO` & `chrononaut-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: chrononaut
-Version: 0.4.0
+Version: 0.4.1
+Summary: UNKNOWN
 Home-page: https://github.com/onecodex/chrononaut
 Author: Nick Greenfield
 Author-email: opensource@onecodex.com
 License: MIT License
 Keywords: Chrononaut
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Flask
 Classifier: Programming Language :: Python
@@ -24,7 +26,9 @@
 
 
 ``chrononaut``
 ------------
 
 ``chrononaut`` is a simple history mixin for SQLAlchemy models,
 adding support for audit logging, record locking, and time travel!
+
+
```

### Comparing `chrononaut-0.4.0/README.md` & `chrononaut-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 # chrononaut
 
 ![test](https://github.com/onecodex/chrononaut/workflows/test/badge.svg) [![codecov](https://codecov.io/gh/onecodex/chrononaut/branch/master/graph/badge.svg)](https://codecov.io/gh/onecodex/chrononaut) ![pre-commit](https://github.com/onecodex/chrononaut/workflows/pre-commit/badge.svg) ![Black Code Style](https://camo.githubusercontent.com/28a51fe3a2c05048d8ca8ecd039d6b1619037326/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667) [![Documentation Status](https://readthedocs.org/projects/chrononaut/badge/?version=latest)](http://chrononaut.readthedocs.io/en/latest/?badge=latest)
 
 A history mixin with audit logging, record locking, and time travel (!) for PostgreSQL and Flask-SQLAlchemy. Requires Flask-SQLAlchemy >= 2.2. See [the documentation](https://chrononaut.readthedocs.io/) for more details. Development and all PRs should pass tests and linting on Github Actions, including use of [`pre-commit`](https://pre-commit.com) for automated linting with `flake8` and `black`.
 
+## Using with `rationale`
+Sometimes you may wish to additionally store a rationale for making a certain change; for these circumstances, you can make use of the `rationale` feature. Example usage:
+
+
+```
+with chrononaut.rationale("reasons"):
+    sample.product = <product>
+    db.session.commit()
+```
+If this is done, your rationale will be saved under `<version>.chrononaut_meta['extra_info']['rationale']` in the version object.
+
+*Note* `db.session.commit()` must be included within the `with` scope, otherwise the `rationale` will not be properly saved.
+
 ## Migrating from 0.2 to 0.3
 If using Alembic, database schema migration will be detected automatically.
 In other cases please look at the table located in `activity_factory` function in `models.py` file.
 Note that you should keep the old `*_history` tables if you with to migrate the data as well.
 
 In order to migrate data from the old model, use the `HistoryModelDataConverter` model.
 Example uses:
```

### Comparing `chrononaut-0.4.0/chrononaut/__init__.py` & `chrononaut-0.4.1/chrononaut/__init__.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut/change_info.py` & `chrononaut-0.4.1/chrononaut/change_info.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut/context_managers.py` & `chrononaut-0.4.1/chrononaut/context_managers.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut/data_converters.py` & `chrononaut-0.4.1/chrononaut/data_converters.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut/flask_versioning.py` & `chrononaut-0.4.1/chrononaut/flask_versioning.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut/models.py` & `chrononaut-0.4.1/chrononaut/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.chrononaut_meta = {
             "table_name": activity_obj.table_name,
             "changed": activity_obj.changed,
             "user_info": activity_obj.user_info,
             "extra_info": activity_obj.extra_info,
         }
         self._untracked = untracked if untracked else []
-        self._hidden = set(hidden) if hidden else {}
+        self._hidden = set(hidden) if hidden else set()
         self._activity_obj = activity_obj
         self.__initialized__ = True
 
     def diff(self, other_history_model):
         hidden_cols = self._hidden
 
         if not other_history_model:
```

### Comparing `chrononaut-0.4.0/chrononaut/unsafe.py` & `chrononaut-0.4.1/chrononaut/unsafe.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut/versioned.py` & `chrononaut-0.4.1/chrononaut/versioned.py`

 * *Files identical despite different names*

### Comparing `chrononaut-0.4.0/chrononaut.egg-info/PKG-INFO` & `chrononaut-0.4.1/chrononaut.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: chrononaut
-Version: 0.4.0
+Version: 0.4.1
+Summary: UNKNOWN
 Home-page: https://github.com/onecodex/chrononaut
 Author: Nick Greenfield
 Author-email: opensource@onecodex.com
 License: MIT License
 Keywords: Chrononaut
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Flask
 Classifier: Programming Language :: Python
@@ -24,7 +26,9 @@
 
 
 ``chrononaut``
 ------------
 
 ``chrononaut`` is a simple history mixin for SQLAlchemy models,
 adding support for audit logging, record locking, and time travel!
+
+
```

### Comparing `chrononaut-0.4.0/setup.py` & `chrononaut-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ``chrononaut`` is a simple history mixin for SQLAlchemy models,
 adding support for audit logging, record locking, and time travel!
 """
 from setuptools import setup, find_packages
 import sys
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 if sys.version_info[0] < 3:
     sys.stderr.write("Requires Python 3 or up\n")
     sys.exit(1)
```

