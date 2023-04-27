# Comparing `tmp/onf_parser-0.2.0-py2.py3-none-any.whl.zip` & `tmp/onf_parser-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8812 bytes, number of entries: 9
+Zip file size: 8819 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      639 b- defN 23-Feb-23 18:20 onf_parser/__init__.py
--rw-rw-r--  2.0 unx     7477 b- defN 23-Mar-14 20:04 onf_parser/models.py
+-rw-rw-r--  2.0 unx     7502 b- defN 23-Apr-25 22:55 onf_parser/models.py
 -rw-rw-r--  2.0 unx     9954 b- defN 23-Mar-13 19:28 onf_parser/parse.py
--rw-rw-r--  2.0 unx       79 b- defN 23-Mar-14 20:05 onf_parser-0.2.0.dist-info/AUTHORS.rst
--rw-rw-r--  2.0 unx     1079 b- defN 23-Mar-14 20:05 onf_parser-0.2.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     3772 b- defN 23-Mar-14 20:05 onf_parser-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Mar-14 20:05 onf_parser-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Mar-14 20:05 onf_parser-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      730 b- defN 23-Mar-14 20:05 onf_parser-0.2.0.dist-info/RECORD
-9 files, 23851 bytes uncompressed, 7552 bytes compressed:  68.3%
+-rw-rw-r--  2.0 unx       79 b- defN 23-Apr-27 19:54 onf_parser-0.2.1.dist-info/AUTHORS.rst
+-rw-rw-r--  2.0 unx     1079 b- defN 23-Apr-27 19:54 onf_parser-0.2.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     3772 b- defN 23-Apr-27 19:54 onf_parser-0.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-27 19:54 onf_parser-0.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Apr-27 19:54 onf_parser-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      730 b- defN 23-Apr-27 19:54 onf_parser-0.2.1.dist-info/RECORD
+9 files, 23876 bytes uncompressed, 7559 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: onf_parser/models.py
 Comment: 
 
 Filename: onf_parser/parse.py
 Comment: 
 
-Filename: onf_parser-0.2.0.dist-info/AUTHORS.rst
+Filename: onf_parser-0.2.1.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: onf_parser-0.2.0.dist-info/LICENSE.txt
+Filename: onf_parser-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: onf_parser-0.2.0.dist-info/METADATA
+Filename: onf_parser-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: onf_parser-0.2.0.dist-info/WHEEL
+Filename: onf_parser-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: onf_parser-0.2.0.dist-info/top_level.txt
+Filename: onf_parser-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: onf_parser-0.2.0.dist-info/RECORD
+Filename: onf_parser-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onf_parser/models.py

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import List, Optional, Tuple, Dict
 
-from nltk import Tree
+from nltk.tree import Tree as NltkTree
 
 
 @dataclass
 class PlainSentence:
     """
     The untokenized sentence as it originally appeared in the source material, or transcribed with typical
     English orthographic conventions.
@@ -58,19 +58,19 @@
         tree_string: str - S-expression formatted PTB tree.
         parsed_tree: Tree - nltk.tree.Tree instance
     """
 
     tree_string: str
 
     @property
-    def parsed_tree(self) -> Tree:
+    def parsed_tree(self) -> NltkTree:
         if hasattr(self, "__parsed_tree"):
             return self.__parsed_tree
         else:
-            t = Tree.fromstring(self.tree_string)
+            t = NltkTree.fromstring(self.tree_string)
             self.__parsed_tree = t
             return t
 
 
 @dataclass
 class PropArg:
     """
```

## Comparing `onf_parser-0.2.0.dist-info/LICENSE.txt` & `onf_parser-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `onf_parser-0.2.0.dist-info/METADATA` & `onf_parser-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onf-parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: OntoNotes Normal Form Parser
 Home-page: https://github.com/lgessler/onf-parser
 Author: Luke Gessler
 Author-email: lukegessler@gmail.com
 License: mit
 Project-URL: Documentation, https://github.com/lgessler/onf-parser
 Platform: any
```

