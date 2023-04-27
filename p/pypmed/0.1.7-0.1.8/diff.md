# Comparing `tmp/pypmed-0.1.7.tar.gz` & `tmp/pypmed-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypmed-0.1.7.tar", max compression
+gzip compressed data, was "pypmed-0.1.8.tar", max compression
```

## Comparing `pypmed-0.1.7.tar` & `pypmed-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-04-27 01:50:04.026195 pypmed-0.1.7/LICENSE
--rw-r--r--   0        0        0     1016 2023-04-27 01:50:04.026195 pypmed-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-27 01:50:04.026195 pypmed-0.1.7/pypmed/__init__.py
--rw-r--r--   0        0        0     5661 2023-04-27 01:50:04.026195 pypmed-0.1.7/pypmed/apis.py
--rw-r--r--   0        0        0      946 2023-04-27 01:50:04.026195 pypmed-0.1.7/pypmed/checks.py
--rw-r--r--   0        0        0     1867 2023-04-27 01:50:04.026195 pypmed-0.1.7/pypmed/filters.py
--rw-r--r--   0        0        0     1296 2023-04-27 01:50:04.026195 pypmed-0.1.7/pypmed/parsers.py
--rw-r--r--   0        0        0      669 2023-04-27 01:50:04.030195 pypmed-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 pypmed-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-27 02:02:52.900935 pypmed-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1016 2023-04-27 02:02:52.900935 pypmed-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:02:52.900935 pypmed-0.1.8/pypmed/__init__.py
+-rw-r--r--   0        0        0     5661 2023-04-27 02:02:52.900935 pypmed-0.1.8/pypmed/apis.py
+-rw-r--r--   0        0        0      946 2023-04-27 02:02:52.900935 pypmed-0.1.8/pypmed/checks.py
+-rw-r--r--   0        0        0     1867 2023-04-27 02:02:52.900935 pypmed-0.1.8/pypmed/filters.py
+-rw-r--r--   0        0        0     1296 2023-04-27 02:02:52.900935 pypmed-0.1.8/pypmed/parsers.py
+-rw-r--r--   0        0        0      669 2023-04-27 02:02:52.904935 pypmed-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 pypmed-0.1.8/PKG-INFO
```

### Comparing `pypmed-0.1.7/LICENSE` & `pypmed-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.7/README.md` & `pypmed-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.7/pypmed/apis.py` & `pypmed-0.1.8/pypmed/apis.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.7/pypmed/checks.py` & `pypmed-0.1.8/pypmed/checks.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.7/pypmed/filters.py` & `pypmed-0.1.8/pypmed/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
         # check if score is better than previous best
         if score > best_score and score > 80:
             best_score = score
             best_match = item
 
     # check if best match for name is not None - if so article is confirmed for author
-    if best_match is not None:
+    if isinstance(best_match, dict):
         # add author info to article package
         article_dict['author_first_name'] = author_metadata['author_first_name']
         article_dict['author_last_name'] = author_metadata['author_last_name']
         # check affiliation if provided
         try:
-            if institution is not None and 'AffiliationInfo' in list(best_match.keys()):
+            if institution is not None and 'AffiliationInfo' in best_match.keys():
                 affiliation_info = best_match['AffiliationInfo']['Affiliation']
                 score = institution_check(institution, affiliation_info)
                 if score > 80:
                     # author and institution confirmed - add to return list
                     article_dict['institution'] = institution
         except Exception as e:
             print(e)
```

### Comparing `pypmed-0.1.7/pypmed/parsers.py` & `pypmed-0.1.8/pypmed/parsers.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.7/pyproject.toml` & `pypmed-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypmed"
-version = "0.1.7"
+version = "0.1.8"
 description = "python wrapper for pubmed apis --> https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi/"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pypmed"}]
 
 license = "MIT"
```

### Comparing `pypmed-0.1.7/PKG-INFO` & `pypmed-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypmed
-Version: 0.1.7
+Version: 0.1.8
 Summary: python wrapper for pubmed apis --> https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi/
 Home-page: https://github.com/jermwatt/pypmed
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

