# Comparing `tmp/gwlandscape-python-0.3.1.tar.gz` & `tmp/gwlandscape-python-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwlandscape-python-0.3.1.tar", max compression
+gzip compressed data, was "gwlandscape-python-0.3.2.tar", max compression
```

## Comparing `gwlandscape-python-0.3.1.tar` & `gwlandscape-python-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.3.1/LICENSE
--rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.3.1/README.rst
--rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.3.1/gwlandscape_python/__init__.py
--rw-r--r--   0        0        0     2140 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/dataset_type.py
--rw-r--r--   0        0        0    17552 2023-04-21 06:22:03.415309 gwlandscape-python-0.3.1/gwlandscape_python/gwlandscape.py
--rw-r--r--   0        0        0     1578 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/keyword_type.py
--rw-r--r--   0        0        0     1890 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/model_type.py
--rw-r--r--   0        0        0     3771 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/publication_type.py
--rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.3.1/gwlandscape_python/settings.py
--rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.1/gwlandscape_python/tests/__init__.py
--rw-r--r--   0        0        0     3052 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/conftest.py
--rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_dataset_type.py
--rw-r--r--   0        0        0    36190 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_gwlandscape_python.py
--rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_keyword_type.py
--rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_model_type.py
--rw-r--r--   0        0        0     4228 2023-04-20 04:41:39.760269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_publication_type.py
--rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.1/gwlandscape_python/tests/utils.py
--rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.1/gwlandscape_python/utils/__init__.py
--rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.1/gwlandscape_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.3.1/gwlandscape_python/utils/utils.py
--rw-r--r--   0        0        0     1074 2023-04-21 06:22:03.419309 gwlandscape-python-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1661 2023-04-21 06:22:10.725775 gwlandscape-python-0.3.1/setup.py
--rw-r--r--   0        0        0     1618 2023-04-21 06:22:10.726006 gwlandscape-python-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.3.2/LICENSE
+-rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.3.2/README.rst
+-rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.3.2/gwlandscape_python/__init__.py
+-rw-r--r--   0        0        0     2170 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/dataset_type.py
+-rw-r--r--   0        0        0    17552 2023-04-21 06:22:03.415309 gwlandscape-python-0.3.2/gwlandscape_python/gwlandscape.py
+-rw-r--r--   0        0        0     1608 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/keyword_type.py
+-rw-r--r--   0        0        0     1920 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/model_type.py
+-rw-r--r--   0        0        0     3801 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/publication_type.py
+-rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.3.2/gwlandscape_python/settings.py
+-rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.2/gwlandscape_python/tests/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_dataset_type.py
+-rw-r--r--   0        0        0    16979 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_gwlandscape_python.py
+-rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_keyword_type.py
+-rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_model_type.py
+-rw-r--r--   0        0        0     3938 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_publication_type.py
+-rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.2/gwlandscape_python/tests/utils.py
+-rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.2/gwlandscape_python/utils/__init__.py
+-rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.2/gwlandscape_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.3.2/gwlandscape_python/utils/utils.py
+-rw-r--r--   0        0        0     1074 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1661 2023-04-27 00:55:40.483421 gwlandscape-python-0.3.2/setup.py
+-rw-r--r--   0        0        0     1618 2023-04-27 00:55:40.483638 gwlandscape-python-0.3.2/PKG-INFO
```

### Comparing `gwlandscape-python-0.3.1/LICENSE` & `gwlandscape-python-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/README.rst` & `gwlandscape-python-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/dataset_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/dataset_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import gwlandscape_python
 from gwlandscape_python.model_type import Model
 from gwlandscape_python.publication_type import Publication
 
 
 @dataclass
 class Dataset:
-    client: gwlandscape_python.gwlandscape.GWLandscape
+    client: gwlandscape_python.gwlandscape.GWLandscape = field(compare=False)
     id: str
     publication: Publication
     model: Model
     files: list
 
     def __repr__(self):
         return f'Dataset({self.publication} - {self.model})'
```

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/gwlandscape.py` & `gwlandscape-python-0.3.2/gwlandscape_python/gwlandscape.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/keyword_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/keyword_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import gwlandscape_python
 
 
 @dataclass
 class Keyword:
-    client: gwlandscape_python.gwlandscape.GWLandscape
+    client: gwlandscape_python.gwlandscape.GWLandscape = field(compare=False)
     id: str
     tag: str
 
     def __repr__(self):
         return f'Keyword("{self.tag}")'
 
     def update(self, tag=None):
```

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/model_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/model_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import gwlandscape_python
 
 
 @dataclass
 class Model:
-    client: gwlandscape_python.gwlandscape.GWLandscape
+    client: gwlandscape_python.gwlandscape.GWLandscape = field(compare=False)
     id: str
     name: str
     summary: str
     description: str
 
     def __repr__(self):
         return f'Model("{self.name}")'
```

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/publication_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/publication_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import gwlandscape_python
 
 
 @dataclass
 class Publication:
-    client: gwlandscape_python.gwlandscape.GWLandscape
+    client: gwlandscape_python.gwlandscape.GWLandscape = field(compare=False)
     id: str
     author: str
     published: bool
     title: str
     year: int
     journal: str
     journal_doi: str
```

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_dataset_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_keyword_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_model_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_publication_type.py` & `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_publication_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,24 @@
         }
     )
 
     for key, val in updated_data.items():
         assert getattr(publication, key) == val
 
 
-def test_update_publication_string_keywords(setup_gwl_request, create_publication, create_keyword):
+def test_update_publication_string_keywords(
+    setup_gwl_request,
+    create_publication,
+    create_keyword,
+    query_keyword_return
+):
     gwl, mock_request = setup_gwl_request
 
     mock_request.side_effect = [
-        *[
-            {
-                "keywords": {
-                    "edges": [
-                        {
-                            "node": {
-                                "id": f"mock_id{i}",
-                                "tag": f"mock_tag{i}"
-                            }
-                        }
-                    ]
-                }
-            } for i in range(100, 103)
-        ],
+        *[query_keyword_return(1, start_id=i) for i in range(100, 103)],
         {
             "update_publication": {
                 "result": True
             }
         }
     ]
```

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/utils/tests/test_utils.py` & `gwlandscape-python-0.3.2/gwlandscape_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/gwlandscape_python/utils/utils.py` & `gwlandscape-python-0.3.2/gwlandscape_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.1/pyproject.toml` & `gwlandscape-python-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwlandscape-python"
-version = "0.3.1"
+version = "0.3.2"
 description = "Wrapper of GWDC API, used for interacting with the GWLandscape endpoints"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>", "Lewis Lakerink <llakerink@swin.edu.au"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwlandscape_python"
 include = ["LICENSE",]
```

### Comparing `gwlandscape-python-0.3.1/setup.py` & `gwlandscape-python-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'tqdm>=4.61.2,<5.0.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.0.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
 
 setup_kwargs = {
     'name': 'gwlandscape-python',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Wrapper of GWDC API, used for interacting with the GWLandscape endpoints',
     'long_description': "GWLandscape Python API\n======================\n\n`GWLandscape <https://gwlandscape.org.au/>`_ is a service used to handle both the submission of COMPAS jobs (todo)\n\nCheck out the `documentation <https://gwlandscape-python.readthedocs.io/en/latest/>`_ for more information.\n\nInstallation\n------------\n\nThe gwlandscape-python package can be installed with\n\n::\n\n    pip install gwlandscape-python\n\n\nExample\n-------\n\n::\n\n    >>> from gwlandscape_python import GWLandscape\n    >>> gwl = GWLandscape(token='<user_api_token_here>')\n\n",
     'author': 'Thomas Reichardt',
     'author_email': 'treichardt@swin.edu.au',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/gravitationalwavedc/gwlandscape_python',
```

### Comparing `gwlandscape-python-0.3.1/PKG-INFO` & `gwlandscape-python-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwlandscape-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: Wrapper of GWDC API, used for interacting with the GWLandscape endpoints
 Home-page: https://github.com/gravitationalwavedc/gwlandscape_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

