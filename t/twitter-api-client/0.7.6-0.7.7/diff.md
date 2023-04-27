# Comparing `tmp/twitter-api-client-0.7.6.tar.gz` & `tmp/twitter-api-client-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.6.tar", last modified: Sun Apr 23 20:08:51 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.7.tar", last modified: Thu Apr 27 14:29:21 2023, max compression
```

## Comparing `twitter-api-client-0.7.6.tar` & `twitter-api-client-0.7.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.6/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6242 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7452 2023-04-23 20:08:46.000000 twitter-api-client-0.7.6/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.6/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.6/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.6/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.6/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11158 2023-04-23 03:55:18.000000 twitter-api-client-0.7.6/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.6/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.6/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-23 20:08:51.453165 twitter-api-client-0.7.6/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6242 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-23 20:08:51.000000 twitter-api-client-0.7.6/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.7/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6243 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7453 2023-04-27 14:27:22.000000 twitter-api-client-0.7.7/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.7/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.7/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.7/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.7/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11024 2023-04-27 14:26:15.000000 twitter-api-client-0.7.7/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.7/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.7/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6243 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.6/LICENSE` & `twitter-api-client-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.6/PKG-INFO` & `twitter-api-client-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
-Requires-Python: >=3.11.0
+Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Implementation of Twitter's v1, v2, and GraphQL APIs
 
 Includes tools to **scrape**, **automate**, and **search**.
```

### Comparing `twitter-api-client-0.7.6/setup.py` & `twitter-api-client-0.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.6",
-    python_requires=">=3.11.0",
+    version="0.7.7",
+    python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     Implementation of Twitter's v1, v2, and GraphQL APIs
     
     Includes tools to **scrape**, **automate**, and **search**.
 
     ### Automation
```

### Comparing `twitter-api-client-0.7.6/twitter/account.py` & `twitter-api-client-0.7.7/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.6/twitter/constants.py` & `twitter-api-client-0.7.7/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.6/twitter/login.py` & `twitter-api-client-0.7.7/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.6/twitter/scraper.py` & `twitter-api-client-0.7.7/twitter/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,18 +155,14 @@
             prev_len = len(ids)
             if prev_len >= limit:
                 return res
 
             r = await self._query(session, _id, operation, cursor=cursor)
             data = r.json()
 
-            if len(find_key(data, 'entries')[0]) <= 2:
-                # only top/bottom cursor in result
-                return res
-
             cursor = get_cursor(data)
             ids |= set(find_key(data, 'rest_id'))
 
             if self.debug:
                 logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
 
             if prev_len == len(ids):
```

### Comparing `twitter-api-client-0.7.6/twitter/search.py` & `twitter-api-client-0.7.7/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.6/twitter/util.py` & `twitter-api-client-0.7.7/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.6/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.7/twitter_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
-Requires-Python: >=3.11.0
+Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Implementation of Twitter's v1, v2, and GraphQL APIs
 
 Includes tools to **scrape**, **automate**, and **search**.
```

