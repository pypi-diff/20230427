# Comparing `tmp/inverted_index_search-1.3.3.tar.gz` & `tmp/inverted_index_search-1.3.4.tar.gz`

## Comparing `inverted_index_search-1.3.3.tar` & `inverted_index_search-1.3.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 inverted_index_search-1.3.3/src/inverted_index_search/__init__.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 inverted_index_search-1.3.3/src/inverted_index_search/keyword_search.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 inverted_index_search-1.3.3/LICENSE
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 inverted_index_search-1.3.3/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 inverted_index_search-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 inverted_index_search-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/.DS_Store
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/src/inverted_index_search/__init__.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/src/inverted_index_search/keyword_search.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 inverted_index_search-1.3.4/PKG-INFO
```

### Comparing `inverted_index_search-1.3.3/LICENSE` & `inverted_index_search-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inverted_index_search-1.3.3/pyproject.toml` & `inverted_index_search-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "inverted_index_search"
-version = "1.3.3"
+version = "1.3.4"
 authors = [{ name="Affan Mir", email="affanmir95@gmail.com" }]
 description = "A module for creating ngrams and searching multiple phrases using inverted index searching in a document"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
         "nltk",
     ]
```

