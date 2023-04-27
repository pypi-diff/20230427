# Comparing `tmp/ejtraderCT-1.0.8.tar.gz` & `tmp/ejtraderCT-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderCT-1.0.8.tar", last modified: Tue Apr 11 10:56:44 2023, max compression
+gzip compressed data, was "ejtraderCT-1.1.0.tar", last modified: Thu Apr 27 18:57:04 2023, max compression
```

## Comparing `ejtraderCT-1.0.8.tar` & `ejtraderCT-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.038385 ejtraderCT-1.0.8/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    35128 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/LICENSE
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       68 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/MANIFEST.in
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4750 2023-04-11 10:56:44.038521 ejtraderCT-1.0.8/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     3459 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/README.md
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.033737 ejtraderCT-1.0.8/ejtraderCT/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       38 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/__init__.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.037550 ejtraderCT-1.0.8/ejtraderCT/api/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     9963 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/Symbol.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      442 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/buffer.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    17077 2023-04-11 10:54:43.000000 ejtraderCT-1.0.8/ejtraderCT/api/ctrader.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    25262 2023-03-28 18:26:39.000000 ejtraderCT-1.0.8/ejtraderCT/api/fix.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      620 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/math.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.035233 ejtraderCT-1.0.8/ejtraderCT.egg-info/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4750 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      423 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/SOURCES.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        1 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/dependency_links.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       15 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/requires.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       11 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/top_level.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/requirements.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       79 2023-04-11 10:56:44.039148 ejtraderCT-1.0.8/setup.cfg
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2010 2023-04-11 10:56:12.000000 ejtraderCT-1.0.8/setup.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.037950 ejtraderCT-1.0.8/test/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      631 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/test/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/ejtraderCT/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/ejtraderCT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/Symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/ctrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/ejtraderCT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 18:57:04.946202 ejtraderCT-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/test/test_math.py
```

### Comparing `ejtraderCT-1.0.8/LICENSE` & `ejtraderCT-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.8/PKG-INFO` & `ejtraderCT-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.0.8
+Version: 1.1.0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
@@ -20,17 +20,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
 
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
+
 # Python Ctrader Fix API
 
 ### ToDo
 
 - [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
 - [x] Peding orders limit and stop 
@@ -75,15 +76,22 @@
 server="h8.p.c-trader.cn" # Host name
 broker="icmarkets" 
 account="3152339"
 password="393214"
 currency="EUR"
 
 api = Ctrader(server,broker,account,password,currency)
+
+```
+
+##### to Disconnect logout from account 
+```python
+api.logout()
 ```
+
 ### Real time quote
 
 ##### Subscribe to symbol 
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
 ##### All symbols quote list
```

### Comparing `ejtraderCT-1.0.8/README.md` & `ejtraderCT-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
+
 # Python Ctrader Fix API
 
 ### ToDo
 
 - [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
 - [x] Peding orders limit and stop 
@@ -46,15 +48,22 @@
 server="h8.p.c-trader.cn" # Host name
 broker="icmarkets" 
 account="3152339"
 password="393214"
 currency="EUR"
 
 api = Ctrader(server,broker,account,password,currency)
+
+```
+
+##### to Disconnect logout from account 
+```python
+api.logout()
 ```
+
 ### Real time quote
 
 ##### Subscribe to symbol 
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
 ##### All symbols quote list
```

### Comparing `ejtraderCT-1.0.8/ejtraderCT/api/Symbol.py` & `ejtraderCT-1.1.0/ejtraderCT/api/Symbol.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.8/ejtraderCT/api/ctrader.py` & `ejtraderCT-1.1.0/ejtraderCT/api/ctrader.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.8/ejtraderCT/api/fix.py` & `ejtraderCT-1.1.0/ejtraderCT/api/fix.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.8/ejtraderCT/api/math.py` & `ejtraderCT-1.1.0/ejtraderCT/api/math.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.8/ejtraderCT.egg-info/PKG-INFO` & `ejtraderCT-1.1.0/ejtraderCT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.0.8
+Version: 1.1.0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
@@ -20,17 +20,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
 
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
+
 # Python Ctrader Fix API
 
 ### ToDo
 
 - [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
 - [x] Peding orders limit and stop 
@@ -75,15 +76,22 @@
 server="h8.p.c-trader.cn" # Host name
 broker="icmarkets" 
 account="3152339"
 password="393214"
 currency="EUR"
 
 api = Ctrader(server,broker,account,password,currency)
+
+```
+
+##### to Disconnect logout from account 
+```python
+api.logout()
 ```
+
 ### Real time quote
 
 ##### Subscribe to symbol 
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
 ##### All symbols quote list
```

### Comparing `ejtraderCT-1.0.8/setup.py` & `ejtraderCT-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderCT',
-    version='1.0.8',
+    version='1.1.0',
     packages=find_packages(),
     url='https://ejtraderCT.readthedocs.io/',
     download_url='https://ejtrader.com',
     license='MIT License',
     author='Emerson Pedroso & Douglas Barros',
     author_email='support@ejtrader.com',
     description='Ctrader Fix API',
@@ -39,17 +39,14 @@
         "Intended Audience :: Developers",
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Investment",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries"
     ],
     python_requires='>=3',
-    extras_require={
-        "docs": requirements(filename='docs/requirements.txt')
-    },
     keywords=', '.join([
         'ctrader', 'fix-api', 'historical-data',
         'financial-data', 'stocks', 'funds', 'etfs',
         'indices', 'currency crosses', 'bonds', 'commodities',
         'crypto currencies'
     ]),
     project_urls={
```

### Comparing `ejtraderCT-1.0.8/test/test_math.py` & `ejtraderCT-1.1.0/test/test_math.py`

 * *Files identical despite different names*

