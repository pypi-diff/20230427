# Comparing `tmp/geomapdemo-0.2.1.tar.gz` & `tmp/geomapdemo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.2.1.tar", last modified: Tue Apr 25 04:12:52 2023, max compression
+gzip compressed data, was "geomapdemo-0.2.2.tar", last modified: Thu Apr 27 03:40:39 2023, max compression
```

## Comparing `geomapdemo-0.2.1.tar` & `geomapdemo-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:12:52.590925 geomapdemo-0.2.1/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/geomapdemo/foliumap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:40:38.996934 geomapdemo-0.2.2/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/geomapdemo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 03:40:38.000000 geomapdemo-0.2.2/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 03:40:39.000934 geomapdemo-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 03:40:26.000000 geomapdemo-0.2.2/setup.py
```

### Comparing `geomapdemo-0.2.1/LICENSE` & `geomapdemo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.2.1/PKG-INFO` & `geomapdemo-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -26,14 +26,15 @@
 [![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
 [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://zyang91.github.io/geomapdemo-jupyter-lite/)
 ![image](https://github.com/zyang91/geomapdemo/workflows/docs/badge.svg)
 ![image](https://github.com/zyang91/geomapdemo/workflows/build/badge.svg)
+[![Github Badge](https://img.shields.io/badge/Github-Repo-yellow)](https://github.com/zyang91/geomapdemo)
 
 **A python package for interactive mapping.**
 
 
 - Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
```

### Comparing `geomapdemo-0.2.1/README.md` & `geomapdemo-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
 [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://zyang91.github.io/geomapdemo-jupyter-lite/)
 ![image](https://github.com/zyang91/geomapdemo/workflows/docs/badge.svg)
 ![image](https://github.com/zyang91/geomapdemo/workflows/build/badge.svg)
+[![Github Badge](https://img.shields.io/badge/Github-Repo-yellow)](https://github.com/zyang91/geomapdemo)
 
 **A python package for interactive mapping.**
 
 
 - Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
```

### Comparing `geomapdemo-0.2.1/geomapdemo/foliumap.py` & `geomapdemo-0.2.2/geomapdemo/foliumap.py`

 * *Files 15% similar despite different names*

```diff
@@ -173,8 +173,59 @@
                 kwargs["style_function"] = lambda x: style_dict
 
 
         geojson = folium.GeoJson(
             data=data, name=layer_name, **kwargs
         )
         self.add_child(geojson)
+    
+    def add_shp(self, path, name="Shapefile", **kwargs):
+
+        """Adds a shapefile to the map
+        Args:
+            path (str): The path to the shapefile.
+            name (str, optional): The name of the shapefile. Defaults to 'Shapefile'.
+            **kwargs: Keyword arguments to be passed to the shapefile.
+        """        
+        import geopandas as gpd
+        gdf = gpd.read_file(path)
+        geojson = gdf.__geo_interface__
+        json= folium.GeoJson(data=geojson, name=name, **kwargs)
+        self.add_child(json)
+        
+    def add_choropleth_map(self, json, csv, columns,key_on,name="choropleth", fill_color='YlGn', legend_name='', **kwargs):
+        """Adds a choropleth map to the map
+        Args:
+            json (str): The path to the json file.
+            csv (str): The path to the csv file.
+            name (str, optional): The name of the choropleth map. Defaults to 'choropleth'.
+            fill_color (str, optional): The color scale of the choropleth map. Defaults to 'YlGn'.
+            legend_name (str, optional): The name of the legend. Defaults to ''.
+            **kwargs: Keyword arguments to be passed to the choropleth map.
+        """        
+        import geopandas as gpd
+        import pandas as pd
+        df = pd.read_csv(csv)
+
+        if "fill_opacity" not in kwargs:
+            kwargs["fill_opacity"] = 0.7
         
+        if "line_opacity" not in kwargs:
+            kwargs["line_opacity"] = 0.2
+
+        choropleth = folium.Choropleth(
+            geo_data=json,
+            name=name,
+            data=df,
+            columns=columns,
+            key_on= key_on,
+            fill_color=fill_color,
+            legend_name=legend_name,
+            **kwargs
+        )
+        self.add_child(choropleth)
+        self.add_child(folium.LayerControl())
+    
+    def add_layer_control(self):
+        """Adds a layer control to the map
+        """        
+        self.add_child(folium.LayerControl())
```

### Comparing `geomapdemo-0.2.1/geomapdemo/geomapdemo.py` & `geomapdemo-0.2.2/geomapdemo/geomapdemo.py`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.2.1/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.2.2/geomapdemo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -26,14 +26,15 @@
 [![Downloads](https://static.pepy.tech/badge/geomapdemo)](https://pepy.tech/project/geomapdemo)
 [![image](https://img.shields.io/pypi/v/geomapdemo.svg)](https://pypi.python.org/pypi/geomapdemo)
 [![image](https://img.shields.io/conda/vn/conda-forge/geomapdemo.svg)](https://anaconda.org/conda-forge/geomapdemo)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zyang91/geomapdemo/HEAD)
 [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://zyang91.github.io/geomapdemo-jupyter-lite/)
 ![image](https://github.com/zyang91/geomapdemo/workflows/docs/badge.svg)
 ![image](https://github.com/zyang91/geomapdemo/workflows/build/badge.svg)
+[![Github Badge](https://img.shields.io/badge/Github-Repo-yellow)](https://github.com/zyang91/geomapdemo)
 
 **A python package for interactive mapping.**
 
 
 - Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
```

### Comparing `geomapdemo-0.2.1/setup.py` & `geomapdemo-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

