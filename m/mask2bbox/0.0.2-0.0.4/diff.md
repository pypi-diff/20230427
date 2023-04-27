# Comparing `tmp/mask2bbox-0.0.2.tar.gz` & `tmp/mask2bbox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.2.tar", last modified: Thu Apr 27 13:36:32 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.4.tar", last modified: Thu Apr 27 21:20:05 2023, max compression
```

## Comparing `mask2bbox-0.0.2.tar` & `mask2bbox-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.676257 mask2bbox-0.0.2/
--rw-r--r--   0 miguelibarra   (501) staff       (20)    35149 2023-04-27 12:24:53.000000 mask2bbox-0.0.2/LICENSE.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       56 2023-04-27 12:51:38.000000 mask2bbox-0.0.2/MANIFEST.in
--rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 13:36:32.676117 mask2bbox-0.0.2/PKG-INFO
--rw-r--r--   0 miguelibarra   (501) staff       (20)      420 2023-04-27 12:31:34.000000 mask2bbox-0.0.2/README.md
--rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 13:36:32.676296 mask2bbox-0.0.2/setup.cfg
--rw-r--r--   0 miguelibarra   (501) staff       (20)      818 2023-04-27 13:30:33.000000 mask2bbox-0.0.2/setup.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.674542 mask2bbox-0.0.2/src/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.2/src/__init__.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.674850 mask2bbox-0.0.2/src/mask2bbox/
--rw-r--r--   0 miguelibarra   (501) staff       (20)     2019 2023-04-27 11:50:58.000000 mask2bbox-0.0.2/src/mask2bbox/BBoxes.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.2/src/mask2bbox/__init__.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)     1808 2023-04-27 12:36:32.000000 mask2bbox-0.0.2/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.675587 mask2bbox-0.0.2/src/mask2bbox.egg-info/
--rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 miguelibarra   (501) staff       (20)      409 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)        1 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       19 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/top_level.txt
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.675730 mask2bbox-0.0.2/tests/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:42:54.000000 mask2bbox-0.0.2/tests/__init__.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.675940 mask2bbox-0.0.2/tests/test_mask2bbox/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:43:28.000000 mask2bbox-0.0.2/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)      127 2023-04-27 13:29:49.000000 mask2bbox-0.0.2/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.273513 mask2bbox-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/src/mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/src/mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/src/mask2bbox/_bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/src/mask2bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/tests/test_mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.2/LICENSE.txt` & `mask2bbox-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.2/setup.py` & `mask2bbox-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.2",
+    version="0.0.4",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `mask2bbox-0.0.2/src/mask2bbox/mask2bbox.py` & `mask2bbox-0.0.4/src/mask2bbox/mask2bbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Import libraries
 import time
 import argparse
-from BBoxes import BBoxes
+from _bboxes import BBoxes
 from pathlib import Path
 
 # Import third-party libraries
 from skimage import io, exposure, transform, restoration
 # from aicsimageio import AICSImage
 import numpy as np
 from tqdm import tqdm
@@ -36,29 +36,36 @@
     args.mask = Path(args.mask).resolve()
     args.output = Path(args.output).resolve()
 
     # Return arguments
     return args
 
 
-# Main
+
 def main(args):
     # Create a BBoxes object and get the bounding boxes
     all_BBoxes = BBoxes(args.mask)
-    print(all_BBoxes.bboxes)
 
+    # Expand the bounding boxes
     all_BBoxes.expand(n=10)
+
+    # Remove the bounding boxes that are on the edge of the image
+    all_BBoxes.remove_edge_boxes()
+
+    # Get the average area of the bounding boxes
     print(all_BBoxes.bboxes)
+    print(all_BBoxes.get_bbox_dims())
+    print(all_BBoxes.get_bbox_areas())
+    print(all_BBoxes.get_bbox_centers())
+    print(all_BBoxes.get_bbox_ratios())
 
     # Save file
     all_BBoxes.save_csv(args.output)
 
 
-
-
 # Run main
 if __name__ == "__main__":
     # Get arguments
     args = get_arguments()
 
     # Run main and time it
     st = time.time()
```

