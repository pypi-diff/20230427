# Comparing `tmp/mask2bbox-0.0.1.tar.gz` & `tmp/mask2bbox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.1.tar", last modified: Thu Apr 27 12:53:50 2023, max compression
+gzip compressed data, was "mask2bbox-0.1.0.tar", last modified: Thu Apr 27 12:06:18 2023, max compression
```

## Comparing `mask2bbox-0.0.1.tar` & `mask2bbox-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,15 @@
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.503103 mask2bbox-0.0.1/
--rw-r--r--   0 miguelibarra   (501) staff       (20)    35149 2023-04-27 12:24:53.000000 mask2bbox-0.0.1/LICENSE.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       56 2023-04-27 12:51:38.000000 mask2bbox-0.0.1/MANIFEST.in
--rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 12:53:50.502956 mask2bbox-0.0.1/PKG-INFO
--rw-r--r--   0 miguelibarra   (501) staff       (20)      420 2023-04-27 12:31:34.000000 mask2bbox-0.0.1/README.md
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.501842 mask2bbox-0.0.1/mask2bbox.egg-info/
--rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 miguelibarra   (501) staff       (20)      389 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)        1 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       19 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       14 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/top_level.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 12:53:50.503142 mask2bbox-0.0.1/setup.cfg
--rw-r--r--   0 miguelibarra   (501) staff       (20)      832 2023-04-27 12:49:03.000000 mask2bbox-0.0.1/setup.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.501965 mask2bbox-0.0.1/src/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.1/src/__init__.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.502318 mask2bbox-0.0.1/src/mask2bbox/
--rw-r--r--   0 miguelibarra   (501) staff       (20)     2019 2023-04-27 11:50:58.000000 mask2bbox-0.0.1/src/mask2bbox/BBoxes.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.1/src/mask2bbox/__init__.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)     1808 2023-04-27 12:36:32.000000 mask2bbox-0.0.1/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.502513 mask2bbox-0.0.1/tests/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:42:54.000000 mask2bbox-0.0.1/tests/__init__.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.502755 mask2bbox-0.0.1/tests/test_mask2bbox/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:43:28.000000 mask2bbox-0.0.1/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)      120 2023-04-27 12:47:29.000000 mask2bbox-0.0.1/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:06:18.271842 mask2bbox-0.1.0/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      442 2023-04-27 12:06:18.271714 mask2bbox-0.1.0/PKG-INFO
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       96 2023-04-25 13:03:12.000000 mask2bbox-0.1.0/README.md
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:06:18.271224 mask2bbox-0.1.0/mask2bbox.egg-info/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      442 2023-04-27 12:06:18.000000 mask2bbox-0.1.0/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      225 2023-04-27 12:06:18.000000 mask2bbox-0.1.0/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        1 2023-04-27 12:06:18.000000 mask2bbox-0.1.0/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       14 2023-04-27 12:06:18.000000 mask2bbox-0.1.0/mask2bbox.egg-info/top_level.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 12:06:18.271877 mask2bbox-0.1.0/setup.cfg
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      613 2023-04-27 12:05:51.000000 mask2bbox-0.1.0/setup.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:06:18.270513 mask2bbox-0.1.0/src/
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:06:18.271559 mask2bbox-0.1.0/src/mask2bbox/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.1.0/src/mask2bbox/__init__.py
+-rw-r--r--   0 miguelibarra   (501) staff       (20)     2019 2023-04-27 11:50:58.000000 mask2bbox-0.1.0/src/mask2bbox/bbox.py
+-rw-r--r--   0 miguelibarra   (501) staff       (20)     1806 2023-04-27 09:13:57.000000 mask2bbox-0.1.0/src/mask2bbox/mask2bbox.py
```

### Comparing `mask2bbox-0.0.1/src/mask2bbox/BBoxes.py` & `mask2bbox-0.1.0/src/mask2bbox/bbox.py`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.1/src/mask2bbox/mask2bbox.py` & `mask2bbox-0.1.0/src/mask2bbox/mask2bbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Import libraries
 import time
 import argparse
-from BBoxes import BBoxes
+from bbox import BBoxes
 from pathlib import Path
 
 # Import third-party libraries
 from skimage import io, exposure, transform, restoration
 # from aicsimageio import AICSImage
 import numpy as np
 from tqdm import tqdm
```

