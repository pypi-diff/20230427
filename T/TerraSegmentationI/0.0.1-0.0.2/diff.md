# Comparing `tmp/TerraSegmentationI-0.0.1.tar.gz` & `tmp/TerraSegmentationI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.5\TerraSegmentation-0.0.5\dist\.tmp-7kops9h4\TerraSegmentationI-0.0.1.tar", last modified: Mon Apr 17 12:40:47 2023, max compression
+gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentationI-0.0.1\TerraSegmentationI-0.0.1\dist\.tmp-23enlph9\TerraSegmentationI-0.0.2.tar", last modified: Thu Apr 27 07:23:11 2023, max compression
```

## Comparing `TerraSegmentationI-0.0.1.tar` & `TerraSegmentationI-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/
--rw-rw-rw-   0        0        0      135 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/TerraSegmentationI/
--rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentationI-0.0.1/TerraSegmentationI/TerraMaskrcnnDemo.py
--rw-rw-rw-   0        0        0    51902 2023-04-17 12:38:41.000000 TerraSegmentationI-0.0.1/TerraSegmentationI/TerraSegmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/TerraSegmentationI.egg-info/
--rw-rw-rw-   0        0        0      135 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/TerraSegmentationI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/TerraSegmentationI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/TerraSegmentationI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/TerraSegmentationI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 12:40:47.000000 TerraSegmentationI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-04-17 12:38:54.000000 TerraSegmentationI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/
+-rw-rw-rw-   0        0        0      135 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/TerraSegmentationI/
+-rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentationI-0.0.2/TerraSegmentationI/TerraMaskrcnnDemo.py
+-rw-rw-rw-   0        0        0    51905 2023-04-27 07:21:23.000000 TerraSegmentationI-0.0.2/TerraSegmentationI/TerraSegmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/TerraSegmentationI.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/TerraSegmentationI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/TerraSegmentationI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/TerraSegmentationI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/TerraSegmentationI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:23:11.000000 TerraSegmentationI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-04-27 07:21:40.000000 TerraSegmentationI-0.0.2/setup.py
```

### Comparing `TerraSegmentationI-0.0.1/TerraSegmentationI/TerraMaskrcnnDemo.py` & `TerraSegmentationI-0.0.2/TerraSegmentationI/TerraMaskrcnnDemo.py`

 * *Files identical despite different names*

### Comparing `TerraSegmentationI-0.0.1/TerraSegmentationI/TerraSegmentation.py` & `TerraSegmentationI-0.0.2/TerraSegmentationI/TerraSegmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
   
   return config
 
 
 def train_model(
   model,
   img_seg_dataset,
-  batch_size,
+  batch_size=64,
   epochs,
   class_list
 ):
   result = train_eval_modelUnet(
     *model, 
     img_seg_dataset.X["train"]["input_1"], 
     img_seg_dataset.Y["train"]["output_1"],
```

