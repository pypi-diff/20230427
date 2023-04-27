# Comparing `tmp/palmari-0.2.7.tar.gz` & `tmp/palmari-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palmari-0.2.7.tar", last modified: Mon Oct 24 09:16:53 2022, max compression
+gzip compressed data, was "palmari-0.2.8.tar", last modified: Mon Oct 24 11:26:17 2022, max compression
```

## Comparing `palmari-0.2.7.tar` & `palmari-0.2.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.425038 palmari-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-24 09:16:31.000000 palmari-0.2.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21780 2022-10-24 09:16:31.000000 palmari-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-24 09:16:31.000000 palmari-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-24 09:16:53.425038 palmari-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-10-24 09:16:31.000000 palmari-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-10-24 09:16:31.000000 palmari-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-24 09:16:53.425038 palmari-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.421038 palmari-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.421038 palmari-0.2.7/src/palmari/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8431 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.421038 palmari-0.2.7/src/palmari/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.421038 palmari-0.2.7/src/palmari/data_structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/data_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21364 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/data_structure/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (121)    16307 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/data_structure/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.421038 palmari-0.2.7/src/palmari/processing/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8279 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/edit_pipeline_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.425038 palmari-0.2.7/src/palmari/processing/steps/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/drift_corrector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/quot_localizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6339 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/quot_tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/trackpy_tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/steps/window_percentile.py
--rw-r--r--   0 runner    (1001) docker     (121)    14976 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/tif_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    22481 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/tif_pipeline_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/processing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.425038 palmari-0.2.7/src/palmari/quot/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15820 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/chunkFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8583 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    23222 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/findSpots.py
--rw-r--r--   0 runner    (1001) docker     (121)    47710 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13888 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/measureGain.py
--rw-r--r--   0 runner    (1001) docker     (121)    38259 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    11057 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/read.py
--rw-r--r--   0 runner    (1001) docker     (121)    14554 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/subpixel.py
--rw-r--r--   0 runner    (1001) docker     (121)    32110 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/track.py
--rw-r--r--   0 runner    (1001) docker     (121)    10373 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/quot/trajUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.425038 palmari-0.2.7/src/palmari/tif_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/tif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/tif_tools/cell_mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3967 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/tif_tools/correct_drift.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/tif_tools/density_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/tif_tools/intensity.py
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-10-24 09:16:31.000000 palmari-0.2.7/src/palmari/tif_tools/localization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 09:16:53.421038 palmari-0.2.7/src/palmari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-24 09:16:53.000000 palmari-0.2.7/src/palmari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-10-24 09:16:53.000000 palmari-0.2.7/src/palmari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 09:16:53.000000 palmari-0.2.7/src/palmari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-24 09:16:53.000000 palmari-0.2.7/src/palmari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-24 09:16:53.000000 palmari-0.2.7/src/palmari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-24 09:16:53.000000 palmari-0.2.7/src/palmari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.600133 palmari-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-24 11:25:58.000000 palmari-0.2.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21780 2022-10-24 11:25:58.000000 palmari-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-24 11:25:58.000000 palmari-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-24 11:26:17.600133 palmari-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-10-24 11:25:58.000000 palmari-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-10-24 11:25:58.000000 palmari-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-10-24 11:26:17.600133 palmari-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/palmari/
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8431 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/palmari/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.596133 palmari-0.2.8/src/palmari/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21364 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/data_structure/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16307 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/data_structure/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.596133 palmari-0.2.8/src/palmari/processing/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8279 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/edit_pipeline_window.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.596133 palmari-0.2.8/src/palmari/processing/steps/
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/drift_corrector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/quot_localizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6339 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/quot_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/trackpy_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/steps/window_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14976 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/tif_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22519 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/tif_pipeline_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/processing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.600133 palmari-0.2.8/src/palmari/quot/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15820 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/chunkFilter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8583 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23222 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/findSpots.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47710 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13888 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/mask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/measureGain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38259 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11057 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/read.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14554 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/subpixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32243 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/track.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10373 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/quot/trajUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.600133 palmari-0.2.8/src/palmari/tif_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/cell_mask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3967 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/correct_drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/density_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-10-24 11:25:58.000000 palmari-0.2.8/src/palmari/tif_tools/localization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:26:17.592133 palmari-0.2.8/src/palmari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-24 11:26:17.000000 palmari-0.2.8/src/palmari.egg-info/top_level.txt
```

### Comparing `palmari-0.2.7/LICENSE` & `palmari-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/PKG-INFO` & `palmari-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmari
-Version: 0.2.7
+Version: 0.2.8
 Summary: A pipeline for PALM movies analysis (pre-processing, localization, drifft correction, tracking)
 Home-page: https://github.com/hippover/palmari
 Author: Hippolyte Verdier
 Author-email: hverdier@pasteur.fr
 License: "CeCILL"
 Project-URL: Bug Tracker, https://github.com/hippover/palmari/issues
 Project-URL: Documentation, https://palmari.readthedocs.io/en/latest/
```

### Comparing `palmari-0.2.7/README.md` & `palmari-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/setup.cfg` & `palmari-0.2.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = palmari
-version = 0.2.7
+version = 0.2.8
 author = Hippolyte Verdier
 author_email = hverdier@pasteur.fr
 url = https://github.com/hippover/palmari
 license = "CeCILL"
 description = A pipeline for PALM movies analysis (pre-processing, localization, drifft correction, tracking)
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `palmari-0.2.7/src/palmari/_runner.py` & `palmari-0.2.8/src/palmari/_runner.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/_tests/test_widget.py` & `palmari-0.2.8/src/palmari/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/_widget.py` & `palmari-0.2.8/src/palmari/_widget.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/data_structure/acquisition.py` & `palmari-0.2.8/src/palmari/data_structure/acquisition.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/data_structure/experiment.py` & `palmari-0.2.8/src/palmari/data_structure/experiment.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/edit_pipeline_window.py` & `palmari-0.2.8/src/palmari/processing/edit_pipeline_window.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/steps/base.py` & `palmari-0.2.8/src/palmari/processing/steps/base.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/steps/drift_corrector.py` & `palmari-0.2.8/src/palmari/processing/steps/drift_corrector.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/steps/quot_localizer.py` & `palmari-0.2.8/src/palmari/processing/steps/quot_localizer.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/steps/quot_tracker.py` & `palmari-0.2.8/src/palmari/processing/steps/quot_tracker.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/steps/trackpy_tracker.py` & `palmari-0.2.8/src/palmari/processing/steps/trackpy_tracker.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/steps/window_percentile.py` & `palmari-0.2.8/src/palmari/processing/steps/window_percentile.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/tif_pipeline.py` & `palmari-0.2.8/src/palmari/processing/tif_pipeline.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/processing/tif_pipeline_widget.py` & `palmari-0.2.8/src/palmari/processing/tif_pipeline_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,27 +235,27 @@
         delta_t_widget = FloatSpinBox(
             name="delta_t",
             label="delta t (s)",
             value=self.delta_t,
             step=0.005,
         )
 
-        def set_delta_t(x):
+        def set_delta_t(x: float):
             self.delta_t = x
 
         delta_t_widget.changed.connect(set_delta_t)
 
         pixel_size_widget = FloatSpinBox(
             name="pixel_size",
             label="pixel size (um)",
             value=self.pixel_size,
             step=0.001,
         )
 
-        def set_pixel_size(x):
+        def set_pixel_size(x: float):
             self.pixel_size = x
             self.rescale_image_layers()
 
         pixel_size_widget.changed.connect(set_pixel_size)
 
         container = Container(
             widgets=[input_widget, delta_t_widget, pixel_size_widget]
@@ -501,32 +501,32 @@
                 input_data = (self._layers[input_layer_idx].data,)
             elif input_type == handled_types.points:
                 input_data = (self._layers[input_layer_idx].result,)
             elif input_type == handled_types.tracks:
                 input_data = (self._layers[input_layer_idx].result,)
             elif input_type == handled_types.detections:
                 detections = pd.DataFrame(
-                    data=self._layers[input_layer_idx].data,
+                    data=self._layers[input_layer_idx].data.copy(),
                     columns=["frame", "x", "y"],
                 )
                 detections[["x", "y"]] /= self.pixel_size
                 # On inverse x et y volontairement
                 detections[["y", "x"]] = detections[["x", "y"]].astype(int)
                 input_data = (
                     self._layers[input_layer_idx - 1].data,
                     detections,
                 )
             elif input_type == handled_types.image_locs_and_pixel_size:
-                detections = pd.DataFrame(
-                    data=self._layers[input_layer_idx].data,
-                    columns=["frame", "x", "y"],
-                )
-                detections[["x", "y"]] /= self.pixel_size
+                # detections = pd.DataFrame(
+                #    data=self._layers[input_layer_idx].data.copy(),
+                #    columns=["frame", "x", "y"],
+                # )
+                # detections[["x", "y"]] /= self.pixel_size
                 # On inverse x et y volontairement
-                detections[["y", "x"]] = detections[["x", "y"]].astype(int)
+                # detections[["y", "x"]] = detections[["x", "y"]].astype(int)
                 input_data = (
                     self._layers[0].data,
                     self._layers[input_layer_idx].result,
                     self.pixel_size,
                 )
             return step.process(*input_data)
```

### Comparing `palmari-0.2.7/src/palmari/processing/utils.py` & `palmari-0.2.8/src/palmari/processing/utils.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/__init__.py` & `palmari-0.2.8/src/palmari/quot/__init__.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/__main__.py` & `palmari-0.2.8/src/palmari/quot/__main__.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/chunkFilter.py` & `palmari-0.2.8/src/palmari/quot/chunkFilter.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/core.py` & `palmari-0.2.8/src/palmari/quot/core.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/findSpots.py` & `palmari-0.2.8/src/palmari/quot/findSpots.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/helper.py` & `palmari-0.2.8/src/palmari/quot/helper.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/mask.py` & `palmari-0.2.8/src/palmari/quot/mask.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/measureGain.py` & `palmari-0.2.8/src/palmari/quot/measureGain.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/plot.py` & `palmari-0.2.8/src/palmari/quot/plot.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/read.py` & `palmari-0.2.8/src/palmari/quot/read.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/subpixel.py` & `palmari-0.2.8/src/palmari/quot/subpixel.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/quot/track.py` & `palmari-0.2.8/src/palmari/quot/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .helper import connected_components
 
 # Deep copy
 from copy import copy
 
 # Filter on the number of spots per frame
 from .trajUtils import filter_on_spots_per_frame
+from tqdm import tqdm
 
 ##################################
 ## LOW-LEVEL TRACKING UTILITIES ##
 ##################################
 
 
 class ScipyMunkres:
@@ -307,18 +308,19 @@
                     ((pos[1:, :] - pos[:-1, :]) ** 2).sum(1) / delta_frames
                 ).mean()
                 * (1 + trajs[ti].n_blinks)
             )
 
         # Log-likelihood of diffusing from last
         # known position to each new position
-        L_diff = np.log(
-            y_diff * (R / local_var2) * np.exp(-R2 / (2 * local_var2))
-            + (1 - y_diff) * (R / max_var2) * np.exp(-R2 / (2 * max_var2))
-        )
+        diff = y_diff * (R / local_var2) * np.exp(-R2 / (2 * local_var2)) + (
+            1 - y_diff
+        ) * (R / max_var2) * np.exp(-R2 / (2 * max_var2))
+        L_diff = np.log(diff)
+        L_diff[diff <= 0] = -np.inf
 
         # Make sure we do NOT reconnect trajectories to localizations
         # outside of their search radii
         L_diff[R > search_radius_pxl] = -np.inf
 
         # Assign reconnection weight
         W[ti, :n_locs] = -(L_blink + L_diff)
@@ -790,15 +792,18 @@
     # "active" Trajectories are eligible for reconnection in
     # this frame, "new" Trajectories will become active
     # Trajectories in the next frame, and "completed" Trajectories
     # have been removed from the pool.
     new = []
     completed = []
 
-    for fi in range(start_frame + 1, stop_frame):
+    for fi in tqdm(
+        range(start_frame + 1, stop_frame),
+        total=stop_frame - (start_frame + 1),
+    ):
 
         # # DEBUG
         # print("FRAME:\t%d" % fi)
         # print("Duplicates in active:\t", is_duplicates(active))
         # print("Duplicates in new:\t", is_duplicates(new))
         # print("Duplicates in completed:\t", is_duplicates(completed))
         # print("Completed trajectories:")
```

### Comparing `palmari-0.2.7/src/palmari/quot/trajUtils.py` & `palmari-0.2.8/src/palmari/quot/trajUtils.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/tif_tools/cell_mask.py` & `palmari-0.2.8/src/palmari/tif_tools/cell_mask.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/tif_tools/correct_drift.py` & `palmari-0.2.8/src/palmari/tif_tools/correct_drift.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/tif_tools/density_filtering.py` & `palmari-0.2.8/src/palmari/tif_tools/density_filtering.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/tif_tools/intensity.py` & `palmari-0.2.8/src/palmari/tif_tools/intensity.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari/tif_tools/localization.py` & `palmari-0.2.8/src/palmari/tif_tools/localization.py`

 * *Files identical despite different names*

### Comparing `palmari-0.2.7/src/palmari.egg-info/PKG-INFO` & `palmari-0.2.8/src/palmari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmari
-Version: 0.2.7
+Version: 0.2.8
 Summary: A pipeline for PALM movies analysis (pre-processing, localization, drifft correction, tracking)
 Home-page: https://github.com/hippover/palmari
 Author: Hippolyte Verdier
 Author-email: hverdier@pasteur.fr
 License: "CeCILL"
 Project-URL: Bug Tracker, https://github.com/hippover/palmari/issues
 Project-URL: Documentation, https://palmari.readthedocs.io/en/latest/
```

### Comparing `palmari-0.2.7/src/palmari.egg-info/SOURCES.txt` & `palmari-0.2.8/src/palmari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

