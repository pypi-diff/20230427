# Comparing `tmp/pygentrification-0.0.4.tar.gz` & `tmp/pygentrification-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentrification-0.0.4.tar", last modified: Tue Apr 25 19:05:09 2023, max compression
+gzip compressed data, was "pygentrification-0.0.5.tar", last modified: Thu Apr 27 15:16:14 2023, max compression
```

## Comparing `pygentrification-0.0.4.tar` & `pygentrification-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.073589 pygentrification-0.0.4/
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)     1508 2023-04-24 16:51:27.000000 pygentrification-0.0.4/LICENSE.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19710 2023-04-25 19:05:09.072774 pygentrification-0.0.4/PKG-INFO
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19103 2023-04-25 18:50:19.000000 pygentrification-0.0.4/README.md
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)      838 2023-04-25 19:04:15.000000 pygentrification-0.0.4/pyproject.toml
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       38 2023-04-25 19:05:09.073770 pygentrification-0.0.4/setup.cfg
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.023789 pygentrification-0.0.4/src/
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.063659 pygentrification-0.0.4/src/pygentrification/
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        1 2023-04-18 20:39:15.000000 pygentrification-0.0.4/src/pygentrification/__init__.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    22697 2023-04-25 19:04:05.000000 pygentrification-0.0.4/src/pygentrification/api_calls.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    31174 2023-04-25 18:45:07.000000 pygentrification-0.0.4/src/pygentrification/bates_freeman_indices.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)     9748 2023-04-24 19:28:05.000000 pygentrification-0.0.4/src/pygentrification/ding_index.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    22886 2023-04-25 18:49:09.000000 pygentrification-0.0.4/src/pygentrification/folium_funcs.py
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.069750 pygentrification-0.0.4/src/pygentrification.egg-info/
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19710 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/PKG-INFO
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)      440 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/SOURCES.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        1 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/dependency_links.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       61 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/requires.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       17 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/top_level.txt
+drwxr-xr-x   0 wc555    (407855680) 1823260766        0 2023-04-27 15:16:14.976260 pygentrification-0.0.5/
+-rw-r--r--   0 wc555    (407855680) 1823260766     1508 2023-04-24 16:51:27.000000 pygentrification-0.0.5/LICENSE.txt
+-rw-r--r--   0 wc555    (407855680) 1823260766    19775 2023-04-27 15:16:14.975622 pygentrification-0.0.5/PKG-INFO
+-rw-r--r--   0 wc555    (407855680) 1823260766    19168 2023-04-27 15:13:33.000000 pygentrification-0.0.5/README.md
+-rw-r--r--   0 wc555    (407855680) 1823260766      838 2023-04-27 15:15:16.000000 pygentrification-0.0.5/pyproject.toml
+-rw-r--r--   0 wc555    (407855680) 1823260766       38 2023-04-27 15:16:14.976386 pygentrification-0.0.5/setup.cfg
+drwxr-xr-x   0 wc555    (407855680) 1823260766        0 2023-04-27 15:16:14.927440 pygentrification-0.0.5/src/
+drwxr-xr-x   0 wc555    (407855680) 1823260766        0 2023-04-27 15:16:14.968680 pygentrification-0.0.5/src/pygentrification/
+-rw-r--r--   0 wc555    (407855680) 1823260766        1 2023-04-18 20:39:15.000000 pygentrification-0.0.5/src/pygentrification/__init__.py
+-rw-r--r--   0 wc555    (407855680) 1823260766    22699 2023-04-27 15:09:58.000000 pygentrification-0.0.5/src/pygentrification/api_calls.py
+-rw-r--r--   0 wc555    (407855680) 1823260766    31174 2023-04-25 18:45:07.000000 pygentrification-0.0.5/src/pygentrification/bates_freeman_indices.py
+-rw-r--r--   0 wc555    (407855680) 1823260766     9748 2023-04-24 19:28:05.000000 pygentrification-0.0.5/src/pygentrification/ding_index.py
+-rw-r--r--   0 wc555    (407855680) 1823260766    22886 2023-04-25 18:49:09.000000 pygentrification-0.0.5/src/pygentrification/folium_funcs.py
+drwxr-xr-x   0 wc555    (407855680) 1823260766        0 2023-04-27 15:16:14.974800 pygentrification-0.0.5/src/pygentrification.egg-info/
+-rw-r--r--   0 wc555    (407855680) 1823260766    19775 2023-04-27 15:16:14.000000 pygentrification-0.0.5/src/pygentrification.egg-info/PKG-INFO
+-rw-r--r--   0 wc555    (407855680) 1823260766      440 2023-04-27 15:16:14.000000 pygentrification-0.0.5/src/pygentrification.egg-info/SOURCES.txt
+-rw-r--r--   0 wc555    (407855680) 1823260766        1 2023-04-27 15:16:14.000000 pygentrification-0.0.5/src/pygentrification.egg-info/dependency_links.txt
+-rw-r--r--   0 wc555    (407855680) 1823260766       61 2023-04-27 15:16:14.000000 pygentrification-0.0.5/src/pygentrification.egg-info/requires.txt
+-rw-r--r--   0 wc555    (407855680) 1823260766       17 2023-04-27 15:16:14.000000 pygentrification-0.0.5/src/pygentrification.egg-info/top_level.txt
```

### Comparing `pygentrification-0.0.4/LICENSE.txt` & `pygentrification-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.4/PKG-INFO` & `pygentrification-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentrification
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for calculating and visualizing gentrification indices from published academic research
 Author-email: Winn Costantini <wc555@drexel.edu>, Adam Thompson <adam.thompson0001@temple.edu>, Josh Scrabeck <joshua.scrabeck@temple.edu>
 Project-URL: Homepage, https://github.com/joshscrabeck/pygentrification
 Keywords: gentrification
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: !=3.10,>=3.9
@@ -107,15 +107,15 @@
 
 ```
 pip install pygentrification
 ```
 	
 ### Executing program
 
-##API Calls
+## API Calls
 
 This module contains all the data requests a user might need to make to calculate the indices included in the package. This includes using 5 Year - American Community Survery, Dicennial Census, and TIGER Census data.
 
 Each index requires data at the tract level and data for the county as a whole. Identiy the county and state using FIPS codes. 
 The two example calls below would return the two dataframes needed to calculate the bates-freeman indices and ding index for Philadelphia County (101) in PA (42) using data from 2000, 2010, and 2020.
 
 The function will return data in EPSG 4269, but requires a proj_parameter that indicates the projected crs that will be used for areal interpolation needed to harmonize data to census tract boundaries for different years.
@@ -126,54 +126,54 @@
 tract_gdf = get_api_data_tract("42", "101", years = [2000, 2010, 2020], indices = ["bates", "ding"], proj_crs = "EPSG: 2272")
 
 county_gdf = get_api_data_county("42", "101", years = [2000, 2010, 2020], indices = ["bates", "ding"])
 
 ```
 
 
-##Bates and Freeman Indices
+## Bates and Freeman Indices
 
 This module contains the data prep steps, index calculation, and dataframe creation of the Bates-Freeman index
 
 
 calc_batesfreeman is a function that calculates the index according to Bates-Freeman, as cited above. If using a GeoDataFrame retrieved with the functions above, an example call would be: 
 
 ```
 from pygentrification.bates_freeman_indices import calc_bates_freeman
 
 bates_freeman_gdf = calc_batesfreeman(county_gdf, tract_gdf, inplace = False)
 
 ```
 
 Users may also use data retrieved in other ways as long as:
-*one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
-*each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
-*they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
+* one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
+* each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
+* they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
 
 ```
 cols_area = ['area_med_house_inc_yr1', 'area_med_house_inc_e_yr1', 'area_med_house_inc_yr2', 'area_med_house_inc_e_yr2', 'area_med_fam_inc_yr2', 'area_med_fam_inc_e_yr2']
 cols_tract = ['pop_tenure_yr1', 'owner_yr1', 'renter_yr1', 'pop_tenure_yr2', 'owner_yr2', 'renter_yr2', 'pop_25_over_yr1', 'ba_degree_m_yr1', 'ma_degree_m_yr1', 'prof_degree_m_yr1', 'doc_degree_m_yr1', 'ba_degree_f_yr1', 'ma_degree_f_yr1', 'prof_degree_f_yr1', 'doc_degree_f_yr1', 'pop_25_over_yr2', 'ba_degree_m_yr2','ma_degree_m_yr2', 'prof_degree_m_yr2', 'doc_degree_m_yr2', 'ba_degree_f_yr2','ma_degree_f_yr2', 'prof_degree_f_yr2', 'doc_degree_f_yr2','pop_race_yr1', 'white_yr1', 'pop_race_yr2', 'white_yr2', 'med_fam_inc_yr2', 'med_home_val_yr0', 'med_home_val_yr1', 'med_home_val_yr2', 'med_house_inc_yr1', 'med_house_inc_yr2', 'tot_house_yr2', 'new_house_col1', 'new_house_col2', 'new_house_col3']
 ```
     
 
-##Ding Index
+## Ding Index
 
 This module contains the data prep steps, index calculation, and dataframe creation of the Ding index
 
 
 calc_batesfreeman is a function that calculates the index according to Ding, as cited above. If using a GeoDataFrame retrieved with the functions above, an example call would be: 
 
 ```
 from pygentrification.ding_index import calc_ding
 
 ding_gdf = calc_ding(county_gdf, tract_gdf, inplace = False):
 
 ``` 
 
-##Folium Maps
+## Folium Maps
 
 This module contains functions to create Folium maps from the output of Bates-Freeman and Ding functions hosted on a local HTML site.
 
 The crs for the input gdf MUST be EPSG: 4269.
 
 This function takes in the GeoDataFrame generated by the calc_batesfreeman function fand outputs and map object of a Folium map. It saves an html file of the map object to the working directory.
 
@@ -188,17 +188,17 @@
 ```
 from pygentrification.folium_funcs import ding_result_map 
 
 ding_result_map(ding_gdf, filename = 'ding_map.html'):
 ```
 
 Users may also use data retrieved in other ways as long as:
-*one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
-*each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
-*they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
+* one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
+* each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
+* they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
 
 ```
 cols_area = ['area_med_rent_yr1', 'area_med_rent_yr2', 'area_med_home_val_yr1', 'area_med_home_val_yr2', 'area_med_house_inc_yr1', 'area_med_house_inc_yr2']
 cols_tract=['med_rent_yr1', 'med_rent_yr2', 'med_home_val_yr1', 'med_home_val_yr2', 'pop_25_over_yr1' 'ba_degree_m_yr1', 'ma_degree_m_yr1', 'prof_degree_m_yr1', 'doc_degree_m_yr1, ba_degree_f_yr1', 'ma_degree_f_yr1', 'prof_degree_f_yr1', 'doc_degree_f_yr1', 'pop_25_over_yr2', 'ba_degree_m_yr2', 'ma_degree_m_yr2', 'prof_degree_m_yr2', 'doc_degree_m_yr2', 'ba_degree_f_yr2', 'ma_degree_f_yr2', 'prof_degree_f_yr2', 'doc_degree_f_yr2', 'med_house_inc_yr1', 'med_house_inc_yr2']
 ```
 
 
@@ -208,16 +208,21 @@
 
 Winn Costantini (https://github.com/wcostantini)
 Adam Thompson (https://github.com/Lubbles)
 Josh Scrabeck (https://github.com/joshscrabeck)
 
 ## Version History
 
-* 0.1
-    * Initial Release
+* 0.0.1
+    *Initial release
+* 0.0.2
+* 0.0.3
+* 0.0.4
+* 0.0.5
+    * Current Release
 
 ## License
 
 This project is licensed under the BSD License - see the LICENSE.txt file for details
 
 ## Acknowledgments
```

### Comparing `pygentrification-0.0.4/README.md` & `pygentrification-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 ```
 pip install pygentrification
 ```
 	
 ### Executing program
 
-##API Calls
+## API Calls
 
 This module contains all the data requests a user might need to make to calculate the indices included in the package. This includes using 5 Year - American Community Survery, Dicennial Census, and TIGER Census data.
 
 Each index requires data at the tract level and data for the county as a whole. Identiy the county and state using FIPS codes. 
 The two example calls below would return the two dataframes needed to calculate the bates-freeman indices and ding index for Philadelphia County (101) in PA (42) using data from 2000, 2010, and 2020.
 
 The function will return data in EPSG 4269, but requires a proj_parameter that indicates the projected crs that will be used for areal interpolation needed to harmonize data to census tract boundaries for different years.
@@ -113,54 +113,54 @@
 tract_gdf = get_api_data_tract("42", "101", years = [2000, 2010, 2020], indices = ["bates", "ding"], proj_crs = "EPSG: 2272")
 
 county_gdf = get_api_data_county("42", "101", years = [2000, 2010, 2020], indices = ["bates", "ding"])
 
 ```
 
 
-##Bates and Freeman Indices
+## Bates and Freeman Indices
 
 This module contains the data prep steps, index calculation, and dataframe creation of the Bates-Freeman index
 
 
 calc_batesfreeman is a function that calculates the index according to Bates-Freeman, as cited above. If using a GeoDataFrame retrieved with the functions above, an example call would be: 
 
 ```
 from pygentrification.bates_freeman_indices import calc_bates_freeman
 
 bates_freeman_gdf = calc_batesfreeman(county_gdf, tract_gdf, inplace = False)
 
 ```
 
 Users may also use data retrieved in other ways as long as:
-*one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
-*each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
-*they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
+* one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
+* each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
+* they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
 
 ```
 cols_area = ['area_med_house_inc_yr1', 'area_med_house_inc_e_yr1', 'area_med_house_inc_yr2', 'area_med_house_inc_e_yr2', 'area_med_fam_inc_yr2', 'area_med_fam_inc_e_yr2']
 cols_tract = ['pop_tenure_yr1', 'owner_yr1', 'renter_yr1', 'pop_tenure_yr2', 'owner_yr2', 'renter_yr2', 'pop_25_over_yr1', 'ba_degree_m_yr1', 'ma_degree_m_yr1', 'prof_degree_m_yr1', 'doc_degree_m_yr1', 'ba_degree_f_yr1', 'ma_degree_f_yr1', 'prof_degree_f_yr1', 'doc_degree_f_yr1', 'pop_25_over_yr2', 'ba_degree_m_yr2','ma_degree_m_yr2', 'prof_degree_m_yr2', 'doc_degree_m_yr2', 'ba_degree_f_yr2','ma_degree_f_yr2', 'prof_degree_f_yr2', 'doc_degree_f_yr2','pop_race_yr1', 'white_yr1', 'pop_race_yr2', 'white_yr2', 'med_fam_inc_yr2', 'med_home_val_yr0', 'med_home_val_yr1', 'med_home_val_yr2', 'med_house_inc_yr1', 'med_house_inc_yr2', 'tot_house_yr2', 'new_house_col1', 'new_house_col2', 'new_house_col3']
 ```
     
 
-##Ding Index
+## Ding Index
 
 This module contains the data prep steps, index calculation, and dataframe creation of the Ding index
 
 
 calc_batesfreeman is a function that calculates the index according to Ding, as cited above. If using a GeoDataFrame retrieved with the functions above, an example call would be: 
 
 ```
 from pygentrification.ding_index import calc_ding
 
 ding_gdf = calc_ding(county_gdf, tract_gdf, inplace = False):
 
 ``` 
 
-##Folium Maps
+## Folium Maps
 
 This module contains functions to create Folium maps from the output of Bates-Freeman and Ding functions hosted on a local HTML site.
 
 The crs for the input gdf MUST be EPSG: 4269.
 
 This function takes in the GeoDataFrame generated by the calc_batesfreeman function fand outputs and map object of a Folium map. It saves an html file of the map object to the working directory.
 
@@ -175,17 +175,17 @@
 ```
 from pygentrification.folium_funcs import ding_result_map 
 
 ding_result_map(ding_gdf, filename = 'ding_map.html'):
 ```
 
 Users may also use data retrieved in other ways as long as:
-*one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
-*each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
-*they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
+* one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
+* each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
+* they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
 
 ```
 cols_area = ['area_med_rent_yr1', 'area_med_rent_yr2', 'area_med_home_val_yr1', 'area_med_home_val_yr2', 'area_med_house_inc_yr1', 'area_med_house_inc_yr2']
 cols_tract=['med_rent_yr1', 'med_rent_yr2', 'med_home_val_yr1', 'med_home_val_yr2', 'pop_25_over_yr1' 'ba_degree_m_yr1', 'ma_degree_m_yr1', 'prof_degree_m_yr1', 'doc_degree_m_yr1, ba_degree_f_yr1', 'ma_degree_f_yr1', 'prof_degree_f_yr1', 'doc_degree_f_yr1', 'pop_25_over_yr2', 'ba_degree_m_yr2', 'ma_degree_m_yr2', 'prof_degree_m_yr2', 'doc_degree_m_yr2', 'ba_degree_f_yr2', 'ma_degree_f_yr2', 'prof_degree_f_yr2', 'doc_degree_f_yr2', 'med_house_inc_yr1', 'med_house_inc_yr2']
 ```
 
 
@@ -195,16 +195,21 @@
 
 Winn Costantini (https://github.com/wcostantini)
 Adam Thompson (https://github.com/Lubbles)
 Josh Scrabeck (https://github.com/joshscrabeck)
 
 ## Version History
 
-* 0.1
-    * Initial Release
+* 0.0.1
+    *Initial release
+* 0.0.2
+* 0.0.3
+* 0.0.4
+* 0.0.5
+    * Current Release
 
 ## License
 
 This project is licensed under the BSD License - see the LICENSE.txt file for details
 
 ## Acknowledgments
```

### Comparing `pygentrification-0.0.4/pyproject.toml` & `pygentrification-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygentrification"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Winn Costantini", email="wc555@drexel.edu"}, {name = "Adam Thompson", email = "adam.thompson0001@temple.edu"}, {name = "Josh Scrabeck", email = "joshua.scrabeck@temple.edu"},
 ]
 description = "A python package for calculating and visualizing gentrification indices from published academic research"
 readme = "README.md"
 requires-python = ">=3.9, !=3.10"
 keywords = ["gentrification"]
```

### Comparing `pygentrification-0.0.4/src/pygentrification/api_calls.py` & `pygentrification-0.0.5/src/pygentrification/api_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,106 +63,15 @@
               'B25034_002E':'new_house_col1', 'B25034_003E':'new_house_col2', 'B25034_004E':'new_house_col3'}
 
 #dict for renaming columns for county-level variables 
 master_county_dict = {'B25064_001E':'area_med_rent', 'B25077_001E':'area_med_home_val',
                       'B19013_001E':'area_med_house_inc', 'B19013_001M':'area_med_house_inc_e',
                       'B19113_001E':'area_med_fam_inc', 'B19113_001M':'area_med_fam_inc_e'}
 
-#%%
-##harmonization function##
-def harmonize_tracts(target_df, input_dfs = []):
-    ''' This function takes in a target GeoDataFrame and a list of input GeoDataFrames. The target_df has the target geometry and the function uses the tobler package's areal interpolation
-    function to harmonize the data in each input GeoDataFrame with the geometry in the target dataframe. 
-    
-    Parameters
-    -------------
-    target_df: GeoDataFrame with target geometry
-    input_dfs: List of GeoDataFrames 
-
-    Returns
-    ------------
-    GeoDataFrame
-    
-    This function will return a single GeoDataFrame with all interpolated columns from all input dfs and the geometry and all original columns from the target df. 
-    The interpolated columns will have suffixes corresponding to their order in the input_dfs parameter. If there is more than one input df (for year o - year n), the suffix will start at '_yr0' and the target_df will have teh suffix '_yr{n}'. If there is only one input df the suffix will be '_yr1' and the target_df will have suffix '_yr2'.
-    
-    References
-    -------------
-    https://github.com/pysal/tobler
-    
-    Notes
-    -------------
-    This function uses lists of possible extensive variables and intensive variables, which together include all possible column names needed to calculate the gentrification indices in this package.
-    
-      '''
-
-    
-    #define lists with all possible intensive and extensive variables
-    all_extensive_vars = ['tot_pop','pop_tenure', 'owner', 'renter', 'pop_25_over', 'ba_degree_m', 'ma_degree_m', 'prof_degree_m', 'doc_degree_m', 'ba_degree_f', 'ma_degree_f', 'prof_degree_f', 'doc_degree_f',  'pop_race', 'white', 'tot_house', 'new_house_col1', 'new_house_col2', 'new_house_col3']
-    all_intensive_vars = ['med_rent','med_fam_inc', 'med_home_val', 'med_house_inc']
-    
-    #take in list of input dfs and make two lists of lists - one for extensive and one for intensive
-    extensive_variables = []
-    intensive_variables = []
-    
-    for input_df in input_dfs:
-        e_vars = []
-        i_vars = []
-        col_list = input_df.columns.to_list()
-        for col in col_list:
-            if col in all_extensive_vars:
-                e_vars.append(col)
-            elif col in all_intensive_vars:
-                i_vars.append(col)
-        if len(e_vars) > 0:
-            extensive_variables.append(e_vars)
-        else:
-            extensive_variables.append(None)
-        if len(i_vars) > 0:
-            intensive_variables.append(i_vars)
-
-        else:
-            intensive_variables.append(None)
-    
-    #initialize vars for areal interpolation loop
-    if len(input_dfs) == 1:
-        i = 1
-    
-    elif len(input_dfs) > 1:
-        i = 0
-    
-    varslist = 0
-    merge_dfs = []
-    
-    #use tobler's areal interpolation function and add output dfs to list
-    for input_df in input_dfs:    
-        interpolated_columns = area_interpolate(input_df, target_df, extensive_variables = extensive_variables[varslist], intensive_variables= intensive_variables[varslist])
-        interpolated_columns.drop(['geometry'], axis = 1, inplace = True)
-        interpolated_columns = interpolated_columns.add_suffix(f'_yr{i}')
-        interpolated_columns = interpolated_columns.reset_index(drop = True)
-        merge_dfs.append(interpolated_columns)
-        i += 1
-        varslist += 1
-       
-    #add suffix to target df, rename columns, and reset index
-    target_df = target_df.add_suffix(f'_yr{i}')
-    target_df = target_df.rename(columns = {f'geometry_yr{i}': 'geometry', f'GEOID_yr{i}': 'GEOID'})
-    target_df = target_df.set_geometry('geometry')
-    target_df = target_df.reset_index(drop = True)
-    #merge_dfs.append(target_df)
-    
-    df_list = [target_df]
-    for df in merge_dfs:
-        df_list.append(df)
-    
-    #merge output dfs from aerial interpolation with target df
-    output = reduce(lambda left,right: left.merge(right, left_index = True, right_index = True, how='inner'), df_list)
-    
 
-    return output
 
 
 #%%
 
 ###api request base functions###
 def acs_request_tract(year, state, county, req_vars):
     
@@ -343,14 +252,106 @@
     '''
     acs_df = acs_df.drop(columns = ['GEOID'])
     gdf = t_df.merge(acs_df, left_index = True, right_index =  True)
 
     return gdf
 
 #%%
+##harmonization function##
+def harmonize_tracts(target_df, input_dfs = []):
+    ''' This function takes in a target GeoDataFrame and a list of input GeoDataFrames. The target_df has the target geometry and the function uses the tobler package's areal interpolation
+    function to harmonize the data in each input GeoDataFrame with the geometry in the target dataframe. 
+    
+    Parameters
+    -------------
+    target_df: GeoDataFrame with target geometry
+    input_dfs: List of GeoDataFrames 
+
+    Returns
+    ------------
+    GeoDataFrame
+    
+    This function will return a single GeoDataFrame with all interpolated columns from all input dfs and the geometry and all original columns from the target df. 
+    The interpolated columns will have suffixes corresponding to their order in the input_dfs parameter. If there is more than one input df (for year o - year n), the suffix will start at '_yr0' and the target_df will have teh suffix '_yr{n}'. If there is only one input df the suffix will be '_yr1' and the target_df will have suffix '_yr2'.
+    
+    References
+    -------------
+    https://github.com/pysal/tobler
+    
+    Notes
+    -------------
+    This function uses lists of possible extensive variables and intensive variables, which together include all possible column names needed to calculate the gentrification indices in this package.
+    
+      '''
+
+    
+    #define lists with all possible intensive and extensive variables
+    all_extensive_vars = ['tot_pop','pop_tenure', 'owner', 'renter', 'pop_25_over', 'ba_degree_m', 'ma_degree_m', 'prof_degree_m', 'doc_degree_m', 'ba_degree_f', 'ma_degree_f', 'prof_degree_f', 'doc_degree_f',  'pop_race', 'white', 'tot_house', 'new_house_col1', 'new_house_col2', 'new_house_col3']
+    all_intensive_vars = ['med_rent','med_fam_inc', 'med_home_val', 'med_house_inc']
+    
+    #take in list of input dfs and make two lists of lists - one for extensive and one for intensive
+    extensive_variables = []
+    intensive_variables = []
+    
+    for input_df in input_dfs:
+        e_vars = []
+        i_vars = []
+        col_list = input_df.columns.to_list()
+        for col in col_list:
+            if col in all_extensive_vars:
+                e_vars.append(col)
+            elif col in all_intensive_vars:
+                i_vars.append(col)
+        if len(e_vars) > 0:
+            extensive_variables.append(e_vars)
+        else:
+            extensive_variables.append(None)
+        if len(i_vars) > 0:
+            intensive_variables.append(i_vars)
+
+        else:
+            intensive_variables.append(None)
+    
+    #initialize vars for areal interpolation loop
+    if len(input_dfs) == 1:
+        i = 1
+    
+    elif len(input_dfs) > 1:
+        i = 0
+    
+    varslist = 0
+    merge_dfs = []
+    
+    #use tobler's areal interpolation function and add output dfs to list
+    for input_df in input_dfs:    
+        interpolated_columns = area_interpolate(input_df, target_df, extensive_variables = extensive_variables[varslist], intensive_variables= intensive_variables[varslist])
+        interpolated_columns.drop(['geometry'], axis = 1, inplace = True)
+        interpolated_columns = interpolated_columns.add_suffix(f'_yr{i}')
+        interpolated_columns = interpolated_columns.reset_index(drop = True)
+        merge_dfs.append(interpolated_columns)
+        i += 1
+        varslist += 1
+       
+    #add suffix to target df, rename columns, and reset index
+    target_df = target_df.add_suffix(f'_yr{i}')
+    target_df = target_df.rename(columns = {f'geometry_yr{i}': 'geometry', f'GEOID_yr{i}': 'GEOID'})
+    target_df = target_df.set_geometry('geometry')
+    target_df = target_df.reset_index(drop = True)
+    #merge_dfs.append(target_df)
+    
+    df_list = [target_df]
+    for df in merge_dfs:
+        df_list.append(df)
+    
+    #merge output dfs from aerial interpolation with target df
+    output = reduce(lambda left,right: left.merge(right, left_index = True, right_index = True, how='inner'), df_list)
+    
+
+    return output
+#%%
 
 ###comprehensive api call function for tract-level###
 
 def get_api_data_tract(state, county, years, indices, proj_crs = 'EPSG:4269'):
     
     ''' 
     This function retrives data from the Census, 5 year
```

### Comparing `pygentrification-0.0.4/src/pygentrification/bates_freeman_indices.py` & `pygentrification-0.0.5/src/pygentrification/bates_freeman_indices.py`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.4/src/pygentrification/ding_index.py` & `pygentrification-0.0.5/src/pygentrification/ding_index.py`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.4/src/pygentrification/folium_funcs.py` & `pygentrification-0.0.5/src/pygentrification/folium_funcs.py`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.4/src/pygentrification.egg-info/PKG-INFO` & `pygentrification-0.0.5/src/pygentrification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentrification
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for calculating and visualizing gentrification indices from published academic research
 Author-email: Winn Costantini <wc555@drexel.edu>, Adam Thompson <adam.thompson0001@temple.edu>, Josh Scrabeck <joshua.scrabeck@temple.edu>
 Project-URL: Homepage, https://github.com/joshscrabeck/pygentrification
 Keywords: gentrification
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: !=3.10,>=3.9
@@ -107,15 +107,15 @@
 
 ```
 pip install pygentrification
 ```
 	
 ### Executing program
 
-##API Calls
+## API Calls
 
 This module contains all the data requests a user might need to make to calculate the indices included in the package. This includes using 5 Year - American Community Survery, Dicennial Census, and TIGER Census data.
 
 Each index requires data at the tract level and data for the county as a whole. Identiy the county and state using FIPS codes. 
 The two example calls below would return the two dataframes needed to calculate the bates-freeman indices and ding index for Philadelphia County (101) in PA (42) using data from 2000, 2010, and 2020.
 
 The function will return data in EPSG 4269, but requires a proj_parameter that indicates the projected crs that will be used for areal interpolation needed to harmonize data to census tract boundaries for different years.
@@ -126,54 +126,54 @@
 tract_gdf = get_api_data_tract("42", "101", years = [2000, 2010, 2020], indices = ["bates", "ding"], proj_crs = "EPSG: 2272")
 
 county_gdf = get_api_data_county("42", "101", years = [2000, 2010, 2020], indices = ["bates", "ding"])
 
 ```
 
 
-##Bates and Freeman Indices
+## Bates and Freeman Indices
 
 This module contains the data prep steps, index calculation, and dataframe creation of the Bates-Freeman index
 
 
 calc_batesfreeman is a function that calculates the index according to Bates-Freeman, as cited above. If using a GeoDataFrame retrieved with the functions above, an example call would be: 
 
 ```
 from pygentrification.bates_freeman_indices import calc_bates_freeman
 
 bates_freeman_gdf = calc_batesfreeman(county_gdf, tract_gdf, inplace = False)
 
 ```
 
 Users may also use data retrieved in other ways as long as:
-*one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
-*each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
-*they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
+* one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
+* each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
+* they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
 
 ```
 cols_area = ['area_med_house_inc_yr1', 'area_med_house_inc_e_yr1', 'area_med_house_inc_yr2', 'area_med_house_inc_e_yr2', 'area_med_fam_inc_yr2', 'area_med_fam_inc_e_yr2']
 cols_tract = ['pop_tenure_yr1', 'owner_yr1', 'renter_yr1', 'pop_tenure_yr2', 'owner_yr2', 'renter_yr2', 'pop_25_over_yr1', 'ba_degree_m_yr1', 'ma_degree_m_yr1', 'prof_degree_m_yr1', 'doc_degree_m_yr1', 'ba_degree_f_yr1', 'ma_degree_f_yr1', 'prof_degree_f_yr1', 'doc_degree_f_yr1', 'pop_25_over_yr2', 'ba_degree_m_yr2','ma_degree_m_yr2', 'prof_degree_m_yr2', 'doc_degree_m_yr2', 'ba_degree_f_yr2','ma_degree_f_yr2', 'prof_degree_f_yr2', 'doc_degree_f_yr2','pop_race_yr1', 'white_yr1', 'pop_race_yr2', 'white_yr2', 'med_fam_inc_yr2', 'med_home_val_yr0', 'med_home_val_yr1', 'med_home_val_yr2', 'med_house_inc_yr1', 'med_house_inc_yr2', 'tot_house_yr2', 'new_house_col1', 'new_house_col2', 'new_house_col3']
 ```
     
 
-##Ding Index
+## Ding Index
 
 This module contains the data prep steps, index calculation, and dataframe creation of the Ding index
 
 
 calc_batesfreeman is a function that calculates the index according to Ding, as cited above. If using a GeoDataFrame retrieved with the functions above, an example call would be: 
 
 ```
 from pygentrification.ding_index import calc_ding
 
 ding_gdf = calc_ding(county_gdf, tract_gdf, inplace = False):
 
 ``` 
 
-##Folium Maps
+## Folium Maps
 
 This module contains functions to create Folium maps from the output of Bates-Freeman and Ding functions hosted on a local HTML site.
 
 The crs for the input gdf MUST be EPSG: 4269.
 
 This function takes in the GeoDataFrame generated by the calc_batesfreeman function fand outputs and map object of a Folium map. It saves an html file of the map object to the working directory.
 
@@ -188,17 +188,17 @@
 ```
 from pygentrification.folium_funcs import ding_result_map 
 
 ding_result_map(ding_gdf, filename = 'ding_map.html'):
 ```
 
 Users may also use data retrieved in other ways as long as:
-*one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
-*each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
-*they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
+* one is a gdf at the tract level of the study area and one is a df or gdf values for the area as a whole 
+* each dataset has data for the acs and census variables required for calculating the indices in this script for the years specified. 
+* they specify column column names as a list with an order that corresponds exactly with the default values for th cols_tract and cols_area parameters.
 
 ```
 cols_area = ['area_med_rent_yr1', 'area_med_rent_yr2', 'area_med_home_val_yr1', 'area_med_home_val_yr2', 'area_med_house_inc_yr1', 'area_med_house_inc_yr2']
 cols_tract=['med_rent_yr1', 'med_rent_yr2', 'med_home_val_yr1', 'med_home_val_yr2', 'pop_25_over_yr1' 'ba_degree_m_yr1', 'ma_degree_m_yr1', 'prof_degree_m_yr1', 'doc_degree_m_yr1, ba_degree_f_yr1', 'ma_degree_f_yr1', 'prof_degree_f_yr1', 'doc_degree_f_yr1', 'pop_25_over_yr2', 'ba_degree_m_yr2', 'ma_degree_m_yr2', 'prof_degree_m_yr2', 'doc_degree_m_yr2', 'ba_degree_f_yr2', 'ma_degree_f_yr2', 'prof_degree_f_yr2', 'doc_degree_f_yr2', 'med_house_inc_yr1', 'med_house_inc_yr2']
 ```
 
 
@@ -208,16 +208,21 @@
 
 Winn Costantini (https://github.com/wcostantini)
 Adam Thompson (https://github.com/Lubbles)
 Josh Scrabeck (https://github.com/joshscrabeck)
 
 ## Version History
 
-* 0.1
-    * Initial Release
+* 0.0.1
+    *Initial release
+* 0.0.2
+* 0.0.3
+* 0.0.4
+* 0.0.5
+    * Current Release
 
 ## License
 
 This project is licensed under the BSD License - see the LICENSE.txt file for details
 
 ## Acknowledgments
```

