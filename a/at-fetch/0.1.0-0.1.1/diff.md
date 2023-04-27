# Comparing `tmp/at_fetch-0.1.0.tar.gz` & `tmp/at_fetch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "at_fetch-0.1.0.tar", max compression
+gzip compressed data, was "at_fetch-0.1.1.tar", max compression
```

## Comparing `at_fetch-0.1.0.tar` & `at_fetch-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      587 2023-04-27 16:20:24.161787 at_fetch-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 03:45:51.032926 at_fetch-0.1.0/fetch/__init__.py
--rw-r--r--   0        0        0     2633 2023-04-27 16:20:32.469816 at_fetch-0.1.0/fetch/fetch.py
--rw-r--r--   0        0        0      345 2023-04-27 16:23:21.102393 at_fetch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 at_fetch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      684 2023-04-27 16:27:38.947280 at_fetch-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 03:45:51.032926 at_fetch-0.1.1/fetch/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-27 13:33:56.779724 at_fetch-0.1.1/fetch/const.py
+-rw-r--r--   0        0        0     2634 2023-04-27 16:27:55.063335 at_fetch-0.1.1/fetch/fetch.py
+-rw-r--r--   0        0        0      345 2023-04-27 16:32:13.700226 at_fetch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 at_fetch-0.1.1/PKG-INFO
```

### Comparing `at_fetch-0.1.0/README.md` & `at_fetch-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ## at_fetch
 
 ```
 pip install at_fetch
+poetry add at_fetch
+```
+
+### example
+
+```
+poetry install
+poetry run python -m example.start_time
 ```
 
 ### usage
 
 ```
 from fetch.fetch import Fetch
 import asyncio
```

### Comparing `at_fetch-0.1.0/fetch/fetch.py` & `at_fetch-0.1.1/fetch/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 import asyncio
-from const import CHUNK_SIZE, CONCURRENT_LIMIT, INTERVAL
+from .const import CHUNK_SIZE, CONCURRENT_LIMIT, INTERVAL
 import httpx
 
 
 class Fetch:
     def __init__(self) -> None:
         self.semaphore = asyncio.Semaphore(CONCURRENT_LIMIT)
```

### Comparing `at_fetch-0.1.0/PKG-INFO` & `at_fetch-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: at-fetch
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: thecatshidog
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -15,14 +15,22 @@
 Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Description-Content-Type: text/markdown
 
 ## at_fetch
 
 ```
 pip install at_fetch
+poetry add at_fetch
+```
+
+### example
+
+```
+poetry install
+poetry run python -m example.start_time
 ```
 
 ### usage
 
 ```
 from fetch.fetch import Fetch
 import asyncio
```

