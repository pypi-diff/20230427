# Comparing `tmp/h5-info-pkg-inra-phenome-1.3.1.tar.gz` & `tmp/h5-info-pkg-inra-phenome-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5-info-pkg-inra-phenome-1.3.1.tar", last modified: Wed Aug 24 14:20:20 2022, max compression
+gzip compressed data, was "h5-info-pkg-inra-phenome-1.3.2.tar", last modified: Wed Apr 12 12:50:04 2023, max compression
```

## Comparing `h5-info-pkg-inra-phenome-1.3.1.tar` & `h5-info-pkg-inra-phenome-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 14:20:20.342877 h5-info-pkg-inra-phenome-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4705 2022-08-24 14:20:20.342877 h5-info-pkg-inra-phenome-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4129 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 14:20:20.342877 h5-info-pkg-inra-phenome-1.3.1/h5_info/
--rw-rw-rw-   0 root         (0) root         (0)    12794 2022-08-24 14:20:15.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/camera_image.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/geo.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/lidar_image.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/multispectral_camera_image.py
--rw-rw-rw-   0 root         (0) root         (0)      639 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/plot.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/position.py
--rw-rw-rw-   0 root         (0) root         (0)    10079 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/session.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2022-08-24 12:14:58.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-24 14:20:20.342877 h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4705 2022-08-24 14:20:20.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2022-08-24 14:20:20.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-24 14:20:20.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-08-24 14:20:20.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-08-24 14:20:20.000000 h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-24 14:20:20.342877 h5-info-pkg-inra-phenome-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      817 2022-08-24 14:20:15.000000 h5-info-pkg-inra-phenome-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:50:04.302847 h5-info-pkg-inra-phenome-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-04-12 12:50:04.302847 h5-info-pkg-inra-phenome-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4129 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:50:04.302847 h5-info-pkg-inra-phenome-1.3.2/h5_info/
+-rw-rw-rw-   0 root         (0) root         (0)    15004 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/camera_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/geo.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/lidar_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/multispectral_camera_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/position.py
+-rw-rw-rw-   0 root         (0) root         (0)    10694 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:50:04.302847 h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-04-12 12:50:04.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-12 12:50:04.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 12:50:04.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 12:50:04.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-12 12:50:04.000000 h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 12:50:04.302847 h5-info-pkg-inra-phenome-1.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-04-12 12:49:58.000000 h5-info-pkg-inra-phenome-1.3.2/setup.py
```

### Comparing `h5-info-pkg-inra-phenome-1.3.1/LICENSE` & `h5-info-pkg-inra-phenome-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/PKG-INFO` & `h5-info-pkg-inra-phenome-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5-info-pkg-inra-phenome
-Version: 1.3.1
+Version: 1.3.2
 Summary: Utility package for extracting, reading and saving metadata from HDF5 Phenomobile V2 and LITERAL acquisition file
 Home-page: https://forgemia.inra.fr/4p/tools/h5info
 Author: Eric David
 Author-email: eric.david@ephesia-consult.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `h5-info-pkg-inra-phenome-1.3.1/README.md` & `h5-info-pkg-inra-phenome-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/__init__.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.geo_filename = os.path.basename(geo_fullname)
         with open(filename, "w") as file:
             file.write(self.to_json())
 
         # Save geolocalisation to file <filename>_geo.csv
         Logger.debug("Saving '" + geo_fullname + "' file")
         with open(geo_fullname, "w+") as file:
-            file.write("date;longitude;latitude;uncertainty;tray_height;heading;course;roll;pitch;sog" + END_LINE_W)
+            file.write("date;longitude;latitude;uncertainty;altitude;uncertainty_altitude;tray_height;heading;course;roll;pitch;sog" + END_LINE_W)
             for geo_item in self.geo:
                 geo_item.write_to(file)
 
     def load_metadata(self, filename):
         """Load a HDF5 Info structure from the given JSON metadata file"""
         Logger.info("Loading '" + filename + "' file")
         with open(filename, "r") as file:
@@ -184,17 +184,24 @@
                 curr_sensor.position.yaw = sensor_attrs['Yaw']
                 curr_sensor.position.z = sensor_attrs['Z']
                 # ST 01032022 : Ajout de la lecture du champ "DataFormatId" qui va renseigner
                 # le format de trame pour le capteur considéré
                 curr_sensor.data_format = sensor_attrs['DataFormatId']
 
                 if curr_sensor.type == TYPE_CAMERA:
-                    curr_sensor.bayer_grid = self.try_get_key_bytes(sensor_path, sensor_attrs, 'BayerGrid')
-                    curr_sensor.focal_length = self.try_get_key(sensor_path, sensor_attrs, 'FocalLength')
-                    curr_sensor.lens_angular_aperture = self.try_get_key(sensor_path, sensor_attrs, 'LensAngularAperture')
+                    if session_gp.get('Vector1/Head1/Positioning').attrs['DataFormatId'] == 12:
+                        curr_sensor.bayer_grid = self.try_get_key_bytes(sensor_path, sensor_attrs, 'PixelFormat')
+                        curr_sensor.focal_length = self.try_get_key(sensor_path, sensor_attrs, 'FocalLength')
+                        curr_sensor.pixel_size = self.try_get_key(sensor_path, sensor_attrs, 'PixelSize')
+                        curr_sensor.width = self.try_get_key(sensor_path, sensor_attrs, 'Width')
+                        curr_sensor.height = self.try_get_key(sensor_path, sensor_attrs, 'Height')
+                    else:
+                        curr_sensor.bayer_grid = self.try_get_key_bytes(sensor_path, sensor_attrs, 'BayerGrid')
+                        curr_sensor.focal_length = self.try_get_key(sensor_path, sensor_attrs, 'FocalLength')
+                        curr_sensor.lens_angular_aperture = self.try_get_key(sensor_path, sensor_attrs, 'LensAngularAperture')
 
                 Logger.debug("Loading '" + sensor_id + "' dataset")
                 data_gp = plot_gp.get("Measurement1/" + sensor_id)
                 curr_sensor.load_data(data_gp, sensor_gp)
 
                 self.sensors.append(curr_sensor)
 
@@ -204,28 +211,47 @@
             Logger.debug("Loading '" + geo_id + "' information")
             geo_gp = plot_gp.get("Measurement1/" + geo_id)
             if geo_gp is None:
                 raise DataError(GROUP_ERROR_MESSAGE, geo_id)
             geo_data = geo_gp.get('Data')
 
             offset = 0
-            while geo_data is not None and offset < len(geo_data):
-                geo_item = Geo()
-                geo_item.date = int.from_bytes(geo_data[offset:offset + 8], "little")
-                geo_item.longitude = struct.unpack('d', geo_data[offset + 8:offset + 16])[0]
-                geo_item.latitude = struct.unpack('d', geo_data[offset + 16:offset + 24])[0]
-                geo_item.uncertainty = struct.unpack('d', geo_data[offset + 24:offset + 32])[0]
-                geo_item.tray_height = struct.unpack('d', geo_data[offset + 32:offset + 40])[0]
-                geo_item.heading = struct.unpack('d', geo_data[offset + 40:offset + 48])[0]
-                geo_item.course = struct.unpack('d', geo_data[offset + 48:offset + 56])[0]
-                geo_item.roll = struct.unpack('d', geo_data[offset + 56:offset + 64])[0]
-                geo_item.pitch = struct.unpack('d', geo_data[offset + 64:offset + 72])[0]
-                geo_item.sog = struct.unpack('d', geo_data[offset + 72:offset + 80])[0]
-                self.geo.append(geo_item)
-                offset += 80
+            if session_gp.get('Vector1/Head1/Positioning').attrs['DataFormatId'] == 12:
+                while geo_data is not None and offset < len(geo_data):
+                    geo_item = Geo()
+                    geo_item.date = int.from_bytes(geo_data[offset:offset + 8], "little")
+                    geo_item.longitude = struct.unpack('d', geo_data[offset + 8:offset + 16])[0]
+                    geo_item.latitude = struct.unpack('d', geo_data[offset + 16:offset + 24])[0]
+                    geo_item.uncertainty = struct.unpack('d', geo_data[offset + 24:offset + 32])[0]
+                    geo_item.altitude = struct.unpack('d', geo_data[offset + 32:offset + 40])[0]
+                    geo_item.uncertainty_altitude = struct.unpack('d', geo_data[offset + 40:offset + 48])[0]
+                    geo_item.tray_height = struct.unpack('d', geo_data[offset + 48:offset + 56])[0]
+                    geo_item.heading = struct.unpack('d', geo_data[offset + 56:offset + 64])[0]
+                    geo_item.course = struct.unpack('d', geo_data[offset + 64:offset + 72])[0]
+                    geo_item.roll = struct.unpack('d', geo_data[offset + 72:offset + 80])[0]
+                    geo_item.pitch = struct.unpack('d', geo_data[offset + 80:offset + 88])[0]
+                    geo_item.sog = struct.unpack('d', geo_data[offset + 88:offset + 96])[0]
+                    self.geo.append(geo_item)
+                    offset += 96
+
+            else:
+                while geo_data is not None and offset < len(geo_data):
+                    geo_item = Geo()
+                    geo_item.date = int.from_bytes(geo_data[offset:offset + 8], "little")
+                    geo_item.longitude = struct.unpack('d', geo_data[offset + 8:offset + 16])[0]
+                    geo_item.latitude = struct.unpack('d', geo_data[offset + 16:offset + 24])[0]
+                    geo_item.uncertainty = struct.unpack('d', geo_data[offset + 24:offset + 32])[0]
+                    geo_item.tray_height = struct.unpack('d', geo_data[offset + 32:offset + 40])[0]
+                    geo_item.heading = struct.unpack('d', geo_data[offset + 40:offset + 48])[0]
+                    geo_item.course = struct.unpack('d', geo_data[offset + 48:offset + 56])[0]
+                    geo_item.roll = struct.unpack('d', geo_data[offset + 56:offset + 64])[0]
+                    geo_item.pitch = struct.unpack('d', geo_data[offset + 64:offset + 72])[0]
+                    geo_item.sog = struct.unpack('d', geo_data[offset + 72:offset + 80])[0]
+                    self.geo.append(geo_item)
+                    offset += 80
 
             # Load Static Transform matrix
             #################################
             transform_id = "StaticTransforms"
             Logger.debug("Loading '" + transform_id + "' information")
             matrix_path = 'Vector1/' + transform_id
             matrix_data = session_gp.get(matrix_path)
@@ -258,15 +284,15 @@
 
         for sensor in self.sensors:
             json_dict["sensors"].append(sensor.to_json())
 
         for key in self.static_transforms:
             json_dict["static_transforms"][key] = self.static_transforms[key].to_json()
 
-        return json.dumps(json_dict)
+        return json.dumps(json_dict, indent=4)
 
     def from_json(self, json_str):
         json_dict = json.loads(json_str)
 
         self.session.from_json(json_dict["session"])
         self.plot.from_json(json_dict["plot"])
         self.vector.from_json(json_dict["vector"])
```

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/camera_image.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/camera_image.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/geo.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/geo.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,67 +4,77 @@
 class Geo:
     """Store HDF5 Geolocalisation attributes in a simplified structure"""
     def __init__(self):
         self.date = 0
         self.longitude = 0.0
         self.latitude = 0.0
         self.uncertainty = 0.0
+        self.altitude = -9999
+        self.uncertainty_altitude = -9999
         self.tray_height = 0.0
         self.heading = 0.0
         self.course = 0.0
         self.roll = 0.0
         self.pitch = 0.0
         self.sog = 0.0
 
     def write_to(self, file):
         file.write(str(self.date) + ";")
         file.write(str(round(self.longitude, 8)) + ";")
         file.write(str(round(self.latitude, 8)) + ";")
         file.write(str(round(self.uncertainty, 6)) + ";")
+        file.write(str(round(self.altitude, 6)) + ";")
+        file.write(str(round(self.uncertainty_altitude, 6)) + ";")
         file.write(str(round(self.tray_height, 6)) + ";")
         file.write(str(round(self.heading, 8)) + ";")
         file.write(str(round(self.course, 8)) + ";")
         file.write(str(round(self.roll, 8)) + ";")
         file.write(str(round(self.pitch, 8)) + ";")
         file.write(str(round(self.sog, 6)) + END_LINE_W)
 
     def read_from_line(self, line):
         values = line.strip().split(';')
 
         self.date = int(values[0])
         self.longitude = float(values[1])
         self.latitude = float(values[2])
         self.uncertainty = float(values[3])
-        self.tray_height = float(values[4])
-        self.heading = float(values[5])
-        self.course = float(values[6])
-        self.roll = float(values[7])
-        self.pitch = float(values[8])
-        self.sog = float(values[9])
+        self.altitude = float(values[4])
+        self.uncertainty_altitude = float(values[5])
+        self.tray_height = float(values[6])
+        self.heading = float(values[7])
+        self.course = float(values[8])
+        self.roll = float(values[9])
+        self.pitch = float(values[10])
+        self.sog = float(values[11])
 
     @staticmethod
     def to_dict_array(geo_list):
         """Converts a list of Geo objects to a dictionary array with Geo attributes as keys"""
         res = {
             'date': [],
             'longitude': [],
             'latitude': [],
             'uncertainty': [],
+            'altitude': [],
+            'uncertainty_altitude': [],
             'tray_height': [],
             'heading': [],
             'course': [],
             'roll': [],
             'pitch': [],
             'sog': [],
         }
         for item in geo_list:
             res['date'].append(item.date)
             res['longitude'].append(item.longitude)
             res['latitude'].append(item.latitude)
             res['uncertainty'].append(item.uncertainty)
+            res['altitude'].append(item.altitude)
+            res['uncertainty_altitude'].append(item.uncertainty_altitude)
             res['tray_height'].append(item.tray_height)
             res['heading'].append(item.heading)
             res['course'].append(item.course)
             res['roll'].append(item.roll)
             res['pitch'].append(item.pitch)
             res['sog'].append(item.sog)
```

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/lidar_image.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/lidar_image.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/logger.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/logger.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/multispectral_camera_image.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/multispectral_camera_image.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/plot.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/plot.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/position.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/position.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/sensor.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         self.id = 0
         # ST 01032022 : Ajout de la lecture du champ "DataFormatId" qui va renseigner 
         # le format de trame pour le capteur considéré
         self.data_format = 0
         self.bayer_grid = ""
         self.focal_length = 0.0
         self.lens_angular_aperture = 0.0
+        self.pixel_size = 0.0
+        self.width = 0.0
+        self.height = 0.0
 
     def to_json(self):
         json_dict = {
             "type": self.type,
             "id": str(self.id),
             "description": self.description,
             "manufacturer": self.manufacturer,
@@ -49,15 +52,21 @@
             "position": self.position.to_json(),
             "images": []
         }
 
         if self.type == TYPE_CAMERA:
             json_dict["bayer_grid"] = self.bayer_grid
             json_dict["focal_length"] = self.focal_length
-            json_dict["lens_angular_aperture"] = self.lens_angular_aperture
+            if self.lens_angular_aperture == "":
+                json_dict["lens_angular_aperture"] = str(self.lens_angular_aperture)
+            else:
+                json_dict["lens_angular_aperture"] = float(self.lens_angular_aperture)
+            json_dict["pixel_size"] = float(self.pixel_size)
+            json_dict["width"] = float(self.width)
+            json_dict["height"] = float(self.height)
 
         for image in self.images:
             json_dict["images"].append(image.to_json())
 
         return json_dict
 
     def from_json(self, json_dict):
@@ -72,14 +81,18 @@
         self.data_format = int(json_dict["format"])
         self.position.from_json(json_dict["position"])
 
         if self.type == TYPE_CAMERA:
             self.bayer_grid = json_dict["bayer_grid"]
             self.focal_length = json_dict["focal_length"]
             self.lens_angular_aperture = json_dict["lens_angular_aperture"]
+            if self.lens_angular_aperture == 0.0:
+                self.pixel_size = json_dict["pixel_size"]
+                self.width = json_dict["width"]
+                self.height = json_dict["height"]
 
         for image_dict in json_dict["images"]:
             if self.type == TYPE_CAMERA:
                 image = CameraImage()
                 image.from_json(image_dict)
                 self.images.append(image)
             elif self.type == TYPE_LIDAR:
```

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/session.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/session.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info/vector.py` & `h5-info-pkg-inra-phenome-1.3.2/h5_info/vector.py`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/PKG-INFO` & `h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5-info-pkg-inra-phenome
-Version: 1.3.1
+Version: 1.3.2
 Summary: Utility package for extracting, reading and saving metadata from HDF5 Phenomobile V2 and LITERAL acquisition file
 Home-page: https://forgemia.inra.fr/4p/tools/h5info
 Author: Eric David
 Author-email: eric.david@ephesia-consult.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `h5-info-pkg-inra-phenome-1.3.1/h5_info_pkg_inra_phenome.egg-info/SOURCES.txt` & `h5-info-pkg-inra-phenome-1.3.2/h5_info_pkg_inra_phenome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h5-info-pkg-inra-phenome-1.3.1/setup.py` & `h5-info-pkg-inra-phenome-1.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="h5-info-pkg-inra-phenome",
-    version="1.3.1",
+    version="1.3.2",
     author="Eric David",
     author_email="eric.david@ephesia-consult.com",
     description="Utility package for extracting, reading and saving metadata from HDF5 Phenomobile V2 and LITERAL acquisition file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://forgemia.inra.fr/4p/tools/h5info",
     packages=setuptools.find_packages(),
```

