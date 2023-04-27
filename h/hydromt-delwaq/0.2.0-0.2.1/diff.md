# Comparing `tmp/hydromt_delwaq-0.2.0.tar.gz` & `tmp/hydromt_delwaq-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt_delwaq-0.2.0.tar", last modified: Wed Dec 21 06:00:27 2022, max compression
+gzip compressed data, was "hydromt_delwaq-0.2.1.tar", last modified: Thu Apr 27 08:39:41 2023, max compression
```

## Comparing `hydromt_delwaq-0.2.0.tar` & `hydromt_delwaq-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1833 2022-12-21 06:00:18.707810 hydromt_delwaq-0.2.0/.gitignore
--rw-r--r--   0        0        0      441 2022-12-21 06:00:18.707810 hydromt_delwaq-0.2.0/.zenodo.json
--rw-r--r--   0        0        0    35821 2022-12-21 06:00:18.711810 hydromt_delwaq-0.2.0/LICENSE
--rw-r--r--   0        0        0     4660 2022-12-21 06:00:18.711810 hydromt_delwaq-0.2.0/README.rst
--rw-r--r--   0        0        0      702 2022-12-21 06:00:18.727810 hydromt_delwaq-0.2.0/environment.yml
--rw-r--r--   0        0        0      299 2022-12-21 06:00:18.807809 hydromt_delwaq-0.2.0/hydromt_delwaq/__init__.py
--rw-r--r--   0        0        0   309240 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/data/admin_bound/gadm_level1_mapping.csv
--rw-r--r--   0        0        0      161 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/data/delwaq/emission_raster.csv
--rw-r--r--   0        0        0       49 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/data/delwaq/emission_vector.csv
--rw-r--r--   0        0        0    79459 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/delwaq.py
--rw-r--r--   0        0        0        0 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/.gitkeep
--rw-r--r--   0        0        0      126 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/__init__.py
--rw-r--r--   0        0        0     8559 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/emissions.py
--rw-r--r--   0        0        0     6609 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/roads.py
--rw-r--r--   0        0        0     4001 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/segments.py
--rw-r--r--   0        0        0     1850 2022-12-21 06:00:18.811809 hydromt_delwaq-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6108 1970-01-01 00:00:00.000000 hydromt_delwaq-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1833 2023-04-27 08:39:30.775248 hydromt_delwaq-0.2.1/.gitignore
+-rw-r--r--   0        0        0      441 2023-04-27 08:39:30.775248 hydromt_delwaq-0.2.1/.zenodo.json
+-rw-r--r--   0        0        0    35821 2023-04-27 08:39:30.775248 hydromt_delwaq-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4659 2023-04-27 08:39:30.775248 hydromt_delwaq-0.2.1/README.rst
+-rw-r--r--   0        0        0      329 2023-04-27 08:39:30.795248 hydromt_delwaq-0.2.1/environment.yml
+-rw-r--r--   0        0        0      334 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/__init__.py
+-rw-r--r--   0        0        0   309240 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/data/admin_bound/gadm_level1_mapping.csv
+-rw-r--r--   0        0        0      161 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/data/delwaq/emission_raster.csv
+-rw-r--r--   0        0        0       49 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/data/delwaq/emission_vector.csv
+-rw-r--r--   0        0        0    79417 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/delwaq.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/.gitkeep
+-rw-r--r--   0        0        0      126 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/__init__.py
+-rw-r--r--   0        0        0     8560 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/emissions.py
+-rw-r--r--   0        0        0     6609 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/roads.py
+-rw-r--r--   0        0        0     4001 2023-04-27 08:39:30.875248 hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/segments.py
+-rw-r--r--   0        0        0     1770 2023-04-27 08:39:30.879248 hydromt_delwaq-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 hydromt_delwaq-0.2.1/PKG-INFO
```

### Comparing `hydromt_delwaq-0.2.0/.gitignore` & `hydromt_delwaq-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydromt_delwaq-0.2.0/LICENSE` & `hydromt_delwaq-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt_delwaq-0.2.0/README.rst` & `hydromt_delwaq-0.2.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 HydroMT-delwaq: DELWAQ plugin for HydroMT
 #########################################
 
 |pypi| |docs_latest| |docs_stable| |codecov| |license| |binder|
 
 What is HydroMT-delwaq?
 -----------------------
-HydroMT-delwaq is a plugin of the `HydroMT core <https://deltares.github.io/hydromt/latest/index.html#>`_, a python package, developed by Deltares, to build 
+HydroMT-delwaq is a plugin of the `HydroMT core <https://deltares.github.io/hydromt/latest/index.html>`_, a python package, developed by Deltares, to build 
 and analyse environmental models. This plugin provides an implementation for the `DELWAQ <https://www.deltares.nl/en/software/module/d-water-quality/>`_ water quality engine. 
 It details the different steps and explains how to use HydroMT to easily get started and work on your own DELWAQ model. WIth this plugin 
 you can interact with both classic **D-Water Quality** models as well as **D-Emission** models.
 
 With the **HydroMT-delwaq plugin**, users can easily benefit from the rich set of tools of the 
 `HydroMT package <https://github.com/Deltares/hydromt>`_ to build and update 
 DELWAQ models from available global and local data.
```

### Comparing `hydromt_delwaq-0.2.0/hydromt_delwaq/data/admin_bound/gadm_level1_mapping.csv` & `hydromt_delwaq-0.2.1/hydromt_delwaq/data/admin_bound/gadm_level1_mapping.csv`

 * *Files identical despite different names*

### Comparing `hydromt_delwaq-0.2.0/hydromt_delwaq/delwaq.py` & `hydromt_delwaq-0.2.1/hydromt_delwaq/delwaq.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,18 +281,18 @@
         mv = -999
         # Read monitoring points source
         if mon_points is not None:
             if mon_points == "segments":
                 monpoints = self.hydromaps["ptid"]
             else:
                 kwargs = {}
-                if isfile(mon_points) and str(mon_points).endswith(".csv"):
+                if isfile(mon_points):
                     kwargs.update(crs=self.crs)
                 gdf = self.data_catalog.get_geodataframe(
-                    str(mon_points), geom=self.basins, assert_gtype="Point", **kwargs
+                    mon_points, geom=self.basins, assert_gtype="Point", **kwargs
                 )
                 gdf = gdf.to_crs(self.crs)
                 if gdf.index.size == 0:
                     self.logger.warning(
                         f"No {mon_points} gauge locations found within domain"
                     )
                 else:
```

### Comparing `hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/emissions.py` & `hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/emissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,15 @@
     # include index_col as parameter (for output to map)
     df["EM_ID"] = df.index
     df.EM_ID = df.EM_ID.astype(np.int32)
     # define list of parameters for which output maps are created
     params = [p for p in df.columns if p.startswith("EM_")]
     # setup ds out
     ds_out = xr.Dataset(coords=ds_like.raster.coords)
+
     # setup reclass method
     def reclass(x):
         return np.vectorize(d.get)(x, nodata)
 
     # apply for each parameter
     for param in params:
         # TODO change average into value with highest occurence
```

### Comparing `hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/roads.py` & `hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/roads.py`

 * *Files identical despite different names*

### Comparing `hydromt_delwaq-0.2.0/hydromt_delwaq/workflows/segments.py` & `hydromt_delwaq-0.2.1/hydromt_delwaq/workflows/segments.py`

 * *Files identical despite different names*

### Comparing `hydromt_delwaq-0.2.0/pyproject.toml` & `hydromt_delwaq-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,21 @@
 authors = [
     {name = "Hélène Boisgontier", email = "helene.boisgontier@deltares.nl"},
     {name = "Sibren Loos", email = "sibren.loos@deltares.nl"},
 ]
 dependencies = [
     "hydromt >=0.5.0",
     "hydromt_wflow >=0.2.0",
-    "dask",
-    "geopandas >=0.10.0",
-    "netcdf4",
+    "geopandas >=0.10",
     "numpy",
     "pandas",
-    "pyflwdir>=0.5.6",
-    "pygeos",
     "pyproj",
     "rasterio",
-    "rioxarray",
     "scipy",
-    "shapely",
+    "shapely >=2.0.0",
     "xarray",
 ]
 requires-python = ">=3.8" # fix tests to support older versions
 readme = "README.rst"
 classifiers = [
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     "Development Status :: 4 - Beta",
```

### Comparing `hydromt_delwaq-0.2.0/PKG-INFO` & `hydromt_delwaq-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 Metadata-Version: 2.1
 Name: hydromt_delwaq
-Version: 0.2.0
+Version: 0.2.1
 Summary: hydroMT plugin for DELWAQ models.
 Author-email: Hélène Boisgontier <helene.boisgontier@deltares.nl>, Sibren Loos <sibren.loos@deltares.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: hydromt >=0.5.0
 Requires-Dist: hydromt_wflow >=0.2.0
-Requires-Dist: dask
-Requires-Dist: geopandas >=0.10.0
-Requires-Dist: netcdf4
+Requires-Dist: geopandas >=0.10
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pyflwdir>=0.5.6
-Requires-Dist: pygeos
 Requires-Dist: pyproj
 Requires-Dist: rasterio
-Requires-Dist: rioxarray
 Requires-Dist: scipy
-Requires-Dist: shapely
+Requires-Dist: shapely >=2.0.0
 Requires-Dist: xarray
 Requires-Dist: nbsphinx ; extra == "doc"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_design ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
 Requires-Dist: sphinx_autosummary_accessors ; extra == "doc"
 Requires-Dist: pytest>=2.7.3 ; extra == "test"
@@ -42,15 +37,15 @@
 HydroMT-delwaq: DELWAQ plugin for HydroMT
 #########################################
 
 |pypi| |docs_latest| |docs_stable| |codecov| |license| |binder|
 
 What is HydroMT-delwaq?
 -----------------------
-HydroMT-delwaq is a plugin of the `HydroMT core <https://deltares.github.io/hydromt/latest/index.html#>`_, a python package, developed by Deltares, to build 
+HydroMT-delwaq is a plugin of the `HydroMT core <https://deltares.github.io/hydromt/latest/index.html>`_, a python package, developed by Deltares, to build 
 and analyse environmental models. This plugin provides an implementation for the `DELWAQ <https://www.deltares.nl/en/software/module/d-water-quality/>`_ water quality engine. 
 It details the different steps and explains how to use HydroMT to easily get started and work on your own DELWAQ model. WIth this plugin 
 you can interact with both classic **D-Water Quality** models as well as **D-Emission** models.
 
 With the **HydroMT-delwaq plugin**, users can easily benefit from the rich set of tools of the 
 `HydroMT package <https://github.com/Deltares/hydromt>`_ to build and update 
 DELWAQ models from available global and local data.
```

