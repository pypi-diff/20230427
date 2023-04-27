# Comparing `tmp/bw_graph_tools-0.1.0.tar.gz` & `tmp/bw_graph_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_graph_tools-0.1.0.tar", last modified: Tue Apr 25 19:10:28 2023, max compression
+gzip compressed data, was "bw_graph_tools-0.1.1.tar", last modified: Thu Apr 27 05:18:01 2023, max compression
```

## Comparing `bw_graph_tools-0.1.0.tar` & `bw_graph_tools-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 19:10:28.862015 bw_graph_tools-0.1.0/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     2941 2023-04-25 19:10:28.862115 bw_graph_tools-0.1.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1974 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 19:10:28.859324 bw_graph_tools-0.1.0/bw_graph_tools/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.0/bw_graph_tools/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      534 2023-04-23 08:47:29.000000 bw_graph_tools-0.1.0/bw_graph_tools/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      119 2023-04-13 06:07:17.000000 bw_graph_tools-0.1.0/bw_graph_tools/errors.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    25928 2023-04-23 19:13:20.000000 bw_graph_tools-0.1.0/bw_graph_tools/graph_traversal.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2092 2023-04-13 07:48:33.000000 bw_graph_tools-0.1.0/bw_graph_tools/graph_traversal_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7920 2023-04-25 18:58:58.000000 bw_graph_tools-0.1.0/bw_graph_tools/matrix_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.1.0/bw_graph_tools/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 19:10:28.860255 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2941 2023-04-25 19:10:28.000000 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      664 2023-04-25 19:10:28.000000 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-25 19:10:28.000000 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      124 2023-04-25 19:10:28.000000 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       29 2023-04-25 19:10:28.000000 bw_graph_tools-0.1.0/bw_graph_tools.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 19:10:28.859095 bw_graph_tools-0.1.0/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1154 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.0/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.0/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1607 2023-04-25 19:10:28.862632 bw_graph_tools-0.1.0/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 19:10:28.861714 bw_graph_tools-0.1.0/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.1.0/tests/test_get_path_from_matrix.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2683 2023-04-25 19:07:42.000000 bw_graph_tools-0.1.0/tests/test_matrix_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-04-13 07:48:29.000000 bw_graph_tools-0.1.0/tests/test_second_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-04-13 07:48:29.000000 bw_graph_tools-0.1.0/tests/test_third_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2057 2023-04-25 19:08:11.000000 bw_graph_tools-0.1.0/tests/test_traversal_basic.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.713289 bw_graph_tools-0.1.1/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.1/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.1/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3160 2023-04-27 05:18:01.713366 bw_graph_tools-0.1.1/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2192 2023-04-26 11:41:49.000000 bw_graph_tools-0.1.1/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.710960 bw_graph_tools-0.1.1/bw_graph_tools/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-27 05:17:33.000000 bw_graph_tools-0.1.1/bw_graph_tools/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      534 2023-04-23 08:47:29.000000 bw_graph_tools-0.1.1/bw_graph_tools/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      119 2023-04-13 06:07:17.000000 bw_graph_tools-0.1.1/bw_graph_tools/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    25928 2023-04-23 19:13:20.000000 bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2092 2023-04-13 07:48:33.000000 bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7702 2023-04-26 14:27:25.000000 bw_graph_tools-0.1.1/bw_graph_tools/matrix_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.1.1/bw_graph_tools/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.711786 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3160 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      664 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      124 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       29 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.710719 bw_graph_tools-0.1.1/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.1.1/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.1/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1607 2023-04-27 05:18:01.713747 bw_graph_tools-0.1.1/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.713092 bw_graph_tools-0.1.1/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.1.1/tests/test_get_path_from_matrix.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2683 2023-04-25 19:07:42.000000 bw_graph_tools-0.1.1/tests/test_matrix_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-04-13 07:48:29.000000 bw_graph_tools-0.1.1/tests/test_second_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-04-13 07:48:29.000000 bw_graph_tools-0.1.1/tests/test_third_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2057 2023-04-25 19:08:11.000000 bw_graph_tools-0.1.1/tests/test_traversal_basic.py
```

### Comparing `bw_graph_tools-0.1.0/LICENSE` & `bw_graph_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/PKG-INFO` & `bw_graph_tools-0.1.1/bw_graph_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bw_graph_tools
-Version: 0.1.0
+Name: bw-graph-tools
+Version: 0.1.1
 Summary: Graph traversal class and utilities
 Home-page: https://github.com/brightway-lca/bw_graph_tools
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -65,13 +65,21 @@
 _bw_graph_tools_ is free and open source software.
 
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
+## Documentation
+
+1. Install the `sphinx-furo` conda environment from the file `.docs/environment.yml`.
+2. Build the documentation locally by running
+
+```
+sphinx-autobuild docs _build/html -a -j auto --open-browser
+```
 
 <!-- github-only -->
 
 [command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
 [license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
 [contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
```

### Comparing `bw_graph_tools-0.1.0/README.md` & `bw_graph_tools-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,13 +38,21 @@
 _bw_graph_tools_ is free and open source software.
 
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
+## Documentation
+
+1. Install the `sphinx-furo` conda environment from the file `.docs/environment.yml`.
+2. Build the documentation locally by running
+
+```
+sphinx-autobuild docs _build/html -a -j auto --open-browser
+```
 
 <!-- github-only -->
 
 [command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
 [license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
-[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
+[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
```

### Comparing `bw_graph_tools-0.1.0/bw_graph_tools/__init__.py` & `bw_graph_tools-0.1.1/bw_graph_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/bw_graph_tools/graph_traversal.py` & `bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/bw_graph_tools/graph_traversal_utils.py` & `bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/bw_graph_tools/matrix_utils.py` & `bw_graph_tools-0.1.1/bw_graph_tools/matrix_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,28 +158,21 @@
     # Every column must have an activity with some reference product or the system
     # is not solvable. Therefore we can look across all columns. We will do
     # all the work in matrix indices.
     missing = np.setdiff1d(
         np.arange(mm.matrix.shape[0]), col_indices, assume_unique=True
     )
 
-    print("After first heuristic:")
-    print(row_indices, col_indices)
-
     # Short circuit other steps if possible; assumption is that this step will
     # be taken for most matrices
     if not missing.size:
         return (row_indices, col_indices)
 
     row_indices, col_indices = gpe_second_heuristic(mm, row_indices, col_indices)
-    print("After second heuristic:")
-    print(row_indices, col_indices)
     row_indices, col_indices = gpe_third_heuristic(mm, row_indices, col_indices)
-    print("After third heuristic:")
-    print(row_indices, col_indices)
 
     # No idea how this could happen, but better raise an error than pass bad data
     if row_indices.shape != col_indices.shape:
         raise ValueError("Guessed row indices do not match guessed column indices.")
 
     missing = np.setdiff1d(
         np.arange(mm.matrix.shape[0]), col_indices, assume_unique=True
```

### Comparing `bw_graph_tools-0.1.0/bw_graph_tools.egg-info/PKG-INFO` & `bw_graph_tools-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bw-graph-tools
-Version: 0.1.0
+Name: bw_graph_tools
+Version: 0.1.1
 Summary: Graph traversal class and utilities
 Home-page: https://github.com/brightway-lca/bw_graph_tools
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -65,13 +65,21 @@
 _bw_graph_tools_ is free and open source software.
 
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
+## Documentation
+
+1. Install the `sphinx-furo` conda environment from the file `.docs/environment.yml`.
+2. Build the documentation locally by running
+
+```
+sphinx-autobuild docs _build/html -a -j auto --open-browser
+```
 
 <!-- github-only -->
 
 [command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
 [license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
 [contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
```

### Comparing `bw_graph_tools-0.1.0/bw_graph_tools.egg-info/SOURCES.txt` & `bw_graph_tools-0.1.1/bw_graph_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/setup.cfg` & `bw_graph_tools-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/tests/test_get_path_from_matrix.py` & `bw_graph_tools-0.1.1/tests/test_get_path_from_matrix.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/tests/test_matrix_utils.py` & `bw_graph_tools-0.1.1/tests/test_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/tests/test_second_heuristic.py` & `bw_graph_tools-0.1.1/tests/test_second_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/tests/test_third_heuristic.py` & `bw_graph_tools-0.1.1/tests/test_third_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.0/tests/test_traversal_basic.py` & `bw_graph_tools-0.1.1/tests/test_traversal_basic.py`

 * *Files identical despite different names*

