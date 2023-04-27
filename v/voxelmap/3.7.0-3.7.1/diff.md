# Comparing `tmp/voxelmap-3.7.0.tar.gz` & `tmp/voxelmap-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-3.7.0.tar", max compression
+gzip compressed data, was "voxelmap-3.7.1.tar", max compression
```

## Comparing `voxelmap-3.7.0.tar` & `voxelmap-3.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-3.7.0/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-3.7.0/README.md
--rw-r--r--   0        0        0      591 2023-04-26 18:14:30.951974 voxelmap-3.7.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-3.7.0/voxelmap/__init__.py
--rw-r--r--   0        0        0    17220 2023-03-31 17:25:56.067763 voxelmap-3.7.0/voxelmap/annex.py
--rwxr-xr-x   0        0        0    29140 2023-04-26 18:13:03.766171 voxelmap-3.7.0/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 voxelmap-3.7.0/setup.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 voxelmap-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-3.7.1/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-3.7.1/README.md
+-rw-r--r--   0        0        0      545 2023-04-27 03:49:34.502547 voxelmap-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-3.7.1/voxelmap/__init__.py
+-rw-r--r--   0        0        0    17220 2023-03-31 17:25:56.067763 voxelmap-3.7.1/voxelmap/annex.py
+-rwxr-xr-x   0        0        0    29140 2023-04-26 18:13:03.766171 voxelmap-3.7.1/voxelmap/jotunn.py
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 voxelmap-3.7.1/setup.py
+-rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 voxelmap-3.7.1/PKG-INFO
```

### Comparing `voxelmap-3.7.0/LICENSE` & `voxelmap-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-3.7.0/README.md` & `voxelmap-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-3.7.0/pyproject.toml` & `voxelmap-3.7.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "3.7.0"
+version = "3.7.1"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -13,14 +13,12 @@
 matplotlib = "^3.6.2"
 pandas = "^1.5.2"
 opencv-python = "^4.7.0.68"
 scipy = "^1.10.0"
 scikit-image = "^0.19.3"
 pyvista = "^0.38.2"
 colorcet = "^3.0.1"
-sphinx = "^6.1.3"
-sphinx-rtd-theme = "^1.2.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `voxelmap-3.7.0/voxelmap/annex.py` & `voxelmap-3.7.1/voxelmap/annex.py`

 * *Files identical despite different names*

### Comparing `voxelmap-3.7.0/voxelmap/jotunn.py` & `voxelmap-3.7.1/voxelmap/jotunn.py`

 * *Files identical despite different names*

### Comparing `voxelmap-3.7.0/setup.py` & `voxelmap-3.7.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,19 @@
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
  'opencv-python>=4.7.0.68,<5.0.0.0',
  'pandas>=1.5.2,<2.0.0',
  'pytest>=7.2.0,<8.0.0',
  'pyvista>=0.38.2,<0.39.0',
  'scikit-image>=0.19.3,<0.20.0',
- 'scipy>=1.10.0,<2.0.0',
- 'sphinx-rtd-theme>=1.2.0,<2.0.0',
- 'sphinx>=6.1.3,<7.0.0']
+ 'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '3.7.0',
+    'version': '3.7.1',
     'description': 'A Python library for making voxel and 3D models from NumPy arrays.',
     'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making voxel and three-dimensional models from NumPy arrays. \n\n<a href="https://voxelmap.readthedocs.io/en/latest/">\n<img src="https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true" width="250"></a>\n\n## Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n\n## Just starting? Remote Usage with a Colab notebook (click below)\n\n<a href="https://colab.research.google.com/drive/1RMEMgZHlk_tKAzfS4QfXLJV9joDgdh8N?usp=sharing">\n<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/colaboratory.png" width="500" ></a>\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is free software. It comes without any warranty, to the extent permitted by applicable law. You can redistribute it and/or modify it under the terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.\n\n**[MIT license](./LICENSE)** Copyright 2022 © <a href="https://github.com/andrewrgarcia" target="_blank">Andrew Garcia</a>.\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
 python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.2.0,<8.0.0',
 'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
-'scipy>=1.10.0,<2.0.0', 'sphinx-rtd-theme>=1.2.0,<2.0.0',
-'sphinx>=6.1.3,<7.0.0'] setup_kwargs = { 'name': 'voxelmap', 'version':
-'3.7.0', 'description': 'A Python library for making voxel and 3D models from
+'scipy>=1.10.0,<2.0.0'] setup_kwargs = { 'name': 'voxelmap', 'version':
+'3.7.1', 'description': 'A Python library for making voxel and 3D models from
 NumPy arrays.', 'long_description': '# voxelmap\n\n[![License](http://
 img.shields.io/:license-mit-blue.svg?style=flat-square)](https://
 raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
 [Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
 Python library for making voxel and three-dimensional models from NumPy arrays.
 \n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
```

### Comparing `voxelmap-3.7.0/PKG-INFO` & `voxelmap-3.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 3.7.0
+Version: 3.7.1
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,16 +17,14 @@
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: pyvista (>=0.38.2,<0.39.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: sphinx (>=6.1.3,<7.0.0)
-Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # voxelmap
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 3.7.0 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 3.7.1 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
 (>=3.6.2,<4.0.0) Requires-Dist: numpy (>=1.24.1,<2.0.0) Requires-Dist: opencv-
 python (>=4.7.0.68,<5.0.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-
 Dist: pytest (>=7.2.0,<8.0.0) Requires-Dist: pyvista (>=0.38.2,<0.39.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0) Requires-Dist: scipy
-(>=1.10.0,<2.0.0) Requires-Dist: sphinx (>=6.1.3,<7.0.0) Requires-Dist: sphinx-
-rtd-theme (>=1.2.0,<2.0.0) Description-Content-Type: text/markdown # voxelmap
-[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
+(>=1.10.0,<2.0.0) Description-Content-Type: text/markdown # voxelmap [!
+[License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
 (https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE) [!
 [Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest) A
 Python library for making voxel and three-dimensional models from NumPy arrays.
 [https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true] ##
 Installation and Local Usage ```ruby pip install voxelmap ``` It is recommended
 you run voxelmap using a `virtualenv` virtual environment. To do so, follow the
```

