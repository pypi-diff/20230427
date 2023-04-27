# Comparing `tmp/pygoogalytics-0.3.1.tar.gz` & `tmp/pygoogalytics-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.3.1.tar", last modified: Thu Apr 20 09:50:47 2023, max compression
+gzip compressed data, was "pygoogalytics-0.3.2.tar", last modified: Thu Apr 27 14:13:36 2023, max compression
```

## Comparing `pygoogalytics-0.3.1.tar` & `pygoogalytics-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 09:50:47.913554 pygoogalytics-0.3.1/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.3.1/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.3.1/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-20 09:50:47.913440 pygoogalytics-0.3.1/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.3.1/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 09:50:47.911798 pygoogalytics-0.3.1/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-20 09:49:27.000000 pygoogalytics-0.3.1/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5386 2023-04-20 08:34:21.000000 pygoogalytics-0.3.1/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 09:50:47.913123 pygoogalytics-0.3.1/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.3.1/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.3.1/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    36784 2023-04-13 07:30:02.000000 pygoogalytics-0.3.1/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.3.1/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    42080 2023-04-13 10:54:44.000000 pygoogalytics-0.3.1/pygoogalytics/kwp_wrappers.py
--rw-r--r--   0 joshua     (501) staff       (20)     2485 2023-04-20 09:49:13.000000 pygoogalytics-0.3.1/pygoogalytics/resource_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.3.1/pygoogalytics/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-20 09:50:47.912472 pygoogalytics-0.3.1/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-20 09:50:47.000000 pygoogalytics-0.3.1/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-20 09:50:47.000000 pygoogalytics-0.3.1/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-20 09:50:47.000000 pygoogalytics-0.3.1/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-20 09:50:47.000000 pygoogalytics-0.3.1/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-20 09:50:47.000000 pygoogalytics-0.3.1/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-20 09:50:47.913590 pygoogalytics-0.3.1/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-20 09:49:27.000000 pygoogalytics-0.3.1/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.807663 pygoogalytics-0.3.2/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.3.2/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.3.2/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-27 14:13:36.807528 pygoogalytics-0.3.2/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.3.2/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.805881 pygoogalytics-0.3.2/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-27 14:13:00.000000 pygoogalytics-0.3.2/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5386 2023-04-20 08:34:21.000000 pygoogalytics-0.3.2/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.807162 pygoogalytics-0.3.2/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.3.2/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.3.2/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    36784 2023-04-13 07:30:02.000000 pygoogalytics-0.3.2/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.3.2/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42100 2023-04-27 14:09:01.000000 pygoogalytics-0.3.2/pygoogalytics/kwp_wrappers.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2485 2023-04-20 09:49:13.000000 pygoogalytics-0.3.2/pygoogalytics/resource_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.3.2/pygoogalytics/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.806668 pygoogalytics-0.3.2/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-27 14:13:36.807702 pygoogalytics-0.3.2/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-27 14:13:00.000000 pygoogalytics-0.3.2/setup.py
```

### Comparing `pygoogalytics-0.3.1/LICENCE.txt` & `pygoogalytics-0.3.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/LICENSE` & `pygoogalytics-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/PKG-INFO` & `pygoogalytics-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.3.1
+Version: 0.3.2
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.3.1/README.md` & `pygoogalytics-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/__init__.py` & `pygoogalytics-0.3.2/pygoogalytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.3.1/pygoogalytics/client.py` & `pygoogalytics-0.3.2/pygoogalytics/client.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.3.2/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.3.2/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.3.2/pygoogalytics/googalytics_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/googlepandas.py` & `pygoogalytics-0.3.2/pygoogalytics/googlepandas.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.3.2/pygoogalytics/kwp_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,16 @@
         monthly_volume_df['month_enum'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[2])
         monthly_volume_df['month'] = monthly_volume_df['month_enum'].apply(_get_month_from_enum_value)
         monthly_volume_df['year'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[1])
 
         monthly_volume_df.dropna(axis='index', subset=['month'], inplace=True)
 
         monthly_volume_df['record_date'] = monthly_volume_df.apply(
-            lambda df: _conv_date(df['year'], df['month'], 15)
+            lambda df: _conv_date(df['year'], df['month'], 15),
+            axis=1
         )
         monthly_volume_df['volume'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[0])
 
         monthly_volume_df.drop(
             columns=['month_enum', 'volume_trend_tuples', 'month', 'year' 'month_name'],
             inplace=True
         )
```

### Comparing `pygoogalytics-0.3.1/pygoogalytics/resource_utils.py` & `pygoogalytics-0.3.2/pygoogalytics/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics/utils.py` & `pygoogalytics-0.3.2/pygoogalytics/utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.3.2/pygoogalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.3.1
+Version: 0.3.2
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.3.1/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.3.2/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.1/setup.py` & `pygoogalytics-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.3.1',
+    version='0.3.2',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

