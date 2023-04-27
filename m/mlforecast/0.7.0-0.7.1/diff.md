# Comparing `tmp/mlforecast-0.7.0.tar.gz` & `tmp/mlforecast-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.7.0.tar", last modified: Tue Apr 11 03:21:28 2023, max compression
+gzip compressed data, was "mlforecast-0.7.1.tar", last modified: Thu Apr 27 04:48:42 2023, max compression
```

## Comparing `mlforecast-0.7.0.tar` & `mlforecast-0.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/
--rw-rw-r--   0 jose      (1000) jose      (1000)     4398 2022-08-24 00:36:43.000000 mlforecast-0.7.0/CONTRIBUTING.md
--rw-rw-r--   0 jose      (1000) jose      (1000)    11336 2022-06-30 02:33:08.000000 mlforecast-0.7.0/LICENSE
--rw-rw-r--   0 jose      (1000) jose      (1000)      111 2022-08-10 00:50:44.000000 mlforecast-0.7.0/MANIFEST.in
--rw-rw-r--   0 jose      (1000) jose      (1000)    12376 2023-04-11 03:21:28.003682 mlforecast-0.7.0/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)    11481 2023-04-11 03:15:06.000000 mlforecast-0.7.0/README.md
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:27.999682 mlforecast-0.7.0/mlforecast/
--rw-rw-r--   0 jose      (1000) jose      (1000)       90 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    28103 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/_modidx.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21383 2023-04-11 03:17:40.000000 mlforecast-0.7.0/mlforecast/core.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/
--rw-rw-r--   0 jose      (1000) jose      (1000)      102 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    25116 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/forecast.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/__init__.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/dask/
--rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/dask/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      714 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/dask/lgb.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      527 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/dask/xgb.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/ray/
--rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/ray/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      450 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/ray/lgb.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      552 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/ray/xgb.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/spark/
--rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/spark/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      836 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/spark/lgb.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      862 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/spark/xgb.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    25498 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/forecast.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     5962 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/grouped_array.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    22132 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/lgb_cv.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     2541 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/target_transforms.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     6309 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:27.999682 mlforecast-0.7.0/mlforecast.egg-info/
--rw-rw-r--   0 jose      (1000) jose      (1000)    12376 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      962 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2022-08-10 00:45:47.000000 mlforecast-0.7.0/mlforecast.egg-info/not-zip-safe
--rw-rw-r--   0 jose      (1000) jose      (1000)      304 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/top_level.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)     1043 2023-04-11 03:17:57.000000 mlforecast-0.7.0/settings.ini
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2023-04-11 03:21:28.003682 mlforecast-0.7.0/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)     2613 2023-03-31 03:20:59.000000 mlforecast-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.589441 mlforecast-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-27 04:48:31.000000 mlforecast-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-27 04:48:31.000000 mlforecast-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 04:48:31.000000 mlforecast-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-27 04:48:42.589441 mlforecast-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-04-27 04:48:31.000000 mlforecast-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.585441 mlforecast-0.7.1/mlforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28756 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.585441 mlforecast-0.7.1/mlforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.585441 mlforecast-0.7.1/mlforecast/distributed/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.585441 mlforecast-0.7.1/mlforecast/distributed/models/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/dask/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/dask/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.585441 mlforecast-0.7.1/mlforecast/distributed/models/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/ray/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/ray/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.589441 mlforecast-0.7.1/mlforecast/distributed/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/spark/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/distributed/models/spark/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/lgb_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-04-27 04:48:31.000000 mlforecast-0.7.1/mlforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:48:42.585441 mlforecast-0.7.1/mlforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-27 04:48:42.000000 mlforecast-0.7.1/mlforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-27 04:48:42.000000 mlforecast-0.7.1/mlforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 04:48:42.000000 mlforecast-0.7.1/mlforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 04:48:42.000000 mlforecast-0.7.1/mlforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-27 04:48:42.000000 mlforecast-0.7.1/mlforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 04:48:42.000000 mlforecast-0.7.1/mlforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-27 04:48:31.000000 mlforecast-0.7.1/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 04:48:42.589441 mlforecast-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-27 04:48:31.000000 mlforecast-0.7.1/setup.py
```

### Comparing `mlforecast-0.7.0/CONTRIBUTING.md` & `mlforecast-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/LICENSE` & `mlforecast-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/PKG-INFO` & `mlforecast-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.7.0
+Version: 0.7.1
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: distributed
 Provides-Extra: dev
 License-File: LICENSE
 
 Nixtla  
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
- ![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)
+ [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <div align="center">
 
 <center>
```

### Comparing `mlforecast-0.7.0/README.md` & `mlforecast-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Nixtla  
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
- ![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)
+ [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <div align="center">
 
 <center>
```

### Comparing `mlforecast-0.7.0/mlforecast/_modidx.py` & `mlforecast-0.7.1/mlforecast/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                                  'mlforecast.core.TimeSeries._transform': ('core.html#timeseries._transform', 'mlforecast/core.py'),
                                  'mlforecast.core.TimeSeries._update_features': ( 'core.html#timeseries._update_features',
                                                                                   'mlforecast/core.py'),
                                  'mlforecast.core.TimeSeries._update_y': ('core.html#timeseries._update_y', 'mlforecast/core.py'),
                                  'mlforecast.core.TimeSeries.features': ('core.html#timeseries.features', 'mlforecast/core.py'),
                                  'mlforecast.core.TimeSeries.fit_transform': ('core.html#timeseries.fit_transform', 'mlforecast/core.py'),
                                  'mlforecast.core.TimeSeries.predict': ('core.html#timeseries.predict', 'mlforecast/core.py'),
+                                 'mlforecast.core.TimeSeries.update': ('core.html#timeseries.update', 'mlforecast/core.py'),
                                  'mlforecast.core._as_tuple': ('core.html#_as_tuple', 'mlforecast/core.py'),
                                  'mlforecast.core._build_transform_name': ('core.html#_build_transform_name', 'mlforecast/core.py'),
                                  'mlforecast.core._expand_target': ('core.html#_expand_target', 'mlforecast/core.py'),
                                  'mlforecast.core._identity': ('core.html#_identity', 'mlforecast/core.py'),
                                  'mlforecast.core._name_models': ('core.html#_name_models', 'mlforecast/core.py')},
             'mlforecast.distributed.forecast': { 'mlforecast.distributed.forecast.DistributedMLForecast': ( 'distributed.forecast.html#distributedmlforecast',
                                                                                                             'mlforecast/distributed/forecast.py'),
@@ -132,26 +133,30 @@
                                                                                              'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.__repr__': ( 'grouped_array.html#groupedarray.__repr__',
                                                                                               'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.__setitem__': ( 'grouped_array.html#groupedarray.__setitem__',
                                                                                                  'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.append': ( 'grouped_array.html#groupedarray.append',
                                                                                             'mlforecast/grouped_array.py'),
+                                          'mlforecast.grouped_array.GroupedArray.append_several': ( 'grouped_array.html#groupedarray.append_several',
+                                                                                                    'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.expand_target': ( 'grouped_array.html#groupedarray.expand_target',
                                                                                                    'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.from_sorted_df': ( 'grouped_array.html#groupedarray.from_sorted_df',
                                                                                                     'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.restore_difference': ( 'grouped_array.html#groupedarray.restore_difference',
                                                                                                         'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.take_from_groups': ( 'grouped_array.html#groupedarray.take_from_groups',
                                                                                                       'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array.GroupedArray.transform_series': ( 'grouped_array.html#groupedarray.transform_series',
                                                                                                       'mlforecast/grouped_array.py'),
-                                          'mlforecast.grouped_array._append_new': ( 'grouped_array.html#_append_new',
+                                          'mlforecast.grouped_array._append_one': ( 'grouped_array.html#_append_one',
                                                                                     'mlforecast/grouped_array.py'),
+                                          'mlforecast.grouped_array._append_several': ( 'grouped_array.html#_append_several',
+                                                                                        'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._apply_difference': ( 'grouped_array.html#_apply_difference',
                                                                                           'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._diff': ('grouped_array.html#_diff', 'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._expand_target': ( 'grouped_array.html#_expand_target',
                                                                                        'mlforecast/grouped_array.py'),
                                           'mlforecast.grouped_array._restore_difference': ( 'grouped_array.html#_restore_difference',
                                                                                             'mlforecast/grouped_array.py'),
```

### Comparing `mlforecast-0.7.0/mlforecast/core.py` & `mlforecast-0.7.1/mlforecast/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -401,15 +401,16 @@
         return self._transform(
             data, dropna=dropna, max_horizon=max_horizon, return_X_y=return_X_y
         )
 
     def _update_y(self, new: np.ndarray) -> None:
         """Appends the elements of `new` to every time serie.
 
-        These values are used to update the transformations and are stored as predictions."""
+        These values are used to update the transformations and are stored as predictions.
+        """
         if not hasattr(self, "y_pred"):
             self.y_pred = []
         self.y_pred.append(new)
         new_arr = np.asarray(new)
         self.ga = self.ga.append(new_arr)
 
     def _update_features(self) -> pd.DataFrame:
@@ -558,7 +559,34 @@
                 dynamic_dfs,
                 before_predict_callback,
             )
         if self.target_transforms is not None:
             for tfm in self.target_transforms[::-1]:
                 preds = tfm.inverse_transform(preds)
         return preds
+
+    def update(self, df: pd.DataFrame) -> None:
+        """Update the values of the stored series."""
+        df = df.sort_values([self.id_col, self.time_col])
+        new_sizes = df.groupby(self.id_col, observed=True).size()
+        prev_sizes = pd.Series(np.full(self.uids.size, 0), index=self.uids)
+        sizes = new_sizes.add(prev_sizes, fill_value=0)
+        values = df[self.target_col].values
+        new_groups = ~sizes.index.isin(self.uids)
+        self.last_dates = pd.Index(
+            df.groupby(self.id_col, observed=True)[self.time_col]
+            .max()
+            .reindex(sizes.index)
+            .fillna(dict(zip(self.uids, self.last_dates)))
+        ).astype(self.last_dates.dtype)
+        self.uids = sizes.index
+        new_statics = df.iloc[new_sizes.cumsum() - 1].set_index(self.id_col)
+        orig_dtypes = self.static_features.dtypes
+        self.static_features = self.static_features.reindex(self.uids)
+        self.static_features.update(new_statics)
+        self.static_features = self.static_features.astype(orig_dtypes)
+        self.ga = self.ga.append_several(
+            new_sizes=sizes.values.astype(np.int32),
+            new_values=values,
+            new_groups=new_groups,
+        )
+        self._ga = GroupedArray(self.ga.data, self.ga.indptr)
```

### Comparing `mlforecast-0.7.0/mlforecast/distributed/forecast.py` & `mlforecast-0.7.1/mlforecast/distributed/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/distributed/models/dask/lgb.py` & `mlforecast-0.7.1/mlforecast/distributed/models/dask/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/distributed/models/dask/xgb.py` & `mlforecast-0.7.1/mlforecast/distributed/models/dask/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/distributed/models/ray/xgb.py` & `mlforecast-0.7.1/mlforecast/distributed/models/ray/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/distributed/models/spark/lgb.py` & `mlforecast-0.7.1/mlforecast/distributed/models/spark/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/distributed/models/spark/xgb.py` & `mlforecast-0.7.1/mlforecast/distributed/models/spark/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/forecast.py` & `mlforecast-0.7.1/mlforecast/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/grouped_array.py` & `mlforecast-0.7.1/mlforecast/grouped_array.py`

 * *Files 15% similar despite different names*

```diff
@@ -80,30 +80,61 @@
             for k in range(upper, max_horizon):
                 out[n, k] = np.nan
             n += 1
     return out
 
 
 @njit
-def _append_new(
+def _append_one(
     data: np.ndarray, indptr: np.ndarray, new: np.ndarray
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Append each value of new to each group in data formed by indptr."""
     n_series = len(indptr) - 1
     new_data = np.empty(data.size + new.size, dtype=data.dtype)
     new_indptr = indptr.copy()
     new_indptr[1:] += np.arange(1, n_series + 1)
     for i in range(n_series):
         prev_slice = slice(indptr[i], indptr[i + 1])
         new_slice = slice(new_indptr[i], new_indptr[i + 1] - 1)
         new_data[new_slice] = data[prev_slice]
         new_data[new_indptr[i + 1] - 1] = new[i]
     return new_data, new_indptr
 
-# %% ../nbs/grouped_array.ipynb 3
+
+@njit
+def _append_several(
+    data: np.ndarray,
+    indptr: np.ndarray,
+    new_sizes: np.ndarray,
+    new_values: np.ndarray,
+    new_groups: np.ndarray,
+) -> Tuple[np.ndarray, np.ndarray]:
+    new_data = np.empty(data.size + new_values.size, dtype=data.dtype)
+    new_indptr = np.empty(new_sizes.size + 1, dtype=indptr.dtype)
+    new_indptr[0] = 0
+    old_indptr_idx = 0
+    new_vals_idx = 0
+    for i, is_new in enumerate(new_groups):
+        new_size = new_sizes[i]
+        if is_new:
+            old_size = 0
+        else:
+            prev_slice = slice(indptr[old_indptr_idx], indptr[old_indptr_idx + 1])
+            old_indptr_idx += 1
+            old_size = prev_slice.stop - prev_slice.start
+            new_size += old_size
+            new_data[new_indptr[i] : new_indptr[i] + old_size] = data[prev_slice]
+        new_indptr[i + 1] = new_indptr[i] + new_size
+        new_data[new_indptr[i] + old_size : new_indptr[i + 1]] = new_values[
+            new_vals_idx : new_vals_idx + new_sizes[i]
+        ]
+        new_vals_idx += new_sizes[i]
+    return new_data, new_indptr
+
+# %% ../nbs/grouped_array.ipynb 4
 class GroupedArray:
     """Array made up of different groups. Can be thought of (and iterated) as a list of arrays.
 
     All the data is stored in a single 1d array `data`.
     The indices for the group boundaries are stored in another 1d array `indptr`."""
 
     def __init__(self, data: np.ndarray, indptr: np.ndarray):
@@ -157,14 +188,22 @@
         indptr = np.append(0, sizes.cumsum())
         return GroupedArray(data, indptr)
 
     def append(self, new: np.ndarray) -> "GroupedArray":
         """Appends each element of `new` to each existing group. Returns a copy."""
         if new.size != self.ngroups:
             raise ValueError(f"new must be of size {self.ngroups}")
-        new_data, new_indptr = _append_new(self.data, self.indptr, new)
+        new_data, new_indptr = _append_one(self.data, self.indptr, new)
+        return GroupedArray(new_data, new_indptr)
+
+    def append_several(
+        self, new_sizes: np.ndarray, new_values: np.ndarray, new_groups: np.ndarray
+    ) -> "GroupedArray":
+        new_data, new_indptr = _append_several(
+            self.data, self.indptr, new_sizes, new_values, new_groups
+        )
         return GroupedArray(new_data, new_indptr)
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(ndata={self.data.size}, ngroups={self.ngroups})"
         )
```

### Comparing `mlforecast-0.7.0/mlforecast/lgb_cv.py` & `mlforecast-0.7.1/mlforecast/lgb_cv.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,59 +48,37 @@
 
 
 def _update(bst, n):
     for _ in range(n):
         bst.update()
 
 
-def _predict(
-    ts,
-    bst,
-    valid,
-    h,
-    id_col,
-    time_col,
-    dynamic_dfs,
-    before_predict_callback,
-    after_predict_callback,
-):
+def _predict(ts, bst, valid, h, before_predict_callback, after_predict_callback):
+    ex_cols_to_drop = [ts.id_col, ts.time_col, ts.target_col]
+    static_features = ts.static_features.columns.tolist()
+    ex_cols_to_drop.extend(static_features)
+    has_ex = not valid.columns.drop(ex_cols_to_drop).empty
+    dynamic_dfs = (
+        [valid.drop(columns=static_features + [ts.target_col])] if has_ex else None
+    )
     preds = ts.predict(
         {"Booster": bst},
         h,
         dynamic_dfs,
         before_predict_callback,
         after_predict_callback,
     )
-    return valid.merge(preds, on=[id_col, time_col], how="left")
+    return valid.merge(preds, on=[ts.id_col, ts.time_col], how="left")
 
 
 def _update_and_predict(
-    ts,
-    bst,
-    valid,
-    n,
-    h,
-    id_col,
-    time_col,
-    dynamic_dfs,
-    before_predict_callback,
-    after_predict_callback,
+    ts, bst, valid, n, h, before_predict_callback, after_predict_callback
 ):
     _update(bst, n)
-    return _predict(
-        ts,
-        bst,
-        valid,
-        h,
-        id_col,
-        time_col,
-        dynamic_dfs,
-        before_predict_callback,
-        after_predict_callback,
-    )
+    return _predict(ts, bst, valid, h, before_predict_callback, after_predict_callback)
 
 # %% ../nbs/lgb_cv.ipynb 6
 CVResult = Tuple[int, float]
 
 # %% ../nbs/lgb_cv.ipynb 7
 class LightGBMCV:
     def __init__(
@@ -262,87 +240,75 @@
                 keep_last_n,
             )
             ds = lgb.Dataset(
                 prep.drop(columns=[id_col, time_col, target_col]), prep[target_col]
             ).construct()
             bst = lgb.Booster({**self.params, "num_threads": self.bst_threads}, ds)
             bst.predict = partial(bst.predict, num_threads=self.bst_threads)
-            valid = valid.set_index(time_col, append=True)
             self.items.append((ts, bst, valid))
         return self
 
     def _single_threaded_partial_fit(
         self,
         metric_values,
         num_iterations,
-        dynamic_dfs,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
     ):
         for j, (ts, bst, valid) in enumerate(self.items):
             preds = _update_and_predict(
                 ts=ts,
                 bst=bst,
                 valid=valid,
                 n=num_iterations,
                 h=self.window_size,
-                id_col=self.id_col,
-                time_col=self.time_col,
-                dynamic_dfs=dynamic_dfs,
                 before_predict_callback=before_predict_callback,
                 after_predict_callback=after_predict_callback,
             )
             metric_values[j] = self.metric_fn(preds[self.target_col], preds["Booster"])
 
     def _multithreaded_partial_fit(
         self,
         metric_values,
         num_iterations,
-        dynamic_dfs,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
     ):
         with ThreadPoolExecutor(self.num_threads) as executor:
             futures = []
             for ts, bst, valid in self.items:
                 _update(bst, num_iterations)
                 future = executor.submit(
                     _predict,
                     ts=ts,
                     bst=bst,
                     valid=valid,
                     h=self.window_size,
-                    id_col=self.id_col,
-                    time_col=self.time_col,
-                    dynamic_dfs=dynamic_dfs,
                     before_predict_callback=before_predict_callback,
                     after_predict_callback=after_predict_callback,
                 )
                 futures.append(future)
             cv_preds = [f.result() for f in futures]
         metric_values[:] = [
             self.metric_fn(preds[self.target_col], preds["Booster"])
             for preds in cv_preds
         ]
 
     def partial_fit(
         self,
         num_iterations: int,
-        dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
     ) -> float:
         """Train the boosters for some iterations.
 
         Parameters
         ----------
         num_iterations : int
             Number of boosting iterations to run
-        dynamic_dfs : list of pandas DataFrame, optional (default=None)
-            Future values of the dynamic features, e.g. prices.
         before_predict_callback : callable, optional (default=None)
             Function to call on the features before computing the predictions.
                 This function will take the input dataframe that will be passed to the model for predicting and should return a dataframe with the same structure.
                 The series identifier is on the index.
         after_predict_callback : callable, optional (default=None)
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
@@ -354,23 +320,21 @@
             Weighted metric after training for num_iterations.
         """
         metric_values = np.empty(len(self.items))
         if self.num_threads == 1:
             self._single_threaded_partial_fit(
                 metric_values,
                 num_iterations,
-                dynamic_dfs,
                 before_predict_callback,
                 after_predict_callback,
             )
         else:
             self._multithreaded_partial_fit(
                 metric_values,
                 num_iterations,
-                dynamic_dfs,
                 before_predict_callback,
                 after_predict_callback,
             )
         return metric_values @ self.weights
 
     def should_stop(self, hist, early_stopping_evals, early_stopping_pct) -> bool:
         if len(hist) < early_stopping_evals + 1:
@@ -396,15 +360,14 @@
         target_col: str = "y",
         step_size: Optional[int] = None,
         num_iterations: int = 100,
         params: Optional[Dict[str, Any]] = None,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
-        dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         eval_every: int = 10,
         weights: Optional[Sequence[float]] = None,
         metric: Union[str, Callable] = "mape",
         verbose_eval: bool = True,
         early_stopping_evals: int = 2,
         early_stopping_pct: float = 0.01,
         compute_cv_preds: bool = False,
@@ -436,16 +399,14 @@
             Parameters to be passed to the LightGBM Boosters.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
-        dynamic_dfs : list of pandas DataFrame, optional (default=None)
-            Future values of the dynamic features, e.g. prices.
         eval_every : int (default=10)
             Number of boosting iterations to train before evaluating on the whole forecast window.
         weights : sequence of float, optional (default=None)
             Weights to multiply the metric of each window. If None, all windows have the same weight.
         metric : str or callable, default='mape'
             Metric used to assess the performance of the models and perform early stopping.
         verbose_eval : bool
@@ -487,15 +448,15 @@
             keep_last_n=keep_last_n,
             weights=weights,
             metric=metric,
         )
         hist = []
         for i in range(0, num_iterations, eval_every):
             metric_value = self.partial_fit(
-                eval_every, dynamic_dfs, before_predict_callback, after_predict_callback
+                eval_every, before_predict_callback, after_predict_callback
             )
             rounds = eval_every + i
             hist.append((rounds, metric_value))
             if verbose_eval:
                 print(f"[{rounds:,d}] {self.metric_name}: {metric_value:,f}")
             if self.should_stop(hist, early_stopping_evals, early_stopping_pct):
                 print(f"Early stopping at round {rounds:,}")
@@ -513,17 +474,14 @@
                 for ts, bst, valid in self.items:
                     future = executor.submit(
                         _predict,
                         ts=ts,
                         bst=bst,
                         valid=valid,
                         h=self.window_size,
-                        id_col=self.id_col,
-                        time_col=self.time_col,
-                        dynamic_dfs=dynamic_dfs,
                         before_predict_callback=before_predict_callback,
                         after_predict_callback=after_predict_callback,
                     )
                     futures.append(future)
                 self.cv_preds_ = pd.concat(
                     [f.result().assign(window=i) for i, f in enumerate(futures)]
                 )
```

### Comparing `mlforecast-0.7.0/mlforecast/target_transforms.py` & `mlforecast-0.7.1/mlforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast/utils.py` & `mlforecast-0.7.1/mlforecast/utils.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.7.1/mlforecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.7.0
+Version: 0.7.1
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: distributed
 Provides-Extra: dev
 License-File: LICENSE
 
 Nixtla  
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
- ![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)
+ [![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <div align="center">
 
 <center>
```

### Comparing `mlforecast-0.7.0/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.7.1/mlforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.0/settings.ini` & `mlforecast-0.7.1/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.7.0
+version = 0.7.1
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
 requirements = numba pandas scikit-learn window-ops
```

### Comparing `mlforecast-0.7.0/setup.py` & `mlforecast-0.7.1/setup.py`

 * *Files identical despite different names*

