# Comparing `tmp/pyaemet-1.1.0rc1.tar.gz` & `tmp/pyaemet-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaemet-1.1.0rc1.tar", max compression
+gzip compressed data, was "pyaemet-1.1.0rc2.tar", max compression
```

## Comparing `pyaemet-1.1.0rc1.tar` & `pyaemet-1.1.0rc2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    35149 2022-08-29 18:57:39.634520 pyaemet-1.1.0rc1/LICENSE
--rw-r--r--   0        0        0     4584 2023-04-24 20:17:14.017440 pyaemet-1.1.0rc1/README.md
--rw-r--r--   0        0        0     1174 2023-04-24 21:29:29.586546 pyaemet-1.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-24 21:27:51.334140 pyaemet-1.1.0rc1/src/pyaemet/__init__.py
--rw-r--r--   0        0        0     6050 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc1/src/pyaemet/aemet_request.py
--rw-r--r--   0        0        0    18982 2023-04-24 21:27:51.334140 pyaemet-1.1.0rc1/src/pyaemet/climatology.py
--rw-r--r--   0        0        0        0 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc1/src/pyaemet/static/__init__.py
--rw-r--r--   0        0        0    33781 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/static/sites/data.csv
--rw-r--r--   0        0        0     3029 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/static/sites/metadata.json
--rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/types_classes/__init__.py
--rw-r--r--   0        0        0      866 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/types_classes/observations.py
--rw-r--r--   0        0        0    10835 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/types_classes/sites.py
--rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/__init__.py
--rw-r--r--   0        0        0     2127 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/coordinates.py
--rw-r--r--   0        0        0     1865 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/curation.py
--rw-r--r--   0        0        0     2511 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/dictionaries.py
--rw-r--r--   0        0        0     5669 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc1/setup.py
--rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-29 18:57:39.634520 pyaemet-1.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     4584 2023-04-24 20:17:14.017440 pyaemet-1.1.0rc2/README.md
+-rw-r--r--   0        0        0     1141 2023-04-26 21:26:32.651907 pyaemet-1.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-04-26 21:02:31.008873 pyaemet-1.1.0rc2/src/pyaemet/__init__.py
+-rw-r--r--   0        0        0     6050 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc2/src/pyaemet/aemet_request.py
+-rw-r--r--   0        0        0    19140 2023-04-26 17:34:07.453859 pyaemet-1.1.0rc2/src/pyaemet/climatology.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc2/src/pyaemet/static/__init__.py
+-rw-r--r--   0        0        0    33781 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/static/sites/data.csv
+-rw-r--r--   0        0        0     3029 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/static/sites/metadata.json
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/types_classes/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/types_classes/observations.py
+-rw-r--r--   0        0        0    11001 2023-04-26 21:00:31.136293 pyaemet-1.1.0rc2/src/pyaemet/types_classes/sites.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/utilities/__init__.py
+-rw-r--r--   0        0        0     2127 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/utilities/coordinates.py
+-rw-r--r--   0        0        0     1865 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/utilities/curation.py
+-rw-r--r--   0        0        0     2511 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc2/src/pyaemet/utilities/dictionaries.py
+-rw-r--r--   0        0        0     5884 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc2/PKG-INFO
```

### Comparing `pyaemet-1.1.0rc1/LICENSE` & `pyaemet-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/README.md` & `pyaemet-1.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/pyproject.toml` & `pyaemet-1.1.0rc2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyaemet"
-version = "1.1.0rc1"
+version = "1.1.0rc2"
 
 description = "Python module to interact with the AEMET API to download meteorological data"
 readme = "README.md"
 homepage = "https://github.com/jaimedgp/pyAEMET"
 repository = "https://github.com/jaimedgp/pyAEMET"
 license = "GPL-3.0-or-later"
 
@@ -30,25 +30,22 @@
     { path = ".env" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/jaimedgp/pyAEMET/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
-requests = "2.24.0"
-numpy = "1.19.0"
-matplotlib = "3.2.2"
-pandas = "1.1.0"
-geocoder = "1.38.0"
-folium = "0.11.0"
-tqdm = "4.46.1"
-
-[tool.poetry.group.dev.dependencies]
-
+python = ">=3.8,<4.0"
+requests = "^2.24.0"
+numpy = "^1.19.0"
+matplotlib = "^3.2.2"
+pandas = "^1.1.0"
+geocoder = "^1.38.0"
+folium = "^0.11.0"
+tqdm = "^4.46.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "6.0.0"
 python-dotenv = "0.14.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/aemet_request.py` & `pyaemet-1.1.0rc2/src/pyaemet/aemet_request.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/climatology.py` & `pyaemet-1.1.0rc2/src/pyaemet/climatology.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Web Service API. It has several functions to request information about
 climatic stations and to download meteorological observations data.
 """
 
 import os
 import logging
 from datetime import date, datetime
+from typing import Optional, Union
 from dateutil.relativedelta import relativedelta
 from pkg_resources import resource_stream
 
 from tqdm import tqdm
 import numpy as np
 from pandas import Series, DataFrame, concat
 
@@ -167,15 +168,15 @@
         # Filter the information of the climatic stations
         return self.aemet_sites.filter_in(**kwargs,)
 
     def estaciones_loc(
         self,
         actualizar: bool = False,
         **kwargs,
-    ) -> DataFrame | None:
+    ) -> Optional[DataFrame]:
         """
         Get location data for stations available in Aemet.
 
         .. deprecated:: 1.1.0
             Please use `sites_in()` instead and take advantage
             of `SitesDataFrame` new options.
 
@@ -204,18 +205,18 @@
 
         return self.sites_in(**new_kwargs, update_first=actualizar) \
                    .as_dataframe() \
                    .rename(columns=V1_TRANSLATION)
 
     def near_sites(
         self,
-        latitude: float | int,
-        longitude: float | int,
-        n_near: int | None = 100,
-        max_distance: float | int = 6237,
+        latitude: Union[float, int],
+        longitude: Union[float, int],
+        n_near: Optional[int] = 100,
+        max_distance: Union[float, int] = 6237,
         update_first: bool = False,
     ) -> NearSitesDataFrame:
         """
         Retrieve information about climatic stations near a set of coordinates.
 
         Parameters
         ----------
@@ -248,20 +249,20 @@
             latitude,
             longitude,
             n_near,
             max_distance)
 
     def estaciones_cerca(
         self,
-        latitud: int | float,
-        longitud: int | float,
-        n_cercanas: int | None = 100,
-        max_distancia: int | float = 6237,
+        latitud: Union[int, float],
+        longitud: Union[int, float],
+        n_cercanas: Optional[int] = 100,
+        max_distancia: Union[int, float] = 6237,
         actualizar: bool = False,
-        ) -> DataFrame | None:
+        ) -> Union[DataFrame]:
         """
         Retrieve information about climatic stations near a set of coordinates.
 
         .. deprecated:: 1.1.0
             Please use `near_sites()` instead and take advantage
             of `NearSitesDataFrame` new options.
 
@@ -300,24 +301,24 @@
                                n_near=n_cercanas,
                                max_distance=max_distancia) \
                     .as_dataframe() \
                     .rename(columns=V1_TRANSLATION)
 
     def sites_curation(
         self,
-        start_dt: date | datetime,
-        sites: ( str | list
-               | Series | DataFrame
-               | SitesDataFrame | NearSitesDataFrame),
-        end_dt: date | datetime = date.today(),
+        start_dt: Union[date, datetime],
+        sites: Union[
+            str, list, Series, DataFrame , SitesDataFrame, NearSitesDataFrame
+        ],
+        end_dt: Union[date, datetime] = date.today(),
         threshold: float = 0.75,
-        variables: str | list = 'all',
-        save_folder: str | os.PathLike | None = ...,
+        variables: Union[str, list] = 'all',
+        save_folder: Optional[Union[str, os.PathLike]] = ...,
         verbosity: bool = True,
-        ) -> SitesDataFrame | NearSitesDataFrame | DataFrame:
+        ) -> Union[SitesDataFrame, NearSitesDataFrame, DataFrame]:
         """
 
         Parameters
         ----------
         sites : str,
         start_dt : date
             Start date to define curation period in which the porcentage of
@@ -409,22 +410,22 @@
             if is_enough and save_folder is not None:
                 data.to_csv(save_folder+st+".csv")
 
         return _sites
 
     def estaciones_curacion(
         self,
-        fecha_ini: date | datetime,
-        fecha_fin: date | datetime = date.today(),
+        fecha_ini: Union[date, datetime],
+        fecha_fin: Union[date, datetime] = date.today(),
         umbral: float = 0.75,
-        variables: str | list = 'all',
-        save_folder: str | None = None,
+        variables: Union[str, list] = 'all',
+        save_folder: Optional[str] = None,
         actualizar: bool = False,
         **kwargs
-        ) -> DataFrame | None:
+        ) -> Optional[DataFrame]:
         """ Docstring """
 
         logger.warning("<AemetClima>.estaciones_curacion() is deprecated "
                        + "since version 1.1.0. Please use "
                        + "<AemetClima>.sites_curation() instead and take "
                        + "advantage of <SitesDataFrame> and "
                        + "<NearSitesDataFrame> new options.")
@@ -443,16 +444,16 @@
                                     ) \
                     .as_dataframe() \
                     .rename(columns=V1_TRANSLATION)
 
     def daily_clima(
         self,
         site,
-        start_dt: date | datetime,
-        end_dt: date | datetime = date.today(),
+        start_dt: Union[date, datetime],
+        end_dt: Union[date, datetime] = date.today(),
         verbosity: bool = True
         ) -> ObservationsDataFrame:
         """
         """
 
         if isinstance(site, str):
             pass
@@ -481,16 +482,16 @@
         return ObservationsDataFrame(data=concat(data_list),
                                      library="pyaemet",
                                      metadata=metadata)
 
     def clima_diaria(
         self,
         estacion,
-        fecha_ini: date | datetime,
-        fecha_fin: date | datetime = date.today()
+        fecha_ini: Union[date, datetime],
+        fecha_fin: Union[date, datetime] = date.today()
         ) -> ObservationsDataFrame:
         """
         """
 
         logger.warning("<AemetClima>.clima_diaria() is deprecated since "
                        + "version 1.1.0. Please use <AemetClima>.daily_clima() "
                        + "instead and take advantage of <SitesDataFrame> "
@@ -498,15 +499,15 @@
 
         return self.daily_clima(site=estacion,
                                 start_dt=fecha_ini,
                                 end_dt=fecha_fin)
 
     @staticmethod
     def _have_enough(data_frame, start_date, end_date,
-                     threshold=0.75, columns: str | list = 'all'):
+                     threshold=0.75, columns: Union[str, list] = 'all'):
         """ Docstring """
 
         if isinstance(columns, str):
             columns = [columns]
 
         if any(col not in data_frame.columns for col in columns):
             return False, 0.0
```

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/static/sites/data.csv` & `pyaemet-1.1.0rc2/src/pyaemet/static/sites/data.csv`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/static/sites/metadata.json` & `pyaemet-1.1.0rc2/src/pyaemet/static/sites/metadata.json`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/types_classes/observations.py` & `pyaemet-1.1.0rc2/src/pyaemet/types_classes/observations.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/types_classes/sites.py` & `pyaemet-1.1.0rc2/src/pyaemet/types_classes/sites.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 SitesDataFrame
 -----------------
 
 """
 
 import os
 import json
+from typing import List, Optional
 
 import pandas
 import folium
 import numpy as np
 
 
 class SitesDataFrame(pandas.DataFrame):
@@ -27,16 +28,16 @@
     def __init__(
             self,
             data=None,
             index=None,
             columns=None,
             dtype=None,
             copy=None,
-            library: str = None,
-            metadata: dict = None,
+            library: Optional[str] = None,
+            metadata: Optional[dict] = None,
     ):
 
         super().__init__(
             data=data,
             index=index,
             columns=columns,
             dtype=dtype,
@@ -67,34 +68,36 @@
         # verify there is a column site and a column name
         if "site" not in obj.columns or "name" not in obj.columns:
             raise AttributeError("Each site must be identify by a code 'site'"
                                  + " and its name 'name'.")
 
     @staticmethod
     def open_from(
-            data_fl: str = None,
-            metadata_fl: str = None,
-            folder_name: str = None
+            data_fl: Optional[str] = None,
+            metadata_fl: Optional[str] = None,
+            folder_name: Optional[str] = None
     ):
         """
         """
 
         if data_fl is None:
             if folder_name is None:
                 raise KeyError("Not correct file path")
             data_fl = folder_name + "data.pkl"
         if metadata_fl is None:
             if folder_name is None:
                 raise KeyError("Not correct file path")
             metadata_fl = folder_name + "metadata.json"
 
+        metadata = json.load(metadata_fl)
+
         return SitesDataFrame(
             data=pandas.read_csv(data_fl),
             library="pyaemet",
-            metadata=json.load(metadata_fl)
+            metadata=metadata
             )
 
     def save(self, folder_name: str, extension: str = 'pickle'):
         """
         """
 
         if not os.path.exists(folder_name):
@@ -243,15 +246,15 @@
         latitude,
         longitude,
         distance (TO THE REFERENCE POINT)
     """
 
     def __init__(
             self,
-            ref_point: [float, float],
+            ref_point: List[float],
             data=None,
             index=None,
             columns=None,
             dtype=None,
             copy=None,
             library=None,
             metadata=None,
@@ -298,14 +301,17 @@
 
     @property
     def map(self):
         """
         plot map with the sites location
         """
 
+        if self.empty:
+            return folium.Map()
+
         index_lat, = np.where(self.columns == "latitude")[0]
         index_lon, = np.where(self.columns == "longitude")[0]
 
         latitudes = self._get_column_array(index_lat)
         longitudes = self._get_column_array(index_lon)
 
         center = [np.mean([np.min(latitudes), np.max(latitudes)]),
```

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/utilities/coordinates.py` & `pyaemet-1.1.0rc2/src/pyaemet/utilities/coordinates.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/utilities/curation.py` & `pyaemet-1.1.0rc2/src/pyaemet/utilities/curation.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/src/pyaemet/utilities/dictionaries.py` & `pyaemet-1.1.0rc2/src/pyaemet/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc1/setup.py` & `pyaemet-1.1.0rc2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyaemet
+Version: 1.1.0rc2
+Summary: Python module to interact with the AEMET API to download meteorological data
+Home-page: https://github.com/jaimedgp/pyAEMET
+License: GPL-3.0-or-later
+Keywords: AEMET,Meteorology,API,AEMET OpenData
+Author: Jaimedgp
+Author-email: jaime.diez.gp@gmail.com
+Maintainer: CarmenGBM
+Maintainer-email: carmen.garcia.be96@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: folium (>=0.11.0,<0.12.0)
+Requires-Dist: geocoder (>=1.38.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.2.2,<4.0.0)
+Requires-Dist: numpy (>=1.19.0,<2.0.0)
+Requires-Dist: pandas (>=1.1.0,<2.0.0)
+Requires-Dist: requests (>=2.24.0,<3.0.0)
+Requires-Dist: tqdm (>=4.46.1,<5.0.0)
+Project-URL: Bug Tracker, https://github.com/jaimedgp/pyAEMET/issues
+Project-URL: Repository, https://github.com/jaimedgp/pyAEMET
+Description-Content-Type: text/markdown
+
+# pyAEMET
+
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pyaemet.svg)](https://pypi.org/project/pyaemet/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5655307.svg)](https://doi.org/10.5281/zenodo.5655307)
+[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/jaimedgp/pyAEMET/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/pyaemet?period=month&units=international_system&left_color=gray&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pyaemet)
+
+A python library developed to download daily climatological values from the Spanish National
+Meteorological Agency (AEMET) through its OpenData API. The library contains several methods
+to facilitate downloading and filtering the climatological data.
+
+> The information that this library collects and uses is property of the Spanish State
+> Meteorological Agency, available through its AEMET OpenData REST API.
+
+
+## Installation
+``` bash
+$ pip install pyaemet
+```
+To use the pyAEMET module, you need to get an API key from the AEMET (Spanish State Meteorological
+Agency) OpenData platform. You can apply for a key [here](https://opendata.aemet.es/centrodedescargas/altaUsuario).
+
+## Usage
+
+Once the module is installed and you have your API key, you can start using the module by
+importing it in your Python script. To use the module's functions, you need to initialize
+the client with your API key:
+
+```python
+import pyaemet
+
+aemet = pyaemet.AemetClima(api_key)
+```
+
+The `AemetClima` class takes an API key as a parameter in its constructor and allows you to get
+information about the available monitoring sites, filter sites based on different parameters
+(e.g., city, province, autonomous community), and get nearby sites to a specific location.
+
+Here is a summary of some of the methods provided by the `AemetClima` class:
+
+* **`sites_info`**: Retrieves information about all the available monitoring sites. The method
+returns an instance of the `SitesDataFrame` class, which is a subclass of the pandas `DataFrame`.
+```python
+aemet.sites_info(update=True)
+```
+
+* **`sites_in`**: Filters the available monitoring sites based on specified parameters
+(e.g., city, province, autonomous community). The method returns an instance of the `SitesDataFrame` class.
+```python
+aemet.sites_in(subregion="Cantabria")
+```
+![image](https://github.com/Jaimedgp/pyAEMET/raw/main/docs/screenshots/sites_cantabria.png)
+
+* **`near_sites`**: Retrieves the ``n_near`` monitoring sites closest to a specified latitude and longitude,
+within a maximum distance of `max_distance` kilometers. The method returns an instance of the
+`NearSitesDataFrame` class.
+```python
+aemet.near_sites(latitude=43.47,
+                 longitude=-3.798,
+                 n_near=5, max_distance=50)
+```
+![image](https://github.com/Jaimedgp/pyAEMET/raw/main/docs/screenshots/near_sites.png)
+
+* **`sites_curation`**: Retrieves the amount of available data of certain `variables` in the monitoring `sites` in a period of time defined by
+    `start_dt` and `end_dt`. The function returns a `SitesDataFrame` or `NearSitesDataFrame` (depends of the type of the `sites` parameter given)
+    with a column with the average `amount` between all `variables` and `has_enough` boolean if the amount is greater or equal to a `threshold`.
+
+* **`daily_clima`**: Retrieves daily climate data for a given ``site`` or a list of sites over a
+specified date range defined by `start_dt` and `end_dt`. The function returns a
+`ObservationsDataFrame` object, which is a data structure that holds the retrieved climate data
+along with any associated metadata.
+```python
+import datetime
+aemet.daily_clima(site=aemet.sites_in(city="Santander"),
+                  start_dt=datetime.date(2022, 6, 3),
+                  end_dt=datetime.date.today())
+```
+
+The module also provides three deprecated methods `estaciones_info`, `estaciones_loc` and `clima_diaria`
+that perform similar functionality as the `sites_info`, `sites_in` and `daily_clima` methods, respectively.
+
+You can find the complete documentation of the module's functions in the GitHub repository,
+under the docs directory.
+
+## FAQ
+## Contributing
+## References
+* ["Estimating changes in air pollutant levels due to COVID-19 lockdown measures based on a business-as-usual prediction scenario using data mining models: A case-study for urban traffic sites in Spain"](https://doi.org/10.1016/j.scitotenv.2022.153786), submitted to Environmental Software & Modelling by [J. González-Pardo](https://orcid.org/0000-0001-7268-9933) et al. (2021)
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pyaemet', 'pyaemet.static', 'pyaemet.types_classes', 'pyaemet.utilities']
-
-package_data = \
-{'': ['*'], 'pyaemet.static': ['sites/*']}
-
-install_requires = \
-['folium==0.11.0',
- 'geocoder==1.38.0',
- 'matplotlib==3.2.2',
- 'numpy==1.19.0',
- 'pandas==1.1.0',
- 'requests==2.24.0',
- 'tqdm==4.46.1']
-
-setup_kwargs = {
-    'name': 'pyaemet',
-    'version': '1.1.0rc1',
-    'description': 'Python module to interact with the AEMET API to download meteorological data',
-    'long_description': '# pyAEMET\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pyaemet.svg)](https://pypi.org/project/pyaemet/)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5655307.svg)](https://doi.org/10.5281/zenodo.5655307)\n[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/jaimedgp/pyAEMET/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pyaemet?period=month&units=international_system&left_color=gray&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pyaemet)\n\nA python library developed to download daily climatological values from the Spanish National\nMeteorological Agency (AEMET) through its OpenData API. The library contains several methods\nto facilitate downloading and filtering the climatological data.\n\n> The information that this library collects and uses is property of the Spanish State\n> Meteorological Agency, available through its AEMET OpenData REST API.\n\n\n## Installation\n``` bash\n$ pip install pyaemet\n```\nTo use the pyAEMET module, you need to get an API key from the AEMET (Spanish State Meteorological\nAgency) OpenData platform. You can apply for a key [here](https://opendata.aemet.es/centrodedescargas/altaUsuario).\n\n## Usage\n\nOnce the module is installed and you have your API key, you can start using the module by\nimporting it in your Python script. To use the module\'s functions, you need to initialize\nthe client with your API key:\n\n```python\nimport pyaemet\n\naemet = pyaemet.AemetClima(api_key)\n```\n\nThe `AemetClima` class takes an API key as a parameter in its constructor and allows you to get\ninformation about the available monitoring sites, filter sites based on different parameters\n(e.g., city, province, autonomous community), and get nearby sites to a specific location.\n\nHere is a summary of some of the methods provided by the `AemetClima` class:\n\n* **`sites_info`**: Retrieves information about all the available monitoring sites. The method\nreturns an instance of the `SitesDataFrame` class, which is a subclass of the pandas `DataFrame`.\n```python\naemet.sites_info(update=True)\n```\n\n* **`sites_in`**: Filters the available monitoring sites based on specified parameters\n(e.g., city, province, autonomous community). The method returns an instance of the `SitesDataFrame` class.\n```python\naemet.sites_in(subregion="Cantabria")\n```\n![image](https://github.com/Jaimedgp/pyAEMET/raw/main/docs/screenshots/sites_cantabria.png)\n\n* **`near_sites`**: Retrieves the ``n_near`` monitoring sites closest to a specified latitude and longitude,\nwithin a maximum distance of `max_distance` kilometers. The method returns an instance of the\n`NearSitesDataFrame` class.\n```python\naemet.near_sites(latitude=43.47,\n                 longitude=-3.798,\n                 n_near=5, max_distance=50)\n```\n![image](https://github.com/Jaimedgp/pyAEMET/raw/main/docs/screenshots/near_sites.png)\n\n* **`sites_curation`**: Retrieves the amount of available data of certain `variables` in the monitoring `sites` in a period of time defined by\n    `start_dt` and `end_dt`. The function returns a `SitesDataFrame` or `NearSitesDataFrame` (depends of the type of the `sites` parameter given)\n    with a column with the average `amount` between all `variables` and `has_enough` boolean if the amount is greater or equal to a `threshold`.\n\n* **`daily_clima`**: Retrieves daily climate data for a given ``site`` or a list of sites over a\nspecified date range defined by `start_dt` and `end_dt`. The function returns a\n`ObservationsDataFrame` object, which is a data structure that holds the retrieved climate data\nalong with any associated metadata.\n```python\nimport datetime\naemet.daily_clima(site=aemet.sites_in(city="Santander"),\n                  start_dt=datetime.date(2022, 6, 3),\n                  end_dt=datetime.date.today())\n```\n\nThe module also provides three deprecated methods `estaciones_info`, `estaciones_loc` and `clima_diaria`\nthat perform similar functionality as the `sites_info`, `sites_in` and `daily_clima` methods, respectively.\n\nYou can find the complete documentation of the module\'s functions in the GitHub repository,\nunder the docs directory.\n\n## FAQ\n## Contributing\n## References\n* ["Estimating changes in air pollutant levels due to COVID-19 lockdown measures based on a business-as-usual prediction scenario using data mining models: A case-study for urban traffic sites in Spain"](https://doi.org/10.1016/j.scitotenv.2022.153786), submitted to Environmental Software & Modelling by [J. González-Pardo](https://orcid.org/0000-0001-7268-9933) et al. (2021)\n',
-    'author': 'Jaimedgp',
-    'author_email': 'jaime.diez.gp@gmail.com',
-    'maintainer': 'CarmenGBM',
-    'maintainer_email': 'carmen.garcia.be96@gmail.com',
-    'url': 'https://github.com/jaimedgp/pyAEMET',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

