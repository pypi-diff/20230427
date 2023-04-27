# Comparing `tmp/rcsb.utils.targets-0.67.tar.gz` & `tmp/rcsb.utils.targets-0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.67.tar", last modified: Thu Apr 13 16:33:31 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.68.tar", last modified: Thu Apr 27 16:15:26 2023, max compression
```

## Comparing `rcsb.utils.targets-0.67.tar` & `rcsb.utils.targets-0.68.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/
--rw-r--r--   0 vsts      (1001) docker     (122)     5758 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.911996 rcsb.utils.targets-0.67/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.911996 rcsb.utils.targets-0.67/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8379 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.911996 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 16:20:13.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-13 16:19:19.000000 rcsb.utils.targets-0.67/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-04-13 16:19:19.000000 rcsb.utils.targets-0.67/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5820 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.442173 rcsb.utils.targets-0.68/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.442173 rcsb.utils.targets-0.68/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10157 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 16:15:26.442173 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 16:03:25.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-27 16:15:26.000000 rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-04-27 16:15:26.446173 rcsb.utils.targets-0.68/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-04-27 16:02:29.000000 rcsb.utils.targets-0.68/setup.py
```

### Comparing `rcsb.utils.targets-0.67/HISTORY.txt` & `rcsb.utils.targets-0.68/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,8 +52,9 @@
    6-Jan-2023  - V0.60 Configuration changes to support tox 4
    9-Feb-2023  - V0.61 Find Highest_Clin_Trial column regardless of month in SAbDabTargetProvider(), Update baseVersion for ChEMBL
   27-Feb-2023  - V0.62 Fix PharosTargetProvider mysql loading issue
    3-Mar-2023  - V0.63 Fix typo and handle missing activityType in PharosTargetCofactorProvider()
   13-Mar-2023  - V0.64 Add CARDTargetAnnotationProvider (to replace CARDTargetFeatureProvider)
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
-  11-Apr-2023  - V0.67 Fix issue with lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
+  11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
+  27-Apr-2023  - V0.68 Update CARD treeNodeList building
```

### Comparing `rcsb.utils.targets-0.67/LICENSE` & `rcsb.utils.targets-0.68/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/PKG-INFO` & `rcsb.utils.targets-0.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.67
+Version: 0.68
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.67/README.md` & `rcsb.utils.targets-0.68/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 #  File:           CARDTargetOntologyProvider.py
 #  Date:           14-Mar-2023 dwp
 #
 #  Updates:
 #   11-Apr-2023 dwp  Fix issue with lineage tree building--handle cases with two parents at same depth;
 #                    Add treeNodeList building and exporting
+#   27-Apr-2023 dwp  Update tree node list generation
 ##
 """
 Accessors for CARD ontologies.
 
 """
 
 import datetime
@@ -151,38 +152,40 @@
         Args:
             parentChildTupleList (list): list of (parent, child) tuples (e.g., [('ARO:1000003', 'ARO:0000000'), ('ARO:1000003', 'ARO:0000001')])
             idNameMapD (dict): dictionary mapping of ARO IDs to their corresponding name
 
         Returns:
             dict: dictionary containing all children as keys and all possible parents as values
                   (including the child itself, but excluding the top-level parent 'ARO:1000001')
+            list: list of all nodes (as dicts) in the tree with their immediate parents only (for building tree in browser)
         """
         # create a dictionary to store the parents of each child
         childToParentD = {}
         for parent, child in parentChildTupleList:
-            if child not in childToParentD:
+            if child not in childToParentD and child != "ARO:1000001":
                 childToParentD[child] = []
-            childToParentD[child].append(parent)
+            if parent != "ARO:1000001":  # Exclude the top-level "ARO:1000001"
+                childToParentD[child].append(parent)
 
+        # depthD = self.__createDepthDict(parentChildTupleList)
         treeNodeL = self.__exportTreeNodeList(childToParentD, idNameMapD)
 
         # create a dictionary to store the ancestors of each child
         lineageD = {}
-        for child in childToParentD.keys():
+        for child in childToParentD:
             lineageD[child] = [{"id": child, "name": idNameMapD[child], "depth": 0}]  # Add the child to its own ancestry list
             stack = [child]
             depth = -1
             while stack:
                 node = stack.pop()
                 if node in childToParentD:
                     for parent in childToParentD[node]:
-                        if parent != "ARO:1000001":  # Exclude the top-level "ARO:1000001"
-                            if parent not in [d["id"] for d in lineageD[child]]:
-                                lineageD[child].append({"id": parent, "name": idNameMapD[parent], "depth": depth})
-                                stack.append(parent)
+                        if parent not in [d["id"] for d in lineageD[child]]:
+                            lineageD[child].append({"id": parent, "name": idNameMapD[parent], "depth": depth})
+                            stack.append(parent)
                     depthLevels = set(i["depth"] for i in lineageD[child])
                     depth = min(depthLevels) - 1
             numDepthLevels = len(set(i["depth"] for i in lineageD[child]))
             #
             # Flip the depth numbering so that oldest ancestor has depth=1 and youngest/most-specific child has depth=n
             nL = []
             for aD in lineageD[child]:
@@ -199,11 +202,53 @@
         {'id': 'ARO:1000003', 'name': 'antibiotic molecule'}
         {'id': 'ARO:0000041', 'name': 'bacitracin', 'parents': ['ARO:3000053', 'ARO:3000707']}
         {'id': 'ARO:0000039', 'name': 'spectinomycin', 'parents': ['ARO:0000016']}
         """
         #
         dL = []
         for child, parentL in childToParentD.items():
-            tD = {"id": child, "name": idNameMapD[child], "parents": parentL}
+            if parentL:
+                tD = {"id": child, "name": idNameMapD[child], "parents": parentL}
+            else:
+                tD = {"id": child, "name": idNameMapD[child]}
             dL.append(tD)
 
         return dL
+
+    # def __createDepthDict(self, parentChildTupleList):
+    #     # Create an adjacency list to represent the graph
+    #     graph = {}
+    #     for parent, child in parentChildTupleList:
+    #         if parent not in graph:
+    #             graph[parent] = set()
+    #         graph[parent].add(child)
+    #     #
+    #     # Initialize the depth dictionary and visited set
+    #     depthD = {}
+    #     visited = set()
+    #     #
+    #     # Define a helper function to traverse the graph
+    #     def traverse(node, depth, cycleNodes):
+    #         # If we have already visited this node, return
+    #         if node in visited:
+    #             return
+    #         #
+    #         # Add the node to the visited set
+    #         visited.add(node)
+    #         #
+    #         # Add the node to the depth dictionary
+    #         if node in depthD:
+    #             depthD[node].extend(cycleNodes + [depth])
+    #         else:
+    #             depthD[node] = cycleNodes + [depth]
+    #         #
+    #         # Traverse the children of the node
+    #         if node in graph:
+    #             for child in graph[node]:
+    #                 traverse(child, depth+1, cycleNodes)
+    #     #
+    #     # Traverse the graph from each node to handle cycles
+    #     for node in graph:
+    #         traverse(node, 0, [])
+    #     #
+    #     # Return the completed depth dictionary
+    #     return depthD
```

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.68/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.67
+Version: 0.68
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.68/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.67/setup.py` & `rcsb.utils.targets-0.68/setup.py`

 * *Files identical despite different names*

