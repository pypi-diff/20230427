# Comparing `tmp/ms-mint-app-0.2.3.0.tar.gz` & `tmp/ms-mint-app-0.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-app-0.2.3.0.tar", last modified: Thu Apr 27 15:34:44 2023, max compression
+gzip compressed data, was "ms-mint-app-0.2.3.1.tar", last modified: Thu Apr 27 16:21:08 2023, max compression
```

## Comparing `ms-mint-app-0.2.3.0.tar` & `ms-mint-app-0.2.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.267049 ms-mint-app-0.2.3.0/ms_mint_app/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 15:34:44.267049 ms-mint-app-0.2.3.0/ms_mint_app/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/add_metab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/hierachical_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/ms_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/peak_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/quality_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/ms_mint_app/static/
--rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Chem.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Groups.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/Standard_Peaklist.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/ms_mint_app/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21604 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/ms_mint_app/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/ms_mint_app/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.251048 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/scripts/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:34:44.267049 ms-mint-app-0.2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/ms_mint_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/ms_mint_app/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/add_metab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/hierachical_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/ms_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/peak_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/quality_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/ms_mint_app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/static/ChEBI-Chem.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/static/ChEBI-Groups.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/static/Standard_Peaklist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:20:50.000000 ms-mint-app-0.2.3.1/ms_mint_app/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-27 16:20:51.000000 ms-mint-app-0.2.3.1/ms_mint_app/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21604 2023-04-27 16:20:51.000000 ms-mint-app-0.2.3.1/ms_mint_app/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-27 16:20:51.000000 ms-mint-app-0.2.3.1/ms_mint_app/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:21:08.776207 ms-mint-app-0.2.3.1/ms_mint_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 16:21:08.000000 ms-mint-app-0.2.3.1/ms_mint_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 16:21:08.000000 ms-mint-app-0.2.3.1/ms_mint_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:21:08.000000 ms-mint-app-0.2.3.1/ms_mint_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 16:21:08.000000 ms-mint-app-0.2.3.1/ms_mint_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 16:21:08.000000 ms-mint-app-0.2.3.1/ms_mint_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-27 16:20:51.000000 ms-mint-app-0.2.3.1/scripts/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 16:21:08.788207 ms-mint-app-0.2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-27 16:20:51.000000 ms-mint-app-0.2.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-27 16:20:51.000000 ms-mint-app-0.2.3.1/versioneer.py
```

### Comparing `ms-mint-app-0.2.3.0/LICENSE` & `ms-mint-app-0.2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/PKG-INFO` & `ms-mint-app-0.2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.2.3.0
+Version: 0.2.3.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-app-0.2.3.0/README.md` & `ms-mint-app-0.2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/add_metab.py` & `ms-mint-app-0.2.3.1/ms_mint_app/add_metab.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/analysis.py` & `ms-mint-app-0.2.3.1/ms_mint_app/analysis.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/app.py` & `ms-mint-app-0.2.3.1/ms_mint_app/app.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/auth.py` & `ms-mint-app-0.2.3.1/ms_mint_app/auth.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/database.py` & `ms-mint-app-0.2.3.1/ms_mint_app/database.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/distributions.py` & `ms-mint-app-0.2.3.1/ms_mint_app/distributions.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/filelock.py` & `ms-mint-app-0.2.3.1/ms_mint_app/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/heatmap.py` & `ms-mint-app-0.2.3.1/ms_mint_app/heatmap.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/hierachical_clustering.py` & `ms-mint-app-0.2.3.1/ms_mint_app/hierachical_clustering.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/messages.py` & `ms-mint-app-0.2.3.1/ms_mint_app/messages.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/metadata.py` & `ms-mint-app-0.2.3.1/ms_mint_app/metadata.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/ms_files.py` & `ms-mint-app-0.2.3.1/ms_mint_app/ms_files.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/pca.py` & `ms-mint-app-0.2.3.1/ms_mint_app/pca.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/peak_optimization.py` & `ms-mint-app-0.2.3.1/ms_mint_app/peak_optimization.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/plotting.py` & `ms-mint-app-0.2.3.1/ms_mint_app/plotting.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/processing.py` & `ms-mint-app-0.2.3.1/ms_mint_app/processing.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/quality_control.py` & `ms-mint-app-0.2.3.1/ms_mint_app/quality_control.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Chem.parquet` & `ms-mint-app-0.2.3.1/ms_mint_app/static/ChEBI-Chem.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Groups.parquet` & `ms-mint-app-0.2.3.1/ms_mint_app/static/ChEBI-Groups.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/targets.py` & `ms-mint-app-0.2.3.1/ms_mint_app/targets.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/tools.py` & `ms-mint-app-0.2.3.1/ms_mint_app/tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app/workspaces.py` & `ms-mint-app-0.2.3.1/ms_mint_app/workspaces.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app.egg-info/PKG-INFO` & `ms-mint-app-0.2.3.1/ms_mint_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.2.3.0
+Version: 0.2.3.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-app-0.2.3.0/ms_mint_app.egg-info/SOURCES.txt` & `ms-mint-app-0.2.3.1/ms_mint_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/scripts/Mint.py` & `ms-mint-app-0.2.3.1/scripts/Mint.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/setup.py` & `ms-mint-app-0.2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.0/versioneer.py` & `ms-mint-app-0.2.3.1/versioneer.py`

 * *Files identical despite different names*

