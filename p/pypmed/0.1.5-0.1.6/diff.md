# Comparing `tmp/pypmed-0.1.5.tar.gz` & `tmp/pypmed-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypmed-0.1.5.tar", max compression
+gzip compressed data, was "pypmed-0.1.6.tar", max compression
```

## Comparing `pypmed-0.1.5.tar` & `pypmed-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-04-27 01:14:20.679096 pypmed-0.1.5/LICENSE
--rw-r--r--   0        0        0     1016 2023-04-27 01:14:20.679096 pypmed-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-27 01:14:20.679096 pypmed-0.1.5/pypmed/__init__.py
--rw-r--r--   0        0        0     5661 2023-04-27 01:14:20.679096 pypmed-0.1.5/pypmed/apis.py
--rw-r--r--   0        0        0      946 2023-04-27 01:14:20.679096 pypmed-0.1.5/pypmed/checks.py
--rw-r--r--   0        0        0     1733 2023-04-27 01:14:20.679096 pypmed-0.1.5/pypmed/filters.py
--rw-r--r--   0        0        0     1296 2023-04-27 01:14:20.679096 pypmed-0.1.5/pypmed/parsers.py
--rw-r--r--   0        0        0      669 2023-04-27 01:14:20.683096 pypmed-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 pypmed-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-27 01:28:50.616457 pypmed-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1016 2023-04-27 01:28:50.616457 pypmed-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 01:28:50.620457 pypmed-0.1.6/pypmed/__init__.py
+-rw-r--r--   0        0        0     5661 2023-04-27 01:28:50.620457 pypmed-0.1.6/pypmed/apis.py
+-rw-r--r--   0        0        0      946 2023-04-27 01:28:50.620457 pypmed-0.1.6/pypmed/checks.py
+-rw-r--r--   0        0        0     1846 2023-04-27 01:28:50.620457 pypmed-0.1.6/pypmed/filters.py
+-rw-r--r--   0        0        0     1296 2023-04-27 01:28:50.620457 pypmed-0.1.6/pypmed/parsers.py
+-rw-r--r--   0        0        0      669 2023-04-27 01:28:50.620457 pypmed-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 pypmed-0.1.6/PKG-INFO
```

### Comparing `pypmed-0.1.5/LICENSE` & `pypmed-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.5/README.md` & `pypmed-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.5/pypmed/apis.py` & `pypmed-0.1.6/pypmed/apis.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.5/pypmed/checks.py` & `pypmed-0.1.6/pypmed/checks.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.5/pypmed/filters.py` & `pypmed-0.1.6/pypmed/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     # check if best match for name is not None - if so article is confirmed for author
     if best_match is not None:
         # add author info to article package
         article_dict['author_first_name'] = author_metadata['author_first_name']
         article_dict['author_last_name'] = author_metadata['author_last_name']
         # check affiliation if provided
         if institution is not None and 'AffiliationInfo' in list(best_match.keys()):
-            affiliation_info = best_match['AffiliationInfo']['Affiliation']
-            score = institution_check(institution, affiliation_info)
-            if score > 80:
-                # author and institution confirmed - add to return list
-                article_dict['institution'] = institution
+            try:
+              affiliation_info = best_match['AffiliationInfo']['Affiliation']
+              score = institution_check(institution, affiliation_info)
+              if score > 80:
+                  # author and institution confirmed - add to return list
+                  article_dict['institution'] = institution
+            except Exception as e:
+                  article_dict['institution'] = ''
         return article_dict
     return None
```

### Comparing `pypmed-0.1.5/pypmed/parsers.py` & `pypmed-0.1.6/pypmed/parsers.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.5/pyproject.toml` & `pypmed-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypmed"
-version = "0.1.5"
+version = "0.1.6"
 description = "python wrapper for pubmed apis --> https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi/"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pypmed"}]
 
 license = "MIT"
```

### Comparing `pypmed-0.1.5/PKG-INFO` & `pypmed-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypmed
-Version: 0.1.5
+Version: 0.1.6
 Summary: python wrapper for pubmed apis --> https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi/
 Home-page: https://github.com/jermwatt/pypmed
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

