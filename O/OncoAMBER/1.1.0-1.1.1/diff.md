# Comparing `tmp/OncoAMBER-1.1.0.tar.gz` & `tmp/OncoAMBER-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.1.0.tar", last modified: Fri Apr 21 20:53:01 2023, max compression
+gzip compressed data, was "OncoAMBER-1.1.1.tar", last modified: Thu Apr 27 16:58:20 2023, max compression
```

## Comparing `OncoAMBER-1.1.0.tar` & `OncoAMBER-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 20:53:01.675457 OncoAMBER-1.1.0/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 20:53:01.657758 OncoAMBER-1.1.0/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2381 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      579 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-04-21 20:53:01.000000 OncoAMBER-1.1.0/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2381 2023-04-21 20:53:01.675158 OncoAMBER-1.1.0/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     1626 2023-04-21 20:48:33.000000 OncoAMBER-1.1.0/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-21 20:53:01.674000 OncoAMBER-1.1.0/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6025 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5291 2023-04-21 20:10:54.000000 OncoAMBER-1.1.0/amber/CONFIG_default.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     1784 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    20986 2023-04-21 20:25:50.000000 OncoAMBER-1.1.0/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.1.0/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      760 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/RunTopas.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14142 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6181 2023-04-21 17:44:48.000000 OncoAMBER-1.1.0/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    21181 2023-04-21 20:26:24.000000 OncoAMBER-1.1.0/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      597 2023-04-21 19:40:53.000000 OncoAMBER-1.1.0/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      104 2023-04-21 19:20:43.000000 OncoAMBER-1.1.0/amber/config_instance.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.1.0/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-21 20:53:01.675580 OncoAMBER-1.1.0/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-04-21 20:48:56.000000 OncoAMBER-1.1.0/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-27 16:58:20.909339 OncoAMBER-1.1.1/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-27 16:58:20.889481 OncoAMBER-1.1.1/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      554 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-04-27 16:58:20.000000 OncoAMBER-1.1.1/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-04-27 16:58:20.909034 OncoAMBER-1.1.1/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-04-27 16:58:20.907870 OncoAMBER-1.1.1/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5291 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/CONFIG_default.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    21348 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.1.1/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      719 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/RunTopas.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14247 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5487 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    21482 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      332 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      326 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.1.1/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-04-27 16:58:20.909422 OncoAMBER-1.1.1/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3009 2023-04-27 16:58:04.000000 OncoAMBER-1.1.1/setup.py
```

### Comparing `OncoAMBER-1.1.0/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.1.1/OncoAMBER.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.1.0
+Version: 1.1.1
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -31,20 +31,37 @@
 This helps to mimic chronic hypoxia. As the tumor grows, it can block and destroy the vasculature, leading to acute hypoxia.
 In response, hypoxia triggers VEGF production and subsequent angiogenesis towards the tumor.
 The angiogenesis process is based on a directed random walk that takes crowding and the VEGF gradient into account.
 
 High crowding or pressure can lead to long-lasting hypoxia of cells and eventually result in their necrosis. 
 We'll integrate the radiation effects on individual cells using the simple interface provided by TOPAS and TOPAS-nBio, as well as other in-house DNA damage and DNA repair models.
 
-## Structure
+## Installation
 
-import amber 
+Download the github repository and run the following command in the main directory:
 
-amber.World(--)
-amber.Cell(--)
-amber.Voxel(--)
-amber.Vessel(--)
-amber.VesselNetwork(--)
-amber.Simulator(--)
+github: https://github.com/lvkunz/OncoAMBER
+
+PyPi: https://pypi.org/project/OncoAMBER/
+
+
+sh install.sh 
+
+## Usage
+
+import amber
+
+amber.World(-)
+amber.Cell(-)
+amber.Voxel(-)
+amber.Vessel(-)
+amber.VesselNetwork(-)
+amber.Simulator(-)
 etc. 
 
-example on github
+run example.py in the same directory as any CONFIG files you want to use using the following command:
+
+python example.py CONFIG 
+
+or on the cluster use:
+
+bash run_AMBER.sh example.py <n_iter> CONFIG
```

### Comparing `OncoAMBER-1.1.0/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.1.1/OncoAMBER.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,10 +16,9 @@
 amber/ScalarField.py
 amber/Terminal.py
 amber/Vessel.py
 amber/Voxel.py
 amber/World.py
 amber/__init__.py
 amber/config.py
-amber/config_instance.py
 amber/save_alpha_dataframe6.csv
 amber/save_beta_dataframe6.csv
```

### Comparing `OncoAMBER-1.1.0/PKG-INFO` & `OncoAMBER-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.1.0
+Version: 1.1.1
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -31,20 +31,37 @@
 This helps to mimic chronic hypoxia. As the tumor grows, it can block and destroy the vasculature, leading to acute hypoxia.
 In response, hypoxia triggers VEGF production and subsequent angiogenesis towards the tumor.
 The angiogenesis process is based on a directed random walk that takes crowding and the VEGF gradient into account.
 
 High crowding or pressure can lead to long-lasting hypoxia of cells and eventually result in their necrosis. 
 We'll integrate the radiation effects on individual cells using the simple interface provided by TOPAS and TOPAS-nBio, as well as other in-house DNA damage and DNA repair models.
 
-## Structure
+## Installation
 
-import amber 
+Download the github repository and run the following command in the main directory:
 
-amber.World(--)
-amber.Cell(--)
-amber.Voxel(--)
-amber.Vessel(--)
-amber.VesselNetwork(--)
-amber.Simulator(--)
+github: https://github.com/lvkunz/OncoAMBER
+
+PyPi: https://pypi.org/project/OncoAMBER/
+
+
+sh install.sh 
+
+## Usage
+
+import amber
+
+amber.World(-)
+amber.Cell(-)
+amber.Voxel(-)
+amber.Vessel(-)
+amber.VesselNetwork(-)
+amber.Simulator(-)
 etc. 
 
-example on github
+run example.py in the same directory as any CONFIG files you want to use using the following command:
+
+python example.py CONFIG 
+
+or on the cluster use:
+
+bash run_AMBER.sh example.py <n_iter> CONFIG
```

### Comparing `OncoAMBER-1.1.0/README.md` & `OncoAMBER-1.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,37 @@
 This helps to mimic chronic hypoxia. As the tumor grows, it can block and destroy the vasculature, leading to acute hypoxia.
 In response, hypoxia triggers VEGF production and subsequent angiogenesis towards the tumor.
 The angiogenesis process is based on a directed random walk that takes crowding and the VEGF gradient into account.
 
 High crowding or pressure can lead to long-lasting hypoxia of cells and eventually result in their necrosis. 
 We'll integrate the radiation effects on individual cells using the simple interface provided by TOPAS and TOPAS-nBio, as well as other in-house DNA damage and DNA repair models.
 
-## Structure
+## Installation
 
-import amber 
+Download the github repository and run the following command in the main directory:
 
-amber.World(--)
-amber.Cell(--)
-amber.Voxel(--)
-amber.Vessel(--)
-amber.VesselNetwork(--)
-amber.Simulator(--)
+github: https://github.com/lvkunz/OncoAMBER
+
+PyPi: https://pypi.org/project/OncoAMBER/
+
+
+sh install.sh 
+
+## Usage
+
+import amber
+
+amber.World(-)
+amber.Cell(-)
+amber.Voxel(-)
+amber.Vessel(-)
+amber.VesselNetwork(-)
+amber.Simulator(-)
 etc. 
 
-example on github
+run example.py in the same directory as any CONFIG files you want to use using the following command:
+
+python example.py CONFIG 
+
+or on the cluster use:
+
+bash run_AMBER.sh example.py <n_iter> CONFIG
```

### Comparing `OncoAMBER-1.1.0/amber/BasicGeometries.py` & `OncoAMBER-1.1.1/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.0/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.1.1/amber/BetaDistributionCalibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy.stats import qmc
+#from scipy.stats import qmc
 import matplotlib.pyplot as plt
 from scipy.stats import beta
 from scipy.optimize import curve_fit
 from mpl_toolkits.mplot3d import Axes3D
 import pandas as pd
 import seaborn as sns
 
@@ -60,23 +60,23 @@
     for p in range(9):
         pressure = 0.1 * p
         pressure = round(pressure, 3)
         print('pressure', pressure)
         for n_idx, n in enumerate(n_values):
             print('n =', n)
             print('side =', side)
-            sampler = qmc.Halton(2)
+            # sampler = qmc.Halton(2)
             multiple_alpha_values = []
             multiple_beta_values = []
             for _ in range(10):
 
-                points_x = sampler.random(n)[:,0] * side #quasi random to have a distribution mimicking distance between vessels
-                points_y = sampler.random(n)[:,1] * side
-                # points_x = np.random.uniform(0, side, n) #pseudo random
-                # points_y = np.random.uniform(0, side, n)
+                # points_x = sampler.random(n)[:,0] * side #quasi random to have a distribution mimicking distance between vessels
+                # points_y = sampler.random(n)[:,1] * side
+                points_x = np.random.uniform(0, side, n) #pseudo random
+                points_y = np.random.uniform(0, side, n)
 
 
                 vessels = []
                 for i in range(len(points_x)):
                     vessels.append(Vessel([points_x[i], points_y[i]], radius))
 
                 points = []
```

### Comparing `OncoAMBER-1.1.0/amber/CONFIG_default.txt` & `OncoAMBER-1.1.1/amber/CONFIG_default.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # General parameters
 half_length_world: 1.2 #cm
 voxel_per_side: 40
 dt: 24 #hours
-endtime: 480 #hours
+endtime: 240 #hours
 seed: 0                                 #seed for random number generator. -1 for random seed
 
 #Initialisation
 vessel_number: 100                       #initial number of vessels for healthy tissue per cm^2
 initial_number_healthy_cells: 100         #initial number of healthy cells per voxel
 initial_number_tumor_cells: 50          #initial total number of tumor cells
 tumor_initial_radius: 0.001 #cm
```

### Comparing `OncoAMBER-1.1.0/amber/Process.py` & `OncoAMBER-1.1.1/amber/Process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from amber.World import *
 from amber.Voxel import *
 from amber.ScalarField import *
 import amber.Terminal as term
 import amber.ReadAndWrite as rw
 import pandas as pd
 from matplotlib.colors import TwoSlopeNorm
-from amber.config_instance import config
 import matplotlib.pyplot as plt
 import os
 
 class Simulator: #this class is used to run the whole simulation
 
-    def __init__(self, list_of_process : list, finish_time, dt):
+    def __init__(self, config, list_of_process : list, finish_time, dt):
         self.list_of_process = list_of_process
         self.finish_time = finish_time
         self.dt = dt
         self.time = 0
+        self.config = config
     def show_cell_and_tumor_volume(self, number_tumor_cells, number_necrotic_cells, tumor_size, times):
         # plot number of cells evolution
         plt.plot(times, number_tumor_cells, 'purple')
         plt.plot(times, number_necrotic_cells, 'black')
         plt.title('Number of cells evolution')
         plt.xlabel('Time')
         plt.ylabel('Number of cells')
@@ -37,34 +37,34 @@
         plt.savefig('Plots/Tumor_size_evolution.png')
         plt.show()
     def show(self, world: World, t = 0): #this function is used to show the world at a certain time
 
         if not os.path.exists('Plots/CurrentPlotting/'):
             os.makedirs('Plots/CurrentPlotting/')
 
+        print('Graphics : ', self.config.show_tumor_and_vessels_3D, self.config.show_slices)
+
         DPI = 100
         size = world.half_length
 
         #plot vasculature
-        if config.show_tumor_and_vessels_3D:
+        if self.config.show_tumor_and_vessels_3D:
             fig, axes = plt.subplots(nrows=1, ncols=1, figsize=(25, 25), dpi=150, subplot_kw={'projection': '3d'})
             fig.suptitle('Visualization at time t = ' + str(t) + ' hours', fontsize=16)
-            axes.view_init(0, 90)
-            size = size/2
             axes.set_xlim(-size, size)
             axes.set_ylim(-size, size)
             axes.set_zlim(-size, size)
+            axes.view_init(90, 0)
             world.show_tumor_3D(axes, fig, 'number_of_tumor_cells', cmap='viridis', vmin=0, vmax=1000)
             world.vasculature.plot(fig, axes)
             axes.set_title('Vasculature')
             plt.savefig('Plots/CurrentPlotting/t' + str(t) + '_Vasculature.png')
             plt.show()
-            size = size*2
 
-        if config.show_slices:
+        if self.config.show_slices:
             fig, axes = plt.subplots(nrows=2, ncols=2, figsize=(25, 20), dpi=DPI)
             fig.suptitle('Visualization at time t = ' + str(t) + ' hours', fontsize=16)
 
             axes[0, 0].set_xlim(-size, size)
             axes[0, 0].set_ylim(-size, size)
             world.show_tumor_slice(axes[0, 0], fig, 'number_of_tumor_cells', levels= np.linspace(1, 1001, 11))
             axes[0,0].grid(True)
@@ -94,15 +94,15 @@
             axes[1, 1].set_facecolor('whitesmoke')
             axes[1, 1].set_title('Necrosis in voxels')
 
             plt.tight_layout()
             plt.savefig('Plots/CurrentPlotting/t' + str(t) + '_AllPlots.png')
             plt.show()
 
-        if config.show_o2_vitality_histograms:
+        if self.config.show_o2_vitality_histograms:
             voxels_positions = [[0,0,0],[0.06, 0.06, 0.0], [0.12,0.12,0.0]]
             fig, axes = plt.subplots(nrows=2, ncols=len(voxels_positions), figsize=(20, 10), dpi=100)
             fig.suptitle('Visualization at time t = ' + str(t) + ' hours', fontsize=16)
             for i in range(len(voxels_positions)):
                 #show histograms for the three voxels
                 axes[0, i].set_title('Voxel ' + str(i))
                 axes[0, i].set_xlabel('Oxygen')
@@ -115,38 +115,39 @@
             plt.show()
 
     def run(self, world: World, video=False):
         print(f'Running simulation for {self.finish_time} hours with dt={self.dt}')
         process_local = [process for process in self.list_of_process if not process.is_global]
         process_global = [process for process in self.list_of_process if process.is_global]
 
-        irradiations_times = [config.first_irradiation_time + i * config.time_between_fractions for i in
-                              range(config.number_fractions)]
+        irradiations_times = [self.config.first_irradiation_time + i * self.config.time_between_fractions for i in
+                              range(self.config.number_fractions)]
         applied_fractions = 0
 
         number_tumor_cells = []; number_necrotic_cells = []; tumor_size = []; times = []
 
         while self.time < self.finish_time:
             print(f'\033[1;31;47mTime: {self.time} hours / {self.finish_time} hours\033[0m')
+            if video:
+                self.show(world, self.time)
 
-            if applied_fractions < config.number_fractions and self.time >= irradiations_times[applied_fractions]:
-                irrad = Irradiation('irrad', self.dt, config.topas_file, config.first_irradiation_time,
-                                    config.irradiation_intensity, world)
+            if applied_fractions < self.config.number_fractions and self.time >= irradiations_times[applied_fractions]:
+                irrad = Irradiation('irrad', self.dt, self.config.topas_file, self.config.first_irradiation_time,
+                                    self.config.irradiation_intensity, world)
                 irrad(world)
                 applied_fractions += 1
 
             for voxel in world.voxel_list:
                 for process in process_local:
                     process(voxel)
             for process in process_global:
                 print('Currently running global process:', process.name)
                 process(world)
 
-            if video:
-                self.show(world, self.time)
+
 
             number_tumor_cells.append(sum([voxel.number_of_tumor_cells() for voxel in world.voxel_list]))
             number_necrotic_cells.append(sum([voxel.number_of_necrotic_cells() for voxel in world.voxel_list]))
             tumor_size_ = world.measure_tumor_volume()
             tumor_size.append(tumor_size_ * 1000)
             times.append(self.time)
 
@@ -154,38 +155,39 @@
                 os.makedirs('DataOutput/')
 
             np.save('DataOutput/number_tumor_cells.npy', number_tumor_cells)
             np.save('DataOutput/number_necrotic_cells.npy', number_necrotic_cells)
             np.save('DataOutput/tumor_size.npy', tumor_size)
             np.save('DataOutput/times.npy', times)
 
-            if config.show_cell_and_tumor_volume:
+            if self.config.show_cell_and_tumor_volume:
                 self.show_cell_and_tumor_volume(number_tumor_cells, number_necrotic_cells, tumor_size, times)
 
             self.time += self.dt
 
         print('Simulation finished')
 
-        if config.show_final:
+        if self.config.show_final:
             self.show(world, self.time)
 
         return
 
 class Process: #abstract class, represents all the processes that can happen in the simulation
-    def __init__(self, name, dt):
+    def __init__(self, config, name, dt):
         self.name = name
         self.dt = dt
         self.is_global = False
+        self.config = config
     def __call__(self, voxel):
         pass
 
 
 class CellDivision(Process): #cell division process, cells divide in a voxel if they have enough vitality
-    def __init__(self, name, dt, cycling_threshold, pressure_threshold = np.inf):
-        super().__init__(name, dt)
+    def __init__(self, config, name, dt, cycling_threshold, pressure_threshold = np.inf):
+        super().__init__(config, 'CellDivision', dt)
         self.dt = dt
         self.cycling_threshold = cycling_threshold
         self.pressure_threshold = pressure_threshold
 
     def __call__(self, voxel):
         if len(voxel.list_of_cells) > 0:
             for cell in voxel.list_of_cells:
@@ -196,16 +198,16 @@
                     new_cell.time_spent_cycling = leftover_time #reset the time spent cycling
                     cell.doubling_time = cell.random_doubling_time() #sample a new doubling time for the old cell
                     cell.time_spent_cycling = leftover_time #reset the time spent cycling
                     voxel.add_cell(new_cell) #add the new cell to the voxel
         return
 
 class CellDeath(Process): #cell necrosis process, cells die in a voxel if they have too low vitality
-    def __init__(self, name, dt, necrosis_threshold, necrosis_probability, apoptosis_threshold, apoptosis_probability):
-        super().__init__('CellNecrosis', dt)
+    def __init__(self, config, name, dt, necrosis_threshold, necrosis_probability, apoptosis_threshold, apoptosis_probability):
+        super().__init__(config, 'CellNecrosis', dt)
         self.necrosis_threshold = necrosis_threshold
         self.necrosis_probability = necrosis_probability
         self.apoptosis_threshold = apoptosis_threshold
         self.apoptosis_probability = apoptosis_probability
         if self.necrosis_threshold > self.apoptosis_threshold:
             raise ValueError('necrosis threshold must be smaller or equal to apoptosis threshold. you can set apoptosis probability to 0 if you want to avoid apoptosis.')
     def necrosis_curve(self, x):
@@ -230,36 +232,36 @@
                     voxel.cell_becomes_necrotic(cell)
                 elif sample < a:
                     #apoptosis
                     voxel.remove_cell(cell)
 
 
 class CellAging(Process): #cell aging process, cells age in a voxel
-    def __init__(self, name, dt):
-        super().__init__('CellAging', dt)
+    def __init__(self, config, name, dt):
+        super().__init__(config,'CellAging', dt)
     def __call__(self, voxel):
         for cell in voxel.list_of_cells:
             if cell.time_before_death is not None:
                 cell.time_before_death -= self.dt
                 if cell.time_before_death < 0:
                     voxel.remove_cell(cell)
-            if cell.type == 'TumorCell' and cell.vitality() > config.vitality_cycling_threshold:
+            if cell.type == 'TumorCell' and cell.vitality() > self.config.vitality_cycling_threshold:
                 cell.time_spent_cycling += self.dt
 
         for n_cell in voxel.list_of_necrotic_cells:
             if n_cell.time_before_death is not None:
                 n_cell.time_before_death -= self.dt
                 if n_cell.time_before_death < 0:
                     voxel.remove_necrotic_cell(n_cell)
         pass
 
 
 class CellMigration(Process): #cell migration process, cells migrate in the world
-    def __init__(self, name, dt, pressure_threshold):
-        super().__init__('CellMigration', dt)
+    def __init__(self, config, name, dt, pressure_threshold):
+        super().__init__(config, 'CellMigration', dt)
         self.is_global = True #run on the whole world, after the other processes
         self.pressure_threshold = pressure_threshold
 
     def __call__(self, world: World):
         exchange_matrix = world.compute_exchange_matrix(self.dt, pressure_threshold=self.pressure_threshold)
         for voxel in world.voxel_list:
             voxel_num = voxel.voxel_number
@@ -272,16 +274,16 @@
                 n_moving_cells = min(n_moving_cells, int(round(len(voxel.list_of_cells)*0.5)))
                 list_of_moving_cells = np.random.choice(voxel.list_of_cells, n_moving_cells, replace=False)
                 for cell in list_of_moving_cells:
                     if neighbor.add_cell(cell):
                         voxel.remove_cell(cell)
 
 class UpdateCellOxygen(Process):
-    def __init__(self, name, dt, voxel_half_length, effective_vessel_radius):
-        super().__init__('UpdateState', dt)
+    def __init__(self, config, name, dt, voxel_half_length, effective_vessel_radius):
+        super().__init__(config, 'UpdateState', dt)
         self.voxel_side = int(voxel_half_length*200) #um/100
         self.effective_vessel_radius = effective_vessel_radius
 
         amber_dir = os.path.abspath(os.path.dirname(__file__))
 
         alpha_file_name = 'save_alpha_dataframe' + str(self.voxel_side) + '.csv'
         beta_file_name = 'save_beta_dataframe' + str(self.voxel_side) + '.csv'
@@ -310,15 +312,15 @@
                 points.append([p, n])
                 values_alpha.append(alpha_value)
                 values_beta.append(beta_value)
 
         self.alpha_map = ScalarField2D(points, values_alpha, bounds_error=False, fill_value= None)
         self.beta_map = ScalarField2D(points, values_beta, bounds_error=False, fill_value= None)
 
-        if config.show_alpha_beta_maps:
+        if self.config.show_alpha_beta_maps:
             # Plot the alpha and beta maps
             fig = plt.figure()
             ax = fig.add_subplot(111, projection='3d')
             ax.figure.set_dpi(100)
             self.alpha_map.show_extra(fig, ax, [min(pressure_column), max(pressure_column)], [min(n_column), max(n_column)])
             plt.show()
 
@@ -349,29 +351,29 @@
                 print('alpha_', alpha_, 'beta_', beta_)
 
             o2_values = np.random.beta(alpha_, beta_, size=n_cells)
 
         for i in range(n_cells):
             voxel.list_of_cells[i].oxygen = o2_values[i]
 class UpdateVoxelMolecules(Process): #update the molecules in the voxel (VEGF), other not implemented yet
-    def __init__(self, name, dt, VEGF_production_per_cell, threshold_for_VEGF_production):
-        super().__init__('UpdateMolecules', dt)
+    def __init__(self, config, name, dt, VEGF_production_per_cell, threshold_for_VEGF_production):
+        super().__init__(config, 'UpdateMolecules', dt)
         self.VEGF_production_per_cell = VEGF_production_per_cell
         self.threshold_for_VEGF_production = threshold_for_VEGF_production
     def __call__(self, voxel: Voxel):
         VEGF = 0
         for cell in voxel.list_of_cells:
             if cell.vitality() < self.threshold_for_VEGF_production and cell.type == 'TumorCell':
                 VEGF = VEGF + self.VEGF_production_per_cell*(1-cell.vitality())
         VEGF = min(VEGF, 1.0)
         voxel.molecular_factors['VEGF'] = VEGF
         return
 class UpdateVasculature(Process): #update the vasculature
-    def __init__(self, name, dt, killing_radius_threshold, killing_length_threshold, o2_per_volume, diffusion_number, splitting_rate, macro_steps, micro_steps, weight_direction, weight_vegf, weight_pressure, radius_pressure_sensitive):
-        super().__init__('UpdateVasculature', dt)
+    def __init__(self, config, name, dt, killing_radius_threshold, killing_length_threshold, o2_per_volume, diffusion_number, splitting_rate, macro_steps, micro_steps, weight_direction, weight_vegf, weight_pressure, radius_pressure_sensitive):
+        super().__init__(config, 'UpdateVasculature', dt)
         self.is_global = True
         self.killing_radius_threshold = killing_radius_threshold
         self.killing_length_threshold = killing_length_threshold
         self.o2_per_volume = o2_per_volume
         self.diffusion_number = diffusion_number
         self.dt = dt
         self.splitting_rate = splitting_rate
@@ -389,20 +391,21 @@
         print('Killed vessels: ', n_killed)
         print('Growing vessels')
         total_VEGF = 0
         for voxel in world.voxel_list:
             total_VEGF += voxel.molecular_factors['VEGF']
         print('Total VEGF: ', total_VEGF)
         vessels = world.vasculature.list_of_vessels
-        n_new_vessels = int(config.new_vessels_per_hour * self.dt)
+        n_new_vessels = int(self.config.new_vessels_per_hour * self.dt)
+        n_new_vessels = min(n_new_vessels, len(vessels))
         chosen_vessels = random.sample(vessels, n_new_vessels)
 
         for vessel in chosen_vessels:
             if len(vessel.path) > 2:
-                point = vessel.choose_random_point()
+                point = vessel.choose_random_point(self.config.seed)
                 world.vasculature.branching(vessel.id, point)
 
         # for i in range(n_new_vessels):
         #     #order by vessels radius, so that the largest vessels are more likely to branch
         #     if i >= len(vessels):
         #         i = i - len(vessels)
         #     vessel = vessels[i]
@@ -414,16 +417,16 @@
 
         world.vasculature_growth(self.dt, self.splitting_rate, self.macro_steps, self.micro_steps, self.weight_direction, self.weight_vegf, self.weight_pressure, self.radius_pressure_sensitive)
         world.update_volume_occupied_by_vessels()
         # world.vasculature.print_vessel_tree()
         world.update_oxygen(o2_per_volume = self.o2_per_volume, diffusion_number=self.diffusion_number)
 
 class Irradiation(Process): #irradiation
-    def __init__(self, name, dt, topas_file, irradiation_time, irradiation_intensity, world: World):
-        super().__init__('Irradiation', dt)
+    def __init__(self, config, name, dt, topas_file, irradiation_time, irradiation_intensity, world: World):
+        super().__init__(config, 'Irradiation', dt)
         self.irradiation_time = irradiation_time
         self.irradiation_intensity = irradiation_intensity
 
         #check if the file exists
         if not os.path.isfile('TopasSimulation/' + topas_file + '.csv'):
             world.topas_param_file(topas_file)
             term.RunTopasSimulation(topas_file)
@@ -437,15 +440,15 @@
         fig = plt.figure(figsize=(10, 10))
         ax = fig.add_subplot(111, projection='3d')
         world.show_voxels_centers_dose(ax, fig, slice=True)
         plt.show()
     def __call__(self, world: World):
         for voxel in world.voxel_list:
             count = 0
-            probability = self.doses[voxel.voxel_number]*self.irradiation_intensity*config.death_rate_radiation
+            probability = self.doses[voxel.voxel_number]*self.irradiation_intensity*self.config.radiosensitivity
             for cell in voxel.list_of_cells:
                 if random.random() < probability:
                     if cell.time_before_death is None:
                         cell.time_before_death = random.lognormvariate(1, 1)
             for n_cell in voxel.list_of_necrotic_cells:
                 if random.random() < probability:
                     n_cell.time_before_death = random.lognormvariate(1, 1)
```

### Comparing `OncoAMBER-1.1.0/amber/ReadAndWrite.py` & `OncoAMBER-1.1.1/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.0/amber/RunTopas.py` & `OncoAMBER-1.1.1/amber/RunTopas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from amber.Terminal import *
 import os
 import amber.ReadAndWrite as rw
 from amber.World import World
 import matplotlib.pyplot as plt
-from amber.config_instance import config
 
 def RunTopasSimulation():
 
     world = World(config.half_length_world, config.voxel_per_side)
     world.topas_param_file(config.TOPAS_file)
     RunTopasSimulation(config.TOPAS_file)
```

### Comparing `OncoAMBER-1.1.0/amber/ScalarField.py` & `OncoAMBER-1.1.1/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.0/amber/Terminal.py` & `OncoAMBER-1.1.1/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.0/amber/Vessel.py` & `OncoAMBER-1.1.1/amber/Vessel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import random
 from amber.BasicGeometries import *
 import sys
-from amber.config_instance import config
 
 sys.setrecursionlimit(1500)
-rng = np.random.default_rng(config.seed)
 
 class Vessel:
-    def __init__(self, path, radius, parent_id=None, children_ids=None, in_growth=True):
+    def __init__(self, path, radius, step_size, parent_id=None, children_ids=None, in_growth=True):
         if children_ids is None:
             children_ids = []
         for point in path:
             if not isinstance(point, np.ndarray) or len(point.shape) != 1 or point.shape[0] != 3:
                 raise ValueError("Each point in the 'path' list must be a 3D array with shape (3,)")
         self.path = np.array(path)
         self.radius = radius
         self.id = id(self)
         self.parent_id = parent_id
         self.children_ids = children_ids
-        self.step_size = config.vessel_step_size
+        self.step_size = step_size
         self.in_growth = in_growth
         self.healthy = False
         self.visible = True
 
     def to_dict(self):
         return {
             "path": self.path.tolist(),
@@ -35,35 +33,35 @@
         }
     def __iter__(self):
         return self
 
     def length(self):
         return np.sum(np.linalg.norm(np.diff(self.path, axis=0), axis=1))
 
-    def grow(self, vegf_gradient, pressure, steps=1, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5):
+    def grow(self, limit_half_length, ref_vegf, ref_pressure, step_stop_threshold, vegf_gradient, pressure, steps=1, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5):
         length = 0
         for i in range(steps):
-            step_size = self.step(vegf_gradient, pressure, weight_direction, weight_vegf, weight_pressure)
-            if step_size < config.growth_step_stop_threshold:
+            step_size = self.step(limit_half_length, ref_vegf, ref_pressure, vegf_gradient, pressure, weight_direction, weight_vegf, weight_pressure)
+            if step_size < step_stop_threshold:
                 self.in_growth = False
                 break
             length += step_size
         return length
         # if step_size < config.growth_stop_threshold'] * self.step_size:
         #     self.in_growth = False
 
-    def step(self, vegf_gradient, pressure, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5):
+    def step(self, half_length_world, ref_vegf, ref_pressure, vegf_gradient, pressure, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5):
         if not isinstance(self.path, np.ndarray) or len(self.path.shape) != 2 or self.path.shape[1] != 3:
             raise ValueError("The 'self.path' array must be a 3D array with shape (n, 3)")
         last_point = np.array(self.path[-1])
         prev_point = np.array(self.path[-2]) if len(self.path) > 1 else last_point
 
-        if last_point[0] < -config.half_length_world or last_point[0] > config.half_length_world or \
-                last_point[1] < -config.half_length_world or last_point[1] > config.half_length_world or \
-                last_point[2] < -config.half_length_world or last_point[2] > config.half_length_world:
+        if last_point[0] < -half_length_world or last_point[0] > half_length_world or \
+                last_point[1] < -half_length_world or last_point[1] > half_length_world or \
+                last_point[2] < -half_length_world or last_point[2] > half_length_world:
             return 0
 
         direction = last_point - prev_point
 
         # Get VEGF gradient at the last point
         vegf_grad = np.array(vegf_gradient(last_point))
         local_pressure = pressure(last_point)
@@ -82,24 +80,20 @@
         # Add random noise
         noise = np.array([random.random()*2 - 1, random.random()*2-1, random.random()*2 - 1])
         weighted_dir += noise
 
         # Normalize the weighted direction
         weighted_dir /= np.linalg.norm(weighted_dir)
 
-        if config.verbose:
-            print('vegf_grad_norm_scalar: ', vegf_grad_norm_scalar)
-            print('local_pressure: ', local_pressure)
-
         # Calculate the new point and add it
         step_size = self.step_size
-        if weight_vegf > 0 and vegf_grad_norm_scalar < config.reference_vegf_gradient:
-            step_size = step_size * (vegf_grad_norm_scalar / config.reference_vegf_gradient)
-        if weight_pressure > 0 and local_pressure > config.reference_pressure:
-            step_size = step_size * (config.reference_pressure / local_pressure)
+        if weight_vegf > 0 and vegf_grad_norm_scalar < ref_vegf:
+            step_size = step_size * (vegf_grad_norm_scalar / ref_vegf)
+        if weight_pressure > 0 and local_pressure > ref_pressure:
+            step_size = step_size * (ref_pressure / local_pressure)
 
         new_point = last_point + step_size * weighted_dir
         self.path = np.append(self.path, [new_point], axis=0)
         return step_size
 
     def volume_per_point(self):
         return np.pi * self.radius ** 2 * self.step_size
@@ -107,33 +101,35 @@
     def plot(self,fig, ax, color='crimson'):
         if self.visible:
             if self.in_growth:
                 ax.plot(self.path[:, 0], self.path[:, 1], self.path[:, 2], color=color, alpha=0.7, linewidth= self.radius*300)
             else:
                 ax.plot(self.path[:, 0], self.path[:, 1], self.path[:, 2], color='mediumblue', alpha=0.1, linewidth= self.radius*300)
         return fig, ax
-    def choose_random_point(self):
+    def choose_random_point(self, seed):
+        rng = np.random.default_rng(seed)
         #choose random point on the path, not the first or last point
         if len(self.path) < 3:
             print(self.path)
             raise ValueError("The vessel path is too short to choose a random point")
         return rng.choice(self.path[1:-1])
     def mean_pressure(self, pressure):
         if len(self.path) < 2:
             return 0
         else:
             return np.mean([pressure(point) for point in self.path])
 
     def max_pressure(self, pressure):
         return np.max([pressure(point) for point in self.path])
 class VasculatureNetwork:
-    def __init__(self, list_of_vessels=None):
+    def __init__(self, config, list_of_vessels=None):
         if list_of_vessels is None:
             list_of_vessels = []
         self.list_of_vessels = list_of_vessels
+        self.config = config
 
     def branching(self, vessel_id, branching_point):
         if branching_point == [] or branching_point is None:
             print("No branching point found, branching point is", branching_point)
             return
         mother_vessel = self.get_vessel(vessel_id)
         if mother_vessel is None:
@@ -147,23 +143,23 @@
         path_begin, path_end = np.split(path, [split_index])
         #remove the first element of path_end to keep the same point distribution in space
         path_end = np.delete(path_end, 0, 0)
         mother_vessel.path = path_begin  # reduce the mother vessel path. It stops growing
         mother_vessel.in_growth = False
 
         # create two new vessels
-        vessel_end = Vessel(path_end, mother_vessel.radius, parent_id= mother_vessel.id, children_ids=mother_vessel.children_ids, in_growth= mother_vessel.in_growth)
+        vessel_end = Vessel(path_end, mother_vessel.radius, self.config.vessel_step_size, parent_id= mother_vessel.id, children_ids=mother_vessel.children_ids, in_growth= mother_vessel.in_growth)
         for child_id in vessel_end.children_ids:
             child = self.get_vessel(child_id)
             child.parent_id = vessel_end.id
         #choose random point around branching point
         #random_point = branching_point + np.array([random.uniform(-mother_vessel.step, mother_vessel.step), random.uniform(-mother_vessel.step, mother_vessel.step), random.uniform(-mother_vessel.step, mother_vessel.step)])
         # the radius has to be updated later
 
-        vessel_new = Vessel([branching_point], config.radius_root_vessels, parent_id= mother_vessel.id)  # the radius has to be updated later
+        vessel_new = Vessel([branching_point], self.config.radius_root_vessels, self.config.vessel_step_size, parent_id= mother_vessel.id)  # the radius has to be updated later
         mother_vessel.children_ids = [vessel_end.id, vessel_new.id]
         self.list_of_vessels.append(vessel_end)
         self.list_of_vessels.append(vessel_new)
         # update the mother vessel
 
 
     def add_vessel(self, vessel: Vessel):
@@ -210,15 +206,15 @@
 
         # Call update_radius_recursive for each root vessel
         for root_vessel in root_vessels:
             update_radius_recursive(root_vessel.id)
 
         if pressure_sensitive:
             for vessel in self.list_of_vessels:
-                vessel.radius = vessel.radius / ((1 + (vessel.mean_pressure(pressure)))**config.radius_decrease_exponent)
+                vessel.radius = vessel.radius / ((1 + (vessel.mean_pressure(pressure)))**self.config.radius_decrease_exponent)
 
     def update_vessels_radius_from_root(self, root_radius, pressure_sensitive=False, pressure=None):
         print("Updating vessels radius from root")
 
         def update_radius_recursive(vessel_id):
             vessel = self.get_vessel(vessel_id)
 
@@ -239,15 +235,15 @@
         for root_vessel in root_vessels:
             root_vessel.radius = root_radius
             update_radius_recursive(root_vessel.id)
 
         if pressure_sensitive:
             for vessel in self.list_of_vessels:
                 vessel.radius = vessel.radius / (
-                            (1 + (vessel.mean_pressure(pressure))) ** config.radius_decrease_exponent)
+                            (1 + (vessel.mean_pressure(pressure))) ** self.config.radius_decrease_exponent)
 
     def volume_occupied(self):
         points = []
         volume = []
         for vessel in self.list_of_vessels:
             for point in vessel.path:
                 points.append(point)
@@ -272,19 +268,19 @@
             print("Macro step {}".format(i))
             j = 0
             for vessel in self.list_of_vessels:
                 splitting_rate_ = splitting_rate
                 if j % 1000 == 0: print('current number of vessels {}'.format(len(self.list_of_vessels)))
                 if vessel.in_growth:
                     total_path_length = vessel.step_size * micro_steps
-                    new_path_length = vessel.grow(vegf_gradient, pressure, micro_steps, weight_direction, weight_vegf, weight_pressure)
+                    new_path_length = vessel.grow(self.config.half_length_world, self.config.reference_vegf_gradient, self.config.reference_pressure, self.config.growth_step_stop_threshold, vegf_gradient, pressure, micro_steps, weight_direction, weight_vegf, weight_pressure)
                     if len(vessel.path) > 3:
                         splitting_rate_ = (new_path_length / total_path_length) * splitting_rate_
                         if random.uniform(0, 1) < splitting_rate_ * dt:
-                            branching_point = vessel.choose_random_point()
+                            branching_point = vessel.choose_random_point(self.config.seed)
                             self.branching(vessel.id, branching_point)
                 j += 1
     def print_vessel_tree_recursive(self, vessels, children_ids, indent):
         for child_id in children_ids:
             child_vessel = next((v for v in vessels if v.id == child_id), None)
             if child_vessel is not None:
                 print(' ' * indent, f"ID: {child_vessel.id}  Radius: {child_vessel.radius:.5f}")
```

### Comparing `OncoAMBER-1.1.0/amber/World.py` & `OncoAMBER-1.1.1/amber/World.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from amber.Voxel import *
 from amber.Vessel import *
 from amber.ScalarField import *
 from amber.BasicGeometries import *
 #np.set_printoptions(threshold=sys.maxsize)
-from scipy.stats import qmc
+# from scipy.stats import qmc
 import matplotlib.tri as mtri
 import scipy.sparse as sparse
-from amber.config_instance import config
 
 class World:
-    def __init__(self, half_length, number_of_voxels : int = 20):
+    def __init__(self, config , half_length, number_of_voxels : int = 20):
         self.half_length = half_length
         self.voxel_list = []
         self.total_number_of_voxels = number_of_voxels ** 3
+        self.config = config
         voxel_length = 2 * half_length / number_of_voxels
 
         for i in range(number_of_voxels):
             for j in range(number_of_voxels):
                 for k in range(number_of_voxels):
                     position = np.array([
                         i * voxel_length - half_length + voxel_length / 2,
                         j * voxel_length - half_length + voxel_length / 2,
                         k * voxel_length - half_length + voxel_length / 2
                     ])
                     self.voxel_list.append(Voxel(position, half_length / number_of_voxels, voxel_number=i * number_of_voxels ** 2 + j * number_of_voxels + k))
         self.number_of_voxels = number_of_voxels
-        self.vasculature = VasculatureNetwork()
+        self.vasculature = VasculatureNetwork(self.config)
 
     def initiate_vasculature(self, list_of_mother_vessels):
-        self.vasculature = VasculatureNetwork(list_of_mother_vessels)
+        self.vasculature = VasculatureNetwork(self.config, list_of_mother_vessels)
         return
 
     def vasculature_growth(self, dt, splitting_rate, macro_steps=1, micro_steps=10, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5, radius_pressure_sensitive = False):
         print('Vasculature growth')
         pressure_map = self.pressure_map(step_voxel=5)
         def pressure(point): return pressure_map.evaluate(point)
-        vegf = self.vegf_map(step_voxel= config.vegf_map_step_voxel)
+        vegf = self.vegf_map(step_voxel= self.config.vegf_map_step_voxel)
 
         def vegf_gradient(point): return vegf.gradient(point)
 
         self.vasculature.grow_and_split(dt = dt,
                                         splitting_rate = splitting_rate,
                                         macro_steps = macro_steps,
                                         micro_steps = micro_steps,
                                         weight_direction = weight_direction,
                                         weight_vegf = weight_vegf,
                                         weight_pressure = weight_pressure,
                                         pressure = pressure,
                                         vegf_gradient = vegf_gradient)
-        self.vasculature.update_vessels_radius_from_last(config.radius_root_vessels, radius_pressure_sensitive, pressure)
+        self.vasculature.update_vessels_radius_from_last(self.config.radius_root_vessels, radius_pressure_sensitive, pressure)
         return
 
     def generate_healthy_vasculature(self, initial_vessel_number, splitting_rate =0.3, mult_macro_steps=1, micro_steps=8, weight_direction=3.0, weight_vegf=1.0, weight_pressure=0.0, extra_step = True):
         initial_vessel_number = int(initial_vessel_number * 4 * self.half_length ** 2)
-        sampler = qmc.Halton(2, seed=config.seed)
-        points_z = (sampler.random(initial_vessel_number)[:,0] - 0.5) * self.half_length*2
-        points_y = (sampler.random(initial_vessel_number)[:,1] - 0.5) * self.half_length*2
+        # sampler = qmc.Halton(2, seed=config.seed)
+        # points_z = (sampler.random(initial_vessel_number)[:,0] - 0.5) * self.half_length*2
+        # points_y = (sampler.random(initial_vessel_number)[:,1] - 0.5) * self.half_length*2
+        points_z = np.random.uniform(-self.half_length, self.half_length, initial_vessel_number)
+        points_y = np.random.uniform(-self.half_length, self.half_length, initial_vessel_number)
         points_x = np.append(self.half_length * np.ones(initial_vessel_number//2), -self.half_length * np.ones(initial_vessel_number//2))
         points = []
         for i in range(len(points_x)):
             points.append([points_x[i], points_y[i], points_z[i]])
         points = np.array(points)
         points2 = []
         for i in range(len(points)):
@@ -68,30 +70,30 @@
             else:
                 points2.append([points[i][0] + 0.01, points[i][1], points[i][2]])
         points2 = np.array(points2)
         print('Initial vessels: ', points[0], points2[0])
 
         list_of_vessels = []
         for j in range(len(points)):
-            list_of_vessels.append(Vessel([points[j], points2[j]], 0.5))
+            list_of_vessels.append(Vessel([points[j], points2[j]], 0.5, step_size=self.config.vessel_step_size))
         self.initiate_vasculature(list_of_vessels)
         def pressure(point):
             return (self.half_length - abs(point[0]))*0.3
         def vegf_gradient(point):
             if point[0] > 0:
                 return np.array([-point[0],0,0])*0.1
             else:
                 return np.array([-point[0],0,0])*0.1
 
         self.vasculature.grow_and_split(
             dt=1,
             splitting_rate=splitting_rate,
             vegf_gradient= vegf_gradient,
             pressure= pressure,
-            macro_steps=int(8.5*self.half_length*mult_macro_steps),
+            macro_steps=int(9*self.half_length*mult_macro_steps),
             micro_steps=micro_steps,
             weight_direction=weight_direction,
             weight_vegf=weight_vegf,
             weight_pressure=weight_pressure
         )
         if extra_step:
             self.vasculature.grow_and_split(
@@ -103,18 +105,18 @@
                 micro_steps=micro_steps,
                 weight_direction=weight_direction,
                 weight_vegf=0.1,
                 weight_pressure=0.0
             )
 
 
-        self.vasculature.update_vessels_radius_from_last(config.radius_root_vessels, False, pressure)
+        self.vasculature.update_vessels_radius_from_last(self.config.radius_root_vessels, False, pressure)
         for vessel in self.vasculature.list_of_vessels:
             vessel.in_growth = False
-            vessel.visible = config.visible_original_vessels
+            vessel.visible = self.config.visible_original_vessels
         return
 
     def random_points_for_voxels_concentration(self, num_points, molecule : str):
         if num_points == 0:
             return []
         if num_points % 1000 == 0:
             print('-- Generating ' + str(num_points) + ' random points for ' + molecule + ' concentration, if no progress is shown, VEGF concentration might be too low')
@@ -231,15 +233,15 @@
 
             for neighbor in neighbors:
                 j = neighbor.voxel_number
 
                 pressure_diff = voxel_pressure - pressures[j]
                 if pressure_diff > pressure_threshold:
                     t_res = (V / pressure_diff) * viscosity
-                    if config.verbose: print('t_res = ', t_res)
+                    if self.config.verbose: print('t_res = ', t_res)
                     n_events = dt / t_res
                     migration_matrix[i, j] = n_events
 
         # Convert the lil_matrix to a csr_matrix for faster arithmetic operations
         migration_matrix = migration_matrix.tocsr()
 
         return migration_matrix
@@ -275,15 +277,15 @@
         for voxel in self.voxel_list:
             voxel.dose = doses[voxel.voxel_number]
         return
 
     def update_oxygen(self, o2_per_volume=1, diffusion_number=5):
         print('-- Computing oxygen map')
         for voxel in self.voxel_list:
-            voxel.oxygen = int((voxel.vessel_volume * o2_per_volume) / (np.pi * config.effective_vessel_radius**2 * voxel.half_length * 2))
+            voxel.oxygen = int((voxel.vessel_volume * o2_per_volume) / (np.pi * self.config.effective_vessel_radius**2 * voxel.half_length * 2))
         for i in range(diffusion_number):
             new_oxygen_map = np.zeros(self.total_number_of_voxels)
             print('--- o2 map computing', i, 'out of', diffusion_number)
             for voxel in self.voxel_list:
                 sum = voxel.oxygen
                 for neighbor in self.find_neighbors(voxel):
                     sum += neighbor.oxygen
@@ -338,30 +340,30 @@
         voxel_list_x = []
 
         for i in range(self.number_of_voxels):
             for j in range(self.number_of_voxels):
                 index = middle_slice_x + j * self.number_of_voxels + i * self.number_of_voxels ** 2
                 voxel_list_x.append(self.voxel_list[index])
 
-        if config.slice == 'x':
+        if self.config.slice == 'x':
             voxel_list = voxel_list_x
         else:
             voxel_list = voxel_list_z
         values = []
         positions = []
         for voxel in voxel_list:
             if factor is not None and isinstance(getattr(voxel, voxel_attribute), dict):
                 value = getattr(voxel, voxel_attribute)[factor]
             else:
                 value = getattr(voxel, voxel_attribute)() if callable(getattr(voxel, voxel_attribute)) else getattr(
                     voxel, voxel_attribute)
             values.append(value)
             positions.append(voxel.position)
 
-        if config.slice == 'x':
+        if self.config.slice == 'x':
             x = np.array([p[0] for p in positions])
             y = np.array([p[1] for p in positions])
             z = np.array(values)
         else:
             x = np.array([p[1] for p in positions])
             y = np.array([p[2] for p in positions])
             z = np.array(values)
```

### Comparing `OncoAMBER-1.1.0/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.1.1/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.0/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.1.1/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.0/setup.py` & `OncoAMBER-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
 
@@ -90,12 +90,12 @@
     packages=find_packages(),
     package_data={'': ['*.txt', '*.csv'],},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     # include_package_data=True,
     zip_safe=False,
     license='MIT',
-    classifiers=[   'License :: OSI Approved :: MIT License',    'Operating System :: MacOS',    'Operating System :: Microsoft :: Windows',    'Programming Language :: Python',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.6',    'Programming Language :: Python :: Implementation :: CPython',    'Programming Language :: Python :: Implementation :: PyPy'],
+    classifiers=[  'License :: OSI Approved :: MIT License',    'Operating System :: MacOS',    'Operating System :: Microsoft :: Windows',    'Programming Language :: Python',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.6',    'Programming Language :: Python :: Implementation :: CPython',    'Programming Language :: Python :: Implementation :: PyPy'],
     cmdclass={
         'upload' : UploadCommand,
     }
 )
```

