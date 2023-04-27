# Comparing `tmp/Geode_SimplexGeosciences-2.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_SimplexGeosciences-2.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 3290 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      111 b- defN 23-Apr-14 08:57 geode_simplexgeosciences/__init__.py
--rw-rw-rw-  2.0 fat      261 b- defN 23-Apr-14 08:57 geode_simplexgeosciences/cross_section.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-Apr-14 08:57 geode_simplexgeosciences/structural_model.py
--rw-rw-rw-  2.0 fat     3330 b- defN 23-Apr-14 08:57 Geode_SimplexGeosciences-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 08:57 Geode_SimplexGeosciences-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-14 08:57 Geode_SimplexGeosciences-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      656 b- defN 23-Apr-14 08:57 Geode_SimplexGeosciences-2.0.0.dist-info/RECORD
-7 files, 4750 bytes uncompressed, 2102 bytes compressed:  55.7%
+Zip file size: 2125209 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      212 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/__init__.py
+-rw-rw-rw-  2.0 fat      261 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/cross_section.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/structural_model.py
+-rw-rw-rw-  2.0 fat  2039296 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll
+-rw-rw-rw-  2.0 fat  2039296 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3330 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1220 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/RECORD
+11 files, 4358439 bytes uncompressed, 2123065 bytes compressed:  51.3%
```

## zipnote {}

```diff
@@ -3,20 +3,32 @@
 
 Filename: geode_simplexgeosciences/cross_section.py
 Comment: 
 
 Filename: geode_simplexgeosciences/structural_model.py
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.0.dist-info/METADATA
+Filename: geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.0.dist-info/WHEEL
+Filename: geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.0.dist-info/top_level.txt
+Filename: geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.0.dist-info/RECORD
+Filename: geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
+Comment: 
+
+Filename: Geode_SimplexGeosciences-2.0.1.dist-info/METADATA
+Comment: 
+
+Filename: Geode_SimplexGeosciences-2.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: Geode_SimplexGeosciences-2.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: Geode_SimplexGeosciences-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_simplexgeosciences/__init__.py

```diff
@@ -1,4 +1,7 @@
 ## Copyright (c) 2019 - 2023 Geode-solutions
 
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
 from .cross_section import *
 from .structural_model import *
```

## Comparing `Geode_SimplexGeosciences-2.0.0.dist-info/METADATA` & `Geode_SimplexGeosciences-2.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-SimplexGeosciences
-Version: 2.0.0
+Version: 2.0.1
 Summary: Geosciences simplex remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-SimplexGeosciences
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-SimplexGeosciences Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: Geode-SimplexGeosciences Version: 2.0.1 Summary:
 Geosciences simplex remeshing Geode-solutions OpenGeode module Home-page:
 https://github.com/Geode-solutions/Geode-SimplexGeosciences Author: Geode-
 solutions Author-email: contact@geode-solutions.com License: Proprietary
 Platform: UNKNOWN Description-Content-Type: text/markdown Requires-Dist: geode-
 common (==25.*,>=25.0.0) Requires-Dist: geode-numerics (==3.*,>=3.0.0)
 Requires-Dist: geode-simplex (==6.*,>=6.0.1) Requires-Dist: opengeode-core
 (==14.*,>=14.0.0) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
```

