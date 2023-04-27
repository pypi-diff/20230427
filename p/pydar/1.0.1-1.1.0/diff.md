# Comparing `tmp/pydar-1.0.1.tar.gz` & `tmp/pydar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydar-1.0.1.tar", last modified: Thu Apr 13 21:16:43 2023, max compression
+gzip compressed data, was "dist/pydar-1.1.0.tar", last modified: Thu Apr 27 20:39:06 2023, max compression
```

## Comparing `pydar-1.0.1.tar` & `pydar-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.188861 pydar-1.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-01-04 06:11:53.000000 pydar-1.0.1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    49602 2023-04-13 21:16:43.188861 pydar-1.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    42710 2023-04-13 21:12:32.000000 pydar-1.0.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.180862 pydar-1.0.1/pydar/
--rw-rw-r--   0 user      (1000) user      (1000)     2345 2023-03-25 01:17:08.000000 pydar-1.0.1/pydar/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.188861 pydar-1.0.1/pydar/data/
--rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-01-01 06:47:05.000000 pydar-1.0.1/pydar/data/cassini_flyby.csv
--rw-rw-r--   0 user      (1000) user      (1000)    15662 2023-02-19 01:03:57.000000 pydar-1.0.1/pydar/data/coradr_jpl_options.csv
--rw-rw-r--   0 user      (1000) user      (1000)    30062 2023-02-19 01:20:45.000000 pydar-1.0.1/pydar/data/feature_name_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)    36144 2023-01-13 02:14:43.000000 pydar-1.0.1/pydar/data/sar_swath_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)   545452 2023-02-19 01:17:22.000000 pydar-1.0.1/pydar/data/swath_coverage_by_time_position.csv
--rw-rw-r--   0 user      (1000) user      (1000)     1774 2023-03-29 19:49:01.000000 pydar-1.0.1/pydar/display_image.py
--rw-rw-r--   0 user      (1000) user      (1000)    20504 2023-04-13 20:28:45.000000 pydar-1.0.1/pydar/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    15942 2023-04-12 19:20:45.000000 pydar-1.0.1/pydar/extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-03-29 22:21:31.000000 pydar-1.0.1/pydar/pydar_testing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.188861 pydar-1.0.1/pydar/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     4488 2023-04-13 20:31:01.000000 pydar-1.0.1/pydar/pytests/test_display_image.py
--rw-rw-r--   0 user      (1000) user      (1000)    14238 2023-04-13 20:14:27.000000 pydar-1.0.1/pydar/pytests/test_extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     9129 2023-04-13 21:00:32.000000 pydar-1.0.1/pydar/pytests/test_read_readme.py
--rw-rw-r--   0 user      (1000) user      (1000)    32985 2023-04-13 21:11:44.000000 pydar-1.0.1/pydar/pytests/test_retrieve_ids_by_time_position.py
--rw-rw-r--   0 user      (1000) user      (1000)    12401 2023-04-13 01:01:16.000000 pydar-1.0.1/pydar/read_readme.py
--rw-rw-r--   0 user      (1000) user      (1000)    14306 2023-04-13 03:32:41.000000 pydar-1.0.1/pydar/retrieve_ids_by_time_position.py
--rw-rw-r--   0 user      (1000) user      (1000)     4081 2023-03-18 07:53:32.000000 pydar-1.0.1/pydar/retrieve_supplementary_backplanes.py
--rw-rw-r--   0 user      (1000) user      (1000)    12251 2023-02-25 05:04:59.000000 pydar-1.0.1/pydar/sbdr_make_shapefile.py
--rw-rw-r--   0 user      (1000) user      (1000)      969 2023-02-18 06:42:56.000000 pydar-1.0.1/pydar/test_bearing_correction.py
--rw-rw-r--   0 user      (1000) user      (1000)     3021 2023-03-21 20:49:44.000000 pydar-1.0.1/pydar/updateCsvCORADARJPLOptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     4075 2023-03-21 20:49:20.000000 pydar-1.0.1/pydar/updateCsvFeatureNameDetails.py
--rw-rw-r--   0 user      (1000) user      (1000)     5609 2023-03-21 20:48:33.000000 pydar-1.0.1/pydar/updateCsvSwathCoverage.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.184862 pydar-1.0.1/pydar.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    49602 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      914 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      132 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-13 21:16:43.188861 pydar-1.0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1669 2023-04-13 20:45:18.000000 pydar-1.0.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-27 20:39:06.115614 pydar-1.1.0/
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2023-01-04 06:11:53.000000 pydar-1.1.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    49984 2023-04-27 20:39:06.115614 pydar-1.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    43076 2023-04-27 20:25:19.000000 pydar-1.1.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-27 20:39:06.103614 pydar-1.1.0/pydar/
+-rw-rw-r--   0 user      (1000) user      (1000)     2345 2023-03-25 01:17:08.000000 pydar-1.1.0/pydar/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-27 20:39:06.107614 pydar-1.1.0/pydar/data/
+-rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-01-01 06:47:05.000000 pydar-1.1.0/pydar/data/cassini_flyby.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    15662 2023-02-19 01:03:57.000000 pydar-1.1.0/pydar/data/coradr_jpl_options.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    30062 2023-02-19 01:20:45.000000 pydar-1.1.0/pydar/data/feature_name_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    36144 2023-01-13 02:14:43.000000 pydar-1.1.0/pydar/data/sar_swath_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)   545452 2023-02-19 01:17:22.000000 pydar-1.1.0/pydar/data/swath_coverage_by_time_position.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     1971 2023-04-26 21:55:32.000000 pydar-1.1.0/pydar/display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20671 2023-04-26 21:56:00.000000 pydar-1.1.0/pydar/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15942 2023-04-12 19:20:45.000000 pydar-1.1.0/pydar/extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2023-03-29 22:21:31.000000 pydar-1.1.0/pydar/pydar_testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-27 20:39:06.111614 pydar-1.1.0/pydar/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     4980 2023-04-26 22:07:48.000000 pydar-1.1.0/pydar/pytests/test_display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14238 2023-04-13 20:14:27.000000 pydar-1.1.0/pydar/pytests/test_extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9129 2023-04-13 21:00:32.000000 pydar-1.1.0/pydar/pytests/test_read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32985 2023-04-13 21:11:44.000000 pydar-1.1.0/pydar/pytests/test_retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12401 2023-04-13 01:01:16.000000 pydar-1.1.0/pydar/read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14306 2023-04-13 03:32:41.000000 pydar-1.1.0/pydar/retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4081 2023-03-18 07:53:32.000000 pydar-1.1.0/pydar/retrieve_supplementary_backplanes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12251 2023-02-25 05:04:59.000000 pydar-1.1.0/pydar/sbdr_make_shapefile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      969 2023-02-18 06:42:56.000000 pydar-1.1.0/pydar/test_bearing_correction.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3021 2023-03-21 20:49:44.000000 pydar-1.1.0/pydar/updateCsvCORADARJPLOptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4075 2023-03-21 20:49:20.000000 pydar-1.1.0/pydar/updateCsvFeatureNameDetails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5609 2023-03-21 20:48:33.000000 pydar-1.1.0/pydar/updateCsvSwathCoverage.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-27 20:39:06.103614 pydar-1.1.0/pydar.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    49984 2023-04-27 20:39:06.000000 pydar-1.1.0/pydar.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      914 2023-04-27 20:39:06.000000 pydar-1.1.0/pydar.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-27 20:39:06.000000 pydar-1.1.0/pydar.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      126 2023-04-27 20:39:06.000000 pydar-1.1.0/pydar.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-27 20:39:06.000000 pydar-1.1.0/pydar.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-27 20:39:06.115614 pydar-1.1.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1663 2023-04-27 20:26:16.000000 pydar-1.1.0/setup.py
```

### Comparing `pydar-1.0.1/PKG-INFO` & `pydar-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.1.0.tar.gz
 Description: # PYDAR
          <p align="center">
           <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/pydar)
         ![license](https://img.shields.io/pypi/l/pydar)
@@ -651,24 +651,26 @@
         <br>
         ['PRODUCT DESCRIPTION', 'DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES', 'POINTERS TO START RECORDS OF OBJECTS IN FILE', 'DESCRIPTION OF OBJECTS CONTAINED IN FILE']
         </details>
         
         ## Use Downloaded Data
         ### displayImages()
         
+        Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
+        
         ```
-        displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120)
+        displayImages(image_directory=None, fig_title=None, cmap="gray", figsize_n=6, fig_dpi=120)
         ```
         
-        * **[REQUIRED]** image_directory (string): directory containing pydar_results with IMG file
+        * **[REQUIRED]** image_directory (string): directory containing a .LBL and .IMG file
         * [OPTIONAL] fig_title (str): figure title, defaults to filename
+        * [OPTIONAL] cmap (str): optional colormaps ([see more options](https://matplotlib.org/stable/tutorials/colors/colormaps.html)), defaults to 'gray'
         * [OPTIONAL] figsize_n (int): plot dimensions, defaults to 6x6
         * [OPTIONAL] fig_dpi (int): plot dpi, defaults to 120
         
-        Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
         
         ```python
         import pydar
         pydar.displayImages(image_directory="pydar_results/CORADR_0065_V03_S01")
         ```
          <p align="center">
           <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
@@ -682,16 +684,14 @@
         
         COMING SOON: Extract metadata from .TAB file (using .FMT as a reference)
         
         ## Developer Notes TODO:
         ### TODO Code:
         * add a colored outline around a feature when displaying as a 2D image
         * save image pixel to an array
-        * extract pdr functionality to reduce overhead
-        * displayImages() bug fix: 87 displays invalid integer
         * segments will be less than 99 (default to 1 - 01 is the primary imaging) (requires segment_options = ['S01', 'S02', 'S03', 'S04'])
         * progress bars print to command line (still downloading...)
         * save .IMG as .SHP for ArcGIS
         
         ### TODO Questions:
         * add details for what a segment_num is
         * associate burst ID from SBDR data to BIDR data for metadata
@@ -712,14 +712,16 @@
         * test: pull beam information and number of looks for each pixel 
         
         ## Credits
         Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
         
         Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
         
+        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not neccessarily reflect the views of the National Science Foundation.
+        
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/unaschneck/pydar/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pydar-1.0.1/README.md` & `pydar-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -643,24 +643,26 @@
 <br>
 ['PRODUCT DESCRIPTION', 'DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES', 'POINTERS TO START RECORDS OF OBJECTS IN FILE', 'DESCRIPTION OF OBJECTS CONTAINED IN FILE']
 </details>
 
 ## Use Downloaded Data
 ### displayImages()
 
+Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
+
 ```
-displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120)
+displayImages(image_directory=None, fig_title=None, cmap="gray", figsize_n=6, fig_dpi=120)
 ```
 
-* **[REQUIRED]** image_directory (string): directory containing pydar_results with IMG file
+* **[REQUIRED]** image_directory (string): directory containing a .LBL and .IMG file
 * [OPTIONAL] fig_title (str): figure title, defaults to filename
+* [OPTIONAL] cmap (str): optional colormaps ([see more options](https://matplotlib.org/stable/tutorials/colors/colormaps.html)), defaults to 'gray'
 * [OPTIONAL] figsize_n (int): plot dimensions, defaults to 6x6
 * [OPTIONAL] fig_dpi (int): plot dpi, defaults to 120
 
-Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
 
 ```python
 import pydar
 pydar.displayImages(image_directory="pydar_results/CORADR_0065_V03_S01")
 ```
  <p align="center">
   <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
@@ -674,16 +676,14 @@
 
 COMING SOON: Extract metadata from .TAB file (using .FMT as a reference)
 
 ## Developer Notes TODO:
 ### TODO Code:
 * add a colored outline around a feature when displaying as a 2D image
 * save image pixel to an array
-* extract pdr functionality to reduce overhead
-* displayImages() bug fix: 87 displays invalid integer
 * segments will be less than 99 (default to 1 - 01 is the primary imaging) (requires segment_options = ['S01', 'S02', 'S03', 'S04'])
 * progress bars print to command line (still downloading...)
 * save .IMG as .SHP for ArcGIS
 
 ### TODO Questions:
 * add details for what a segment_num is
 * associate burst ID from SBDR data to BIDR data for metadata
@@ -704,10 +704,12 @@
 * test: pull beam information and number of looks for each pixel 
 
 ## Credits
 Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
 Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
 
+This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not neccessarily reflect the views of the National Science Foundation.
+
 ## Bug and Feature Request
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/unaschneck/pydar/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `pydar-1.0.1/pydar/__init__.py` & `pydar-1.1.0/pydar/__init__.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/data/cassini_flyby.csv` & `pydar-1.1.0/pydar/data/cassini_flyby.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/data/coradr_jpl_options.csv` & `pydar-1.1.0/pydar/data/coradr_jpl_options.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/data/feature_name_details.csv` & `pydar-1.1.0/pydar/data/feature_name_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/data/sar_swath_details.csv` & `pydar-1.1.0/pydar/data/sar_swath_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/data/swath_coverage_by_time_position.csv` & `pydar-1.1.0/pydar/data/swath_coverage_by_time_position.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/display_image.py` & `pydar-1.1.0/pydar/display_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 ## Display PDR images in Matplotlib
 
 # Built in Python functions
 import logging
 import os
 
 # External Python libraries (installed via pip install)
-from planetaryimage import PDS3Image
+import rasterio
 import matplotlib.pyplot as plt
 
 # Internal Pydar reference to access functions, global variables, and error handling
 import pydar
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
 #### DISPLAY ALL PDR IMAGES IN A DIRECTORY #############################
-def displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120):
+def displayImages(image_directory=None, fig_title=None, cmap="gray", figsize_n=6, fig_dpi=120):
 	# Display all images in the image directory specified
 	#	plt.show() all imgs in a given directory
 
 	pydar.errorHandlingDisplayImages(image_directory=image_directory,
 									fig_title=fig_title,
+									cmap=cmap,
 									figsize_n=figsize_n,
 									fig_dpi=fig_dpi)
 
 	# Display all IMG files in directory
 	for filename in os.listdir(image_directory):
-		if 'IMG' in filename:
+		if 'LBL' in filename:
 			image_file = os.path.join("{0}/{1}".format(image_directory, filename))
 
 			logger.info("Displaying Image: {0}".format(image_file))
-
-			image = PDS3Image.open(image_file)
-			logger.debug("Displaying Dimensions: {0}".format(image.shape))
+			image = rasterio.open(image_file).read()
+			image = image[0,:,:]
 
 			fig = plt.figure(figsize=(figsize_n,figsize_n), dpi=fig_dpi)
 			if fig_title is None:
 				plt.title(filename)
 			else:
 				plt.title(fig_title)
 			plt.xlabel("Pixels #")
 			plt.ylabel("Pixels #")
-			plt.imshow(image.image, cmap='gray')
+			plt.imshow(image, cmap=cmap)
 			plt.show()
 
 	# Log error to user if no image files given
+	if not any(".LBL" in sub for sub in os.listdir(image_directory)): # if directory files does not contain any .IMG files
+		logger.info("\nINFO: Unable to display images, {0} does not contain an LBL file\n".format(image_directory))
 	if not any(".IMG" in sub for sub in os.listdir(image_directory)): # if directory files does not contain any .IMG files
 		logger.info("\nINFO: Unable to display images, {0} does not contain an IMG file\n".format(image_directory))
```

### Comparing `pydar-1.0.1/pydar/error_handling.py` & `pydar-1.1.0/pydar/error_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,28 +157,32 @@
 		if take_ob_num == flyby_observation_num:
 			observation_num_found = True
 			break
 	if not observation_num_found:
 		logger.critical("\nCRITICAL ERROR, [flyby_observation_num]: Invalid flyby_observation_num, '{0}', choose from:\n{1}".format(flyby_observation_num, valid_observation_nums))
 		exit()
 
-def errorHandlingDisplayImages(image_directory=None, fig_title=None, figsize_n=None, fig_dpi=None):
+def errorHandlingDisplayImages(image_directory=None, fig_title=None, cmap=None, figsize_n=None, fig_dpi=None):
 	# Error Handling for Displaying Images from an Image Directory: displayImages()
 	if image_directory == None:
 		logger.critical("\nCRITICAL ERROR, [image_directory]: image_directory is required")
 		exit()
 	else:
 		if type(image_directory) != str:
 			logger.critical("\nCRITICAL ERROR, [image_directory]: Must be a str, current type = '{0}'".format(type(image_directory)))
 			exit()
 
 	if fig_title is not None and type(fig_title) != str:
 		logger.critical("\nCRITICAL ERROR, [fig_title]: Must be a str, current type = '{0}'".format(type(fig_title)))
 		exit()
 
+	if cmap is not None and type(cmap) != str:
+		logger.critical("\nCRITICAL ERROR, [cmap]: Must be a str, current type = '{0}'".format(type(cmap)))
+		exit()
+
 	if type(figsize_n) != int:
 		logger.critical("\nCRITICAL ERROR, [figsize_n]: Must be a int, current type = '{0}'".format(type(figsize_n)))
 		exit()
 	else:
 		if figsize_n < 1:
 			logger.critical("\nCRITICAL ERROR, [figsize_n]: figsize_n must be greater than 1, current value = '{0}'".format(figsize_n))
 			exit()
```

### Comparing `pydar-1.0.1/pydar/extract_flyby_parameters.py` & `pydar-1.1.0/pydar/extract_flyby_parameters.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/pytests/test_display_image.py` & `pydar-1.1.0/pydar/pytests/test_display_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,23 @@
 	# Test:
 	with pytest.raises(SystemExit):
 		pydar.displayImages(image_directory="pydar_results/testing", fig_title=fig_title_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [fig_title]: Must be a str, current type = '{0}'".format(fig_title_error_output)
 
+@pytest.mark.parametrize("cmap_invalid, cmap_error_output", invalid_non_str_options)
+def test_displayImages_cmapInvalidTypes(caplog, cmap_invalid, cmap_error_output):
+	# Test:
+	with pytest.raises(SystemExit):
+		pydar.displayImages(image_directory="pydar_results/testing", cmap=cmap_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [cmap]: Must be a str, current type = '{0}'".format(cmap_error_output)
+
 @pytest.mark.parametrize("figsize_n_invalid, figsize_n_error_output", invalid_non_int_options)
 def test_displayImages_figureSizeInvalidTypes(caplog, figsize_n_invalid, figsize_n_error_output):
 	# Test:
 	with pytest.raises(SystemExit):
 		pydar.displayImages(image_directory="pydar_results/testing", figsize_n=figsize_n_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
@@ -85,8 +94,9 @@
 def test_displayImages_figureDPIInvalidRange(caplog):
 	# Test:
 	with pytest.raises(SystemExit):
 		pydar.displayImages(image_directory="pydar_results/testing", fig_dpi=0)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [fig_dpi]: fig_dpi must be greater than 1, current value = '0'"
+
 ## displayImages() #####################################################
```

### Comparing `pydar-1.0.1/pydar/pytests/test_extract_flyby_parameters.py` & `pydar-1.1.0/pydar/pytests/test_extract_flyby_parameters.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/pytests/test_read_readme.py` & `pydar-1.1.0/pydar/pytests/test_read_readme.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/pytests/test_retrieve_ids_by_time_position.py` & `pydar-1.1.0/pydar/pytests/test_retrieve_ids_by_time_position.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/read_readme.py` & `pydar-1.1.0/pydar/read_readme.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/retrieve_ids_by_time_position.py` & `pydar-1.1.0/pydar/retrieve_ids_by_time_position.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/retrieve_supplementary_backplanes.py` & `pydar-1.1.0/pydar/retrieve_supplementary_backplanes.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/sbdr_make_shapefile.py` & `pydar-1.1.0/pydar/sbdr_make_shapefile.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/test_bearing_correction.py` & `pydar-1.1.0/pydar/test_bearing_correction.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/updateCsvCORADARJPLOptions.py` & `pydar-1.1.0/pydar/updateCsvCORADARJPLOptions.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/updateCsvFeatureNameDetails.py` & `pydar-1.1.0/pydar/updateCsvFeatureNameDetails.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar/updateCsvSwathCoverage.py` & `pydar-1.1.0/pydar/updateCsvSwathCoverage.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/pydar.egg-info/PKG-INFO` & `pydar-1.1.0/pydar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.1.0.tar.gz
 Description: # PYDAR
          <p align="center">
           <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/pydar)
         ![license](https://img.shields.io/pypi/l/pydar)
@@ -651,24 +651,26 @@
         <br>
         ['PRODUCT DESCRIPTION', 'DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES', 'POINTERS TO START RECORDS OF OBJECTS IN FILE', 'DESCRIPTION OF OBJECTS CONTAINED IN FILE']
         </details>
         
         ## Use Downloaded Data
         ### displayImages()
         
+        Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
+        
         ```
-        displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120)
+        displayImages(image_directory=None, fig_title=None, cmap="gray", figsize_n=6, fig_dpi=120)
         ```
         
-        * **[REQUIRED]** image_directory (string): directory containing pydar_results with IMG file
+        * **[REQUIRED]** image_directory (string): directory containing a .LBL and .IMG file
         * [OPTIONAL] fig_title (str): figure title, defaults to filename
+        * [OPTIONAL] cmap (str): optional colormaps ([see more options](https://matplotlib.org/stable/tutorials/colors/colormaps.html)), defaults to 'gray'
         * [OPTIONAL] figsize_n (int): plot dimensions, defaults to 6x6
         * [OPTIONAL] fig_dpi (int): plot dpi, defaults to 120
         
-        Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
         
         ```python
         import pydar
         pydar.displayImages(image_directory="pydar_results/CORADR_0065_V03_S01")
         ```
          <p align="center">
           <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
@@ -682,16 +684,14 @@
         
         COMING SOON: Extract metadata from .TAB file (using .FMT as a reference)
         
         ## Developer Notes TODO:
         ### TODO Code:
         * add a colored outline around a feature when displaying as a 2D image
         * save image pixel to an array
-        * extract pdr functionality to reduce overhead
-        * displayImages() bug fix: 87 displays invalid integer
         * segments will be less than 99 (default to 1 - 01 is the primary imaging) (requires segment_options = ['S01', 'S02', 'S03', 'S04'])
         * progress bars print to command line (still downloading...)
         * save .IMG as .SHP for ArcGIS
         
         ### TODO Questions:
         * add details for what a segment_num is
         * associate burst ID from SBDR data to BIDR data for metadata
@@ -712,14 +712,16 @@
         * test: pull beam information and number of looks for each pixel 
         
         ## Credits
         Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
         
         Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
         
+        This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not neccessarily reflect the views of the National Science Foundation.
+        
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/unaschneck/pydar/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pydar-1.0.1/pydar.egg-info/SOURCES.txt` & `pydar-1.1.0/pydar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydar-1.0.1/setup.py` & `pydar-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.0.1"
+VERSION="1.1.0"
 DESCRIPTION="A Python package to access, download, view, and manipulate Cassini RADAR images"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="pydar",
@@ -40,14 +40,14 @@
 	packages=find_namespace_packages(include=['pydar', 'pydar.*']),
 	include_package_data=True,
 	install_requires=[
 			"beautifulsoup4>=4.11.1",
 			"matplotlib>=3.1.0",
 			"pandas>=1.5.2",
 			"pdr>=0.7.3",
-			"planetaryimage>=0.5.0",
 			"pyproj>=3.4.1",
 			"pytest>=7.2.2",
+			"rasterio>=1.3.6",
 			"urllib3>=1.26.9"
 			],
 	python_requires='>=3.9'
 )
```

