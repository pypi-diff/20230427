# Comparing `tmp/daftlistings-2.0.2.tar.gz` & `tmp/daftlistings-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daftlistings-2.0.2.tar", last modified: Fri Jun 10 07:09:43 2022, max compression
+gzip compressed data, was "daftlistings-2.0.3.tar", last modified: Thu Apr 27 09:46:08 2023, max compression
```

## Comparing `daftlistings-2.0.2.tar` & `daftlistings-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 07:09:43.287575 daftlistings-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     8394 2022-06-10 07:09:43.287575 daftlistings-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5768 2022-06-10 07:07:11.000000 daftlistings-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 07:09:43.285575 daftlistings-2.0.2/daftlistings/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-10 07:02:46.000000 daftlistings-2.0.2/daftlistings/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12280 2022-06-10 07:02:46.000000 daftlistings-2.0.2/daftlistings/daft.py
--rw-r--r--   0 root         (0) root         (0)     5588 2022-06-10 07:02:46.000000 daftlistings-2.0.2/daftlistings/enums.py
--rw-r--r--   0 root         (0) root         (0)     5514 2022-06-10 07:02:46.000000 daftlistings-2.0.2/daftlistings/listing.py
--rw-r--r--   0 root         (0) root         (0)   469421 2022-06-10 07:02:46.000000 daftlistings-2.0.2/daftlistings/location.py
--rw-r--r--   0 root         (0) root         (0)     3701 2022-06-10 07:02:46.000000 daftlistings-2.0.2/daftlistings/map_visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 07:09:43.286574 daftlistings-2.0.2/daftlistings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8394 2022-06-10 07:09:43.000000 daftlistings-2.0.2/daftlistings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2022-06-10 07:09:43.000000 daftlistings-2.0.2/daftlistings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 07:09:43.000000 daftlistings-2.0.2/daftlistings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 07:03:32.000000 daftlistings-2.0.2/daftlistings.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-10 07:09:43.000000 daftlistings-2.0.2/daftlistings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-06-10 07:09:43.000000 daftlistings-2.0.2/daftlistings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-10 07:09:43.287575 daftlistings-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2077 2022-06-10 07:09:35.000000 daftlistings-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:46:08.052675 daftlistings-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 09:45:53.000000 daftlistings-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-27 09:46:08.052675 daftlistings-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-27 09:45:53.000000 daftlistings-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:46:08.048675 daftlistings-2.0.3/daftlistings/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-27 09:45:53.000000 daftlistings-2.0.3/daftlistings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-27 09:45:53.000000 daftlistings-2.0.3/daftlistings/daft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-27 09:45:53.000000 daftlistings-2.0.3/daftlistings/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-27 09:45:53.000000 daftlistings-2.0.3/daftlistings/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   469421 2023-04-27 09:45:53.000000 daftlistings-2.0.3/daftlistings/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-27 09:45:53.000000 daftlistings-2.0.3/daftlistings/map_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:46:08.052675 daftlistings-2.0.3/daftlistings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-27 09:46:08.000000 daftlistings-2.0.3/daftlistings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-27 09:46:08.000000 daftlistings-2.0.3/daftlistings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:46:08.000000 daftlistings-2.0.3/daftlistings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:46:07.000000 daftlistings-2.0.3/daftlistings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:46:08.000000 daftlistings-2.0.3/daftlistings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 09:46:08.000000 daftlistings-2.0.3/daftlistings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:46:08.052675 daftlistings-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-27 09:45:53.000000 daftlistings-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:46:08.052675 daftlistings-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-04-27 09:45:53.000000 daftlistings-2.0.3/tests/test_daft_search.py
```

### Comparing `daftlistings-2.0.2/README.md` & `daftlistings-2.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ``` bash
 pip install https://github.com/AnthonyBloomer/daftlistings/archive/dev.zip
 ```
 
 ## Usage
 
-```python
+``` python
 from daftlistings import Daft
 
 daft = Daft()
 listings = daft.search()
 
 for listing in listings:
     print(listing.title)
```

### Comparing `daftlistings-2.0.2/daftlistings/daft.py` & `daftlistings-2.0.3/daftlistings/daft.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     def __init__(self):
         self._section = None
         self._filters = list()
         self._andFilters = list()
         self._ranges = list()
         self._geoFilter = dict()
         self._sort_filter = dict()
-        self._paging = self._PAGE_0
         self._total_results = 0
 
     @property
     def total_results(self):
         return self._total_results
 
     def _set_range_to(self, name: str, to: str):
@@ -237,15 +236,15 @@
             payload["andFilters"] = self._andFilters
         if self._ranges:
             payload["ranges"] = self._ranges
         if self._geoFilter:
             payload["geoFilter"] = self._geoFilter
         if self._sort_filter:
             payload["sort"] = self._sort_filter
-        payload["paging"] = self._paging
+        payload["paging"] = deepcopy(self._PAGE_0)
         return payload
 
     def search(self, max_pages: Optional[int] = None) -> List[Listing]:
         print("Searching...")
         _payload = self._make_payload()
         r = requests.post(self._ENDPOINT,
                           headers=self._HEADER,
```

### Comparing `daftlistings-2.0.2/daftlistings/enums.py` & `daftlistings-2.0.3/daftlistings/enums.py`

 * *Files identical despite different names*

### Comparing `daftlistings-2.0.2/daftlistings/listing.py` & `daftlistings-2.0.3/daftlistings/listing.py`

 * *Files identical despite different names*

### Comparing `daftlistings-2.0.2/daftlistings/location.py` & `daftlistings-2.0.3/daftlistings/location.py`

 * *Files identical despite different names*

### Comparing `daftlistings-2.0.2/daftlistings/map_visualization.py` & `daftlistings-2.0.3/daftlistings/map_visualization.py`

 * *Files identical despite different names*

### Comparing `daftlistings-2.0.2/setup.py` & `daftlistings-2.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,26 +42,25 @@
         self.status('Uploading the package to PyPi via Twine…')
         os.system('twine upload dist/*')
 
         sys.exit()
 
 
 setup(name='daftlistings',
-      version='2.0.2',
+      version='2.0.3',
       description='A library that enables programmatic interaction with daft.ie. Daft.ie has nationwide coverage and contains about 80% of the total available properties in Ireland.',
-      long_description_content_type='text/markdown',
       long_description=long_descr,
+      long_description_content_type='text/markdown',
       url='https://github.com/AnthonyBloomer/daftlistings',
       author='Anthony Bloomer',
       keywords=['daft', 'real estate', 'daft.ie'],
       author_email='ant0@protonmail.ch',
       license='MIT',
       packages=['daftlistings'],
       install_requires=[
-          'enum34',
           'requests',
           'folium'
       ],
       classifiers=[
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           "Topic :: Software Development :: Libraries",
```

