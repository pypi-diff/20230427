# Comparing `tmp/mini_memgraph-0.1.0.tar.gz` & `tmp/mini_memgraph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_memgraph-0.1.0.tar", max compression
+gzip compressed data, was "mini_memgraph-0.1.1.tar", max compression
```

## Comparing `mini_memgraph-0.1.0.tar` & `mini_memgraph-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      295 2023-04-19 22:45:44.043599 mini_memgraph-0.1.0/README.md
--rw-r--r--   0        0        0       43 2023-04-19 22:06:02.794299 mini_memgraph-0.1.0/mini_memgraph/__init__.py
--rw-r--r--   0        0        0     2509 2023-04-19 22:55:12.409316 mini_memgraph-0.1.0/mini_memgraph/db.py
--rw-r--r--   0        0        0    13276 2023-04-19 22:55:12.416868 mini_memgraph-0.1.0/mini_memgraph/memgraph.py
--rw-r--r--   0        0        0      441 2023-04-19 22:06:02.800400 mini_memgraph-0.1.0/mini_memgraph/utility.py
--rw-r--r--   0        0        0      580 2023-04-19 22:44:35.601072 mini_memgraph-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 mini_memgraph-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      726 2023-04-21 19:26:38.882323 mini_memgraph-0.1.1/README.md
+-rw-r--r--   0        0        0       43 2023-04-19 22:06:02.794299 mini_memgraph-0.1.1/mini_memgraph/__init__.py
+-rw-r--r--   0        0        0     2509 2023-04-19 22:55:12.409316 mini_memgraph-0.1.1/mini_memgraph/db.py
+-rw-r--r--   0        0        0    13471 2023-04-21 22:25:00.110508 mini_memgraph-0.1.1/mini_memgraph/memgraph.py
+-rw-r--r--   0        0        0      441 2023-04-19 22:06:02.800400 mini_memgraph-0.1.1/mini_memgraph/utility.py
+-rw-r--r--   0        0        0      598 2023-04-27 20:31:41.101723 mini_memgraph-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 mini_memgraph-0.1.1/PKG-INFO
```

### Comparing `mini_memgraph-0.1.0/mini_memgraph/db.py` & `mini_memgraph-0.1.1/mini_memgraph/db.py`

 * *Files identical despite different names*

### Comparing `mini_memgraph-0.1.0/mini_memgraph/memgraph.py` & `mini_memgraph-0.1.1/mini_memgraph/memgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,16 +156,16 @@
     def write_edges(self, edge_list: List[Dict], source_label: str, edge_label: str, target_label: str,
                     source_id_label: str = 'id', target_id_label: str = 'id',
                     add_attributes: Union[List, Set, Tuple] = None,
                     chunk_size=100000,
                     custom_query=None,
                     on_duplicate_edges: str = 'update'):
 
-        if on_duplicate_edges not in ('update', 'increment'):
-            raise ValueError(f'on_duplicate_edges must be either "update" or "increment". {on_duplicate_edges=}')
+        if on_duplicate_edges not in ('update', 'increment', 'duplicate'):
+            raise ValueError(f'on_duplicate_edges must be either "update", "increment" or "duplicate". {on_duplicate_edges=}')
         if add_attributes is not None:
             attributes_statement = ", ".join([
                 f"r.{val} = row.{val}" for val in add_attributes
             ])
             update_create_set = f"ON CREATE SET {attributes_statement}"
             increment_create_set = f"ON CREATE SET {attributes_statement}, r.weight = 1"
             update_match_set = f"ON MATCH SET {attributes_statement}"
@@ -177,20 +177,24 @@
         on_duplicate_options = {
             'update': {
                 'create': update_create_set,
                 'match': update_match_set
             },
             'increment': {
                 'create': increment_create_set,
-                'match': 'ON MATCH SET r.weight = r.weight +1'}
+                'match': 'ON MATCH SET r.weight = r.weight +1'},
+            'duplicate':{
+                'create': update_create_set,
+                'match': ''
+            }
         }
 
         unwind_statement = "UNWIND $edge_list AS row"
         match_nodes = f"MATCH (s:{source_label} {{id:row.source}}), (t:{target_label} {{id:row.target}})"
-        merge_rel = f"MERGE (s)-[r:{edge_label}]->(t)"
+        merge_rel = f"{'CREATE' if on_duplicate_edges == 'duplicate' else 'MERGE'} (s)-[r:{edge_label}]->(t)"
         on_create = on_duplicate_options[on_duplicate_edges]['create']
         on_match = on_duplicate_options[on_duplicate_edges]['match']
 
         query = ' '.join([unwind_statement, match_nodes, merge_rel, on_create, on_match])
         for edge_chunk in chunks(edge_list, chunk_size):
             self.write(query, edge_list=edge_chunk)
```

### Comparing `mini_memgraph-0.1.0/pyproject.toml` & `mini_memgraph-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "mini-memgraph"
-version = "0.1.0"
+version = "0.1.1"
 description = "A basic wrapper to simplify interacting with a local Memgraph instance using Python."
 license = "MIT"
 authors = ["James Allen-Robertson <minyall@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Minyall/mini_memgraph"
 packages = [{include = "mini_memgraph"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Database"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pymgclient = "^1.3.1"
+pandas = "^2.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mini_memgraph-0.1.0/PKG-INFO` & `mini_memgraph-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 Metadata-Version: 2.1
 Name: mini-memgraph
-Version: 0.1.0
+Version: 0.1.1
 Summary: A basic wrapper to simplify interacting with a local Memgraph instance using Python.
 Home-page: https://github.com/Minyall/mini_memgraph
 License: MIT
 Author: James Allen-Robertson
 Author-email: minyall@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pymgclient (>=1.3.1,<2.0.0)
 Project-URL: Repository, https://github.com/Minyall/mini_memgraph
 Description-Content-Type: text/markdown
 
 # Mini-Memgraph
 A basic wrapper to simplify interacting with a local [Memgraph](https://memgraph.com/) instance using Python.
 
 Produced predominantly to serve as a common backend class for my other projects, but should be suitable for general use. Docstrings incoming and pull requests welcomed.
+
+## Installation
+Install from [PyPI](https://pypi.org/project/mini-memgraph/)
+
+`pip install mini-memgraph`
+
+## Disclaimer
+This software was produced as a backend interface for an unsecured locally hosted Memgraph database for data analysis 
+and research. I am not qualified to write secure code that would be suitable for a production environment. 
+Do not use this code for production. All code is utilised at user's own risk etc.
```

