# Comparing `tmp/tralda-1.0.1.tar.gz` & `tmp/tralda-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tralda-1.0.1.tar", last modified: Wed May  4 09:33:28 2022, max compression
+gzip compressed data, was "tralda-1.1.0.tar", last modified: Thu Apr 27 17:12:56 2023, max compression
```

## Comparing `tralda-1.0.1.tar` & `tralda-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.475747 tralda-1.0.1/
--rw-r--r--   0 david      (501) staff       (20)    35149 2021-06-30 12:32:57.000000 tralda-1.0.1/LICENSE
--rw-r--r--   0 david      (501) staff       (20)     8632 2022-05-04 09:33:28.475868 tralda-1.0.1/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     8036 2022-05-04 08:05:36.000000 tralda-1.0.1/README.md
--rw-r--r--   0 david      (501) staff       (20)       85 2022-05-04 09:20:26.000000 tralda-1.0.1/pyproject.toml
--rw-r--r--   0 david      (501) staff       (20)      721 2022-05-04 09:33:28.476336 tralda-1.0.1/setup.cfg
--rwxr-xr-x   0 david      (501) staff       (20)       99 2022-05-04 09:10:56.000000 tralda-1.0.1/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.466315 tralda-1.0.1/src/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.467955 tralda-1.0.1/src/tralda/
--rwxr-xr-x   0 david      (501) staff       (20)       23 2021-01-11 15:57:42.000000 tralda-1.0.1/src/tralda/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.469988 tralda-1.0.1/src/tralda/cograph/
--rwxr-xr-x   0 david      (501) staff       (20)     3844 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/cograph/ClusterDeletion.py
--rwxr-xr-x   0 david      (501) staff       (20)    15957 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/cograph/Cograph.py
--rwxr-xr-x   0 david      (501) staff       (20)    21328 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/cograph/CographEditor.py
--rwxr-xr-x   0 david      (501) staff       (20)      499 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/cograph/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.472835 tralda-1.0.1/src/tralda/datastructures/
--rwxr-xr-x   0 david      (501) staff       (20)    20575 2020-12-17 13:04:17.000000 tralda-1.0.1/src/tralda/datastructures/AVLTree.py
--rwxr-xr-x   0 david      (501) staff       (20)    11835 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/datastructures/DoublyLinkedList.py
--rwxr-xr-x   0 david      (501) staff       (20)     6441 2020-12-17 13:04:17.000000 tralda-1.0.1/src/tralda/datastructures/LinkedList.py
--rwxr-xr-x   0 david      (501) staff       (20)     1936 2021-06-30 13:30:34.000000 tralda-1.0.1/src/tralda/datastructures/Partition.py
--rwxr-xr-x   0 david      (501) staff       (20)    46343 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/datastructures/Tree.py
--rw-r--r--   0 david      (501) staff       (20)      353 2021-06-30 15:25:03.000000 tralda-1.0.1/src/tralda/datastructures/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.473684 tralda-1.0.1/src/tralda/datastructures/hdtgraph/
--rwxr-xr-x   0 david      (501) staff       (20)    14468 2021-06-30 13:27:57.000000 tralda-1.0.1/src/tralda/datastructures/hdtgraph/DynamicGraph.py
--rwxr-xr-x   0 david      (501) staff       (20)    33795 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/datastructures/hdtgraph/ETTree.py
--rwxr-xr-x   0 david      (501) staff       (20)       24 2020-12-17 13:04:17.000000 tralda-1.0.1/src/tralda/datastructures/hdtgraph/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.474843 tralda-1.0.1/src/tralda/supertree/
--rwxr-xr-x   0 david      (501) staff       (20)    16753 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/supertree/Build.py
--rwxr-xr-x   0 david      (501) staff       (20)    15192 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/supertree/BuildST.py
--rwxr-xr-x   0 david      (501) staff       (20)     6934 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/supertree/CommonRefinement.py
--rwxr-xr-x   0 david      (501) staff       (20)     9359 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/supertree/LooseConsensus.py
--rwxr-xr-x   0 david      (501) staff       (20)      704 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/supertree/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.475485 tralda-1.0.1/src/tralda/tools/
--rwxr-xr-x   0 david      (501) staff       (20)     8852 2021-01-11 15:57:42.000000 tralda-1.0.1/src/tralda/tools/GraphTools.py
--rwxr-xr-x   0 david      (501) staff       (20)     1377 2021-09-28 15:42:10.000000 tralda-1.0.1/src/tralda/tools/TreeTools.py
--rwxr-xr-x   0 david      (501) staff       (20)       23 2022-05-04 08:05:36.000000 tralda-1.0.1/src/tralda/tools/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-05-04 09:33:28.468757 tralda-1.0.1/src/tralda.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     8632 2022-05-04 09:33:28.000000 tralda-1.0.1/src/tralda.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     1020 2022-05-04 09:33:28.000000 tralda-1.0.1/src/tralda.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2022-05-04 09:33:28.000000 tralda-1.0.1/src/tralda.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       15 2022-05-04 09:33:28.000000 tralda-1.0.1/src/tralda.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)        7 2022-05-04 09:33:28.000000 tralda-1.0.1/src/tralda.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.657585 tralda-1.1.0/
+-rw-r--r--   0 david      (501) staff       (20)     1058 2023-04-27 17:11:34.000000 tralda-1.1.0/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)     8565 2023-04-27 17:12:56.657671 tralda-1.1.0/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     8032 2023-04-27 17:11:34.000000 tralda-1.1.0/README.md
+-rw-r--r--   0 david      (501) staff       (20)       85 2022-05-04 09:37:34.000000 tralda-1.1.0/pyproject.toml
+-rw-r--r--   0 david      (501) staff       (20)      695 2023-04-27 17:12:56.658043 tralda-1.1.0/setup.cfg
+-rwxr-xr-x   0 david      (501) staff       (20)       99 2022-05-04 09:37:34.000000 tralda-1.1.0/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.649974 tralda-1.1.0/src/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.651240 tralda-1.1.0/src/tralda/
+-rwxr-xr-x   0 david      (501) staff       (20)       23 2021-01-11 15:57:42.000000 tralda-1.1.0/src/tralda/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.653423 tralda-1.1.0/src/tralda/cograph/
+-rwxr-xr-x   0 david      (501) staff       (20)     3844 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/cograph/ClusterDeletion.py
+-rwxr-xr-x   0 david      (501) staff       (20)    15957 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/cograph/Cograph.py
+-rwxr-xr-x   0 david      (501) staff       (20)    21328 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/cograph/CographEditor.py
+-rwxr-xr-x   0 david      (501) staff       (20)      499 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/cograph/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.654917 tralda-1.1.0/src/tralda/datastructures/
+-rwxr-xr-x   0 david      (501) staff       (20)    20575 2020-12-17 13:04:17.000000 tralda-1.1.0/src/tralda/datastructures/AVLTree.py
+-rwxr-xr-x   0 david      (501) staff       (20)    11835 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/datastructures/DoublyLinkedList.py
+-rwxr-xr-x   0 david      (501) staff       (20)     6441 2020-12-17 13:04:17.000000 tralda-1.1.0/src/tralda/datastructures/LinkedList.py
+-rwxr-xr-x   0 david      (501) staff       (20)     1936 2021-06-30 13:30:34.000000 tralda-1.1.0/src/tralda/datastructures/Partition.py
+-rwxr-xr-x   0 david      (501) staff       (20)    52182 2023-04-27 17:11:34.000000 tralda-1.1.0/src/tralda/datastructures/Tree.py
+-rw-r--r--   0 david      (501) staff       (20)      353 2021-06-30 15:25:03.000000 tralda-1.1.0/src/tralda/datastructures/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.655717 tralda-1.1.0/src/tralda/datastructures/hdtgraph/
+-rwxr-xr-x   0 david      (501) staff       (20)    14468 2021-06-30 13:27:57.000000 tralda-1.1.0/src/tralda/datastructures/hdtgraph/DynamicGraph.py
+-rwxr-xr-x   0 david      (501) staff       (20)    33795 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/datastructures/hdtgraph/ETTree.py
+-rwxr-xr-x   0 david      (501) staff       (20)       24 2020-12-17 13:04:17.000000 tralda-1.1.0/src/tralda/datastructures/hdtgraph/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.656672 tralda-1.1.0/src/tralda/supertree/
+-rwxr-xr-x   0 david      (501) staff       (20)    16753 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/supertree/Build.py
+-rwxr-xr-x   0 david      (501) staff       (20)    15192 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/supertree/BuildST.py
+-rwxr-xr-x   0 david      (501) staff       (20)     6934 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/supertree/CommonRefinement.py
+-rwxr-xr-x   0 david      (501) staff       (20)     9359 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/supertree/LooseConsensus.py
+-rwxr-xr-x   0 david      (501) staff       (20)      704 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/supertree/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.657340 tralda-1.1.0/src/tralda/tools/
+-rwxr-xr-x   0 david      (501) staff       (20)     8852 2021-01-11 15:57:42.000000 tralda-1.1.0/src/tralda/tools/GraphTools.py
+-rwxr-xr-x   0 david      (501) staff       (20)     1377 2021-09-28 15:42:10.000000 tralda-1.1.0/src/tralda/tools/TreeTools.py
+-rwxr-xr-x   0 david      (501) staff       (20)       23 2022-05-04 08:05:36.000000 tralda-1.1.0/src/tralda/tools/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-04-27 17:12:56.652458 tralda-1.1.0/src/tralda.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     8565 2023-04-27 17:12:56.000000 tralda-1.1.0/src/tralda.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     1020 2023-04-27 17:12:56.000000 tralda-1.1.0/src/tralda.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-04-27 17:12:56.000000 tralda-1.1.0/src/tralda.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)       15 2023-04-27 17:12:56.000000 tralda-1.1.0/src/tralda.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)        7 2023-04-27 17:12:56.000000 tralda-1.1.0/src/tralda.egg-info/top_level.txt
```

### Comparing `tralda-1.0.1/PKG-INFO` & `tralda-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: tralda
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library for tree data structures and algorithms
 Home-page: https://github.com/david-schaller/tralda
 Author: David Schaller
 Author-email: sdavid@bioinf.uni-leipzig.de
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/david-schaller/tralda/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tralda
 
-[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/badge/pypi-v1.0.1-blue.svg)](https://pypi.org/project/tralda/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi version](https://img.shields.io/badge/pypi-v1.1.0-blue.svg)](https://pypi.org/project/tralda/)
 
 A Python library for **tr**ee **al**gorithms and **da**ta structures.
 
 ## Installation
 
 The package requires Python 3.7 or higher.
 
@@ -171,9 +169,7 @@
 
 * **Schaller, D., Hellmuth, M., Stadler, P.F. (2021) A Simple Linear-Time Algorithm for the Common Refinement of Rooted Phylogenetic Trees on a Common Leaf Set.**
 
 Additional references to algorithms that were implemented are given in the source code.
 
 Please report any bugs and questions in the [Issues](https://github.com/david-schaller/tralda/issues) section.
 Also, feel free to make suggestions for improvement and/or new functionalities.
-
-
```

### Comparing `tralda-1.0.1/README.md` & `tralda-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # tralda
 
-[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/badge/pypi-v1.0.1-blue.svg)](https://pypi.org/project/tralda/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi version](https://img.shields.io/badge/pypi-v1.1.0-blue.svg)](https://pypi.org/project/tralda/)
 
 A Python library for **tr**ee **al**gorithms and **da**ta structures.
 
 ## Installation
 
 The package requires Python 3.7 or higher.
```

### Comparing `tralda-1.0.1/setup.cfg` & `tralda-1.1.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = tralda
-version = 1.0.1
+version = 1.1.0
 author = David Schaller
 author_email = sdavid@bioinf.uni-leipzig.de
 description = A library for tree data structures and algorithms
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/david-schaller/tralda
 project_urls = 
 	Bug Tracker = https://github.com/david-schaller/tralda/issues
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
```

### Comparing `tralda-1.0.1/src/tralda/cograph/ClusterDeletion.py` & `tralda-1.1.0/src/tralda/cograph/ClusterDeletion.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/cograph/Cograph.py` & `tralda-1.1.0/src/tralda/cograph/Cograph.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/cograph/CographEditor.py` & `tralda-1.1.0/src/tralda/cograph/CographEditor.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/datastructures/AVLTree.py` & `tralda-1.1.0/src/tralda/datastructures/AVLTree.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/datastructures/DoublyLinkedList.py` & `tralda-1.1.0/src/tralda/datastructures/DoublyLinkedList.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/datastructures/LinkedList.py` & `tralda-1.1.0/src/tralda/datastructures/LinkedList.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/datastructures/Partition.py` & `tralda-1.1.0/src/tralda/datastructures/Partition.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/datastructures/Tree.py` & `tralda-1.1.0/src/tralda/datastructures/Tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,15 @@
     def __str__(self):
         
         return str(self.label) if hasattr(self, 'label') else ''
     
     
     def __repr__(self):
         
-        return '<TN: {}>'.format(self.label if hasattr(self, 'label') 
-                                            else id(self))
+        return f'<TN: {self.label if hasattr(self, "label") else id(self)}>'
     
     
     def attributes(self):
         """A generator for the node attributes.
         
         Yields
         ------
@@ -102,16 +101,15 @@
         child_node : TreeNode
             The node to add as a new child to this node.
         right_of : TreeNode
             The child of this node right of which 'child_node' gets inserted.
         """
         
         if right_of.parent is not self:
-            return KeyError('{} is not a child of node {}'.format(right_of,
-                                                                  self))
+            return KeyError(f'{right_of} is not a child of node {self}')
         
         if child_node.parent is not None:
             child_node.parent.remove_child(child_node)
             
         child_node.parent = self
         child_node._par_dll_node = \
             self.children.insert_right_of(right_of._par_dll_node, child_node)
@@ -132,16 +130,15 @@
         """
         
         if child_node.parent is self:
             self.children.remove_node(child_node._par_dll_node)
             child_node.parent = None
             child_node._par_dll_node = None
         else:
-            raise KeyError('{} is not a child of node {}'.format(child_node,
-                                                                 self))
+            raise KeyError(f'{child_node} is not a child of node {self}')
             
             
     def detach(self):
         """Detach this node from its parent.
         
         The node has no parent afterwards.
         """
@@ -183,47 +180,49 @@
         Raises
         ------
         KeyError
             If 'right_node' or 'left_node' is not a child of this node.
         """
         
         if left_node.parent is not self:
-            raise KeyError('{} is not a child of node {}'.format(left_node,
-                                                                 self))
+            raise KeyError(f'{left_node} is not a child of node {self}')
         if right_node.parent is not self:
-            raise KeyError('{} is not a child of node {}'.format(right_node,
-                                                                 self))
+            raise KeyError(f'{right_node} is not a child of node {self}')
         
         return self.children.sublist(left_node._par_dll_node,
                                      right_node._par_dll_node)
         
 
 class Tree:
-    """Basic class for trees.
+    """Rooted tree whose nodes may have an arbitrary number of children.
     
     Attributes
     ----------
     root : TreeNode
         The root node of the tree.
     """
     
-    # corresponding node type
-    node_type = TreeNode
     
-    
-    def __init__(self, root):
+    def __init__(self, arg):
         """Constructor for the class tree.
         
         Parameters
         ----------
-        root : TreeNode
-            The root node for the newly created tree.
+        arg : TreeNode or str
+            The root node for the newly created tree or a Newick representation
+            of a tree.
         """
         
-        self.root = root
+        if isinstance(arg, TreeNode) or arg is None:
+            self.root = arg
+        elif isinstance(arg, str):
+            self.root = Tree._parse_newick_and_return_root(arg)
+        else:
+            raise TypeError(f'Tree cannot be initialized with argument of type '
+                            f'{type(arg)}')
         
     
     def leaves(self):
         """Generator for leaves of the tree.
         
         Yields
         ------
@@ -524,14 +523,17 @@
                         for a, b in itertools.combinations(leaves[v2], 2):
                             yield a, b, c
     
     
     def delete_and_reconnect(self, node):
         """Delete a node from the tree and reconnect its parent and children.
         
+        This function preserves the 'sibling order' of the remaining nodes
+        of the tree.
+        
         Parameters
         ----------
         node : TreeNode
             The node to be deleted.
         
         Returns
         -------
@@ -540,57 +542,26 @@
             node could not be deleted, i.e., it has no parent.
         """
         
         parent = node.parent
         if not parent:
             return False
         else:
-            parent.remove_child(node)
-            
             # copy list of children to edit edges
             children = [child for child in node.children]
+            
             for child in children:
-                parent.add_child(child)
-                    
+                parent.add_child_right_of(child, node)
+            
+            parent.remove_child(node)
             node.children.clear()
         
         return parent
         
     
-    def to_newick(self, node=None):
-        """Newick representation of the tree.
-        
-        Parameters
-        ----------
-        node : TreeNode, optional
-            The node whose subtree shall be returned as a Newick string, the
-            default is None, in which case the whole tree is returned in Newick
-            format.
-        
-        Returns
-        -------
-        str
-            A newick representation of the (sub)tree.
-        """
-        
-        def _to_newick(node):
-            if not node.children:
-                return str(node)
-            else:
-                s = ''
-                for child in node.children:
-                    s += _to_newick(child) + ','
-                return "({}){}".format(s[:-1], node)
-        
-        if self.root:
-            return _to_newick(self.root) + ';'
-        else:
-            return ';'
-        
-    
     def random_leaves(self, proportion):
         """A random sample of the leaves.
         
         Parameters
         ----------
         proportion : float
             The proportion of the sample w.r.t. the full set of leaves.
@@ -756,18 +727,17 @@
     
     
     def _assert_integrity(self):
         
         for v in self.preorder():
             for child in v.children:
                 if child is v:
-                    raise RuntimeError('loop at {}'.format(v))
+                    raise RuntimeError(f'loop at {v}')
                 if child.parent is not v:
-                    raise RuntimeError('Tree invalid for '\
-                                       '{} and {}'.format(v, child))
+                    raise RuntimeError(f'Tree invalid for {v} and {child}')
         
         return True
     
     
     def copy(self, mapping=False):
         """Return a copy of the tree.
         
@@ -805,14 +775,198 @@
             for key, value in orig.attributes():
                 setattr(new, key, value)
         
         if mapping:
             return Tree(orig_to_new[self.root]), orig_to_new
         else:
             return Tree(orig_to_new[self.root])
+
+
+# --------------------------------------------------------------------------
+#                         TREE  <--->  NEWICK
+# --------------------------------------------------------------------------
+
+    def to_newick(self, node=None):
+        """Newick representation of the tree.
+        
+        Parameters
+        ----------
+        node : TreeNode, optional
+            The node whose subtree shall be returned as a Newick string, the
+            default is None, in which case the whole tree is returned in Newick
+            format.
+        
+        Returns
+        -------
+        str
+            A newick representation of the (sub)tree.
+        """
+        
+        def _to_newick(node):
+            
+            node_str = str(node)
+            
+            # add colon and distance if available
+            if hasattr(node, 'dist'):
+                node_str += f':{node.dist}'
+            
+            if not node.children:
+                return node_str
+            else:
+                s = ''
+                for child in node.children:
+                    s += _to_newick(child) + ','
+                return f'({s[:-1]}){node_str}'
+        
+        if self.root:
+            return _to_newick(self.root) + ';'
+        else:
+            return ';'
+    
+    
+    @staticmethod
+    def _parse_newick_and_return_root(newick):
+        """Parses trees in Newick format and returns the root.
+        
+        If available (after colons in the Newick strings), the distance is 
+        stored in the 'dist' attribute of the nodes. Moreover, labels are
+        converted to integers if possible.
+        
+        Parameters
+        ----------
+        newick : str
+            A tree in Newick format.
+        
+        Returns
+        -------
+        TreeNode
+            The root of the parsed tree.
+        
+        Raises
+        ------
+        TypeError
+            If the input is not a string.
+        ValueError
+            If the input is not a valid Newick string.
+        """
+        
+        def _parse_subtree(subroot, subtree_string):
+            """Recursive function to parse the subtrees."""
+            
+            children = _split_children(subtree_string)
+            
+            for child in children:
+                
+                node = TreeNode()
+                subroot.add_child(node)
+                end = -1
+                
+                # the child has subtrees
+                if child[0] == '(':
+                    end = child.rfind(')')
+                    if end == -1:
+                        raise ValueError('invalid Newick string')
+                    # recursive call
+                    _parse_subtree(node, child[1:end])               
+                    
+                child = child[end+1:].strip()
+                
+                label = child
+                
+                if child.find(':') != -1:
+                    label, dist = child.rsplit(':', 1)
+                    
+                    try:
+                        node.dist = float(dist)
+                    except ValueError:
+                        raise ValueError('invalid distance in Newick string: ' \
+                                         f'{dist}')
+                
+                # convert label to integer if possible
+                node.label = int(label) if label.isdigit() else label
+                    
+                        
+        def _split_children(child_string):
+            """Splits a given string by all ',' that are not enclosed by 
+            parentheses.
+            """
+            
+            stack = 0
+            children = []
+            current = ''
+            
+            for c in child_string:
+                if (stack == 0) and c == ',':
+                    children.append(current)
+                    current = ''
+                elif c == '(':
+                    stack += 1
+                    current += c
+                elif c == ')':
+                    if stack <= 0:
+                        raise ValueError('invalid Newick string')
+                    stack -= 1
+                    current += c
+                else:
+                    current += c
+                    
+            children.append(current.strip())
+            return children
+        
+        if not isinstance(newick, str):
+            raise TypeError("Newick parser needs a 'str' as input")
+            
+        end = newick.find(';')
+        if end != -1:
+            newick = newick[:end]
+        
+        temp_root = TreeNode()
+        _parse_subtree(temp_root, newick)
+        
+        if temp_root.children:
+            root = temp_root.children[0]
+            # remove the parent temp_root
+            root.detach()
+            return root
+        else:
+            raise ValueError('invalid Newick string')
+    
+    
+    @staticmethod
+    def parse_newick(newick):
+        """Parses trees in Newick format into object of type 'Tree'.
+        
+        If available (after colons in the Newick strings), the distance is 
+        stored in the 'dist' attribute of the nodes. Moreover, labels are
+        converted to integers if possible.
+        
+        Parameters
+        ----------
+        newick : str
+            A tree in Newick format.
+        
+        Returns
+        -------
+        Tree
+            The parsed tree.
+        
+        Raises
+        ------
+        TypeError
+            If the input is not a string.
+        ValueError
+            If the input is not a valid Newick string.
+        
+        Notes
+        -----
+        Do not use this function for serialization and reloading Tree
+        objects. Use the `serialize()` function instead.
+        """
+        
+        return Tree(Tree._parse_newick_and_return_root(newick))
     
     
 # --------------------------------------------------------------------------
 #                         TREE  <--->  NETWORKX
 # --------------------------------------------------------------------------
             
     def to_nx(self):
@@ -840,35 +994,35 @@
         for v in self.preorder():
             G.add_node(id(v))
             for key, value in v.attributes():
                 G.nodes[id(v)][key] = value
         
         for u, v, sibling_nr in self.edges_sibling_order():
             if u is v:
-                raise RuntimeError('loop at {} and {}'.format(u, v))
+                raise RuntimeError(f'loop at {u} and {v}')
             G.add_edge(id(u), id(v))
             G.nodes[id(v)]['sibling_nr'] = sibling_nr
             
         return G, id(self.root)
     
     
     @staticmethod
     def parse_nx(G, root):
-        """Convert a NetworkX Graph version back into a PhyloTree.
+        """Convert a NetworkX Graph version back into a Tree.
         
         Parameters
         ----------
         G : networkx.Graph
             A tree represented as a Networkx Graph.
         root : int
             The node in the graph corresponding to the root.
         
         Returns
         -------
-        PhyloTree
+        Tree
             The reconstructed tree.
         """
         
         number_of_leaves = 0
         
         if root is None:
             return Tree(None)
@@ -899,14 +1053,74 @@
         tree.number_of_species = number_of_leaves
         
         return tree
 
 # --------------------------------------------------------------------------
 #                           SERIALIZATION
 # --------------------------------------------------------------------------
+
+    def to_dict(self):
+        """Convert the tree into a nested dictionary.
+        
+        Raises
+        ------
+        RuntimeError
+            If the tree is empty.
+        """
+        
+        def _to_dict(node):
+            
+            node_dict = {k: v for k, v in node.attributes()}
+            
+            for i, child in enumerate(node.children):
+                node_dict[f'_child{i}'] = _to_dict(child)
+            
+            return node_dict
+        
+        if self.root:
+            return _to_dict(self.root)
+        else:
+            raise RuntimeError('cannot convert empty tree to dict')
+    
+    
+    @staticmethod
+    def parse_dict(tree_dict):
+        """Convert a dictionary representation back into a Tree.
+        
+        Parameters
+        ----------
+        tree_dict : dict
+            A dictionary representation of the tree.
+        
+        Returns
+        -------
+        Tree
+            The reconstructed tree.
+        """
+        
+        def _parse_dict(node_dict):
+            
+            node = TreeNode()
+            children = {}
+            
+            for k, v in node_dict.items():
+                
+                if k.startswith('_child'):
+                    children[int(k[6:])] = _parse_dict(v)
+                else:
+                    setattr(node, k, v)
+            
+            for i in sorted(children):
+                node.add_child(children[i])
+            
+            return node
+        
+        return Tree(_parse_dict(tree_dict))
+        
+    
     
     @staticmethod
     def _infer_serialization_mode(filename):
         
         _, file_ext = os.path.splitext(filename)
         
         if file_ext.lower() == '.json':
@@ -933,33 +1147,30 @@
         ------
         ValueError
             If the serialization mode is unknown or could not be inferred.
         """
         
         if not mode:
             mode = Tree._infer_serialization_mode(filename)
-        
-        tree_nx, root_id = self.to_nx()
-        
-        if mode == 'json':
-            data = nx.readwrite.json_graph.tree_data(tree_nx, root=root_id)
             
+        if mode == 'json':
             with open(filename, 'w') as f:
-                f.write( json.dumps(data) )
+                json.dump(self.to_dict(), f)
                 
         elif mode == 'pickle':
+            tree_nx, root_id = self.to_nx()
             pickle.dump( (tree_nx, root_id), open(filename, 'wb') )
             
         else:
-            raise ValueError("serialization mode '{}' not supported".format(mode))
+            raise ValueError(f"serialization mode '{mode}' not supported")
     
     
     @staticmethod
     def load(filename, mode=None):
-        """Reload a PhyloTree from a file (pickle or json).
+        """Reload a Tree from a file (pickle or json).
         
         Parameters
         ----------
         filename : str
             The filename (including the path) of the file to be loaded.
         mode : str or None, optional
             The serialization mode. Supported are pickle and json. The default
@@ -977,36 +1188,23 @@
         """
         
         if not mode:
             mode = Tree._infer_serialization_mode(filename)
         
         if mode == 'json':
             with open(filename, 'r') as f:
-                data = json.loads( f.read() )
-                
-            tree_nx = nx.readwrite.json_graph.tree_graph(data)
-            
-            root_id = None
-            for v in tree_nx:
-                if tree_nx.in_degree(v) == 0:
-                    root_id = v
-                    break
-                
-            if root_id is None:
-                raise RuntimeError('could not identify root')
+                tree_dict = json.load(f)
+            return Tree.parse_dict(tree_dict)
                 
         elif mode == 'pickle':
-            tree_nx, root_id = pickle.load( open(filename, 'rb') )
+            return Tree.parse_nx( *pickle.load(open(filename, 'rb')) )
             
         else:
-            raise ValueError("serialization mode '{}' not supported".format(mode))
-        
-        tree = Tree.parse_nx(tree_nx, root_id)
-        
-        return tree
+            raise ValueError(f"serialization mode '{mode}' not supported")
+
 
 # --------------------------------------------------------------------------
 #                             RANDOM TREE
 # --------------------------------------------------------------------------
     
     @staticmethod
     def random_tree(N, binary=False):
```

### Comparing `tralda-1.0.1/src/tralda/datastructures/hdtgraph/DynamicGraph.py` & `tralda-1.1.0/src/tralda/datastructures/hdtgraph/DynamicGraph.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/datastructures/hdtgraph/ETTree.py` & `tralda-1.1.0/src/tralda/datastructures/hdtgraph/ETTree.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/supertree/Build.py` & `tralda-1.1.0/src/tralda/supertree/Build.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/supertree/BuildST.py` & `tralda-1.1.0/src/tralda/supertree/BuildST.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/supertree/CommonRefinement.py` & `tralda-1.1.0/src/tralda/supertree/CommonRefinement.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/supertree/LooseConsensus.py` & `tralda-1.1.0/src/tralda/supertree/LooseConsensus.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/supertree/__init__.py` & `tralda-1.1.0/src/tralda/supertree/__init__.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/tools/GraphTools.py` & `tralda-1.1.0/src/tralda/tools/GraphTools.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda/tools/TreeTools.py` & `tralda-1.1.0/src/tralda/tools/TreeTools.py`

 * *Files identical despite different names*

### Comparing `tralda-1.0.1/src/tralda.egg-info/PKG-INFO` & `tralda-1.1.0/src/tralda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: tralda
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library for tree data structures and algorithms
 Home-page: https://github.com/david-schaller/tralda
 Author: David Schaller
 Author-email: sdavid@bioinf.uni-leipzig.de
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/david-schaller/tralda/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tralda
 
-[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pypi version](https://img.shields.io/badge/pypi-v1.0.1-blue.svg)](https://pypi.org/project/tralda/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi version](https://img.shields.io/badge/pypi-v1.1.0-blue.svg)](https://pypi.org/project/tralda/)
 
 A Python library for **tr**ee **al**gorithms and **da**ta structures.
 
 ## Installation
 
 The package requires Python 3.7 or higher.
 
@@ -171,9 +169,7 @@
 
 * **Schaller, D., Hellmuth, M., Stadler, P.F. (2021) A Simple Linear-Time Algorithm for the Common Refinement of Rooted Phylogenetic Trees on a Common Leaf Set.**
 
 Additional references to algorithms that were implemented are given in the source code.
 
 Please report any bugs and questions in the [Issues](https://github.com/david-schaller/tralda/issues) section.
 Also, feel free to make suggestions for improvement and/or new functionalities.
-
-
```

### Comparing `tralda-1.0.1/src/tralda.egg-info/SOURCES.txt` & `tralda-1.1.0/src/tralda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

