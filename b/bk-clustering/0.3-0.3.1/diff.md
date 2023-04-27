# Comparing `tmp/bk_clustering-0.3.tar.gz` & `tmp/bk_clustering-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk_clustering-0.3.tar", max compression
+gzip compressed data, was "bk_clustering-0.3.1.tar", max compression
```

## Comparing `bk_clustering-0.3.tar` & `bk_clustering-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-22 21:57:10.406160 bk_clustering-0.3/README.md
--rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.3/bk_clustering/__init__.py
--rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.3/bk_clustering/_hierarchy.pyx
--rw-r--r--   0        0        0     9236 2023-04-22 01:06:37.965085 bk_clustering-0.3/bk_clustering/main.py
--rw-r--r--   0        0        0     3586 2023-04-22 22:05:11.378453 bk_clustering-0.3/bk_clustering/run_batch.py
--rw-r--r--   0        0        0        1 2023-04-11 00:55:31.723142 bk_clustering-0.3/bk_clustering/utilities/__init__.py
--rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.3/bk_clustering/utilities/calculation_utilities.py
--rw-r--r--   0        0        0     5155 2023-04-11 00:55:31.879142 bk_clustering-0.3/bk_clustering/utilities/cluster_calculations.py
--rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.3/bk_clustering/utilities/density_peak.py
--rw-r--r--   0        0        0     3788 2023-04-22 01:06:37.965085 bk_clustering-0.3/bk_clustering/utilities/load_save.py
--rw-r--r--   0        0        0    17756 2023-04-22 01:06:37.965085 bk_clustering-0.3/bk_clustering/utilities/method_comparison.py
--rw-r--r--   0        0        0     8278 2023-04-13 11:16:17.707177 bk_clustering-0.3/bk_clustering/utilities/metrics.py
--rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.3/bk_clustering/utilities/plot_utilities.py
--rw-r--r--   0        0        0     2607 2023-04-15 00:03:42.881455 bk_clustering-0.3/bk_clustering/utilities/preprocessing.py
--rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.3/bk_clustering/utilities/tree_traversal.py
--rw-r--r--   0        0        0      453 2023-04-22 22:01:42.307723 bk_clustering-0.3/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bk_clustering-0.3/PKG-INFO
+-rw-r--r--   0        0        0     3589 2023-04-27 10:56:15.518241 bk_clustering-0.3.1/README.md
+-rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.3.1/bk_clustering/__init__.py
+-rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.3.1/bk_clustering/_hierarchy.pyx
+-rw-r--r--   0        0        0     9283 2023-04-25 19:13:21.122903 bk_clustering-0.3.1/bk_clustering/main.py
+-rw-r--r--   0        0        0     3776 2023-04-27 10:39:46.156891 bk_clustering-0.3.1/bk_clustering/run_batch.py
+-rw-r--r--   0        0        0        1 2023-04-24 00:00:09.354511 bk_clustering-0.3.1/bk_clustering/utilities/__init__.py
+-rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.3.1/bk_clustering/utilities/calculation_utilities.py
+-rw-r--r--   0        0        0     5155 2023-04-27 10:47:08.290038 bk_clustering-0.3.1/bk_clustering/utilities/cluster_calculations.py
+-rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.3.1/bk_clustering/utilities/density_peak.py
+-rw-r--r--   0        0        0     3843 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/load_save.py
+-rw-r--r--   0        0        0    24666 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/method_comparison.py
+-rw-r--r--   0        0        0     8278 2023-04-24 00:00:09.354511 bk_clustering-0.3.1/bk_clustering/utilities/metrics.py
+-rw-r--r--   0        0        0     4511 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/plot_utilities.py
+-rw-r--r--   0        0        0      527 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/postprocessing.py
+-rw-r--r--   0        0        0     2607 2023-04-24 00:00:09.354511 bk_clustering-0.3.1/bk_clustering/utilities/preprocessing.py
+-rw-r--r--   0        0        0    13106 2023-04-25 19:02:17.088220 bk_clustering-0.3.1/bk_clustering/utilities/tree_traversal.py
+-rw-r--r--   0        0        0      472 2023-04-27 10:59:16.883400 bk_clustering-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4161 1970-01-01 00:00:00.000000 bk_clustering-0.3.1/PKG-INFO
```

### Comparing `bk_clustering-0.3/bk_clustering/_hierarchy.pyx` & `bk_clustering-0.3.1/bk_clustering/_hierarchy.pyx`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/main.py` & `bk_clustering-0.3.1/bk_clustering/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from bk_clustering.utilities import (
     calculation_utilities,
     cluster_calculations,
     tree_traversal,
     load_save,
     plot_utilities,
+    postprocessing,
 )
 
 
 class BurjKhalifaClustering:
     def __init__(
         self,
         dH0: float = 0,
@@ -110,15 +111,15 @@
                 result_dict,
                 dtf,
                 cluster_df,
                 cluster_info,
                 node_tree,
             ) = self.calculate_clusters(X, linkage_type=self.linkage)
 
-        self.labels_ = list(result_dict.values())
+        self.labels_ = postprocessing.convert_to_array(result_dict.values())
         self.n_clusters = len(set(self.labels_))
         self.dtf_ = dtf
         self.cluster_info_ = cluster_info
         self.cluster_df_ = cluster_df
         self.node_tree_ = node_tree
 
         return self
```

### Comparing `bk_clustering-0.3/bk_clustering/run_batch.py` & `bk_clustering-0.3.1/bk_clustering/run_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utilities import load_save, metrics #method_comparison
+from utilities import load_save, metrics  # method_comparison
 import os
 from timeit import default_timer as timer
 from main import BurjKhalifaClustering
 
 SKIP_COLUMNS_IN_DATASET = {
     ("real", "wdbc"): ["idnumber"],
     ("real", "spectrometer"): ["LRS-name"],
@@ -14,14 +14,15 @@
     depth=2,
     chain_ratio=5,
     parent_split_ratio=10,
     min_leaves=0,
     n_clusters=None,
 ):
     result_dict = {}
+    pred_dict = {}
     for idx, dataset_name in enumerate(dataset_names):
         try:
             start = timer()
             skip_columns = (
                 []
                 if dataset_name not in SKIP_COLUMNS_IN_DATASET
                 else SKIP_COLUMNS_IN_DATASET[dataset_name]
@@ -38,17 +39,20 @@
             )
             bk_model.fit(X)
             predict_labels = bk_model.labels_
             error_results = metrics.calculate_metrics(true_labels, predict_labels)
             result_dict[dataset_name] = load_save.format_results(
                 error_results, timer() - start
             )
+            pred_dict[dataset_name] = load_save.encode_json(predict_labels)
         except Exception as e:
             print(e)
-
+    load_save.save_json(
+        pred_dict, "./../results/predictions/bk_clustering_predictions.json"
+    )
     return result_dict
 
 
 def run_batch():
     skip_datasets = [
         "water-treatment",  # no class
         "autos",
@@ -73,19 +77,19 @@
         ]
 
     number_of_clusters = [
         load_save.read_arff(x[0], x[1]).iloc[:, -1].nunique() for x in dataset_names
     ]
 
     # run bk_clustering
-    """
+
     results = run_multiple_datasets(dataset_names)
     filename = f"./../results/bk_clustering_results.json"  # Define the filename to save the results
     load_save.save_json(results, filename)  # Save the results to a JSON file
-    """
+
     # method_comparison.run_birch(dataset_names, number_of_clusters)
     # method_comparison.run_dbscan(dataset_names, number_of_clusters)
     # method_comparison.run_kmeans(dataset_names, number_of_clusters)
     # method_comparison.run_kmeans_mini_batch(dataset_names, number_of_clusters)
     # method_comparison.run_mean_shift(dataset_names, number_of_clusters)
     # method_comparison.run_agglomerative(dataset_names, number_of_clusters)
     # method_comparison.run_gmm(dataset_names, number_of_clusters)
```

### Comparing `bk_clustering-0.3/bk_clustering/utilities/calculation_utilities.py` & `bk_clustering-0.3.1/bk_clustering/utilities/calculation_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/utilities/cluster_calculations.py` & `bk_clustering-0.3.1/bk_clustering/utilities/cluster_calculations.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/utilities/density_peak.py` & `bk_clustering-0.3.1/bk_clustering/utilities/density_peak.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/utilities/load_save.py` & `bk_clustering-0.3.1/bk_clustering/utilities/load_save.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,18 @@
     Returns:
         None
     """
     with open(filename, "w") as outfile:
         ujson.dump(data, outfile)  # Use ujson.dump to write data to the JSON file
 
 
+def encode_json(data):
+    return ujson.encode(data)
+
+
 def load_json(filename):
     with open(filename) as outfile:
         data = ujson.load(outfile)
         return data
 
 
 def format_results(results: dict, time: float) -> dict:
```

### Comparing `bk_clustering-0.3/bk_clustering/utilities/metrics.py` & `bk_clustering-0.3.1/bk_clustering/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/utilities/plot_utilities.py` & `bk_clustering-0.3.1/bk_clustering/utilities/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/utilities/preprocessing.py` & `bk_clustering-0.3.1/bk_clustering/utilities/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3/bk_clustering/utilities/tree_traversal.py` & `bk_clustering-0.3.1/bk_clustering/utilities/tree_traversal.py`

 * *Files identical despite different names*

