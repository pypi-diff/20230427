# Comparing `tmp/ms-mint-app-0.2.2.2.tar.gz` & `tmp/ms-mint-app-0.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-app-0.2.2.2.tar", last modified: Thu Mar  9 23:46:43 2023, max compression
+gzip compressed data, was "ms-mint-app-0.2.3.0.tar", last modified: Thu Apr 27 15:34:44 2023, max compression
```

## Comparing `ms-mint-app-0.2.2.2.tar` & `ms-mint-app-0.2.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:43.074008 ms-mint-app-0.2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-09 23:46:43.074008 ms-mint-app-0.2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:43.074008 ms-mint-app-0.2.2.2/ms_mint_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-09 23:46:43.074008 ms-mint-app-0.2.2.2/ms_mint_app/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/add_metab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/hierachical_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/ms_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/peak_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/quality_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:43.070008 ms-mint-app-0.2.2.2/ms_mint_app/static/
--rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/static/ChEBI-Chem.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/static/ChEBI-Groups.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/static/Standard_Peaklist.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:32.000000 ms-mint-app-0.2.2.2/ms_mint_app/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-03-09 23:46:33.000000 ms-mint-app-0.2.2.2/ms_mint_app/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    20834 2023-03-09 23:46:33.000000 ms-mint-app-0.2.2.2/ms_mint_app/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-03-09 23:46:33.000000 ms-mint-app-0.2.2.2/ms_mint_app/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:43.058008 ms-mint-app-0.2.2.2/ms_mint_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-09 23:46:42.000000 ms-mint-app-0.2.2.2/ms_mint_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-09 23:46:43.000000 ms-mint-app-0.2.2.2/ms_mint_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 23:46:42.000000 ms-mint-app-0.2.2.2/ms_mint_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-09 23:46:42.000000 ms-mint-app-0.2.2.2/ms_mint_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 23:46:42.000000 ms-mint-app-0.2.2.2/ms_mint_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 23:46:43.070008 ms-mint-app-0.2.2.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-03-09 23:46:33.000000 ms-mint-app-0.2.2.2/scripts/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-09 23:46:43.074008 ms-mint-app-0.2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-09 23:46:33.000000 ms-mint-app-0.2.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-03-09 23:46:33.000000 ms-mint-app-0.2.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.267049 ms-mint-app-0.2.3.0/ms_mint_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 15:34:44.267049 ms-mint-app-0.2.3.0/ms_mint_app/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/add_metab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/hierachical_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/ms_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/peak_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/quality_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/ms_mint_app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Chem.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Groups.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/Standard_Peaklist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:17.000000 ms-mint-app-0.2.3.0/ms_mint_app/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/ms_mint_app/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21604 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/ms_mint_app/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/ms_mint_app/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.251048 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:34:44.000000 ms-mint-app-0.2.3.0/ms_mint_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:34:44.263049 ms-mint-app-0.2.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/scripts/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:34:44.267049 ms-mint-app-0.2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-27 15:34:18.000000 ms-mint-app-0.2.3.0/versioneer.py
```

### Comparing `ms-mint-app-0.2.2.2/LICENSE` & `ms-mint-app-0.2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/PKG-INFO` & `ms-mint-app-0.2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.2.2.2
+Version: 0.2.3.0
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,30 @@
 The metabolites can be used to define biomarkers used in medicine to find treatments for diseases or for the development of diagnostic tests 
 or for the identification of pathogens such as methicillin resistant _Staphylococcus aureus_ (MRSA). 
 More information on how to install and run the program can be found in the [Documentation](https://LewisResearchGroup.github.io/ms-mint-app/) or check out the 
 [Tutorial](https:///LewisResearchGroup.github.io/ms-mint-app/quickstart/) to jump right into it.
 
 ## Release notes
 
+### 0.3.0 Milestones
+- Be able to share a workspace with another user
+- Be able to rename a workspace
+- Explanation of expected metadata in app
+  - explain what can be put as colors
+- describe accepted file types in ms_files tab
+- target-list add columns database_ref, formula, polarity
+- add descriptions to the optimization tab
+- total ion chromatogram (TIC)
+- full extracted ion chromatogram (EIC or XIC)
+- feature to convert intensities to concentrations
+
+### 0.2.2
+- version strings in GUI
+- fixed issues with QC figures
+
 ### 0.2.1
 - uses ms-mint 0.2.1 with new implementation of `peak_area_top3`
 - new quality control tab
 
 ### 0.1.9
 MINT has been split into the Python library and the app. This repository contains the Python library. The underlying Python library `ms-mint` can be found [here](https://github.com/LewisResearchGroup/ms-mint).
```

### Comparing `ms-mint-app-0.2.2.2/README.md` & `ms-mint-app-0.2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,30 @@
 The metabolites can be used to define biomarkers used in medicine to find treatments for diseases or for the development of diagnostic tests 
 or for the identification of pathogens such as methicillin resistant _Staphylococcus aureus_ (MRSA). 
 More information on how to install and run the program can be found in the [Documentation](https://LewisResearchGroup.github.io/ms-mint-app/) or check out the 
 [Tutorial](https:///LewisResearchGroup.github.io/ms-mint-app/quickstart/) to jump right into it.
 
 ## Release notes
 
+### 0.3.0 Milestones
+- Be able to share a workspace with another user
+- Be able to rename a workspace
+- Explanation of expected metadata in app
+  - explain what can be put as colors
+- describe accepted file types in ms_files tab
+- target-list add columns database_ref, formula, polarity
+- add descriptions to the optimization tab
+- total ion chromatogram (TIC)
+- full extracted ion chromatogram (EIC or XIC)
+- feature to convert intensities to concentrations
+
+### 0.2.2
+- version strings in GUI
+- fixed issues with QC figures
+
 ### 0.2.1
 - uses ms-mint 0.2.1 with new implementation of `peak_area_top3`
 - new quality control tab
 
 ### 0.1.9
 MINT has been split into the Python library and the app. This repository contains the Python library. The underlying Python library `ms-mint` can be found [here](https://github.com/LewisResearchGroup/ms-mint).
```

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/add_metab.py` & `ms-mint-app-0.2.3.0/ms_mint_app/add_metab.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/analysis.py` & `ms-mint-app-0.2.3.0/ms_mint_app/analysis.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/app.py` & `ms-mint-app-0.2.3.0/ms_mint_app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,25 @@
 
 from dash import html, dcc
 
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 from dash.dcc import Download
 from dash_extensions.enrich import FileSystemCache
+from dash.long_callback import DiskcacheLongCallbackManager
+
+
 
 import dash_bootstrap_components as dbc
 
 from flask_caching import Cache
 from flask_login import current_user
 
 import ms_mint
+import ms_mint_app
 
 from . import tools as T
 
 from . import workspaces
 from . import ms_files
 from . import metadata
 from . import targets
@@ -57,14 +61,26 @@
 
 config = {
     "DEBUG": True,  # some Flask specific configs
     "CACHE_TYPE": "simple",  # Flask-Caching related configs
     "CACHE_DEFAULT_TIMEOUT": 300,
 }
 
+logging.info(f'CACHEDIR: {CACHEDIR}')
+logging.info(f'TMPDIR: {TMPDIR}')
+
+## Diskcache
+from uuid import uuid4
+import diskcache
+launch_uid = uuid4()
+cache = diskcache.Cache(CACHEDIR)
+long_callback_manager = DiskcacheLongCallbackManager(
+    cache, cache_by=[lambda: launch_uid], expire=60,
+)
+
 pd.options.display.max_colwidth = 1000
 
 _modules = [
     workspaces,
     ms_files,
     metadata,
     targets,
@@ -162,16 +178,19 @@
 
         messages.layout(),
 
         html.Div(id="pko-image-store", style={"visibility": "hidden", "height": "0px"}),
         html.Div(id="tab-content"),
         html.Div(id="viewport-container", style={"visibility": "hidden"}),
         _outputs,
+        html.Div(f'ms-mint: {ms_mint.__version__}'),
+        html.Div(f'ms-mint-app: {ms_mint_app.__version__}'),
     ],
     style={"margin": "2%"},
+
 )
 
 
 def register_callbacks(app, cache, fsc):
     logging.info("Register callbacks")
     upload_root = os.getenv("MINT_DATA_DIR", tempfile.gettempdir())
     upload_dir = str(P(upload_root) / "MINT-Uploads")
@@ -238,14 +257,15 @@
 
 def create_app(**kwargs):
 
     logging.warning(f'ms-mint: {ms_mint.__version__}, ({ms_mint.__file__})')
 
     app = dash.Dash(
         __name__,
+        long_callback_manager=long_callback_manager,
         external_stylesheets=[
             dbc.themes.MINTY,
             "https://codepen.io/chriddyp/pen/bWLwgP.css",
         ],
         **kwargs,
     )
```

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/auth.py` & `ms-mint-app-0.2.3.0/ms_mint_app/auth.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/database.py` & `ms-mint-app-0.2.3.0/ms_mint_app/database.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/distributions.py` & `ms-mint-app-0.2.3.0/ms_mint_app/distributions.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/filelock.py` & `ms-mint-app-0.2.3.0/ms_mint_app/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/heatmap.py` & `ms-mint-app-0.2.3.0/ms_mint_app/heatmap.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/hierachical_clustering.py` & `ms-mint-app-0.2.3.0/ms_mint_app/hierachical_clustering.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/messages.py` & `ms-mint-app-0.2.3.0/ms_mint_app/messages.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/metadata.py` & `ms-mint-app-0.2.3.0/ms_mint_app/metadata.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/ms_files.py` & `ms-mint-app-0.2.3.0/ms_mint_app/ms_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,15 @@
 
 
     @du.callback(
         output=Output('ms-uploader-fns', 'children'),
         id='ms-uploader',
     )
     def upload_completed(status):
+        logging.warning(f'Upload status: {status} ({type(status)})')
         return [str(fn) for fn in status.uploaded_files]
 
     @app.callback(
         Output({"index": "ms-uploader-output", "type": "output"}, "children"),
         Input("ms-uploader-fns", "children"),
         State("wdir", "children"),
     )
```

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/pca.py` & `ms-mint-app-0.2.3.0/ms_mint_app/pca.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/peak_optimization.py` & `ms-mint-app-0.2.3.0/ms_mint_app/peak_optimization.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/plotting.py` & `ms-mint-app-0.2.3.0/ms_mint_app/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             raise PreventUpdate
         results = T.get_complete_results(wdir)
         results = results.dropna(axis=1, how="all")
         cols = results.columns
         options = [{"value": x, "label": x} for x in cols]
         return [options] * 7
 
-    @app.callback(
+    @app.long_callback(
         Output("plot-figures", "children"),
         Input("plot-update", "n_clicks"),
         State("plot-kind", "value"),
         State("plot-fig-height", "value"),
         State("plot-fig-aspect", "value"),
         State("plot-x", "value"),
         State("plot-y", "value"),
@@ -334,14 +334,15 @@
         State("ana-file-types", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
         State("ana-ms-order", "value"),
         State("plot-palette", "value"),
         State("plot-options", "value"),
         State("wdir", "children"),
+        cancel=[Input("plot-update", "n_clicks")],
     )
     def create_figure(
         n_clicks,
         kind,
         height,
         aspect,
         x,
```

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/processing.py` & `ms-mint-app-0.2.3.0/ms_mint_app/processing.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/quality_control.py` & `ms-mint-app-0.2.3.0/ms_mint_app/quality_control.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/static/ChEBI-Chem.parquet` & `ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Chem.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/static/ChEBI-Groups.parquet` & `ms-mint-app-0.2.3.0/ms_mint_app/static/ChEBI-Groups.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/targets.py` & `ms-mint-app-0.2.3.0/ms_mint_app/targets.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/tools.py` & `ms-mint-app-0.2.3.0/ms_mint_app/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,15 +350,24 @@
         "MS-file",
     ]:
         if col not in df.columns:
             df[col] = None
 
     df = df[df["MS-file"] != ""]
 
-    df = df.groupby("MS-file").first().reindex(ms_files).reset_index()
+    new_files = [e for e in ms_files if e not in df['MS-file'].values]
+
+    df = df.groupby("MS-file").first().reindex(ms_files, ).reset_index()
+    
+    print('NEW FILES:', new_files)
+    if new_files :
+        # Default for PeakOpt for new files should be False
+        ndx = df[df['MS-file'].isin(new_files)].index
+        print('INDEX:', ndx)
+        df.loc[ndx, 'PeakOpt'] = False
 
     if "PeakOpt" not in df.columns:
         df["PeakOpt"] = False
 
     else:
         df["PeakOpt"] = df["PeakOpt"].astype(bool)
 
@@ -382,15 +391,15 @@
 def init_metadata(ms_files):
     ms_files = list(ms_files)
     ms_files = [filename_to_label(fn) for fn in ms_files]
     df = pd.DataFrame({"MS-file": ms_files})
     df["InAnalysis"] = True
     df["Label"] = ""
     df["Color"] = None
-    df["Type"] = "Biological Sample"
+    df["Type"] = "Unknown"
     df["RunOrder"] = ""
     df["Batch"] = ""
     df["Row"] = ""
     df["Column"] = ""
     df["PeakOpt"] = ""
     return df
 
@@ -601,30 +610,45 @@
 
     plt.close("all")
     out_img.seek(0)  # rewind file
     encoded = base64.b64encode(out_img.read()).decode("ascii").replace("\n", "")
     return "data:image/png;base64,{}".format(encoded)
 
 
-def merge_metadata(old, new):
-    old = old.set_index("MS-file")
+def merge_metadata(old: pd.DataFrame, new: pd.DataFrame, index_col='MS-file') -> pd.DataFrame:
+    """
+    This function updates one existing dataframe 
+    with information from a second dataframe.
+    If a column of the new dataframe does not 
+    exist it will be created.
+
+    Parameters:
+    old (pd.DataFrame): The DataFrame to merge new data into.
+    new (pd.DataFrame): The DataFrame containing the new data to merge.
+
+    Returns:
+    pd.DataFrame: The merged DataFrame.
 
-    new = new.groupby("MS-file").first().replace("null", None)
+    """    
+    old = old.set_index(index_col)
+
+    new = new.groupby(index_col).first().replace("null", None)
 
     for col in new.columns:
         if col == "" or col.startswith("Unnamed"):
             continue
         if not col in old.columns:
             old[col] = None
         for ndx in new.index:
             value = new.loc[ndx, col]
             if value is None:
                 continue
             if ndx in old.index:
                 old.loc[ndx, col] = value
+
     return old.reset_index()
 
 
 def file_colors(wdir):
     meta = get_metadata(wdir)
     colors = {}
     for ndx, (fn, co) in meta[["MS-file", "Color"]].iterrows():
```

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app/workspaces.py` & `ms-mint-app-0.2.3.0/ms_mint_app/workspaces.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app.egg-info/PKG-INFO` & `ms-mint-app-0.2.3.0/ms_mint_app.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.2.2.2
+Version: 0.2.3.0
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,30 @@
 The metabolites can be used to define biomarkers used in medicine to find treatments for diseases or for the development of diagnostic tests 
 or for the identification of pathogens such as methicillin resistant _Staphylococcus aureus_ (MRSA). 
 More information on how to install and run the program can be found in the [Documentation](https://LewisResearchGroup.github.io/ms-mint-app/) or check out the 
 [Tutorial](https:///LewisResearchGroup.github.io/ms-mint-app/quickstart/) to jump right into it.
 
 ## Release notes
 
+### 0.3.0 Milestones
+- Be able to share a workspace with another user
+- Be able to rename a workspace
+- Explanation of expected metadata in app
+  - explain what can be put as colors
+- describe accepted file types in ms_files tab
+- target-list add columns database_ref, formula, polarity
+- add descriptions to the optimization tab
+- total ion chromatogram (TIC)
+- full extracted ion chromatogram (EIC or XIC)
+- feature to convert intensities to concentrations
+
+### 0.2.2
+- version strings in GUI
+- fixed issues with QC figures
+
 ### 0.2.1
 - uses ms-mint 0.2.1 with new implementation of `peak_area_top3`
 - new quality control tab
 
 ### 0.1.9
 MINT has been split into the Python library and the app. This repository contains the Python library. The underlying Python library `ms-mint` can be found [here](https://github.com/LewisResearchGroup/ms-mint).
```

### Comparing `ms-mint-app-0.2.2.2/ms_mint_app.egg-info/SOURCES.txt` & `ms-mint-app-0.2.3.0/ms_mint_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/scripts/Mint.py` & `ms-mint-app-0.2.3.0/scripts/Mint.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.2.2/setup.py` & `ms-mint-app-0.2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 install_requires = [
-    "ms-mint==0.2.2",
+    "ms-mint",
     "xlsxwriter",
     "waitress",
     "dash",
     "dash_extensions",
     "dash_bootstrap_components",
     "flask_login",
     "urllib3",
```

### Comparing `ms-mint-app-0.2.2.2/versioneer.py` & `ms-mint-app-0.2.3.0/versioneer.py`

 * *Files identical despite different names*

