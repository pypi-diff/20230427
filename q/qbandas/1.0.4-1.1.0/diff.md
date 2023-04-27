# Comparing `tmp/qbandas-1.0.4.tar.gz` & `tmp/qbandas-1.1.0.tar.gz`

## Comparing `qbandas-1.0.4.tar` & `qbandas-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.0.4/requirements.txt
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/__main__.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/headers.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/pack.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/schema.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/test_headers.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/upload.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/util.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 qbandas-1.0.4/qbandas/data/field_types.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 qbandas-1.0.4/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.0.4/LICENSE
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 qbandas-1.0.4/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 qbandas-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 qbandas-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/__main__.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/headers.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/pack.py
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/records.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/schema.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/util.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 qbandas-1.1.0/qbandas/data/field_types.json
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 qbandas-1.1.0/test/test_headers.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 qbandas-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 qbandas-1.1.0/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 qbandas-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 qbandas-1.1.0/PKG-INFO
```

### Comparing `qbandas-1.0.4/qbandas/__init__.py` & `qbandas-1.1.0/qbandas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     for t in field_types:
         if field_types[t]["pack"]:
             field_types[t]["pack"] = PACKING_FUNCS[field_types[t]["pack"]]
     
     return field_types
 FIELD_TYPES = setup1()
 
-from . import headers, schema, upload
+from . import headers, records, schema
```

### Comparing `qbandas-1.0.4/qbandas/__main__.py` & `qbandas-1.1.0/qbandas/__main__.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/qbandas/headers.py` & `qbandas-1.1.0/qbandas/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 DEFAULT_HOST = '<demo.quickbase.com>'
 DEFAULT_USER = 'user'
 DEFAULT_AUTH = '<QB-USER-TOKEN xxxxxx_xxx_x_xxxxxxxxxxxxxxxxxxxxxxxxxx>'
 
 def create(interactive: bool = False, repair: bool = False, *, 
            host: str = DEFAULT_HOST, user: str = DEFAULT_USER, 
            auth: str = DEFAULT_AUTH, directory: Path|str = None,
-           **kwargs) -> NoReturn:
+           **kwargs) -> None:
     '''
     Create a header file if there isn't one
 
     If this function does not create or repair a header file, it does 
     nothing.
 
     Parameters
@@ -158,20 +158,20 @@
 
     # check the keys are correct
     if not {"QB-Realm-Hostname","User-Agent","Authorization"} == set(contents):
         if warn_: warn(f'header file: {header_path} has invalid keys')
         return False
 
     # check hostname
-    if not re.match(r'^[a-zA-Z]+\.quickbase\.com$', contents["QB-Realm-Hostname"]):
+    if not re.match(r'^[\w\-]+\.quickbase\.com$',contents["QB-Realm-Hostname"]):
         if warn_: warn(f'header file: {header_path} has invalid hostname')
         return False
     
     # check authorization
-    if not re.match(r'^QB-(USER|TEMP)-TOKEN \w{6}_\w{3}_\w_\w{26}$', contents["Authorization"]):
+    if not re.match(r'^QB-(USER|TEMP)-TOKEN \w{6}_\w{2,5}_\w_\w{20,30}$', contents["Authorization"]):
         if warn_: warn(f'header file: {header_path} has invalid authorization')
         return False
 
     return True
 
 
 def read(directory: Path|str = None, **kwargs) -> dict[str, str]:
@@ -193,12 +193,12 @@
     directory = directory if directory else os.getcwd()  
     if not os.path.isdir(directory):
         raise FileNotFoundError(f'{directory = } is not a valid directory')
 
     if not exists(directory = directory):
         raise FileNotFoundError(f'No header file found in {directory}')
     
-    if not valid(directory = directory):
+    if not valid(directory = directory, warn_=True):
         raise ValueError(f'header file in {directory} is invalid')
     
     with open(join(directory, HEADER_FILE_NAME)) as f:
         return json.load(f)
```

### Comparing `qbandas-1.0.4/qbandas/pack.py` & `qbandas-1.1.0/qbandas/pack.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/qbandas/schema.py` & `qbandas-1.1.0/qbandas/schema.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/qbandas/test_headers.py` & `qbandas-1.1.0/test/test_headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import unittest
 import os
+import unittest
 from os.path import exists
 
-from . import headers
+from qbandas import headers
+
 
 class TestHeaders(unittest.TestCase):
 
     def setUp(self) -> None:
         '''Remove any leftover header files'''
         if exists(headers.HEADER_FILE_NAME):
             os.remove(headers.HEADER_FILE_NAME)
```

### Comparing `qbandas-1.0.4/qbandas/util.py` & `qbandas-1.1.0/qbandas/util.py`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/qbandas/data/field_types.json` & `qbandas-1.1.0/qbandas/data/field_types.json`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/LICENSE` & `qbandas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/README.md` & `qbandas-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qbandas-1.0.4/pyproject.toml` & `qbandas-1.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 2022 7061 6e64 6173 3d3d 312e 342e 3322   "pandas==1.4.3"
 00000040: 2c0d 0a20 2022 7265 7175 6573 7473 3d3d  ,..  "requests==
 00000050: 322e 3238 2e31 220d 0a20 205d 0d0a 6275  2.28.1"..  ]..bu
 00000060: 696c 642d 6261 636b 656e 6420 3d20 2268  ild-backend = "h
 00000070: 6174 6368 6c69 6e67 2e62 7569 6c64 220d  atchling.build".
 00000080: 0a0d 0a5b 7072 6f6a 6563 745d 0d0a 6e61  ...[project]..na
 00000090: 6d65 203d 2022 7162 616e 6461 7322 0d0a  me = "qbandas"..
-000000a0: 7665 7273 696f 6e20 3d20 2231 2e30 2e34  version = "1.0.4
+000000a0: 7665 7273 696f 6e20 3d20 2231 2e31 2e30  version = "1.1.0
 000000b0: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
 000000c0: 2020 7b20 6e61 6d65 3d22 4a6f 7368 7561    { name="Joshua
 000000d0: 2048 6f70 776f 6f64 2220 7d2c 0d0a 5d0d   Hopwood" },..].
 000000e0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 000000f0: 496e 7465 6772 6174 6573 2074 6865 2070  Integrates the p
 00000100: 6f70 756c 6172 2064 6174 6120 6861 6e64  opular data hand
 00000110: 6c69 6e67 206c 6962 7261 7279 2050 616e  ling library Pan
```

### Comparing `qbandas-1.0.4/PKG-INFO` & `qbandas-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbandas
-Version: 1.0.4
+Version: 1.1.0
 Summary: Integrates the popular data handling library Pandas and the QuickBase API
 Project-URL: Homepage, https://github.com/jhopwood-jjk/qBandas
 Author: Joshua Hopwood
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

