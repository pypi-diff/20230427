# Comparing `tmp/drb-driver-wcs-1.1.0.tar.gz` & `tmp/drb-driver-wcs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-wcs-1.1.0.tar", last modified: Wed Dec 21 15:22:53 2022, max compression
+gzip compressed data, was "drb-driver-wcs-1.2.0.tar", last modified: Thu Apr 27 13:29:45 2023, max compression
```

## Comparing `drb-driver-wcs-1.1.0.tar` & `drb-driver-wcs-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.728963 drb-driver-wcs-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3225 2022-12-21 15:22:53.728963 drb-driver-wcs-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2766 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.724963 drb-driver-wcs-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.724963 drb-driver-wcs-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.732963 drb-driver-wcs-1.1.0/drb/drivers/wcs/
--rw-rw-rw-   0 root         (0) root         (0)      455 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/drb/drivers/wcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-21 15:22:53.732963 drb-driver-wcs-1.1.0/drb/drivers/wcs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3665 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/drb/drivers/wcs/wcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.728963 drb-driver-wcs-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/drb/exceptions/wcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.724963 drb-driver-wcs-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.728963 drb-driver-wcs-1.1.0/drb/topics/wcs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/drb/topics/wcs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/drb/topics/wcs/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 15:22:53.728963 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3225 2022-12-21 15:22:53.000000 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2022-12-21 15:22:53.000000 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 15:22:53.000000 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2022-12-21 15:22:53.000000 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-21 15:22:53.000000 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-21 15:22:53.000000 drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-12-21 15:22:53.732963 drb-driver-wcs-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-21 14:22:16.000000 drb-driver-wcs-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.283644 drb-driver-wcs-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:01:21.000000 drb-driver-wcs-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-21 14:22:16.000000 drb-driver-wcs-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-04-27 13:29:45.283644 drb-driver-wcs-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-25 21:13:22.000000 drb-driver-wcs-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.235643 drb-driver-wcs-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.235643 drb-driver-wcs-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.287644 drb-driver-wcs-1.2.0/drb/drivers/wcs/
+-rw-rw-rw-   0 root         (0) root         (0)      455 2022-12-21 14:22:16.000000 drb-driver-wcs-1.2.0/drb/drivers/wcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-27 13:29:45.287644 drb-driver-wcs-1.2.0/drb/drivers/wcs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2023-04-26 15:08:35.000000 drb-driver-wcs-1.2.0/drb/drivers/wcs/wcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.247643 drb-driver-wcs-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-21 14:22:16.000000 drb-driver-wcs-1.2.0/drb/exceptions/wcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.235643 drb-driver-wcs-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.247643 drb-driver-wcs-1.2.0/drb/topics/wcs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-21 14:22:16.000000 drb-driver-wcs-1.2.0/drb/topics/wcs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-27 13:28:56.000000 drb-driver-wcs-1.2.0/drb/topics/wcs/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.251644 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-04-27 13:29:45.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      583 2023-04-27 13:29:45.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 13:29:45.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-27 13:29:45.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 13:29:44.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 13:29:45.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-27 13:29:45.000000 drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-25 21:13:22.000000 drb-driver-wcs-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-25 21:13:22.000000 drb-driver-wcs-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-27 13:29:45.287644 drb-driver-wcs-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-25 21:13:22.000000 drb-driver-wcs-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:29:45.251644 drb-driver-wcs-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6271 2022-12-21 14:22:16.000000 drb-driver-wcs-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-04-26 12:10:09.000000 drb-driver-wcs-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    21744 2023-04-26 15:08:35.000000 drb-driver-wcs-1.2.0/tests/test_wcs.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-21 14:22:16.000000 drb-driver-wcs-1.2.0/versioneer.py
```

### Comparing `drb-driver-wcs-1.1.0/PKG-INFO` & `drb-driver-wcs-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wcs
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB WCS OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/wcs
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wcs
+Project-URL: Source, https://gitlab.com/drb-python/impl/wcs
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WCS driver
 The web coverage service driver extends abstracts WxS driver with the GetCoverage feature.
 
 
 # Nodes
 ### WcsServiceNode
@@ -71,22 +72,22 @@
 from drb.drivers.wcs import WcsServiceNode
 
 url_wcs='https+wcs://myserver_wcs/wcs'
 
 
 service_wcs = WcsServiceNode(url_wcs)
 
-list_cap = service_wcs.children
+list_cap = service_wcs[:]
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wcs.children:
+for child in service_wcs:
     print(child)
     print(child.name)
 
 # => <drb_driver_wxs.wXs_node.WXSNodeOperation object at 0x7fea3b54ac70>
 # => GetCapabilities
 # => <drb_driver_wcs.wcs_nodes.WcsNodeOperationDescribeCoverage object at 0x7fea3b5652e0>
 # => DescribeCoverage
@@ -106,9 +107,7 @@
 print(describe[0].name)
 # => <drb_driver_xml.xml_node.XmlNode object at 0x7f7aa91f0be0>
 # => CoverageDescription
 
 ```
 
 
-
-
```

### Comparing `drb-driver-wcs-1.1.0/README.md` & `drb-driver-wcs-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 from drb.drivers.wcs import WcsServiceNode
 
 url_wcs='https+wcs://myserver_wcs/wcs'
 
 
 service_wcs = WcsServiceNode(url_wcs)
 
-list_cap = service_wcs.children
+list_cap = service_wcs[:]
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wcs.children:
+for child in service_wcs:
     print(child)
     print(child.name)
 
 # => <drb_driver_wxs.wXs_node.WXSNodeOperation object at 0x7fea3b54ac70>
 # => GetCapabilities
 # => <drb_driver_wcs.wcs_nodes.WcsNodeOperationDescribeCoverage object at 0x7fea3b5652e0>
 # => DescribeCoverage
```

### Comparing `drb-driver-wcs-1.1.0/drb/drivers/wcs/wcs.py` & `drb-driver-wcs-1.2.0/drb/drivers/wcs/wcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 from __future__ import annotations
 
 from drb.core import Predicate, DrbFactory, DrbNode
 from drb.drivers.http import DrbHttpNode
 from drb.drivers.wxs import WXSServiceNode, WXSNodeOperation
 from drb.exceptions.core import DrbFactoryException
 from requests.auth import AuthBase
-from typing import Optional
 
 
 class WcsServiceNode(WXSServiceNode):
     def __init__(self, url: str, auth: AuthBase = None, **kwargs):
         if kwargs is not None and len(kwargs) > 0:
             super(WcsServiceNode, self).__init__(url, auth=auth, **kwargs)
         else:
             super(WcsServiceNode, self).__init__(url, auth)
         self._service_url = url.replace('+wcs', '') \
             if '+wcs' in url else url
+        self.namespace_uri = 'WCS'
+        self.name = self._service_url
 
     @property
     def type_service(self):
         return 'WCS'
 
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return 'WCS'
-
-    @property
-    def name(self) -> str:
-        return self._service_url
-
     def manage_predefined_operations_metadata(self, name, request_cap, attr):
         operation = None
         if name == 'GetCoverage':
             operation = WcsNodeOperationGetCoverage(
                 self,
                 name=name,
                 namespace=request_cap.namespace_uri,
@@ -50,15 +43,14 @@
     def read_capabilities(self, xmlnode_tree):
         super().read_capabilities(xmlnode_tree)
 
 
 class WcsDescribeCoveragePredicate(Predicate):
 
     def __init__(self, coverage_id, **kwargs):
-
         self._coverage_id = coverage_id
         self.others = dict(**kwargs)
 
     def to_dict(self, version):
         arg_dict = {}
 
         # If the predicate force a specific version
```

### Comparing `drb-driver-wcs-1.1.0/drb_driver_wcs.egg-info/PKG-INFO` & `drb-driver-wcs-1.2.0/drb_driver_wcs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wcs
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB WCS OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/wcs
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wcs
+Project-URL: Source, https://gitlab.com/drb-python/impl/wcs
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WCS driver
 The web coverage service driver extends abstracts WxS driver with the GetCoverage feature.
 
 
 # Nodes
 ### WcsServiceNode
@@ -71,22 +72,22 @@
 from drb.drivers.wcs import WcsServiceNode
 
 url_wcs='https+wcs://myserver_wcs/wcs'
 
 
 service_wcs = WcsServiceNode(url_wcs)
 
-list_cap = service_wcs.children
+list_cap = service_wcs[:]
 
 print('----------------------------------------')
 print('list_cap')
 
 print(list_cap)
 
-for child in service_wcs.children:
+for child in service_wcs:
     print(child)
     print(child.name)
 
 # => <drb_driver_wxs.wXs_node.WXSNodeOperation object at 0x7fea3b54ac70>
 # => GetCapabilities
 # => <drb_driver_wcs.wcs_nodes.WcsNodeOperationDescribeCoverage object at 0x7fea3b5652e0>
 # => DescribeCoverage
@@ -106,9 +107,7 @@
 print(describe[0].name)
 # => <drb_driver_xml.xml_node.XmlNode object at 0x7f7aa91f0be0>
 # => CoverageDescription
 
 ```
 
 
-
-
```

### Comparing `drb-driver-wcs-1.1.0/versioneer.py` & `drb-driver-wcs-1.2.0/versioneer.py`

 * *Files identical despite different names*

