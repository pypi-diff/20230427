# Comparing `tmp/easqlite-0.1.4.tar.gz` & `tmp/easqlite-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easqlite-0.1.4.tar", last modified: Thu Apr 27 18:34:08 2023, max compression
+gzip compressed data, was "easqlite-0.1.5.tar", last modified: Thu Apr 27 18:43:54 2023, max compression
```

## Comparing `easqlite-0.1.4.tar` & `easqlite-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-0.1.4/.gitignore
--rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-0.1.4/LICENSE
--rw-r--r--   0        0        0     2639 2023-04-27 18:03:54.450260 easqlite-0.1.4/README.md
--rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-0.1.4/justfile
--rw-r--r--   0        0        0      723 2023-04-27 18:33:51.584947 easqlite-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-0.1.4/src/easqlite/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-27 17:39:05.530097 easqlite-0.1.4/src/easqlite/_blob.py
--rw-r--r--   0        0        0    11816 2023-04-27 18:09:01.032648 easqlite-0.1.4/src/easqlite/_connection.py
--rw-r--r--   0        0        0     6210 2023-04-27 18:33:24.768473 easqlite-0.1.4/src/easqlite/_cursor.py
--rw-r--r--   0        0        0      913 2023-04-27 18:02:30.616786 easqlite-0.1.4/src/easqlite/_global.py
--rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-0.1.4/src/easqlite/_types.py
--rw-r--r--   0        0        0     1917 2023-04-27 18:33:36.201675 easqlite-0.1.4/src/easqlite/_util.py
--rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-0.1.4/src/easqlite/py.typed
--rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-0.1.4/test/__init__.py
--rw-r--r--   0        0        0     3947 2023-04-27 18:29:19.587138 easqlite-0.1.4/test/test_simple.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 easqlite-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2639 2023-04-27 18:03:54.450260 easqlite-0.1.5/README.md
+-rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-0.1.5/justfile
+-rw-r--r--   0        0        0      723 2023-04-27 18:43:16.027959 easqlite-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-0.1.5/src/easqlite/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-27 17:39:05.530097 easqlite-0.1.5/src/easqlite/_blob.py
+-rw-r--r--   0        0        0    11923 2023-04-27 18:41:18.897880 easqlite-0.1.5/src/easqlite/_connection.py
+-rw-r--r--   0        0        0     6210 2023-04-27 18:33:24.768473 easqlite-0.1.5/src/easqlite/_cursor.py
+-rw-r--r--   0        0        0      884 2023-04-27 18:40:07.993622 easqlite-0.1.5/src/easqlite/_global.py
+-rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-0.1.5/src/easqlite/_types.py
+-rw-r--r--   0        0        0     1917 2023-04-27 18:33:36.201675 easqlite-0.1.5/src/easqlite/_util.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-0.1.5/src/easqlite/py.typed
+-rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-0.1.5/test/__init__.py
+-rw-r--r--   0        0        0     4694 2023-04-27 18:42:59.692669 easqlite-0.1.5/test/test_simple.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 easqlite-0.1.5/PKG-INFO
```

### Comparing `easqlite-0.1.4/.gitignore` & `easqlite-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.4/LICENSE` & `easqlite-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.4/README.md` & `easqlite-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.4/pyproject.toml` & `easqlite-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'easqlite'
-version = '0.1.4'
+version = '0.1.5'
 readme = 'README.md'
 license = {text = 'MIT'}
 description = "An executor-based async sqlite wrapper"
 keywords = ['asyncio', 'sqlite']
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `easqlite-0.1.4/src/easqlite/_blob.py` & `easqlite-0.1.5/src/easqlite/_blob.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.4/src/easqlite/_connection.py` & `easqlite-0.1.5/src/easqlite/_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from os import PathLike
 import sqlite3
 
 from functools import partial
 from concurrent.futures import Executor, ThreadPoolExecutor
 from types import TracebackType
-from typing import Any, AsyncIterable, Iterable, Optional, Type, Union, overload, Callable
+from typing import (
+    Any, AsyncIterable, Iterable, Optional, Type, Union, overload, Callable
+)
 from weakref import finalize
 from asyncio import get_running_loop, Lock
 from sys import version_info
 from . import _blob, _cursor
 from ._util import _Unset, _unset, _IterDump, _close_in_executor
 from ._types import ExecReturn, IsolationLevel, RowFactory, TextFactory
 
@@ -87,15 +89,20 @@
                     isolation_level = self.__isolation_level,
                     check_same_thread = self.__check_same_thread,
                     factory = self.__factory,
                     cached_statements = self.__cached_statements,
                     uri = self.__uri,
                 )
 
-                self.__finalizer = finalize(self, _close_in_executor, self.__executor, self._connection)
+                self.__finalizer = finalize(
+                    self,
+                    _close_in_executor,
+                    self.__executor,
+                    self._connection,
+                )
 
                 self.__opened = True
 
 
     async def __aenter__(self) -> 'Connection':
         await self._open()
         return self
```

### Comparing `easqlite-0.1.4/src/easqlite/_cursor.py` & `easqlite-0.1.5/src/easqlite/_cursor.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.4/src/easqlite/_global.py` & `easqlite-0.1.5/src/easqlite/_global.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sqlite3
-from types import ModuleType
 
 from typing import Any, Literal, Optional, Type, TypeVar, Callable, Union
 from ._connection import Connection
 from ._util import _exec
 
 connect = Connection
```

### Comparing `easqlite-0.1.4/src/easqlite/_util.py` & `easqlite-0.1.5/src/easqlite/_util.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.4/test/test_simple.py` & `easqlite-0.1.5/test/test_simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import unittest
-import sqlite3
 import easqlite
-import asyncio 
 import tempfile
 from pathlib import Path
 
 class SimpleTests(unittest.IsolatedAsyncioTestCase):
     async def test_some_queries(self):
         with tempfile.TemporaryDirectory() as dir:
-            db = Path(dir) / "test.db"
-            async with easqlite.connect(Path(dir) / "test.db", isolation_level=None) as connection:
+            Path(dir) / "test.db"
+            async with easqlite.connect(
+                Path(dir) / "test.db",
+                isolation_level=None,
+            ) as connection:
                 await connection.execute('''
                     CREATE TABLE foo (
                         id INTEGER PRIMARY KEY NOT NULL,
                         alpha TEXT NULL,
                         beta BLOB NOT NULL
                     )
                 ''')
@@ -24,61 +25,90 @@
                     await cursor.execute(sql, (2, 'Alpha test two', b'Beta test two'))
                     await connection.commit()
 
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     await cursor.execute(sql)
-                    self.assertEqual(await cursor.fetchone(), (1, None, b'Beta test one'))
-                    self.assertEqual(await cursor.fetchone(), (2, 'Alpha test two', b'Beta test two'))
+                    self.assertEqual(
+                        await cursor.fetchone(),
+                        (1, None, b'Beta test one'),
+                    )
+                    self.assertEqual(
+                        await cursor.fetchone(),
+                        (2, 'Alpha test two', b'Beta test two'),
+                    )
                     self.assertIs(await cursor.fetchone(), None)
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     await cursor.execute(sql)
-                    self.assertEqual(await cursor.fetchmany(), [(1, None, b'Beta test one')])
-                    self.assertEqual(await cursor.fetchmany(), [(2, 'Alpha test two', b'Beta test two')])
-                    self.assertEqual(await cursor.fetchmany(), [])
+                    self.assertEqual(
+                        await cursor.fetchmany(),
+                        [(1, None, b'Beta test one')],
+                    )
+                    self.assertEqual(
+                        await cursor.fetchmany(),
+                        [(2, 'Alpha test two', b'Beta test two')],
+                    )
+                    self.assertEqual(
+                        await cursor.fetchmany(),
+                        [],
+                    )
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     await cursor.execute(sql)
-                    self.assertEqual(await cursor.fetchmany(1000), [
+                    self.assertEqual(
+                        await cursor.fetchmany(1000),
+                        [
                         (1, None, b'Beta test one'),
                         (2, 'Alpha test two', b'Beta test two'),
                     ])
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     await cursor.execute(sql)
                     await cursor.arraysize(-1)
-                    self.assertEqual(await cursor.fetchmany(), [
-                        (1, None, b'Beta test one'),
-                        (2, 'Alpha test two', b'Beta test two'),
-                    ])
+                    self.assertEqual(
+                        await cursor.fetchmany(),
+                        [
+                            (1, None, b'Beta test one'),
+                            (2, 'Alpha test two', b'Beta test two'),
+                        ],
+                    )
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     await cursor.execute(sql)
-                    self.assertEqual(await cursor.fetchmany(-1), [
-                        (1, None, b'Beta test one'),
-                        (2, 'Alpha test two', b'Beta test two'),
-                    ])
+                    self.assertEqual(
+                        await cursor.fetchmany(-1),
+                        [
+                            (1, None, b'Beta test one'),
+                            (2, 'Alpha test two', b'Beta test two'),
+                        ],
+                    )
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     await cursor.execute(sql)
-                    self.assertEqual(await cursor.fetchall(), [
-                        (1, None, b'Beta test one'),
-                        (2, 'Alpha test two', b'Beta test two'),
-                    ])
+                    self.assertEqual(
+                        await cursor.fetchall(),
+                        [
+                            (1, None, b'Beta test one'),
+                            (2, 'Alpha test two', b'Beta test two'),
+                        ],
+                    )
 
                 async with connection.cursor() as cursor:
                     sql = 'SELECT id, alpha, beta FROM foo ORDER BY id ASC'
                     rows = []
                     async for row in await cursor.execute(sql):
                         rows.append(row)
 
-                    self.assertEqual(rows, [
-                        (1, None, b'Beta test one'),
-                        (2, 'Alpha test two', b'Beta test two'),
-                    ])
+                    self.assertEqual(
+                        rows,
+                        [
+                            (1, None, b'Beta test one'),
+                            (2, 'Alpha test two', b'Beta test two'),
+                        ],
+                    )
```

### Comparing `easqlite-0.1.4/PKG-INFO` & `easqlite-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easqlite
-Version: 0.1.4
+Version: 0.1.5
 Summary: An executor-based async sqlite wrapper
 Keywords: asyncio,sqlite
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

