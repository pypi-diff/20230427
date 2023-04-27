# Comparing `tmp/LineageTree-1.0.2.tar.gz` & `tmp/LineageTree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LineageTree-1.0.2.tar", last modified: Tue Jan 31 18:36:54 2023, max compression
+gzip compressed data, was "LineageTree-1.1.0.tar", last modified: Thu Apr 27 10:28:56 2023, max compression
```

## Comparing `LineageTree-1.0.2.tar` & `LineageTree-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 18:36:54.896783 LineageTree-1.0.2/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-08-16 08:53:03.000000 LineageTree-1.0.2/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)     2362 2023-01-31 18:36:54.896670 LineageTree-1.0.2/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1895 2022-08-16 08:53:03.000000 LineageTree-1.0.2/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      567 2023-01-31 18:36:43.000000 LineageTree-1.0.2/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)       38 2023-01-31 18:36:54.896815 LineageTree-1.0.2/setup.cfg
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1067 2023-01-31 18:36:43.000000 LineageTree-1.0.2/setup.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 18:36:54.894894 LineageTree-1.0.2/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 18:36:54.895612 LineageTree-1.0.2/src/LineageTree/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       59 2023-01-31 18:36:43.000000 LineageTree-1.0.2/src/LineageTree/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    74622 2023-01-31 17:57:57.000000 LineageTree-1.0.2/src/LineageTree/lineageTree.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 18:36:54.896428 LineageTree-1.0.2/src/LineageTree.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     2362 2023-01-31 18:36:54.000000 LineageTree-1.0.2/src/LineageTree.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      319 2023-01-31 18:36:54.000000 LineageTree-1.0.2/src/LineageTree.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-01-31 18:36:54.000000 LineageTree-1.0.2/src/LineageTree.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       50 2023-01-31 18:36:54.000000 LineageTree-1.0.2/src/LineageTree.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       12 2023-01-31 18:36:54.000000 LineageTree-1.0.2/src/LineageTree.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-01-31 18:36:54.896532 LineageTree-1.0.2/test/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      264 2023-01-31 17:57:50.000000 LineageTree-1.0.2/test/test_lineageTree.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.765994 LineageTree-1.1.0/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-08-16 08:53:03.000000 LineageTree-1.1.0/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     2362 2023-04-27 10:28:56.765842 LineageTree-1.1.0/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1895 2022-08-16 08:53:03.000000 LineageTree-1.1.0/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      567 2023-04-27 10:28:38.000000 LineageTree-1.1.0/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       38 2023-04-27 10:28:56.766036 LineageTree-1.1.0/setup.cfg
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1052 2023-04-27 10:28:38.000000 LineageTree-1.1.0/setup.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.762978 LineageTree-1.1.0/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.763749 LineageTree-1.1.0/src/LineageTree/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       59 2023-04-27 10:28:38.000000 LineageTree-1.1.0/src/LineageTree/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    75126 2023-04-27 10:26:30.000000 LineageTree-1.1.0/src/LineageTree/lineageTree.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.764379 LineageTree-1.1.0/src/LineageTree.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     2362 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      319 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       50 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       12 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.765570 LineageTree-1.1.0/test/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      264 2023-01-31 17:57:50.000000 LineageTree-1.1.0/test/test_lineageTree.py
```

### Comparing `LineageTree-1.0.2/LICENSE` & `LineageTree-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LineageTree-1.0.2/PKG-INFO` & `LineageTree-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LineageTree
-Version: 1.0.2
+Version: 1.1.0
 Summary: Lineage tree structure for TGMM algorithm
 Home-page: https://github.com/leoguignard/TGMMlibraries
 Author: Leo Guignard
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LineageTree-1.0.2/README.md` & `LineageTree-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `LineageTree-1.0.2/pyproject.toml` & `LineageTree-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 line-length = 79
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.bumpver]
-current_version = "1.0.2"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `LineageTree-1.0.2/setup.py` & `LineageTree-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="LineageTree",
-    version="1.0.2",
+    version="1.1.0",
     description="Lineage tree structure for TGMM algorithm",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/leoguignard/TGMMlibraries",
     author="Leo Guignard",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `LineageTree-1.0.2/src/LineageTree/lineageTree.py` & `LineageTree-1.1.0/src/LineageTree/lineageTree.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 from multiprocessing import Pool
 from scipy.spatial import Delaunay
 from itertools import combinations
 from numbers import Number
 import struct
 from scipy.spatial.distance import cdist
-
+import pickle as pkl
 
 class lineageTree(object):
     def get_next_id(self):
         """Computes the next authorized id.
 
         Returns:
             int: next authorized id
@@ -451,42 +451,34 @@
                             (factor * x1, factor * y1),
                             node_size(c),
                             fill=svgwrite.rgb(*(node_color(c))),
                         )
                     )
         dwg.save()
 
-    def to_treex(self):
+    def to_treex(self, sampling=1):
         """Convert the lineage tree into a treex file."""
         from treex.tree import Tree
 
-        # id_to_tree = {id: Tree() for id in self.nodes}
-
-        # for id_m, ids_d in self.successor.items():
-        #     for id_d in ids_d:
-        #         id_to_tree[id_m].add_subtree(id_to_tree[id_d])
-        # roots = [id_to_tree[id] for id in set(self.successor).difference(self.predecessor)]
-
-        roots = set(self.successor).difference(self.predecessor)
-        id_to_tree = {}
-        root_trees = []
-        for r in roots:
-            to_do = [r]
-            while 0 < len(to_do):
-                curr = to_do.pop()
-                cycle = self.get_cycle(curr)
-                lifetime = len(cycle)
-                cell = Tree()
-                cell.add_attribute_to_id("len", lifetime)
-                if cycle[0] in self.predecessor:
-                    id_to_tree[self.predecessor[cycle[0]][0]].add_subtree(cell)
-                else:
-                    root_trees.append(cell)
-                id_to_tree[cycle[-1]] = cell
-                to_do.extend(self.successor.get(cycle[-1], []))
+        id_to_tree = {id: Tree() for id in self.nodes}
+        times_to_consider = [t for t, n in self.time_nodes.items() if 0<len(n)]
+        times_to_consider = times_to_consider[::sampling]
+        for t in times_to_consider:
+            for id_mother in self.time_nodes[t]:
+                ids_daughters = self.successor.get(id_mother, [])
+                new_ids_daughters = ids_daughters.copy()
+                for _ in range(sampling-1):
+                    tmp = []
+                    for d in new_ids_daughters:
+                        tmp.extend(self.successor.get(d, [d]))
+                    new_ids_daughters = tmp
+                for daugther in new_ids_daughters: ## For each daughter in the list of daughters
+                    id_to_tree[id_mother].add_subtree(id_to_tree[daugther]) ## Add the Treex daughter as a subtree of the Treex mother   
+        
+        roots = [id_to_tree[id] for id in set(self.successor).difference(self.predecessor)] 
 
         return roots
 
     def to_tlp(
         self,
         fname,
         t_min=-1,
@@ -572,15 +564,15 @@
                     edges_to_use += [
                         e
                         for e in self.edges
                         if t_min < self.time[e[0]] < t_max
                     ]
                 if spatial:
                     edges_to_use += [
-                        (e, ei)
+                        e
                         for e in s_edges
                         if t_min < self.time[e[0]] < t_max
                     ]
             else:
                 nodes_to_use = list(self.nodes)
                 edges_to_use = []
                 if temporal:
@@ -959,19 +951,21 @@
                         * len(nodes),
                     )
                 )
             )
 
         unique_id = 0
         id_corres = {}
+        self.image_label = {}
         for n in nodes:
             if n in prob_cells:
                 self.prob_cells.add(unique_id)
             # if n in pos and n in names:
             t = n // 10**4
+            self.image_label[unique_id] = n % 10**4
             self.lT2pkl[unique_id] = n
             self.pkl2lT[n] = unique_id
             self.name[unique_id] = names.get(n, "")
             position = np.array(pos.get(n, [0, 0, 0]), dtype=float)
             self.time_nodes.setdefault(t, set()).add(unique_id)
             self.nodes.add(unique_id)
             self.pos[unique_id] = position
@@ -1043,16 +1037,15 @@
             for child in root:
                 value = _set_dictionary_value(child)
                 if value is not None:
                     dictionary[str(child.tag)] = value
         return dictionary
 
     def _read_from_ASTEC_pkl(self, file_path, eigen=False):
-        import pickle as pkl
-
+        
         with open(file_path, "rb") as f:
             tmp_data = pkl.load(f, encoding="latin1")
             f.close()
         new_ref = {}
         for k, v in self._astec_keydictionary.items():
             for key in v["input_keys"]:
                 new_ref[key] = v["output_key"]
@@ -1573,14 +1566,28 @@
         self.nodes = set(nodes)
         self.edges = set(edges)
         self.t_b = min(time_nodes.keys())
         self.t_e = max(time_nodes.keys())
         self.is_root = is_root
         self.max_id = max(self.nodes)
 
+    def write(self, fname):
+        if os.path.splitext(fname)[-1] != '.lT':
+            os.path.extsep.join(fname, 'lT')
+        with open(fname, 'bw') as f:
+            pkl.dump(self, f)
+            f.close()
+
+    @classmethod
+    def load(clf, fname):
+        with open(fname, 'br') as f:
+            lT = pkl.load(f)
+            f.close()
+        return lT
+
     def get_idx3d(self, t):
         """Get a 3d kdtree for the dataset at time *t* .
         The  kdtree is stored in *self.kdtrees[t]*
 
         Args:
             t (int): time
         Returns:
@@ -1932,9 +1939,11 @@
             self.read_from_txt_for_celegans_CAO(
                 file_format, reorder=reorder, shape=shape, raw_size=raw_size
             )
         elif file_type == "astec":
             self.read_from_ASTEC(file_format, eigen)
         elif file_type == "csv":
             self.read_from_csv(file_format, z_mult, link=1, delim=delim)
+        elif file_format is not None and '.lT' in file_format:
+            self.read(file_format)
         elif file_format is not None:
             self.read_from_binary(file_format)
```

### Comparing `LineageTree-1.0.2/src/LineageTree.egg-info/PKG-INFO` & `LineageTree-1.1.0/src/LineageTree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LineageTree
-Version: 1.0.2
+Version: 1.1.0
 Summary: Lineage tree structure for TGMM algorithm
 Home-page: https://github.com/leoguignard/TGMMlibraries
 Author: Leo Guignard
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

