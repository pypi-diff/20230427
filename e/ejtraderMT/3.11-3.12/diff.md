# Comparing `tmp/ejtraderMT-3.11.tar.gz` & `tmp/ejtraderMT-3.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderMT-3.11.tar", last modified: Thu Jan 12 19:58:46 2023, max compression
+gzip compressed data, was "ejtraderMT-3.12.tar", last modified: Thu Apr 27 19:08:32 2023, max compression
```

## Comparing `ejtraderMT-3.11.tar` & `ejtraderMT-3.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-01-12 19:58:46.784522 ejtraderMT-3.11/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    35128 2023-01-12 18:53:17.000000 ejtraderMT-3.11/LICENSE
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       64 2023-01-12 18:53:17.000000 ejtraderMT-3.11/MANIFEST.in
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    14550 2023-01-12 19:58:46.784670 ejtraderMT-3.11/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    13279 2023-01-12 18:53:17.000000 ejtraderMT-3.11/README.md
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-01-12 19:58:46.782413 ejtraderMT-3.11/ejtraderMT/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       37 2023-01-12 18:53:17.000000 ejtraderMT-3.11/ejtraderMT/__init__.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-01-12 19:58:46.784271 ejtraderMT-3.11/ejtraderMT/api/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-01-12 18:53:17.000000 ejtraderMT-3.11/ejtraderMT/api/__init__.py
--rwxr-xr-x   0 emersonpedroso   (501) staff       (20)    28658 2023-01-12 19:29:13.000000 ejtraderMT-3.11/ejtraderMT/api/mql.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-01-12 19:58:46.783828 ejtraderMT-3.11/ejtraderMT.egg-info/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    14550 2023-01-12 19:58:46.000000 ejtraderMT-3.11/ejtraderMT.egg-info/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      306 2023-01-12 19:58:46.000000 ejtraderMT-3.11/ejtraderMT.egg-info/SOURCES.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        1 2023-01-12 19:58:46.000000 ejtraderMT-3.11/ejtraderMT.egg-info/dependency_links.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      115 2023-01-12 19:58:46.000000 ejtraderMT-3.11/ejtraderMT.egg-info/requires.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       11 2023-01-12 19:58:46.000000 ejtraderMT-3.11/ejtraderMT.egg-info/top_level.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      110 2023-01-12 19:53:57.000000 ejtraderMT-3.11/requirements.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       79 2023-01-12 19:58:46.785372 ejtraderMT-3.11/setup.cfg
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     1989 2023-01-12 19:54:28.000000 ejtraderMT-3.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-04-27 19:08:19.000000 ejtraderMT-3.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 19:08:19.000000 ejtraderMT-3.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-04-27 19:08:32.212210 ejtraderMT-3.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-04-27 19:08:19.000000 ejtraderMT-3.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/ejtraderMT/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 19:08:19.000000 ejtraderMT-3.12/ejtraderMT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/ejtraderMT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:19.000000 ejtraderMT-3.12/ejtraderMT/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28732 2023-04-27 19:08:19.000000 ejtraderMT-3.12/ejtraderMT/api/mql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:08:32.208210 ejtraderMT-3.12/ejtraderMT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 19:08:32.000000 ejtraderMT-3.12/ejtraderMT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 19:08:19.000000 ejtraderMT-3.12/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 19:08:32.212210 ejtraderMT-3.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-27 19:08:19.000000 ejtraderMT-3.12/setup.py
```

### Comparing `ejtraderMT-3.11/LICENSE` & `ejtraderMT-3.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.11/PKG-INFO` & `ejtraderMT-3.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.11
+Version: 3.12
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
@@ -20,17 +20,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
 
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderMT/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)
+
 # EjtraderMT Python Metatrader 5 API
 
 
 ##### Install stable version using pip 
 ```
 pip install ejtraderMT -U
 ```
```

### Comparing `ejtraderMT-3.11/README.md` & `ejtraderMT-3.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderMT/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)
+
 # EjtraderMT Python Metatrader 5 API
 
 
 ##### Install stable version using pip 
 ```
 pip install ejtraderMT -U
 ```
```

### Comparing `ejtraderMT-3.11/ejtraderMT/api/mql.py` & `ejtraderMT-3.12/ejtraderMT/api/mql.py`

 * *Files 1% similar despite different names*

```diff
@@ -759,16 +759,17 @@
                                     del current[5]
                                 else:
                                     del current[6]
                     
                                 current.columns = [f'{active}_open', f'{active}_high',
                                                 f'{active}_low', f'{active}_close', f'{active}_volume', f'{active}_spread']
 
-                            main = pd.merge(main, current, how='inner',
-                                            left_index=True, right_index=True)
+                            # main = pd.merge(main, current, how='inner',
+                            #                 left_index=True, right_index=True)
+                            main = pd.merge(main, current, on='date')
                         except KeyError:
                             pass
                 
                 main = main.loc[~main.index.duplicated(keep='first')]
                 appended_data.append(main)
              
                 start_date += delta
```

### Comparing `ejtraderMT-3.11/ejtraderMT.egg-info/PKG-INFO` & `ejtraderMT-3.12/ejtraderMT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.11
+Version: 3.12
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
@@ -20,17 +20,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
 
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderMT/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderMT)
+
 # EjtraderMT Python Metatrader 5 API
 
 
 ##### Install stable version using pip 
 ```
 pip install ejtraderMT -U
 ```
```

### Comparing `ejtraderMT-3.11/setup.py` & `ejtraderMT-3.12/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderMT',
-    version='3.11',
+    version='3.12',
     packages=find_packages(),
     url='https://ejtraderMT.readthedocs.io/',
     download_url='https://ejtrader.com',
     license='MIT License',
     author='Emerson Pedroso',
     author_email='support@ejtrader.com',
     description='Metatrader API',
@@ -39,22 +39,19 @@
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
         'metatrader', 'f-api', 'historical-data',
         'financial-data', 'stocks', 'funds', 'etfs',
         'indices', 'currency crosses', 'bonds', 'commodities',
         'crypto currencies'
     ]),
     project_urls={
         'Bug Reports': 'https://github.com/traderpedroso/ejtraderMT/issues',
         'Source': 'https://github.com/traderpedroso/ejtraderMT',
         'Documentation': 'https://ejtrader.readthedocs.io/'
     },
-)
+)
```

