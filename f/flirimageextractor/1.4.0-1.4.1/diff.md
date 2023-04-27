# Comparing `tmp/flirimageextractor-1.4.0.tar.gz` & `tmp/flirimageextractor-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flirimageextractor-1.4.0.tar", last modified: Tue Mar 17 02:49:30 2020, max compression
+gzip compressed data, was "flirimageextractor-1.4.1.tar", max compression
```

## Comparing `flirimageextractor-1.4.0.tar` & `flirimageextractor-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 aidankinzett   (501) staff       (20)        0 2020-03-17 02:49:30.000000 flirimageextractor-1.4.0/
--rw-r--r--   0 aidankinzett   (501) staff       (20)     5204 2020-03-17 02:49:30.000000 flirimageextractor-1.4.0/PKG-INFO
--rw-r--r--   0 aidankinzett   (501) staff       (20)     4111 2020-03-17 02:46:15.000000 flirimageextractor-1.4.0/README.md
-drwxr-xr-x   0 aidankinzett   (501) staff       (20)        0 2020-03-17 02:49:30.000000 flirimageextractor-1.4.0/flirimageextractor/
--rw-r--r--   0 aidankinzett   (501) staff       (20)       98 2019-11-21 07:16:08.000000 flirimageextractor-1.4.0/flirimageextractor/__init__.py
--rw-r--r--   0 aidankinzett   (501) staff       (20)    15674 2020-03-17 02:46:09.000000 flirimageextractor-1.4.0/flirimageextractor/flirimageextractor.py
-drwxr-xr-x   0 aidankinzett   (501) staff       (20)        0 2020-03-17 02:49:30.000000 flirimageextractor-1.4.0/flirimageextractor.egg-info/
--rw-r--r--   0 aidankinzett   (501) staff       (20)     5204 2020-03-17 02:49:29.000000 flirimageextractor-1.4.0/flirimageextractor.egg-info/PKG-INFO
--rw-r--r--   0 aidankinzett   (501) staff       (20)      299 2020-03-17 02:49:29.000000 flirimageextractor-1.4.0/flirimageextractor.egg-info/SOURCES.txt
--rw-r--r--   0 aidankinzett   (501) staff       (20)        1 2020-03-17 02:49:29.000000 flirimageextractor-1.4.0/flirimageextractor.egg-info/dependency_links.txt
--rw-r--r--   0 aidankinzett   (501) staff       (20)       24 2020-03-17 02:49:29.000000 flirimageextractor-1.4.0/flirimageextractor.egg-info/requires.txt
--rw-r--r--   0 aidankinzett   (501) staff       (20)       19 2020-03-17 02:49:29.000000 flirimageextractor-1.4.0/flirimageextractor.egg-info/top_level.txt
--rw-r--r--   0 aidankinzett   (501) staff       (20)       38 2020-03-17 02:49:30.000000 flirimageextractor-1.4.0/setup.cfg
--rw-r--r--   0 aidankinzett   (501) staff       (20)      741 2020-03-17 02:48:52.000000 flirimageextractor-1.4.0/setup.py
+-rw-r--r--   0        0        0     1073 2023-04-27 11:01:17.379121 flirimageextractor-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3450 2023-04-27 11:01:17.379121 flirimageextractor-1.4.1/README.md
+-rw-r--r--   0        0        0      100 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/__init__.py
+-rw-r--r--   0        0        0     3604 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/__main__.py
+-rw-r--r--   0        0        0     2135 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/dialogs.py
+-rw-r--r--   0        0        0    16918 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/flir_image_extractor.py
+-rw-r--r--   0        0        0     9492 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/flyr_unpack.py
+-rw-r--r--   0        0        0     4140 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/processing.py
+-rw-r--r--   0        0        0    42181 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/thermal_base.py
+-rw-r--r--   0        0        0     9341 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/flirimageextractor/utils.py
+-rw-r--r--   0        0        0     1568 2023-04-27 11:01:17.403121 flirimageextractor-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 flirimageextractor-1.4.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flirimageextractor-1.4.0/flirimageextractor/flirimageextractor.py` & `flirimageextractor-1.4.1/flirimageextractor/flir_image_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import io
 import json
 import os
 import re
-import csv
 import subprocess
-from PIL import Image, ImageEnhance
-from math import sqrt, exp, log
-from matplotlib import pyplot as plt, cm
-from io import StringIO, BytesIO
+from math import sqrt, exp
+
 import numpy as np
+from PIL import Image, ImageEnhance
 from loguru import logger
-
-
+from matplotlib import pyplot as plt, cm
+from flirimageextractor.thermal_base import ThermalImage
 class FlirImageExtractor:
     """
     Instance of FlirImageExtractor
 
     """
 
     def __init__(self, exiftool_path="exiftool", is_debug=False, palettes=None):
@@ -79,15 +77,15 @@
         """
         Given a valid image path, return a boolean of whether the image contains thermal data.
 
         :param flir_img_filename: File path or file like object to load the image from
         :return: Bool
         """
         metadata = self.get_metadata(flir_img_filename)
-        return "RawThermalImageType" in metadata
+        return ("RawThermalImageType" in metadata) or ("ThermalData"  in metadata)
 
     def process_image(self, flir_img_file, RGB=False):
         """
         Given a valid image path, process the file: extract real thermal values
         and an RGB image if specified
 
         :param flir_img_file: File path or file like object to load the image from
@@ -98,17 +96,22 @@
         self.loadfile(flir_img_file)
 
         # if its a TIFF different settings are required
         if self.get_image_type().upper().strip() == "TIFF":
             # valid for tiff images from Zenmuse XTR
             self.use_thumbnail = True
             self.fix_endian = False
+        if self.get_image_type().upper().strip() == "DJI":
+            # valid for radiometric format thermal camera images from DJI Zenmuse ZH20T camera
+            image = ThermalImage(image_path=flir_img_file, camera_manufacturer="dji")
+            self.thermal_image_np  = image.thermal_np   
+        else:
 
-        # extract the thermal image and set it to the class variable
-        self.thermal_image_np = self.extract_thermal_image()
+            # extract the thermal image and set it to the class variable
+            self.thermal_image_np = self.extract_thermal_image()
 
         if RGB:
             self.rgb_image_np = self.extract_embedded_image()
 
     def get_image_type(self):
         """
         Get the embedded thermal image type, generally can be TIFF or PNG
@@ -125,15 +128,17 @@
                 ]
             )
         else:
             self.flir_img_bytes.seek(0)
             args = ["exiftool", "-RawThermalImageType", "-j", "-"]
             p = subprocess.Popen(args, stdin=subprocess.PIPE, stdout=subprocess.PIPE)
             meta_json, err = p.communicate(input=self.flir_img_bytes.read())
-
+     
+        if "RawThermalImageType" not in json.loads(meta_json.decode())[0]:
+            return "DJI"
         return json.loads(meta_json.decode())[0]["RawThermalImageType"]
 
     def get_rgb_np(self):
         """
         Return the last extracted rgb image
 
         :return:
@@ -422,22 +427,41 @@
             img_thermal = enhancer.enhance(3)
 
             if bytesIO:
                 bytes = io.BytesIO()
                 img_thermal.save(bytes, "jpeg", quality=100)
                 return_array.append(bytes)
             else:
-                filename_array = thermal_output_filename.split(".")
+                transformed_filename = transform_filename_into_directory(
+                    thermal_output_filename, str(palette.name)
+                )
+                filename_array = transformed_filename.split(".")
                 filename = (
                     filename_array[0]
                     + "_"
                     + str(palette.name)
                     + "."
                     + filename_array[1]
                 )
                 if self.is_debug:
                     logger.debug("Saving Thermal image to:{}".format(filename))
 
                 img_thermal.save(filename, "jpeg", quality=100)
                 return_array.append(filename)
 
         return return_array
+
+
+def transform_filename_into_directory(path: str, palette: str) -> str:
+    """
+    Creates a directory for the processed files color palette, if one doesn't exist
+    :param path:
+    :param palette: the palette to create a directory for e.g. "bwr",
+    :return: The new path for the file with the directory created and inserted into the string
+    @author Conor Brosnan <c.brosnan@nationaldrones.com>
+    """
+    head, tail = os.path.split(path)
+    directory = os.path.join(head, palette)
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+    filename = os.path.join(directory, tail)
+    return filename
```

