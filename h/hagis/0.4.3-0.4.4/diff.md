# Comparing `tmp/hagis-0.4.3.tar.gz` & `tmp/hagis-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.4.3.tar", last modified: Wed Apr 26 12:24:40 2023, max compression
+gzip compressed data, was "hagis-0.4.4.tar", last modified: Thu Apr 27 09:02:41 2023, max compression
```

## Comparing `hagis-0.4.3.tar` & `hagis-0.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 12:24:40.378947 hagis-0.4.3/
--rw-rw-rw-   0        0        0      923 2023-04-26 12:24:40.378947 hagis-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 12:24:40.338128 hagis-0.4.3/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.4.3/hagis/__init__.py
--rw-rw-rw-   0        0        0    14858 2023-04-26 12:20:31.000000 hagis-0.4.3/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:24:40.370697 hagis-0.4.3/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-26 12:23:53.000000 hagis-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 12:24:40.387134 hagis-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 09:02:41.489391 hagis-0.4.4/
+-rw-rw-rw-   0        0        0      923 2023-04-27 09:02:41.487918 hagis-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 09:02:41.449150 hagis-0.4.4/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.4.4/hagis/__init__.py
+-rw-rw-rw-   0        0        0    15258 2023-04-27 08:57:37.000000 hagis-0.4.4/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:02:41.481335 hagis-0.4.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-27 09:02:41.000000 hagis-0.4.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-27 09:02:41.000000 hagis-0.4.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 09:02:41.000000 hagis-0.4.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-27 09:02:41.000000 hagis-0.4.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-27 09:01:48.000000 hagis-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 09:02:41.489391 hagis-0.4.4/setup.cfg
```

### Comparing `hagis-0.4.3/PKG-INFO` & `hagis-0.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.3
+Version: 0.4.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.3/hagis/hagis.py` & `hagis-0.4.4/hagis/hagis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ A high availability GIS client. """
+from concurrent import futures
 from datetime import datetime
 from hashlib import md5
 from inspect import signature
 from itertools import chain, islice
 from json import dumps, loads
 from time import time
 from types import SimpleNamespace
@@ -113,24 +114,25 @@
         """ Sets the static token.
 
         Args:
             token (str): Token.
         """
         self._generate_token = lambda: token
 
-    def query(self, where_clause: Optional[str] = None, record_count: Optional[int] = None, wkid: Optional[int] = None,
-              **kwargs: Any) -> Iterator[T]:
+    def query(self, where_clause: Optional[str] = None, record_count: Optional[int] = None,
+              wkid: Optional[int] = None, max_worker: Optional[int] = None, **kwargs: Any) -> Iterator[T]:
         """ Executes a query.
 
         Args:
             where_clause (str, optional): Where clause.  Defaults to None.
             record_count (Optional[int], optional): Maximum record count.  Defaults to None.
             wkid (Optional[int], optional): Spatial reference.  Defaults to None.
+            max_worker (Optional[int], optional): Max worker count (degree of parallelism). Defaults to None.
 
-        Returns:
+        Yields:
             Iterator[T]: Items.
         """
         if not where_clause:
             where_clause = "1=1"
 
         if record_count == 0:
             return
@@ -141,23 +143,20 @@
         else:
             # Otherwise, request only what is used by the model.
             fields = ",".join([f for (_, f) in self._fields.items() if f != self._shape_property_name.lower()])
             if not self._shape_property_name:
                 kwargs["returnGeometry"] = False
 
         if record_count:
-            keep_querying = True
             kwargs["resultRecordCount"] = record_count
-        else:
-            keep_querying = False
 
         if wkid:
             kwargs["outSR"] = wkid
 
-        for row in islice(self._query(where_clause, fields, keep_querying, **kwargs), record_count):
+        for row in islice(self._query(where_clause, fields, record_count, max_worker, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 dictionary = {property: getattr(row, field) for (property, field) in self._fields.items()}
                 if self._has_parameterless_constructor:
                     item = self._model()
                     for property_name, property_value in dictionary.items():
@@ -328,31 +327,37 @@
                 shape = self._shape_property_type(row.geometry.__dict__)
             else:
                 shape = self._shape_property_type()
                 shape.__dict__ = row.geometry.__dict__
 
         return SimpleNamespace(**row.attributes.__dict__, **{self._shape_property_name: shape})
 
-    def _query(self, where_clause: str, fields: str, keep_querying: bool, **kwargs: Any) -> Iterator[SimpleNamespace]:
+    def _query(self, where_clause: str, fields: str, record_count: Optional[int], max_worker: Optional[int],
+               **kwargs: Any) -> Iterator[SimpleNamespace]:
         def get_rows(where_clause: str):
             return self._get_rows(where_clause, fields, **kwargs)
 
         rows, exceeded_transfer_limit = get_rows(where_clause)
 
         for row in rows:
             yield self._map(row)
 
-        if exceeded_transfer_limit and keep_querying:
+        if exceeded_transfer_limit and record_count:
+            def get_more_rows(batch: List[int]):
+                more_rows, _ = get_rows(self.generate_where_clause(*batch))
+                return more_rows
+
             size = len(rows)
-            oids = self._get_oids(where_clause)
-            for number in range(size, len(oids), size):
-                more_where_clause = f"{self._oid_field} IN ({','.join(map(str, oids[number:number+size]))})"
-                more_rows, _ = get_rows(more_where_clause)
-                for row in more_rows:
-                    yield self._map(row)
+            remaining_oids = list(islice(self._get_oids(where_clause)[size:], record_count - size))
+            remaining_batches = [remaining_oids[i: i + size] for i in range(len(remaining_oids))[::size]]
+
+            with futures.ThreadPoolExecutor(max_worker) as executor:
+                for rows in executor.map(get_more_rows, remaining_batches):
+                    for row in rows:
+                        yield self._map(row)
 
 
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
     """
     x: float
     y: float
```

### Comparing `hagis-0.4.3/hagis.egg-info/PKG-INFO` & `hagis-0.4.4/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.3
+Version: 0.4.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.3/pyproject.toml` & `hagis-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

