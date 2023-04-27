# Comparing `tmp/kmlb-0.0.88.tar.gz` & `tmp/kmlb-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmlb-0.0.88.tar", last modified: Wed Apr 26 02:31:30 2023, max compression
+gzip compressed data, was "kmlb-0.0.90.tar", last modified: Thu Apr 27 00:28:53 2023, max compression
```

## Comparing `kmlb-0.0.88.tar` & `kmlb-0.0.90.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 02:31:30.954977 kmlb-0.0.88/
--rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.88/LICENSE.md
--rw-rw-rw-   0        0        0    38527 2023-04-26 02:31:30.954977 kmlb-0.0.88/PKG-INFO
--rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.88/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 02:31:30.920969 kmlb-0.0.88/kmlb/
--rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.88/kmlb/__init__.py
--rw-rw-rw-   0        0        0    37252 2023-04-26 00:13:57.000000 kmlb-0.0.88/kmlb/base.py
--rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.88/kmlb/gis_basics.py
--rw-rw-rw-   0        0        0     6919 2023-04-26 02:24:30.000000 kmlb-0.0.88/kmlb/shapes.py
-drwxrwxrwx   0        0        0        0 2023-04-26 02:31:30.953970 kmlb-0.0.88/kmlb.egg-info/
--rw-rw-rw-   0        0        0    38527 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 02:31:30.954977 kmlb-0.0.88/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-26 02:27:06.000000 kmlb-0.0.88/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 00:28:53.466524 kmlb-0.0.90/
+-rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.90/LICENSE.md
+-rw-rw-rw-   0        0        0    38527 2023-04-27 00:28:53.466524 kmlb-0.0.90/PKG-INFO
+-rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.90/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 00:28:53.453124 kmlb-0.0.90/kmlb/
+-rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.90/kmlb/__init__.py
+-rw-rw-rw-   0        0        0    42701 2023-04-27 00:25:38.000000 kmlb-0.0.90/kmlb/base.py
+-rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.90/kmlb/gis_basics.py
+-rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.90/kmlb/shapes.py
+drwxrwxrwx   0        0        0        0 2023-04-27 00:28:53.465241 kmlb-0.0.90/kmlb.egg-info/
+-rw-rw-rw-   0        0        0    38527 2023-04-27 00:28:53.000000 kmlb-0.0.90/kmlb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-27 00:28:53.000000 kmlb-0.0.90/kmlb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 00:28:53.000000 kmlb-0.0.90/kmlb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 00:28:53.000000 kmlb-0.0.90/kmlb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 00:28:53.466524 kmlb-0.0.90/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-27 00:28:11.000000 kmlb-0.0.90/setup.py
```

### Comparing `kmlb-0.0.88/LICENSE.md` & `kmlb-0.0.90/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.88/PKG-INFO` & `kmlb-0.0.90/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.88
+Version: 0.0.90
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.88/README.md` & `kmlb-0.0.90/README.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.88/kmlb/base.py` & `kmlb-0.0.90/kmlb/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Functions for creating KML files.
 """
 
 import xml.etree.ElementTree as ET
 from pathlib import Path
+import zipfile
 
 
 def altitude_modes(altitude_mode='CTG'):
     """
     Expands an abbreviated altitude mode to its full length name.
 
     INPUT:
@@ -780,64 +781,83 @@
     outline = ET.SubElement(style, "LineStyle")
     ET.SubElement(outline, "color").text = kml_color(*outline_color)
     ET.SubElement(outline, "width").text = str(outline_width)
 
     return style
 
 
-def folder(name, loose_items, description='', collapsed=True, hidden=True, camera=None):
+def folder(name, loose_items, description='', folder_type=1, collapsed=True, hidden=False, camera=None):
     """
     Creates a KML a folder and fills it with specified KML elements.
 
     OVERVIEW:
         Creates a folder to organize loose KML elements sych as points, lines, polygon or even other folders.
 
     INPUTS:
         name (String):
             The name of the folder to be created.
         loose_items (List):
             A list of loose items to include in the new folder.
         description (String) [Optional]:
             A small body of descriptive text for the folder.
+        folder_type (Integer):
+            Can be any of the following values:
+            1 = check, 2 = radioFolder, 3 = checkOffOnly, 4 = checkHideChildren
         collapsed (Bool) [Optional]:
             True = Folder is collapsed.
             False = Folder is open/expanded.
         hidden (Bool) [Optional]:
             True = Folder is hidden.
             False = Folder is visible.
-                Note: A folder's visibility is ultimately determined by the visibility of the contents within. The
-                default is to have folders set to hidden so that empty folders are not visible. If an item gets added
-                to a folder and that item is set to be visible, the containing folder will become visible as well -
-                even if the folder set to hidden. (Default = `True`)
+                Note: A folder's visibility is ultimately determined by the visibility of the contents within.
+                If an item gets added to a folder and that item is set to be visible, the containing folder will become
+                visible as well - even if the folder set to hidden. (Default = False)
         camera (Element) [Optional]:
             A KML 'LookAt' element that defines the default camera angle to the line.
 
     OUTPUT:
         new_folder (Object):
             An XML element representing a KML folder.
 
     Parameters
     ----------
     name : str
     loose_items : list
     description : str, optional
+    folder_type : int, optional
     collapsed : bool, optional
     hidden : bool, optional
     camera : element, optional
 
     Returns
     -------
     new_folder : object
 
     """
 
     new_folder = ET.Element("Folder")
     ET.SubElement(new_folder, "name").text = str(name)
     ET.SubElement(new_folder, "description").text = str(description)
 
+    f_style = ET.SubElement(new_folder, "Style")
+    list_style = ET.SubElement(f_style, "ListStyle")
+
+    if folder_type == 1:
+        folder_type = 'check'
+    elif folder_type == 2:
+        folder_type = 'radioFolder'
+    elif folder_type == 3:
+        folder_type = 'checkOffOnly'
+    elif folder_type == 4:
+        folder_type = 'checkHideChildren'
+    else:
+        folder_type = 'check'
+
+    ET.SubElement(list_style, "listItemType").text = folder_type
+
     if collapsed is False:
         collapsed = 1
     else:
         collapsed = 0
 
     ET.SubElement(new_folder, "open").text = str(collapsed)
 
@@ -867,16 +887,16 @@
 
     INPUTS:
         name (String):
             The name of the KML
         features (List):
             A list of the defined point, line, polygon, and/or folder objects to include in the KML
         path (String) [Optional]:
-            The path to the folder where the KML file will be written to. The KML's file name is defined in the path.
-            Necessary folders will be created of they do not exist.
+            The path where the KML file will be written to. The KML's file name is defined in the path.
+            Necessary folders will be created if they do not exist.
             Note: The file path should end '.kml'
         description (String) [Optional]:
                 A small body of descriptive text for the kml.
         styles (List) [Optional]:
             A list of the defined style object to include in the KML
         collapsed (Bool) [Optional]:
                 True = Root folder is collapsed.
@@ -938,34 +958,34 @@
             f.write(kml_string)
     else:
         pass
 
     return kml_string
 
 
-def networklink_kml(name, link_path, write_path=None, description='', refresh_interval=300, collapsed=True):
+def networklink_kml(name, link_path, write_path=None, description='', refresh_interval=None, collapsed=True):
     """
        Creates a KML string.
 
        OVERVIEW:
            Creates an XML string that defines the KML document with a network link. This string can be written to text file with a '.kml' extension.
 
        INPUTS:
            name (String):
                The name of the KML
            link_path (String):
                url to hosted kml
            write_path (String) [Optional]:
-               The path to the folder where the KML file will be written to. The KML's file name is defined in the path.
-               Necessary folders will be created of they do not exist.
+               The path where the KML file will be written to. The KML's file name is defined in the path.
+               Necessary folders will be created if they do not exist.
                Note: The file path should end '.kml'
            description (String) [Optional]:
                    A small body of descriptive text for the kml.
            refresh_interval (Int) [Optional]:
-               Number of seconds between file refreshes.
+               Number of seconds between file refreshes. (Default = None)
            collapsed (Bool) [Optional]:
                    True = Root folder is collapsed.
                    False = Root folder is open/expanded.
 
        OUTPUT:
            kml_string (String):
             xml string of kml file
@@ -994,16 +1014,20 @@
 
     style = ET.SubElement(ntwrk, "Style")
     list_style = ET.SubElement(style, "ListStyle")
     ET.SubElement(list_style, "listItemType").text = 'check'
 
     link = ET.SubElement(ntwrk, "Link")
     ET.SubElement(link, "href").text = link_path
-    ET.SubElement(link, "refreshMode").text = 'onInterval'
-    ET.SubElement(link, "refreshInterval").text = str(refresh_interval)
+
+    if refresh_interval is not None:
+        ET.SubElement(link, "refreshMode").text = 'onInterval'
+        ET.SubElement(link, "refreshInterval").text = str(refresh_interval)
+    else:
+        pass
 
     kml_string = '<?xml version="1.0" encoding="UTF-8"?>'
     kml_string += ET.tostring(kml_doc, encoding='unicode', method='xml')
 
     if write_path is not None:
         filepath = Path(write_path)
         filepath.parent.mkdir(parents=True, exist_ok=True)
@@ -1012,15 +1036,97 @@
             f.write(kml_string)
     else:
         pass
 
     return kml_string
 
 
-def ground_overlay(name, img_path, bounds, description='', opacity=100, refresh_interval=300, altitude=0, altitude_mode='CTG', hidden=False, camera=None):
+def network_link(name, link_path, description='', refresh_interval=None, folder_type=1, collapsed=True, camera=None):
+    """
+       Creates a NetworkLink element.
+
+       OVERVIEW:
+           Creates an XML element that defines a network link. This string element can be added to kml and folders.
+
+       INPUTS:
+           name (String):
+               The name of the Network Link element
+           link_path (String):
+                Path to file
+           description (String) [Optional]:
+                A small body of descriptive text for the NetworkLink element.
+           refresh_interval (Int) [Optional]:
+                Number of seconds between file refreshes. (Default = None)
+            folder_type (Integer):
+                Can be any of the following values:
+                1 = check, 2 = radioFolder, 3 = checkOffOnly, 4 = checkHideChildren
+           collapsed (Bool) [Optional]:
+                True = Root folder is collapsed.
+                False = Root folder is open/expanded.
+            camera (Element) [Optional]:
+                A KML 'LookAt' element that defines the default camera angle to the kml.
+
+       OUTPUT:
+           network_link (String):
+                xml element of network link
+
+       Parameters
+       ----------
+       name : str
+       link_path : str
+       description : str, optional
+       refresh_interval : int, optional
+       folder_type : int, optional
+       collapsed : bool, optional
+       camera : element, optional
+
+       Returns
+       -------
+       network_link : element
+
+       """
+
+    network_link = ET.Element("NetworkLink")
+    ET.SubElement(network_link, "name").text = str(name)
+    ET.SubElement(network_link, "description").text = str(description)
+    collapsed = 0 if collapsed is True else 1
+    ET.SubElement(network_link, "open").text = str(collapsed)
+
+    style = ET.SubElement(network_link, "Style")
+    list_style = ET.SubElement(style, "ListStyle")
+    if folder_type == 1:
+        folder_type = 'check'
+    elif folder_type == 2:
+        folder_type = 'radioFolder'
+    elif folder_type == 3:
+        folder_type = 'checkOffOnly'
+    elif folder_type == 4:
+        folder_type = 'checkHideChildren'
+    else:
+        folder_type = 'check'
+
+    ET.SubElement(list_style, "listItemType").text = folder_type
+
+    link = ET.SubElement(network_link, "Link")
+    ET.SubElement(link, "href").text = link_path
+
+    if refresh_interval is not None:
+        ET.SubElement(link, "refreshMode").text = 'onInterval'
+        ET.SubElement(link, "refreshInterval").text = str(refresh_interval)
+    else:
+        pass
+
+    # Network Link Camera Angle
+    if camera is not None:
+        network_link.append(camera)
+
+    return network_link
+
+
+def ground_overlay(name, img_path, bounds, description='', opacity=100, refresh_interval=None, altitude=0, altitude_mode='CTG', hidden=False, camera=None):
     """
     INPUTS:
     name (String):
         The name to be given to the overlay.
     img_path (String):
         Path to the image to be used
     bounds (List of four floats):
@@ -1064,16 +1170,19 @@
     ET.SubElement(overlay, "description").text = str(description)
     ET.SubElement(overlay, "color").text = kml_color('#FFFFFF', opacity)
     ET.SubElement(overlay, "altitude").text = str(altitude)
     ET.SubElement(overlay, "altitudeMode").text = altitude_modes(altitude_mode)
 
     icon = ET.SubElement(overlay, "Icon")
     ET.SubElement(icon, "href").text = img_path
-    ET.SubElement(icon, "refreshMode").text = "onInterval"
-    ET.SubElement(icon, "refreshInterval").text = str(refresh_interval)
+    if refresh_interval is not None:
+        ET.SubElement(icon, "refreshMode").text = "onInterval"
+        ET.SubElement(icon, "refreshInterval").text = str(refresh_interval)
+    else:
+        pass
 
     llbox = ET.SubElement(overlay, "LatLonBox")
     ET.SubElement(llbox, "north").text = str(bounds[0])
     ET.SubElement(llbox, "south").text = str(bounds[1])
     ET.SubElement(llbox, "east").text = str(bounds[2])
     ET.SubElement(llbox, "west").text = str(bounds[3])
 
@@ -1085,7 +1194,68 @@
     ET.SubElement(overlay, 'visibility').text = str(visibility)
 
     # Image Default Camera Angle
     if camera is not None:
         overlay.append(camera)
 
     return overlay
+
+
+def kmz(kmz_name, kmls, path, files_as_bytes=None, **kwargs):
+    """
+    Creates a KMZ file.
+
+       OVERVIEW:
+           Creates a KMZ file that can contain KMLs and files such as images.
+
+       INPUTS:
+            kmz_name (String):
+                The name of the KMZ
+            kmls (Tuples):
+                 (Layer Name, KML as XML str, folder_type)
+            path (String) [Optional]:
+                The path where the kmz file will be written to. The KMz's file name is defined within the path.
+                Necessary folders will be created if they do not exist.
+                Note: The file path should end '.kmz'
+            files_as_bytes (Tuple) [Optional]:
+                 (desitnation path of file within KMZ root, data as bytes)
+            kwargs
+                Any argument accepted by the kml function
+
+       OUTPUT:
+           kml_string (String):
+            xml string of kml file
+
+       Parameters
+       ----------
+       kmz_name: str
+       kmls: tuple
+       path: str
+       files_as_bytes: tuple
+       kwargs
+
+       Returns
+       -------
+       network_link : element
+
+    """
+
+    network_link_elements = list()
+
+    with zipfile.ZipFile(path, 'w') as zf:
+        for count, doc in enumerate(kmls):
+            name = doc[0]
+            data = doc[1].encode()
+            folder_type = doc[2]
+            doc_path = f"kmls/doc_{count}.kml"
+            zf.writestr(doc_path, data)
+            nl = network_link(name, doc_path, folder_type=folder_type)
+            network_link_elements.append(nl)
+
+        if files_as_bytes is not None:
+            for fb in files_as_bytes:
+                file_path = fb[0]
+                data = fb[1]
+                zf.writestr(file_path, data)
+
+        index_k = kml(kmz_name, network_link_elements, **kwargs).encode()
+        zf.writestr("doc.kml", index_k)
```

### Comparing `kmlb-0.0.88/kmlb/gis_basics.py` & `kmlb-0.0.90/kmlb/gis_basics.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.88/kmlb/shapes.py` & `kmlb-0.0.90/kmlb/shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     # Create polygon
     circle_poly = kmlb.base.polygon([coords], name, headers, attributes, **kwargs)
 
     return circle_poly
 
 
-def graduated_rings(center, start, increment, count, folder_name='Rings', point_style_to_use='RingStyle', label_angle=90, **kwargs):
+def graduated_rings(center, start, increment, count, folder_name='Rings', point_style_to_use='g_ring_pts', label_angle=135, **kwargs):
     """
     Creates a folder of graduated rings and labels.
 
     OVERVIEW:
         Creates a folder of graduated rings and labels that can be included in a KML document.
         The rings are polyons and the labels are labeled points.
 
@@ -158,15 +158,15 @@
         count (Integer):
             The number of rings to generate
         folder_name (String) [Optional]:
             The name of the containing folder.
             (Default = Rings)
         point_style_to_use (String) [Optional]:
             The name of the point style to be used.
-            (Default = 'RingStyle')
+            (Default = 'g_ring_pts')
         label_angle (Float) [Optional]:
             The angle in degrees from north at which to label the rings.
             (Default = 90)
         **kwargs:
             Any keyword argument accepted by the kmlb.base.polygon function. Used to define the rings.
 
     OUTPUT:
```

### Comparing `kmlb-0.0.88/kmlb.egg-info/PKG-INFO` & `kmlb-0.0.90/kmlb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.88
+Version: 0.0.90
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.88/setup.py` & `kmlb-0.0.90/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kmlb",
-    version="0.0.88",
+    version="0.0.90",
     author="HFM3",
     description="A Straightforward Google Earth KML Builder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HFM3/kmlb",
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "images", "art"]),
     classifiers=[
```

