# Comparing `tmp/ampy-0.1.1.tar.gz` & `tmp/ampy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampy-0.1.1.tar", last modified: Fri Apr 14 15:37:14 2023, max compression
+gzip compressed data, was "ampy-0.1.2.tar", last modified: Thu Apr 27 18:48:01 2023, max compression
```

## Comparing `ampy-0.1.1.tar` & `ampy-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11990 2023-04-14 15:36:54.343139 ampy-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-14 15:36:54.343139 ampy-0.1.1/ampy/__init__.py
--rw-r--r--   0        0        0    15955 2023-04-14 15:36:54.343139 ampy-0.1.1/ampy/processing.py
--rw-r--r--   0        0        0     8994 2023-04-14 15:36:54.343139 ampy-0.1.1/ampy/statistics2d.py
--rw-r--r--   0        0        0     6265 2023-04-14 15:36:54.343139 ampy-0.1.1/ampy/statistics3d.py
--rw-r--r--   0        0        0     1284 2023-04-14 15:36:54.343139 ampy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13204 1970-01-01 00:00:00.000000 ampy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    12256 2023-04-27 18:47:47.886134 ampy-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 18:47:47.886134 ampy-0.1.2/ampy/__init__.py
+-rw-r--r--   0        0        0    17616 2023-04-27 18:47:47.886134 ampy-0.1.2/ampy/processing.py
+-rw-r--r--   0        0        0     9129 2023-04-27 18:47:47.886134 ampy-0.1.2/ampy/statistics2d.py
+-rw-r--r--   0        0        0     6265 2023-04-27 18:47:47.886134 ampy-0.1.2/ampy/statistics3d.py
+-rw-r--r--   0        0        0     1263 2023-04-27 18:47:47.886134 ampy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13441 1970-01-01 00:00:00.000000 ampy-0.1.2/PKG-INFO
```

### Comparing `ampy-0.1.1/README.md` & `ampy-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-[pypi-version-image]: https://badge.fury.io/py/ampy.svg
+[pypi-version-image]: https://badge.fury.io/py/ampy.svg?
 [pypi-version-url]: https://badge.fury.io/py/ampy
 
-[linting-image]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml/badge.svg
-[linting-url]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml
-
 [docs-image]: https://readthedocs.org/projects/ampy/badge/?version=latest
 [docs-url]: https://ampy.readthedocs.io/en/latest
 
+[linting-image]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml/badge.svg
+[linting-url]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml
+
 [coverage-image]: https://coveralls.io/repos/github/swarmtronics/AMPy/badge.svg?service=github&kill_cache=0
 [coverage-url]: https://coveralls.io/github/swarmtronics/AMPy
 
+[pypi-license-image]: https://img.shields.io/pypi/l/ampy
+
 ![Pipeline_image](materials/logo_header_bl_font.png#gh-light-mode-only)
 ![Pipeline_image](materials/logo_header_wh_font.png#gh-dark-mode-only)
 
 
+[![Python](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org)
 [![PyPI version][pypi-version-image]][pypi-version-url]
-[![Linting Status][linting-image]][linting-url]
-[![Coverage Status][coverage-image]][coverage-url]
 [![Docs Status][docs-image]][docs-url]
+[![Coverage Status][coverage-image]][coverage-url]
+[![Linting Status][linting-image]][linting-url]
+![PyPI - License][pypi-license-image]
 
-
-**[Website](swarmtronics.com)** (TBD) | **[Documentation](https://ampy.readthedocs.io/en/latest/)** | **[Paper](TBD)** (TBD) | **[Video Tutorial](TBD)** (TBD) | **[Colab Notebook](TBD)** (TBD)
+**[Website](swarmtronics.com)** (TBD) | **[Documentation](https://ampy.readthedocs.io/en/latest/)** | **[Paper](TBD)** (TBD) | **[Video Tutorial](TBD)** (TBD) | **[Colab Notebook](https://colab.research.google.com/drive/1hiCGXoDtOEO3LOm6RG12111Kiwofh069?usp=sharing)**
 
 **AMPy** is a *baseline* library built upon [OpenCV](https://opencv.org/) and [NumPy](https://numpy.org/) to easily process experimental video data for active matter and disordered systems. Our library turns the processing of experiment recordings into a cakewalk, considerably accelerating extraction of system dynamics.
 
 # Library content
 
 - [Overview](#overview)  
 - [Processing](#processing)
```

### Comparing `ampy-0.1.1/ampy/statistics2d.py` & `ampy-0.1.2/ampy/statistics2d.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 
 
 RAD2DEG = 180 / np.pi
 DEG2RAD = np.pi / 180
 
 
-def _orientation_angles(kinematics: list) -> list:
+def _orientation_angles(kinematics: list) -> list: # pragma: no cover
     angles = list(np.array(kinematics, dtype=object)[:, :, 1])
     return angles
 
 
 def _positions(kinematics: list) -> list:
     positions = list(np.array(kinematics, dtype=object)[:, :, 2])
     return positions
@@ -88,20 +88,20 @@
     """
 
     angles = _polar_angles(kinematics)
     mean_angles_raw = np.array(angles, dtype=float).mean(axis=1)
     mean_angles_corrected = [mean_angles_raw[0]]
     for i_frame in range(1, len(mean_angles_raw)):
         difference = mean_angles_raw[i_frame] - mean_angles_raw[i_frame - 1]
-        if abs(difference) < 100:
+        if abs(difference) < 100: # pragma: no cover
             mean_angles_corrected.append(mean_angles_corrected[-1] + difference)
         else:
-            if difference > 0:
+            if difference > 0: # pragma: no cover
                 mean_angles_corrected.append(mean_angles_corrected[-1] + difference - 360)
-            else:
+            else: # pragma: no cover
                 mean_angles_corrected.append(mean_angles_corrected[-1] - difference + 360)
     return mean_angles_corrected
 
 
 def mean_polar_angle_absolute(kinematics: list):
     """
     Returns average particles' polar angle for each frame. Angle for certain frame calculating
@@ -112,17 +112,17 @@
     """
 
     angles = _polar_angles(kinematics)
     mean_angles_raw = np.array(angles, dtype=float).mean(axis=1)
     mean_angles_accumulated = [mean_angles_raw[0]]
     for i_frame in range(1, len(mean_angles_raw)):
         absolute_difference = abs(mean_angles_raw[i_frame] - mean_angles_raw[i_frame - 1])
-        if absolute_difference < 100:
+        if absolute_difference < 100: # pragma: no cover
             mean_angles_accumulated.append(mean_angles_accumulated[-1] + absolute_difference)
-        else:
+        else: # pragma: no cover
             mean_angles_accumulated.append(mean_angles_accumulated[-1] - absolute_difference + 360)
     return mean_angles_accumulated
 
 
 def mean_cartesian_displacements(kinematics: list):
     """
     Returns average particles' cartesian displacement for each frame
@@ -207,20 +207,19 @@
                                        kinematics[i_frame][i_bot][2]) >= 0)
         q /= N
         q_sequence.append(q)
     t_corr = N * np.std(q_sequence)
     return t_corr
 
 
-def _is_collide(bot_1: list, bot_2: list) -> bool:  # pragma: no cover
-    D = 300
-    return calc_distance(bot_1[2], bot_2[2]) <= D
+def _is_collide(bot_1: list, bot_2: list, d: int = 300) -> bool:  # pragma: no cover
+    return calc_distance(bot_1[2], bot_2[2]) <= d
 
 
-def _adjacency_matrix(kinematics_frame: list, collide_function) -> list:
+def _adjacency_matrix(kinematics_frame: list, collide_function) -> list: # pragma: no cover
     N = len(kinematics_frame)
     adj_matrix = [[0 for i in range(N)] for j in range(N)]
     for i_bot in range(N):
         for j_bot in range(N):
             if i_bot == j_bot:
                 continue
             adj_matrix[i_bot][j_bot] = \
```

### Comparing `ampy-0.1.1/ampy/statistics3d.py` & `ampy-0.1.2/ampy/statistics3d.py`

 * *Files identical despite different names*

### Comparing `ampy-0.1.1/pyproject.toml` & `ampy-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="ampy"
-version="0.1.1"
+version="0.1.2"
 authors=[
     {name="Vadim Porvatov", email="eighonet@gmail.com"},
     {name="Mikhail Buzakov", email="m.k.buzakov@gmail.com"}
 ]
 description="Python-based Processing Tool for Active Matter Experiments"
 readme="README.md"
 requires-python=">=3.8"
@@ -25,23 +25,22 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies=[
-    "numpy==1.24.2",
-    "matplotlib==3.7.1",
-    "scipy==1.10.1",
-    "ffmpeg-python==0.2.0",
+    "numpy<=1.21.6",
+    "matplotlib>=3.7.1",
+    "ffmpeg-python>=0.2.0",
     "opencv-contrib-python==4.6.0.66",
-    "imageio-ffmpeg==0.4.8",
-    "imutils==0.5.4",
-    "celluloid==0.2.0",
-    "imageio==2.27.0",
+    "imageio-ffmpeg>=0.4.8",
+    "imutils>=0.5.4",
+    "celluloid>=0.2.0",
+    "imageio>=2.27.0",
 ]
 
 [project.urls]
 homepage="https://swarmtronics.com"
 documentation="https://ampy.readthedocs.io"
 repository="https://github.com/swarmtronics/AMPy.git"
```

### Comparing `ampy-0.1.1/PKG-INFO` & `ampy-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 Metadata-Version: 2.1
 Name: ampy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python-based Processing Tool for Active Matter Experiments
 Keywords: active-matter,disordered-systems,swarm-robotics,order-parameter,correlation-map
 Author-email: Vadim Porvatov <eighonet@gmail.com>, Mikhail Buzakov <m.k.buzakov@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: numpy==1.24.2
-Requires-Dist: matplotlib==3.7.1
-Requires-Dist: scipy==1.10.1
-Requires-Dist: ffmpeg-python==0.2.0
+Requires-Dist: numpy<=1.21.6
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: ffmpeg-python>=0.2.0
 Requires-Dist: opencv-contrib-python==4.6.0.66
-Requires-Dist: imageio-ffmpeg==0.4.8
-Requires-Dist: imutils==0.5.4
-Requires-Dist: celluloid==0.2.0
-Requires-Dist: imageio==2.27.0
+Requires-Dist: imageio-ffmpeg>=0.4.8
+Requires-Dist: imutils>=0.5.4
+Requires-Dist: celluloid>=0.2.0
+Requires-Dist: imageio>=2.27.0
 Project-URL: documentation, https://ampy.readthedocs.io
 Project-URL: homepage, https://swarmtronics.com
 Project-URL: repository, https://github.com/swarmtronics/AMPy.git
 
-[pypi-version-image]: https://badge.fury.io/py/ampy.svg
+[pypi-version-image]: https://badge.fury.io/py/ampy.svg?
 [pypi-version-url]: https://badge.fury.io/py/ampy
 
-[linting-image]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml/badge.svg
-[linting-url]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml
-
 [docs-image]: https://readthedocs.org/projects/ampy/badge/?version=latest
 [docs-url]: https://ampy.readthedocs.io/en/latest
 
+[linting-image]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml/badge.svg
+[linting-url]: https://github.com/swarmtronics/AMPy/actions/workflows/pylint.yml
+
 [coverage-image]: https://coveralls.io/repos/github/swarmtronics/AMPy/badge.svg?service=github&kill_cache=0
 [coverage-url]: https://coveralls.io/github/swarmtronics/AMPy
 
+[pypi-license-image]: https://img.shields.io/pypi/l/ampy
+
 ![Pipeline_image](materials/logo_header_bl_font.png#gh-light-mode-only)
 ![Pipeline_image](materials/logo_header_wh_font.png#gh-dark-mode-only)
 
 
+[![Python](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org)
 [![PyPI version][pypi-version-image]][pypi-version-url]
-[![Linting Status][linting-image]][linting-url]
-[![Coverage Status][coverage-image]][coverage-url]
 [![Docs Status][docs-image]][docs-url]
+[![Coverage Status][coverage-image]][coverage-url]
+[![Linting Status][linting-image]][linting-url]
+![PyPI - License][pypi-license-image]
 
-
-**[Website](swarmtronics.com)** (TBD) | **[Documentation](https://ampy.readthedocs.io/en/latest/)** | **[Paper](TBD)** (TBD) | **[Video Tutorial](TBD)** (TBD) | **[Colab Notebook](TBD)** (TBD)
+**[Website](swarmtronics.com)** (TBD) | **[Documentation](https://ampy.readthedocs.io/en/latest/)** | **[Paper](TBD)** (TBD) | **[Video Tutorial](TBD)** (TBD) | **[Colab Notebook](https://colab.research.google.com/drive/1hiCGXoDtOEO3LOm6RG12111Kiwofh069?usp=sharing)**
 
 **AMPy** is a *baseline* library built upon [OpenCV](https://opencv.org/) and [NumPy](https://numpy.org/) to easily process experimental video data for active matter and disordered systems. Our library turns the processing of experiment recordings into a cakewalk, considerably accelerating extraction of system dynamics.
 
 # Library content
 
 - [Overview](#overview)  
 - [Processing](#processing)
```

