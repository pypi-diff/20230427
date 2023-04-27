# Comparing `tmp/DeepSlice-1.1.1.tar.gz` & `tmp/DeepSlice-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSlice-1.1.1.tar", last modified: Tue Apr 11 11:18:03 2023, max compression
+gzip compressed data, was "DeepSlice-1.1.2.tar", last modified: Thu Apr 27 09:58:21 2023, max compression
```

## Comparing `DeepSlice-1.1.1.tar` & `DeepSlice-1.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/setup.py
```

### Comparing `DeepSlice-1.1.1/DeepSlice/coord_post_processing/angle_methods.py` & `DeepSlice-1.1.2/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,17 @@
             min, max = 0, 528
         elif species == "rat":
             min, max = 0, 1024
         if len(df_center) > 2:
             weighted_accuracy = plane_alignment.make_gaussian_weights(max)
         else:
             weighted_accuracy = [1.0] * len(df_center)
+        df_center = np.array(df_center)
+        df_center[df_center < min] = min
+        df_center[df_center > max] = max-1
         weighted_accuracy = [weighted_accuracy[int(y)] for y in df_center]
         print(weighted_accuracy)
         DV_angle = np.average(DV_list, weights=weighted_accuracy)
         ML_angle = np.average(ML_list, weights=weighted_accuracy)
     else:
         raise ValueError("method must be one of 'mean' or 'weighted_mean'")
     return DV_angle, ML_angle
@@ -107,14 +110,15 @@
     if method == "weighted_mean":
         depths = calculate_brain_center_depths(
             df[["ox", "oy", "oz", "ux", "uy", "uz", "vx", "vy", "vz"]]
         )
     DV_angle, ML_angle = get_mean_angle(
         DV_angle_list, ML_angle_list, method, depths, species
     )
+    print(f"DV angle: {DV_angle}\nML angle: {ML_angle}")
     # adjust the angles for each section in the dataset
     df = set_angles(df, DV_angle, ML_angle)
     return df
 
 
 def set_angles(df, DV_angle, ML_angle):
     """
```

### Comparing `DeepSlice-1.1.1/DeepSlice/coord_post_processing/depth_estimation.py` & `DeepSlice-1.1.2/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     )
 
 
 
 def make_gaussian_weights(size):
     x = np.linspace(-np.pi, np.pi, size)
     weights = np.exp(-(x ** 2) / 2) / np.sqrt(2 * np.pi)
+    weights[weights>size-1] = size-1
+    weights[weights<0] = 0
     return weights
 
 
 def get_axis(m, translation_vector, direction, plane_of_section=None, atlas="AMBA"):
     """
     :param m: the matrix to rotate
     :type m: 3x3 :any:`numpy.ndarray`
```

### Comparing `DeepSlice-1.1.1/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `DeepSlice-1.1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/DeepSlice/main.py` & `DeepSlice-1.1.2/DeepSlice/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,18 +20,20 @@
         weights =    metadata_loader.get_data_path(self.config["weight_file_paths"][self.species]["primary"], self.metadata_path)
         self.model = neural_network.initialise_network(xception_weights, weights, self.species)
         
 
 
     def predict(
         self,
-        image_directory: str,
+        image_directory: str = None,
         ensemble: bool = None,
         section_numbers: bool = True,
         legacy_section_numbers=False,
+        image_list = None,
+        use_secondary_model = False,
     ):
         """predicts the atlas position for a folder full of histological brain sections
 
         :param image_directory: the directory containing the brain sections
         :type image_directory: str
         :param ensemble: whether to use multiple models, this will default to True when available, defaults to None
         :type ensemble: bool, optional
@@ -43,26 +45,48 @@
 
         # We set this to false as predict is the entry point for a new brain and therefore we need to reset all values which may persist from a previous animal.
         self.bad_sections_present = False
         # Different species may or may not have an ensemble model, so we need to check for this before defaulting to True
         if ensemble == None:
             ensemble = self.config["ensemble_status"][self.species]
             ensemble = eval(ensemble)
-
-        image_generator, width, height = neural_network.load_images(image_directory)
+        if image_list:
+            image_generator, width, height = neural_network.load_images_from_list(
+                image_list
+            )
+            if image_directory:
+                print(
+                    "WARNING: image_directory is set but image_list is also set. image_directory will be ignored."
+                )
+        else:
+            image_generator, width, height = neural_network.load_images_from_path(
+                image_directory
+            )
         primary_weights = metadata_loader.get_data_path(self.config["weight_file_paths"][self.species]["primary"], self.metadata_path)
  
         secondary_weights = metadata_loader.get_data_path(self.config["weight_file_paths"][self.species]["secondary"], self.metadata_path)
 
         if secondary_weights == "None":
             print(f"ensemble is not available for {self.species}")
+            if use_secondary_model:
+                print("WARNING: use_secondary_model is set but no secondary model is available. use_secondary_model will be ignored.")
+                use_secondary_model = False
             ensemble = False
-        predictions = neural_network.predictions_util(
-            self.model, image_generator, primary_weights, secondary_weights, ensemble
-        )
+        if use_secondary_model and ensemble:
+            print("WARNING: use_secondary_model is set but ensemble is also set. use_secondary_model will be ignored.")
+            use_secondary_model = False
+        if use_secondary_model:
+            print("Using secondary model")
+            predictions = neural_network.predictions_util(
+                self.model, image_generator, secondary_weights,None, ensemble
+            )
+        else:
+            predictions = neural_network.predictions_util(
+                self.model, image_generator, primary_weights, secondary_weights, ensemble
+            )
         predictions["width"] = width
         predictions["height"] = height
         if section_numbers:
             predictions["nr"] = spacing_and_indexing.number_sections(
                 predictions["Filenames"], legacy_section_numbers
             )
             predictions["nr"] = predictions["nr"].astype(int)
```

### Comparing `DeepSlice-1.1.1/DeepSlice/metadata/config.json` & `DeepSlice-1.1.2/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/DeepSlice/metadata/metadata_loader.py` & `DeepSlice-1.1.2/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/DeepSlice/neural_network/neural_network.py` & `DeepSlice-1.1.2/DeepSlice/neural_network/neural_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
     if weights != None:
         model.load_weights(weights)
     return model
 
 
 
-def load_images(image_path: str) -> np.ndarray:
+
+def load_images_from_path(image_path: str) -> np.ndarray:
     """
     Load the images from the given path
-
     :param image_path: The path to the images
     :type image_path: str
     :return: an Image generator for the found images
     :rtype: keras.preprocessing.image.ImageDataGenerator
     """
     if not os.path.isdir(image_path):
         raise ValueError("The path provided is not a directory")
@@ -90,21 +90,54 @@
             preprocessing_function=gray_scale, samplewise_std_normalization=True
         ).flow_from_dataframe(
             image_df,
             x_col="Filenames",
             y_col=None,
             target_size=(299, 299),
             batch_size=1,
-            
             colormode="rgb",
             shuffle=False,
             class_mode=None,
         )
     return image_generator, width, height
-
+    
+def load_images_from_list(image_list: list) -> np.ndarray:
+    """
+    Load the images from the given list
+    :param image_list: The list of images
+    :type image_list: list
+    :return: an Image generator for the found images
+    :rtype: keras.preprocessing.image.ImageDataGenerator
+    """
+    valid_formats = [".jpg", ".jpeg", ".png"]
+    images = [i for i in image_list if os.path.splitext(i)[1].lower() in valid_formats]
+    sizes = [get_image_size(i) for i in images]
+    width = [i[0] for i in sizes]
+    height = [i[1] for i in sizes]
+    if len(images) == 0:
+        raise ValueError(
+            f"No images found in the directory, please ensure image files are one of the following formats: {', '.join(valid_formats)}"
+        )
+    image_df = pd.DataFrame({"Filenames": images})
+    with warnings.catch_warnings():
+        ##throws warning about samplewise_std_normalization conflicting with samplewise_center which we don't use.
+        warnings.simplefilter("ignore")
+        image_generator = ImageDataGenerator(
+            preprocessing_function=gray_scale, samplewise_std_normalization=True
+        ).flow_from_dataframe(
+            image_df,
+            x_col="Filenames",
+            y_col=None,
+            target_size=(299, 299),
+            batch_size=1,
+            colormode="rgb",
+            shuffle=False,
+            class_mode=None,
+        )
+    return image_generator, width, height
 
 def predictions_util(
     model: Sequential,
     image_generator: ImageDataGenerator,
     primary_weights: str,
     secondary_weights: str,
     ensemble: bool = False,
```

### Comparing `DeepSlice-1.1.1/DeepSlice/read_and_write/QuickNII_functions.py` & `DeepSlice-1.1.2/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/DeepSlice.egg-info/PKG-INFO` & `DeepSlice-1.1.2/DeepSlice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.1.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.2.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.1 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.2 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.1.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.2.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.1/DeepSlice.egg-info/SOURCES.txt` & `DeepSlice-1.1.2/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/LICENSE` & `DeepSlice-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/PKG-INFO` & `DeepSlice-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.1.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.2.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.1 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.2 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.1.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.2.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.1/README.md` & `DeepSlice-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.1/setup.py` & `DeepSlice-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.1.1',
+    version='1.1.2',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.1.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.2.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow==1.15.0',
         'h5py==2.10.0',
```

