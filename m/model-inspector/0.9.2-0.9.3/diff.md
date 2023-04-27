# Comparing `tmp/model_inspector-0.9.2.tar.gz` & `tmp/model_inspector-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_inspector-0.9.2.tar", last modified: Sun Mar  7 23:02:31 2021, max compression
+gzip compressed data, was "model_inspector-0.9.3.tar", last modified: Thu Mar 11 03:30:05 2021, max compression
```

## Comparing `model_inspector-0.9.2.tar` & `model_inspector-0.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gGandenberger   (503) staff       (20)        0 2021-03-07 23:02:31.457630 model_inspector-0.9.2/
--rw-r--r--   0 gGandenberger   (503) staff       (20)     2348 2020-10-13 02:39:48.000000 model_inspector-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 gGandenberger   (503) staff       (20)    11357 2020-10-13 02:39:48.000000 model_inspector-0.9.2/LICENSE
--rw-r--r--   0 gGandenberger   (503) staff       (20)      111 2020-10-13 02:39:48.000000 model_inspector-0.9.2/MANIFEST.in
--rw-r--r--   0 gGandenberger   (503) staff       (20)      956 2021-03-07 23:02:31.457159 model_inspector-0.9.2/PKG-INFO
--rw-r--r--   0 gGandenberger   (503) staff       (20)      157 2021-03-07 23:00:58.000000 model_inspector-0.9.2/README.md
-drwxr-xr-x   0 gGandenberger   (503) staff       (20)        0 2021-03-07 23:02:31.451727 model_inspector-0.9.2/model_inspector/
--rw-r--r--   0 gGandenberger   (503) staff       (20)       22 2021-03-07 23:00:57.000000 model_inspector-0.9.2/model_inspector/__init__.py
--rw-r--r--   0 gGandenberger   (503) staff       (20)     1023 2021-03-07 23:00:57.000000 model_inspector-0.9.2/model_inspector/_nbdev.py
--rw-r--r--   0 gGandenberger   (503) staff       (20)    16056 2021-03-07 23:00:57.000000 model_inspector-0.9.2/model_inspector/inspect.py
--rw-r--r--   0 gGandenberger   (503) staff       (20)     2906 2021-03-07 23:00:57.000000 model_inspector-0.9.2/model_inspector/tune.py
-drwxr-xr-x   0 gGandenberger   (503) staff       (20)        0 2021-03-07 23:02:31.456443 model_inspector-0.9.2/model_inspector.egg-info/
--rw-r--r--   0 gGandenberger   (503) staff       (20)      956 2021-03-07 23:02:31.000000 model_inspector-0.9.2/model_inspector.egg-info/PKG-INFO
--rw-r--r--   0 gGandenberger   (503) staff       (20)      446 2021-03-07 23:02:31.000000 model_inspector-0.9.2/model_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 gGandenberger   (503) staff       (20)        1 2021-03-07 23:02:31.000000 model_inspector-0.9.2/model_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 gGandenberger   (503) staff       (20)       20 2021-03-07 23:02:31.000000 model_inspector-0.9.2/model_inspector.egg-info/entry_points.txt
--rw-r--r--   0 gGandenberger   (503) staff       (20)        1 2020-10-14 03:02:29.000000 model_inspector-0.9.2/model_inspector.egg-info/not-zip-safe
--rw-r--r--   0 gGandenberger   (503) staff       (20)       74 2021-03-07 23:02:31.000000 model_inspector-0.9.2/model_inspector.egg-info/requires.txt
--rw-r--r--   0 gGandenberger   (503) staff       (20)       16 2021-03-07 23:02:31.000000 model_inspector-0.9.2/model_inspector.egg-info/top_level.txt
--rw-r--r--   0 gGandenberger   (503) staff       (20)     2288 2021-03-07 23:00:50.000000 model_inspector-0.9.2/settings.ini
--rw-r--r--   0 gGandenberger   (503) staff       (20)       38 2021-03-07 23:02:31.457769 model_inspector-0.9.2/setup.cfg
--rw-r--r--   0 gGandenberger   (503) staff       (20)     1921 2020-10-13 02:39:48.000000 model_inspector-0.9.2/setup.py
+drwxr-xr-x   0 gGandenberger   (503) staff       (20)        0 2021-03-11 03:30:05.432926 model_inspector-0.9.3/
+-rw-r--r--   0 gGandenberger   (503) staff       (20)     2348 2020-10-13 02:39:48.000000 model_inspector-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 gGandenberger   (503) staff       (20)    11357 2020-10-13 02:39:48.000000 model_inspector-0.9.3/LICENSE
+-rw-r--r--   0 gGandenberger   (503) staff       (20)      111 2020-10-13 02:39:48.000000 model_inspector-0.9.3/MANIFEST.in
+-rw-r--r--   0 gGandenberger   (503) staff       (20)      956 2021-03-11 03:30:05.432485 model_inspector-0.9.3/PKG-INFO
+-rw-r--r--   0 gGandenberger   (503) staff       (20)      157 2021-03-11 03:27:07.000000 model_inspector-0.9.3/README.md
+drwxr-xr-x   0 gGandenberger   (503) staff       (20)        0 2021-03-11 03:30:05.427724 model_inspector-0.9.3/model_inspector/
+-rw-r--r--   0 gGandenberger   (503) staff       (20)       22 2021-03-11 03:27:01.000000 model_inspector-0.9.3/model_inspector/__init__.py
+-rw-r--r--   0 gGandenberger   (503) staff       (20)     1077 2021-03-11 03:27:01.000000 model_inspector-0.9.3/model_inspector/_nbdev.py
+-rw-r--r--   0 gGandenberger   (503) staff       (20)    17764 2021-03-11 03:27:01.000000 model_inspector-0.9.3/model_inspector/inspect.py
+-rw-r--r--   0 gGandenberger   (503) staff       (20)     2906 2021-03-11 03:27:01.000000 model_inspector-0.9.3/model_inspector/tune.py
+drwxr-xr-x   0 gGandenberger   (503) staff       (20)        0 2021-03-11 03:30:05.431751 model_inspector-0.9.3/model_inspector.egg-info/
+-rw-r--r--   0 gGandenberger   (503) staff       (20)      956 2021-03-11 03:30:05.000000 model_inspector-0.9.3/model_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 gGandenberger   (503) staff       (20)      446 2021-03-11 03:30:05.000000 model_inspector-0.9.3/model_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 gGandenberger   (503) staff       (20)        1 2021-03-11 03:30:05.000000 model_inspector-0.9.3/model_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 gGandenberger   (503) staff       (20)       20 2021-03-11 03:30:05.000000 model_inspector-0.9.3/model_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 gGandenberger   (503) staff       (20)        1 2020-10-14 03:02:29.000000 model_inspector-0.9.3/model_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 gGandenberger   (503) staff       (20)       90 2021-03-11 03:30:05.000000 model_inspector-0.9.3/model_inspector.egg-info/requires.txt
+-rw-r--r--   0 gGandenberger   (503) staff       (20)       16 2021-03-11 03:30:05.000000 model_inspector-0.9.3/model_inspector.egg-info/top_level.txt
+-rw-r--r--   0 gGandenberger   (503) staff       (20)     2304 2021-03-11 02:53:46.000000 model_inspector-0.9.3/settings.ini
+-rw-r--r--   0 gGandenberger   (503) staff       (20)       38 2021-03-11 03:30:05.433050 model_inspector-0.9.3/setup.cfg
+-rw-r--r--   0 gGandenberger   (503) staff       (20)     1921 2020-10-13 02:39:48.000000 model_inspector-0.9.3/setup.py
```

### Comparing `model_inspector-0.9.2/CONTRIBUTING.md` & `model_inspector-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `model_inspector-0.9.2/LICENSE` & `model_inspector-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `model_inspector-0.9.2/PKG-INFO` & `model_inspector-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_inspector
-Version: 0.9.2
+Version: 0.9.3
 Summary: Inspect machine learning models
 Home-page: https://github.com/gsganden/model_inspector/tree/master/
 Author: Greg Gandenberger
 Author-email: gsganden@gmail.com
 License: Apache Software License 2.0
 Description: # Model Inspector
         > Inspect machine learning models
```

### Comparing `model_inspector-0.9.2/model_inspector/_nbdev.py` & `model_inspector-0.9.3/model_inspector/_nbdev.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # AUTOGENERATED BY NBDEV! DO NOT EDIT!
 
 __all__ = ["index", "modules", "custom_doc_links", "git_url"]
 
 index = {"generate_linear_model_html": "00_inspect.ipynb",
          "generate_logistic_model_html": "00_inspect.ipynb",
+         "plot_linear_waterfall": "00_inspect.ipynb",
          "plot_2d_regression": "00_inspect.ipynb",
          "plot_2d_regression_3d": "00_inspect.ipynb",
          "plot_2d_classification": "00_inspect.ipynb",
          "plot_2d_binary_classification_3d": "00_inspect.ipynb",
          "map_correlation": "00_inspect.ipynb",
          "plot_linear_coefs_vs_hparam": "00_inspect.ipynb",
          "plot_logistic_coefs_vs_hparam": "00_inspect.ipynb",
```

### Comparing `model_inspector-0.9.2/model_inspector/inspect.py` & `model_inspector-0.9.3/model_inspector/inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: 00_inspect.ipynb (unless otherwise specified).
 
-__all__ = ['generate_linear_model_html', 'generate_logistic_model_html', 'plot_2d_regression', 'plot_2d_regression_3d',
-           'plot_2d_classification', 'plot_2d_binary_classification_3d', 'map_correlation',
+__all__ = ['generate_linear_model_html', 'generate_logistic_model_html', 'plot_linear_waterfall', 'plot_2d_regression',
+           'plot_2d_regression_3d', 'plot_2d_classification', 'plot_2d_binary_classification_3d', 'map_correlation',
            'plot_linear_coefs_vs_hparam', 'plot_logistic_coefs_vs_hparam']
 
 # Cell
 from typing import Iterable, Optional, Sequence, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from sklearn.preprocessing import MinMaxScaler
+import waterfall_chart
 
 # Cell
 def generate_linear_model_html(
     model,
     feature_names: Iterable[str],
     target_name: str,
     intercept_formatter: str = ".2f",
@@ -93,14 +94,62 @@
                 <span style='color:green'>{"+" if coef >= 0 else "-"} {abs(coef):{coef_formatter}}</span>
                 * <span style='color:blue'>{feature_col}</span>
             """
         model_string += "</p>"
     return model_string
 
 # Cell
+def plot_linear_waterfall(
+    model,
+    feature_names: Sequence[str],
+    item: Union[pd.Series, np.array],
+    bar_num_formatter: str = ".1f",
+    tick_num_formatter: str = ".2f",
+    sort: bool = True,
+    thresh: Optional[float] = 0.01,
+    rot: float = 30,
+):
+    """Make a waterfall chart for a linear regression prediction.
+
+    This chart shows how the intercept and each feature contribute to
+    the model's prediction on a particular item.
+
+    Parameters:
+    - `model`: fitted scikit-learn linear model of the form
+    `y = b0 + b1 * x1 + ...`.
+    - `feature_names`: feature names in the order in which they were
+    given to the model
+    - `item`: feature values for the item in question
+    - `bar_num_formatter`: Format specifier for numbers in the chart
+    - `tick_num_formatter`: Format specifier for numbers in the chart
+    - `sort`: Whether to sort features by the magnitude of their
+    contribution
+    - `thresh`: Combine as "other" features whose absolute contribution
+    is smaller than this proportion of the total magnitude of the
+    feature contributions.
+    - `rot`: Angle of rotation to apply to xtick labels
+    """
+    index = ["int"] + [
+        f"{name}: {val:{tick_num_formatter}}" for name, val in zip(feature_names, item)
+    ]
+    vals = [model.intercept_] + list(model.coef_ * item)
+    waterfall_chart.plot(
+        index,
+        vals,
+        x_lab="Feature name and value",
+        y_lab="Contribution to prediction",
+        formatting=f"{{:,{bar_num_formatter}}}",
+        sorted_value=sort,
+        threshold=thresh,
+        net_label="pred",
+        rotation_value=rot,
+    )
+    return plt.gca()
+
+# Cell
 def plot_2d_regression(
     model,
     X: pd.DataFrame,
     y: Union[np.array, pd.Series],
     cmap="viridis",
     tick_formatter: str = ".2f",
     ax=None,
```

### Comparing `model_inspector-0.9.2/model_inspector/tune.py` & `model_inspector-0.9.3/model_inspector/tune.py`

 * *Files identical despite different names*

### Comparing `model_inspector-0.9.2/model_inspector.egg-info/PKG-INFO` & `model_inspector-0.9.3/model_inspector.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-inspector
-Version: 0.9.2
+Version: 0.9.3
 Summary: Inspect machine learning models
 Home-page: https://github.com/gsganden/model_inspector/tree/master/
 Author: Greg Gandenberger
 Author-email: gsganden@gmail.com
 License: Apache Software License 2.0
 Description: # Model Inspector
         > Inspect machine learning models
```

### Comparing `model_inspector-0.9.2/settings.ini` & `model_inspector-0.9.3/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 user = gsganden
 description = Inspect machine learning models
 keywords = machine-learning
 author = Greg Gandenberger
 author_email = gsganden@gmail.com
 copyright = Greg Gandenberger
 branch = master
-version = 0.9.2
+version = 0.9.3
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
 status = 2
 
 # Optional. Same format as setuptools requirements
-requirements = IPython matplotlib nb_black nbdev numpy pandas scikit-learn>=0.23 seaborn
+requirements = IPython matplotlib nb_black nbdev numpy pandas scikit-learn>=0.23 seaborn waterfallcharts
 # Optional. Same format as setuptools console_scripts
 # console_scripts = 
 # Optional. Same format as setuptools dependency-links
 # dep_links = 
 
 ###
 # You probably won't need to change anything under here,
```

### Comparing `model_inspector-0.9.2/setup.py` & `model_inspector-0.9.3/setup.py`

 * *Files identical despite different names*

