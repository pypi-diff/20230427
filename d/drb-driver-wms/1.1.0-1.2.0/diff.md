# Comparing `tmp/drb-driver-wms-1.1.0.tar.gz` & `tmp/drb-driver-wms-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-wms-1.1.0.tar", last modified: Wed Dec 21 15:38:20 2022, max compression
+gzip compressed data, was "drb-driver-wms-1.2.0.tar", last modified: Thu Apr 27 09:50:10 2023, max compression
```

## Comparing `drb-driver-wms-1.1.0.tar` & `drb-driver-wms-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.449986 drb-driver-wms-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4204 2022-12-21 15:38:20.449986 drb-driver-wms-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3745 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.429985 drb-driver-wms-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.429985 drb-driver-wms-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.449986 drb-driver-wms-1.1.0/drb/drivers/wms/
--rw-rw-rw-   0 root         (0) root         (0)      439 2022-12-21 15:02:35.000000 drb-driver-wms-1.1.0/drb/drivers/wms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-21 15:38:20.449986 drb-driver-wms-1.1.0/drb/drivers/wms/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2022-12-21 15:02:35.000000 drb-driver-wms-1.1.0/drb/drivers/wms/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5087 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/drb/drivers/wms/wms_nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.441986 drb-driver-wms-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/drb/exceptions/wms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.429985 drb-driver-wms-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.441986 drb-driver-wms-1.1.0/drb/topics/wms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/drb/topics/wms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/drb/topics/wms/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:20.449986 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4204 2022-12-21 15:38:20.000000 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2022-12-21 15:38:20.000000 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 15:38:20.000000 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2022-12-21 15:38:20.000000 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-21 15:38:20.000000 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-21 15:38:20.000000 drb-driver-wms-1.1.0/drb_driver_wms.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-12-21 15:38:20.449986 drb-driver-wms-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-12-21 14:30:05.000000 drb-driver-wms-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-06-22 06:39:39.000000 drb-driver-wms-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.837634 drb-driver-wms-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:12:10.000000 drb-driver-wms-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-21 14:30:05.000000 drb-driver-wms-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4272 2023-04-27 09:50:10.837634 drb-driver-wms-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-04-26 15:39:30.000000 drb-driver-wms-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.813634 drb-driver-wms-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.813634 drb-driver-wms-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.837634 drb-driver-wms-1.2.0/drb/drivers/wms/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2022-12-21 15:02:35.000000 drb-driver-wms-1.2.0/drb/drivers/wms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-27 09:50:10.837634 drb-driver-wms-1.2.0/drb/drivers/wms/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2022-12-21 15:02:35.000000 drb-driver-wms-1.2.0/drb/drivers/wms/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2023-04-26 15:43:00.000000 drb-driver-wms-1.2.0/drb/drivers/wms/wms_nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.829634 drb-driver-wms-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-21 14:30:05.000000 drb-driver-wms-1.2.0/drb/exceptions/wms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.813634 drb-driver-wms-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.829634 drb-driver-wms-1.2.0/drb/topics/wms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-21 14:30:05.000000 drb-driver-wms-1.2.0/drb/topics/wms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-27 09:49:10.000000 drb-driver-wms-1.2.0/drb/topics/wms/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.833634 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4272 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      616 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-27 09:50:10.000000 drb-driver-wms-1.2.0/drb_driver_wms.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-27 09:22:32.000000 drb-driver-wms-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-26 15:39:30.000000 drb-driver-wms-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-27 09:50:10.837634 drb-driver-wms-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 15:39:30.000000 drb-driver-wms-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:50:10.833634 drb-driver-wms-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7643 2022-12-21 14:30:05.000000 drb-driver-wms-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2023-04-26 15:40:22.000000 drb-driver-wms-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    13972 2023-04-26 15:39:30.000000 drb-driver-wms-1.2.0/tests/test_wms.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-06-22 06:39:39.000000 drb-driver-wms-1.2.0/versioneer.py
```

### Comparing `drb-driver-wms-1.1.0/PKG-INFO` & `drb-driver-wms-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wms
-Version: 1.1.0
-Summary: DRB WMS OGC Service Driver
-Home-page: https://gitlab.com/drb-python/impl/wms
+Version: 1.2.0
+Summary: DRB WMS OGC Service driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wms
+Project-URL: Source, https://gitlab.com/drb-python/impl/wms
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WMS Driver
 
 The web map service driver extends abstracts WxS driver with the getMap feature.
 
 # Nodes
 
@@ -83,15 +84,15 @@
 list_cap = service_wms.children
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wms.children:
+for child in service_wms:
     print(child)
     print(child.name)
 
 #=> <drb.drivers.wXs.wXs_node.WXSNodeOperation object at 0x7fc2cb0aeaf0>
 #=> GetCapabilities
 #=> <drb.drivers.wXs.wXs_node.WXSNodeOperation object at 0x7fc2cb0ae520>
 #=> GetMap
@@ -104,23 +105,21 @@
 
 
 get_map = service_wms['GetMap']
 
 print('----------------------------------------')
 print('GetMap : Format')
 
-print(get_map.get_attribute('Format'))
+print(get_map @ 'Format')
 #=> ['image/png', 'application/atom+xml', 'application/json;type=geojson', 'application/json;type=topojson', 'application/json;type=utfgrid', 'application/pdf', 'application/rss+xml', 'application/vnd.google-earth.kml+xml', 'application/vnd.google-earth.kml+xml;mode=networklink', 'application/vnd.google-earth.kmz', 'application/vnd.mapbox-vector-tile', 'image/geotiff', 'image/geotiff8', 'image/gif', 'image/jpeg', 'image/png; mode=8bit', 'image/svg+xml', 'image/tiff', 'image/tiff8', 'image/vnd.jpeg-png', 'image/vnd.jpeg-png8', 'text/html; subtype=openlayers', 'text/html; subtype=openlayers2', 'text/html; subtype=openlayers3']
 
 dict_request = {'layers': 'mgrs_region', 'format': 'image/png', 'height': 256, 'width': 256, 'crs': 'EPSG:3857', 'bbox': '7514065.628545968,7514065.628545967,10018754.171394622,10018754.171394628'}
 
 
 get_map = service_wms['GetMap'][dict_request]
 
 print('----------------------------------------')
 print('GetMap : with parameter return image')
 print(get_map)
 #=>  <drb.drivers.image.image_node_factory.DrbImageBaseNode object at 0x7fc2cb23efa0>
 
 ```
-
-
```

### Comparing `drb-driver-wms-1.1.0/README.md` & `drb-driver-wms-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 list_cap = service_wms.children
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wms.children:
+for child in service_wms:
     print(child)
     print(child.name)
 
 #=> <drb.drivers.wXs.wXs_node.WXSNodeOperation object at 0x7fc2cb0aeaf0>
 #=> GetCapabilities
 #=> <drb.drivers.wXs.wXs_node.WXSNodeOperation object at 0x7fc2cb0ae520>
 #=> GetMap
@@ -89,15 +89,15 @@
 
 
 get_map = service_wms['GetMap']
 
 print('----------------------------------------')
 print('GetMap : Format')
 
-print(get_map.get_attribute('Format'))
+print(get_map @ 'Format')
 #=> ['image/png', 'application/atom+xml', 'application/json;type=geojson', 'application/json;type=topojson', 'application/json;type=utfgrid', 'application/pdf', 'application/rss+xml', 'application/vnd.google-earth.kml+xml', 'application/vnd.google-earth.kml+xml;mode=networklink', 'application/vnd.google-earth.kmz', 'application/vnd.mapbox-vector-tile', 'image/geotiff', 'image/geotiff8', 'image/gif', 'image/jpeg', 'image/png; mode=8bit', 'image/svg+xml', 'image/tiff', 'image/tiff8', 'image/vnd.jpeg-png', 'image/vnd.jpeg-png8', 'text/html; subtype=openlayers', 'text/html; subtype=openlayers2', 'text/html; subtype=openlayers3']
 
 dict_request = {'layers': 'mgrs_region', 'format': 'image/png', 'height': 256, 'width': 256, 'crs': 'EPSG:3857', 'bbox': '7514065.628545968,7514065.628545967,10018754.171394622,10018754.171394628'}
 
 
 get_map = service_wms['GetMap'][dict_request]
```

### Comparing `drb-driver-wms-1.1.0/drb/drivers/wms/factory.py` & `drb-driver-wms-1.2.0/drb/drivers/wms/factory.py`

 * *Files identical despite different names*

### Comparing `drb-driver-wms-1.1.0/drb/drivers/wms/wms_nodes.py` & `drb-driver-wms-1.2.0/drb/drivers/wms/wms_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from __future__ import annotations
 from drb.core.predicate import Predicate
 
 from requests.auth import AuthBase
-from typing import Optional
 
 from drb.drivers.wxs import WXSServiceNode, WXSNodeOperation
 
 
 class WmsServiceNode(WXSServiceNode):
     def __init__(self, url: str, auth: AuthBase = None, **kwargs):
         if kwargs is not None and len(kwargs) > 0:
             super(WmsServiceNode, self).__init__(url, auth=auth, **kwargs)
         else:
             super(WmsServiceNode, self).__init__(url, auth)
         self._service_url = url.replace("+wms", "") if "+wms" in url else url
+        self.namespace_uri = "WMS"
+        self.name = self._service_url
 
     @property
     def type_service(self):
         return "WMS"
 
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return "WMS"
-
-    @property
-    def name(self) -> str:
-        return self._service_url
+    def manage_predefined_operations_metadata(self):
+        return None
 
     def read_capabilities(self, xmlnode_tree):
         super().read_capabilities(xmlnode_tree)
         xmlnode = xmlnode_tree["Capability"]
 
         for child in xmlnode:
             if child.name == "Request":
```

### Comparing `drb-driver-wms-1.1.0/drb_driver_wms.egg-info/PKG-INFO` & `drb-driver-wms-1.2.0/drb_driver_wms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wms
-Version: 1.1.0
-Summary: DRB WMS OGC Service Driver
-Home-page: https://gitlab.com/drb-python/impl/wms
+Version: 1.2.0
+Summary: DRB WMS OGC Service driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wms
+Project-URL: Source, https://gitlab.com/drb-python/impl/wms
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WMS Driver
 
 The web map service driver extends abstracts WxS driver with the getMap feature.
 
 # Nodes
 
@@ -83,15 +84,15 @@
 list_cap = service_wms.children
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wms.children:
+for child in service_wms:
     print(child)
     print(child.name)
 
 #=> <drb.drivers.wXs.wXs_node.WXSNodeOperation object at 0x7fc2cb0aeaf0>
 #=> GetCapabilities
 #=> <drb.drivers.wXs.wXs_node.WXSNodeOperation object at 0x7fc2cb0ae520>
 #=> GetMap
@@ -104,23 +105,21 @@
 
 
 get_map = service_wms['GetMap']
 
 print('----------------------------------------')
 print('GetMap : Format')
 
-print(get_map.get_attribute('Format'))
+print(get_map @ 'Format')
 #=> ['image/png', 'application/atom+xml', 'application/json;type=geojson', 'application/json;type=topojson', 'application/json;type=utfgrid', 'application/pdf', 'application/rss+xml', 'application/vnd.google-earth.kml+xml', 'application/vnd.google-earth.kml+xml;mode=networklink', 'application/vnd.google-earth.kmz', 'application/vnd.mapbox-vector-tile', 'image/geotiff', 'image/geotiff8', 'image/gif', 'image/jpeg', 'image/png; mode=8bit', 'image/svg+xml', 'image/tiff', 'image/tiff8', 'image/vnd.jpeg-png', 'image/vnd.jpeg-png8', 'text/html; subtype=openlayers', 'text/html; subtype=openlayers2', 'text/html; subtype=openlayers3']
 
 dict_request = {'layers': 'mgrs_region', 'format': 'image/png', 'height': 256, 'width': 256, 'crs': 'EPSG:3857', 'bbox': '7514065.628545968,7514065.628545967,10018754.171394622,10018754.171394628'}
 
 
 get_map = service_wms['GetMap'][dict_request]
 
 print('----------------------------------------')
 print('GetMap : with parameter return image')
 print(get_map)
 #=>  <drb.drivers.image.image_node_factory.DrbImageBaseNode object at 0x7fc2cb23efa0>
 
 ```
-
-
```

### Comparing `drb-driver-wms-1.1.0/versioneer.py` & `drb-driver-wms-1.2.0/versioneer.py`

 * *Files identical despite different names*

