# Comparing `tmp/SQLAlchemy-Utils-0.9.tar.gz` & `tmp/SQLAlchemy-Utils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SQLAlchemy-Utils-0.9.tar", last modified: Thu Apr 11 14:03:42 2013, max compression
+gzip compressed data, was "dist/SQLAlchemy-Utils-0.9.1.tar", last modified: Mon Apr 15 07:15:10 2013, max compression
```

## Comparing `SQLAlchemy-Utils-0.9.tar` & `SQLAlchemy-Utils-0.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/
--rw-r--r--   0 konsta     (501) staff       (20)     1983 2013-04-11 13:56:08.000000 SQLAlchemy-Utils-0.9/CHANGES.rst
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/docs/
--rw-r--r--   0 konsta     (501) staff       (20)     8125 2013-02-19 10:32:49.000000 SQLAlchemy-Utils-0.9/docs/conf.py
--rw-r--r--   0 konsta     (501) staff       (20)     2406 2013-04-03 10:00:28.000000 SQLAlchemy-Utils-0.9/docs/index.rst
--rw-r--r--   0 konsta     (501) staff       (20)     5116 2013-02-19 09:16:09.000000 SQLAlchemy-Utils-0.9/docs/make.bat
--rw-r--r--   0 konsta     (501) staff       (20)     5604 2013-02-19 09:16:09.000000 SQLAlchemy-Utils-0.9/docs/Makefile
--rw-r--r--   0 konsta     (501) staff       (20)     1437 2013-01-12 10:37:44.000000 SQLAlchemy-Utils-0.9/LICENSE
--rw-r--r--   0 konsta     (501) staff       (20)      193 2013-01-12 10:37:27.000000 SQLAlchemy-Utils-0.9/MANIFEST.in
--rw-r--r--   0 konsta     (501) staff       (20)      749 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)      308 2013-02-19 09:01:14.000000 SQLAlchemy-Utils-0.9/README.rst
--rw-r--r--   0 konsta     (501) staff       (20)       59 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/setup.cfg
--rw-r--r--   0 konsta     (501) staff       (20)     1327 2013-04-11 13:55:31.000000 SQLAlchemy-Utils-0.9/setup.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/sqlalchemy_utils/
--rw-r--r--   0 konsta     (501) staff       (20)      653 2013-04-11 13:59:49.000000 SQLAlchemy-Utils-0.9/sqlalchemy_utils/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     5434 2013-04-08 10:21:37.000000 SQLAlchemy-Utils-0.9/sqlalchemy_utils/functions.py
--rw-r--r--   0 konsta     (501) staff       (20)     3931 2013-03-26 10:58:47.000000 SQLAlchemy-Utils-0.9/sqlalchemy_utils/merge.py
--rw-r--r--   0 konsta     (501) staff       (20)     1259 2013-04-11 13:55:21.000000 SQLAlchemy-Utils-0.9/sqlalchemy_utils/operators.py
--rw-r--r--   0 konsta     (501) staff       (20)     9197 2013-04-11 13:41:40.000000 SQLAlchemy-Utils-0.9/sqlalchemy_utils/types.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/
--rw-r--r--   0 konsta     (501) staff       (20)        1 2013-04-11 14:03:41.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 konsta     (501) staff       (20)        1 2013-03-01 13:32:59.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/not-zip-safe
--rw-r--r--   0 konsta     (501) staff       (20)      749 2013-04-11 14:03:41.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)       53 2013-04-11 14:03:41.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/requires.txt
--rw-r--r--   0 konsta     (501) staff       (20)      734 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 konsta     (501) staff       (20)       17 2013-04-11 14:03:41.000000 SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-11 14:03:42.000000 SQLAlchemy-Utils-0.9/tests/
--rw-r--r--   0 konsta     (501) staff       (20)     2479 2013-03-26 10:53:50.000000 SQLAlchemy-Utils-0.9/tests/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     1274 2013-04-11 13:55:26.000000 SQLAlchemy-Utils-0.9/tests/test_case_insensitive_comparator.py
--rw-r--r--   0 konsta     (501) staff       (20)      723 2013-04-11 13:45:25.000000 SQLAlchemy-Utils-0.9/tests/test_email.py
--rw-r--r--   0 konsta     (501) staff       (20)      528 2013-03-26 10:57:01.000000 SQLAlchemy-Utils-0.9/tests/test_instrumented_list.py
--rw-r--r--   0 konsta     (501) staff       (20)     6418 2013-03-26 10:55:31.000000 SQLAlchemy-Utils-0.9/tests/test_merge.py
--rw-r--r--   0 konsta     (501) staff       (20)     2332 2013-04-11 13:57:57.000000 SQLAlchemy-Utils-0.9/tests/test_number_range.py
--rw-r--r--   0 konsta     (501) staff       (20)     2871 2013-03-28 07:10:32.000000 SQLAlchemy-Utils-0.9/tests/test_phonenumber_type.py
--rw-r--r--   0 konsta     (501) staff       (20)     1917 2013-04-03 10:22:42.000000 SQLAlchemy-Utils-0.9/tests/test_scalar_list.py
--rw-r--r--   0 konsta     (501) staff       (20)     2978 2013-04-08 10:22:09.000000 SQLAlchemy-Utils-0.9/tests/test_utility_functions.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/
+-rw-r--r--   0 konsta     (501) staff       (20)     2125 2013-04-15 07:09:39.000000 SQLAlchemy-Utils-0.9.1/CHANGES.rst
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/docs/
+-rw-r--r--   0 konsta     (501) staff       (20)     8125 2013-02-19 10:32:49.000000 SQLAlchemy-Utils-0.9.1/docs/conf.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2406 2013-04-03 10:00:28.000000 SQLAlchemy-Utils-0.9.1/docs/index.rst
+-rw-r--r--   0 konsta     (501) staff       (20)     5116 2013-02-19 09:16:09.000000 SQLAlchemy-Utils-0.9.1/docs/make.bat
+-rw-r--r--   0 konsta     (501) staff       (20)     5604 2013-02-19 09:16:09.000000 SQLAlchemy-Utils-0.9.1/docs/Makefile
+-rw-r--r--   0 konsta     (501) staff       (20)     1437 2013-01-12 10:37:44.000000 SQLAlchemy-Utils-0.9.1/LICENSE
+-rw-r--r--   0 konsta     (501) staff       (20)      193 2013-01-12 10:37:27.000000 SQLAlchemy-Utils-0.9.1/MANIFEST.in
+-rw-r--r--   0 konsta     (501) staff       (20)      751 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)      308 2013-02-19 09:01:14.000000 SQLAlchemy-Utils-0.9.1/README.rst
+-rw-r--r--   0 konsta     (501) staff       (20)       59 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/setup.cfg
+-rw-r--r--   0 konsta     (501) staff       (20)     1329 2013-04-15 07:08:27.000000 SQLAlchemy-Utils-0.9.1/setup.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/
+-rw-r--r--   0 konsta     (501) staff       (20)      669 2013-04-15 07:07:12.000000 SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     5434 2013-04-08 10:21:37.000000 SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/functions.py
+-rw-r--r--   0 konsta     (501) staff       (20)     3931 2013-03-26 10:58:47.000000 SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/merge.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1259 2013-04-11 13:55:21.000000 SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/operators.py
+-rw-r--r--   0 konsta     (501) staff       (20)     9205 2013-04-15 07:06:07.000000 SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/types.py
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 konsta     (501) staff       (20)        1 2013-03-01 13:32:59.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/not-zip-safe
+-rw-r--r--   0 konsta     (501) staff       (20)      751 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 konsta     (501) staff       (20)       53 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/requires.txt
+-rw-r--r--   0 konsta     (501) staff       (20)      734 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 konsta     (501) staff       (20)       17 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 konsta     (501) staff       (20)        0 2013-04-15 07:15:10.000000 SQLAlchemy-Utils-0.9.1/tests/
+-rw-r--r--   0 konsta     (501) staff       (20)     2479 2013-03-26 10:53:50.000000 SQLAlchemy-Utils-0.9.1/tests/__init__.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1282 2013-04-15 07:08:08.000000 SQLAlchemy-Utils-0.9.1/tests/test_case_insensitive_comparator.py
+-rw-r--r--   0 konsta     (501) staff       (20)      731 2013-04-15 07:07:27.000000 SQLAlchemy-Utils-0.9.1/tests/test_email.py
+-rw-r--r--   0 konsta     (501) staff       (20)      528 2013-03-26 10:57:01.000000 SQLAlchemy-Utils-0.9.1/tests/test_instrumented_list.py
+-rw-r--r--   0 konsta     (501) staff       (20)     6418 2013-03-26 10:55:31.000000 SQLAlchemy-Utils-0.9.1/tests/test_merge.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2548 2013-04-15 07:13:22.000000 SQLAlchemy-Utils-0.9.1/tests/test_number_range.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2871 2013-03-28 07:10:32.000000 SQLAlchemy-Utils-0.9.1/tests/test_phonenumber_type.py
+-rw-r--r--   0 konsta     (501) staff       (20)     1929 2013-04-15 07:07:52.000000 SQLAlchemy-Utils-0.9.1/tests/test_scalar_list.py
+-rw-r--r--   0 konsta     (501) staff       (20)     2978 2013-04-08 10:22:09.000000 SQLAlchemy-Utils-0.9.1/tests/test_utility_functions.py
```

### Comparing `SQLAlchemy-Utils-0.9/CHANGES.rst` & `SQLAlchemy-Utils-0.9.1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 ---------
 
 Here you can see the full list of changes between each SQLAlchemy-Utils release.
 
 
+0.9.1 (2013-04-15)
+^^^^^^^^^^^^^^^^^^
+
+- Renamed Email to EmailType and ScalarList to ScalarListType (unified type class naming convention)
+
+
 0.9.0 (2013-04-11)
 ^^^^^^^^^^^^^^^^^^
 
 - Added CaseInsensitiveComparator
 - Added Email type
```

### Comparing `SQLAlchemy-Utils-0.9/docs/conf.py` & `SQLAlchemy-Utils-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/docs/index.rst` & `SQLAlchemy-Utils-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/docs/make.bat` & `SQLAlchemy-Utils-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/docs/Makefile` & `SQLAlchemy-Utils-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/LICENSE` & `SQLAlchemy-Utils-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/PKG-INFO` & `SQLAlchemy-Utils-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SQLAlchemy-Utils
-Version: 0.9
+Version: 0.9.1
 Summary: Various utility functions for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-utils
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         SQLAlchemy-Utils
```

### Comparing `SQLAlchemy-Utils-0.9/setup.py` & `SQLAlchemy-Utils-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def run(self):
         errno = subprocess.call(['py.test'])
         raise SystemExit(errno)
 
 setup(
     name='SQLAlchemy-Utils',
-    version='0.9',
+    version='0.9.1',
     url='https://github.com/kvesteri/sqlalchemy-utils',
     license='BSD',
     author='Konsta Vesterinen',
     author_email='konsta@fastmonkeys.com',
     description=(
         'Various utility functions for SQLAlchemy.'
     ),
```

### Comparing `SQLAlchemy-Utils-0.9/sqlalchemy_utils/__init__.py` & `SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from .functions import sort_query, defer_except, escape_like
 from .merge import merge, Merger
 from .types import (
-    Email,
+    EmailType,
     instrumented_list,
     InstrumentedList,
     PhoneNumber,
     PhoneNumberType,
     NumberRange,
     NumberRangeException,
     NumberRangeRawType,
     NumberRangeType,
-    ScalarList,
+    ScalarListType,
     ScalarListException,
 )
 
 
 __all__ = (
     sort_query,
     defer_except,
     escape_like,
     instrumented_list,
     merge,
-    Email,
+    EmailType,
     InstrumentedList,
     Merger,
     NumberRange,
     NumberRangeException,
     NumberRangeRawType,
     NumberRangeType,
     PhoneNumber,
     PhoneNumberType,
-    ScalarList,
+    ScalarListType,
     ScalarListException,
 )
```

### Comparing `SQLAlchemy-Utils-0.9/sqlalchemy_utils/functions.py` & `SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/functions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/sqlalchemy_utils/merge.py` & `SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/merge.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/sqlalchemy_utils/operators.py` & `SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/operators.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/sqlalchemy_utils/types.py` & `SQLAlchemy-Utils-0.9.1/sqlalchemy_utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         return value
 
 
 class ScalarListException(Exception):
     pass
 
 
-class ScalarList(types.TypeDecorator):
+class ScalarListType(types.TypeDecorator):
     impl = sa.UnicodeText()
 
     def __init__(self, coerce_func=unicode, separator=u','):
         self.separator = unicode(separator)
         self.coerce_func = coerce_func
 
     def process_bind_param(self, value, dialect):
@@ -115,15 +115,15 @@
                 return []
             # coerce each value
             return map(
                 self.coerce_func, value.split(self.separator)
             )
 
 
-class Email(sa.types.TypeDecorator):
+class EmailType(sa.types.TypeDecorator):
     impl = sa.Unicode(255)
     comparator_factory = CaseInsensitiveComparator
 
     def process_bind_param(self, value, dialect):
         if value is not None:
             return value.lower()
         return value
```

### Comparing `SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/PKG-INFO` & `SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SQLAlchemy-Utils
-Version: 0.9
+Version: 0.9.1
 Summary: Various utility functions for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-utils
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Description: 
         SQLAlchemy-Utils
```

### Comparing `SQLAlchemy-Utils-0.9/SQLAlchemy_Utils.egg-info/SOURCES.txt` & `SQLAlchemy-Utils-0.9.1/SQLAlchemy_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/tests/__init__.py` & `SQLAlchemy-Utils-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/tests/test_case_insensitive_comparator.py` & `SQLAlchemy-Utils-0.9.1/tests/test_case_insensitive_comparator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sqlalchemy as sa
-from sqlalchemy_utils import Email
+from sqlalchemy_utils import EmailType
 from tests import DatabaseTestCase
 
 
 class TestCaseInsensitiveComparator(DatabaseTestCase):
     def create_models(self):
         class User(self.Base):
             __tablename__ = 'user'
             id = sa.Column(sa.Integer, primary_key=True)
-            email = sa.Column(Email)
+            email = sa.Column(EmailType)
 
             def __repr__(self):
                 return 'Building(%r)' % self.id
 
         self.User = User
 
     def test_supports_equals(self):
```

### Comparing `SQLAlchemy-Utils-0.9/tests/test_email.py` & `SQLAlchemy-Utils-0.9.1/tests/test_email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sqlalchemy as sa
-from sqlalchemy_utils import Email
+from sqlalchemy_utils import EmailType
 from tests import DatabaseTestCase
 
 
 class TestEmailType(DatabaseTestCase):
     def create_models(self):
         class User(self.Base):
             __tablename__ = 'user'
             id = sa.Column(sa.Integer, primary_key=True)
-            email = sa.Column(Email)
+            email = sa.Column(EmailType)
 
             def __repr__(self):
                 return 'Building(%r)' % self.id
 
         self.User = User
 
     def test_saves_email_as_lowercased(self):
```

### Comparing `SQLAlchemy-Utils-0.9/tests/test_instrumented_list.py` & `SQLAlchemy-Utils-0.9.1/tests/test_instrumented_list.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/tests/test_merge.py` & `SQLAlchemy-Utils-0.9.1/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/tests/test_number_range.py` & `SQLAlchemy-Utils-0.9.1/tests/test_number_range.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,7 +65,13 @@
         with raises(NumberRangeException):
             NumberRange.from_str('1 - ')
 
     def test_from_normalized_str(self):
         assert str(NumberRange.from_normalized_str('[1,2]')) == '1 - 2'
         assert str(NumberRange.from_normalized_str('[1,3)')) == '1 - 2'
         assert str(NumberRange.from_normalized_str('(1,3)')) == '2'
+
+    def test_add_operator(self):
+        assert NumberRange(1, 2) + NumberRange(1, 2) == NumberRange(2, 4)
+
+    def test_sub_operator(self):
+        assert NumberRange(1, 3) - NumberRange(1, 2) == NumberRange(0, 1)
```

### Comparing `SQLAlchemy-Utils-0.9/tests/test_phonenumber_type.py` & `SQLAlchemy-Utils-0.9.1/tests/test_phonenumber_type.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Utils-0.9/tests/test_scalar_list.py` & `SQLAlchemy-Utils-0.9.1/tests/test_scalar_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sqlalchemy as sa
-from sqlalchemy_utils import ScalarList
+from sqlalchemy_utils import ScalarListType
 from pytest import raises
 from tests import DatabaseTestCase
 
 
 class TestScalarIntegerList(DatabaseTestCase):
     def create_models(self):
         class User(self.Base):
             __tablename__ = 'user'
             id = sa.Column(sa.Integer, primary_key=True)
-            some_list = sa.Column(ScalarList(int))
+            some_list = sa.Column(ScalarListType(int))
 
             def __repr__(self):
                 return 'User(%r)' % self.id
 
         self.User = User
 
     def test_save_integer_list(self):
@@ -29,15 +29,15 @@
 
 
 class TestScalarUnicodeList(DatabaseTestCase):
     def create_models(self):
         class User(self.Base):
             __tablename__ = 'user'
             id = sa.Column(sa.Integer, primary_key=True)
-            some_list = sa.Column(ScalarList(unicode))
+            some_list = sa.Column(ScalarListType(unicode))
 
             def __repr__(self):
                 return 'User(%r)' % self.id
 
         self.User = User
 
     def test_throws_exception_if_using_separator_in_list_values(self):
```

### Comparing `SQLAlchemy-Utils-0.9/tests/test_utility_functions.py` & `SQLAlchemy-Utils-0.9.1/tests/test_utility_functions.py`

 * *Files identical despite different names*

