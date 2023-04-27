# Comparing `tmp/NCBIQuery-1.3.tar.gz` & `tmp/NCBIQuery-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NCBIQuery-1.3.tar", last modified: Mon Mar 27 19:32:38 2023, max compression
+gzip compressed data, was "NCBIQuery-1.4.tar", last modified: Thu Apr 27 19:46:06 2023, max compression
```

## Comparing `NCBIQuery-1.3.tar` & `NCBIQuery-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 leosun    (1001) leosun    (1001)        0 2023-03-27 19:32:38.000000 NCBIQuery-1.3/
--rw-rw-r--   0 leosun    (1001) leosun    (1001)     1064 2023-03-27 18:38:27.000000 NCBIQuery-1.3/LICENSE.md
-drwxrwxr-x   0 leosun    (1001) leosun    (1001)        0 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery/
--rw-rw-r--   0 leosun    (1001) leosun    (1001)     2345 2023-03-21 13:48:18.000000 NCBIQuery-1.3/NCBIQuery/NCBIQuery.py
--rw-rw-r--   0 leosun    (1001) leosun    (1001)       94 2023-03-21 13:56:45.000000 NCBIQuery-1.3/NCBIQuery/__init__.py
--rw-rw-r--   0 leosun    (1001) leosun    (1001)       19 2023-03-27 19:32:37.000000 NCBIQuery-1.3/NCBIQuery/version.py
-drwxrwxr-x   0 leosun    (1001) leosun    (1001)        0 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery.egg-info/
--rw-rw-r--   0 leosun    (1001) leosun    (1001)      209 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery.egg-info/PKG-INFO
--rw-rw-r--   0 leosun    (1001) leosun    (1001)      269 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery.egg-info/SOURCES.txt
--rw-rw-r--   0 leosun    (1001) leosun    (1001)        1 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery.egg-info/dependency_links.txt
--rw-rw-r--   0 leosun    (1001) leosun    (1001)       20 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery.egg-info/requires.txt
--rw-rw-r--   0 leosun    (1001) leosun    (1001)       10 2023-03-27 19:32:38.000000 NCBIQuery-1.3/NCBIQuery.egg-info/top_level.txt
--rw-rw-r--   0 leosun    (1001) leosun    (1001)      209 2023-03-27 19:32:38.000000 NCBIQuery-1.3/PKG-INFO
--rw-rw-r--   0 leosun    (1001) leosun    (1001)     2275 2023-03-21 13:14:54.000000 NCBIQuery-1.3/README.md
--rw-rw-r--   0 leosun    (1001) leosun    (1001)       95 2023-03-27 19:32:38.000000 NCBIQuery-1.3/setup.cfg
--rw-rw-r--   0 leosun    (1001) leosun    (1001)      425 2023-03-27 19:31:18.000000 NCBIQuery-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:46:06.445273 NCBIQuery-1.4/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-18 18:58:13.000000 NCBIQuery-1.4/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:46:06.445273 NCBIQuery-1.4/NCBIQuery/
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-04-27 19:41:51.000000 NCBIQuery-1.4/NCBIQuery/NCBIQuery.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-18 18:58:13.000000 NCBIQuery-1.4/NCBIQuery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 19:43:19.000000 NCBIQuery-1.4/NCBIQuery/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:46:06.445273 NCBIQuery-1.4/NCBIQuery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-27 19:46:06.445273 NCBIQuery-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-04-27 19:42:06.000000 NCBIQuery-1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       95 2023-04-27 19:46:06.445273 NCBIQuery-1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-18 18:58:13.000000 NCBIQuery-1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `NCBIQuery-1.3/LICENSE.md` & `NCBIQuery-1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NCBIQuery-1.3/NCBIQuery/NCBIQuery.py` & `NCBIQuery-1.4/NCBIQuery/NCBIQuery.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import requests
 import xml.etree.ElementTree as ET
 from tokenizers import ByteLevelBPETokenizer
 
 
 base = 'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/'
 
-def query_id(db='pubmed', search_field_tags='tw', contents='', retmax=5000):
+def query_id(db='pubmed', search_field_tags='tw', contents='', retmax=10000):
     if not isinstance(search_field_tags, list):
         search_field_tags = [search_field_tags]
     if not isinstance(contents, list):
         contents = [contents]
     n = min(len(search_field_tags), len(contents))
     if n < 1:
         return []
     query_string = contents[0] + '[' + search_field_tags[0] + ']'
     for i in range(1, n):
         query_string += ' AND ' + contents[i] + '[' + search_field_tags[i] + ']'
     query_string = html.escape(query_string)
-    retmax = min(retmax, 5000) # Maximum number of results returning for a query is 5000
+    retmax = min(retmax, 10000) # Maximum number of results returning for a query is 10000
     search_url = base + 'esearch.fcgi?db=' + db + '&term=' + query_string + '&usehistory=y&retmax=' + str(retmax) + '&sort=relevance' # Records are sorted based on relevance to your search. For more information about PubMed’s relevance ranking, see the PubMed Help section on Computation of Weighted Relevance Order in PubMed.
     res = requests.get(search_url).content
     search_et = ET.fromstring(res)
     search_ids = []
     for child in search_et.iter('*'):
         if child.tag == 'Id':
             search_ids.append(child.text)
@@ -45,10 +45,10 @@
                 if child.text is not None:
                     article_abstracts.append(child.text)
                 else:
                     article_abstracts.append('')
                 break
     return article_abstracts
 
-def query_abstract(db='pubmed', search_field_tags='tw', contents='', retmax=5000):
+def query_abstract(db='pubmed', search_field_tags='tw', contents='', retmax=10000):
     search_ids = query_id(db, search_field_tags, contents, retmax)
     return id_abstract(search_ids, db)
```

### Comparing `NCBIQuery-1.3/README.md` & `NCBIQuery-1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 
 Arguments:
 | Parameter                 | Default       | Description   |   
 | :------------------------ |:-------------:| :-------------|
 | db           |    pubmed           |  The database which you search from |
 | search_field_tags          | tw           | A list of (or a single) search field tag(s) |
 | contents         |                    | A list of (or a single) search content(s) corresponding to each tag |
-| retmax           |        5000            | The maximum number of papers to return (cannot exceed 5000) |
+| retmax           |        10000            | The maximum number of papers to return (cannot exceed 10000) |
 
 Return: A list of paper ids.
 ### query_abstract()
 
 Get paper abstracts from search text.
 
 Arguments:
 | Parameter                 | Default       | Description   |   
 | :------------------------ |:-------------:| :-------------|
 | db           |    pubmed           |  The database which you search from |
 | search_field_tags          | tw           | A list of (or a single) search field tag(s) |
 | contents         |                    | A list of (or a single) search content(s) corresponding to each tag |
-| retmax           |        5000            | The maximum number of papers to return (cannot exceed 5000) |
+| retmax           |        10000            | The maximum number of papers to return (cannot exceed 10000) |
 
 Return: A list of paper abstracts.
 
 ### id_abstract()
 
 Get paper abstracts from id.
```

