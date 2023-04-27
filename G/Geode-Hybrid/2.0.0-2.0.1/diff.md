# Comparing `tmp/Geode_Hybrid-2.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Hybrid-2.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2277 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       69 b- defN 23-Apr-14 09:39 geode_hybrid/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 23-Apr-14 09:39 geode_hybrid/brep.py
--rw-rw-rw-  2.0 fat     2183 b- defN 23-Apr-14 09:39 Geode_Hybrid-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 09:39 Geode_Hybrid-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-14 09:39 Geode_Hybrid-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      474 b- defN 23-Apr-14 09:39 Geode_Hybrid-2.0.0.dist-info/RECORD
-6 files, 3073 bytes uncompressed, 1415 bytes compressed:  54.0%
+Zip file size: 1112118 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      170 b- defN 23-Apr-27 11:36 geode_hybrid/__init__.py
+-rw-rw-rw-  2.0 fat      234 b- defN 23-Apr-27 11:36 geode_hybrid/brep.py
+-rw-rw-rw-  2.0 fat  2167296 b- defN 23-Apr-27 11:36 geode_hybrid/bin/Geode-Hybrid_brep.dll
+-rw-rw-rw-  2.0 fat   136704 b- defN 23-Apr-27 11:36 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2183 b- defN 23-Apr-27 11:36 Geode_Hybrid-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-27 11:36 Geode_Hybrid-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-27 11:36 Geode_Hybrid-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      688 b- defN 23-Apr-27 11:36 Geode_Hybrid-2.0.1.dist-info/RECORD
+8 files, 2307388 bytes uncompressed, 1110916 bytes compressed:  51.9%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: geode_hybrid/__init__.py
 Comment: 
 
 Filename: geode_hybrid/brep.py
 Comment: 
 
-Filename: Geode_Hybrid-2.0.0.dist-info/METADATA
+Filename: geode_hybrid/bin/Geode-Hybrid_brep.dll
 Comment: 
 
-Filename: Geode_Hybrid-2.0.0.dist-info/WHEEL
+Filename: geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Hybrid-2.0.0.dist-info/top_level.txt
+Filename: Geode_Hybrid-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Hybrid-2.0.0.dist-info/RECORD
+Filename: Geode_Hybrid-2.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_Hybrid-2.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_Hybrid-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_hybrid/__init__.py

```diff
@@ -1,3 +1,6 @@
 ## Copyright (c) 2019 - 2023 Geode-solutions
 
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
 from .brep import *
```

## Comparing `Geode_Hybrid-2.0.0.dist-info/METADATA` & `Geode_Hybrid-2.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Hybrid
-Version: 2.0.0
+Version: 2.0.1
 Summary: Hybrid remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-Hybrid
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.0 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.0.1 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
 text/markdown Requires-Dist: geode-common (==25.*,>=25.0.0) Requires-Dist:
 geode-numerics (==3.*,>=3.0.0) Requires-Dist: geode-simplex (==6.*,>=6.0.1)
 Requires-Dist: opengeode-core (==14.*,>=14.0.0)
          ****** Geode-ModuleTemplate_privateby Geode-solutions ******
```

