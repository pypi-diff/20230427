# Comparing `tmp/sportydatagen-0.1.0.tar.gz` & `tmp/sportydatagen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportydatagen-0.1.0.tar", max compression
+gzip compressed data, was "sportydatagen-0.2.0.tar", max compression
```

## Comparing `sportydatagen-0.1.0.tar` & `sportydatagen-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-15 17:58:53.525688 sportydatagen-0.1.0/LICENSE
--rw-r--r--   0        0        0     1577 2023-04-15 17:58:53.525688 sportydatagen-0.1.0/README.md
--rw-r--r--   0        0        0     1838 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      188 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/__init__.py
--rw-r--r--   0        0        0     3261 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/activity.py
--rw-r--r--   0        0        0     1276 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/csv_utils.py
--rw-r--r--   0        0        0     2492 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/gpx_convert_to_csv.py
--rw-r--r--   0        0        0     7148 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/return_random_data.py
--rw-r--r--   0        0        0     2581 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/saf_tcx_extract_data_to_csv.py
--rw-r--r--   0        0        0     3891 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/tcx_convert_to_csv.py
--rw-r--r--   0        0        0     4504 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/tcx_feature_extraction_utils.py
--rw-r--r--   0        0        0     3773 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/tcx_utils.py
--rw-r--r--   0        0        0     1934 2023-04-15 17:58:53.652689 sportydatagen-0.1.0/sportydatagen/utils.py
--rw-r--r--   0        0        0     2360 2023-04-15 17:59:35.084875 sportydatagen-0.1.0/setup.py
--rw-r--r--   0        0        0     2299 2023-04-15 17:59:35.085121 sportydatagen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 15:01:59.848205 sportydatagen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1576 2023-04-27 15:01:59.848205 sportydatagen-0.2.0/README.md
+-rw-r--r--   0        0        0     1800 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/__init__.py
+-rw-r--r--   0        0        0     5358 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/activity.py
+-rw-r--r--   0        0        0     2878 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/banister_trimp_v2.py
+-rw-r--r--   0        0        0     7186 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/convert_to_csv.py
+-rw-r--r--   0        0        0     5020 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/csv_utils.py
+-rw-r--r--   0        0        0     8784 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/feature_extraction_utils.py
+-rw-r--r--   0        0        0      142 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/filetype.py
+-rw-r--r--   0        0        0     7148 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/return_random_data.py
+-rw-r--r--   0        0        0     2895 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/saf_extract_features_to_csv.py
+-rw-r--r--   0        0        0      459 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/sportfile_utils.py
+-rw-r--r--   0        0        0     2514 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/utils.py
+-rw-r--r--   0        0        0     2358 2023-04-27 15:02:06.761357 sportydatagen-0.2.0/setup.py
+-rw-r--r--   0        0        0     2298 2023-04-27 15:02:06.761613 sportydatagen-0.2.0/PKG-INFO
```

### Comparing `sportydatagen-0.1.0/LICENSE` & `sportydatagen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.1.0/README.md` & `sportydatagen-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
 ## License
 
 This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
 
 ## Disclaimer
 
 This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
-
```

### Comparing `sportydatagen-0.1.0/pyproject.toml` & `sportydatagen-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sportydatagen"
-version = "0.1.0"
+version = "0.2.0"
 description = "Sports activity generator module"
 license="MIT"
 readme = "README.md"
 keywords = ['artificial sport trainer', 'computational intelligence', 'data mining', 'sport activities', 'tcx']
 authors = ["Rok Kukovec <rok.kukovec1@student.um.si>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
 homepage = "https://gitlab.com/firefly-cpp/sportydatagen"
 repository = "https://gitlab.com/firefly-cpp/sportydatagen"
@@ -13,17 +13,16 @@
 python = "^3.11"
 niapy = "^2.0.5"
 sport-activities-features = "^0.3.11"
 numpy = "^1.24.2"
 pandas = "*"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.0"
+pytest = "^7.3.1"
 black = "^23.1.0"
-flask = "^2.2.3"
 isort = "^5.12.0"
 ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -40,15 +39,15 @@
 # Black = 88, but we're using 79 to match Flake8.
 line-length = 79
 # every check supported by Ruff
 select = [
     'ALL',
 ]
 
-ignore = ['D211', 'D213']
+ignore = ['D211', 'D213', 'EXE002']
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     '.git',
     '.ruff_cache',
     '.tox',
     '.venv',
@@ -65,15 +64,15 @@
 ]
 
 [tool.ruff.per-file-ignores]
 'basic_run.py' = ['T201'] # Prints output into console
 # Delete next 3 lines in release version
 'sportydatagen/*.py' = ['T201'] # Prints progress into console
 'examples/*.py' = ['T201'] # Prints progress into console
-'tests/*.py' = ['S101'] # Prints progress into console
+'tests/*.py' = ['S101']
 
 [tool.ruff.flake8-quotes]
 inline-quotes = 'single'
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
```

### Comparing `sportydatagen-0.1.0/sportydatagen/return_random_data.py` & `sportydatagen-0.2.0/sportydatagen/return_random_data.py`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.1.0/sportydatagen/saf_tcx_extract_data_to_csv.py` & `sportydatagen-0.2.0/sportydatagen/saf_extract_features_to_csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Extracting data from multiple TCX files using sport-activities-features."""
 
 import os
 from pathlib import Path
 
 import pandas as pd
-from sport_activities_features import TCXFile
+from sport_activities_features import GPXFile, TCXFile
 
-tcx_file = TCXFile()
+from sportydatagen.convert_to_csv import check_file_type
 
 
-def extract_convert_saf_tcx_to_csv(
-        tcx_directory: str = './tcx/',
-        output_file: str =
-        './extracted_metrics/saf_extracted_interval_metrics.csv',
+def saf_extract_metrics_convert_to_csv(
+        sportfile_directory: str,
+        output_file: str,
 ) -> None:
-    """Convert TCX file to CSV file using sports-activities-features."""
+    """Convert TCX/GPX files to CSV file using sports-activities-features."""
     # Create a new dataframe for the extracted metrics
     df_to_save_to = pd.DataFrame(
         columns=[
             'index',
             'filename',
             'activity_type',
             'distance',
@@ -38,27 +37,37 @@
     )
     # Set filename as index
     df_to_save_to = df_to_save_to.set_index('filename')
     # Counter for index
     i = 1
     # Remove first row beacuse it is empty
     df_to_save_to = df_to_save_to.drop(df_to_save_to.index[0])
-    for filename in os.listdir(tcx_directory):
-        """Extract data from a single TCX file using sports_activities_features
+
+    # Extract data from a single TCX file using sports_activities_features
+    TCXFile()
+    GPXFile()
+
+
+    for filename in os.listdir(sportfile_directory):
+        """Extract metrics from sportfile file using sports_activities_features
         :return: pd.DataFrame with metrics"""
 
         # Print progress
         print(filename)
 
-        # Extract data from a single TCX file using sports_activities_features
-        tcx_file = TCXFile()
-        # Extract metrics from TCX file
-        activity_metrics = tcx_file.extract_integral_metrics(
-            tcx_directory + filename,
+        sport_file = check_file_type(filename)
+
+        if sport_file is None:
+            print(f'File {filename} is not TCX or GPX file')
+            return
+
+        activity_metrics = sport_file.extract_integral_metrics(
+            sportfile_directory + filename,
         )
+
         # Add index to dictionary
         activity_metrics['index'] = i
         # Add filename to dictionary
         activity_metrics['filename'] = filename
 
         # Pandas concat dictionary to empty dataframe
         row_to_append = pd.DataFrame([activity_metrics]).round(2)
@@ -70,16 +79,20 @@
     # Save to csv
     df_to_save_to.to_csv(
         Path(output_file),
         sep=';',
         na_rep='NULL',
         index=False,
     )
-    # Drop rows with all null values
-    df_to_save_to = df_to_save_to.dropna(axis=0)
+    # Drop rows with any null values, ignore activity_type column
+    df_to_save_to = df_to_save_to.dropna(
+            subset=df_to_save_to.columns.difference(['activity_type',
+                                                     'steps']),
+            how='any',
+            axis=0)
     # Replace output file with no null values
     output_file = output_file.replace('.csv', '_no_null.csv')
     # Save new csv with no null values
     df_to_save_to.to_csv(
         Path(output_file),
         sep=';',
         na_rep='NULL',
```

### Comparing `sportydatagen-0.1.0/setup.py` & `sportydatagen-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['niapy>=2.0.5,<3.0.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas',
  'sport-activities-features>=0.3.11,<0.4.0']
 
 setup_kwargs = {
     'name': 'sportydatagen',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Sports activity generator module',
-    'long_description': '# SportyDataGen -- Generator of Endurance Sports Activity Collections (datasets)\n\n## About\n\nSportyDataGen Library is a Python library designed to work with sport GPX and TCX files. It allows users to easily convert these file types into CSV format, extract feature data, and return random data based on specified conditions.\n\nIt aims to help researchers to create datasets for machine learning and data mining applications.\n\n## Features\n* Conversion of GPX and TCX files to CSV format\n* Extraction of feature data from sport files, including GPS coordinates, ascent, heart rate, distance and more\n* Merge of multiple csv files into a single dataset\n* Random selection of data based on the number of rows, percentage of rows in a file or custom conditions\n* Integration with Python scripts to provide an efficient data processing pipeline\n\n## Reference Papers:\n\nIdeas are based on the following research papers:\n\n[1] Fister, I., Jr.; Vrbančič, G.; Brezočnik, L.; Podgorelec, V.; Fister, I. [SportyDataGen: An Online Generator of Endurance Sports Activity Collections](https://www.iztok-jr-fister.eu/static/publications/225.pdf). In Proceedings of the Central European Conference on Information and Intelligent Systems, Varaždin, Croatia, 19–21 September 2018; pp. 171–178.\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n\n',
+    'long_description': '# SportyDataGen -- Generator of Endurance Sports Activity Collections (datasets)\n\n## About\n\nSportyDataGen Library is a Python library designed to work with sport GPX and TCX files. It allows users to easily convert these file types into CSV format, extract feature data, and return random data based on specified conditions.\n\nIt aims to help researchers to create datasets for machine learning and data mining applications.\n\n## Features\n* Conversion of GPX and TCX files to CSV format\n* Extraction of feature data from sport files, including GPS coordinates, ascent, heart rate, distance and more\n* Merge of multiple csv files into a single dataset\n* Random selection of data based on the number of rows, percentage of rows in a file or custom conditions\n* Integration with Python scripts to provide an efficient data processing pipeline\n\n## Reference Papers:\n\nIdeas are based on the following research papers:\n\n[1] Fister, I., Jr.; Vrbančič, G.; Brezočnik, L.; Podgorelec, V.; Fister, I. [SportyDataGen: An Online Generator of Endurance Sports Activity Collections](https://www.iztok-jr-fister.eu/static/publications/225.pdf). In Proceedings of the Central European Conference on Information and Intelligent Systems, Varaždin, Croatia, 19–21 September 2018; pp. 171–178.\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
     'author': 'Rok Kukovec',
     'author_email': 'rok.kukovec1@student.um.si',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/firefly-cpp/sportydatagen',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sportydatagen-0.1.0/PKG-INFO` & `sportydatagen-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sportydatagen
-Version: 0.1.0
+Version: 0.2.0
 Summary: Sports activity generator module
 Home-page: https://gitlab.com/firefly-cpp/sportydatagen
 License: MIT
 Keywords: artificial sport trainer,computational intelligence,data mining,sport activities,tcx
 Author: Rok Kukovec
 Author-email: rok.kukovec1@student.um.si
 Requires-Python: >=3.11,<4.0
@@ -42,8 +42,7 @@
 
 This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
 
 ## Disclaimer
 
 This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
 
-
```

