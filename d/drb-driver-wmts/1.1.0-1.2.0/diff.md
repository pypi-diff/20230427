# Comparing `tmp/drb-driver-wmts-1.1.0.tar.gz` & `tmp/drb-driver-wmts-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-wmts-1.1.0.tar", last modified: Wed Dec 21 15:38:31 2022, max compression
+gzip compressed data, was "drb-driver-wmts-1.2.0.tar", last modified: Thu Apr 27 09:53:56 2023, max compression
```

## Comparing `drb-driver-wmts-1.1.0.tar` & `drb-driver-wmts-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4006 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3544 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.054181 drb-driver-wmts-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.054181 drb-driver-wmts-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/drb/drivers/wmts/
--rw-rw-rw-   0 root         (0) root         (0)      456 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/drb/drivers/wmts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/drb/drivers/wmts/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/drb/drivers/wmts/wmts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/drb/exceptions/wmts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.054181 drb-driver-wmts-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/drb/topics/wmts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/drb/topics/wmts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/drb/topics/wmts/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4006 2022-12-21 15:38:31.000000 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-12-21 15:38:31.000000 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 15:38:31.000000 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2022-12-21 15:38:31.000000 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-21 15:38:31.000000 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-21 15:38:31.000000 drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-21 15:38:31.058181 drb-driver-wmts-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-21 14:44:57.000000 drb-driver-wmts-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.505279 drb-driver-wmts-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:23:20.000000 drb-driver-wmts-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-21 14:44:57.000000 drb-driver-wmts-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-04-27 09:53:56.505279 drb-driver-wmts-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3535 2023-04-26 16:20:03.000000 drb-driver-wmts-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.465278 drb-driver-wmts-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.465278 drb-driver-wmts-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.509279 drb-driver-wmts-1.2.0/drb/drivers/wmts/
+-rw-rw-rw-   0 root         (0) root         (0)      456 2022-12-21 14:44:57.000000 drb-driver-wmts-1.2.0/drb/drivers/wmts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-27 09:53:56.509279 drb-driver-wmts-1.2.0/drb/drivers/wmts/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5363 2023-04-26 16:20:03.000000 drb-driver-wmts-1.2.0/drb/drivers/wmts/wmts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.497279 drb-driver-wmts-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2022-12-21 14:44:57.000000 drb-driver-wmts-1.2.0/drb/exceptions/wmts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.465278 drb-driver-wmts-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.501279 drb-driver-wmts-1.2.0/drb/topics/wmts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-21 14:44:57.000000 drb-driver-wmts-1.2.0/drb/topics/wmts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-27 09:53:12.000000 drb-driver-wmts-1.2.0/drb/topics/wmts/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.501279 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-27 09:53:56.000000 drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-27 09:23:07.000000 drb-driver-wmts-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-26 16:20:03.000000 drb-driver-wmts-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-27 09:53:56.509279 drb-driver-wmts-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 16:20:03.000000 drb-driver-wmts-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:53:56.505279 drb-driver-wmts-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7629 2022-12-21 14:44:57.000000 drb-driver-wmts-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-04-26 16:20:03.000000 drb-driver-wmts-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    83764 2023-04-26 16:20:03.000000 drb-driver-wmts-1.2.0/tests/test_wmts.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-21 14:44:57.000000 drb-driver-wmts-1.2.0/versioneer.py
```

### Comparing `drb-driver-wmts-1.1.0/PKG-INFO` & `drb-driver-wmts-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: drb-driver-wmts
-Version: 1.1.0
-Summary: DRB wmts OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/wmts
-Author: GAEL Systems
-Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # WMTS driver
 The web map tile service driver extends abstracts WxS driver with the getTile feature.
 
 # Nodes
 ### WmtsServiceNode
 Represents the WMTS service. This node has no attribute and
 has as children WmtsOperationNode like GetTile.
@@ -76,15 +61,15 @@
 list_cap = service_wmts.children
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wmts.children:
+for child in service_wmts:
     print(child)
     print(child.name)
 
 #=>  <drb_driver_wXs.wXs_node.WXSNodeOperation object at 0x7f5403865d90>
 #=>  GetCapabilities
 #=>  <drb_driver_wmts.wmts_nodes.WmtsNodeOperationGetTile object at 0x7f54047b4700>
 #=>  GetTile
@@ -119,9 +104,7 @@
 print(tile_res)
 #=>  <drb_driver_image.image_node_factory.DrbImageBaseNode object at 0x7f54047b4970>
 
 ```
 
 
 
-
-
```

### Comparing `drb-driver-wmts-1.1.0/README.md` & `drb-driver-wmts-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: drb-driver-wmts
+Version: 1.2.0
+Summary: DRB wmts OGC Service driver
+Author: GAEL Systems
+Author-email: drb-python@gael.fr
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wmts
+Project-URL: Source, https://gitlab.com/drb-python/impl/wmts
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # WMTS driver
 The web map tile service driver extends abstracts WxS driver with the getTile feature.
 
 # Nodes
 ### WmtsServiceNode
 Represents the WMTS service. This node has no attribute and
 has as children WmtsOperationNode like GetTile.
@@ -61,15 +77,15 @@
 list_cap = service_wmts.children
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wmts.children:
+for child in service_wmts:
     print(child)
     print(child.name)
 
 #=>  <drb_driver_wXs.wXs_node.WXSNodeOperation object at 0x7f5403865d90>
 #=>  GetCapabilities
 #=>  <drb_driver_wmts.wmts_nodes.WmtsNodeOperationGetTile object at 0x7f54047b4700>
 #=>  GetTile
```

### Comparing `drb-driver-wmts-1.1.0/drb/drivers/wmts/wmts.py` & `drb-driver-wmts-1.2.0/drb/drivers/wmts/wmts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 from __future__ import annotations
 
 from drb.core import Predicate, DrbFactory, DrbNode
 from drb.drivers.http import DrbHttpNode
 from drb.drivers.wxs import WXSServiceNode, WXSNodeOperation
 from drb.exceptions.core import DrbFactoryException
 from requests.auth import AuthBase
-from typing import Optional
 
 
 class WmtsServiceNode(WXSServiceNode):
     def __init__(self, url: str, auth: AuthBase = None, **kwargs):
         if kwargs is not None and len(kwargs) > 0:
             super(WmtsServiceNode, self).__init__(url, auth=auth, **kwargs)
         else:
             super(WmtsServiceNode, self).__init__(url, auth)
         self._service_url = url.replace('+wmts', '') \
             if '+wmts' in url else url
+        self.namespace_uri = 'WMTS'
+        self.name = self._service_url
 
     @property
     def type_service(self):
         return 'WMTS'
 
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return 'WMTS'
-
-    @property
-    def name(self) -> str:
-        return self._service_url
-
     def manage_predefined_operations_metadata(self, name, request_cap, attr):
         operation = None
         if name == 'GetTile':
             operation = WmtsNodeOperationGetTile(
                 self,
                 name=name,
                 namespace=request_cap.namespace_uri,
```

### Comparing `drb-driver-wmts-1.1.0/drb_driver_wmts.egg-info/PKG-INFO` & `drb-driver-wmts-1.2.0/drb_driver_wmts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wmts
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB wmts OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/wmts
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wmts
+Project-URL: Source, https://gitlab.com/drb-python/impl/wmts
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WMTS driver
 The web map tile service driver extends abstracts WxS driver with the getTile feature.
 
 # Nodes
 ### WmtsServiceNode
 Represents the WMTS service. This node has no attribute and
@@ -76,15 +77,15 @@
 list_cap = service_wmts.children
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wmts.children:
+for child in service_wmts:
     print(child)
     print(child.name)
 
 #=>  <drb_driver_wXs.wXs_node.WXSNodeOperation object at 0x7f5403865d90>
 #=>  GetCapabilities
 #=>  <drb_driver_wmts.wmts_nodes.WmtsNodeOperationGetTile object at 0x7f54047b4700>
 #=>  GetTile
@@ -119,9 +120,7 @@
 print(tile_res)
 #=>  <drb_driver_image.image_node_factory.DrbImageBaseNode object at 0x7f54047b4970>
 
 ```
 
 
 
-
-
```

### Comparing `drb-driver-wmts-1.1.0/versioneer.py` & `drb-driver-wmts-1.2.0/versioneer.py`

 * *Files identical despite different names*

