# Comparing `tmp/tinydb_sqlite-0.1.1.tar.gz` & `tmp/tinydb_sqlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinydb_sqlite-0.1.1.tar", last modified: Fri Aug 14 07:25:21 2020, max compression
+gzip compressed data, was "tinydb_sqlite-0.1.2.tar", max compression
```

## Comparing `tinydb_sqlite-0.1.1.tar` & `tinydb_sqlite-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2020-08-08 01:42:24.515401 tinydb_sqlite-0.1.1/LICENSE
--rw-r--r--   0        0        0      363 2020-08-14 07:24:52.843891 tinydb_sqlite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      179 2020-08-14 07:23:30.702583 tinydb_sqlite-0.1.1/README.md
--rw-r--r--   0        0        0      156 2020-08-08 03:47:09.937032 tinydb_sqlite-0.1.1/tinydb_sqlite/__init__.py
--rw-r--r--   0        0        0     6900 2020-08-13 02:00:50.526192 tinydb_sqlite-0.1.1/tinydb_sqlite/storages.py
--rw-r--r--   0        0        0      888 2020-08-08 05:18:21.392093 tinydb_sqlite-0.1.1/tinydb_sqlite/utils.py
--rw-r--r--   0        0        0      777 2020-08-14 07:25:21.471570 tinydb_sqlite-0.1.1/setup.py
--rw-r--r--   0        0        0      566 2020-08-14 07:25:21.471570 tinydb_sqlite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-27 04:01:05.462114 tinydb_sqlite-0.1.2/LICENSE
+-rw-r--r--   0        0        0      552 2023-04-27 04:45:55.206627 tinydb_sqlite-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-04-27 04:01:05.463113 tinydb_sqlite-0.1.2/README.md
+-rw-r--r--   0        0        0      187 2023-04-27 04:25:57.622224 tinydb_sqlite-0.1.2/tinydb_sqlite/__init__.py
+-rw-r--r--   0        0        0     6943 2023-04-27 04:32:41.760873 tinydb_sqlite-0.1.2/tinydb_sqlite/storages.py
+-rw-r--r--   0        0        0      866 2023-04-27 04:26:45.908425 tinydb_sqlite-0.1.2/tinydb_sqlite/utils.py
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 tinydb_sqlite-0.1.2/PKG-INFO
```

### Comparing `tinydb_sqlite-0.1.1/LICENSE` & `tinydb_sqlite-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Cologler
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Cologler
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tinydb_sqlite-0.1.1/tinydb_sqlite/storages.py` & `tinydb_sqlite-0.1.2/tinydb_sqlite/storages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (c) 2020~2999 - Cologler <skyoflw@gmail.com>
 # ----------
 #
 # ----------
 
-from typing import *
+from typing import Any, Tuple, Dict, Optional
 from collections.abc import MutableMapping, ItemsView, ValuesView
 from sqlite3 import Connection, connect, Cursor
 from contextlib import closing
 import json
 
 from tinydb.storages import Storage
 
@@ -76,17 +76,17 @@
     def _decode_value(self, type_id: str, value):
         type_ = _V2T.get(type_id)
         if type_ is not None:
             if type_ is type(None):
                 return None # type(None)() takes no arguments
             else:
                 return type_(value)
-        if type_ == 'j':
+        if type_id == 'j':
             return json.loads(value)
-        raise NotImplementedError
+        raise NotImplementedError(type_id, value)
 
     def _encode_value(self, value) -> Tuple[str, Any]:
         type_ = type(value)
         type_id = _T2V.get(type_)
         if type_id is not None:
             return type_id, value
         return 'j', json.dumps(value, ensure_ascii=False)
```

### Comparing `tinydb_sqlite-0.1.1/tinydb_sqlite/utils.py` & `tinydb_sqlite-0.1.2/tinydb_sqlite/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (c) 2020~2999 - Cologler <skyoflw@gmail.com>
 # ----------
 #
 # ----------
 
-from typing import *
 from collections.abc import MutableMapping
 
 class TrackedMapping(MutableMapping):
     def __init__(self, mapping: dict):
         super().__init__()
         self._mapping = mapping
         self.history = []
```

