# Comparing `tmp/bibx-0.0.1a1.tar.gz` & `tmp/bibx-0.0.1a2.tar.gz`

## Comparing `bibx-0.0.1a1.tar` & `bibx-0.0.1a2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a1/Makefile
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a1/.github/workflows/cd.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a1/.github/workflows/ci.yml
--rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a1/docs/examples/bit-pattern-savedrecs.txt
--rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a1/docs/examples/scopus.bib
--rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a1/docs/examples/scopus.ris
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a1/docs/examples/single-article.txt
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/__main__.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/article.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/base.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/cross_ref.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/generic.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/isi.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/scopus.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/_entities/collection_builders/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/algorithms/__init__.py
--rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 bibx-0.0.1a1/src/bibx/algorithms/sap.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a1/tests/test_works.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a1/tests/algorithms/test_sap.py
--rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 bibx-0.0.1a1/tests/entities/collection_builders/test_scopus.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 bibx-0.0.1a1/README.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bibx-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 bibx-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a2/Makefile
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/bit-pattern-savedrecs.txt
+-rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/scopus.bib
+-rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/scopus.ris
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/single-article.txt
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/__main__.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/article.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/base.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/cross_ref.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/generic.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/isi.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/scopus.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/algorithms/__init__.py
+-rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/algorithms/sap.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a2/tests/test_works.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a2/tests/algorithms/test_sap.py
+-rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 bibx-0.0.1a2/tests/entities/collection_builders/test_scopus.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 bibx-0.0.1a2/README.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bibx-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 bibx-0.0.1a2/PKG-INFO
```

### Comparing `bibx-0.0.1a1/.pre-commit-config.yaml` & `bibx-0.0.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/.github/workflows/cd.yml` & `bibx-0.0.1a2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/.github/workflows/ci.yml` & `bibx-0.0.1a2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/docs/examples/bit-pattern-savedrecs.txt` & `bibx-0.0.1a2/docs/examples/bit-pattern-savedrecs.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/docs/examples/scopus.bib` & `bibx-0.0.1a2/docs/examples/scopus.bib`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/docs/examples/scopus.ris` & `bibx-0.0.1a2/docs/examples/scopus.ris`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/docs/examples/single-article.txt` & `bibx-0.0.1a2/docs/examples/single-article.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/__init__.py` & `bibx-0.0.1a2/src/bibx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bibx._entities.article import Article
 from bibx._entities.collection import Collection
 from bibx._entities.collection_builders.isi import IsiCollectionBuilder
 from bibx._entities.collection_builders.scopus import ScopusCollectionBuilder
 
 __all__ = ["Article", "Collection", "read_scopus", "read_wos"]
 
-__version__ = "0.0.1a1"
+__version__ = "0.0.1a2"
 
 
 def read_scopus(*files: TextIO) -> Collection:
     """
     Takes any number of bibtex files from scopus and generates a collection.
 
     :param files: Scopus bib files open.
```

### Comparing `bibx-0.0.1a1/src/bibx/__main__.py` & `bibx-0.0.1a2/src/bibx/__main__.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/exceptions.py` & `bibx-0.0.1a2/src/bibx/exceptions.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/_entities/article.py` & `bibx-0.0.1a2/src/bibx/_entities/article.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/_entities/collection.py` & `bibx-0.0.1a2/src/bibx/_entities/collection.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/_entities/collection_builders/isi.py` & `bibx-0.0.1a2/src/bibx/_entities/collection_builders/isi.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/_entities/collection_builders/scopus.py` & `bibx-0.0.1a2/src/bibx/_entities/collection_builders/scopus.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/src/bibx/algorithms/sap.py` & `bibx-0.0.1a2/src/bibx/algorithms/sap.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         """
         g = graph.copy()
         valid_roots = [
             (n, g.in_degree(n)) for n in g.nodes if g.out_degree(n) == 0  # noqa
         ]
         sorted_roots = _limit(valid_roots, self.max_roots)
         nx.set_node_attributes(g, 0, ROOT)
-        for (node, degree) in sorted_roots:
+        for node, degree in sorted_roots:
             g.nodes[node][ROOT] = degree
         return g
 
     def _compute_leaves(self, graph: nx.DiGraph) -> nx.DiGraph:
         """
         Takes in a connected graph and returns it labeled with a `leaf` property.
         :param graph: Connected and filtered graph to work with.
@@ -201,23 +201,27 @@
         nx.set_node_attributes(g, 0, TRUNK)
         for node, sap in potential_trunk:
             g.nodes[node][TRUNK] = sap
         return g
 
     def _compute_branches(self, graph: nx.DiGraph) -> nx.DiGraph:
         """
-        Tags leaves.
+        Tags branches.
         """
         g = graph.copy()
         undirected = g.to_undirected()
         communities: List[Set] = louvain_communities(undirected)
         branches = list(sorted(communities, key=len))[:3]
         nx.set_node_attributes(g, 0, BRANCH)
         for i, branch in enumerate(branches, start=1):
-            potential_branch = [(n, g.nodes[n][YEAR]) for n in branch]
+            potential_branch = [
+                (n, g.nodes[n][YEAR])
+                for n in branch
+                if g.nodes[n][ROOT] == 0 and g.nodes[n][TRUNK] == 0
+            ]
             potential_branch = _limit(potential_branch, self.max_branch_size)
             for node, _ in potential_branch:
                 g.nodes[node][BRANCH] = i
         return g
 
     @staticmethod
     def _clear(graph: nx.DiGraph) -> nx.DiGraph:
```

### Comparing `bibx-0.0.1a1/tests/algorithms/test_sap.py` & `bibx-0.0.1a2/tests/algorithms/test_sap.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/tests/entities/collection_builders/test_scopus.py` & `bibx-0.0.1a2/tests/entities/collection_builders/test_scopus.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/.gitignore` & `bibx-0.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/LICENSE` & `bibx-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/README.md` & `bibx-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/pyproject.toml` & `bibx-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a1/PKG-INFO` & `bibx-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibx
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Python bibliometric tools.
 Author-email: Core of Science Team <technology@coreofscience.org>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bibliometrics,science,text mining
 Requires-Dist: bibtexparser~=1.4.0
 Requires-Dist: networkx~=3.0
```

