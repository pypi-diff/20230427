# Comparing `tmp/Geode_Viewables-2.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Viewables-2.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 3774 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      101 b- defN 23-Apr-14 09:42 geode_viewables/__init__.py
--rw-rw-rw-  2.0 fat     1284 b- defN 23-Apr-14 09:42 geode_viewables/conversion.py
--rw-rw-rw-  2.0 fat     1251 b- defN 23-Apr-14 09:42 geode_viewables/qem_proxy.py
--rw-rw-rw-  2.0 fat     1965 b- defN 23-Apr-14 09:43 Geode_Viewables-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 09:43 Geode_Viewables-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-14 09:43 Geode_Viewables-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      585 b- defN 23-Apr-14 09:43 Geode_Viewables-2.0.0.dist-info/RECORD
-7 files, 5302 bytes uncompressed, 2732 bytes compressed:  48.5%
+Zip file size: 156068 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      202 b- defN 23-Apr-27 11:27 geode_viewables/__init__.py
+-rw-rw-rw-  2.0 fat     1284 b- defN 23-Apr-27 11:27 geode_viewables/conversion.py
+-rw-rw-rw-  2.0 fat     1251 b- defN 23-Apr-27 11:27 geode_viewables/qem_proxy.py
+-rw-rw-rw-  2.0 fat    27648 b- defN 23-Apr-27 11:27 geode_viewables/bin/Geode-Viewables_conversion.dll
+-rw-rw-rw-  2.0 fat    56320 b- defN 23-Apr-27 11:27 geode_viewables/bin/Geode-Viewables_qem_proxy.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Apr-27 11:27 geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   126464 b- defN 23-Apr-27 11:27 geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1965 b- defN 23-Apr-27 11:27 Geode_Viewables-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-27 11:27 Geode_Viewables-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-27 11:27 Geode_Viewables-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1053 b- defN 23-Apr-27 11:27 Geode_Viewables-2.0.1.dist-info/RECORD
+11 files, 369903 bytes uncompressed, 154254 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -3,20 +3,32 @@
 
 Filename: geode_viewables/conversion.py
 Comment: 
 
 Filename: geode_viewables/qem_proxy.py
 Comment: 
 
-Filename: Geode_Viewables-2.0.0.dist-info/METADATA
+Filename: geode_viewables/bin/Geode-Viewables_conversion.dll
 Comment: 
 
-Filename: Geode_Viewables-2.0.0.dist-info/WHEEL
+Filename: geode_viewables/bin/Geode-Viewables_qem_proxy.dll
 Comment: 
 
-Filename: Geode_Viewables-2.0.0.dist-info/top_level.txt
+Filename: geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Viewables-2.0.0.dist-info/RECORD
+Filename: geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
+Comment: 
+
+Filename: Geode_Viewables-2.0.1.dist-info/METADATA
+Comment: 
+
+Filename: Geode_Viewables-2.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_Viewables-2.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_Viewables-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_viewables/__init__.py

```diff
@@ -1,4 +1,7 @@
 ## Copyright (c) 2019 - 2023 Geode-solutions
 
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
 from .conversion import *
 from .qem_proxy import *
```

## Comparing `Geode_Viewables-2.0.0.dist-info/METADATA` & `Geode_Viewables-2.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Viewables
-Version: 2.0.0
+Version: 2.0.1
 Summary: Geode module to objects visualization
 Home-page: https://github.com/Geode-solutions/Geode-Viewables
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-Viewables Version: 2.0.0 Summary: Geode
+Metadata-Version: 2.1 Name: Geode-Viewables Version: 2.0.1 Summary: Geode
 module to objects visualization Home-page: https://github.com/Geode-solutions/
 Geode-Viewables Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
 text/markdown Requires-Dist: geode-common (==25.*,>=25.0.0) Requires-Dist:
 opengeode-core (==14.*,>=14.0.0) Requires-Dist: opengeode-geosciences
 (==7.*,>=7.0.0) Requires-Dist: opengeode-io (==6.*,>=6.0.0)
                 ****** Geode-Viewablesby Geode-solutions ******
```

