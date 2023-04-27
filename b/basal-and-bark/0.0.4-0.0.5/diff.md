# Comparing `tmp/basal_and_bark-0.0.4.tar.gz` & `tmp/basal_and_bark-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basal_and_bark-0.0.4.tar", last modified: Fri Apr 21 19:24:09 2023, max compression
+gzip compressed data, was "basal_and_bark-0.0.5.tar", last modified: Thu Apr 27 15:48:18 2023, max compression
```

## Comparing `basal_and_bark-0.0.4.tar` & `basal_and_bark-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/basal_and_bark/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/basal_and_bark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/basal_and_bark/basal_and_bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/basal_and_bark/basal_and_bark_folium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/basal_and_bark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 19:23:57.000000 basal_and_bark-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-21 19:23:57.000000 basal_and_bark-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/basal_and_bark/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/basal_and_bark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/basal_and_bark/basal_and_bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/basal_and_bark/basal_and_bark_folium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/basal_and_bark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 15:47:58.000000 basal_and_bark-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-27 15:47:58.000000 basal_and_bark-0.0.5/setup.py
```

### Comparing `basal_and_bark-0.0.4/LICENSE` & `basal_and_bark-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.4/PKG-INFO` & `basal_and_bark-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal_and_bark
-Version: 0.0.4
+Version: 0.0.5
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,14 +21,16 @@
 License-File: LICENSE
 
 # basal_and_bark
 
 
 [![image](https://img.shields.io/pypi/v/basal_and_bark.svg)](https://pypi.python.org/pypi/basal_and_bark)
 [![image](https://img.shields.io/conda/vn/conda-forge/basal_and_bark.svg)](https://anaconda.org/conda-forge/basal_and_bark)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/basal-and-bark/badges/version.svg)](https://anaconda.org/conda-forge/basal-and-bark)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/basal-and-bark/badges/downloads.svg)](https://anaconda.org/conda-forge/basal-and-bark)
 
 
 **Welcome to Basal and Bark, a spatial python package for working with forest data!**
 
 
 -   Free software: MIT license
 -   Documentation: https://ZachDorm.github.io/basal_and_bark
```

### Comparing `basal_and_bark-0.0.4/basal_and_bark/basal_and_bark.py` & `basal_and_bark-0.0.5/basal_and_bark/basal_and_bark.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import string
 import random
 import ipyleaflet
 from ipyleaflet import GeoData, LayersControl, GeoJSON
 # import folium
 # from folium import TileLayer
 import xyzservices.providers as xyz
+import ipywidgets as widgets
+from ipyleaflet import WidgetControl
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries
 
 def generate_random_string(length):
     """Generates a random string
 
@@ -246,27 +248,90 @@
 
     def add_image(self, url, **kwargs):
         """Add a static image to the bottom right corner of a basal_and_bark map.
 
         Args:
             url (String): The url where the image to add is located.
         """        
-        import ipywidgets as widgets
-        from ipyleaflet import WidgetControl
+        # import ipywidgets as widgets
+        # from ipyleaflet import WidgetControl
 
         output_widget = widgets.Output(layout={'border': '1px solid black'})
         output_widget.clear_output()
         output_control = WidgetControl(widget=output_widget, position='bottomright')
         self.add_control(output_control)
         logo = widgets.HTML(
             value='<img src="https://wvstateparks.com/wp-content/uploads/2017/03/Ascend-WV-Brand-Photo-Coopers-Rock-State-Forest-Morgantown-scaled.jpg" width="200" height="200">'
             )
         with output_widget:
             display(logo)
 
+    def add_interactive_basemap(self, **kwargs):
+        """Add a dropdown ipywidget that provides options for a basemap from xyz.services
+
+        Args:
+            self: basal_and_bark map: Map the user wants to add the interactive basemap to.
+
+        Returns:
+            basal_and_bark map: basal_and_bark map with new basemap, function is observing for change in value
+        """        
+        output_widget = widgets.Output(layout={'border': '1px solid black'})
+        output_widget.clear_output()
+        basemap_ctrl = WidgetControl(widget=output_widget, position='bottomright')
+        self.add_control(basemap_ctrl)
+
+        dropdown = widgets.Dropdown(
+            options = ["Topo", "ShadeRelief", "Gray"], 
+            value=None,
+            description='Basemap',
+            )
+
+        close_button = widgets.ToggleButton(
+            value=True,
+            tooltip="Open or close basemap selector",
+            icon="desktop",
+            button_style="primary",
+            #layout=widgets.Layout(height="28px", width="28px", padding=padding),
+        )
+        close_button
+
+        h = widgets.VBox([close_button, dropdown])
+
+
+        with output_widget:
+            # if basemap_ctrl not in leaflet_map.controls:
+            display(h)
+
+        def change_basemap(change):
+            if change["new"] == "Topo":
+                self.add_basemap(basemap= "Esri.WorldTopoMap")
+            if change["new"] == "ShadeRelief":
+                self.add_basemap(basemap= "Esri.WorldShadedRelief")
+            if change["new"] == "Gray":
+                self.add_basemap(basemap= "Esri.WorldGrayCanvas")
+        
+        dropdown.observe(change_basemap, "value")
+
+        def close_basemap(change):
+    
+            if change["new"] == True:
+                output_widget.clear_output()
+                with output_widget:
+            # if basemap_ctrl not in leaflet_map.controls:
+                    display(h)
+            else:
+                output_widget.clear_output()
+                with output_widget:
+            # if basemap_ctrl not in leaflet_map.controls:
+                    display(close_button)
+        
+        close_button.observe(close_basemap, "value")
+
+
+
```

### Comparing `basal_and_bark-0.0.4/basal_and_bark/basal_and_bark_folium.py` & `basal_and_bark-0.0.5/basal_and_bark/basal_and_bark_folium.py`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.4/setup.py` & `basal_and_bark-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='basal_and_bark',
     name='basal_and_bark',
     packages=find_packages(include=['basal_and_bark', 'basal_and_bark.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZachDorm/basal_and_bark',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

