# Comparing `tmp/sar_handler-0.1.4.tar.gz` & `tmp/sar_handler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sar_handler-0.1.4.tar", last modified: Thu Apr 27 11:08:27 2023, max compression
+gzip compressed data, was "sar_handler-0.1.5.tar", last modified: Thu Apr 27 12:23:43 2023, max compression
```

## Comparing `sar_handler-0.1.4.tar` & `sar_handler-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:08:27.034872 sar_handler-0.1.4/
--rw-rw-rw-   0        0        0      488 2023-04-27 11:08:27.034872 sar_handler-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-27 10:58:50.000000 sar_handler-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 11:08:27.016872 sar_handler-0.1.4/sar_handler/
--rw-rw-rw-   0        0        0     9353 2023-03-07 18:48:04.000000 sar_handler-0.1.4/sar_handler/FC_Classifier.py
--rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.4/sar_handler/__init__.py
--rw-rw-rw-   0        0        0     4268 2023-04-27 09:32:47.000000 sar_handler-0.1.4/sar_handler/assistive_funcs.py
--rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.4/sar_handler/check_validity_of_values.py
--rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.4/sar_handler/csv_dataloader.py
--rw-rw-rw-   0        0        0     9321 2023-03-01 09:31:44.000000 sar_handler-0.1.4/sar_handler/dataset_creator.py
--rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.4/sar_handler/fastaniso.py
--rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.4/sar_handler/image_processing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:08:27.032871 sar_handler-0.1.4/sar_handler.egg-info/
--rw-rw-rw-   0        0        0      488 2023-04-27 11:08:26.000000 sar_handler-0.1.4/sar_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-27 11:08:26.000000 sar_handler-0.1.4/sar_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:08:26.000000 sar_handler-0.1.4/sar_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-27 11:08:26.000000 sar_handler-0.1.4/sar_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 11:08:26.000000 sar_handler-0.1.4/sar_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 11:08:27.034872 sar_handler-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-27 11:07:53.000000 sar_handler-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:23:43.468683 sar_handler-0.1.5/
+-rw-rw-rw-   0        0        0     1057 2023-04-27 11:30:14.000000 sar_handler-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      511 2023-04-27 12:23:43.467682 sar_handler-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-27 10:58:50.000000 sar_handler-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 12:23:43.455681 sar_handler-0.1.5/sar_handler/
+-rw-rw-rw-   0        0        0     9353 2023-03-07 18:48:04.000000 sar_handler-0.1.5/sar_handler/FC_Classifier.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.5/sar_handler/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-04-27 12:20:24.000000 sar_handler-0.1.5/sar_handler/assistive_funcs.py
+-rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.5/sar_handler/check_validity_of_values.py
+-rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.5/sar_handler/csv_dataloader.py
+-rw-rw-rw-   0        0        0     9324 2023-04-27 12:20:58.000000 sar_handler-0.1.5/sar_handler/dataset_creator.py
+-rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.5/sar_handler/fastaniso.py
+-rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.5/sar_handler/image_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:23:43.466682 sar_handler-0.1.5/sar_handler.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 12:23:43.469682 sar_handler-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-27 12:22:30.000000 sar_handler-0.1.5/setup.py
```

### Comparing `sar_handler-0.1.4/sar_handler/FC_Classifier.py` & `sar_handler-0.1.5/sar_handler/FC_Classifier.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.4/sar_handler/assistive_funcs.py` & `sar_handler-0.1.5/sar_handler/assistive_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from time import time
 from os import listdir
 from PIL import Image, ImageOps
 import numpy as np
-from torch import Tensor, no_grad
 import pathlib
+from torch import Tensor, no_grad
 from tqdm import tqdm
-from image_processing import add_borders
 from skimage.metrics import structural_similarity as ssim
 from scipy import signal
+from .image_processing import add_borders
 
 
 def delta_time():
     start = time()
 
     def wrapper() -> float:
         return time() - start
```

### Comparing `sar_handler-0.1.4/sar_handler/check_validity_of_values.py` & `sar_handler-0.1.5/sar_handler/check_validity_of_values.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.4/sar_handler/csv_dataloader.py` & `sar_handler-0.1.5/sar_handler/csv_dataloader.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.4/sar_handler/dataset_creator.py` & `sar_handler-0.1.5/sar_handler/dataset_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import csv
 from random import randint
 from os import listdir
 from PIL import ImageOps, Image
-from image_processing import *
-from check_validity_of_values import *
-from assistive_funcs import *
+from .image_processing import *
+from .check_validity_of_values import *
+from .assistive_funcs import *
 
 
 def generate_csv(*, win_size, dump_to_file=1000, step=1,
                  img_path=r"..\data\images",
                  datasets_path=r"..\data\csv_files",
                  noise_imgs_path=r"..\data\FC_imgs_with_noise",
                  dataset_name=None,
```

### Comparing `sar_handler-0.1.4/sar_handler/fastaniso.py` & `sar_handler-0.1.5/sar_handler/fastaniso.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.4/sar_handler/image_processing.py` & `sar_handler-0.1.5/sar_handler/image_processing.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.4/setup.py` & `sar_handler-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='sar_handler',
     packages=find_packages(include=['sar_handler']),
-    version='0.1.4',
+    version='0.1.5',
     description='Handler SAR images',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Felecort',
     # author_email="@gmail.com",
     url="https://github.com/Felecort/SAR_Handler",
     license='MIT',
```

