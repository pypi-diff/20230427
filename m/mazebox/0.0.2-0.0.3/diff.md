# Comparing `tmp/mazebox-0.0.2.tar.gz` & `tmp/mazebox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/smgroves/Documents/GitHub/mazebox/dist/tmpwkcq_sfg/mazebox-0.0.2.tar", last modified: Sun Oct  2 03:12:35 2022, max compression
+gzip compressed data, was "/Users/smgroves/Documents/GitHub/mazebox/dist/.tmp-pd2qbpag/mazebox-0.0.3.tar", last modified: Thu Apr 27 16:54:01 2023, max compression
```

## Comparing `mazebox-0.0.2.tar` & `mazebox-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,43 @@
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/
--rw-r--r--   0 smgroves   (501) staff       (20)     1069 2022-10-02 02:46:42.000000 mazebox-0.0.2/LICENSE
--rw-r--r--   0 smgroves   (501) staff       (20)     1451 2022-10-02 03:12:35.000000 mazebox-0.0.2/PKG-INFO
--rw-r--r--   0 smgroves   (501) staff       (20)      830 2022-10-02 03:09:49.000000 mazebox-0.0.2/README.rst
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox/
--rw-r--r--   0 smgroves   (501) staff       (20)      820 2021-12-03 02:50:28.000000 mazebox-0.0.2/mazebox/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)     5219 2021-12-03 02:50:30.000000 mazebox-0.0.2/mazebox/_settings.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox/archetypes/
--rw-r--r--   0 smgroves   (501) staff       (20)      332 2022-01-15 02:14:12.000000 mazebox-0.0.2/mazebox/archetypes/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)     5955 2022-01-10 23:54:04.000000 mazebox-0.0.2/mazebox/archetypes/_bulk_signature.py
--rw-r--r--   0 smgroves   (501) staff       (20)    15399 2022-01-19 23:17:18.000000 mazebox-0.0.2/mazebox/archetypes/_cell_state_space.py
--rw-r--r--   0 smgroves   (501) staff       (20)     6591 2022-01-10 23:48:17.000000 mazebox-0.0.2/mazebox/archetypes/_intra_inter_heterogeneity.py
--rw-r--r--   0 smgroves   (501) staff       (20)    17703 2022-01-19 23:19:32.000000 mazebox-0.0.2/mazebox/archetypes/_signature_scoring.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox/network/
--rw-r--r--   0 smgroves   (501) staff       (20)       62 2021-12-03 02:05:08.000000 mazebox-0.0.2/mazebox/network/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)        0 2020-11-26 18:23:00.000000 mazebox-0.0.2/mazebox/network/_build_network.py
--rw-r--r--   0 smgroves   (501) staff       (20)        0 2020-11-26 18:27:01.000000 mazebox-0.0.2/mazebox/network/_fit.py
--rw-r--r--   0 smgroves   (501) staff       (20)        0 2020-11-26 18:27:06.000000 mazebox-0.0.2/mazebox/network/_sim.py
--rw-r--r--   0 smgroves   (501) staff       (20)        0 2020-11-26 18:27:12.000000 mazebox-0.0.2/mazebox/network/_utils.py
--rw-r--r--   0 smgroves   (501) staff       (20)     1895 2021-12-03 02:05:08.000000 mazebox-0.0.2/mazebox/network/generate_timepoints.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox/plasticity/
--rw-r--r--   0 smgroves   (501) staff       (20)      215 2021-07-21 18:35:47.000000 mazebox-0.0.2/mazebox/plasticity/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)    17390 2022-02-09 23:02:36.000000 mazebox-0.0.2/mazebox/plasticity/_ctrp.py
--rw-r--r--   0 smgroves   (501) staff       (20)     4710 2021-12-03 02:50:03.000000 mazebox-0.0.2/mazebox/plasticity/_utils.py
--rw-r--r--   0 smgroves   (501) staff       (20)      957 2021-12-03 02:50:06.000000 mazebox-0.0.2/mazebox/plasticity/_velocity.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox/plotting/
--rw-r--r--   0 smgroves   (501) staff       (20)      313 2022-01-10 23:48:05.000000 mazebox-0.0.2/mazebox/plotting/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)    25021 2021-12-03 02:50:14.000000 mazebox-0.0.2/mazebox/plotting/_archetype_plots.py
--rw-r--r--   0 smgroves   (501) staff       (20)     3070 2022-01-19 23:15:40.000000 mazebox-0.0.2/mazebox/plotting/_circular_projection.py
--rw-r--r--   0 smgroves   (501) staff       (20)       81 2020-11-26 18:25:11.000000 mazebox-0.0.2/mazebox/plotting/_network_plots.py
--rw-r--r--   0 smgroves   (501) staff       (20)     1918 2021-12-03 02:50:22.000000 mazebox-0.0.2/mazebox/plotting/_plasticity_plots.py
--rw-r--r--   0 smgroves   (501) staff       (20)     5350 2021-12-03 02:50:19.000000 mazebox-0.0.2/mazebox/plotting/_utils.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox/preprocessing/
--rw-r--r--   0 smgroves   (501) staff       (20)      180 2021-01-04 20:09:55.000000 mazebox-0.0.2/mazebox/preprocessing/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)     7510 2022-01-10 19:07:05.000000 mazebox-0.0.2/mazebox/preprocessing/_filter.py
--rw-r--r--   0 smgroves   (501) staff       (20)     1118 2021-12-03 02:49:18.000000 mazebox-0.0.2/mazebox/preprocessing/_imputation.py
--rw-r--r--   0 smgroves   (501) staff       (20)     2018 2021-12-01 16:18:38.000000 mazebox-0.0.2/mazebox/preprocessing/_integrate.py
--rw-r--r--   0 smgroves   (501) staff       (20)      189 2021-12-03 02:50:26.000000 mazebox-0.0.2/mazebox/preprocessing/_read.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox.egg-info/
--rw-r--r--   0 smgroves   (501) staff       (20)     1451 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox.egg-info/PKG-INFO
--rw-r--r--   0 smgroves   (501) staff       (20)     1109 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox.egg-info/SOURCES.txt
--rw-r--r--   0 smgroves   (501) staff       (20)        1 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox.egg-info/dependency_links.txt
--rw-r--r--   0 smgroves   (501) staff       (20)      205 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox.egg-info/requires.txt
--rw-r--r--   0 smgroves   (501) staff       (20)        8 2022-10-02 03:12:35.000000 mazebox-0.0.2/mazebox.egg-info/top_level.txt
--rw-r--r--   0 smgroves   (501) staff       (20)       80 2022-10-02 02:58:36.000000 mazebox-0.0.2/pyproject.toml
--rw-r--r--   0 smgroves   (501) staff       (20)       38 2022-10-02 03:12:35.000000 mazebox-0.0.2/setup.cfg
--rw-r--r--   0 smgroves   (501) staff       (20)     1489 2022-10-02 03:12:08.000000 mazebox-0.0.2/setup.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/
+-rw-r--r--   0 smgroves   (501) staff       (20)     1069 2022-10-02 02:46:42.000000 mazebox-0.0.3/LICENSE
+-rw-r--r--   0 smgroves   (501) staff       (20)     1521 2023-04-27 16:54:01.000000 mazebox-0.0.3/PKG-INFO
+-rw-r--r--   0 smgroves   (501) staff       (20)      900 2023-04-27 16:53:43.000000 mazebox-0.0.3/README.rst
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox/
+-rw-r--r--   0 smgroves   (501) staff       (20)      820 2021-12-03 02:50:28.000000 mazebox-0.0.3/mazebox/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     5219 2021-12-03 02:50:30.000000 mazebox-0.0.3/mazebox/_settings.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox/archetypes/
+-rw-r--r--   0 smgroves   (501) staff       (20)      332 2022-01-15 02:14:12.000000 mazebox-0.0.3/mazebox/archetypes/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     5955 2022-01-10 23:54:04.000000 mazebox-0.0.3/mazebox/archetypes/_bulk_signature.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    15399 2022-01-19 23:17:18.000000 mazebox-0.0.3/mazebox/archetypes/_cell_state_space.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     6591 2022-01-10 23:48:17.000000 mazebox-0.0.3/mazebox/archetypes/_intra_inter_heterogeneity.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    17703 2022-01-19 23:19:32.000000 mazebox-0.0.3/mazebox/archetypes/_signature_scoring.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox/network/
+-rw-r--r--   0 smgroves   (501) staff       (20)       62 2021-12-03 02:05:08.000000 mazebox-0.0.3/mazebox/network/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     1895 2021-12-03 02:05:08.000000 mazebox-0.0.3/mazebox/network/generate_timepoints.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox/plasticity/
+-rw-r--r--   0 smgroves   (501) staff       (20)      215 2021-07-21 18:35:47.000000 mazebox-0.0.3/mazebox/plasticity/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    17390 2022-02-09 23:02:36.000000 mazebox-0.0.3/mazebox/plasticity/_ctrp.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     4710 2021-12-03 02:50:03.000000 mazebox-0.0.3/mazebox/plasticity/_utils.py
+-rw-r--r--   0 smgroves   (501) staff       (20)      957 2021-12-03 02:50:06.000000 mazebox-0.0.3/mazebox/plasticity/_velocity.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox/plotting/
+-rw-r--r--   0 smgroves   (501) staff       (20)      313 2022-01-10 23:48:05.000000 mazebox-0.0.3/mazebox/plotting/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    25021 2021-12-03 02:50:14.000000 mazebox-0.0.3/mazebox/plotting/_archetype_plots.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     3070 2022-01-19 23:15:40.000000 mazebox-0.0.3/mazebox/plotting/_circular_projection.py
+-rw-r--r--   0 smgroves   (501) staff       (20)       81 2020-11-26 18:25:11.000000 mazebox-0.0.3/mazebox/plotting/_network_plots.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     1918 2021-12-03 02:50:22.000000 mazebox-0.0.3/mazebox/plotting/_plasticity_plots.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     5350 2021-12-03 02:50:19.000000 mazebox-0.0.3/mazebox/plotting/_utils.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox/preprocessing/
+-rw-r--r--   0 smgroves   (501) staff       (20)      180 2021-01-04 20:09:55.000000 mazebox-0.0.3/mazebox/preprocessing/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     7564 2023-04-26 18:36:24.000000 mazebox-0.0.3/mazebox/preprocessing/_filter.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     1118 2021-12-03 02:49:18.000000 mazebox-0.0.3/mazebox/preprocessing/_imputation.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     2018 2021-12-01 16:18:38.000000 mazebox-0.0.3/mazebox/preprocessing/_integrate.py
+-rw-r--r--   0 smgroves   (501) staff       (20)      189 2021-12-03 02:50:26.000000 mazebox-0.0.3/mazebox/preprocessing/_read.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox.egg-info/
+-rw-r--r--   0 smgroves   (501) staff       (20)     1521 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox.egg-info/PKG-INFO
+-rw-r--r--   0 smgroves   (501) staff       (20)     1001 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox.egg-info/SOURCES.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)        1 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox.egg-info/dependency_links.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)      205 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox.egg-info/requires.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)        8 2023-04-27 16:54:01.000000 mazebox-0.0.3/mazebox.egg-info/top_level.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)       80 2022-10-02 02:58:36.000000 mazebox-0.0.3/pyproject.toml
+-rw-r--r--   0 smgroves   (501) staff       (20)       38 2023-04-27 16:54:01.000000 mazebox-0.0.3/setup.cfg
+-rw-r--r--   0 smgroves   (501) staff       (20)     1489 2023-04-27 16:51:38.000000 mazebox-0.0.3/setup.py
```

### Comparing `mazebox-0.0.2/LICENSE` & `mazebox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/PKG-INFO` & `mazebox-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazebox
-Version: 0.0.2
+Version: 0.0.3
 Summary: A suite of tools for analyzing single-cell transcriptomics data
 Home-page: https://github.com/smgroves/mazebox
 Author: Sarah Groves
 Author-email: sarahmaddoxgroves@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -19,27 +19,28 @@
 =======================================================
 Mazebox
 =======================================================
 .. image:: https://badge.fury.io/py/mazebox.svg
     :target: https://pypi.org/project/mazebox/
     :alt: Latest PYPi Version
 
-Mazebox is a suite of tools for analyzing single-cell transcriptomics data. 
+Mazebox is a suite of tools for analyzing single-cell transcriptomics data.
 
 
 Installation
 ~~~~~~~~~~~~~~~~~
 
 To install ``Mazebox``, please use::
 
     pip install mazebox
 
 Dependencies
 ---------------------
 
-The ``graph-tool`` python package will need to be installed. This can be installed with `Conda`, `homebrew`, etc as seen `here <https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions>`_. All other dependencies will be installed with this package.
+The ``dropkick`` python package will need to be installed, as seen `here <https://github.com/KenLauLab/dropkick>`_.
+The ``graph-tool`` python package will need to be installed. This can be installed with `Conda`, `homebrew`, etc as seen on graph-tool's `website <https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions>`_. 
+
+All other dependencies will be installed with this package.
 
-The ``dropkick`` python package will also need to be installed. 
 
 Mazebox Usage:
 ~~~~~~~~~~~~~~~~~~~~~~~~
-
```

### Comparing `mazebox-0.0.2/README.rst` & `mazebox-0.0.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 =======================================================
 Mazebox
 =======================================================
 .. image:: https://badge.fury.io/py/mazebox.svg
     :target: https://pypi.org/project/mazebox/
     :alt: Latest PYPi Version
 
-Mazebox is a suite of tools for analyzing single-cell transcriptomics data. 
+Mazebox is a suite of tools for analyzing single-cell transcriptomics data.
 
 
 Installation
 ~~~~~~~~~~~~~~~~~
 
 To install ``Mazebox``, please use::
 
     pip install mazebox
 
 Dependencies
 ---------------------
 
-The ``graph-tool`` python package will need to be installed. This can be installed with `Conda`, `homebrew`, etc as seen `here <https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions>`_. All other dependencies will be installed with this package.
+The ``dropkick`` python package will need to be installed, as seen `here <https://github.com/KenLauLab/dropkick>`_.
+The ``graph-tool`` python package will need to be installed. This can be installed with `Conda`, `homebrew`, etc as seen on graph-tool's `website <https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions>`_. 
+
+All other dependencies will be installed with this package.
 
-The ``dropkick`` python package will also need to be installed. 
 
 Mazebox Usage:
 ~~~~~~~~~~~~~~~~~~~~~~~~
-
```

### Comparing `mazebox-0.0.2/mazebox/__init__.py` & `mazebox-0.0.3/mazebox/__init__.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/_settings.py` & `mazebox-0.0.3/mazebox/_settings.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/archetypes/_bulk_signature.py` & `mazebox-0.0.3/mazebox/archetypes/_bulk_signature.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/archetypes/_cell_state_space.py` & `mazebox-0.0.3/mazebox/archetypes/_cell_state_space.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/archetypes/_intra_inter_heterogeneity.py` & `mazebox-0.0.3/mazebox/archetypes/_intra_inter_heterogeneity.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/archetypes/_signature_scoring.py` & `mazebox-0.0.3/mazebox/archetypes/_signature_scoring.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/network/generate_timepoints.py` & `mazebox-0.0.3/mazebox/network/generate_timepoints.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plasticity/_ctrp.py` & `mazebox-0.0.3/mazebox/plasticity/_ctrp.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plasticity/_utils.py` & `mazebox-0.0.3/mazebox/plasticity/_utils.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plasticity/_velocity.py` & `mazebox-0.0.3/mazebox/plasticity/_velocity.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plotting/_archetype_plots.py` & `mazebox-0.0.3/mazebox/plotting/_archetype_plots.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plotting/_circular_projection.py` & `mazebox-0.0.3/mazebox/plotting/_circular_projection.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plotting/_plasticity_plots.py` & `mazebox-0.0.3/mazebox/plotting/_plasticity_plots.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/plotting/_utils.py` & `mazebox-0.0.3/mazebox/plotting/_utils.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/preprocessing/_filter.py` & `mazebox-0.0.3/mazebox/preprocessing/_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     retain_genes=None,
     batch_categories=None,
     mito_names="^mt-|^MT-",
     n_ambient=10,
     target_sum=None,
     X_final="arcsinh_norm",
     n_comps=50,
+    scale = False
 ):
     print("Running dropkick on each sample and filtering...")
     if len(adatas) == 1:
         adata = adatas[0]
         if "dropkick_score" not in adata.obs.keys():
             adata_rc = dk.dropkick(adata, n_jobs=4, verbose=verbose)
         if plot:
@@ -115,21 +116,23 @@
     # normalize counts before transforming
     # with target_sum = None, this is equivalent to scv.pp.normalize_per_cell
     sc.pp.normalize_total(adata, target_sum=target_sum, layers=None, layer_norm=None)
     adata.layers["norm_counts"] = adata.X.copy()
 
     # arcsinh-transform normalized counts (adata.layers["arcsinh_norm"])
     adata.X = np.arcsinh(adata.layers["norm_counts"])
-    sc.pp.scale(adata)  # scale genes for feeding into model
+    if scale:
+        sc.pp.scale(adata)  # scale genes for feeding into model
     adata.layers[
         "arcsinh_norm"
     ] = adata.X.copy()  # save arcsinh scaled counts in .layers
 
     adata.X = np.log1p(adata.layers["norm_counts"])
-    sc.pp.scale(adata)  # scale genes for feeding into model
+    if scale:
+        sc.pp.scale(adata)  # scale genes for feeding into model
     adata.layers["log1p_norm"] = adata.X.copy()  # save log1p scaled counts in .layers
 
     # HVGs
     if n_hvgs is not None:
         if verbose:
             print("Determining {} highly variable genes".format(n_hvgs))
         # log1p transform for HVGs (adata.layers["log1p_norm"])
```

### Comparing `mazebox-0.0.2/mazebox/preprocessing/_imputation.py` & `mazebox-0.0.3/mazebox/preprocessing/_imputation.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox/preprocessing/_integrate.py` & `mazebox-0.0.3/mazebox/preprocessing/_integrate.py`

 * *Files identical despite different names*

### Comparing `mazebox-0.0.2/mazebox.egg-info/PKG-INFO` & `mazebox-0.0.3/mazebox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazebox
-Version: 0.0.2
+Version: 0.0.3
 Summary: A suite of tools for analyzing single-cell transcriptomics data
 Home-page: https://github.com/smgroves/mazebox
 Author: Sarah Groves
 Author-email: sarahmaddoxgroves@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -19,27 +19,28 @@
 =======================================================
 Mazebox
 =======================================================
 .. image:: https://badge.fury.io/py/mazebox.svg
     :target: https://pypi.org/project/mazebox/
     :alt: Latest PYPi Version
 
-Mazebox is a suite of tools for analyzing single-cell transcriptomics data. 
+Mazebox is a suite of tools for analyzing single-cell transcriptomics data.
 
 
 Installation
 ~~~~~~~~~~~~~~~~~
 
 To install ``Mazebox``, please use::
 
     pip install mazebox
 
 Dependencies
 ---------------------
 
-The ``graph-tool`` python package will need to be installed. This can be installed with `Conda`, `homebrew`, etc as seen `here <https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions>`_. All other dependencies will be installed with this package.
+The ``dropkick`` python package will need to be installed, as seen `here <https://github.com/KenLauLab/dropkick>`_.
+The ``graph-tool`` python package will need to be installed. This can be installed with `Conda`, `homebrew`, etc as seen on graph-tool's `website <https://git.skewed.de/count0/graph-tool/-/wikis/installation-instructions>`_. 
+
+All other dependencies will be installed with this package.
 
-The ``dropkick`` python package will also need to be installed. 
 
 Mazebox Usage:
 ~~~~~~~~~~~~~~~~~~~~~~~~
-
```

### Comparing `mazebox-0.0.2/mazebox.egg-info/SOURCES.txt` & `mazebox-0.0.3/mazebox.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 mazebox.egg-info/top_level.txt
 mazebox/archetypes/__init__.py
 mazebox/archetypes/_bulk_signature.py
 mazebox/archetypes/_cell_state_space.py
 mazebox/archetypes/_intra_inter_heterogeneity.py
 mazebox/archetypes/_signature_scoring.py
 mazebox/network/__init__.py
-mazebox/network/_build_network.py
-mazebox/network/_fit.py
-mazebox/network/_sim.py
-mazebox/network/_utils.py
 mazebox/network/generate_timepoints.py
 mazebox/plasticity/__init__.py
 mazebox/plasticity/_ctrp.py
 mazebox/plasticity/_utils.py
 mazebox/plasticity/_velocity.py
 mazebox/plotting/__init__.py
 mazebox/plotting/_archetype_plots.py
```

### Comparing `mazebox-0.0.2/setup.py` & `mazebox-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 readme = open("README.rst").read()
 
 
 setup(
     name="mazebox",
-    version="0.0.2",
+    version="0.0.3",
     description="A suite of tools for analyzing single-cell transcriptomics data",
     long_description=readme,
     long_description_content_type="text/x-rst",
     author="Sarah Groves",
     author_email="sarahmaddoxgroves@gmail.com",
     url="https://github.com/smgroves/mazebox",
     install_requires=install_requires,
```

