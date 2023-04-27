# Comparing `tmp/gstatsim-1.0.1.tar.gz` & `tmp/gstatsim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstatsim-1.0.1.tar", last modified: Wed Nov  2 19:02:51 2022, max compression
+gzip compressed data, was "gstatsim-1.0.2.tar", last modified: Thu Apr 27 17:10:39 2023, max compression
```

## Comparing `gstatsim-1.0.1.tar` & `gstatsim-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2022-11-02 19:02:51.921013 gstatsim-1.0.1/
--rw-r--r--   0 michaelfield   (502) staff       (20)     1072 2022-10-27 14:50:52.000000 gstatsim-1.0.1/LICENSE
--rw-r--r--   0 michaelfield   (502) staff       (20)     4885 2022-11-02 19:02:51.920899 gstatsim-1.0.1/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)     4345 2022-11-02 19:02:36.000000 gstatsim-1.0.1/README.md
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2022-11-02 19:02:51.920738 gstatsim-1.0.1/gstatsim.egg-info/
--rw-r--r--   0 michaelfield   (502) staff       (20)     4885 2022-11-02 19:02:51.000000 gstatsim-1.0.1/gstatsim.egg-info/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)      197 2022-11-02 19:02:51.000000 gstatsim-1.0.1/gstatsim.egg-info/SOURCES.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        1 2022-11-02 19:02:51.000000 gstatsim-1.0.1/gstatsim.egg-info/dependency_links.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)       69 2022-11-02 19:02:51.000000 gstatsim-1.0.1/gstatsim.egg-info/requires.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        9 2022-11-02 19:02:51.000000 gstatsim-1.0.1/gstatsim.egg-info/top_level.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)    48456 2022-11-02 18:59:33.000000 gstatsim-1.0.1/gstatsim.py
--rw-r--r--   0 michaelfield   (502) staff       (20)       38 2022-11-02 19:02:51.921052 gstatsim-1.0.1/setup.cfg
--rw-r--r--   0 michaelfield   (502) staff       (20)      938 2022-11-02 19:02:20.000000 gstatsim-1.0.1/setup.py
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-04-27 17:10:39.252550 gstatsim-1.0.2/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-04-27 17:08:18.000000 gstatsim-1.0.2/LICENSE
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-04-27 17:10:39.252421 gstatsim-1.0.2/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)     4620 2023-04-27 17:10:19.000000 gstatsim-1.0.2/README.md
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-04-27 17:10:39.252265 gstatsim-1.0.2/gstatsim.egg-info/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/requires.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/top_level.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)    56584 2023-04-27 16:20:42.000000 gstatsim-1.0.2/gstatsim.py
+-rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-04-27 17:10:39.252585 gstatsim-1.0.2/setup.cfg
+-rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-04-27 17:10:12.000000 gstatsim-1.0.2/setup.py
```

### Comparing `gstatsim-1.0.1/LICENSE` & `gstatsim-1.0.2/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 GatorGlaciology
+Copyright (c) 2022 Emma MacKie
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gstatsim-1.0.1/PKG-INFO` & `gstatsim-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # GStatSim
 GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
+We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
+
 In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
 
 We will continuously develop new tools and tutorials to address specific technical challenges in geostatistics. Do you have feedback or suggestions? Specific things that we should account for? Feel free to contact me at emackie@ufl.edu. Our goal is to create tools that are useful and accessible, so we welcome your thoughts and insight.
 
 
 # Features
 
@@ -70,28 +72,32 @@
 
 or
 
 *git clone https://github.com/GatorGlaciology/GStatSim*
 
 
 
-## Package dependencies
+# Package dependencies
 * Numpy
 * Pandas
 * Scipy
 * tqdm
 * Sklearn
 
-## Requirements for visualization and variogram analysis
+# Requirements for visualization and variogram analysis
 * Matplotlib
 * SciKit-GStat
 
 These can all be installed using the command *pip install (package name)*. We have included a plot_utils.py file with plotting routines.
 
-## Cite as
+# Educational use
+
+GStatSim is well-suited for educational use. Please contact us if you plan on using GStatSim material in a course so we can track the impact of our work.
+
+# Cite as
 
 MacKie, Emma, Field, Michael, Wang, Lijing, Yin, Zhen, Schoedl, Nathan, & Hibbs, Matthew. (2022). GStatSim (1.0). Zenodo. https://doi.org/10.5281/zenodo.7230276
 
 or
 
 @software{mackie_emma_2022_7274640,
   author       = {MacKie, Emma and
```

### Comparing `gstatsim-1.0.1/README.md` & `gstatsim-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 # GStatSim
 GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
+We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
+
 In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
 
 We will continuously develop new tools and tutorials to address specific technical challenges in geostatistics. Do you have feedback or suggestions? Specific things that we should account for? Feel free to contact me at emackie@ufl.edu. Our goal is to create tools that are useful and accessible, so we welcome your thoughts and insight.
 
 
 # Features
 
@@ -54,28 +56,32 @@
 
 or
 
 *git clone https://github.com/GatorGlaciology/GStatSim*
 
 
 
-## Package dependencies
+# Package dependencies
 * Numpy
 * Pandas
 * Scipy
 * tqdm
 * Sklearn
 
-## Requirements for visualization and variogram analysis
+# Requirements for visualization and variogram analysis
 * Matplotlib
 * SciKit-GStat
 
 These can all be installed using the command *pip install (package name)*. We have included a plot_utils.py file with plotting routines.
 
-## Cite as
+# Educational use
+
+GStatSim is well-suited for educational use. Please contact us if you plan on using GStatSim material in a course so we can track the impact of our work.
+
+# Cite as
 
 MacKie, Emma, Field, Michael, Wang, Lijing, Yin, Zhen, Schoedl, Nathan, & Hibbs, Matthew. (2022). GStatSim (1.0). Zenodo. https://doi.org/10.5281/zenodo.7230276
 
 or
 
 @software{mackie_emma_2022_7274640,
   author       = {MacKie, Emma and
```

### Comparing `gstatsim-1.0.1/gstatsim.egg-info/PKG-INFO` & `gstatsim-1.0.2/gstatsim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # GStatSim
 GStatSim is a Python package specifically designed for geostatistical interpolation and simulation. It is inspired by open source geostatistical resources such as GeostatsPy and SciKit-GStat. The functions are intended to address the challenges of working with datasets with large crossover errors, non-linear trends, variability in measurement density, and non-stationarity. These tools are part of our ongoing effort to develop and adapt open-access geostatistical functions.
 
+We have created Jupyter Book tutorials here: https://gatorglaciology.github.io/gstatsimbook/intro.html
+
 In its current state, the demos focus on the geostatistical simulation of subglacial topography. However, these protocols could be applied to a number topics in glaciology, or geoscientific problems in general.
 
 We will continuously develop new tools and tutorials to address specific technical challenges in geostatistics. Do you have feedback or suggestions? Specific things that we should account for? Feel free to contact me at emackie@ufl.edu. Our goal is to create tools that are useful and accessible, so we welcome your thoughts and insight.
 
 
 # Features
 
@@ -70,28 +72,32 @@
 
 or
 
 *git clone https://github.com/GatorGlaciology/GStatSim*
 
 
 
-## Package dependencies
+# Package dependencies
 * Numpy
 * Pandas
 * Scipy
 * tqdm
 * Sklearn
 
-## Requirements for visualization and variogram analysis
+# Requirements for visualization and variogram analysis
 * Matplotlib
 * SciKit-GStat
 
 These can all be installed using the command *pip install (package name)*. We have included a plot_utils.py file with plotting routines.
 
-## Cite as
+# Educational use
+
+GStatSim is well-suited for educational use. Please contact us if you plan on using GStatSim material in a course so we can track the impact of our work.
+
+# Cite as
 
 MacKie, Emma, Field, Michael, Wang, Lijing, Yin, Zhen, Schoedl, Nathan, & Hibbs, Matthew. (2022). GStatSim (1.0). Zenodo. https://doi.org/10.5281/zenodo.7230276
 
 or
 
 @software{mackie_emma_2022_7274640,
   author       = {MacKie, Emma and
```

### Comparing `gstatsim-1.0.1/gstatsim.py` & `gstatsim-1.0.2/gstatsim.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,23 +22,34 @@
 ############################
 
 class Gridding:
 
     def prediction_grid(xmin, xmax, ymin, ymax, res):
         """
         Make prediction grid
-        Inputs:
-            xmin - minimum x extent
-            xmax - maximum x extent
-            ymin - minimum y extent
-            ymax - maximum y extent
-            res - grid cell resolution
-        Outputs:
-            prediction_grid_xy - x,y array of coordinates
+        
+        Parameters
+        ----------
+            xmin : float, int
+                minimum x extent
+            xmax : float, int
+                maximum x extent
+            ymin : float, int
+                minimum y extent
+            ymax : float, int
+                maximum y extent
+            res : float, int
+                grid cell resolution
+        
+        Returns
+        -------
+            prediction_grid_xy : numpy.ndarray
+                x,y array of coordinates
         """ 
+        
         cols = np.rint((xmax - xmin + res)/res)
         rows = np.rint((ymax - ymin + res)/res)  
         x = np.linspace(xmin, xmin+(cols*res), num=int(cols), endpoint=False)
         y = np.linspace(ymin, ymin+(rows*res), num=int(rows), endpoint=False)
         xx, yy = np.meshgrid(x,y) 
         yy = np.flip(yy) 
         x = np.reshape(xx, (int(rows)*int(cols), 1))
@@ -46,25 +57,38 @@
         prediction_grid_xy = np.concatenate((x,y), axis = 1)
         
         return prediction_grid_xy
  
     def make_grid(xmin, xmax, ymin, ymax, res):
         """
         Generate coordinates for output of gridded data  
-        Inputs:
-            xmin - minimum x extent
-            xmax - maximum x extent
-            ymin - minimum y extent
-            ymax - maximum y extent
-            res - grid cell resolution
-        Outputs:
-            prediction_grid_xy - x,y array of coordinates
-            rows - number of rows 
-            cols - number of columns
+        
+        Parameters
+        ----------
+            xmin : float, int
+                minimum x extent
+            xmax : float, int
+                maximum x extent
+            ymin : float, int
+                minimum y extent
+            ymax : float, int
+                maximum y extent
+            res : float, int
+                grid cell resolution
+        
+        Returns
+        -------
+            prediction_grid_xy : numpy.ndarray
+                x,y array of coordinates
+            rows : int
+                number of rows 
+            cols : int 
+                number of columns
         """ 
+        
         cols = np.rint((xmax - xmin)/res) 
         rows = np.rint((ymax - ymin)/res)  
         rows = rows.astype(int)
         cols = cols.astype(int)
         x = np.arange(xmin,xmax,res); y = np.arange(ymin,ymax,res)
         xx, yy = np.meshgrid(x,y) 
         x = np.reshape(xx, (int(rows)*int(cols), 1)) 
@@ -72,25 +96,38 @@
         prediction_grid_xy = np.concatenate((x,y), axis = 1)
         
         return prediction_grid_xy, cols, rows
     
     def grid_data(df, xx, yy, zz, res):
         """
         Grid conditioning data
-        Inputs:
-            df - dataframe of conditioning data
-            xx - column name for x coordinates of input data frame
-            yy - column name for y coordinates of input data frame
-            zz - column for z values (or data variable) of input data frame
-            res - grid cell resolution
-        Outputs:
-            df_grid - dataframe of gridded data
-            grid_matrix - matrix of gridded data
-            rows - number of rows in grid_matrix
-            cols - number of columns in grid_matrix
+        
+        Parameters
+        ----------
+            df : pandas DataFrame 
+                dataframe of conditioning data and coordinates
+            xx : string 
+                column name for x coordinates of input data frame
+            yy : string
+                column name for y coordinates of input data frame
+            zz : string
+                column for z values (or data variable) of input data frame
+            res : float, int
+                grid cell resolution
+        
+        Returns
+        -------
+            df_grid : pandas DataFrame
+                dataframe of gridded data
+            grid_matrix : numpy.ndarray
+                matrix of gridded data
+            rows : int
+                number of rows in grid_matrix
+            cols : int
+                number of columns in grid_matrix
         """ 
         df = df.rename(columns = {xx: "X", yy: "Y", zz: "Z"})
 
         xmin = df['X'].min()
         xmax = df['X'].max()
         ymin = df['Y'].min()
         ymax = df['Y'].max()
@@ -142,20 +179,29 @@
 # RBF trend estimation
 
 ###################################
 
 def rbf_trend(grid_matrix, smooth_factor, res):
     """
     Estimate trend using radial basis functions
-    Inputs:
-        grid_matrix - matrix of gridded conditioning data
-        smooth_factor - regularizing parameter
-        res - grid cell resolution
-    Outputs:
-        trend_rbf - trend estimate
+    
+    Parameters
+    ----------
+        grid_matrix : numpy.ndarray
+            matrix of gridded conditioning data
+        smooth_factor : float
+            Parameter controlling smoothness of trend. Values greater than 
+            zero increase the smoothness of the approximation.
+        res : float
+            grid cell resolution
+            
+    Returns
+    -------
+        trend_rbf : numpy.ndarray
+            RBF trend estimate
     """ 
     sigma = np.rint(smooth_factor/res)
     ny, nx = grid_matrix.shape
     rbfi = Rbf(np.where(~np.isnan(grid_matrix))[1],
                np.where(~np.isnan(grid_matrix))[0], 
                grid_matrix[~np.isnan(grid_matrix)],smooth = sigma)
 
@@ -175,63 +221,97 @@
 ####################################
 
 class NearestNeighbor:
 
     def center(arrayx, arrayy, centerx, centery):
         """
         Shift data points so that grid cell of interest is at the origin
-        Inputs:
-            arrayx - x coordinates of data
-            arrayy - y coordinates of data
-            centerx - x coordinate of grid cell of interest
-            centery - y coordinate of grid cell of interest
-        Outputs:
-            centered_array - array of coordinates that are shifted with respect to grid cell of interest
+        
+        Parameters
+        ----------
+            arrayx : numpy.ndarray
+                x coordinates of data
+            arrayy : numpy.ndarray
+                y coordinates of data
+            centerx : float
+                x coordinate of grid cell of interest
+            centery : float
+                y coordinate of grid cell of interest
+        
+        Returns
+        -------
+            centered_array : numpy.ndarray
+                array of coordinates that are shifted with respect to grid cell of interest
         """ 
+        
         centerx = arrayx - centerx
         centery = arrayy - centery
         centered_array = np.array([centerx, centery])
         
         return centered_array
 
     def distance_calculator(centered_array):
         """
         Compute distances between coordinates and the origin
-        Inputs:
-            centered_array - array of coordinates
-        Outputs:
-            dist - array of distances between coordinates and origin
+        
+        Parameters
+        ----------
+            centered_array : numpy.ndarray
+                array of coordinates
+        
+        Returns
+        -------
+            dist : numpy.ndarray
+                array of distances between coordinates and origin
         """ 
+        
         dist = np.linalg.norm(centered_array, axis=0)
         
         return dist
 
     def angle_calculator(centered_array):
         """
         Compute angles between coordinates and the origin
-        Inputs:
-            centered_array - array of coordinates
-        Outputs:
-            angles - array of angles between coordinates and origin
+        
+        Parameters
+        ----------
+            centered_array : numpy.ndarray
+                array of coordinates
+        
+        Returns
+        -------
+            angles : numpy.ndarray
+                array of angles between coordinates and origin
         """ 
+        
         angles = np.arctan2(centered_array[0], centered_array[1])
         
         return angles
     
     def nearest_neighbor_search(radius, num_points, loc, data2):
         """
         Nearest neighbor octant search
-        Inputs:
-            radius - search radius
-            num_points - number of points to search for
-            loc - coordinates for grid cell of interest
-            data2 - data 
-        Outputs:
-            near - nearest neighbors
+        
+        Parameters
+        ----------
+            radius : int, float
+                search radius
+            num_points : int
+                number of points to search for
+            loc : numpy.ndarray
+                coordinates for grid cell of interest
+            data2 : pandas DataFrame
+                data 
+        
+        Returns
+        -------
+            near : numpy.ndarray
+                nearest neighbors
         """ 
+        
         locx = loc[0]
         locy = loc[1]
         data = data2.copy()
         centered_array = NearestNeighbor.center(data['X'].values, data['Y'].values, 
                                 locx, locy)
         data["dist"] = NearestNeighbor.distance_calculator(centered_array) 
         data["angles"] = NearestNeighbor.angle_calculator(centered_array)
@@ -250,23 +330,34 @@
         near = smallest[~np.isnan(smallest)].reshape(-1,3) 
         
         return near
     
     def nearest_neighbor_search_cluster(radius, num_points, loc, data2):
         """
         Nearest neighbor octant search when doing sgs with clusters
-        Inputs:
-            radius - search radius
-            num_points - number of points to search for
-            loc - coordinates for grid cell of interest
-            data2 - data 
-        Outputs:
-            near - nearest neighbors
-            cluster_number - nearest neighbor cluster number
+        
+        Parameters
+        ----------
+            radius : int, float
+                search radius
+            num_points : int
+                number of points to search for
+            loc : numpy.ndarray
+                coordinates for grid cell of interest
+            data2 : pandas DataFrame
+                data 
+        
+        Returns
+        -------
+            near : numpy.ndarray
+                nearest neighbors
+            cluster_number : int
+                nearest neighbor cluster number
         """ 
+        
         locx = loc[0]
         locy = loc[1]
         data = data2.copy()
         centered_array = NearestNeighbor.center(data['X'].values, data['Y'].values, 
                                 locx, locy)
         data["dist"] = NearestNeighbor.distance_calculator(centered_array)
         data["angles"] = NearestNeighbor.angle_calculator(centered_array)
@@ -287,20 +378,28 @@
         near = smallest[~np.isnan(smallest)].reshape(-1,3) 
         
         return near, cluster_number
 
     def nearest_neighbor_secondary(loc, data2):
         """
         Find the neareset neighbor secondary data point to grid cell of interest
-        Inputs:
-            loc - coordinates for grid cell of interest
-            data2 - secondary data
-        Outputs:
-            nearest_second - nearest neighbor value to secondary data
+        
+        Parameters
+        ----------
+            loc : numpy.ndarray
+                coordinates for grid cell of interest
+            data2 : pandas DataFrame
+                secondary data
+        
+        Returns
+        -------
+            nearest_second : float
+                nearest neighbor value to secondary data
         """ 
+        
         locx = loc[0]
         locy = loc[1]
         data = data2.copy()
         centered_array = NearestNeighbor.center(data['X'].values, data['Y'].values, 
                                 locx, locy)
         data["dist"] = NearestNeighbor.distance_calculator(centered_array)
         data = data.sort_values('dist', ascending = True) 
@@ -308,26 +407,39 @@
         nearest_second = data.iloc[0][['X','Y','Z']].values 
         
         return nearest_second
 
     def find_colocated(df1, xx1, yy1, zz1, df2, xx2, yy2, zz2): 
         """
         Find colocated data between primary and secondary variables
-        Inputs:
-            df1 - data frame of primary conditioning data
-            xx1 - column name for x coordinates of input data frame for primary data
-            yy1 - column name for y coordinates of input data frame for primary data
-            zz1 - column for z values (or data variable) of input data frame for primary data
-            df2 - data frame of secondary data
-            xx2 - column name for x coordinates of input data frame for secondary data
-            yy2 - column name for y coordinates of input data frame for secondary data
-            zz2 - column for z values (or data variable) of input data frame for secondary data
-        Outputs:
-            df_colocated - data frame of colocated values
+        
+        Parameters
+        ----------
+            df1 : pandas DataFrame
+                data frame of primary conditioning data
+            xx1 : string
+                column name for x coordinates of input data frame for primary data
+            yy1 : string
+                column name for y coordinates of input data frame for primary data
+            zz1 : string
+                column for z values (or data variable) of input data frame for primary data
+            df2 : pandas DataFrame
+                data frame of secondary data
+            xx2 : string
+                column name for x coordinates of input data frame for secondary data
+            yy2 : string
+                column name for y coordinates of input data frame for secondary data
+            zz2 : string
+                column for z values (or data variable) of input data frame for secondary data
+        Returns
+        -------
+            df_colocated : pandas DataFrame
+                data frame of colocated values
         """ 
+        
         df1 = df1.rename(columns = {xx1: "X", yy1: "Y", zz1: "Z"}) 
         df2 = df2.rename(columns = {xx2: "X", yy2: "Y", zz2: "Z"}) 
         secondary_variable_xy = df2[['X','Y']].values
         secondary_variable_tree = KDTree(secondary_variable_xy) 
         primary_variable_xy = df1[['X','Y']].values
         nearest_indices = np.zeros(len(primary_variable_xy)) 
 
@@ -348,27 +460,41 @@
 # adaptive partioning
 
 ###############################
 
 def adaptive_partitioning(df_data, xmin, xmax, ymin, ymax, i, max_points, min_length, max_iter=None):
     """
     Rercursively split clusters until they are all below max_points, but don't go smaller than min_length
-    Inputs:
-        df_data - DataFrame with X, Y, and K (cluster id)
-        xmin - min x value of this partion
-        xmax - max x value of this partion
-        ymin - min y value of this partion
-        ymax - max y value of this partion
-        i - keeps track of total calls to this function
-        max_points - all clusters will be "quartered" until points below this
-        min_length - minimum side length of sqaures, preference over max_points
-        max_iter - maximum iterations if worried about unending recursion
-    Outputs:
-        df_data - updated DataFrame with new cluster assigned the next integer
-        i - number of iterations
+    
+    Parameters
+    ----------
+        df_data : pandas DataFrame 
+            DataFrame with X, Y, and K (cluster id) columns
+        xmin : float
+            min x value of this partion
+        xmax : float
+            max x value of this partion
+        ymin : float
+            min y value of this partion
+        ymax : float
+            max y value of this partion
+        i : int
+            keeps track of total calls to this function
+        max_points : int
+            all clusters will be "quartered" until points below this
+        min_length : float
+            minimum side length of sqaures, preference over max_points
+        max_iter : int
+            maximum iterations if worried about unending recursion
+    Returns
+    -------
+        df_data : pandas DataFrame
+            updated DataFrame with new cluster assigned
+        i : int
+            number of iterations
     """
     # optional 'safety' if there is concern about runaway recursion
     if max_iter is not None:
         if i >= max_iter:
             return df_data, i
     
     dx = xmax - xmin
@@ -410,21 +536,30 @@
 # Rotation Matrix
 
 #########################
 
 def make_rotation_matrix(azimuth, major_range, minor_range):
     """
     Make rotation matrix for accommodating anisotropy
-    Inputs:
-        azimuth - angle (in degrees from horizontal) of axis of orientation
-        major_range - range parameter of variogram in major direction, or azimuth
-        minor_range - range parameter of variogram in minor direction, or orthogonal to azimuth
-    Outputs:
-        rotation_matrix - 2x2 rotation matrix used to perform coordinate transformations
+    
+    Parameters
+    ----------
+        azimuth : int, float
+            angle (in degrees from horizontal) of axis of orientation
+        major_range : int, float
+            range parameter of variogram in major direction, or azimuth
+        minor_range : int, float
+            range parameter of variogram in minor direction, or orthogonal to azimuth
+    
+    Returns
+    -------
+        rotation_matrix : numpy.ndarray
+            2x2 rotation matrix used to perform coordinate transformations
     """
+    
     theta = (azimuth / 180.0) * np.pi 
     
     rotation_matrix = np.dot(
         np.array([[np.cos(theta), -np.sin(theta)],
                 [np.sin(theta), np.cos(theta)],]),
         np.array([[1 / major_range, 0], [0, 1 / minor_range]]))
     
@@ -434,90 +569,146 @@
 ###########################
 
 # Covariance functions
 
 ###########################
 
 class Covariance:
-
-    def covar(effective_lag, sill, nug):
+    
+    def covar(effective_lag, sill, nug, vtype):
         """
-        Compute covariance using exponential covariance model
-        Inputs:
-            effective_lag - lag distance that is normalized to a range of 1
-            sill - sill of variogram
-            nug - nugget of variogram
-        Outputs:
-            c - covariance
+        Compute covariance
+        
+        Parameters
+        ----------
+            effective_lag : int, float
+                lag distance that is normalized to a range of 1
+            sill : int, float
+                sill of variogram
+            nug : int, float
+                nugget of variogram
+            vtype : string
+                type of variogram model (Exponential, Gaussian, or Spherical)
+        
+        Returns
+        -------
+            c : numpy.ndarray
+                covariance
         """
-        c = (sill - nug)*np.exp(-3 * effective_lag)
-
+        
+        if vtype == 'Exponential':
+            c = (sill - nug)*np.exp(-3 * effective_lag)
+        elif vtype == 'Gaussian':
+            c = (sill - nug)*np.exp(-3 * np.square(effective_lag))
+        elif vtype == 'Spherical':
+            c = sill - nug - 1.5 * effective_lag + 0.5 * np.power(effective_lag, 3)
+            c[effective_lag > 1] = sill - 1
         return c
 
     def make_covariance_matrix(coord, vario, rotation_matrix):
         """
         Make covariance matrix showing covariances between each pair of input coordinates
-        Inputs:
-            coord - coordinates of data points
-            vario - array of variogram parameters
-            rotation_matrix - rotation matrix used to perform coordinate transformations
-        Outputs:
-            covariance_matrix - nxn matrix of covariance between n points
+        
+        Parameters
+        ----------
+            coord : numpy.ndarray
+                coordinates of data points
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            rotation_matrix : numpy.ndarray
+                rotation matrix used to perform coordinate transformations
+        
+        Returns
+        -------
+            covariance_matrix : numpy.ndarray 
+                nxn matrix of covariance between n points
         """
+        
         nug = vario[1]
-        sill = vario[4]   
+        sill = vario[4]  
+        vtype = vario[5]
         mat = np.matmul(coord, rotation_matrix)
         effective_lag = pairwise_distances(mat,mat) 
-        covariance_matrix = Covariance.covar(effective_lag, sill, nug) 
+        covariance_matrix = Covariance.covar(effective_lag, sill, nug, vtype) 
 
         return covariance_matrix
 
     def make_covariance_array(coord1, coord2, vario, rotation_matrix):
         """
         Make covariance array showing covariances between each data points and grid cell of interest
-        Inputs:
-            coord1 - coordinates of n data points
-            coord2 - coordinates of grid cell of interest (i.e. grid cell being simulated) that is repeated n times
-            vario - array of variogram parameters
+        
+        Parameters
+        ----------
+            coord1 : numpy.ndarray
+                coordinates of n data points
+            coord2 : numpy.ndarray
+                coordinates of grid cell of interest (i.e. grid cell being simulated) that is repeated n times
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
             rotation_matrix - rotation matrix used to perform coordinate transformations
-        Outputs:
-            covariance_array - nx1 array of covariance between n points and grid cell of interest
+        
+        Returns
+        -------
+            covariance_array : numpy.ndarray
+                nx1 array of covariance between n points and grid cell of interest
         """
+        
         nug = vario[1]
         sill = vario[4]
+        vtype = vario[5]
         mat1 = np.matmul(coord1, rotation_matrix) 
         mat2 = np.matmul(coord2.reshape(-1,2), rotation_matrix) 
         effective_lag = np.sqrt(np.square(mat1 - mat2).sum(axis=1))
-        covariance_array = Covariance.covar(effective_lag, sill, nug)
+        covariance_array = Covariance.covar(effective_lag, sill, nug, vtype)
 
         return covariance_array
 
 ######################################
 
 # Simple Kriging Function
 
 ######################################
 
 class Interpolation: 
 
     def skrige(prediction_grid, df, xx, yy, zz, num_points, vario, radius):
         """
         Simple kriging interpolation
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df - data frame of conditioning data
-            xx - column name for x coordinates of input data frame
-            yy - column name for y coordinates of input data frame
-            zz - column for z values (or data variable) of input data frame
-            num_points - the number of conditioning points to search for
-            vario - numpy array of variogram parameters describing the spatial statistics
-            radius - search radius
-        Outputs:
-            est_sk - simple kriging estimate for each coordinate in prediction_grid
-            var_sk - simple kriging variance 
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df : pandas DataFrame
+                data frame of conditioning data
+            xx : string
+                column name for x coordinates of input data frame
+            yy : string 
+                column name for y coordinates of input data frame
+            zz : string
+                column for z values (or data variable) of input data frame
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+        
+        Returns
+        -------
+            est_sk : numpy.ndarray
+                simple kriging estimate for each coordinate in prediction_grid
+            var_sk : numpy.ndarray 
+                simple kriging variance 
         """
         
         # unpack variogram parameters
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
@@ -556,35 +747,52 @@
                 # covariance between data points
                 covariance_matrix.reshape(((new_num_pts)), ((new_num_pts)))
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, 
                                                           covariance_array, rcond = None)
 
                 est_sk[z] = mean_1 + (np.sum(k_weights*(norm_data_val[:] - mean_1))) 
                 var_sk[z] = var_1 - np.sum(k_weights*covariance_array)
+                #var_sk[z] = np.absolute(var_sk[z])
+                var_sk[var_sk < 0] = 0
             else:
                 est_sk[z] = df['Z'].values[np.where(test_idx==2)[0][0]]
                 var_sk[z] = 0
-
         return est_sk, var_sk
 
     def okrige(prediction_grid, df, xx, yy, zz, num_points, vario, radius):
         """
         Ordinary kriging interpolation
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df - data frame of conditioning data
-            xx - column name for x coordinates of input data frame
-            yy - column name for y coordinates of input data frame
-            zz - column for z values (or data variable) of input data frame
-            num_points - the number of conditioning points to search for
-            vario - numpy array of variogram parameters describing the spatial statistics
-            radius - search radius
-        Outputs:
-            est_ok - ordinary kriging estimate for each coordinate in prediction_grid
-            var_ok - ordinary kriging variance 
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df : pandas DataFrame
+                data frame of conditioning data
+            xx : string
+                column name for x coordinates of input data frame
+            yy : string 
+                column name for y coordinates of input data frame
+            zz : string
+                column for z values (or data variable) of input data frame
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+        
+        Returns
+        -------
+            est_ok : numpy.ndarray
+                ordinary kriging estimate for each coordinate in prediction_grid
+            var_ok : numpy.ndarray
+                ordinary kriging variance 
         """
 
         # unpack variogram parameters
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
@@ -624,34 +832,50 @@
                 covariance_array[new_num_pts] = 1 
                 covariance_matrix.reshape(((new_num_pts+1)), ((new_num_pts+1)))
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, 
                                                           covariance_array, rcond = None) 
                 
                 est_ok[z] = local_mean + np.sum(k_weights[0:new_num_pts]*(norm_data_val[:] - local_mean)) 
                 var_ok[z] = var_1 - np.sum(k_weights[0:new_num_pts]*covariance_array[0:new_num_pts])
+                #var_ok[z] = np.absolute(var_ok[z])
+                var_ok[var_ok < 0] = 0
             else:
                 est_ok[z] = df['Z'].values[np.where(test_idx==2)[0][0]]
-                var_ok[z] = 0
-
+                var_ok[z] = 0   
         return est_ok, var_ok
   
     def skrige_sgs(prediction_grid, df, xx, yy, zz, num_points, vario, radius):
         """
         Sequential Gaussian simulation using simple kriging 
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df - data frame of conditioning data
-            xx - column name for x coordinates of input data frame
-            yy - column name for y coordinates of input data frame
-            zz - column for z values (or data variable) of input data frame
-            num_points - the number of conditioning points to search for
-            vario - numpy array of variogram parameters describing the spatial statistics
-            radius - search radius
-        Outputs:
-            sgs - simulated value for each coordinate in prediction_grid
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df : pandas DataFrame
+                data frame of conditioning data
+            xx : string
+                column name for x coordinates of input data frame
+            yy : string 
+                column name for y coordinates of input data frame
+            zz : string
+                column for z values (or data variable) of input data frame
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+        
+        Returns
+        -------
+            sgs : numpy.ndarray
+                simulated value for each coordinate in prediction_grid
         """
 
         # unpack variogram parameters
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
@@ -701,25 +925,40 @@
                                              'Z': [sgs[z]]})], sort=False) 
 
         return sgs
    
     def okrige_sgs(prediction_grid, df, xx, yy, zz, num_points, vario, radius):
         """
         Sequential Gaussian simulation using ordinary kriging 
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df - data frame of conditioning data
-            xx - column name for x coordinates of input data frame
-            yy - column name for y coordinates of input data frame
-            zz - column for z values (or data variable) of input data frame
-            num_points - the number of conditioning points to search for
-            vario - numpy array of variogram parameters describing the spatial statistics
-            radius - search radius
-        Outputs:
-            sgs - simulated value for each coordinate in prediction_grid
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df : pandas DataFrame
+                data frame of conditioning data
+            xx : string
+                column name for x coordinates of input data frame
+            yy : string 
+                column name for y coordinates of input data frame
+            zz : string
+                column for z values (or data variable) of input data frame
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+        
+        Returns
+        -------
+            sgs : numpy.ndarray
+                simulated value for each coordinate in prediction_grid
         """
 
         # unpack variogram parameters
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
@@ -774,27 +1013,43 @@
 
         return sgs
 
 
     def cluster_sgs(prediction_grid, df, xx, yy, zz, kk, num_points, df_gamma, radius):
         """
         Sequential Gaussian simulation where variogram parameters are different for each k cluster. Uses simple kriging 
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df - data frame of conditioning data
-            xx - column name for x coordinates of input data frame
-            yy - column name for y coordinates of input data frame
-            zz - column for z values (or data variable) of input data frame
-            kk - column of k cluster numbers for each point
-            num_points - the number of conditioning points to search for
-            df_gamma - dataframe with variogram parameters for each cluster
-            radius - search radius
-        Outputs:
-            sgs - simulated value for each coordinate in prediction_grid
-        """ 
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df : pandas DataFrame
+                data frame of conditioning data
+            xx : string
+                column name for x coordinates of input data frame
+            yy : string 
+                column name for y coordinates of input data frame
+            zz : string
+                column for z values (or data variable) of input data frame
+            kk : string
+                column of k cluster numbers for each point
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+        
+        Returns
+        -------
+            sgs : numpy.ndarray
+                simulated value for each coordinate in prediction_grid
+        """
 
         df = df.rename(columns = {xx: "X", yy: "Y", zz: "Z", kk: "K"})  
         xyindex = np.arange(len(prediction_grid)) 
         random.shuffle(xyindex)
         mean_1 = np.average(df["Z"].values) 
         sgs = np.zeros(shape=len(prediction_grid)) 
 
@@ -847,45 +1102,65 @@
                                              'Z': [sgs[z]], 'K': [cluster_number]})], sort=False)
 
         return sgs
 
     def cokrige_mm1(prediction_grid, df1, xx1, yy1, zz1, df2, xx2, yy2, zz2, num_points, vario, radius, corrcoef):
         """
         Simple collocated cokriging under Markov model 1 assumptions
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df1 - data frame of primary conditioning data
-            xx1 - column name for x coordinates of input data frame for primary data
-            yy1 - column name for y coordinates of input data frame for primary data
-            zz1 - column for z values (or data variable) of input data frame for primary data
-            df2 - data frame of secondary data
-            xx2 - column name for x coordinates of input data frame for secondary data
-            yy2 - column name for y coordinates of input data frame for secondary data
-            zz2 - column for z values (or data variable) of input data frame for secondary data
-            num_points - the number of conditioning points to search for
-            vario - numpy array of variogram parameters describing the spatial statistics
-            radius - search radius
-            corrcoef - correlation coefficient between primary and secondary data
-        Outputs:
-            est_cokrige - cokriging estimate for each point in coordinate grid
-            var_cokrige - variances
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df1 : pandas DataFrame
+                data frame of primary conditioning data
+            xx1 : string
+                column name for x coordinates of input data frame for primary data
+            yy1 : string 
+                column name for y coordinates of input data frame for primary data
+            zz1 : string
+                column for z values (or data variable) of input data frame for primary data
+            df2 : pandas DataFrame
+                data frame of secondary data
+            xx2 : string
+                column name for x coordinates of input data frame for secondary data
+            yy2 : string
+                column name for y coordinates of input data frame for secondary data
+            zz2 : string
+                column for z values (or data variable) of input data frame for secondary data
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+            corrcoef : float
+                correlation coefficient between primary and secondary data
+        
+        Returns
+        -------
+            est_cokrige : numpy.ndarray
+                cokriging estimate for each point in coordinate grid
+            var_cokrige : numpy.ndarray
+                cokriging variances
         """
         
         # unpack variogram parameters for rotation matrix
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range) 
 
         df1 = df1.rename(columns = {xx1: "X", yy1: "Y", zz1: "Z"})
         df2 = df2.rename(columns = {xx2: "X", yy2: "Y", zz2: "Z"})
 
         mean_1 = np.average(df1['Z']) 
-        var_1 = np.var(df1['Z'])
-        vario[4] = np.var(df1['Z'])
+        var_1 = vario[4]
         mean_2 = np.average(df2['Z']) 
         var_2 = np.var(df2['Z'])
 
         est_cokrige = np.zeros(shape=len(prediction_grid)) 
         var_cokrige = np.zeros(shape=len(prediction_grid))
 
         for z, predxy in enumerate(tqdm(prediction_grid, position=0, leave=True)):
@@ -929,55 +1204,74 @@
 
                 # solve kriging system
                 k_weights, res, rank, s = np.linalg.lstsq(covariance_matrix, covariance_array, rcond = None) 
                 part1 = mean_1 + np.sum(k_weights[0:new_num_pts]*(norm_data_val[0:new_num_pts] - mean_1)/np.sqrt(var_1))
                 part2 = k_weights[new_num_pts] * (nearest_second[-1] - mean_2)/np.sqrt(var_2)
                                
                 est_cokrige[z] = part1 + part2 
-                var_cokrige[z] = var_1 - np.sum(k_weights*covariance_array)
+                var_cokrige[z] = var_1 - np.sum(k_weights[0:new_num_pts+1]*covariance_array[0:new_num_pts+1]) 
             else:
                 est_cokrige[z] = df1['Z'].values[np.where(test_idx==2)[0][0]]
                 var_cokrige[z] = 0
 
         return est_cokrige, var_cokrige
 
     def cosim_mm1(prediction_grid, df1, xx1, yy1, zz1, df2, xx2, yy2, zz2, num_points, vario, radius, corrcoef):
         """
         Cosimulation under Markov model 1 assumptions
-        Inputs:
-            prediction_grid - x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
-            df1 - data frame of primary conditioning data
-            xx1 - column name for x coordinates of input data frame for primary data
-            yy1 - column name for y coordinates of input data frame for primary data
-            zz1 - column for z values (or data variable) of input data frame for primary data
-            df2 - data frame of secondary data
-            xx2 - column name for x coordinates of input data frame for secondary data
-            yy2 - column name for y coordinates of input data frame for secondary data
-            zz2 - column for z values (or data variable) of input data frame for secondary data
-            num_points - the number of conditioning points to search for
-            vario - numpy array of variogram parameters describing the spatial statistics
-            radius - search radius
-            corrcoef - correlation coefficient between primary and secondary data
-        Outputs:
-            cosim - cosimulation for each point in coordinate grid
+        
+        Parameters
+        ----------
+            prediction_grid : numpy.ndarray
+                x,y coordinate numpy array of prediction grid, or grid cells that will be estimated
+            df1 : pandas DataFrame
+                data frame of primary conditioning data
+            xx1 : string
+                column name for x coordinates of input data frame for primary data
+            yy1 : string 
+                column name for y coordinates of input data frame for primary data
+            zz1 : string
+                column for z values (or data variable) of input data frame for primary data
+            df2 : pandas DataFrame
+                data frame of secondary data
+            xx2 : string
+                column name for x coordinates of input data frame for secondary data
+            yy2 : string
+                column name for y coordinates of input data frame for secondary data
+            zz2 : string
+                column for z values (or data variable) of input data frame for secondary data
+            num_points : int
+                the number of conditioning points to search for
+            vario : list
+                list of variogram parameters [azimuth, nugget, major_range, minor_range, sill, vtype]
+                azimuth, nugget, major_range, minor_range, and sill can be int or float type
+                vtype is a string that can be either 'Exponential', 'Spherical', or 'Gaussian'
+            radius : int, float
+                search radius
+            corrcoef : float
+                correlation coefficient between primary and secondary data
+        
+        Returns
+        -------
+            cosim : numpy.ndarray
+                cosimulation for each point in coordinate grid
         """
             
         # unpack variogram parameters
         azimuth = vario[0]
         major_range = vario[2]
         minor_range = vario[3]
         rotation_matrix = make_rotation_matrix(azimuth, major_range, minor_range)
         df1 = df1.rename(columns = {xx1: "X", yy1: "Y", zz1: "Z"}) 
         df2 = df2.rename(columns = {xx2: "X", yy2: "Y", zz2: "Z"})
         xyindex = np.arange(len(prediction_grid)) 
         random.shuffle(xyindex)
 
         mean_1 = np.average(df1['Z']) 
-        var_1 = np.var(df1['Z'])
-        vario[4] = np.var(df1['Z'])
+        var_1 = vario[4]
         mean_2 = np.average(df2['Z']) 
         var_2 = np.var(df2['Z'])
    
         cosim = np.zeros(shape=len(prediction_grid))
 
         # for each coordinate in the prediction grid
         for idx, predxy in enumerate(tqdm(prediction_grid, position=0, leave=True)):
@@ -1009,15 +1303,15 @@
                 covariance_array = np.zeros(shape=(new_num_pts + 1)) 
                 k_weights = np.zeros(shape=(new_num_pts + 1))
                 covariance_array[0:new_num_pts+1] = Covariance.make_covariance_array(xy_val, 
                                                                                      np.tile(prediction_grid[z], 
                                                                                              new_num_pts + 1), 
                                                                                      vario, rotation_matrix)
                 covariance_array[new_num_pts] = covariance_array[new_num_pts] * corrcoef 
-                
+
                 # update covariance matrix with secondary info (gamma2 = rho12 * gamma1)
                 covariance_matrix[new_num_pts, 0 : new_num_pts+1] = covariance_matrix[new_num_pts, 0 : new_num_pts+1] * corrcoef
                 covariance_matrix[0 : new_num_pts+1, new_num_pts] = covariance_matrix[0 : new_num_pts+1, new_num_pts] * corrcoef
                 covariance_matrix[new_num_pts, new_num_pts] = 1
                 covariance_matrix.reshape(((new_num_pts + 1)), ((new_num_pts + 1)))
 
                 # solve kriging system
```

### Comparing `gstatsim-1.0.1/setup.py` & `gstatsim-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.1'
+version = '1.0.2'
 
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
```

