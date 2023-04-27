# Comparing `tmp/piproc-0.1.7.tar.gz` & `tmp/piproc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piproc-0.1.7.tar", last modified: Wed Apr 19 10:39:21 2023, max compression
+gzip compressed data, was "piproc-0.1.8.tar", last modified: Thu Apr 27 14:13:36 2023, max compression
```

## Comparing `piproc-0.1.7.tar` & `piproc-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:39:21.463962 piproc-0.1.7/
--rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      266 2023-04-19 10:39:21.463962 piproc-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 10:39:21.445192 piproc-0.1.7/piproc/
--rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.7/piproc/__init__.py
--rw-rw-rw-   0        0        0    15621 2023-04-17 15:22:00.000000 piproc-0.1.7/piproc/main.py
--rw-rw-rw-   0        0        0     2834 2023-04-12 12:34:42.000000 piproc-0.1.7/piproc/tables.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:39:21.462984 piproc-0.1.7/piproc.egg-info/
--rw-rw-rw-   0        0        0      266 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 10:39:21.000000 piproc-0.1.7/piproc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      366 2023-04-19 10:39:21.464932 piproc-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:13:36.111532 piproc-0.1.8/
+-rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-04-27 14:13:36.112042 piproc-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 14:13:36.094682 piproc-0.1.8/piproc/
+-rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.8/piproc/__init__.py
+-rw-rw-rw-   0        0        0    15987 2023-04-27 14:10:12.000000 piproc-0.1.8/piproc/main.py
+-rw-rw-rw-   0        0        0     2834 2023-04-12 12:34:42.000000 piproc-0.1.8/piproc/tables.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:13:36.110528 piproc-0.1.8/piproc.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-27 14:13:36.000000 piproc-0.1.8/piproc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      366 2023-04-27 14:13:36.113045 piproc-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.8/setup.py
```

### Comparing `piproc-0.1.7/LICENSE` & `piproc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `piproc-0.1.7/README.md` & `piproc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `piproc-0.1.7/piproc/main.py` & `piproc-0.1.8/piproc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import os
 import yaml
 import boto3
 import psycopg2
 import sqlalchemy
 
+from botocore.exceptions import NoCredentialsError
 from sqlalchemy.orm import sessionmaker
 from shapely.geometry import Polygon
 from os.path import dirname as up
 
 from .tables import Processing, Products, PlanetProc, PlanetProd
 
 class Piproc:
@@ -19,18 +20,22 @@
     def __init__(self):
         '''
         Initialise connection to the processing database, using locally found credentials or
         downloading them from s3.
         '''
         cred_path = os.path.join(up(up(__file__)), 'credentials.yml')
 
-        if not os.path.isfile(cred_path):
-            s3 = boto3.client('s3')
-            s3.download_file('dockerfilecfg', 'credentials.yml', 
-                os.path.join(up(up(__file__)), 'credentials.yml'))
+        # The try/except is a hack for the cassini project, remove once competition is done.
+        try:
+            if not os.path.isfile(cred_path):
+                s3 = boto3.client('s3')
+                s3.download_file('dockerfilecfg', 'credentials.yml', 
+                    os.path.join(up(up(__file__)), 'credentials.yml'))
+        except NoCredentialsError:
+            cred_path = '/opt/cassini_vis/cred_files/credentials_piproc.yml'
 
         with open(cred_path, 'r') as f:
             self.cred = yaml.safe_load(f)
 
         db = sqlalchemy.create_engine('postgresql:///processing', 
             connect_args={'host': self.cred['processing_db']['host'],
                           'user': self.cred['processing_db']['user'],
@@ -63,15 +68,15 @@
         '''
         A function to check in the Plastic-i processing db if a Planet SuperDove scene has already
         been downloaded.
         '''
         product_id = tile_dict['id']
 
         tile_date = tile_dict['properties']['acquired']
-        tile_date = datetime.datetime.strptime(tile_date, '%Y-%m-%dT%H:%M:%SZ')
+        tile_date = datetime.datetime.strptime(tile_date, '%Y-%m-%dT%H:%M:%S.%fZ')
         out_tile_date = datetime.datetime.strftime(tile_date, '%Y%m%d%H%M%S')
 
         # TODO: This needs to be checked it produces the correct output with clipped imagery
         bounds = Polygon(tile_dict['geometry']['coordinates'][0]).bounds
         lats = str([bounds[1], bounds[3]])
         lons = str([bounds[0], bounds[2]])
 
@@ -82,14 +87,15 @@
         elif file and redownload:
             return False, product_id, out_tile_date
         else:
 
             file = PlanetProc(id=product_id, lons=lons, lats=lats, tile_date=tile_date, 
                               downloaded=0)
             self.session.add(file)
+            self.session.commit()
             return False, product_id, out_tile_date
 
     def check_download(self, tile_dict, redownload):
         '''
         A function to check in the Plastic-i processing db if a tile has already been
         downloaded.
         '''
@@ -189,23 +195,24 @@
         output = {'path': file.download_path,
                 'dt': file.tile_date,
                 'crs': file.crs,
                 'id': file.id
                 }
         return output
 
-    def update_index(self, product_id, yaml_path, satellite='sentinel2', result=2, env=None):
+    def update_index(self, product_id, yaml_path, satellite='sentinel2', result=2, env=None, crs=None):
         '''
         Update the processing db with the status of a Sentinel-2 index process.
         '''
 
         if satellite == 'sentinel2':
             file = self.session.query(Processing).get(product_id)
         elif satellite == 'planet':
             file = self.session.query(PlanetProc).get(product_id)
+            file.crs = crs
 
         file.indexed = result
 
         if result == 2:
             # Only update number of times downloaded if download was successful
             try:
                 file.no_indexed += 1
```

### Comparing `piproc-0.1.7/piproc/tables.py` & `piproc-0.1.8/piproc/tables.py`

 * *Files identical despite different names*

