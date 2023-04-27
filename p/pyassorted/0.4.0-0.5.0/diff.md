# Comparing `tmp/pyassorted-0.4.0.tar.gz` & `tmp/pyassorted-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassorted-0.4.0.tar", max compression
+gzip compressed data, was "pyassorted-0.5.0.tar", max compression
```

## Comparing `pyassorted-0.4.0.tar` & `pyassorted-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.4.0/LICENSE
--rw-r--r--   0        0        0     1799 2023-04-01 13:40:14.939548 pyassorted-0.4.0/README.md
--rw-r--r--   0        0        0       53 2023-04-01 11:02:45.222349 pyassorted-0.4.0/pyassorted/__init__.py
--rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.4.0/pyassorted/asyncio/__init__.py
--rw-r--r--   0        0        0     1349 2023-04-01 11:02:45.222726 pyassorted-0.4.0/pyassorted/asyncio/executor.py
--rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.4.0/pyassorted/asyncio/utils.py
--rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.4.0/pyassorted/cache/__init__.py
--rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.4.0/pyassorted/cache/cache.py
--rw-r--r--   0        0        0       56 2023-04-01 11:02:45.223359 pyassorted-0.4.0/pyassorted/lock/__init__.py
--rw-r--r--   0        0        0     4191 2023-04-01 11:02:45.223582 pyassorted-0.4.0/pyassorted/lock/filelock.py
--rw-r--r--   0        0        0       18 2023-04-01 13:42:20.936364 pyassorted-0.4.0/pyassorted/version.py
--rw-r--r--   0        0        0      495 2023-04-01 13:42:29.048796 pyassorted-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 pyassorted-0.4.0/setup.py
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 pyassorted-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1799 2023-04-01 13:44:09.331817 pyassorted-0.5.0/README.md
+-rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.5.0/pyassorted/__init__.py
+-rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.5.0/pyassorted/asyncio/__init__.py
+-rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.5.0/pyassorted/asyncio/executor.py
+-rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.5.0/pyassorted/asyncio/utils.py
+-rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.5.0/pyassorted/cache/__init__.py
+-rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.5.0/pyassorted/cache/cache.py
+-rw-r--r--   0        0        0      148 2023-04-26 07:11:33.288957 pyassorted-0.5.0/pyassorted/datetime/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-26 03:26:51.215458 pyassorted-0.5.0/pyassorted/datetime/datetime.py
+-rw-r--r--   0        0        0     1001 2023-04-26 09:05:15.499398 pyassorted-0.5.0/pyassorted/datetime/timer.py
+-rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.5.0/pyassorted/lock/__init__.py
+-rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.5.0/pyassorted/lock/filelock.py
+-rw-r--r--   0        0        0       18 2023-04-01 13:44:09.335865 pyassorted-0.5.0/pyassorted/version.py
+-rw-r--r--   0        0        0      495 2023-04-27 07:53:32.556778 pyassorted-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 pyassorted-0.5.0/PKG-INFO
```

### Comparing `pyassorted-0.4.0/LICENSE` & `pyassorted-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassorted-0.4.0/README.md` & `pyassorted-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyassorted-0.4.0/pyassorted/asyncio/executor.py` & `pyassorted-0.5.0/pyassorted/asyncio/executor.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.4.0/pyassorted/asyncio/utils.py` & `pyassorted-0.5.0/pyassorted/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.4.0/pyassorted/cache/cache.py` & `pyassorted-0.5.0/pyassorted/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.4.0/pyassorted/lock/filelock.py` & `pyassorted-0.5.0/pyassorted/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.4.0/PKG-INFO` & `pyassorted-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyassorted
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library has light-weight assorted utils in Prue-Python.
 License: MIT
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

