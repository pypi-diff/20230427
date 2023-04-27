# Comparing `tmp/hyperfetch-1.0.5.tar.gz` & `tmp/hyperfetch-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.0.5.tar", last modified: Tue Apr 25 19:22:16 2023, max compression
+gzip compressed data, was "hyperfetch-1.0.6.tar", last modified: Wed Apr 26 19:15:11 2023, max compression
```

## Comparing `hyperfetch-1.0.5.tar` & `hyperfetch-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.748423 hyperfetch-1.0.5/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.5/LICENSE
--rw-rw-rw-   0        0        0    10367 2023-04-25 19:22:16.747423 hyperfetch-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.5/README.md
--rw-rw-rw-   0        0        0     4794 2023-04-25 19:14:42.000000 hyperfetch-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 19:22:16.748423 hyperfetch-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.671912 hyperfetch-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.704422 hyperfetch-1.0.5/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-04-16 16:06:24.000000 hyperfetch-1.0.5/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-04-15 07:49:41.000000 hyperfetch-1.0.5/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-04-16 21:41:06.000000 hyperfetch-1.0.5/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     2118 2023-04-13 19:35:11.000000 hyperfetch-1.0.5/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    33572 2023-04-25 19:17:47.000000 hyperfetch-1.0.5/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4926 2023-04-25 19:17:51.000000 hyperfetch-1.0.5/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0      825 2023-04-16 16:50:23.000000 hyperfetch-1.0.5/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:22:16.745423 hyperfetch-1.0.5/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0    10367 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     2238 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 19:22:16.000000 hyperfetch-1.0.5/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 19:15:11.068340 hyperfetch-1.0.6/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0    10466 2023-04-26 19:15:11.068340 hyperfetch-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1689 2023-04-26 19:13:58.000000 hyperfetch-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 19:15:11.068340 hyperfetch-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 19:15:11.033552 hyperfetch-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 19:15:11.039416 hyperfetch-1.0.6/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-04-16 16:06:24.000000 hyperfetch-1.0.6/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-26 18:57:42.000000 hyperfetch-1.0.6/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-04-16 21:41:06.000000 hyperfetch-1.0.6/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     2118 2023-04-13 19:35:11.000000 hyperfetch-1.0.6/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    33572 2023-04-26 19:01:52.000000 hyperfetch-1.0.6/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4991 2023-04-26 19:01:06.000000 hyperfetch-1.0.6/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0      825 2023-04-16 16:50:23.000000 hyperfetch-1.0.6/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:15:11.066350 hyperfetch-1.0.6/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0    10466 2023-04-26 19:15:11.000000 hyperfetch-1.0.6/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-26 19:15:11.000000 hyperfetch-1.0.6/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 19:15:11.000000 hyperfetch-1.0.6/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-26 19:15:11.000000 hyperfetch-1.0.6/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      211 2023-04-26 19:15:11.000000 hyperfetch-1.0.6/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 19:15:11.000000 hyperfetch-1.0.6/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.0.5/LICENSE` & `hyperfetch-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/PKG-INFO` & `hyperfetch-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.5
+Version: 1.0.6
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
@@ -29,14 +29,16 @@
 Project-URL: Website, https://github.com/karolisw/hyperFetch/tree/frontend
 Project-URL: Source, https://github.com/karolisw/hyperFetch
 Keywords: reinforcement learning,hyperparameters,replication
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: FastAPI
 Requires-Python: <3.11.0,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hyperfetch-1.0.5/README.md` & `hyperfetch-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.0.6/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/src/hyperfetch/auth_connection.py` & `hyperfetch-1.0.6/src/hyperfetch/auth_connection.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/src/hyperfetch/callbacks.py` & `hyperfetch-1.0.6/src/hyperfetch/callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/src/hyperfetch/manager.py` & `hyperfetch-1.0.6/src/hyperfetch/manager.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/src/hyperfetch/tuning.py` & `hyperfetch-1.0.6/src/hyperfetch/tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,8 +106,11 @@
     parser = argparse.ArgumentParser(description='"save" script allows for persisting hyperparameters that are not '
                                                  'tuned in HyperFetch.')
     parser.add_argument('config_path', type=str, help='The path to the config file (.yaml). Can be a new file or t'
                                                       'he same as for the tuning() method.')
 
     args = parser.parse_args()
     manager = Manager(config_path=args.config_path)
-    asyncio.run(manager.save_custom(client=MONGODB_URL, db=MONGO_DB, collection=MONGO_COLLECTION))
+    asyncio.run(manager.save_custom(client=MONGODB_URL, db=MONGO_DB, collection=MONGO_COLLECTION))
+
+if __name__ == '__main__':
+    tune("tuning_parameters.yml")
```

### Comparing `hyperfetch-1.0.5/src/hyperfetch/util.py` & `hyperfetch-1.0.6/src/hyperfetch/util.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.5/src/hyperfetch.egg-info/PKG-INFO` & `hyperfetch-1.0.6/src/hyperfetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.5
+Version: 1.0.6
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
@@ -29,14 +29,16 @@
 Project-URL: Website, https://github.com/karolisw/hyperFetch/tree/frontend
 Project-URL: Source, https://github.com/karolisw/hyperFetch
 Keywords: reinforcement learning,hyperparameters,replication
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: FastAPI
 Requires-Python: <3.11.0,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

