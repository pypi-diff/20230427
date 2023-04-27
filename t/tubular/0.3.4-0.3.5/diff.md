# Comparing `tmp/tubular-0.3.4.tar.gz` & `tmp/tubular-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubular-0.3.4.tar", last modified: Tue Mar 21 16:47:53 2023, max compression
+gzip compressed data, was "tubular-0.3.5.tar", last modified: Thu Apr 27 10:17:30 2023, max compression
```

## Comparing `tubular-0.3.4.tar` & `tubular-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-21 16:47:53.671426 tubular-0.3.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1550 2023-03-21 16:45:20.000000 tubular-0.3.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4335 2023-03-21 16:47:53.671426 tubular-0.3.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3706 2023-03-21 16:45:20.000000 tubular-0.3.4/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-03-21 16:47:53.671426 tubular-0.3.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1457 2023-03-21 16:45:20.000000 tubular-0.3.4/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-21 16:47:53.659426 tubular-0.3.4/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-03-21 16:45:20.000000 tubular-0.3.4/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13610 2023-03-21 16:45:20.000000 tubular-0.3.4/tests/test_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4876 2023-03-21 16:45:20.000000 tubular-0.3.4/tests/test_transformers.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-21 16:47:53.667426 tubular-0.3.4/tubular/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      286 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/_version.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14927 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20028 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/capping.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1985 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/comparison.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    41595 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/dates.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13464 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/imputers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17192 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/mapping.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2002 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/misc.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38818 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/nominal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30363 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/numeric.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6024 2023-03-21 16:45:20.000000 tubular-0.3.4/tubular/strings.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-21 16:47:53.671426 tubular-0.3.4/tubular.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4335 2023-03-21 16:47:53.000000 tubular-0.3.4/tubular.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-03-21 16:47:53.000000 tubular-0.3.4/tubular.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-03-21 16:47:53.000000 tubular-0.3.4/tubular.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2023-03-21 16:47:53.000000 tubular-0.3.4/tubular.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-03-21 16:47:53.000000 tubular-0.3.4/tubular.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.464595 tubular-0.3.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1550 2023-04-27 10:11:36.000000 tubular-0.3.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4335 2023-04-27 10:17:30.464595 tubular-0.3.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3706 2023-04-27 10:11:36.000000 tubular-0.3.5/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-27 10:17:30.464595 tubular-0.3.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1457 2023-04-27 10:11:36.000000 tubular-0.3.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.456595 tubular-0.3.5/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:11:36.000000 tubular-0.3.5/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14672 2023-04-27 10:11:36.000000 tubular-0.3.5/tests/test_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4876 2023-04-27 10:11:36.000000 tubular-0.3.5/tests/test_transformers.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.460595 tubular-0.3.5/tubular/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      286 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/_version.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14927 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20028 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/capping.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1985 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/comparison.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    41786 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/dates.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13464 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/imputers.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17192 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/mapping.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2002 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/misc.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42279 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/nominal.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30363 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/numeric.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6024 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/strings.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.464595 tubular-0.3.5/tubular.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4335 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       40 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/top_level.txt
```

### Comparing `tubular-0.3.4/LICENSE` & `tubular-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/PKG-INFO` & `tubular-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.4
+Version: 0.3.5
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tubular-0.3.4/README.md` & `tubular-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/setup.py` & `tubular-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tests/test_data.py` & `tubular-0.3.5/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,47 @@
     )
 
     df["c"] = df["c"].astype("category")
 
     return df
 
 
+def create_MeanResponseTransformer_test_df_unseen_levels():
+    """Create DataFrame to use in MeanResponseTransformer tests that check correct values are
+    generated when using transform method on data with unseen levels.
+    DataFrame column a is the response, the other columns are categorical columns
+    of types; object, category, int, float, bool.
+
+    """
+    df = pd.DataFrame(
+        {
+            "a": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 3.0],
+            "b": ["a", "b", "c", "d", "e", "f", "g", "h"],
+            "c": ["a", "b", "c", "d", "e", "f", "g", "h"],
+            "d": [1, 2, 3, 4, 5, 6, 7, 8],
+            "e": [1, 2, 3, 4, 5, 6.0, 7, 8],
+            "f": [False, False, False, True, True, True, True, False],
+            "multi_level_response": [
+                "blue",
+                "blue",
+                "yellow",
+                "yellow",
+                "green",
+                "green",
+                "yellow",
+                "blue",
+            ],
+        }
+    )
+
+    df["c"] = df["c"].astype("category")
+
+    return df
+
+
 def create_OrdinalEncoderTransformer_test_df():
     """Create DataFrame to use OrdinalEncoderTransformer tests that correct values are
 
     DataFrame column a is the response, the other columns are categorical columns
     of types; object, category, int, float, bool.
 
     """
```

### Comparing `tubular-0.3.4/tests/test_transformers.py` & `tubular-0.3.5/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/base.py` & `tubular-0.3.5/tubular/base.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/capping.py` & `tubular-0.3.5/tubular/capping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/comparison.py` & `tubular-0.3.5/tubular/comparison.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/dates.py` & `tubular-0.3.5/tubular/dates.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         column_lower,
         column_upper,
         new_column_name,
         drop_cols,
         missing_replacement=None,
         **kwargs,
     ):
-
         if not isinstance(column_lower, str):
             raise TypeError(f"{self.classname()}: column_lower should be a str")
 
         if not isinstance(column_upper, str):
             raise TypeError(f"{self.classname()}: column_upper should be a str")
 
         if not isinstance(new_column_name, str):
@@ -117,15 +116,14 @@
         if not isinstance(row, pd.Series):
             raise TypeError(f"{self.classname()}: row should be a pd.Series")
 
         if (pd.isnull(row[self.columns[0]])) or (pd.isnull(row[self.columns[1]])):
             return self.missing_replacement
 
         else:
-
             if not type(row[self.columns[1]]) in [datetime.date, datetime.datetime]:
                 raise TypeError(
                     f"{self.classname()}: upper column values should be datetime.datetime or datetime.date objects"
                 )
 
             if not type(row[self.columns[0]]) in [datetime.date, datetime.datetime]:
                 raise TypeError(
@@ -201,56 +199,52 @@
         column_lower,
         column_upper,
         new_column_name=None,
         units="D",
         copy=True,
         verbose=False,
     ):
-
         if not type(column_lower) is str:
-
             raise TypeError(f"{self.classname()}: column_lower must be a str")
 
         if not type(column_upper) is str:
-
             raise TypeError(f"{self.classname()}: column_upper must be a str")
 
         columns = [column_lower, column_upper]
 
         accepted_values_units = [
             "Y",
             "M",
             "D",
             "h",
             "m",
             "s",
         ]
 
         if not type(units) is str:
-
             raise TypeError(f"{self.classname()}: units must be a str")
 
         if units not in accepted_values_units:
-
             raise ValueError(
                 f"{self.classname()}: units must be one of {accepted_values_units}, got {units}"
             )
+        if units in ["Y", "M"]:
+            warnings.warn(
+                f"{self.classname()}: Y/M units will be changed or deprecated in a future version, consider using DateDiffLeapYearTransformer or D units instead"
+            )
 
         self.units = units
 
         if new_column_name is not None:
-
             if not type(new_column_name) is str:
-
                 raise TypeError(f"{self.classname()}: new_column_name must be a str")
 
             self.new_column_name = new_column_name
 
         else:
-
             self.new_column_name = f"{column_upper}_{column_lower}_datediff_{units}"
 
         super().__init__(columns=columns, copy=copy, verbose=verbose)
 
         # This attribute is not for use in any method, use 'columns' instead.
         # Here only as a fix to allow string representation of transformer.
         self.column_lower = column_lower
@@ -293,37 +287,30 @@
 
     **kwargs
         Arbitrary keyword arguments passed onto pd.to_datetime().
 
     """
 
     def __init__(self, column, new_column_name, to_datetime_kwargs={}, **kwargs):
-
         if not type(column) is str:
-
             raise TypeError(
                 f"{self.classname()}: column should be a single str giving the column to transform to datetime"
             )
 
         if not type(new_column_name) is str:
-
             raise TypeError(f"{self.classname()}: new_column_name must be a str")
 
         if not type(to_datetime_kwargs) is dict:
-
             raise TypeError(
                 f"{self.classname()}: to_datetime_kwargs should be a dict but got type {type(to_datetime_kwargs)}"
             )
 
         else:
-
             for i, k in enumerate(to_datetime_kwargs.keys()):
-
                 if not type(k) is str:
-
                     raise TypeError(
                         f"{self.classname()}: unexpected type ({type(k)}) for to_datetime_kwargs key in position {i}, must be str"
                     )
 
         self.to_datetime_kwargs = to_datetime_kwargs
         self.new_column_name = new_column_name
 
@@ -405,72 +392,60 @@
         Dictionary of keyword arguments to call the pd.Series.dt method with.
 
     """
 
     def __init__(
         self, new_column_name, pd_method_name, column, pd_method_kwargs={}, **kwargs
     ):
-
         if type(column) is not str:
-
             raise TypeError(
                 f"{self.classname()}: column should be a str but got {type(column)}"
             )
 
         super().__init__(columns=column, **kwargs)
 
         if type(new_column_name) is not str:
-
             raise TypeError(
                 f"{self.classname()}: unexpected type ({type(new_column_name)}) for new_column_name, must be str"
             )
 
         if type(pd_method_name) is not str:
-
             raise TypeError(
                 f"{self.classname()}: unexpected type ({type(pd_method_name)}) for pd_method_name, expecting str"
             )
 
         if type(pd_method_kwargs) is not dict:
-
             raise TypeError(
                 f"{self.classname()}: pd_method_kwargs should be a dict but got type {type(pd_method_kwargs)}"
             )
 
         else:
-
             for i, k in enumerate(pd_method_kwargs.keys()):
-
                 if not type(k) is str:
-
                     raise TypeError(
                         f"{self.classname()}: unexpected type ({type(k)}) for pd_method_kwargs key in position {i}, must be str"
                     )
 
         self.new_column_name = new_column_name
         self.pd_method_name = pd_method_name
         self.pd_method_kwargs = pd_method_kwargs
 
         try:
-
             ser = pd.Series([datetime.datetime(2020, 12, 21)])
             getattr(ser.dt, pd_method_name)
 
         except Exception as err:
-
             raise AttributeError(
                 f"""{self.classname()}: error accessing "dt.{pd_method_name}" method on pd.Series object - pd_method_name should be a pd.Series.dt method"""
             ) from err
 
         if callable(getattr(ser.dt, pd_method_name)):
-
             self._callable = True
 
         else:
-
             self._callable = False
 
         # This attribute is not for use in any method, use 'columns' instead.
         # Here only as a fix to allow string representation of transformer.
         self.column = column
 
     def transform(self, X):
@@ -492,21 +467,19 @@
             running the pd.Series.dt method.
 
         """
 
         X = super().transform(X)
 
         if self._callable:
-
             X[self.new_column_name] = getattr(
                 X[self.columns[0]].dt, self.pd_method_name
             )(**self.pd_method_kwargs)
 
         else:
-
             X[self.new_column_name] = getattr(
                 X[self.columns[0]].dt, self.pd_method_name
             )
 
         return X
 
 
@@ -576,15 +549,14 @@
         column_between,
         column_upper,
         new_column_name,
         lower_inclusive=True,
         upper_inclusive=True,
         **kwargs,
     ):
-
         if type(column_lower) is not str:
             raise TypeError(f"{self.classname()}: column_lower should be str")
 
         if type(column_between) is not str:
             raise TypeError(f"{self.classname()}: column_between should be str")
 
         if type(column_upper) is not str:
@@ -629,41 +601,34 @@
             boolean and indicates if the middle column is between the other 2.
 
         """
 
         X = super().transform(X)
 
         for col in self.columns:
-
             if not pd.api.types.is_datetime64_dtype(X[col]):
-
                 raise TypeError(
                     f"{self.classname()}: {col} should be datetime64[ns] type but got {X[col].dtype}"
                 )
 
         if not (X[self.columns[0]] <= X[self.columns[2]]).all():
-
             warnings.warn(
                 f"{self.classname()}: not all {self.columns[2]} are greater than or equal to {self.columns[0]}"
             )
 
         if self.lower_inclusive:
-
             lower_comparison = X[self.columns[0]] <= X[self.columns[1]]
 
         else:
-
             lower_comparison = X[self.columns[0]] < X[self.columns[1]]
 
         if self.upper_inclusive:
-
             upper_comparison = X[self.columns[1]] <= X[self.columns[2]]
 
         else:
-
             upper_comparison = X[self.columns[1]] < X[self.columns[2]]
 
         X[self.new_column_name] = lower_comparison & upper_comparison
 
         return X
 
 
@@ -739,15 +704,14 @@
     def __init__(
         self,
         columns,
         include=["timeofday", "timeofmonth", "timeofyear", "dayofweek"],
         datetime_mappings={},
         **kwargs,
     ):
-
         if not type(include) is list:
             raise TypeError(f"{self.classname()}: include should be List")
 
         if not type(datetime_mappings) is dict:
             raise TypeError(f"{self.classname()}: datetime_mappings should be Dict")
 
         super().__init__(columns=columns, **kwargs)
@@ -878,15 +842,14 @@
                         set(range(7)) - set(self.dayofweek_mapping.keys()),
                     )
                 )
         else:
             self.dayofweek_mapping = {}
 
     def _map_values(self, value, interval: str):
-
         """
         Method to apply mappings for a specified interval ("timeofday", "timeofmonth", "timeofyear" or "dayofweek")
         from corresponding mapping attribute to a single value.
 
         Parameters
         ----------
         interval : str
@@ -1030,15 +993,14 @@
     def __init__(
         self,
         columns: Union[str, List[str]],
         method: Union[str, List[str]],
         units: Union[str, dict],
         period: Union[int, float, dict, dict] = 2 * np.pi,
     ):
-
         super().__init__(columns, copy=True)
 
         if not isinstance(method, str) and not isinstance(method, list):
             raise TypeError(
                 "{}: method must be a string or list but got {}".format(
                     self.classname(), type(method)
                 )
@@ -1169,15 +1131,14 @@
             Input X with additional columns added, these are named "<method>_<original_column>"
         """
 
         X = super().transform(X)
 
         for column in self.columns:
             if not pd.api.types.is_datetime64_dtype(X[column]):
-
                 raise TypeError(
                     f"{self.classname()} : {column} should be datetime64[ns] type but got {X[column].dtype}"
                 )
             if not isinstance(self.units, dict):
                 column_in_desired_unit = getattr(X[column].dt, self.units)
                 desired_units = self.units
             elif isinstance(self.units, dict):
@@ -1185,15 +1146,14 @@
                 desired_units = self.units[column]
             if not isinstance(self.period, dict):
                 desired_period = self.period
             elif isinstance(self.period, dict):
                 desired_period = self.period[column]
 
             for method in self.method:
-
                 new_column_name = f"{method}_{desired_period}_{desired_units}_{column}"
 
                 X[new_column_name] = getattr(np, method)(
                     column_in_desired_unit * (2.0 * np.pi / desired_period)
                 )
 
         return X
```

### Comparing `tubular-0.3.4/tubular/imputers.py` & `tubular-0.3.5/tubular/imputers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/mapping.py` & `tubular-0.3.5/tubular/mapping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/misc.py` & `tubular-0.3.5/tubular/misc.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/nominal.py` & `tubular-0.3.5/tubular/nominal.py`

 * *Files 4% similar despite different names*

```diff
@@ -474,15 +474,17 @@
     For a continuous or binary response the categorical columns specified will have values
     replaced with the mean response for each category.
 
     For an n > 1 level categorical response, up to n binary responses can be created, which in
     turn can then be used to encode each categorical column specified. This will generate up
     to n * len(columns) new columns, of with names of the form {column}_{response_level}. The
     original columns will be removed from the dataframe. This functionality is controlled using
-    the 'level' parameter.
+    the 'level' parameter. Note that the above only works for a n > 1 level categorical response.
+    Do not use 'level' parameter for a n > 1 level numerical response. In this case, use the standard
+    mean response transformer without the 'level' parameter.
 
     If a categorical variable contains null values these will not be transformed.
 
     The same weights and prior are applied to each response level in the multi-level case.
 
     Parameters
     ----------
@@ -498,14 +500,21 @@
         its statistics to be considered reliable (hence default value of 0 means no regularisation).
 
     level : str, list or None, default = None
         Parameter to control encoding against a multi-level categorical response. For a continuous or
         binary response, leave this as None. In the multi-level case, set to 'all' to encode against every
         response level or provide a list of response levels to encode against.
 
+    unseen_level_handling : str("Mean", "Median", "Lowest" or "Highest) or int/float, default = None
+        Parameter to control the logic for handling unseen levels of the categorical features to encode in
+        data when using transform method. Default value of None will output error when attempting to use transform
+        on data with unseen levels in categorical columns to encode. Set this parameter to one of the options above
+        in order to encode unseen levels in each categorical column with the mean, median etc. of
+        each column. One can also pass an arbitrary int/float value to use for encoding unseen levels.
+
     **kwargs
         Arbitrary keyword arguments passed onto BaseTransformer.init method.
 
     Attributes
     ----------
     columns : str or list
         Categorical columns to encode in the input data.
@@ -533,19 +542,28 @@
         Only created in the multi-level case. A list of the new columns produced by encoded the columns in self.columns
         against multiple response levels, of the form {column}_{level}.
 
     transformer_dict : dict
         Only created in the mutli-level case. A dictionary of the form level : transformer containing the mean response
         transformers for each level to be encoded against.
 
+    unseen_levels_encoding_dict: dict
+        Dict containing the values (based on chosen unseen_level_handling) derived from the encoded columns to use when handling unseen levels in data passed to transform method.
+
 
     """
 
     def __init__(
-        self, columns=None, weights_column=None, prior=0, level=None, **kwargs
+        self,
+        columns=None,
+        weights_column=None,
+        prior=0,
+        level=None,
+        unseen_level_handling=None,
+        **kwargs,
     ):
 
         if weights_column is not None:
 
             if type(weights_column) is not str:
 
                 raise TypeError(f"{self.classname()}: weights_column should be a str")
@@ -560,18 +578,25 @@
         if level:
 
             if not isinstance(level, str) and not isinstance(level, list):
 
                 raise TypeError(
                     f"{self.classname()}: Level should be a NoneType, list or str but got {type(level)}"
                 )
+        if unseen_level_handling:
+            if unseen_level_handling not in ["Mean", "Median", "Lowest", "Highest"]:
+                if not isinstance(unseen_level_handling, (int, float)):
+                    raise ValueError(
+                        f"{self.classname()}: unseen_level_handling should be the option: Mean, Median, Lowest, Highest or an arbitrary int/float value"
+                    )
 
         self.weights_column = weights_column
         self.prior = prior
         self.level = level
+        self.unseen_level_handling = unseen_level_handling
         # TODO: set default prior to None and refactor to only use prior regularisation when it is set?
 
         BaseNominalTransformer.__init__(self, columns=columns, **kwargs)
 
     def _prior_regularisation(self, target_means, cat_freq):
         """Regularise encoding values by pushing encodings of infrequent categories towards the global mean.  If prior is zero this will return target_means unaltered.
 
@@ -694,14 +719,16 @@
             Response variable or target.
 
         """
 
         BaseNominalTransformer.fit(self, X, y)
 
         self.mappings = {}
+        self.unseen_levels_encoding_dict = {}
+        X_temp = X.copy()
 
         if self.level:
 
             if self.level == "all":
 
                 self.response_levels = y.unique()
 
@@ -721,32 +748,61 @@
             mapped_columns = []
 
             for level in self.response_levels:
                 mapping_columns_for_this_level = [
                     column + "_" + level for column in self.columns
                 ]
 
-                X_temp = X.copy()
                 for column in self.columns:
                     X_temp[column + "_" + level] = X[column].copy()
 
                 # keep nans to preserve null check functionality of binary response MRE transformer
                 y_temp = y.apply(lambda x: x == level if not pd.isnull(x) else np.nan)
 
                 self.transformer_dict[level] = self._fit_binary_response(
                     X_temp, y_temp, mapping_columns_for_this_level
                 )
 
                 mapped_columns += mapping_columns_for_this_level
 
             self.mapped_columns = list(set(mapped_columns) - set(self.columns))
+            self.encoded_feature_columns = self.mapped_columns
 
         else:
 
             self._fit_binary_response(X, y, self.columns)
+            self.encoded_feature_columns = self.columns
+
+        if self.unseen_level_handling == "Mean":
+            for c in self.encoded_feature_columns:
+                self.unseen_levels_encoding_dict[c] = (
+                    X_temp[c].map(self.mappings[c]).mean()
+                )
+
+        elif self.unseen_level_handling == "Median":
+            for c in self.encoded_feature_columns:
+                self.unseen_levels_encoding_dict[c] = (
+                    X_temp[c].map(self.mappings[c]).median()
+                )
+
+        elif self.unseen_level_handling == "Lowest":
+            for c in self.encoded_feature_columns:
+                self.unseen_levels_encoding_dict[c] = (
+                    X_temp[c].map(self.mappings[c]).min()
+                )
+
+        elif self.unseen_level_handling == "Highest":
+            for c in self.encoded_feature_columns:
+                self.unseen_levels_encoding_dict[c] = (
+                    X_temp[c].map(self.mappings[c]).max()
+                )
+
+        elif isinstance(self.unseen_level_handling, (int, float)):
+            for c in self.encoded_feature_columns:
+                self.unseen_levels_encoding_dict[c] = float(self.unseen_level_handling)
 
         return self
 
     def transform(self, X):
         """Transform method to apply mean response encoding stored in the mappings attribute to
         each column in the columns attribute.
 
@@ -764,25 +820,34 @@
 
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with levels mapped accoriding to mappings dict.
 
         """
-
         if self.level:
             for response_level in self.response_levels:
                 for column in self.columns:
                     X[column + "_" + response_level] = X[column]
             temp_columns = self.columns
             # Temporarily overwriting self.columns to use BaseMappingTransformMixin
             self.columns = self.mapped_columns
 
-        self.check_mappable_rows(X)
-        X = BaseMappingTransformMixin.transform(self, X)
+        if self.unseen_level_handling:
+            self.check_is_fitted(["mappings"])
+            unseen_indices = {}
+            for c in self.columns:
+                # finding rows with values not in the keys of mappings dictionary
+                unseen_indices[c] = X[~X[c].isin(self.mappings[c].keys())].index
+            X = BaseMappingTransformMixin.transform(self, X)
+            for c in self.columns:
+                X.loc[unseen_indices[c], c] = self.unseen_levels_encoding_dict[c]
+        else:
+            self.check_mappable_rows(X)
+            X = BaseMappingTransformMixin.transform(self, X)
 
         if self.level:
             # Setting self.columns back so that the transformer object is unchanged after transform is called
             self.columns = temp_columns
             X.drop(columns=self.columns, inplace=True)
 
         return X
```

### Comparing `tubular-0.3.4/tubular/numeric.py` & `tubular-0.3.5/tubular/numeric.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular/strings.py` & `tubular-0.3.5/tubular/strings.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.4/tubular.egg-info/PKG-INFO` & `tubular-0.3.5/tubular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.4
+Version: 0.3.5
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

