# Comparing `tmp/factly_standard_names-0.1.4.tar.gz` & `tmp/factly_standard_names-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factly_standard_names-0.1.4.tar", max compression
+gzip compressed data, was "factly_standard_names-0.1.5.tar", max compression
```

## Comparing `factly_standard_names-0.1.4.tar` & `factly_standard_names-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       22 2022-02-16 12:54:55.000000 factly_standard_names-0.1.4/factly/standard_names/__init__.py
--rw-r--r--   0        0        0     1959 2022-11-04 08:44:25.361994 factly_standard_names-0.1.4/factly/standard_names/airline.csv
--rw-r--r--   0        0        0     2081 2022-11-04 08:44:25.362202 factly_standard_names-0.1.4/factly/standard_names/airline.py
--rw-r--r--   0        0        0     3625 2022-11-04 08:41:33.503022 factly_standard_names-0.1.4/factly/standard_names/banks.csv
--rw-r--r--   0        0        0     2077 2022-11-04 08:41:33.503110 factly_standard_names-0.1.4/factly/standard_names/banks.py
--rw-r--r--   0        0        0     1126 2022-11-04 08:44:25.362306 factly_standard_names-0.1.4/factly/standard_names/cities.csv
--rw-r--r--   0        0        0     2104 2022-11-04 08:44:25.362402 factly_standard_names-0.1.4/factly/standard_names/cities.py
--rw-r--r--   0        0        0     2546 2022-10-27 12:15:51.240626 factly_standard_names-0.1.4/factly/standard_names/country.csv
--rw-r--r--   0        0        0     2093 2022-11-04 08:44:25.363159 factly_standard_names-0.1.4/factly/standard_names/country.py
--rw-r--r--   0        0        0     2497 2022-11-04 08:44:25.363224 factly_standard_names-0.1.4/factly/standard_names/crops.csv
--rw-r--r--   0        0        0     2065 2022-11-04 08:44:25.363345 factly_standard_names-0.1.4/factly/standard_names/crops.py
--rw-r--r--   0        0        0      633 2022-10-27 12:15:51.241079 factly_standard_names-0.1.4/factly/standard_names/state.csv
--rw-r--r--   0        0        0      534 2022-11-04 08:44:25.363413 factly_standard_names-0.1.4/factly/standard_names/states-and-abbreviations.csv
--rw-r--r--   0        0        0     4573 2022-11-04 08:44:25.363640 factly_standard_names-0.1.4/factly/standard_names/states.py
--rw-r--r--   0        0        0     1757 2022-11-04 08:41:33.503204 factly_standard_names-0.1.4/factly/standard_names/units.py
--rw-r--r--   0        0        0      363 2022-11-04 08:44:40.476831 factly_standard_names-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 factly_standard_names-0.1.4/setup.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 factly_standard_names-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-09-27 06:09:48.279615 factly_standard_names-0.1.5/factly/standard_names/__init__.py
+-rw-r--r--   0        0        0     1959 2023-04-27 06:43:49.151220 factly_standard_names-0.1.5/factly/standard_names/airline.csv
+-rw-r--r--   0        0        0     2087 2023-04-27 06:43:49.151303 factly_standard_names-0.1.5/factly/standard_names/airline.py
+-rw-r--r--   0        0        0     3625 2023-04-27 06:43:49.151381 factly_standard_names-0.1.5/factly/standard_names/banks.csv
+-rw-r--r--   0        0        0     2077 2023-04-27 06:43:49.151454 factly_standard_names-0.1.5/factly/standard_names/banks.py
+-rw-r--r--   0        0        0     1126 2023-04-27 06:43:49.151521 factly_standard_names-0.1.5/factly/standard_names/cities.csv
+-rw-r--r--   0        0        0     2104 2023-04-27 06:43:49.151575 factly_standard_names-0.1.5/factly/standard_names/cities.py
+-rw-r--r--   0        0        0     2546 2023-03-03 09:57:28.878749 factly_standard_names-0.1.5/factly/standard_names/country.csv
+-rw-r--r--   0        0        0     2093 2023-04-27 06:43:49.151691 factly_standard_names-0.1.5/factly/standard_names/country.py
+-rw-r--r--   0        0        0     2497 2023-04-27 06:43:49.151756 factly_standard_names-0.1.5/factly/standard_names/crops.csv
+-rw-r--r--   0        0        0     2071 2023-04-27 06:43:49.151816 factly_standard_names-0.1.5/factly/standard_names/crops.py
+-rw-r--r--   0        0        0     1848 2023-04-27 07:03:40.846989 factly_standard_names-0.1.5/factly/standard_names/enums.py
+-rw-r--r--   0        0        0      633 2023-03-03 09:57:28.878994 factly_standard_names-0.1.5/factly/standard_names/state.csv
+-rw-r--r--   0        0        0      534 2023-04-27 06:43:49.151875 factly_standard_names-0.1.5/factly/standard_names/states-and-abbreviations.csv
+-rw-r--r--   0        0        0     4579 2023-04-27 06:43:49.151962 factly_standard_names-0.1.5/factly/standard_names/states.py
+-rw-r--r--   0        0        0     1757 2023-04-27 06:43:49.152022 factly_standard_names-0.1.5/factly/standard_names/units.py
+-rw-r--r--   0        0        0      363 2023-04-27 06:46:01.811905 factly_standard_names-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 factly_standard_names-0.1.5/setup.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 factly_standard_names-0.1.5/PKG-INFO
```

### Comparing `factly_standard_names-0.1.4/factly/standard_names/airline.csv` & `factly_standard_names-0.1.5/factly/standard_names/airline.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/airline.py` & `factly_standard_names-0.1.5/factly/standard_names/airline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 from pathlib import Path
 
 import pandas as pd
 from fuzzywuzzy import fuzz, process
 
 
-def airline_names(dfObj, column_name, thresh=70, manual_changes={}, identifier="None"):
+def airline_names(
+    dfObj, column_name, thresh=70, manual_changes={}, identifier="None"
+):
     """
     find all improper airline names from a given dataframe
     and replaces it with standard names proved.
     dfObj : DataFrame object on which airlines name should be standardize
     column_name : name of column which has entries as airline name
     manual_changes = Dict , default : null dict , changes in names done manually.
     """
```

### Comparing `factly_standard_names-0.1.4/factly/standard_names/banks.csv` & `factly_standard_names-0.1.5/factly/standard_names/banks.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/banks.py` & `factly_standard_names-0.1.5/factly/standard_names/banks.py`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/cities.csv` & `factly_standard_names-0.1.5/factly/standard_names/cities.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/cities.py` & `factly_standard_names-0.1.5/factly/standard_names/cities.py`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/country.csv` & `factly_standard_names-0.1.5/factly/standard_names/country.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/country.py` & `factly_standard_names-0.1.5/factly/standard_names/country.py`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/crops.csv` & `factly_standard_names-0.1.5/factly/standard_names/crops.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/crops.py` & `factly_standard_names-0.1.5/factly/standard_names/crops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 from pathlib import Path
 
 import pandas as pd
 from fuzzywuzzy import fuzz, process
 
 
-def crop_names(dfObj, column_name, thresh=70, manual_changes={}, identifier="None"):
+def crop_names(
+    dfObj, column_name, thresh=70, manual_changes={}, identifier="None"
+):
     """
     find all improper crop names from a given dataframe
     and replaces it with standard names proved.
     dfObj : DataFrame object on which crops name should be standardize
     column_name : name of column which has entries as crop name
     manual_changes = Dict , default : null dict , changes in names done manually.
     """
```

### Comparing `factly_standard_names-0.1.4/factly/standard_names/state.csv` & `factly_standard_names-0.1.5/factly/standard_names/state.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/states-and-abbreviations.csv` & `factly_standard_names-0.1.5/factly/standard_names/states-and-abbreviations.csv`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/factly/standard_names/states.py` & `factly_standard_names-0.1.5/factly/standard_names/states.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,17 @@
 
     # replacing values that needs to be changes only to specific column
     dfObj = dfObj.replace({column_name: changes})
 
     return dfObj
 
 
-def state_abbr_std_names(dfObj, column_name, manual_changes={}, identifier="None"):
+def state_abbr_std_names(
+    dfObj, column_name, manual_changes={}, identifier="None"
+):
 
     """
     find all state names from respective state abbreviation from a given dataframe
     and replaces it with standard names proved.
     dfObj : DataFrame object on which states abbreviation should be standardize
     column_name : name of column which has entries as state abbreviation
     manual_changes = Dict , default : null dict , changes in names done manually.
```

### Comparing `factly_standard_names-0.1.4/factly/standard_names/units.py` & `factly_standard_names-0.1.5/factly/standard_names/units.py`

 * *Files identical despite different names*

### Comparing `factly_standard_names-0.1.4/setup.py` & `factly_standard_names-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['fuzzywuzzy>=0.18.0,<0.19.0', 'pandas>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'factly-standard-names',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': 'None',
     'author': 'Factly Labs',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

