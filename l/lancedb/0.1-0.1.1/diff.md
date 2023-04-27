# Comparing `tmp/lancedb-0.1.tar.gz` & `tmp/lancedb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.tar", last modified: Thu Apr 20 06:34:05 2023, max compression
+gzip compressed data, was "lancedb-0.1.1.tar", last modified: Thu Apr 27 00:01:10 2023, max compression
```

## Comparing `lancedb-0.1.tar` & `lancedb-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.567274 lancedb-0.1/
--rw-r--r--   0 changshe   (501) staff       (20)      994 2023-04-20 06:34:05.567124 lancedb-0.1/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.565726 lancedb-0.1/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.1/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.1/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.1/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     3058 2023-04-20 04:26:50.000000 lancedb-0.1/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3644 2023-04-20 04:26:39.000000 lancedb-0.1/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3336 2023-03-24 06:56:52.000000 lancedb-0.1/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     7486 2023-04-20 04:26:50.000000 lancedb-0.1/lancedb/table.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.566264 lancedb-0.1/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)      994 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      386 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      150 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-04-20 06:34:05.000000 lancedb-0.1/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1323 2023-04-20 06:25:59.000000 lancedb-0.1/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-04-20 06:34:05.567312 lancedb-0.1/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.1/setup.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-20 06:34:05.566925 lancedb-0.1/tests/
--rw-r--r--   0 changshe   (501) staff       (20)     2796 2023-04-20 04:26:50.000000 lancedb-0.1/tests/test_db.py
--rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.1/tests/test_embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     1814 2023-03-23 01:47:48.000000 lancedb-0.1/tests/test_query.py
--rw-r--r--   0 changshe   (501) staff       (20)     3763 2023-04-20 04:26:50.000000 lancedb-0.1/tests/test_table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.529805 lancedb-0.1.1/
+-rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-27 00:01:10.529662 lancedb-0.1.1/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.528124 lancedb-0.1.1/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.1.1/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.1.1/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.1.1/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3058 2023-04-20 04:26:50.000000 lancedb-0.1.1/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3721 2023-04-25 01:36:57.000000 lancedb-0.1.1/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3970 2023-04-26 23:53:57.000000 lancedb-0.1.1/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     7884 2023-04-26 23:53:57.000000 lancedb-0.1.1/lancedb/table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.528675 lancedb-0.1.1/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      386 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      150 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-04-27 00:01:10.000000 lancedb-0.1.1/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1325 2023-04-26 23:55:01.000000 lancedb-0.1.1/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-04-27 00:01:10.529843 lancedb-0.1.1/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.1.1/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-27 00:01:10.529463 lancedb-0.1.1/tests/
+-rw-r--r--   0 changshe   (501) staff       (20)     2796 2023-04-20 04:26:50.000000 lancedb-0.1.1/tests/test_db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.1.1/tests/test_embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2457 2023-04-26 23:53:57.000000 lancedb-0.1.1/tests/test_query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3763 2023-04-20 04:26:50.000000 lancedb-0.1.1/tests/test_table.py
```

### Comparing `lancedb-0.1/PKG-INFO` & `lancedb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1
+Version: 0.1.1
 Summary: lancedb
 Author-email: Lance Devs <dev@eto.ai>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1/lancedb/__init__.py` & `lancedb-0.1.1/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/lancedb/common.py` & `lancedb-0.1.1/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/lancedb/context.py` & `lancedb-0.1.1/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/lancedb/db.py` & `lancedb-0.1.1/lancedb/db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/lancedb/embeddings.py` & `lancedb-0.1.1/lancedb/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import math
+import sys
+
 from retry import retry
 from typing import Callable, Union
 
 from lance.vector import vec_to_table
 import numpy as np
 import pandas as pd
 import pyarrow as pa
@@ -60,34 +62,33 @@
 
         else:
 
             def embed_func(c):
                 return self.func(c.tolist())
 
         if len(self.rate_limiter_kwargs) > 0:
-            import ratelimiter
-
-            max_calls = self.rate_limiter_kwargs["max_calls"]
-            limiter = ratelimiter.RateLimiter(
-                max_calls, period=self.rate_limiter_kwargs["period"]
-            )
-            embed_func = limiter(embed_func)
+            v = int(sys.version_info.minor)
+            if v >= 11:
+                print("WARNING: rate limit only support up to 3.10, proceeding without rate limiter")
+            else:
+                import ratelimiter
+
+                max_calls = self.rate_limiter_kwargs["max_calls"]
+                limiter = ratelimiter.RateLimiter(
+                    max_calls, period=self.rate_limiter_kwargs["period"]
+                )
+                embed_func = limiter(embed_func)
         batches = self.to_batches(text)
         embeds = [emb for c in batches for emb in embed_func(c)]
         return embeds
 
     def __repr__(self):
         return f"EmbeddingFunction(func={self.func})"
 
     def rate_limit(self, max_calls=0.9, period=1.0):
-        import sys
-
-        v = int(sys.version_info.minor)
-        if v >= 11:
-            raise ValueError("rate limit only support up to 3.10")
         self.rate_limiter_kwargs = dict(max_calls=max_calls, period=period)
         return self
 
     def retry(self, tries=10, delay=1, max_delay=30, backoff=3, jitter=1):
         self.retry_kwargs = dict(
             tries=tries,
             delay=delay,
```

### Comparing `lancedb-0.1/lancedb/query.py` & `lancedb-0.1.1/lancedb/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class LanceQueryBuilder:
     """
     A builder for nearest neighbor queries for LanceDB.
     """
 
     def __init__(self, table: "lancedb.table.LanceTable", query: np.ndarray):
+        self._metric = "L2"
         self._nprobes = 20
         self._refine_factor = None
         self._table = table
         self._query = query
         self._limit = 10
         self._columns = None
         self._where = None
@@ -73,14 +74,29 @@
         Returns
         -------
         The LanceQueryBuilder object.
         """
         self._where = where
         return self
 
+    def metric(self, metric: str) -> LanceQueryBuilder:
+        """Set the distance metric to use.
+
+        Parameters
+        ----------
+        metric: str
+            The distance metric to use. By default "l2" is used.
+
+        Returns
+        -------
+        The LanceQueryBuilder object.
+        """
+        self._metric = metric
+        return self
+
     def nprobes(self, nprobes: int) -> LanceQueryBuilder:
         """Set the number of probes to use.
 
         Parameters
         ----------
         nprobes: int
             The number of probes to use.
@@ -104,22 +120,28 @@
         -------
         The LanceQueryBuilder object.
         """
         self._refine_factor = refine_factor
         return self
 
     def to_df(self) -> pd.DataFrame:
-        """Execute the query and return the results as a pandas DataFrame."""
+        """
+        Execute the query and return the results as a pandas DataFrame.
+        In addition to the selected columns, LanceDB also returns a vector
+        and also the "score" column which is the distance between the query
+        vector and the returned vector.
+        """
         ds = self._table.to_lance()
         # TODO indexed search
         tbl = ds.to_table(
             columns=self._columns,
             filter=self._where,
             nearest={
                 "column": VECTOR_COLUMN_NAME,
                 "q": self._query,
                 "k": self._limit,
+                "metric": self._metric,
                 "nprobes": self._nprobes,
                 "refine_factor": self._refine_factor,
             },
         )
         return tbl.to_pandas()
```

### Comparing `lancedb-0.1/lancedb/table.py` & `lancedb-0.1.1/lancedb/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,29 +102,33 @@
         """Return the table as a pyarrow Table."""
         return self._dataset.to_table()
 
     @property
     def _dataset_uri(self) -> str:
         return os.path.join(self._conn.uri, f"{self.name}.lance")
 
-    def create_index(self, num_partitions=256, num_sub_vectors=96):
+    def create_index(self, metric="L2", num_partitions=256, num_sub_vectors=96):
         """Create an index on the table.
 
         Parameters
         ----------
+        metric: str, default "L2"
+            The distance metric to use when creating the index. Valid values are "L2" or "cosine".
+            L2 is euclidean distance.
         num_partitions: int
             The number of IVF partitions to use when creating the index.
             Default is 256.
         num_sub_vectors: int
             The number of PQ sub-vectors to use when creating the index.
             Default is 96.
         """
         self._dataset.create_index(
             column=VECTOR_COLUMN_NAME,
             index_type="IVF_PQ",
+            metric=metric,
             num_partitions=num_partitions,
             num_sub_vectors=num_sub_vectors,
         )
         self._reset_dataset()
 
     @cached_property
     def _dataset(self) -> LanceDataset:
@@ -162,14 +166,17 @@
         ----------
         query: list, np.ndarray
             The query vector.
 
         Returns
         -------
         A LanceQueryBuilder object representing the query.
+        Once executed, the query returns selected columns, the vector,
+        and also the "score" column which is the distance between the query
+        vector and the returned vector.
         """
         if isinstance(query, list):
             query = np.array(query)
         if isinstance(query, np.ndarray):
             query = query.astype(np.float32)
         else:
             raise TypeError(f"Unsupported query type: {type(query)}")
```

### Comparing `lancedb-0.1/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.1/lancedb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1
+Version: 0.1.1
 Summary: lancedb
 Author-email: Lance Devs <dev@eto.ai>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1/pyproject.toml` & `lancedb-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lancedb"
-version = "0.1"
-dependencies = ["pylance>=0.4.3", "ratelimiter", "retry", "tqdm"]
+version = "0.1.1"
+dependencies = ["pylance>=0.4.4", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "Lance Devs", email = "dev@eto.ai" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `lancedb-0.1/setup.py` & `lancedb-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/tests/test_db.py` & `lancedb-0.1.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/tests/test_embeddings.py` & `lancedb-0.1.1/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1/tests/test_query.py` & `lancedb-0.1.1/tests/test_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import lance
 from lancedb.query import LanceQueryBuilder
 
+import numpy as np
 import pandas as pd
+import pandas.testing as tm
 import pyarrow as pa
 
 import pytest
 
 
 class MockTable:
     def __init__(self, tmp_path):
@@ -56,7 +58,25 @@
     assert all(df["vector"].values[0] == [1, 2])
 
 
 def test_query_builder_with_filter(table):
     df = LanceQueryBuilder(table, [0, 0]).where("id = 2").to_df()
     assert df["id"].values[0] == 2
     assert all(df["vector"].values[0] == [3, 4])
+
+
+def test_query_builder_with_metric(table):
+    query = [4, 8]
+    df_default = LanceQueryBuilder(table, query).to_df()
+    df_l2 = LanceQueryBuilder(table, query).metric("l2").to_df()
+    tm.assert_frame_equal(df_default, df_l2)
+
+    df_cosine = LanceQueryBuilder(table, query).metric("cosine").limit(1).to_df()
+    assert df_cosine.score[0] == pytest.approx(
+        cosine_distance(query, df_cosine.vector[0]),
+        abs=1e-6,
+    )
+    assert 0 <= df_cosine.score[0] <= 1
+
+
+def cosine_distance(vec1, vec2):
+    return 1 - np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2))
```

### Comparing `lancedb-0.1/tests/test_table.py` & `lancedb-0.1.1/tests/test_table.py`

 * *Files identical despite different names*

