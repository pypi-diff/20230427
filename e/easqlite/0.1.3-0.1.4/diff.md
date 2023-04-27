# Comparing `tmp/easqlite-0.1.3.tar.gz` & `tmp/easqlite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easqlite-0.1.3.tar", last modified: Thu Apr 27 18:11:06 2023, max compression
+gzip compressed data, was "easqlite-0.1.4.tar", last modified: Thu Apr 27 18:34:08 2023, max compression
```

## Comparing `easqlite-0.1.3.tar` & `easqlite-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-0.1.3/.gitignore
--rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-0.1.3/LICENSE
--rw-r--r--   0        0        0     2639 2023-04-27 18:03:54.450260 easqlite-0.1.3/README.md
--rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-0.1.3/justfile
--rw-r--r--   0        0        0      723 2023-04-27 18:10:52.522608 easqlite-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-0.1.3/src/easqlite/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-27 17:39:05.530097 easqlite-0.1.3/src/easqlite/_blob.py
--rw-r--r--   0        0        0    11816 2023-04-27 18:09:01.032648 easqlite-0.1.3/src/easqlite/_connection.py
--rw-r--r--   0        0        0     5619 2023-04-27 18:10:46.210497 easqlite-0.1.3/src/easqlite/_cursor.py
--rw-r--r--   0        0        0      913 2023-04-27 18:02:30.616786 easqlite-0.1.3/src/easqlite/_global.py
--rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-0.1.3/src/easqlite/_types.py
--rw-r--r--   0        0        0     1907 2023-04-27 17:37:04.830961 easqlite-0.1.3/src/easqlite/_util.py
--rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-0.1.3/src/easqlite/py.typed
--rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-0.1.3/test/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-27 18:05:15.564685 easqlite-0.1.3/test/test_simple.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 easqlite-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2639 2023-04-27 18:03:54.450260 easqlite-0.1.4/README.md
+-rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-0.1.4/justfile
+-rw-r--r--   0        0        0      723 2023-04-27 18:33:51.584947 easqlite-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-0.1.4/src/easqlite/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-27 17:39:05.530097 easqlite-0.1.4/src/easqlite/_blob.py
+-rw-r--r--   0        0        0    11816 2023-04-27 18:09:01.032648 easqlite-0.1.4/src/easqlite/_connection.py
+-rw-r--r--   0        0        0     6210 2023-04-27 18:33:24.768473 easqlite-0.1.4/src/easqlite/_cursor.py
+-rw-r--r--   0        0        0      913 2023-04-27 18:02:30.616786 easqlite-0.1.4/src/easqlite/_global.py
+-rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-0.1.4/src/easqlite/_types.py
+-rw-r--r--   0        0        0     1917 2023-04-27 18:33:36.201675 easqlite-0.1.4/src/easqlite/_util.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-0.1.4/src/easqlite/py.typed
+-rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-0.1.4/test/__init__.py
+-rw-r--r--   0        0        0     3947 2023-04-27 18:29:19.587138 easqlite-0.1.4/test/test_simple.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 easqlite-0.1.4/PKG-INFO
```

### Comparing `easqlite-0.1.3/.gitignore` & `easqlite-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.3/LICENSE` & `easqlite-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.3/README.md` & `easqlite-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.3/src/easqlite/_blob.py` & `easqlite-0.1.4/src/easqlite/_blob.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.3/src/easqlite/_connection.py` & `easqlite-0.1.4/src/easqlite/_connection.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.3/src/easqlite/_cursor.py` & `easqlite-0.1.4/src/easqlite/_cursor.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 from types import TracebackType
 from typing import Any, Iterable, List, Optional, Tuple, Type, Union, overload
 from . import _connection
 from ._util import _Unset, _unset
 from ._types import RowFactory
 from asyncio import Lock
 
+class _RaisedStopIteration:
+    __slots__ = ()
+
+_raised_stop_iteration = _RaisedStopIteration()
+
+def _next(it) -> Any:
+    '''Calls next, turning a raised stopiteration into _raised_stop_iteration.
+
+    We need this because coroutines are not allowed to throw StopIteration at
+    all.  They get converted to RuntimeError.
+    '''
+    try:
+        return next(it)
+    except StopIteration:
+        return _raised_stop_iteration
+
 class Cursor:
     __slots__ = (
         '__connection',
         '__factory',
         '__cursor',
         '__opened',
         '__lock',
@@ -77,15 +93,15 @@
 
     async def fetchone(self) -> Any:
         await self._open()
         return await self.__connection._exec(self.__cursor.fetchone)
 
     async def fetchmany(self, size: Optional[int] = None) -> List[Any]:
         await self._open()
-        if size is None:
+        if size is not None:
             return await self.__connection._exec(self.__cursor.fetchmany, size)
         else:
             return await self.__connection._exec(self.__cursor.fetchmany)
 
     async def fetchall(self) -> List[Any]:
         await self._open()
         return await self.__connection._exec(self.__cursor.fetchall)
@@ -180,15 +196,18 @@
         )
 
     def __aiter__(self) -> 'Cursor':
         return self
 
     async def __anext__(self) -> Any:
         await self._open()
-        try:
-            return await self.__connection._exec(
-                next,
-                self.__cursor,
-            )
-        except StopIteration:
+        # We need this because coroutines are not allowed to throw StopIteration
+        # at all.  They get converted to RuntimeError
+        item = await self.__connection._exec(
+            _next,
+            self.__cursor,
+        )
+        if item is _raised_stop_iteration:
             raise StopAsyncIteration
+        else:
+            return item
```

### Comparing `easqlite-0.1.3/src/easqlite/_global.py` & `easqlite-0.1.4/src/easqlite/_global.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.3/src/easqlite/_util.py` & `easqlite-0.1.4/src/easqlite/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from concurrent.futures import Executor, ThreadPoolExecutor
 from typing import Any, AsyncIterable, Iterator, AsyncIterator, cast, Callable
 from asyncio import get_running_loop
 from . import _connection
 from ._types import ExecReturn
 
 class _Unset:
-    pass
+    __slots__ = ()
 
 _unset = _Unset()
 
 def _close_in_executor(executor: Executor, closeable: Any):
     '''A blocking finalizer that runs in the given executor.
 
     This should ideally never be relied upon.
```

### Comparing `easqlite-0.1.3/PKG-INFO` & `easqlite-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easqlite
-Version: 0.1.3
+Version: 0.1.4
 Summary: An executor-based async sqlite wrapper
 Keywords: asyncio,sqlite
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

