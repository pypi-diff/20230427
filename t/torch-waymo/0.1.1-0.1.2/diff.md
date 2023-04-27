# Comparing `tmp/torch_waymo-0.1.1.tar.gz` & `tmp/torch_waymo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_waymo-0.1.1.tar", last modified: Tue Jan 31 18:47:53 2023, max compression
+gzip compressed data, was "torch_waymo-0.1.2.tar", last modified: Thu Apr 27 01:38:50 2023, max compression
```

## Comparing `torch_waymo-0.1.1.tar` & `torch_waymo-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/
--rw-r--r--   0 william   (1000) william   (1000)     1078 2023-01-31 16:43:26.000000 torch_waymo-0.1.1/LICENSE
--rw-r--r--   0 william   (1000) william   (1000)     2082 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)     1507 2023-01-31 18:47:44.000000 torch_waymo-0.1.1/README.md
--rw-r--r--   0 william   (1000) william   (1000)      833 2023-01-31 18:47:44.000000 torch_waymo-0.1.1/pyproject.toml
--rw-r--r--   0 william   (1000) william   (1000)       38 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/setup.cfg
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/src/
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/src/torch_waymo/
--rw-r--r--   0 william   (1000) william   (1000)      102 2023-01-31 18:05:50.000000 torch_waymo-0.1.1/src/torch_waymo/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)     3449 2023-01-31 18:19:13.000000 torch_waymo-0.1.1/src/torch_waymo/convert_waymo.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/src/torch_waymo/dataset/
--rw-r--r--   0 william   (1000) william   (1000)        0 2023-01-11 14:53:42.000000 torch_waymo-0.1.1/src/torch_waymo/dataset/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)      355 2023-01-31 18:09:13.000000 torch_waymo-0.1.1/src/torch_waymo/dataset/simplified_frame.py
--rw-r--r--   0 william   (1000) william   (1000)     1296 2023-01-31 18:09:13.000000 torch_waymo-0.1.1/src/torch_waymo/dataset/waymo_dataset.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/src/torch_waymo/protocol/
--rw-r--r--   0 william   (1000) william   (1000)        0 2023-01-10 18:59:44.000000 torch_waymo-0.1.1/src/torch_waymo/protocol/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)     4456 2023-01-31 18:09:13.000000 torch_waymo-0.1.1/src/torch_waymo/protocol/dataset_proto.py
--rw-r--r--   0 william   (1000) william   (1000)     1753 2023-01-31 18:09:13.000000 torch_waymo-0.1.1/src/torch_waymo/protocol/keypoint_proto.py
--rw-r--r--   0 william   (1000) william   (1000)     1647 2023-01-31 18:09:13.000000 torch_waymo-0.1.1/src/torch_waymo/protocol/label_proto.py
--rw-r--r--   0 william   (1000) william   (1000)      281 2023-01-24 23:52:49.000000 torch_waymo-0.1.1/src/torch_waymo/protocol/utils.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-01-31 18:47:53.660065 torch_waymo-0.1.1/src/torch_waymo.egg-info/
--rw-r--r--   0 william   (1000) william   (1000)     2082 2023-01-31 18:47:53.000000 torch_waymo-0.1.1/src/torch_waymo.egg-info/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)      646 2023-01-31 18:47:53.000000 torch_waymo-0.1.1/src/torch_waymo.egg-info/SOURCES.txt
--rw-r--r--   0 william   (1000) william   (1000)        1 2023-01-31 18:47:53.000000 torch_waymo-0.1.1/src/torch_waymo.egg-info/dependency_links.txt
--rw-r--r--   0 william   (1000) william   (1000)       71 2023-01-31 18:47:53.000000 torch_waymo-0.1.1/src/torch_waymo.egg-info/entry_points.txt
--rw-r--r--   0 william   (1000) william   (1000)       54 2023-01-31 18:47:53.000000 torch_waymo-0.1.1/src/torch_waymo.egg-info/requires.txt
--rw-r--r--   0 william   (1000) william   (1000)       12 2023-01-31 18:47:53.000000 torch_waymo-0.1.1/src/torch_waymo.egg-info/top_level.txt
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/
+-rw-r--r--   0 william   (1000) william   (1000)     1078 2023-01-31 16:43:26.000000 torch_waymo-0.1.2/LICENSE
+-rw-r--r--   0 william   (1000) william   (1000)     2082 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/PKG-INFO
+-rw-r--r--   0 william   (1000) william   (1000)     1507 2023-01-31 18:53:42.000000 torch_waymo-0.1.2/README.md
+-rw-r--r--   0 william   (1000) william   (1000)      853 2023-04-27 01:38:42.000000 torch_waymo-0.1.2/pyproject.toml
+-rw-r--r--   0 william   (1000) william   (1000)       38 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/setup.cfg
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/src/
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/src/torch_waymo/
+-rw-r--r--   0 william   (1000) william   (1000)      102 2023-01-31 18:05:50.000000 torch_waymo-0.1.2/src/torch_waymo/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)     3449 2023-01-31 18:19:13.000000 torch_waymo-0.1.2/src/torch_waymo/convert_waymo.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/src/torch_waymo/dataset/
+-rw-r--r--   0 william   (1000) william   (1000)        0 2023-01-11 14:53:42.000000 torch_waymo-0.1.2/src/torch_waymo/dataset/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)      355 2023-01-31 18:09:13.000000 torch_waymo-0.1.2/src/torch_waymo/dataset/simplified_frame.py
+-rw-r--r--   0 william   (1000) william   (1000)     1296 2023-01-31 18:09:13.000000 torch_waymo-0.1.2/src/torch_waymo/dataset/waymo_dataset.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/src/torch_waymo/protocol/
+-rw-r--r--   0 william   (1000) william   (1000)        0 2023-01-10 18:59:44.000000 torch_waymo-0.1.2/src/torch_waymo/protocol/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)     4456 2023-01-31 18:09:13.000000 torch_waymo-0.1.2/src/torch_waymo/protocol/dataset_proto.py
+-rw-r--r--   0 william   (1000) william   (1000)     1753 2023-01-31 18:09:13.000000 torch_waymo-0.1.2/src/torch_waymo/protocol/keypoint_proto.py
+-rw-r--r--   0 william   (1000) william   (1000)     1647 2023-01-31 18:09:13.000000 torch_waymo-0.1.2/src/torch_waymo/protocol/label_proto.py
+-rw-r--r--   0 william   (1000) william   (1000)      281 2023-01-24 23:52:49.000000 torch_waymo-0.1.2/src/torch_waymo/protocol/utils.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 01:38:50.465176 torch_waymo-0.1.2/src/torch_waymo.egg-info/
+-rw-r--r--   0 william   (1000) william   (1000)     2082 2023-04-27 01:38:50.000000 torch_waymo-0.1.2/src/torch_waymo.egg-info/PKG-INFO
+-rw-r--r--   0 william   (1000) william   (1000)      646 2023-04-27 01:38:50.000000 torch_waymo-0.1.2/src/torch_waymo.egg-info/SOURCES.txt
+-rw-r--r--   0 william   (1000) william   (1000)        1 2023-04-27 01:38:50.000000 torch_waymo-0.1.2/src/torch_waymo.egg-info/dependency_links.txt
+-rw-r--r--   0 william   (1000) william   (1000)       71 2023-04-27 01:38:50.000000 torch_waymo-0.1.2/src/torch_waymo.egg-info/entry_points.txt
+-rw-r--r--   0 william   (1000) william   (1000)       71 2023-04-27 01:38:50.000000 torch_waymo-0.1.2/src/torch_waymo.egg-info/requires.txt
+-rw-r--r--   0 william   (1000) william   (1000)       12 2023-04-27 01:38:50.000000 torch_waymo-0.1.2/src/torch_waymo.egg-info/top_level.txt
```

### Comparing `torch_waymo-0.1.1/LICENSE` & `torch_waymo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.1/PKG-INFO` & `torch_waymo-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_waymo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Load Waymo Open Dataset in PyTorch
 Author-email: William Guimont-Martin <william.guimont-martin.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/willGuimont/torch_waymo
 Project-URL: Bug Tracker, https://github.com/willGuimont/torch_waymo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 # torch_waymo
 
 Load Waymo Open Dataset in PyTorch
 
 Cite this repository:
 ```
-@software{Guimont-Martin_A_PyTorch_dataloader_2022,
+@software{Guimont-Martin_A_PyTorch_dataloader_2023,
     author = {Guimont-Martin, William},
     month = {1},
     title = {{A PyTorch dataloader for Waymo Open Dataset}},
     version = {0.1.1},
     year = {2023}
 }
 ```
```

### Comparing `torch_waymo-0.1.1/README.md` & `torch_waymo-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # torch_waymo
 
 Load Waymo Open Dataset in PyTorch
 
 Cite this repository:
 ```
-@software{Guimont-Martin_A_PyTorch_dataloader_2022,
+@software{Guimont-Martin_A_PyTorch_dataloader_2023,
     author = {Guimont-Martin, William},
     month = {1},
     title = {{A PyTorch dataloader for Waymo Open Dataset}},
     version = {0.1.1},
     year = {2023}
 }
 ```
```

### Comparing `torch_waymo-0.1.1/pyproject.toml` & `torch_waymo-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "torch_waymo"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "William Guimont-Martin", email = "william.guimont-martin.1@ulaval.ca" },
 ]
 description = "Load Waymo Open Dataset in PyTorch"
 readme = "README.md"
 requires-python = ">=3.7,<3.10"
 dependencies = [
@@ -17,13 +17,13 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.optional-dependencies]
-waymo = ["waymo-open-dataset-tf-2-6-0"]
+waymo = ["waymo-open-dataset-tf-2-6-0", "protobuf==3.20.0"]
 [project.urls]
 "Homepage" = "https://github.com/willGuimont/torch_waymo"
 "Bug Tracker" = "https://github.com/willGuimont/torch_waymo/issues"
 [project.scripts]
 torch-waymo-convert = "torch_waymo.convert_waymo:main"
```

### Comparing `torch_waymo-0.1.1/src/torch_waymo/convert_waymo.py` & `torch_waymo-0.1.2/src/torch_waymo/convert_waymo.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.1/src/torch_waymo/dataset/waymo_dataset.py` & `torch_waymo-0.1.2/src/torch_waymo/dataset/waymo_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.1/src/torch_waymo/protocol/dataset_proto.py` & `torch_waymo-0.1.2/src/torch_waymo/protocol/dataset_proto.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.1/src/torch_waymo/protocol/keypoint_proto.py` & `torch_waymo-0.1.2/src/torch_waymo/protocol/keypoint_proto.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.1/src/torch_waymo/protocol/label_proto.py` & `torch_waymo-0.1.2/src/torch_waymo/protocol/label_proto.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.1/src/torch_waymo.egg-info/PKG-INFO` & `torch_waymo-0.1.2/src/torch_waymo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-waymo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Load Waymo Open Dataset in PyTorch
 Author-email: William Guimont-Martin <william.guimont-martin.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/willGuimont/torch_waymo
 Project-URL: Bug Tracker, https://github.com/willGuimont/torch_waymo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 # torch_waymo
 
 Load Waymo Open Dataset in PyTorch
 
 Cite this repository:
 ```
-@software{Guimont-Martin_A_PyTorch_dataloader_2022,
+@software{Guimont-Martin_A_PyTorch_dataloader_2023,
     author = {Guimont-Martin, William},
     month = {1},
     title = {{A PyTorch dataloader for Waymo Open Dataset}},
     version = {0.1.1},
     year = {2023}
 }
 ```
```

### Comparing `torch_waymo-0.1.1/src/torch_waymo.egg-info/SOURCES.txt` & `torch_waymo-0.1.2/src/torch_waymo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

