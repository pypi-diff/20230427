# Comparing `tmp/eeg_blinks-0.0.4.tar.gz` & `tmp/eeg_blinks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eeg_blinks-0.0.4.tar", last modified: Thu Apr 27 09:03:07 2023, max compression
+gzip compressed data, was "eeg_blinks-0.0.5.tar", last modified: Thu Apr 27 11:08:09 2023, max compression
```

## Comparing `eeg_blinks-0.0.4.tar` & `eeg_blinks-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/
--rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/PKG-INFO
--rw-r--r--   0 rpb       (1000) rpb       (1000)      540 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/README.md
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/
--rw-r--r--   0 rpb       (1000) rpb       (1000)       94 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     1196 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/default_setting.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     3252 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/pyblinker.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/utilities/
--rw-r--r--   0 rpb       (1000) rpb       (1000)       16 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)    11250 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/extractBlinkProperties.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2976 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/fit_blink.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     5828 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/getCandidateSignal.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     1526 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/misc.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)    18968 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/zero_crossing.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/vislab/
--rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)      916 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/base_left_right.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2590 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/blink_posi_vislab.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2677 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/getBlinkPositions_vislab.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/viz/
--rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/viz/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2932 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/viz/viz_pd.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     3580 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/viz/viz_sanity.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks.egg-info/
--rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/PKG-INFO
--rw-r--r--   0 rpb       (1000) rpb       (1000)      721 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/SOURCES.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)        1 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/dependency_links.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)        8 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/requires.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)       11 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/top_level.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)       38 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/setup.cfg
--rw-r--r--   0 rpb       (1000) rpb       (1000)      349 2023-04-27 09:01:59.000000 eeg_blinks-0.0.4/setup.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/PKG-INFO
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      540 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/README.md
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/eeg_blinks/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       94 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     1196 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/default_setting.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     3252 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/pyblinker.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/eeg_blinks/utilities/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       16 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/utilities/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)    11285 2023-04-27 09:39:21.000000 eeg_blinks-0.0.5/eeg_blinks/utilities/extractBlinkProperties.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2976 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/utilities/fit_blink.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     5828 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/utilities/getCandidateSignal.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     1526 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/utilities/misc.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)    18968 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/utilities/zero_crossing.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/eeg_blinks/vislab/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/vislab/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      916 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/vislab/base_left_right.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2590 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/vislab/blink_posi_vislab.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2677 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/vislab/getBlinkPositions_vislab.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/eeg_blinks/viz/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/viz/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2932 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/viz/viz_pd.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     3580 2023-04-27 08:26:37.000000 eeg_blinks-0.0.5/eeg_blinks/viz/viz_sanity.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/eeg_blinks.egg-info/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 11:08:09.000000 eeg_blinks-0.0.5/eeg_blinks.egg-info/PKG-INFO
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      721 2023-04-27 11:08:09.000000 eeg_blinks-0.0.5/eeg_blinks.egg-info/SOURCES.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        1 2023-04-27 11:08:09.000000 eeg_blinks-0.0.5/eeg_blinks.egg-info/dependency_links.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        8 2023-04-27 11:08:09.000000 eeg_blinks-0.0.5/eeg_blinks.egg-info/requires.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       11 2023-04-27 11:08:09.000000 eeg_blinks-0.0.5/eeg_blinks.egg-info/top_level.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       38 2023-04-27 11:08:09.227002 eeg_blinks-0.0.5/setup.cfg
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      349 2023-04-27 10:53:11.000000 eeg_blinks-0.0.5/setup.py
```

### Comparing `eeg_blinks-0.0.4/README.md` & `eeg_blinks-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/default_setting.py` & `eeg_blinks-0.0.5/eeg_blinks/default_setting.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/pyblinker.py` & `eeg_blinks-0.0.5/eeg_blinks/pyblinker.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/utilities/extractBlinkProperties.py` & `eeg_blinks-0.0.5/eeg_blinks/utilities/extractBlinkProperties.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 def getGoodBlinkMask(df, zThresholds):
     "used Feb 02 2023"
     ## These is the default value
     correlationThreshold_s1, correlationThreshold_s2, zScoreThreshold_s1, zScoreThreshold_s2 = zThresholds
 
     df['rightR2'] = df['rightR2'].abs()
     df_data = df[['leftR2', 'rightR2', 'maxValues']]
-
-    indicesNaN = df_data.isnull().any(1)
+    G=df_data.isnull()
+    indicesNaN = df_data.isnull().any(axis='columns')
 
     ### GET MASK OPTIMISE
 
     goodMaskTop_bool, bestMedian, bestRobustStd = get_mask_optimise(df_data, indicesNaN, correlationThreshold_s1,
                                                                     zScoreThreshold_s1)
 
     df_s2_bool, worstMedian, worstRobustStd = get_mask_optimise(df_data, indicesNaN, correlationThreshold_s2,
```

### Comparing `eeg_blinks-0.0.4/eeg_blinks/utilities/fit_blink.py` & `eeg_blinks-0.0.5/eeg_blinks/utilities/fit_blink.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/utilities/getCandidateSignal.py` & `eeg_blinks-0.0.5/eeg_blinks/utilities/getCandidateSignal.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/utilities/misc.py` & `eeg_blinks-0.0.5/eeg_blinks/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/utilities/zero_crossing.py` & `eeg_blinks-0.0.5/eeg_blinks/utilities/zero_crossing.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/vislab/base_left_right.py` & `eeg_blinks-0.0.5/eeg_blinks/vislab/base_left_right.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/vislab/blink_posi_vislab.py` & `eeg_blinks-0.0.5/eeg_blinks/vislab/blink_posi_vislab.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/vislab/getBlinkPositions_vislab.py` & `eeg_blinks-0.0.5/eeg_blinks/vislab/getBlinkPositions_vislab.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/viz/viz_pd.py` & `eeg_blinks-0.0.5/eeg_blinks/viz/viz_pd.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks/viz/viz_sanity.py` & `eeg_blinks-0.0.5/eeg_blinks/viz/viz_sanity.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.4/eeg_blinks.egg-info/SOURCES.txt` & `eeg_blinks-0.0.5/eeg_blinks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

