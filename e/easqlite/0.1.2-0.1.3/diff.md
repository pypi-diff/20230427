# Comparing `tmp/easqlite-0.1.2.tar.gz` & `tmp/easqlite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easqlite-0.1.2.tar", last modified: Thu Apr 27 18:09:26 2023, max compression
+gzip compressed data, was "easqlite-0.1.3.tar", last modified: Thu Apr 27 18:11:06 2023, max compression
```

## Comparing `easqlite-0.1.2.tar` & `easqlite-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-0.1.2/.gitignore
--rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-0.1.2/LICENSE
--rw-r--r--   0        0        0     2639 2023-04-27 18:03:54.450260 easqlite-0.1.2/README.md
--rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-0.1.2/justfile
--rw-r--r--   0        0        0      723 2023-04-27 18:09:14.303881 easqlite-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-0.1.2/src/easqlite/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-27 17:39:05.530097 easqlite-0.1.2/src/easqlite/_blob.py
--rw-r--r--   0        0        0    11816 2023-04-27 18:09:01.032648 easqlite-0.1.2/src/easqlite/_connection.py
--rw-r--r--   0        0        0     5652 2023-04-27 17:44:46.362112 easqlite-0.1.2/src/easqlite/_cursor.py
--rw-r--r--   0        0        0      913 2023-04-27 18:02:30.616786 easqlite-0.1.2/src/easqlite/_global.py
--rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-0.1.2/src/easqlite/_types.py
--rw-r--r--   0        0        0     1907 2023-04-27 17:37:04.830961 easqlite-0.1.2/src/easqlite/_util.py
--rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-0.1.2/src/easqlite/py.typed
--rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-0.1.2/test/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-27 18:05:15.564685 easqlite-0.1.2/test/test_simple.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 easqlite-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2639 2023-04-27 18:03:54.450260 easqlite-0.1.3/README.md
+-rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-0.1.3/justfile
+-rw-r--r--   0        0        0      723 2023-04-27 18:10:52.522608 easqlite-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-0.1.3/src/easqlite/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-27 17:39:05.530097 easqlite-0.1.3/src/easqlite/_blob.py
+-rw-r--r--   0        0        0    11816 2023-04-27 18:09:01.032648 easqlite-0.1.3/src/easqlite/_connection.py
+-rw-r--r--   0        0        0     5619 2023-04-27 18:10:46.210497 easqlite-0.1.3/src/easqlite/_cursor.py
+-rw-r--r--   0        0        0      913 2023-04-27 18:02:30.616786 easqlite-0.1.3/src/easqlite/_global.py
+-rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-0.1.3/src/easqlite/_types.py
+-rw-r--r--   0        0        0     1907 2023-04-27 17:37:04.830961 easqlite-0.1.3/src/easqlite/_util.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-0.1.3/src/easqlite/py.typed
+-rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-0.1.3/test/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-27 18:05:15.564685 easqlite-0.1.3/test/test_simple.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 easqlite-0.1.3/PKG-INFO
```

### Comparing `easqlite-0.1.2/.gitignore` & `easqlite-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/LICENSE` & `easqlite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/README.md` & `easqlite-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/pyproject.toml` & `easqlite-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'easqlite'
-version = '0.1.2'
+version = '0.1.3'
 readme = 'README.md'
 license = {text = 'MIT'}
 description = "An executor-based async sqlite wrapper"
 keywords = ['asyncio', 'sqlite']
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `easqlite-0.1.2/src/easqlite/_blob.py` & `easqlite-0.1.3/src/easqlite/_blob.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/src/easqlite/_connection.py` & `easqlite-0.1.3/src/easqlite/_connection.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/src/easqlite/_cursor.py` & `easqlite-0.1.3/src/easqlite/_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,15 @@
             await self.__connection._exec(
                 setattr,
                 self.__cursor,
                 'row_factory',
                 value,
         )
 
-    async def __aiter__(self) -> 'Cursor':
-        await self._open()
+    def __aiter__(self) -> 'Cursor':
         return self
 
     async def __anext__(self) -> Any:
         await self._open()
         try:
             return await self.__connection._exec(
                 next,
```

### Comparing `easqlite-0.1.2/src/easqlite/_global.py` & `easqlite-0.1.3/src/easqlite/_global.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/src/easqlite/_util.py` & `easqlite-0.1.3/src/easqlite/_util.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/test/test_simple.py` & `easqlite-0.1.3/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `easqlite-0.1.2/PKG-INFO` & `easqlite-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easqlite
-Version: 0.1.2
+Version: 0.1.3
 Summary: An executor-based async sqlite wrapper
 Keywords: asyncio,sqlite
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

