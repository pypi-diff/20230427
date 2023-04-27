# Comparing `tmp/criterion-site-parser-1.6.tar.gz` & `tmp/criterion-site-parser-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criterion-site-parser-1.6.tar", last modified: Mon Mar 27 19:00:14 2023, max compression
+gzip compressed data, was "criterion-site-parser-1.7.tar", last modified: Thu Apr 27 18:31:12 2023, max compression
```

## Comparing `criterion-site-parser-1.6.tar` & `criterion-site-parser-1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:00:14.543688 criterion-site-parser-1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-27 19:00:14.539688 criterion-site-parser-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/license
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:00:14.543688 criterion-site-parser-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:00:14.539688 criterion-site-parser-1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:00:14.539688 criterion-site-parser-1.6/src/criterion_site_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-27 19:00:14.000000 criterion-site-parser-1.6/src/criterion_site_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 19:00:14.000000 criterion-site-parser-1.6/src/criterion_site_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:00:14.000000 criterion-site-parser-1.6/src/criterion_site_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 19:00:14.000000 criterion-site-parser-1.6/src/criterion_site_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 19:00:14.000000 criterion-site-parser-1.6/src/criterion_site_parser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:00:14.539688 criterion-site-parser-1.6/src/critparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/CriterionMiniSeriesParse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/CriterionMovieParse.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/CriterionParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/OutApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/OutText.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/critparse/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:00:14.539688 criterion-site-parser-1.6/src/testcritparse/
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/testcritparse/test_CriterionMovieParse.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-03-27 19:00:01.000000 criterion-site-parser-1.6/src/testcritparse/test_CriterionParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/license
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.513909 criterion-site-parser-1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/src/critparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/CriterionMiniSeriesParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/CriterionMovieParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/CriterionParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/OutApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/OutText.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/src/testcritparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/testcritparse/test_CriterionMovieParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/testcritparse/test_CriterionParser.py
```

### Comparing `criterion-site-parser-1.6/PKG-INFO` & `criterion-site-parser-1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criterion-site-parser
-Version: 1.6
+Version: 1.7
 Summary: Prints movies information parsed from criterionchannel.com
 Author-email: pistolbarrel <gboes@pistolbarrel.net>
 License: MIT License
         
         Copyright (c) 2022 pistolbarrel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `criterion-site-parser-1.6/license` & `criterion-site-parser-1.7/license`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/pyproject.toml` & `criterion-site-parser-1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "criterion-site-parser"
-version = "1.6"
+version = "1.7"
 description = "Prints movies information parsed from criterionchannel.com"
 readme = "README.md"
 authors = [{ name = "pistolbarrel", email = "gboes@pistolbarrel.net" }]
 license = { file = "license" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `criterion-site-parser-1.6/src/criterion_site_parser.egg-info/PKG-INFO` & `criterion-site-parser-1.7/src/criterion_site_parser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criterion-site-parser
-Version: 1.6
+Version: 1.7
 Summary: Prints movies information parsed from criterionchannel.com
 Author-email: pistolbarrel <gboes@pistolbarrel.net>
 License: MIT License
         
         Copyright (c) 2022 pistolbarrel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `criterion-site-parser-1.6/src/criterion_site_parser.egg-info/SOURCES.txt` & `criterion-site-parser-1.7/src/criterion_site_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/src/critparse/CriterionMiniSeriesParse.py` & `criterion-site-parser-1.7/src/critparse/CriterionMiniSeriesParse.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/src/critparse/CriterionMovieParse.py` & `criterion-site-parser-1.7/src/critparse/CriterionMovieParse.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/src/critparse/CriterionParser.py` & `criterion-site-parser-1.7/src/critparse/CriterionParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,21 @@
         :return: None
         """
         for movie in movies_list:
             time, url = movie[0], movie[1]
             response = requests.get(url)
             soup = BeautifulSoup(response.content, 'html5lib')
             url_type = CriterionParser.determine_url_type(soup)
-            if url_type == 'collection':
-                time, url = CriterionParser.extract_title_feature_from_collection(soup)[0]
+            if url_type == 'collection' or url_type == 'edition':
+                time, url, title = CriterionParser.extract_title_feature_from_collection(soup)[0]
                 if time == '0:00':
                     continue
+            elif not url_type:
+                # can't deal with a series or movie list embedded in a series or movie list
+                continue
             movie_parser = CriterionMovieParse.MovieParse(url, time)
             self.all_movie_parsed_data.append(movie_parser.get_parsed_info())
         # a collection of one is not a (named) collection
         if len(self.all_movie_parsed_data) == 1 and self.url_type == "collection":
             self.series_name = ""
 
     def __explore_possible_collections(self, movies_list):
@@ -260,15 +263,15 @@
     def determine_url_type(soup):
         """
         Determines the type of url of the soup instance.
 
         :param soup: instance to search/parse
 
         :return:
-            "" represents a series or movie list.
+            None represents a series or movie list.
             "movie" represents a movie link.
             "collection" represents a cover page to one movie.
             "edition" is a Criterion Edition set of movies.
         """
         match_star = CriterionParser.match_star
         match_directed_by = CriterionParser.match_directed_by
         match_edition = CriterionParser.match_edition
```

### Comparing `criterion-site-parser-1.6/src/critparse/OutApi.py` & `criterion-site-parser-1.7/src/critparse/OutApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             print('Added "' + movie_info.title + '" via api')
 
     if not suppress_print:
         print()
 
 
 def addViaApi(movie, collection=None, supplied_length=None):
-    put_uri = "http://localhost:8080/rest/movie"
+    put_uri = "http://tower.local:8080/rest/movie"
     movie_dto = {"title": movie.just_title,
                  "year": movie.year,
                  "actors": movie.stars,
                  "directors": movie.director,
                  "countries": movie.country,
                  "collections": collection,
                  "description": movie.descr}
```

### Comparing `criterion-site-parser-1.6/src/critparse/OutText.py` & `criterion-site-parser-1.7/src/critparse/OutText.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/src/critparse/__main__.py` & `criterion-site-parser-1.7/src/critparse/__main__.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/src/testcritparse/test_CriterionMovieParse.py` & `criterion-site-parser-1.7/src/testcritparse/test_CriterionMovieParse.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.6/src/testcritparse/test_CriterionParser.py` & `criterion-site-parser-1.7/src/testcritparse/test_CriterionParser.py`

 * *Files identical despite different names*

