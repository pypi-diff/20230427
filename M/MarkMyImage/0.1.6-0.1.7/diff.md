# Comparing `tmp/MarkMyImage-0.1.6.tar.gz` & `tmp/MarkMyImage-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarkMyImage-0.1.6.tar", last modified: Wed Apr 26 11:22:31 2023, max compression
+gzip compressed data, was "MarkMyImage-0.1.7.tar", last modified: Thu Apr 27 12:38:34 2023, max compression
```

## Comparing `MarkMyImage-0.1.6.tar` & `MarkMyImage-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/MarkMyImage/
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     3575 2023-04-26 11:22:16.000000 MarkMyImage-0.1.6/MarkMyImage/__init__.py
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/MarkMyImage.egg-info/
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     2215 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/PKG-INFO
--rw-rw-r--   0 alatas    (1001) alatas    (1001)      254 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/SOURCES.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)        1 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/dependency_links.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       41 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/entry_points.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)        7 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/requires.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       12 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/top_level.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     2215 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/PKG-INFO
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     1602 2023-04-26 09:00:08.000000 MarkMyImage-0.1.6/README.md
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       38 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/setup.cfg
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     1003 2023-04-26 11:22:26.000000 MarkMyImage-0.1.6/setup.py
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/MarkMyImage/
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     4135 2023-04-27 12:36:14.000000 MarkMyImage-0.1.7/MarkMyImage/__init__.py
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/MarkMyImage.egg-info/
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     2208 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/PKG-INFO
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)      254 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)        1 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       41 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/entry_points.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       14 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/requires.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       12 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/top_level.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     2208 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/PKG-INFO
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     1595 2023-04-27 12:38:10.000000 MarkMyImage-0.1.7/README.md
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       38 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/setup.cfg
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     1013 2023-04-27 12:38:33.000000 MarkMyImage-0.1.7/setup.py
```

### Comparing `MarkMyImage-0.1.6/MarkMyImage/__init__.py` & `MarkMyImage-0.1.7/MarkMyImage/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 import os
 import argparse
 import logging
-from PIL import Image, ImageEnhance
+from PIL import Image, ImageEnhance, ImageFile
+import pyheif
 
+ImageFile.LOAD_TRUNCATED_IMAGES = True
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
+
 def apply_transparency(watermark, transparency):
     alpha = watermark.split()[3]
     alpha = ImageEnhance.Brightness(alpha).enhance(transparency)
     watermark.putalpha(alpha)
     return watermark
 
+
+def open_heic_image(image_path):
+    heif_file = pyheif.read(image_path)
+    return Image.frombytes(
+        heif_file.mode,
+        heif_file.size,
+        heif_file.data,
+        "raw",
+        heif_file.mode,
+    )
+
+
 def add_watermark(input_folder, watermark_path, output_folder, position, transparency, rotation_angle, logo_scale):
     if not os.path.exists(output_folder):
-        logging.INFO(f"Specified output_folder does not exist, it will be created -> {output_folder}.")
+        logging.info(f"Specified output_folder does not exist, it will be created -> {output_folder}.")
         os.makedirs(output_folder)
 
     try:
         watermark = Image.open(watermark_path).convert("RGBA")
     except FileNotFoundError:
         logging.error(f"Watermark file not found: {watermark_path}")
         return
     except IOError:
         logging.error(f"Unable to open watermark file: {watermark_path}")
         return
-    
+
     watermark = apply_transparency(watermark, transparency)
 
     for item in os.listdir(input_folder):
 
-        if not item.endswith(".jpg") and not item.endswith(".png"):
-            logging.info(f"File {item} is not supported. Only jpg and png files allowed")
+        if not item.endswith((".jpg", ".jpeg", ".png", ".heic")):
+            logging.info(f"File {item} is not supported. Only jpg, jpeg, heic and png files allowed")
             continue
 
         logging.info(f'Processing image: {item}')
         image_path = os.path.join(input_folder, item)
         try:
-            img = Image.open(image_path).convert("RGB")
+            if item.lower().endswith(".heic"):
+                img = open_heic_image(image_path).convert("RGB")
+            else:
+                img = Image.open(image_path).convert("RGB")
         except IOError:
             logging.error(f"Unable to open image file: {image_path}")
             continue
 
         # Adjust logo size in relation to the image size
         ratio = min(img.width, img.height) * logo_scale / max(watermark.width, watermark.height)
         new_size = (int(watermark.width * ratio), int(watermark.height * ratio))
@@ -49,24 +67,31 @@
         # Rotate the logo
         rotated_watermark = resized_watermark.rotate(rotation_angle, expand=True, resample=Image.BICUBIC)
 
         x, y = position
         if x == 0 and y == 0:
             x = (img.width - rotated_watermark.width) // 2
             y = (img.height - rotated_watermark.height) // 2
-        img.paste(rotated_watermark, (x, y, x + rotated_watermark.width, y + rotated_watermark.height), rotated_watermark)
+        img.paste(rotated_watermark, (x, y, x + rotated_watermark.width, y + rotated_watermark.height),
+                  rotated_watermark)
         img.save(os.path.join(output_folder, item))
         logging.info(f'Saved watermarked image to: {os.path.join(output_folder, item)}')
 
+
 def main():
     parser = argparse.ArgumentParser(description="Add a watermark to all images in a folder.")
     parser.add_argument("input_folder", help="Path to the input image folder.")
     parser.add_argument("watermark_path", help="Path to the watermark logo image.")
     parser.add_argument("output_folder", help="Path to the output image folder.")
-    parser.add_argument("-p", "--position", nargs=2, type=int, default=[0, 0], help="Coordinates (x, y) of the logo's center. Default: 0 0")
-    parser.add_argument("-t", "--transparency", type=float, default=1, help="Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 1")
-    parser.add_argument("-r", "--rotation_angle", type=float, default=0, help="Rotation angle of the logo (in degrees). Default: 0")
-    parser.add_argument("-l", "--logo_scale", type=float, default=1, help="Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 1")
+    parser.add_argument("-p", "--position", nargs=2, type=int, default=[0, 0],
+                        help="Coordinates (x, y) of the logo's center. Default: 0 0")
+    parser.add_argument("-t", "--transparency", type=float, default=1,
+                        help="Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 1")
+    parser.add_argument("-r", "--rotation_angle", type=float, default=0,
+                        help="Rotation angle of the logo (in degrees). Default: 0")
+    parser.add_argument("-l", "--logo_scale", type=float, default=1,
+                        help="Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 1")
 
     args = parser.parse_args()
 
-    add_watermark(args.input_folder, args.watermark_path, args.output_folder, args.position, args.transparency, args.rotation_angle, args.logo_scale)
+    add_watermark(args.input_folder, args.watermark_path, args.output_folder, args.position, args.transparency,
+                  args.rotation_angle, args.logo_scale)
```

### Comparing `MarkMyImage-0.1.6/MarkMyImage.egg-info/PKG-INFO` & `MarkMyImage-0.1.7/MarkMyImage.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarkMyImage
-Version: 0.1.6
+Version: 0.1.7
 Summary: Add a watermark to all images in a folder.
 Author: Lomezno
 Author-email: dbwspain@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -41,18 +41,18 @@
 
 - `input_folder`: Path to the folder containing the input images.
 - `watermark_path`: Path to the watermark logo image (PNG format recommended for transparency support).
 - `output_folder`: Path to the folder where the watermarked images will be saved.
 
 ### Options
 
-- `--position X Y`: Coordinates (X, Y) of the top-left corner of the logo. Default: 10 10
-- `--transparency VALUE`: Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 0.5
-- `--rotation_angle VALUE`: Rotation angle of the logo (in degrees). Default: 30
-- `--logo_scale VALUE`: Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 0.2
+- `--position X Y`: Coordinates (X, Y) of the top-left corner of the logo. Default: 0 0
+- `--transparency VALUE`: Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 1
+- `--rotation_angle VALUE`: Rotation angle of the logo (in degrees). Default: 0
+- `--logo_scale VALUE`: Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 1
 
 ### Example
 
 ```
 mmi /path/to/input/folder /path/to/watermark/logo.png /path/to/output/folder --position 10 10 --transparency 0.7 --rotation_angle 45 --logo_scale 0.15
 ```
```

### Comparing `MarkMyImage-0.1.6/PKG-INFO` & `MarkMyImage-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarkMyImage
-Version: 0.1.6
+Version: 0.1.7
 Summary: Add a watermark to all images in a folder.
 Author: Lomezno
 Author-email: dbwspain@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -41,18 +41,18 @@
 
 - `input_folder`: Path to the folder containing the input images.
 - `watermark_path`: Path to the watermark logo image (PNG format recommended for transparency support).
 - `output_folder`: Path to the folder where the watermarked images will be saved.
 
 ### Options
 
-- `--position X Y`: Coordinates (X, Y) of the top-left corner of the logo. Default: 10 10
-- `--transparency VALUE`: Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 0.5
-- `--rotation_angle VALUE`: Rotation angle of the logo (in degrees). Default: 30
-- `--logo_scale VALUE`: Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 0.2
+- `--position X Y`: Coordinates (X, Y) of the top-left corner of the logo. Default: 0 0
+- `--transparency VALUE`: Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 1
+- `--rotation_angle VALUE`: Rotation angle of the logo (in degrees). Default: 0
+- `--logo_scale VALUE`: Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 1
 
 ### Example
 
 ```
 mmi /path/to/input/folder /path/to/watermark/logo.png /path/to/output/folder --position 10 10 --transparency 0.7 --rotation_angle 45 --logo_scale 0.15
 ```
```

### Comparing `MarkMyImage-0.1.6/README.md` & `MarkMyImage-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 - `input_folder`: Path to the folder containing the input images.
 - `watermark_path`: Path to the watermark logo image (PNG format recommended for transparency support).
 - `output_folder`: Path to the folder where the watermarked images will be saved.
 
 ### Options
 
-- `--position X Y`: Coordinates (X, Y) of the top-left corner of the logo. Default: 10 10
-- `--transparency VALUE`: Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 0.5
-- `--rotation_angle VALUE`: Rotation angle of the logo (in degrees). Default: 30
-- `--logo_scale VALUE`: Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 0.2
+- `--position X Y`: Coordinates (X, Y) of the top-left corner of the logo. Default: 0 0
+- `--transparency VALUE`: Transparency level of the logo (0-1, 0 is fully transparent, 1 is opaque). Default: 1
+- `--rotation_angle VALUE`: Rotation angle of the logo (in degrees). Default: 0
+- `--logo_scale VALUE`: Size of the logo in relation to the image (0-1, where 1 is equal to the size of the image). Default: 1
 
 ### Example
 
 ```
 mmi /path/to/input/folder /path/to/watermark/logo.png /path/to/output/folder --position 10 10 --transparency 0.7 --rotation_angle 45 --logo_scale 0.15
 ```
```

### Comparing `MarkMyImage-0.1.6/setup.py` & `MarkMyImage-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MarkMyImage",
-    version="0.1.6",
+    version="0.1.7",
     description="Add a watermark to all images in a folder.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lomezno",
     author_email="dbwspain@gmail.com",
     packages=find_packages(),
-    install_requires=["Pillow"],
+    install_requires=["Pillow", "pyheif"],
     entry_points={
         "console_scripts": [
             "mmi=MarkMyImage:main",
         ],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
```

