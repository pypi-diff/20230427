# Comparing `tmp/proxiflow-0.1.7.tar.gz` & `tmp/proxiflow-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxiflow-0.1.7.tar", max compression
+gzip compressed data, was "proxiflow-0.1.8.tar", last modified: Thu Apr 27 13:52:33 2023, max compression
```

## Comparing `proxiflow-0.1.7.tar` & `proxiflow-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,40 @@
--rw-r--r--   0        0        0     1069 2023-02-22 10:18:01.514049 proxiflow-0.1.7/LICENSE
--rw-r--r--   0        0        0     3252 2023-03-20 15:00:54.143668 proxiflow-0.1.7/README.md
--rw-r--r--   0        0        0       42 2023-02-22 10:18:01.538979 proxiflow-0.1.7/proxiflow/__init__.py
--rw-r--r--   0        0        0      104 2023-02-22 10:18:01.539066 proxiflow-0.1.7/proxiflow/__main__.py
--rw-r--r--   0        0        0     2177 2023-03-20 15:00:54.145543 proxiflow-0.1.7/proxiflow/cli.py
--rw-r--r--   0        0        0      148 2023-02-22 10:18:01.539283 proxiflow-0.1.7/proxiflow/config/__init__.py
--rw-r--r--   0        0        0     3906 2023-03-20 15:00:54.145854 proxiflow-0.1.7/proxiflow/config/config.py
--rw-r--r--   0        0        0      144 2023-03-20 15:00:54.146055 proxiflow-0.1.7/proxiflow/core/__init__.py
--rw-r--r--   0        0        0     6521 2023-03-20 15:00:54.146366 proxiflow-0.1.7/proxiflow/core/cleaner.py
--rw-r--r--   0        0        0      691 2023-03-20 15:00:54.146563 proxiflow-0.1.7/proxiflow/core/core_utils.py
--rw-r--r--   0        0        0     3935 2023-03-20 15:00:54.146759 proxiflow-0.1.7/proxiflow/core/engineer.py
--rw-r--r--   0        0        0     5570 2023-03-20 15:00:54.147007 proxiflow-0.1.7/proxiflow/core/normalizer.py
--rw-r--r--   0        0        0      177 2023-03-20 15:00:54.147326 proxiflow-0.1.7/proxiflow/utils/__init__.py
--rw-r--r--   0        0        0     1663 2023-03-20 15:00:54.147613 proxiflow-0.1.7/proxiflow/utils/data.py
--rw-r--r--   0        0        0     1362 2023-03-20 15:00:54.147827 proxiflow-0.1.7/proxiflow/utils/errors.py
--rw-r--r--   0        0        0      863 2023-03-20 15:00:54.148120 proxiflow-0.1.7/proxiflow/utils/logger.py
--rw-r--r--   0        0        0     2111 2023-03-20 15:29:56.367227 proxiflow-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 proxiflow-0.1.7/setup.py
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 proxiflow-0.1.7/PKG-INFO
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.143210 proxiflow-0.1.8/
+-rw-r--r--   0 martin     (501) staff       (20)     1069 2023-02-22 10:18:01.000000 proxiflow-0.1.8/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)     5102 2023-04-27 13:52:33.143077 proxiflow-0.1.8/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     4240 2023-04-27 13:51:21.000000 proxiflow-0.1.8/README.md
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.136836 proxiflow-0.1.8/docs/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.137971 proxiflow-0.1.8/docs/source/
+-rw-r--r--   0 martin     (501) staff       (20)     1168 2023-03-20 15:14:57.000000 proxiflow-0.1.8/docs/source/conf.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.138686 proxiflow-0.1.8/proxiflow/
+-rw-r--r--   0 martin     (501) staff       (20)       42 2023-02-22 10:18:01.000000 proxiflow-0.1.8/proxiflow/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      104 2023-04-27 12:49:05.000000 proxiflow-0.1.8/proxiflow/__main__.py
+-rw-r--r--   0 martin     (501) staff       (20)     2177 2023-03-20 15:00:54.000000 proxiflow-0.1.8/proxiflow/cli.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.139782 proxiflow-0.1.8/proxiflow/config/
+-rw-r--r--   0 martin     (501) staff       (20)      148 2023-02-22 10:18:01.000000 proxiflow-0.1.8/proxiflow/config/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     4348 2023-04-27 07:34:23.000000 proxiflow-0.1.8/proxiflow/config/config.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.140938 proxiflow-0.1.8/proxiflow/core/
+-rw-r--r--   0 martin     (501) staff       (20)      144 2023-03-20 15:00:54.000000 proxiflow-0.1.8/proxiflow/core/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     7694 2023-04-27 13:29:24.000000 proxiflow-0.1.8/proxiflow/core/cleaner.py
+-rw-r--r--   0 martin     (501) staff       (20)      691 2023-03-20 15:00:54.000000 proxiflow-0.1.8/proxiflow/core/core_utils.py
+-rw-r--r--   0 martin     (501) staff       (20)     3958 2023-04-27 13:12:50.000000 proxiflow-0.1.8/proxiflow/core/engineer.py
+-rw-r--r--   0 martin     (501) staff       (20)     5723 2023-04-27 08:26:47.000000 proxiflow-0.1.8/proxiflow/core/normalizer.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.141839 proxiflow-0.1.8/proxiflow/utils/
+-rw-r--r--   0 martin     (501) staff       (20)      177 2023-03-20 15:00:54.000000 proxiflow-0.1.8/proxiflow/utils/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1517 2023-04-27 13:29:29.000000 proxiflow-0.1.8/proxiflow/utils/data.py
+-rw-r--r--   0 martin     (501) staff       (20)     1457 2023-04-26 18:55:20.000000 proxiflow-0.1.8/proxiflow/utils/errors.py
+-rw-r--r--   0 martin     (501) staff       (20)      893 2023-04-26 18:46:04.000000 proxiflow-0.1.8/proxiflow/utils/logger.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.139462 proxiflow-0.1.8/proxiflow.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     5102 2023-04-27 13:52:33.000000 proxiflow-0.1.8/proxiflow.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      720 2023-04-27 13:52:33.000000 proxiflow-0.1.8/proxiflow.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-27 13:52:33.000000 proxiflow-0.1.8/proxiflow.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)       53 2023-04-27 13:52:33.000000 proxiflow-0.1.8/proxiflow.egg-info/entry_points.txt
+-rw-r--r--   0 martin     (501) staff       (20)      126 2023-04-27 13:52:33.000000 proxiflow-0.1.8/proxiflow.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       26 2023-04-27 13:52:33.000000 proxiflow-0.1.8/proxiflow.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)     1552 2023-04-27 13:41:06.000000 proxiflow-0.1.8/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)       38 2023-04-27 13:52:33.143242 proxiflow-0.1.8/setup.cfg
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-27 13:52:33.142855 proxiflow-0.1.8/tests/
+-rw-r--r--   0 martin     (501) staff       (20)      114 2023-02-22 10:18:01.000000 proxiflow-0.1.8/tests/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     4903 2023-04-27 11:49:43.000000 proxiflow-0.1.8/tests/test_cleaner.py
+-rw-r--r--   0 martin     (501) staff       (20)     2994 2023-03-20 15:00:54.000000 proxiflow-0.1.8/tests/test_config.py
+-rw-r--r--   0 martin     (501) staff       (20)     2976 2023-04-27 13:17:09.000000 proxiflow-0.1.8/tests/test_engineer.py
+-rw-r--r--   0 martin     (501) staff       (20)     3563 2023-03-20 15:00:54.000000 proxiflow-0.1.8/tests/test_normalizer.py
```

### Comparing `proxiflow-0.1.7/LICENSE` & `proxiflow-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proxiflow-0.1.7/proxiflow/cli.py` & `proxiflow-0.1.8/proxiflow/cli.py`

 * *Files identical despite different names*

### Comparing `proxiflow-0.1.7/proxiflow/config/config.py` & `proxiflow-0.1.8/proxiflow/config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import yaml
-from typing import Dict
+from typing import Dict, Any, cast
 
 
 class Config:
     """
     A class for loading configuration data from a YAML file.
 
     :param file_path: The path to the YAML configuration file.
@@ -11,32 +11,35 @@
     """
 
     def __init__(self, file_path: str):
         self.file_path = file_path
         self.config = self.load_config(file_path)
 
     @staticmethod
-    def load_config(file_path: str) -> Dict:
+    def load_config(file_path: str) -> Dict[str, Any]:
         """
         Load a YAML configuration file from the specified file path.
 
         :param file_path: The path to the YAML configuration file.
         :type file_path: str
 
         :returns: A dictionary containing the configuration values.
         :rtype: Dict
 
         :raises FileNotFoundError: If the specified file path does not exist.
         :raises ValueError: If the specified file is empty or cannot be parsed as YAML.
+        :raises TypeError: If the loaded YAML data is not a dictionary with string keys.
         """
         try:
             with open(file_path, "r") as f:
-                config = yaml.safe_load(f)
+                config = cast(Dict[str, Any], yaml.safe_load(f))
             if config is None:
                 raise ValueError("Config file is empty")
+            if not isinstance(config, dict) or not all(isinstance(k, str) for k in config.keys()):
+                raise TypeError("The loaded YAML data is not a dictionary with string keys")
             return config
         except FileNotFoundError:
             raise FileNotFoundError("Config file not found")
         except yaml.YAMLError as e:
             raise ValueError(f"Error parsing config file: {str(e)}")
 
     @property
@@ -46,70 +49,70 @@
 
         :returns: A string containing the input file type
         :rtype: str
 
         :raises ValueError: If the "input_format" key is not present in the configuration dictionary.
         """
         try:
-            return self.config["input_format"]
+            return cast(str, self.config["input_format"])
         except KeyError:
             raise ValueError("input file format not found in config file")
 
     @property
     def output_format(self) -> str:
         """
         Get the output file format configuration dictionary.
 
         :returns: A string containing the output file type
         :rtype: str
 
         :raises ValueError: If the "output_format" key is not present in the configuration dictionary.
         """
         try:
-            return self.config["output_format"]
+            return cast(str, self.config["output_format"])
         except KeyError:
             raise ValueError("output file format not found in config file")
 
     @property
-    def cleaning_config(self) -> Dict:
+    def cleaning_config(self) -> Dict[str, Any]:
         """
         Get the data cleaning configuration values from the configuration dictionary.
 
         :returns: A dictionary containing the data cleaning configuration values.
         :rtype: Dict
 
         :raises ValueError: If the "data_cleaning" key is not present in the configuration dictionary.
         """
         try:
-            return self.config["data_cleaning"]
+            return cast(Dict[str, Any], self.config["data_cleaning"])
         except KeyError:
             raise ValueError("data_cleaning config not found in config file")
 
     @property
-    def normalization_config(self) -> Dict:
+    def normalization_config(self) -> Dict[str, Any]:
         """
         Get the data normalization configuration values from the configuration dictionary.
 
         :returns: A dictionary containing the data normalization configuration values.
         :rtype: Dict
 
         :raises ValueError: If the "data_normalization" key is not present in the configuration dictionary.
         """
         try:
-            return self.config["data_normalization"]
+            return cast(Dict[str, Any], self.config["data_normalization"])
         except KeyError:
             raise ValueError("data_normalization config not found in config file")
 
     @property
-    def feature_engineering_config(self) -> Dict:
+    def feature_engineering_config(self) -> Dict[str, Any]:
         """
         Get the feature engineering configuration values from the configuration dictionary.
 
         :returns: A dictionary containing the feature engineering configuration values.
         :rtype: Dict
 
         :raises ValueError: If the "feature_engineering" key is not present in the configuration dictionary.
         """
         try:
-            return self.config["feature_engineering"]
+            return cast(Dict[str, Any], self.config["feature_engineering"])
         except KeyError:
             raise ValueError("feature_engineering config not found in config file")
```

### Comparing `proxiflow-0.1.7/proxiflow/core/cleaner.py` & `proxiflow-0.1.8/proxiflow/core/cleaner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import polars as pl
+from sklearn.impute import KNNImputer
 from proxiflow.config import Config
 from proxiflow.utils import generate_trace
 
 
 class Cleaner:
     """
     A class for performing data preprocessing tasks such as cleaning, normalization, and feature engineering.
@@ -50,14 +51,22 @@
             try:
                 cleaned_df = self._mean_missing(cleaned_df)
             except Exception as e:
                 trace = generate_trace(e, self._mean_missing)
                 raise Exception(f"Trying to fill missing values with the mean: {trace}")
             return cleaned_df
 
+        # Fill missing values with KNN Imputer
+        if missing_values["knn"]:
+            try:
+                cleaned_df = self._knn_impute_missing(cleaned_df)
+            except Exception as e:
+                trace = generate_trace(e, self._knn_impute_missing)
+                raise Exception(f"Trying to fill missing values with KNN Imputer: {trace}")
+
         # NOTE: This is currently disabled because it randomly fails with:
         # Fill missing values with the mode of the column.
         # if missing_values["mode"]:
         #     cleaned_df = self.mode_missing(cleaned_df)
         #     return cleaned_df
 
         # Fill outliers with the median of the column
@@ -141,14 +150,35 @@
             if clone_df[col].dtype == pl.Int64 or clone_df[col].dtype == pl.Utf8:
                 mode = clone_df[col].mode()
                 mode_s = clone_df[col].fill_null(value=mode[0])
                 clone_df.replace(col, mode_s)
 
         return clone_df
 
+    def _knn_impute_missing(self, df: pl.DataFrame) -> pl.DataFrame:
+        """
+        Fill missing values using KNN imputation.
+        :param df: The DataFrame to fill missing values in.
+        :type df: polars.DataFrame
+        :returns: The DataFrame with missing values filled.
+        :rtype: polars.DataFrame
+        """
+        clone_df = df.clone()
+        # Convert the DataFrame to numpy array
+        np_df = clone_df.to_numpy()
+
+        # Initialize the KNN Imputer
+        knn_imputer = KNNImputer(n_neighbors=5, weights="uniform")
+        imputed_np_df = knn_imputer.fit_transform(np_df)
+
+        # Convert the imputed numpy array back to polars DataFrame
+        imputed_df = pl.DataFrame(imputed_np_df, schema=clone_df.schema)
+
+        return imputed_df
+
     # Handle outliers with IQR method
     def _handle_outliers(self, df: pl.DataFrame) -> pl.DataFrame:
         """
         Handle outliers in a polars DataFrame by replacing them with median of the
 
         :param df: The DataFrame to handle outliers in.
         :type df: polars.DataFrame
```

### Comparing `proxiflow-0.1.7/proxiflow/core/core_utils.py` & `proxiflow-0.1.8/proxiflow/core/core_utils.py`

 * *Files identical despite different names*

### Comparing `proxiflow-0.1.7/proxiflow/core/engineer.py` & `proxiflow-0.1.8/proxiflow/core/engineer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         """
         Initialize a new Engineer object with the specified configuration.
 
         :param config: A Config object containing the feature engineering configuration values.
         :type config: Config
         """
         self.config = config.feature_engineering_config
+        print(self.config)
 
     def execute(self, df: pl.DataFrame) -> pl.DataFrame:
         """
         Perform feature engineering on the specified DataFrame using the specified configuration.
 
         :param df: The DataFrame to perform feature engineering on.
         :type df: polars.DataFrame
@@ -79,17 +80,19 @@
         :type columns: List[str]
         :param degree: The degree of the polynomial features to create.
         :type degree: int
         :return: The DataFrame with polynomial features.
         :rtype: polars.DataFrame
         """
         clone_df = df.clone()
-        columns = check_columns(clone_df, columns)
-        if len(columns) == 0:
+
+        if not columns:
             return clone_df
+
+        columns = check_columns(clone_df, columns)
         # Add polynomial features for each column
         for col in columns:
             # We can not square root strings
             if clone_df[col].dtype == pl.Int64 or clone_df[col].dtype == pl.Float64:
                 # Create a new column for each degree of the polynomial
                 degrees = range(2, degree + 1)
                 # Use list comprehension to generate the new columns
```

### Comparing `proxiflow-0.1.7/proxiflow/core/normalizer.py` & `proxiflow-0.1.8/proxiflow/core/normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 import polars as pl
 import scipy.stats as stats
 from proxiflow.config import Config
 from proxiflow.utils import generate_trace
 from .core_utils import check_columns
 
+from typing import Dict, Any, List, Union, cast
+
 
 class Normalizer:
     """
     A class for performing data normalizing tasks.
     """
 
     def __init__(self, config: Config):
         """
         Initialize a new Normalizer object with the specified configuration.
 
         :param config: A Config object containing the normalization configuration values.
         :type config: Config
         """
-        self.config = config.normalization_config
+        self.config: Dict[str, Any] = config.normalization_config
 
     def normalize(self, df: pl.DataFrame) -> pl.DataFrame:
         """
         Normalize the specified DataFrame using the specified configuration.
 
         :param df: The DataFrame to normalize.
         :type df: polars.DataFrame
         :return: The normalized DataFrame.
         :rtype: polars.DataFrame
         """
         normalized_df = df.clone()
         # Apply min-max normalization
-        min_max_cols = self.config["min_max"]
+        min_max_cols: List[str] = self.config["min_max"]
         if min_max_cols:
             # Normalize the specified columns
             try:
                 normalized_df = self._min_max_normalize(normalized_df, min_max_cols)
             except Exception as e:
-                trace = generate_trace(e, self._min_max_normalize)
+                trace: str = generate_trace(e, self._min_max_normalize)
                 raise Exception(f"Trying min-max normalization: {trace}")
 
         # Apply z-score normalization
-        z_score_cols = self.config["z_score"]
+        z_score_cols: List[str] = self.config["z_score"]
         if z_score_cols:
             # Normalize the specified columns
             try:
                 normalized_df = self._z_score_normalize(normalized_df, z_score_cols)
             except Exception as e:
                 trace = generate_trace(e, self._z_score_normalize)
                 raise Exception(f"Trying z-score normalization: {trace}")
 
         # Apply log normalization
-        log_cols = self.config["log"]
+        log_cols: List[str] = self.config["log"]
         if log_cols:
             # Normalize the specified columns
             try:
                 normalized_df = self._log_normalize(normalized_df, log_cols)
             except Exception as e:
                 trace = generate_trace(e, self._log_normalize)
                 raise Exception(f"Trying log normalization: {trace}")
 
         return normalized_df
 
-    def _min_max_normalize(self, df: pl.DataFrame, columns: list[str]) -> pl.DataFrame:
+    def _min_max_normalize(self, df: pl.DataFrame, columns: List[str]) -> pl.DataFrame:
         """
         Applies min-max normalization to the specified columns of the given DataFrame.
 
         :param df: The DataFrame to normalize.
         :type df: polars.DataFrame
         :param columns: The columns to normalize.
         :type columns: List[str]
@@ -80,25 +82,25 @@
         # Select the specified columns
         selected_df = clone_df.select(columns)
 
         for col in selected_df.columns:
             # We can not subtract strings, so we only normalize numeric columns
             if clone_df[col].dtype == pl.Int64 or clone_df[col].dtype == pl.Float64:
                 # Get the min and max values of the column
-                min_val = selected_df[col].min()
-                max_val = selected_df[col].max()
+                min_val = cast(Union[int, float], selected_df[col].min())
+                max_val = cast(Union[int, float], selected_df[col].max())
                 if max_val - min_val == 0:
                     raise ValueError(f"Error normalizing min-max column {col}: division by zero")
                 # Normalize the column
                 min_max = (df[col] - min_val) / (max_val - min_val)
                 clone_df.replace(col, min_max)
 
         return clone_df
 
-    def _z_score_normalize(self, df: pl.DataFrame, columns: list[str]) -> pl.DataFrame:
+    def _z_score_normalize(self, df: pl.DataFrame, columns: List[str]) -> pl.DataFrame:
         """
         Applies z-score normalization to the specified columns of the given DataFrame.
 
         :param df: The DataFrame to normalize.
         :type df: polars.DataFrame
         :param columns: The columns to normalize.
         :type columns: List[str]
@@ -118,15 +120,15 @@
                 # Get the values of the column. Filter out None values
                 values = list(filter(lambda x: x is not None, clone_df[col].to_list()))
                 z_score = stats.zscore(values)
                 clone_df.replace(col, pl.Series(z_score))
 
         return clone_df
 
-    def _log_normalize(self, df: pl.DataFrame, columns: list[str]) -> pl.DataFrame:
+    def _log_normalize(self, df: pl.DataFrame, columns: List[str]) -> pl.DataFrame:
         """
         Applies log normalization to the specified columns of the given DataFrame.
 
         :param df: The DataFrame to normalize.
         :type df: polars.DataFrame
         :param columns: The columns to normalize.
         :type columns: List[str]
```

### Comparing `proxiflow-0.1.7/proxiflow/utils/data.py` & `proxiflow-0.1.8/proxiflow/utils/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import polars as pl
+from typing import Optional
 
 
-def load_data(data_file: str, input_file_format: str) -> pl.DataFrame:
+def load_data(data_file: str, input_file_format: str) -> Optional[pl.DataFrame]:
     """
     Load a CSV file and return a polars DataFrame.
 
     :param data_file: The path to the CSV file to load.
     :type data_file: str
 
     :returns: The DataFrame containing the CSV data.
     :rtype: polars.DataFrame
 
     :raises FileNotFoundError: If the specified file path does not exist.
     :raises ValueError: If the specified file is empty or cannot be parsed as a CSV file.
     """
     try:
         if input_file_format == "csv":
-            # Attempt to load the CSV file
             df = pl.read_csv(data_file)
             if df.shape[0] == 0:
                 raise ValueError("Data file is empty")
             return df
+        return None
     except FileNotFoundError:
-        # If the file is not found, raise a FileNotFoundError
         raise FileNotFoundError("Data file not found")
     except Exception as e:
-        # If there is an error loading the CSV file, raise a ValueError with the error message
         raise ValueError(f"Error loading data file: {str(e)}")
 
 
 def write_data(data: pl.DataFrame, output_file: str, output_file_format: str) -> None:
     """
     Writes a given DataFrame to a CSV file.
 
@@ -40,10 +39,10 @@
 
     :returns: None
 
     :raises Exception: If there is an error while writing the data.
     """
     try:
         if output_file_format == "csv":
-            data.write_csv(output_file, sep=",")
+            data.write_csv(file=output_file)
     except Exception as e:
         raise Exception(f"Error writing data to {output_file}: {str(e)}")
```

### Comparing `proxiflow-0.1.7/proxiflow/utils/errors.py` & `proxiflow-0.1.8/proxiflow/utils/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import traceback
 import inspect
 import os
 import sys
+from typing import Callable
+import polars as pl
 
 
-def generate_trace(exception, target_method):
+def generate_trace(exception: Exception, target_method: Callable[..., pl.DataFrame]) -> str:
     """
     Generate a custom error message containing the file name, line number, and error description.
 
     This function walks the traceback and filters out frames originating from external libraries,
     returning an error message with the first frame from the user's codebase.
 
     :param exception: The caught exception object
```

### Comparing `proxiflow-0.1.7/proxiflow/utils/logger.py` & `proxiflow-0.1.8/proxiflow/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 
-def get_logger(name, level=logging.INFO):
+def get_logger(name: str, level: int = logging.INFO) -> logging.Logger:
     """
     Create a logger instance with the specified name and log level.
 
     :param name: The name of the logger instance.
     :type name: str
     :param level: The logging level for the logger instance. Defaults to logging.INFO.
     :type level: int
```

