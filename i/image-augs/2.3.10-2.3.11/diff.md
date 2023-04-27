# Comparing `tmp/image_augs-2.3.10.tar.gz` & `tmp/image_augs-2.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-2.3.10.tar", last modified: Wed Apr 26 13:31:50 2023, max compression
+gzip compressed data, was "dist/image_augs-2.3.11.tar", last modified: Thu Apr 27 06:02:50 2023, max compression
```

## Comparing `image_augs-2.3.10.tar` & `image_augs-2.3.11.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8487 2023-04-26 13:31:50.000000 image_augs-2.3.10/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     7906 2023-04-25 07:14:06.000000 image_augs-2.3.10/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.3.10/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9929 2023-04-26 10:51:29.000000 image_augs-2.3.10/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    15771 2023-04-26 11:03:13.000000 image_augs-2.3.10/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.3.10/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8487 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      363 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-26 13:31:50.000000 image_augs-2.3.10/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.3.10/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    18793 2023-04-26 13:30:48.000000 image_augs-2.3.10/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    28547 2023-04-26 13:05:10.000000 image_augs-2.3.10/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.3.10/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4719 2023-04-26 13:22:59.000000 image_augs-2.3.10/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.3.10/instance_seg/yml_writer_poly.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-26 13:31:50.000000 image_augs-2.3.10/object_detection_new/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.3.10/object_detection_new/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    18848 2023-04-26 13:09:06.000000 image_augs-2.3.10/object_detection_new/augmentation_rect.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.3.10/object_detection_new/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    27750 2023-04-26 11:46:09.000000 image_augs-2.3.10/object_detection_new/txt_reader_rect.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4844 2023-04-26 08:52:52.000000 image_augs-2.3.10/object_detection_new/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-25 08:31:35.000000 image_augs-2.3.10/object_detection_new/yml_writer_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-26 13:31:50.000000 image_augs-2.3.10/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.3.10/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-27 06:02:50.000000 image_augs-2.3.11/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8571 2023-04-27 06:02:50.000000 image_augs-2.3.11/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7990 2023-04-27 05:12:07.000000 image_augs-2.3.11/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-27 06:02:50.000000 image_augs-2.3.11/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.3.11/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9929 2023-04-26 10:51:29.000000 image_augs-2.3.11/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    15771 2023-04-26 11:03:13.000000 image_augs-2.3.11/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.3.11/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-27 06:02:50.000000 image_augs-2.3.11/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8571 2023-04-27 06:02:50.000000 image_augs-2.3.11/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-27 06:02:50.000000 image_augs-2.3.11/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-27 06:02:50.000000 image_augs-2.3.11/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      363 2023-04-27 06:02:50.000000 image_augs-2.3.11/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-27 06:02:50.000000 image_augs-2.3.11/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-27 06:02:50.000000 image_augs-2.3.11/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.3.11/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    18793 2023-04-26 13:30:48.000000 image_augs-2.3.11/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    28585 2023-04-27 05:52:13.000000 image_augs-2.3.11/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.3.11/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4725 2023-04-27 05:51:37.000000 image_augs-2.3.11/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.3.11/instance_seg/yml_writer_poly.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-27 06:02:50.000000 image_augs-2.3.11/object_detection_new/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.3.11/object_detection_new/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    18848 2023-04-26 13:09:06.000000 image_augs-2.3.11/object_detection_new/augmentation_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.3.11/object_detection_new/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    27789 2023-04-27 05:52:16.000000 image_augs-2.3.11/object_detection_new/txt_reader_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4804 2023-04-27 05:50:13.000000 image_augs-2.3.11/object_detection_new/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-25 08:31:35.000000 image_augs-2.3.11/object_detection_new/yml_writer_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-27 06:02:50.000000 image_augs-2.3.11/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.3.11/setup.py
```

### Comparing `image_augs-2.3.10/PKG-INFO` & `image_augs-2.3.11/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 2.3.10
+Version: 2.3.11
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -70,144 +70,151 @@
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 
-annotation_folder = 'Vehicle registration plate'
-new_aug_saved_folder = 'new_2'
-train_split = 1.0
+annotation_folder = 'your folder'
+new_aug_saved_folder = 'new saved folder'
+train_split = 0.90
 image_H = 640  #check above for height and width setting
 image_W = 'keep_aspect_ratio'
 
 
 rect_aug = RectAugmentation(new_aug_saved_folder)
 
 rect_aug.Image_augmentation(annotation_folder,
                                  
                                 train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=False,  blur_f=0.7,
+                                 blur=False,  blur_f=0.8,
 
-                                 rotate=False, rotate_f = 0.7, 
+                                 motionBlur= False , motionBlur_f= 0.8 ,
+
+                                 rotate=False, rotate_f = 0.8, 
 
                                  noise=False, noise_f=0.8,
 
-                                 perspective=False, perspective_f = 0.7,
+                                 perspective=False, perspective_f = 0.8,
 
-                                 affine=False, affine_f=0.7,
+                                 affine=False, affine_f=0.8,
 
-                                 brightness=False, brightness_f=0.7,
+                                 brightness=False, brightness_f=0.8,
                                     
-                                 hue=False, hue_f=0.7,
+                                 hue=False, hue_f=0.8,
 
                                  removesaturation=False, removesaturation_f=0.8,
 
-                                 contrast=False, contrast_f=0.5,
+                                 contrast=False, contrast_f=0.8,
 
-                                 upflip=False, upflip_f=0.5,
+                                 upflip=False, upflip_f=0.8,
 
-                                 shear=False , shear_f=0.7, 
+                                 shear=False, shear_f=0.8, 
 
-                                 rotate90=False, rotate90_f =0.6,
+                                 rotate90=False, rotate90_f =0.8,
 
-                                 blur_and_noise=False, blur_and_noise_f=0.7,
+                                 blur_and_noise=False, blur_and_noise_f=0.8,
 
                                  image_cutout = False, image_cutout_f=0.8,
                                     
-                                 mix_aug=False, mix_aug_f=0.4, 
+                                 mix_aug= False, mix_aug_f=0.8, 
                                     
-                                 temperature_change=False, temperature_change_f=0.7,  # change color temperature from cool to warm color
+                                 temperature_change= False, temperature_change_f=0.8,  # change color temperature from cool to warm color
 
-                                 weather_change=True,weather_change_f=0.3), # add rain , fog , snow in your images
+                                 weather_change=True,weather_change_f=0.8), # add rain , fog , snow in your images
+                               
                                 
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
 ```python
 #import these modules in your created <scriptname>.py file
 from instance_seg.json_reader_poly import PolygonAugmentation
 
 
+
+
 ################# image height and width combination  ##################
 
 # first combination --> for custom image size
 #  image_height = < custom image size > ; 640
 #  image_width = < custom image size > ; 320
 
 
 # second combination --> keep aspect ratio of the image
 #  image_height = 640
-#  image_width  = 'keep_aspect_ratio_true'
+#  image_width  = 'keep_aspect_ratio_False'
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 #### yolo ####
-# if yolo True then it will normalize all images and save it as txt , if false augmentations will be saved as json.
+# if yolo False then it will normalize all images and save it as txt , if false augmentations will be saved as json.
 
 
-annotation_folder = '<your annotation folder>'
-new_aug_saved_folder = '<where you want to save your images , just  provide a name>'
-train_split = .90
-image_H = 'keep_original_image_height' #check above for height and width setting
-image_W = 'keep_original_image_width'
-yolo = True 
+annotation_folder = 'your data'
+new_aug_saved_folder = 'new saved dataset name'
+train_split = 0.70
+image_H = 640  #check above for height and width setting
+image_W = 'keep_aspect_ratio'
+yolo = True
 
 
 im_aug_helper = PolygonAugmentation(aug_save_folder_name=new_aug_saved_folder,
                                     yolo=yolo)
 
 im_aug_helper.Image_augmentation(annotation_folder,
                                  
                                  train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=True,  blur_f=0.1,
+                                 blur=True,  blur_f=0.8,
 
-                                 rotate=False, rotate_f = 0.2, 
+                                 motionBlur= False , motionBlur_f= 0.5,
 
-                                 noise=False, noise_f=0.8,
+                                 rotate=True, rotate_f = 0.8, 
 
-                                 perspective=False, perspective_f = 0.8,
+                                 noise=True, noise_f=0.6,
 
-                                 affine=False, affine_f=0.8,
+                                 perspective=True, perspective_f = 0.6,
 
-                                 brightness=False, brightness_f=0.8,
+                                 affine=True, affine_f=0.6,
+
+                                 brightness=True, brightness_f=0.6,
                                     
-                                 hue=True, hue_f=0.2,
+                                 hue=True, hue_f=0.6,
 
-                                 removesaturation=True, removesaturation_f=0.1,
+                                 removesaturation=True, removesaturation_f=0.6,
 
-                                 contrast=False, contrast_f=0.8,
+                                 contrast=True, contrast_f=0.6,
 
-                                 upflip=False, upflip_f=0.8,
+                                 upflip=True, upflip_f=0.8,
 
-                                 shear=False , shear_f=0.8, 
+                                 shear=True , shear_f=0.7, 
 
-                                 rotate90=False, rotate90_f =0.8,
+                                 rotate90=True, rotate90_f =1.0,
 
-                                 blur_and_noise=False, blur_and_noise_f=0.8,
+                                 blur_and_noise=True, blur_and_noise_f=0.6,
 
-                                 image_cutout = False, image_cutout_f=0.8,
+                                 image_cutout = True, image_cutout_f=0.6,
                                     
-                                 mix_aug=False, mix_aug_f=0.8,
+                                 mix_aug=True, mix_aug_f=0.7,
                                     
-                                 temperature_change=False, temperature_change_f=0.8,
+                                 temperature_change=True, temperature_change_f=0.5,
                                  
                                  weather_change=True,weather_change_f=0.3)
 #results will be saved in < your given folder >
 ```
 
 **This Script is for IMAGE CLASSIFICATION**
```

### Comparing `image_augs-2.3.10/README.md` & `image_augs-2.3.11/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,144 +55,151 @@
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 
-annotation_folder = 'Vehicle registration plate'
-new_aug_saved_folder = 'new_2'
-train_split = 1.0
+annotation_folder = 'your folder'
+new_aug_saved_folder = 'new saved folder'
+train_split = 0.90
 image_H = 640  #check above for height and width setting
 image_W = 'keep_aspect_ratio'
 
 
 rect_aug = RectAugmentation(new_aug_saved_folder)
 
 rect_aug.Image_augmentation(annotation_folder,
                                  
                                 train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=False,  blur_f=0.7,
+                                 blur=False,  blur_f=0.8,
 
-                                 rotate=False, rotate_f = 0.7, 
+                                 motionBlur= False , motionBlur_f= 0.8 ,
+
+                                 rotate=False, rotate_f = 0.8, 
 
                                  noise=False, noise_f=0.8,
 
-                                 perspective=False, perspective_f = 0.7,
+                                 perspective=False, perspective_f = 0.8,
 
-                                 affine=False, affine_f=0.7,
+                                 affine=False, affine_f=0.8,
 
-                                 brightness=False, brightness_f=0.7,
+                                 brightness=False, brightness_f=0.8,
                                     
-                                 hue=False, hue_f=0.7,
+                                 hue=False, hue_f=0.8,
 
                                  removesaturation=False, removesaturation_f=0.8,
 
-                                 contrast=False, contrast_f=0.5,
+                                 contrast=False, contrast_f=0.8,
 
-                                 upflip=False, upflip_f=0.5,
+                                 upflip=False, upflip_f=0.8,
 
-                                 shear=False , shear_f=0.7, 
+                                 shear=False, shear_f=0.8, 
 
-                                 rotate90=False, rotate90_f =0.6,
+                                 rotate90=False, rotate90_f =0.8,
 
-                                 blur_and_noise=False, blur_and_noise_f=0.7,
+                                 blur_and_noise=False, blur_and_noise_f=0.8,
 
                                  image_cutout = False, image_cutout_f=0.8,
                                     
-                                 mix_aug=False, mix_aug_f=0.4, 
+                                 mix_aug= False, mix_aug_f=0.8, 
                                     
-                                 temperature_change=False, temperature_change_f=0.7,  # change color temperature from cool to warm color
+                                 temperature_change= False, temperature_change_f=0.8,  # change color temperature from cool to warm color
 
-                                 weather_change=True,weather_change_f=0.3), # add rain , fog , snow in your images
+                                 weather_change=True,weather_change_f=0.8), # add rain , fog , snow in your images
+                               
                                 
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
 ```python
 #import these modules in your created <scriptname>.py file
 from instance_seg.json_reader_poly import PolygonAugmentation
 
 
+
+
 ################# image height and width combination  ##################
 
 # first combination --> for custom image size
 #  image_height = < custom image size > ; 640
 #  image_width = < custom image size > ; 320
 
 
 # second combination --> keep aspect ratio of the image
 #  image_height = 640
-#  image_width  = 'keep_aspect_ratio_true'
+#  image_width  = 'keep_aspect_ratio_False'
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 #### yolo ####
-# if yolo True then it will normalize all images and save it as txt , if false augmentations will be saved as json.
+# if yolo False then it will normalize all images and save it as txt , if false augmentations will be saved as json.
 
 
-annotation_folder = '<your annotation folder>'
-new_aug_saved_folder = '<where you want to save your images , just  provide a name>'
-train_split = .90
-image_H = 'keep_original_image_height' #check above for height and width setting
-image_W = 'keep_original_image_width'
-yolo = True 
+annotation_folder = 'your data'
+new_aug_saved_folder = 'new saved dataset name'
+train_split = 0.70
+image_H = 640  #check above for height and width setting
+image_W = 'keep_aspect_ratio'
+yolo = True
 
 
 im_aug_helper = PolygonAugmentation(aug_save_folder_name=new_aug_saved_folder,
                                     yolo=yolo)
 
 im_aug_helper.Image_augmentation(annotation_folder,
                                  
                                  train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=True,  blur_f=0.1,
+                                 blur=True,  blur_f=0.8,
 
-                                 rotate=False, rotate_f = 0.2, 
+                                 motionBlur= False , motionBlur_f= 0.5,
 
-                                 noise=False, noise_f=0.8,
+                                 rotate=True, rotate_f = 0.8, 
 
-                                 perspective=False, perspective_f = 0.8,
+                                 noise=True, noise_f=0.6,
 
-                                 affine=False, affine_f=0.8,
+                                 perspective=True, perspective_f = 0.6,
 
-                                 brightness=False, brightness_f=0.8,
+                                 affine=True, affine_f=0.6,
+
+                                 brightness=True, brightness_f=0.6,
                                     
-                                 hue=True, hue_f=0.2,
+                                 hue=True, hue_f=0.6,
 
-                                 removesaturation=True, removesaturation_f=0.1,
+                                 removesaturation=True, removesaturation_f=0.6,
 
-                                 contrast=False, contrast_f=0.8,
+                                 contrast=True, contrast_f=0.6,
 
-                                 upflip=False, upflip_f=0.8,
+                                 upflip=True, upflip_f=0.8,
 
-                                 shear=False , shear_f=0.8, 
+                                 shear=True , shear_f=0.7, 
 
-                                 rotate90=False, rotate90_f =0.8,
+                                 rotate90=True, rotate90_f =1.0,
 
-                                 blur_and_noise=False, blur_and_noise_f=0.8,
+                                 blur_and_noise=True, blur_and_noise_f=0.6,
 
-                                 image_cutout = False, image_cutout_f=0.8,
+                                 image_cutout = True, image_cutout_f=0.6,
                                     
-                                 mix_aug=False, mix_aug_f=0.8,
+                                 mix_aug=True, mix_aug_f=0.7,
                                     
-                                 temperature_change=False, temperature_change_f=0.8,
+                                 temperature_change=True, temperature_change_f=0.5,
                                  
                                  weather_change=True,weather_change_f=0.3)
 #results will be saved in < your given folder >
 ```
 
 **This Script is for IMAGE CLASSIFICATION**
```

### Comparing `image_augs-2.3.10/classification/classification_.py` & `image_augs-2.3.11/classification/classification_.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/classification/classification_combined.py` & `image_augs-2.3.11/classification/classification_combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/classification/logging_util.py` & `image_augs-2.3.11/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/image_augs.egg-info/PKG-INFO` & `image_augs-2.3.11/image_augs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-augs
-Version: 2.3.10
+Version: 2.3.11
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -70,144 +70,151 @@
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 
-annotation_folder = 'Vehicle registration plate'
-new_aug_saved_folder = 'new_2'
-train_split = 1.0
+annotation_folder = 'your folder'
+new_aug_saved_folder = 'new saved folder'
+train_split = 0.90
 image_H = 640  #check above for height and width setting
 image_W = 'keep_aspect_ratio'
 
 
 rect_aug = RectAugmentation(new_aug_saved_folder)
 
 rect_aug.Image_augmentation(annotation_folder,
                                  
                                 train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=False,  blur_f=0.7,
+                                 blur=False,  blur_f=0.8,
 
-                                 rotate=False, rotate_f = 0.7, 
+                                 motionBlur= False , motionBlur_f= 0.8 ,
+
+                                 rotate=False, rotate_f = 0.8, 
 
                                  noise=False, noise_f=0.8,
 
-                                 perspective=False, perspective_f = 0.7,
+                                 perspective=False, perspective_f = 0.8,
 
-                                 affine=False, affine_f=0.7,
+                                 affine=False, affine_f=0.8,
 
-                                 brightness=False, brightness_f=0.7,
+                                 brightness=False, brightness_f=0.8,
                                     
-                                 hue=False, hue_f=0.7,
+                                 hue=False, hue_f=0.8,
 
                                  removesaturation=False, removesaturation_f=0.8,
 
-                                 contrast=False, contrast_f=0.5,
+                                 contrast=False, contrast_f=0.8,
 
-                                 upflip=False, upflip_f=0.5,
+                                 upflip=False, upflip_f=0.8,
 
-                                 shear=False , shear_f=0.7, 
+                                 shear=False, shear_f=0.8, 
 
-                                 rotate90=False, rotate90_f =0.6,
+                                 rotate90=False, rotate90_f =0.8,
 
-                                 blur_and_noise=False, blur_and_noise_f=0.7,
+                                 blur_and_noise=False, blur_and_noise_f=0.8,
 
                                  image_cutout = False, image_cutout_f=0.8,
                                     
-                                 mix_aug=False, mix_aug_f=0.4, 
+                                 mix_aug= False, mix_aug_f=0.8, 
                                     
-                                 temperature_change=False, temperature_change_f=0.7,  # change color temperature from cool to warm color
+                                 temperature_change= False, temperature_change_f=0.8,  # change color temperature from cool to warm color
 
-                                 weather_change=True,weather_change_f=0.3), # add rain , fog , snow in your images
+                                 weather_change=True,weather_change_f=0.8), # add rain , fog , snow in your images
+                               
                                 
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
 ```python
 #import these modules in your created <scriptname>.py file
 from instance_seg.json_reader_poly import PolygonAugmentation
 
 
+
+
 ################# image height and width combination  ##################
 
 # first combination --> for custom image size
 #  image_height = < custom image size > ; 640
 #  image_width = < custom image size > ; 320
 
 
 # second combination --> keep aspect ratio of the image
 #  image_height = 640
-#  image_width  = 'keep_aspect_ratio_true'
+#  image_width  = 'keep_aspect_ratio_False'
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 #### yolo ####
-# if yolo True then it will normalize all images and save it as txt , if false augmentations will be saved as json.
+# if yolo False then it will normalize all images and save it as txt , if false augmentations will be saved as json.
 
 
-annotation_folder = '<your annotation folder>'
-new_aug_saved_folder = '<where you want to save your images , just  provide a name>'
-train_split = .90
-image_H = 'keep_original_image_height' #check above for height and width setting
-image_W = 'keep_original_image_width'
-yolo = True 
+annotation_folder = 'your data'
+new_aug_saved_folder = 'new saved dataset name'
+train_split = 0.70
+image_H = 640  #check above for height and width setting
+image_W = 'keep_aspect_ratio'
+yolo = True
 
 
 im_aug_helper = PolygonAugmentation(aug_save_folder_name=new_aug_saved_folder,
                                     yolo=yolo)
 
 im_aug_helper.Image_augmentation(annotation_folder,
                                  
                                  train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=True,  blur_f=0.1,
+                                 blur=True,  blur_f=0.8,
 
-                                 rotate=False, rotate_f = 0.2, 
+                                 motionBlur= False , motionBlur_f= 0.5,
 
-                                 noise=False, noise_f=0.8,
+                                 rotate=True, rotate_f = 0.8, 
 
-                                 perspective=False, perspective_f = 0.8,
+                                 noise=True, noise_f=0.6,
 
-                                 affine=False, affine_f=0.8,
+                                 perspective=True, perspective_f = 0.6,
 
-                                 brightness=False, brightness_f=0.8,
+                                 affine=True, affine_f=0.6,
+
+                                 brightness=True, brightness_f=0.6,
                                     
-                                 hue=True, hue_f=0.2,
+                                 hue=True, hue_f=0.6,
 
-                                 removesaturation=True, removesaturation_f=0.1,
+                                 removesaturation=True, removesaturation_f=0.6,
 
-                                 contrast=False, contrast_f=0.8,
+                                 contrast=True, contrast_f=0.6,
 
-                                 upflip=False, upflip_f=0.8,
+                                 upflip=True, upflip_f=0.8,
 
-                                 shear=False , shear_f=0.8, 
+                                 shear=True , shear_f=0.7, 
 
-                                 rotate90=False, rotate90_f =0.8,
+                                 rotate90=True, rotate90_f =1.0,
 
-                                 blur_and_noise=False, blur_and_noise_f=0.8,
+                                 blur_and_noise=True, blur_and_noise_f=0.6,
 
-                                 image_cutout = False, image_cutout_f=0.8,
+                                 image_cutout = True, image_cutout_f=0.6,
                                     
-                                 mix_aug=False, mix_aug_f=0.8,
+                                 mix_aug=True, mix_aug_f=0.7,
                                     
-                                 temperature_change=False, temperature_change_f=0.8,
+                                 temperature_change=True, temperature_change_f=0.5,
                                  
                                  weather_change=True,weather_change_f=0.3)
 #results will be saved in < your given folder >
 ```
 
 **This Script is for IMAGE CLASSIFICATION**
```

### Comparing `image_augs-2.3.10/image_augs.egg-info/SOURCES.txt` & `image_augs-2.3.11/image_augs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/instance_seg/augment_poly.py` & `image_augs-2.3.11/instance_seg/augment_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/instance_seg/json_reader_poly.py` & `image_augs-2.3.11/instance_seg/json_reader_poly.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,158 +129,158 @@
         
         
         # combining all the augmentations here
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
             
             if blur:
            
-                frac_data  = int(self.split * blur_f)
+                frac_data  = round(self.split * blur_f)
                 if no_track <= frac_data:
                     try:
                         points =  executor.submit(self.augment.image_blur,im_read,poly_on_image,image_height,image_width)
                         p , im = next(points.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
                     except Exception as e:
                         logger.warning(f'Blur problem : {e} ')
             
             if rotate:
-                frac_data  = int(self.split * rotate_f)
+                frac_data  = round(self.split * rotate_f)
                 if no_track <= frac_data:
                     try:
                         points2  = executor.submit(self.augment.image_rotate,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'ROTATION problem : {e} ')
                 
             if noise:
-                frac_data  = int(self.split * noise_f)
+                frac_data  = round(self.split * noise_f)
                 if no_track <= frac_data:
                     try:
                         points3  = executor.submit(self.augment.image_noise,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points3.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'Noise problem : {e} ')
                 
             if perspective:
-                frac_data  = int(self.split * perspective_f)
+                frac_data  = round(self.split * perspective_f)
                 if no_track <= frac_data:
                     try:
                         points4  = executor.submit(self.augment.image_perspective_transform,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points4.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'Perspective problem : {e} ')
                 
             if affine:
-                frac_data  = int(self.split * affine_f)
+                frac_data  = round(self.split * affine_f)
                 if no_track <= frac_data:
                     try:
                         points5  = executor.submit(self.augment.image_affine,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points5.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'Affine problem : {e} ')
                 
             if brightness:
-                frac_data  = int(self.split * brightness_f)
+                frac_data  = round(self.split * brightness_f)
                 if no_track <= frac_data:
                     try:
                         points6  = executor.submit(self.augment.image_brightness,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points6.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
                     except Exception as e:
                         logger.warning(f'Brightness problem : {e} ')
             
             if hue:
-                frac_data  = int(self.split * hue_f)
+                frac_data  = round(self.split * hue_f)
                 if no_track <= frac_data:
                     try:
                         points6  = executor.submit(self.augment.image_hue,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points6.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'hue problem : {e} ')
                 
             if removesaturation:
-                frac_data  = int(self.split * removesaturation_f)
+                frac_data  = round(self.split * removesaturation_f)
                 if no_track <= frac_data:
                     try:
                         points7  = executor.submit(self.augment.image_removeSaturation,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points7.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'remove saturation problem : {e} ')
                 
             if contrast:
-                frac_data  = int(self.split * contrast_f)
+                frac_data  = round(self.split * contrast_f)
                 if no_track <= frac_data:
                     try:
                         points8 = executor.submit(self.augment.image_contrast,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points8.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'Contrast problem : {e} ')
                 
             if upflip:
-                frac_data  = int(self.split * upflip_f)
+                frac_data  = round(self.split * upflip_f)
                 if no_track <= frac_data:
                     try:
                         points9  = executor.submit(self.augment.image_upFlip,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points9.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'upflip problem : {e} ')
                     
             if shear:
-                frac_data  = int(self.split * shear_f)
+                frac_data  = round(self.split * shear_f)
                 if no_track <= frac_data:
                     try:
                         points10  = executor.submit(self.augment.image_shear,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points10.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
                     except Exception as e:
                         logger.warning(f'shear problem : {e} ')
                 
             if rotate90:
-                frac_data  = int(self.split * rotate90_f)
+                frac_data  = round(self.split * rotate90_f)
                 if no_track <= frac_data:
                     try:
                         points11  = executor.submit(self.augment.image_rotate90,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points11.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'rotate90 problem : {e} ')
                 
             if blur_and_noise:
-                frac_data  = int(self.split * blur_and_noise_f)
+                frac_data  = round(self.split * blur_and_noise_f)
                 if no_track <= frac_data:
                     try:
                         points12  = executor.submit(self.augment.blur_and_noise,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points12.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'Blur and noise problem : {e} ')
                 
             if image_cutout:
-                frac_data  = int(self.split * image_cutout_f)
+                frac_data  = round(self.split * image_cutout_f)
                 if no_track <= frac_data:
                     try:
                         points13  = executor.submit(self.augment.image_cutOut,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points13.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'ImageCut problem : {e} ')
             
             if mix_aug:
-                frac_data  = int(self.split * mix_aug_f)
+                frac_data  = round(self.split * mix_aug_f)
                 if no_track <= frac_data:
                     try:
                         points14  = executor.submit(self.augment.mixed_aug_1,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points14.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     
                     except Exception as e:
@@ -307,36 +307,36 @@
                         p , im = next(points17.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     
                     except Exception as e:
                         logger.warning(f'Mixaug 4 problem : {e} ')
             
             if temperature_change:
-                frac_data  = int(self.split * temperature_change_f)
+                frac_data  = round(self.split * temperature_change_f)
                 if no_track <= frac_data:
                     try:
                         points18  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points18.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     except Exception as e:
                         logger.warning(f'Temperature change problem : {e} ')
 
             if weather_change:
-                frac_data  = int(self.split * weather_change_f)
+                frac_data  = round(self.split * weather_change_f)
                 if no_track <= frac_data:
                     try:
                         points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
                     
                     except Exception as e:
                         logger.warning(f'weather change problem : {e} ')
 
             if motionBlur:
-                frac_data  = int(self.split * motion_blur_f)
+                frac_data  = round(self.split * motion_blur_f)
                 if no_track <= frac_data:
                     try:
                         points2  = executor.submit(self.augment.image_motionBlur,im_read,poly_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
 
                     except Exception as e:
@@ -468,15 +468,15 @@
             
         
         #shuffling all images
         random.shuffle(all_images)
         # checking how many images
         self.len_total_images = len(all_images)
         # spliting into training set
-        self.split = int(self.len_total_images * train_split)
+        self.split = round(self.len_total_images * train_split)
         
         console.print(f'[bold cyan] [+] Total images : {self.len_total_images}   |   Train Split : {self.split} images   |    Test split : {self.len_total_images-self.split} images [bold cyan]')
         
         if train_split == 1.0:
                     shutil.rmtree(self.aug_save_folder_name)
                     shutil.rmtree(f'{self.aug_save_folder_name}/test')
```

### Comparing `image_augs-2.3.10/instance_seg/logging_util.py` & `image_augs-2.3.11/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/instance_seg/utils_poly.py` & `image_augs-2.3.11/instance_seg/utils_poly.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 def create_new_txt(image , label ,  points,train_path_images , train_path_labels,dict,yolo=True):
 
     if yolo:
 
         try:
             save_name = uuid.uuid4()
             
-            if type(image) == str:
-                image = cv2.imread(image)
+            # if type(image) == str:
+            #     image = cv2.imread(image)
 
-            cv2.imwrite(f'{train_path_images}/{save_name}.jpg',image)
+            # cv2.imwrite(f'{train_path_images}/{save_name}.jpg',image)
             txt_path=f'{train_path_labels}/{save_name}.txt'
             
             new_height , new_width , c = image.shape
         
             for p in points: 
                 labels = p.label 
                 label = dict[labels]
```

### Comparing `image_augs-2.3.10/instance_seg/yml_writer_poly.py` & `image_augs-2.3.11/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/object_detection_new/augmentation_rect.py` & `image_augs-2.3.11/object_detection_new/augmentation_rect.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/object_detection_new/logging_util.py` & `image_augs-2.3.11/object_detection_new/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.3.10/object_detection_new/txt_reader_rect.py` & `image_augs-2.3.11/object_detection_new/txt_reader_rect.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,184 +126,184 @@
     def Combined_augmentation(self,im_read , rect_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640,blur=True , blur_f = 0.5 ,motionBlur=True, motionBlur_f = 0.5, rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                             brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                             shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
                             mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
             if rotate:
-                frac_data  = int(self.split * rotate_f)
+                frac_data  = round(self.split * rotate_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_rotate,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                 except Exception as e:
                     logger.warning(f'Image rotation problem : {e}')
 
             if blur:
                 
-                frac_data  = int(self.split * blur_f)
+                frac_data  = round(self.split * blur_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_blur,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
-                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+                        utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path,)
                 except:
                   
                     logger.warning(f'Image blur problem : {e}')
 
             if noise:
-                frac_data  = int(self.split * noise_f)
+                frac_data  = round(self.split * noise_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_noise,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image noise problem : {e}')
 
             if perspective:
-                frac_data  = int(self.split * perspective_f)
+                frac_data  = round(self.split * perspective_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_perspective_transform,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image perpective problem : {e}')
             
             if affine:
-                frac_data  = int(self.split * affine_f)
+                frac_data  = round(self.split * affine_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_affine,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image affine problem : {e}')
 
             if brightness:
-                frac_data  = int(self.split * brightness_f)
+                frac_data  = round(self.split * brightness_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_brightness,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image brightness problem : {e}')
 
             if hue:
-                frac_data  = int(self.split * hue_f)
+                frac_data  = round(self.split * hue_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_hue,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image hue problem : {e}')
 
             if removesaturation:
 
-                frac_data  = int(self.split * removesaturation_f)
+                frac_data  = round(self.split * removesaturation_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_removeSaturation,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                 
                 except Exception as e:
                     logger.warning(f'Image remove saturation problem : {e}')
             
             if contrast:
-                frac_data  = int(self.split * contrast_f)
+                frac_data  = round(self.split * contrast_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_contrast,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image contrast problem : {e}')
 
             if upflip:
-                frac_data  = int(self.split * upflip_f)
+                frac_data  = round(self.split * upflip_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_upFlip,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image upflip problem : {e}')
 
             if shear:
-                frac_data  = int(self.split * shear_f)
+                frac_data  = round(self.split * shear_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_shear,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image shear problem : {e}')
 
             if rotate90:
-                frac_data  = int(self.split * rotate90_f)
+                frac_data  = round(self.split * rotate90_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_rotate90,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image rotation90 problem : {e}')
 
             if blur_and_noise:
-                frac_data  = int(self.split * blur_and_noise_f)
+                frac_data  = round(self.split * blur_and_noise_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.blur_and_noise,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image blur and noise problem : {e}')
 
             if image_cutout:
-                frac_data  = int(self.split * image_cutout_f)
+                frac_data  = round(self.split * image_cutout_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_cutOut,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image cutout problem : {e}')
 
             if mix_aug:
-                frac_data  = int(self.split * mix_aug_f)
+                frac_data  = round(self.split * mix_aug_f)
                 if no_track <= frac_data:
                     try:
                         points14  = executor.submit(self.augment.mixed_aug_1,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points14.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                     
                     except Exception as e:
@@ -333,40 +333,40 @@
                         p , im = next(points17.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                     except Exception as e:
                         logger.warning(f'Mixaug 4 problem : {e}')
             
             if temperature_change:
-                frac_data  = int(self.split * temperature_change_f)
+                frac_data  = round(self.split * temperature_change_f)
                 try:
                     if no_track <= frac_data:
                 
                         points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points2.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
 
                 except Exception as e:
                     logger.warning(f'Image temperature problem : {e}')
 
             if motionBlur:
-                frac_data  = int(self.split * motionBlur_f)
+                frac_data  = round(self.split * motionBlur_f)
                 try:
                     if no_track <= frac_data:
                         
                         points20  = executor.submit(self.augment.image_motionBlur,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points20.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                         
                 except Exception as e:
                     logger.warning(f'Image motion_blur problem : {e}')
 
 
             if weather_change:
-                frac_data  = int(self.split * weather_change_f)
+                frac_data  = round(self.split * weather_change_f)
                 try:
                     if no_track <= frac_data:
                         
                         points20  = executor.submit(self.augment.image_weatherChange,im_read,rect_on_image,image_height,image_width) 
                         p , im = next(points20.result())
                         utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
                         
@@ -518,15 +518,15 @@
             
         
         #shuffling all images
         random.shuffle(all_images)
         # checking how many images
         self.len_total_images = len(all_images)
         # spliting into training set
-        self.split = int(self.len_total_images * train_split)
+        self.split = round(self.len_total_images * train_split)
         
         console.print(f'[bold cyan] [+] Total images : {self.len_total_images}   |   Train Split : {self.split} images   |    Test split : {self.len_total_images-self.split} images [bold cyan]')
         
         if train_split == 1.0:
                     shutil.rmtree(f'{self.aug_save_folder_name}/test')
         
         # if c value less than equal to train split then we will add those images in training data and rest will go for test data
```

### Comparing `image_augs-2.3.10/object_detection_new/utils_poly.py` & `image_augs-2.3.11/object_detection_new/utils_poly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import uuid
 import cv2
 import os
 
-from numpyencoder import NumpyEncoder
-
 
 
 import instance_seg.logging_util as logging_util
 
 logger = logging_util.get_logger(os.path.basename(__file__).split('.')[0])
 
 def create_new_txt(image ,points,train_path_images , train_path_labels):
@@ -46,15 +44,15 @@
                         f.write('\n')
                     
                         
                     del new_name
             
             
     except Exception as e:
-            logger.warning(f'problem : create new json  desc : {e}')
+            logger.warning(f'problem : create new txt  desc : {e}')
 
 
 def convert_to_normal_bbox(yolo_bbox, image_width, image_height):
     """
     Convert YOLO's normalized bounding box coordinates to normal bounding box format.
     yolo_bbox: Tuple of (x, y, w, h) normalized bounding box coordinates from YOLO's output.
     image_width: Width of the input image.
```

### Comparing `image_augs-2.3.10/setup.py` & `image_augs-2.3.11/setup.py`

 * *Files identical despite different names*

