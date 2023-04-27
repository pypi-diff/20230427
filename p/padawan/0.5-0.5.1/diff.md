# Comparing `tmp/padawan-0.5.tar.gz` & `tmp/padawan-0.5.1.tar.gz`

## Comparing `padawan-0.5.tar` & `padawan-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.5/.readthedocs.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.5/.pytest_cache/README.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 padawan-0.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.5/docs/Makefile
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 padawan-0.5/docs/api.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.5/docs/conf.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.5/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.5/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.5/docs/requirements.txt
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/__init__.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/collated_dataset.py
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/dataset.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/joined_dataset.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/json_io.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/mapped_dataset.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/metadata.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/ordering.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/parallelize.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/persisted_dataset.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/reindexed_dataset.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/renamed_dataset.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/repartitioned_dataset.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.5/src/padawan/sliced_dataset.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 padawan-0.5/tests/fixtures.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_collate.py
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_io.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_join.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_map.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_rename.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_repartition.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.5/tests/test_slice.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.5/tests/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.5/.gitignore
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.5/LICENSE
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.5/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 padawan-0.5/pyproject.toml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 padawan-0.5/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/api.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/__init__.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/collated_dataset.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/dataset.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/joined_dataset.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/json_io.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/mapped_dataset.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/metadata.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/ordering.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/parallelize.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/persisted_dataset.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/reindexed_dataset.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/renamed_dataset.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/repartitioned_dataset.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/sliced_dataset.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/fixtures.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_collate.py
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_io.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_join.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_map.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_rename.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_repartition.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_slice.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.5.1/.gitignore
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.5.1/LICENSE
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.5.1/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 padawan-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 padawan-0.5.1/PKG-INFO
```

### Comparing `padawan-0.5/.pytest_cache/v/cache/nodeids` & `padawan-0.5.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `padawan-0.5/docs/Makefile` & `padawan-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `padawan-0.5/docs/conf.py` & `padawan-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/docs/index.rst` & `padawan-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `padawan-0.5/docs/make.bat` & `padawan-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/collated_dataset.py` & `padawan-0.5.1/src/padawan/collated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/dataset.py` & `padawan-0.5.1/src/padawan/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,18 +471,14 @@
           polars.DataFrame: A single dataframe with all partitions
             concatenated.
         """
         if self._npartitions == 0:
             return dataframe_from_schema(self._schema)
 
         partition_indices = list(range(self._npartitions))
-        if is_parallel_config(parallel):
-            parts = parallel_map(
-                self._get_greedy,
-                partition_indices,
-                workers=parallel,
-                progress=progress,
-            )
-            return pl.concat(parts)
-        else:
-            parts = [self[i] for i in partition_indices]
-            return pl.concat(parts).collect()
+        parts = parallel_map(
+            self._get_greedy,
+            partition_indices,
+            workers=parallel,
+            progress=progress,
+        )
+        return pl.concat(parts)
```

### Comparing `padawan-0.5/src/padawan/joined_dataset.py` & `padawan-0.5.1/src/padawan/joined_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/json_io.py` & `padawan-0.5.1/src/padawan/json_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/mapped_dataset.py` & `padawan-0.5.1/src/padawan/mapped_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/metadata.py` & `padawan-0.5.1/src/padawan/metadata.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/ordering.py` & `padawan-0.5.1/src/padawan/ordering.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/parallelize.py` & `padawan-0.5.1/src/padawan/parallelize.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/persisted_dataset.py` & `padawan-0.5.1/src/padawan/persisted_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/reindexed_dataset.py` & `padawan-0.5.1/src/padawan/reindexed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/renamed_dataset.py` & `padawan-0.5.1/src/padawan/renamed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/repartitioned_dataset.py` & `padawan-0.5.1/src/padawan/repartitioned_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/src/padawan/sliced_dataset.py` & `padawan-0.5.1/src/padawan/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/fixtures.py` & `padawan-0.5.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_collate.py` & `padawan-0.5.1/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_io.py` & `padawan-0.5.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_join.py` & `padawan-0.5.1/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_map.py` & `padawan-0.5.1/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_rename.py` & `padawan-0.5.1/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_repartition.py` & `padawan-0.5.1/tests/test_repartition.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/tests/test_slice.py` & `padawan-0.5.1/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5/LICENSE` & `padawan-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `padawan-0.5/README.md` & `padawan-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `padawan-0.5/pyproject.toml` & `padawan-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "padawan"
-version = "0.5"
+version = "0.5.1"
 authors = [
   { name="Martin Wiebusch" },
 ]
 description = "Wrangle partitioned data with polars."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `padawan-0.5/PKG-INFO` & `padawan-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: padawan
-Version: 0.5
+Version: 0.5.1
 Summary: Wrangle partitioned data with polars.
 Project-URL: Homepage, https://github.com/mwiebusch78/padawan
 Project-URL: Bug Tracker, https://github.com/mwiebusch78/padawan/issues
 Project-URL: Documentation, https://padawan.readthedocs.io/en/latest/
 Author: Martin Wiebusch
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

