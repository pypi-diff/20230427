# Comparing `tmp/duro_rest-0.0.6.tar.gz` & `tmp/duro_rest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duro_rest-0.0.6.tar", max compression
+gzip compressed data, was "duro_rest-0.0.7.tar", max compression
```

## Comparing `duro_rest-0.0.6.tar` & `duro_rest-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    16726 2022-12-13 18:32:39.878220 duro_rest-0.0.6/LICENSE
--rw-r--r--   0        0        0     1758 2022-12-15 15:51:37.207962 duro_rest-0.0.6/README.md
--rw-r--r--   0        0        0      477 2022-12-19 16:20:02.232066 duro_rest-0.0.6/duro_rest/__init__.py
--rw-r--r--   0        0        0     7257 2022-12-19 16:21:49.248370 duro_rest-0.0.6/duro_rest/bom_client.py
--rw-r--r--   0        0        0     8275 2022-12-19 17:10:26.528406 duro_rest-0.0.6/duro_rest/duro_client.py
--rw-r--r--   0        0        0      641 2022-12-13 22:48:34.469642 duro_rest-0.0.6/duro_rest/error.py
--rw-r--r--   0        0        0      556 2022-12-19 17:12:31.264697 duro_rest-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 duro_rest-0.0.6/setup.py
--rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 duro_rest-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    16726 2022-12-13 18:32:39.878220 duro_rest-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1758 2022-12-15 15:51:37.207962 duro_rest-0.0.7/README.md
+-rw-r--r--   0        0        0      477 2022-12-19 16:20:02.232066 duro_rest-0.0.7/duro_rest/__init__.py
+-rw-r--r--   0        0        0     7679 2023-04-27 18:07:29.757753 duro_rest-0.0.7/duro_rest/bom_client.py
+-rw-r--r--   0        0        0     8312 2023-04-27 17:19:54.511297 duro_rest-0.0.7/duro_rest/duro_client.py
+-rw-r--r--   0        0        0      641 2022-12-13 22:48:34.469642 duro_rest-0.0.7/duro_rest/error.py
+-rw-r--r--   0        0        0      556 2023-04-27 13:40:55.065101 duro_rest-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 duro_rest-0.0.7/setup.py
+-rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 duro_rest-0.0.7/PKG-INFO
```

### Comparing `duro_rest-0.0.6/LICENSE` & `duro_rest-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `duro_rest-0.0.6/README.md` & `duro_rest-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `duro_rest-0.0.6/duro_rest/bom_client.py` & `duro_rest-0.0.7/duro_rest/bom_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 # Copyright 2022 Oxide Computer Company
 
 import copy
+import json
 from duro_rest.duro_client import Client, Cache
 
 class FlattenedBOM(list):
   def __init__(self, data: list):
     list.__init__(self, data)
     self.__data = data
 
@@ -54,14 +55,15 @@
       component['quantity'] = component['multiplied_quantity']
 
       # We need to drop a few fields that we are not interested in, or can not merge
       component.pop('isAddedAfterPullRequest', None)
       component.pop('itemNumber', None)
       component.pop('multiplied_quantity', None)
       component.pop('parents', None)
+      component.pop('parent_cpns', None)
       component.pop('level', None)
 
       # For each component, check the id to see if we already have it in the list of unique
       # components
       existing = next((c for c in unique_components if component['_id'] == c['_id']), None)
 
       # If we found an existing component, sum together the quantities of the current component and
@@ -114,14 +116,15 @@
 def component_list(component) -> list:
   # When we start processing a component, set its multiplied quantity to its non-multiplied
   # quantity. As we traverse back up the tree this field will be updated as needed
   component['multiplied_quantity'] = component['quantity']
 
   # Start an empty lit of parent component ids
   component['parents'] = []
+  component['parent_cpns'] = []
 
   # Component depth starts at 0 and will be incremented as we walk back up the tree
   component['level'] = 0
 
   # The component passed in represents a portion of the nested BOM. Here we are going to flatten all
   # of this component's children (and nested children) by calling component_list on each child
   # component. Since component_list returns a list of components, the map call here will end up
@@ -132,14 +135,15 @@
   for child in flattened_children:
     # For each child component we multiply its quantity by the quantity of the current component
     # we are looking at. We store the value to make future work easier
     child['multiplied_quantity'] = component['multiplied_quantity'] * child['multiplied_quantity']
 
     # We also want to track the parents list to identify the path back up the tree from a leaf
     child['parents'].append(component['_id'])
+    child['parent_cpns'].append(component['cpn'])
 
     # Increment the level of each child component by one
     child['level'] = child['level'] + 1
 
   # Since we are flattening the BOM we no longer want the components to have references to their
   # children
   component.pop('children', None)
@@ -168,15 +172,22 @@
     return NestedBOM(parent)
 
 def expand_child_components(parent, components):
   # The components list contains most of the needed data, but we need some of the properties that
   # are defined by the parent component (specifically the quantity). Therefore we combine the
   # properties of the parent we are currently expanding with the expanded data available from
   # fetching all of the components
-  expanded_parent = {**parent, **next(component for component in components if component['_id'] == parent['component'])}
+  matching_components = list(component for component in components if component['_id'] == parent['component'])
+
+  if len(matching_components) == 0:
+    raise LookupError('Failed to find component in cache ' + parent['component'])
+  elif len(matching_components) > 1:
+    raise LookupError('Found multiple components in cache ' + parent['component'])
+
+  expanded_parent = {**parent, **matching_components[0]}
 
   # Now that we have expanded the parent component, we need to expand each of the child components
   expanded_parent['children'] = list(map(lambda child: expand_child_components(child, components), expanded_parent['children']))
 
   return expanded_parent
 
 def flatten(l):
```

### Comparing `duro_rest-0.0.6/duro_rest/duro_client.py` & `duro_rest-0.0.7/duro_rest/duro_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
       self.__cache_file = open(path, "w")
       pass
     finally:
       # Make sure we always rewind to the start of the file
       self.__cache_file.seek(0, 0)
 
   def save(self):
+    self.__cache_file.truncate()
     self.__cache_file.write(json.dumps(self._Cache__data))
     self.__cache_file.seek(0, 0)
 
 class Client:
   def __init__(self, api_key, url = "https://public-api.duro.app", cache = Cache(0)):
     self.__base_url = url + "/v1/"
     self.__api_key = api_key
@@ -298,15 +299,15 @@
 
     total_results = page["resultCount"]
     pages = math.ceil(total_results / 100)
 
     resources = resources + page[resultKey]
 
     if pages > 1:
-      for page_index in range(2, pages):
+      for page_index in range(2, pages + 1):
         page = self.__get(path, params = {**params, "perPage": 100, "page": page_index})
         resources = resources + page[resultKey]
 
     # For each resource we found populate its individual record in the cache
     for resource in resources:
       self.__cache.insert(path + "/" + resource["_id"] + "::{}", resource)
```

### Comparing `duro_rest-0.0.6/duro_rest/error.py` & `duro_rest-0.0.7/duro_rest/error.py`

 * *Files identical despite different names*

### Comparing `duro_rest-0.0.6/pyproject.toml` & `duro_rest-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "duro_rest"
-version = "0.0.6"
+version = "0.0.7"
 description = "An API client for the Duro REST API"
 license = "MPL-2.0"
 authors = [
   "Augustus Mayo <augustus@oxidecomputer.com>"
 ]
 maintainers = [
   "Augustus Mayo <augustus@oxidecomputer.com>"
```

### Comparing `duro_rest-0.0.6/setup.py` & `duro_rest-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2,<3']
 
 setup_kwargs = {
     'name': 'duro-rest',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'An API client for the Duro REST API',
     'long_description': '# duro_rest\n\nAn API client for the [Duro REST API](https://public-api.duro.app/v1/docs/).\n\n## Installation\n\nInstalling from [PyPi]()\n\n```pip install duro_rest```\n\nInstalling from [conda-forge]()\n\nTBD\n\n## Examples\n\nThe Duro client is a very minimal API client for reading data from the [Duro v1 REST API](https://public-api.duro.app/v1/docs/). It does not define classes for each object type and instead returns plain dictionaries\nand lists.\n\n#### Base Client\n\n```python\nfrom duro_rest import Client\n\n# Create a new client, providing your API key. By default clients will make calls to the public REST\n# API, but the endpoint base can be overridden if needed\nclient = Client("your-api-key")\n\n# Fetch a component by its Duro assigned id (as opposed to the CPN)\ncomponent = client.component("component-id")\n\n# Fetch a list of all components in Duro\ncomponents = client.components()\n\n# Fetch a list of all components in Duro filtered by status\ncomponents = client.components(status = "OBSOLETE")\n```\n\n#### BOM Client\n\nThe Duro API does not support pulling BOMs directly. The BOM Client is here to make that experience\na little easier.\n\n```python\nfrom duro_rest import BOMClient\n\n# Create a new bom client for fetching full BOMs (either nested or flattened). It accepts the same\n# arguments as the base client\nclient = Client("your-api-key")\n\n# Get a nested BOM starting from a product\nnested_product_bom = client.product_bom("product-id")\n\n# Get a nested BOM starting from a component\nnested_component_bom = client.component("component-id")\n\n# Convert the nested BOM into flattened BOM\nindented_product_bom = nested_product_bom.idented()\n\n# Flattening will collapse rows for the same components together\nflattened_product_bom = indented_product_bom.flatten()\n```',
     'author': 'Augustus Mayo',
     'author_email': 'augustus@oxidecomputer.com',
     'maintainer': 'Augustus Mayo',
     'maintainer_email': 'augustus@oxidecomputer.com',
     'url': 'https://pypi.org/project/duro-rest/',
```

### Comparing `duro_rest-0.0.6/PKG-INFO` & `duro_rest-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duro-rest
-Version: 0.0.6
+Version: 0.0.7
 Summary: An API client for the Duro REST API
 Home-page: https://pypi.org/project/duro-rest/
 License: MPL-2.0
 Author: Augustus Mayo
 Author-email: augustus@oxidecomputer.com
 Maintainer: Augustus Mayo
 Maintainer-email: augustus@oxidecomputer.com
```

