# Comparing `tmp/eeg_blinks-0.0.3.tar.gz` & `tmp/eeg_blinks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eeg_blinks-0.0.3.tar", last modified: Thu Apr 27 08:53:08 2023, max compression
+gzip compressed data, was "eeg_blinks-0.0.4.tar", last modified: Thu Apr 27 09:03:07 2023, max compression
```

## Comparing `eeg_blinks-0.0.3.tar` & `eeg_blinks-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/
--rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/PKG-INFO
--rw-r--r--   0 rpb       (1000) rpb       (1000)      540 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/README.md
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/
--rw-r--r--   0 rpb       (1000) rpb       (1000)       94 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)      125 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/_version.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     1196 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/default_setting.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     3252 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/pyblinker.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/utilities/
--rw-r--r--   0 rpb       (1000) rpb       (1000)       16 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)    11250 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/extractBlinkProperties.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2976 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/fit_blink.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     5828 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/getCandidateSignal.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     1526 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/misc.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)    18968 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/utilities/zero_crossing.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/vislab/
--rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)      916 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/base_left_right.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2590 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/blink_posi_vislab.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2677 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/vislab/getBlinkPositions_vislab.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks/viz/
--rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/viz/__init__.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     2932 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/viz/viz_pd.py
--rw-r--r--   0 rpb       (1000) rpb       (1000)     3580 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/eeg_blinks/viz/viz_sanity.py
-drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/eeg_blinks.egg-info/
--rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/PKG-INFO
--rw-r--r--   0 rpb       (1000) rpb       (1000)      744 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/SOURCES.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)        1 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/dependency_links.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)        8 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/requires.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)       11 2023-04-27 08:53:08.000000 eeg_blinks-0.0.3/eeg_blinks.egg-info/top_level.txt
--rw-r--r--   0 rpb       (1000) rpb       (1000)       38 2023-04-27 08:53:08.890377 eeg_blinks-0.0.3/setup.cfg
--rw-r--r--   0 rpb       (1000) rpb       (1000)      349 2023-04-27 08:26:37.000000 eeg_blinks-0.0.3/setup.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/PKG-INFO
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      540 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/README.md
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       94 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     1196 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/default_setting.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     3252 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/pyblinker.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/utilities/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       16 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)    11250 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/extractBlinkProperties.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2976 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/fit_blink.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     5828 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/getCandidateSignal.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     1526 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/misc.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)    18968 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/utilities/zero_crossing.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/vislab/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      916 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/base_left_right.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2590 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/blink_posi_vislab.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2677 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/vislab/getBlinkPositions_vislab.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks/viz/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        0 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/viz/__init__.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     2932 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/viz/viz_pd.py
+-rw-r--r--   0 rpb       (1000) rpb       (1000)     3580 2023-04-27 08:26:37.000000 eeg_blinks-0.0.4/eeg_blinks/viz/viz_sanity.py
+drwxr-xr-x   0 rpb       (1000) rpb       (1000)        0 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/eeg_blinks.egg-info/
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      127 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/PKG-INFO
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      721 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/SOURCES.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        1 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/dependency_links.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)        8 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/requires.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       11 2023-04-27 09:03:07.000000 eeg_blinks-0.0.4/eeg_blinks.egg-info/top_level.txt
+-rw-r--r--   0 rpb       (1000) rpb       (1000)       38 2023-04-27 09:03:07.580128 eeg_blinks-0.0.4/setup.cfg
+-rw-r--r--   0 rpb       (1000) rpb       (1000)      349 2023-04-27 09:01:59.000000 eeg_blinks-0.0.4/setup.py
```

### Comparing `eeg_blinks-0.0.3/README.md` & `eeg_blinks-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/default_setting.py` & `eeg_blinks-0.0.4/eeg_blinks/default_setting.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/pyblinker.py` & `eeg_blinks-0.0.4/eeg_blinks/pyblinker.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/utilities/extractBlinkProperties.py` & `eeg_blinks-0.0.4/eeg_blinks/utilities/extractBlinkProperties.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/utilities/fit_blink.py` & `eeg_blinks-0.0.4/eeg_blinks/utilities/fit_blink.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/utilities/getCandidateSignal.py` & `eeg_blinks-0.0.4/eeg_blinks/utilities/getCandidateSignal.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/utilities/misc.py` & `eeg_blinks-0.0.4/eeg_blinks/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/utilities/zero_crossing.py` & `eeg_blinks-0.0.4/eeg_blinks/utilities/zero_crossing.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/vislab/base_left_right.py` & `eeg_blinks-0.0.4/eeg_blinks/vislab/base_left_right.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/vislab/blink_posi_vislab.py` & `eeg_blinks-0.0.4/eeg_blinks/vislab/blink_posi_vislab.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/vislab/getBlinkPositions_vislab.py` & `eeg_blinks-0.0.4/eeg_blinks/vislab/getBlinkPositions_vislab.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/viz/viz_pd.py` & `eeg_blinks-0.0.4/eeg_blinks/viz/viz_pd.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks/viz/viz_sanity.py` & `eeg_blinks-0.0.4/eeg_blinks/viz/viz_sanity.py`

 * *Files identical despite different names*

### Comparing `eeg_blinks-0.0.3/eeg_blinks.egg-info/SOURCES.txt` & `eeg_blinks-0.0.4/eeg_blinks.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.py
 eeg_blinks/__init__.py
-eeg_blinks/_version.py
 eeg_blinks/default_setting.py
 eeg_blinks/pyblinker.py
 eeg_blinks.egg-info/PKG-INFO
 eeg_blinks.egg-info/SOURCES.txt
 eeg_blinks.egg-info/dependency_links.txt
 eeg_blinks.egg-info/requires.txt
 eeg_blinks.egg-info/top_level.txt
```

