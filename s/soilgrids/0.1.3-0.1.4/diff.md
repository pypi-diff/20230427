# Comparing `tmp/soilgrids-0.1.3-py3-none-any.whl.zip` & `tmp/soilgrids-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12371 bytes, number of entries: 11
--rw-r--r--  2.0 unx      290 b- defN 22-Aug-11 20:56 soilgrids/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 22-Aug-11 21:12 soilgrids/_version.py
--rw-r--r--  2.0 unx    22361 b- defN 22-Aug-11 20:56 soilgrids/bmi.py
--rw-r--r--  2.0 unx     2566 b- defN 22-Aug-11 20:56 soilgrids/cli.py
--rw-r--r--  2.0 unx     8122 b- defN 22-Aug-11 20:56 soilgrids/soilgrids.py
--rwxr-xr-x  2.0 unx     1065 b- defN 22-Aug-11 21:12 soilgrids-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4356 b- defN 22-Aug-11 21:12 soilgrids-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-11 21:12 soilgrids-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 22-Aug-11 21:12 soilgrids-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 22-Aug-11 21:12 soilgrids-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      877 b- defN 22-Aug-11 21:12 soilgrids-0.1.3.dist-info/RECORD
-11 files, 40286 bytes uncompressed, 10891 bytes compressed:  73.0%
+Zip file size: 12655 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      290 b- defN 23-Apr-26 21:30 soilgrids/__init__.py
+-rw-r--r--  2.0 unx      498 b- defN 23-Apr-26 22:26 soilgrids/_version.py
+-rw-r--r--  2.0 unx    22361 b- defN 23-Apr-26 21:30 soilgrids/bmi.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Apr-26 21:30 soilgrids/cli.py
+-rw-r--r--  2.0 unx     8362 b- defN 23-Apr-26 21:51 soilgrids/soilgrids.py
+-rwxr-xr-x  2.0 unx     1065 b- defN 23-Apr-26 22:26 soilgrids-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4896 b- defN 23-Apr-26 22:26 soilgrids-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 22:26 soilgrids-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-26 22:26 soilgrids-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-26 22:26 soilgrids-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      877 b- defN 23-Apr-26 22:26 soilgrids-0.1.4.dist-info/RECORD
+11 files, 41066 bytes uncompressed, 11175 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: soilgrids/cli.py
 Comment: 
 
 Filename: soilgrids/soilgrids.py
 Comment: 
 
-Filename: soilgrids-0.1.3.dist-info/LICENSE.txt
+Filename: soilgrids-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: soilgrids-0.1.3.dist-info/METADATA
+Filename: soilgrids-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: soilgrids-0.1.3.dist-info/WHEEL
+Filename: soilgrids-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: soilgrids-0.1.3.dist-info/entry_points.txt
+Filename: soilgrids-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: soilgrids-0.1.3.dist-info/top_level.txt
+Filename: soilgrids-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: soilgrids-0.1.3.dist-info/RECORD
+Filename: soilgrids-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## soilgrids/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-08-11T14:55:15-0600",
+ "date": "2023-04-26T16:09:42-0600",
  "dirty": false,
  "error": null,
- "full-revisionid": "49e4ad5f0bd8eb6d039fbf61a5c71d4ad0a8ec85",
- "version": "v0.1.3"
+ "full-revisionid": "3eb2219663e5d4a39362c42a23087ad67b65e7bb",
+ "version": "v0.1.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## soilgrids/soilgrids.py

```diff
@@ -70,14 +70,20 @@
 
         'ocd': {
             'name': 'Organic carbon densities',
             'link': 'https://maps.isric.org/mapserv?map=/map/ocd.map',
             'units': 'hg/dm3'
         },
 
+        'wrb': {
+            'name': 'World Reference Base (WRB) classes and probabilities',
+            'link': 'https://maps.isric.org/mapserv?map=/map/wrb.map',
+            'units': 'none'
+        },
+
     }  # service info at http://maps.isric.org/ https://www.isric.org/explore/soilgrids/faq-soilgrids
 
     def __init__(self):
         self._tif_file = None
         self._metadata = None
 
     @property
@@ -88,16 +94,16 @@
     def metadata(self):
         return self._metadata
 
     @property
     def map_services(self):
         string_list = []
         for key, value in SoilGrids.MAP_SERVICES.items():
-            string_list.append('service id: {} \nvariable name: {} \nservice link: {}\n'.
-                               format(key, value['name'], value['link']))
+            string_list.append('service id: {} \nvariable name: {} \nvariable units: {}\nservice link: {}\n'.
+                               format(key, value['name'], value['units'], value['link']))
         print('\n'.join(string_list))
 
         return None
 
     def get_coverage_list(self, service_id):
         _, coverage_list = self._get_service_and_coverage_list(service_id)
```

## Comparing `soilgrids-0.1.3.dist-info/LICENSE.txt` & `soilgrids-0.1.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `soilgrids-0.1.3.dist-info/METADATA` & `soilgrids-0.1.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soilgrids
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fetch global gridded soil information from the SoilGrids system https://www.isric.org/explore/soilgrids
 Home-page: http://csdms.colorado.edu
 Author: Tian Gan
 Author-email: jamy127@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: bmipy
@@ -20,31 +20,41 @@
 # soilgrids
 [![Documentation Status](https://readthedocs.org/projects/soilgrids/badge/?version=latest)](https://soilgrids.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/gantian127/soilgrids/blob/master/LICENSE.txt)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gantian127/soilgrids/master?filepath=notebooks%2Fsoilgrids.ipynb)
 
 
 
-Python library to fetch the global gridded soil information from [SoilGrids](https://www.isric.org/explore/soilgrids),
+soilgrids provides a set of functions that allow downloading of
+the global gridded soil information from [SoilGrids](https://www.isric.org/explore/soilgrids),
 a system for global digital soil mapping to map the spatial distribution of soil properties across the globe.  
 
+soilgrids also includes a [Basic Model Interface (BMI)](https://bmi.readthedocs.io/en/latest/),
+which converts the SoilGrids dataset into a reusable,
+plug-and-play data component ([pymt_soilgrids](https://pymt-soilgrids.readthedocs.io/)) for 
+the [PyMT](https://pymt.readthedocs.io/en/latest/?badge=latest) modeling framework developed 
+by Community Surface Dynamics Modeling System ([CSDMS](https://csdms.colorado.edu/wiki/Main_Page)).
+
 If you have any suggestion to improve the current function, please create a github issue 
 [here](https://github.com/gantian127/soilgrids/issues).
 
 ## Get Started
 
 #### Install package
 
 ##### Stable Release
 
-The soilgrids package and its dependencies can be installed with pip.
+The soilgrids package and its dependencies can be installed with pip
 ```
 $ pip install soilgrids
 ```
-
+or with conda.
+```
+$ conda install -c conda-forge soilgrids
+```
 ##### From Source
 
 After downloading the source code, run the following command from top-level folder 
 (the one that contains setup.py) to install soilgrids.
 ```
 $ pip install -e .
 ```
```

## Comparing `soilgrids-0.1.3.dist-info/RECORD` & `soilgrids-0.1.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 soilgrids/__init__.py,sha256=hrXcPBHO4iQn6FZfr7z0rbl32ufCGn2yexlawNNk1D4,290
-soilgrids/_version.py,sha256=GdlSejYer4mPFH1CVDyc8pT9zmVyDpb-gvIuKitlVa0,498
+soilgrids/_version.py,sha256=5Jv2rq5BGWzVw6qGg2rXworwgR2Wh3irnK18PLCoIyU,498
 soilgrids/bmi.py,sha256=-lbT1CMltEAtvkS5PQ0EMIv4M_pbwMzu4tOLAUhyYP8,22361
 soilgrids/cli.py,sha256=_bfiKSgElUzdTEu1jQ3sRx4kNPGCknrlfWAKdULOjIw,2566
-soilgrids/soilgrids.py,sha256=3kLpTobKFaOikd5GQfjMNE-oA5gJctFXyxxU2lhjeC8,8122
-soilgrids-0.1.3.dist-info/LICENSE.txt,sha256=RB2j7Q7yo5Fj82wh-ux_ogm2xiecsc7J8hhvepCn_KI,1065
-soilgrids-0.1.3.dist-info/METADATA,sha256=Ts30mEA4IBUyqAClaqW8V2l1u1cxCTyU6Vdr14cOMWk,4356
-soilgrids-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-soilgrids-0.1.3.dist-info/entry_points.txt,sha256=OUQ0kclXeoov1TRXQta76lihi8rrfbLC5QS2_0THfJ0,49
-soilgrids-0.1.3.dist-info/top_level.txt,sha256=9O5NyVtjGc42dnQulr0XzyqgpJ07VYW_c5xI1PTx5GU,10
-soilgrids-0.1.3.dist-info/RECORD,,
+soilgrids/soilgrids.py,sha256=JeXf9XOXEoF2zqFVSe_v79nltEc25ob-IiiyiksXBTw,8362
+soilgrids-0.1.4.dist-info/LICENSE.txt,sha256=RB2j7Q7yo5Fj82wh-ux_ogm2xiecsc7J8hhvepCn_KI,1065
+soilgrids-0.1.4.dist-info/METADATA,sha256=mL4kM8ZUGdvFBGSVGEhcGRni76HUf4VV_LSNCCEl-38,4896
+soilgrids-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+soilgrids-0.1.4.dist-info/entry_points.txt,sha256=OUQ0kclXeoov1TRXQta76lihi8rrfbLC5QS2_0THfJ0,49
+soilgrids-0.1.4.dist-info/top_level.txt,sha256=9O5NyVtjGc42dnQulr0XzyqgpJ07VYW_c5xI1PTx5GU,10
+soilgrids-0.1.4.dist-info/RECORD,,
```

