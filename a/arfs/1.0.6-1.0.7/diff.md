# Comparing `tmp/arfs-1.0.6.tar.gz` & `tmp/arfs-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-1.0.6.tar", last modified: Thu Apr 20 12:50:30 2023, max compression
+gzip compressed data, was "arfs-1.0.7.tar", last modified: Thu Apr 27 11:33:29 2023, max compression
```

## Comparing `arfs-1.0.6.tar` & `arfs-1.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.196236 arfs-1.0.6/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.0.6/LICENSE.md
--rw-rw-rw-   0        0        0    11069 2023-04-20 12:50:30.197235 arfs-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.0.6/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1389 2023-04-20 12:50:30.207234 arfs-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.741232 arfs-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.887245 arfs-1.0.6/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-04-20 12:35:02.000000 arfs-1.0.6/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    87331 2023-01-06 14:55:52.000000 arfs-1.0.6/src/arfs/association.py
--rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.743234 arfs-1.0.6/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.033234 arfs-1.0.6/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.0.6/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.0.6/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.160235 arfs-1.0.6/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    84003 2023-01-06 14:55:53.000000 arfs-1.0.6/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    12730 2023-04-20 12:13:54.000000 arfs-1.0.6/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2627 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    15051 2023-01-06 14:55:49.000000 arfs-1.0.6/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    14766 2023-01-11 17:15:13.000000 arfs-1.0.6/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    22780 2023-01-09 09:22:51.000000 arfs-1.0.6/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.0.6/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    29121 2023-01-11 15:36:18.000000 arfs-1.0.6/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15581 2023-01-06 14:55:50.000000 arfs-1.0.6/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    22356 2023-01-06 15:03:38.000000 arfs-1.0.6/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:29.962233 arfs-1.0.6/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.0.6/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      365 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-20 12:50:29.000000 arfs-1.0.6/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 12:50:30.185234 arfs-1.0.6/tests/
--rw-rw-rw-   0        0        0    10657 2023-01-09 09:22:50.000000 arfs-1.0.6/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19566 2023-01-09 09:22:50.000000 arfs-1.0.6/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.390123 arfs-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-1.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0    11069 2023-04-27 11:33:29.392091 arfs-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10379 2023-01-09 09:31:15.000000 arfs-1.0.7/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1389 2023-04-27 11:33:29.401091 arfs-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.028442 arfs-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.147727 arfs-1.0.7/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-04-21 14:47:13.000000 arfs-1.0.7/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    86574 2023-04-27 11:30:49.000000 arfs-1.0.7/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6677 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.030439 arfs-1.0.7/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.268991 arfs-1.0.7/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-1.0.7/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-1.0.7/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.362636 arfs-1.0.7/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    83997 2023-04-27 11:30:49.000000 arfs-1.0.7/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5393 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    12718 2023-04-27 11:30:47.000000 arfs-1.0.7/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2627 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    15051 2023-01-06 14:55:49.000000 arfs-1.0.7/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    14764 2023-04-27 11:30:48.000000 arfs-1.0.7/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    22780 2023-01-09 09:22:51.000000 arfs-1.0.7/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5784 2023-01-06 14:55:48.000000 arfs-1.0.7/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    29117 2023-04-27 11:30:48.000000 arfs-1.0.7/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15517 2023-04-27 11:30:48.000000 arfs-1.0.7/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    22356 2023-01-06 15:03:38.000000 arfs-1.0.7/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.204252 arfs-1.0.7/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-04-27 11:33:29.000000 arfs-1.0.7/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-1.0.7/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      365 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 11:33:28.000000 arfs-1.0.7/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 11:33:29.381089 arfs-1.0.7/tests/
+-rw-rw-rw-   0        0        0    10657 2023-01-09 09:22:50.000000 arfs-1.0.7/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19566 2023-01-09 09:22:50.000000 arfs-1.0.7/tests/test_featselect.py
```

### Comparing `arfs-1.0.6/LICENSE.md` & `arfs-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/PKG-INFO` & `arfs-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.0.6
+Version: 1.0.7
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.0.6/README.md` & `arfs-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/setup.cfg` & `arfs-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/association.py` & `arfs-1.0.7/src/arfs/association.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,27 +77,31 @@
     -------
     float
         weighted conditional entropy
     """
 
     if sample_weight is None:
         sample_weight = np.ones(len(x))
+    elif np.count_nonzero(sample_weight) == 0:
+        raise ValueError(
+            "All elements in sample_weight are zero. Cannot divide by zero."
+        )
 
     df = pd.DataFrame({"x": x, "y": y, "sample_weight": sample_weight})
-    # df = df.fillna(0)
     tot_weight = df["sample_weight"].sum()
     y_counter = df[["y", "sample_weight"]].groupby("y").sum().to_dict()
     y_counter = y_counter["sample_weight"]
     xy_counter = df[["x", "y", "sample_weight"]].groupby(["x", "y"]).sum().to_dict()
     xy_counter = xy_counter["sample_weight"]
     h_xy = 0.0
     for xy in xy_counter.keys():
-        p_xy = xy_counter[xy] / tot_weight
-        p_y = y_counter[xy[1]] / tot_weight
-        h_xy += p_xy * math.log(p_y / p_xy, math.e)
+        p_xy = xy_counter[xy] / tot_weight if tot_weight != 0 else 0
+        p_y = y_counter[xy[1]] / tot_weight if tot_weight != 0 else 0
+        if p_xy != 0:
+            h_xy += p_xy * math.log(p_y / p_xy, math.e)
     return h_xy
 
 
 def weighted_theils_u(x, y, sample_weight=None, as_frame=False):
     """weighted_theils_u computes the weighted Theil's U statistic between two
     categorical predictors.
 
@@ -118,49 +122,46 @@
         predictor names and value of the Theil's U statistic
     """
 
     if sample_weight is None:
         sample_weight = np.ones(len(x))
 
     df = pd.DataFrame({"x": x, "y": y, "sample_weight": sample_weight})
-    # df = df.fillna(0)
     tot_weight = df["sample_weight"].sum()
     y_counter = df[["y", "sample_weight"]].groupby("y").sum().to_dict()
     y_counter = y_counter["sample_weight"]
     x_counter = df[["x", "sample_weight"]].groupby("x").sum().to_dict()
     x_counter = x_counter["sample_weight"]
     p_x = list(map(lambda n: n / tot_weight, x_counter.values()))
     h_x = ss.entropy(p_x)
     xy_counter = df[["x", "y", "sample_weight"]].groupby(["x", "y"]).sum().to_dict()
     xy_counter = xy_counter["sample_weight"]
     h_xy = 0.0
     for xy in xy_counter.keys():
-        p_xy = xy_counter[xy] / tot_weight
-        p_y = y_counter[xy[1]] / tot_weight
-        h_xy += p_xy * math.log(p_y / p_xy, math.e)
+        p_xy = xy_counter[xy] / tot_weight if tot_weight != 0 else 0
+        p_y = y_counter[xy[1]] / tot_weight if tot_weight != 0 else 0
+        if p_xy != 0:
+            h_xy += p_xy * math.log(p_y / p_xy, math.e)
 
     if h_x == 0:
         return 1.0
     else:
         u = (h_x - h_xy) / h_x
-        if -_PRECISION <= u < 0.0 or 1.0 < u <= 1.0 + _PRECISION:
-            rounded_u = 0.0 if u < 0 else 1.0
+        if abs(u) < _PRECISION or abs(u - 1.0) < _PRECISION:
+            rounded_u = round(u)
             warnings.warn(
                 f"Rounded U = {u} to {rounded_u}. This is probably due to floating point precision issues.",
                 RuntimeWarning,
             )
-            teil_u_val = rounded_u
-        else:
-            teil_u_val = u
+            u = rounded_u
+
     if as_frame:
-        return pd.DataFrame(
-            {"row": x.name, "col": y.name, "val": teil_u_val}, index=[0]
-        )
+        return pd.DataFrame({"row": x.name, "col": y.name, "val": u}, index=[0])
     else:
-        return teil_u_val
+        return u
 
 
 def theils_u_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
     """theils_u_matrix theils_u_matrix computes the weighted Theil's U statistic for
     categorical-categorical association. This is an asymmetric coefficient: U(x,y) != U(y,x)
     U(x, y) means the uncertainty of x given y: value is on the range of [0,1] -
     where 0 means y provides no information about x, and 1 means y provides full information about x
@@ -518,15 +519,15 @@
             (
                 x[safe_mask(x, y == k)],
                 sample_weight[safe_mask(sample_weight, y == k)],
             )
             for k in np.unique(y)
         ]
     else:
-        TypeError(
+        raise TypeError(
             "one of the two series should be categorical/object and the other numerical"
         )
 
     if as_frame:
         x_name = x.name if isinstance(x, pd.Series) else "var"
         y_name = y.name if isinstance(y, pd.Series) else "target"
         v = _weighted_correlation_ratio(*args)[0]
@@ -2138,36 +2139,14 @@
     L = sch.linkage(d, method=method)
     ind = sch.fcluster(L, 0.5 * d.max(), "distance")
     columns = [sq_matrix.columns.tolist()[i] for i in list((np.argsort(ind)))]
     sq_matrix = sq_matrix.reindex(columns, axis=1)
     sq_matrix = sq_matrix.reindex(columns, axis=0)
     return sq_matrix
 
-    """
-    Create a heatmap from a numpy array and two lists of labels.
-
-    Parameters
-    ----------
-    data
-        A 2D numpy array of shape (M, N).
-    row_labels
-        A list or array of length M with the labels for the rows.
-    col_labels
-        A list or array of length N with the labels for the columns.
-    ax
-        A `matplotlib.axes.Axes` instance to which the heatmap is plotted.  If
-        not provided, use current axes or create a new one.  Optional.
-    cbar_kw
-        A dictionary with arguments to `matplotlib.Figure.colorbar`.  Optional.
-    cbarlabel
-        The label for the colorbar.  Optional.
-    **kwargs
-        All other arguments are forwarded to `imshow`.
-    """
-
 
 def heatmap(
     data, row_labels, col_labels, ax=None, cbar_kw=None, cbarlabel="", **kwargs
 ):
     """heatmap Create a heatmap from a numpy array and two lists of labels.
 
     Parameters
@@ -2423,17 +2402,14 @@
     -------
     panel.Column
         the panel object
     """
 
     cmap = cmap if cmap is not None else "coolwarm"
 
-    # if features is None:
-    #     features = list(assoc_mat.columns)
-
     # rename the columns for keeping track of num vs cat columns
     if suffix_dic is not None:
         rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
         assoc_mat = assoc_mat.rename(columns=rename_dic)
         assoc_mat = assoc_mat.rename(index=rename_dic)
 
     if cluster_matrix:
@@ -2449,19 +2425,17 @@
         width=figsize[0],
         toolbar="left",
         colorbar=True,
         cmap=cmap,
         fontsize={"title": 12, "ticks": 12, "minor_ticks": 12},
         xrotation=90,
         invert_xaxis=False,
-        invert_yaxis=True,  # title=title_str,
+        invert_yaxis=True,
         xlabel="",
         ylabel="",
-        # gridstyle={'grid_line_color': 'black', 'grid_line_width': 20},
-        # show_grid=True
     )
     title_str = "**Continuous (con) and Categorical (nom) Associations **"
     sub_title_str = (
         "*Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1. The uncertainty "
         "coefficient is assymmetrical, (approximating how much the elements on the "
         "left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical "
         "correlations (Pearson's) from -1 to 1*"
```

### Comparing `arfs-1.0.6/src/arfs/benchmark.py` & `arfs-1.0.7/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-1.0.7/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/dataset/data/housing.zip` & `arfs-1.0.7/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/feature_selection/__init__.py` & `arfs-1.0.7/src/arfs/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/feature_selection/allrelevant.py` & `arfs-1.0.7/src/arfs/feature_selection/allrelevant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1241,15 +1241,14 @@
         cutoff=4,
         iters=10,
         max_rounds=500,
         delta=0.1,
         silent=True,
         importance="shap",
     ):
-
         self.est = est
         self.cutoff = cutoff
         self.iters = iters
         self.max_rounds = max_rounds
         self.delta = delta
         self.silent = silent
         self.importance = importance
@@ -1811,15 +1810,14 @@
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
 
     """
 
     def __init__(
         self, objective=None, cutoff=1, n_folds=5, n_iter=5, silent=True, rf=False
     ):
-
         self.objective = objective
         self.cutoff = cutoff
         self.n_folds = n_folds
         self.n_iter = n_iter
         self.silent = silent
         self.rf = rf
         self.cv_df = None
@@ -2140,15 +2138,14 @@
     cat_idx = [X.columns.get_loc(col) for col in category_cols]
 
     rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
     i = 0
     for tridx, validx in tqdm(
         rkf.split(X, y), total=rkf.get_n_splits(), desc="Repeated k-fold"
     ):
-
         if weight is not None:
             X_train, y_train, weight_tr = (
                 X.iloc[tridx, :],
                 y.iloc[tridx],
                 weight.iloc[tridx],
             )
             X_val, y_val, weight_val = (
```

### Comparing `arfs-1.0.6/src/arfs/feature_selection/base.py` & `arfs-1.0.7/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/feature_selection/mrmr.py` & `arfs-1.0.7/src/arfs/feature_selection/mrmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,19 +186,17 @@
         selected_features = []
         not_selected_features = features.copy()
         self.ranking_ = pd.Series(
             dtype="float64"
         )  # pd.DataFrame(columns=['var_name', 'mrmr', 'relevancy', 'redundancy'])
         self.redundancy_ = pd.Series(dtype="float64")
         for i in tqdm(range(self.n_features_to_select), disable=not self.show_progress):
-
             score_numerator = relevance.loc[not_selected_features]
 
             if i > 0:
-
                 last_selected_feature = selected_features[-1]
 
                 if self.only_same_domain:
                     not_selected_features_sub = [
                         c
                         for c in not_selected_features
                         if c.split("_")[0] == last_selected_feature.split("_")[0]
@@ -259,15 +257,15 @@
         # (redundancy with NULL is 0 and dividing by zero is INF)
         self.ranking_.iloc[0, 0] = float("Inf")
         self.selected_features_ = selected_features
         self.support_ = np.asarray(
             [x in selected_features for x in self.feature_names_in_]
         )
         self.not_selected_features_ = not_selected_features
-        
+
         return self
 
     def transform(self, X):
         """
         Transform the data, returns a transformed version of `X`.
 
         Parameters
```

### Comparing `arfs-1.0.6/src/arfs/feature_selection/summary.py` & `arfs-1.0.7/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/feature_selection/unsupervised.py` & `arfs-1.0.7/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/feature_selection/variable_importance.py` & `arfs-1.0.7/src/arfs/feature_selection/variable_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,14 @@
     encode=False,
     task="regression",
     n_iterations=10,
     verbose=-1,
     encoder_kwargs=None,
     lgb_kwargs={"objective": "rmse", "zero_as_missing": False},
 ):
-
     if task not in ["regression", "classification", "multiclass"]:
         raise ValueError('Task must be either "classification" or "regression"')
 
     if y is None:
         raise ValueError("No training labels provided.")
 
     if encode:
```

### Comparing `arfs-1.0.6/src/arfs/gbm.py` & `arfs-1.0.7/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/parallel.py` & `arfs-1.0.7/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs/preprocessing.py` & `arfs-1.0.7/src/arfs/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         exclude_cols=None,
         output_dtype=np.float64,
         handle_unknown="use_encoded_value",
         unknown_value=np.nan,
         encoded_missing_value=np.nan,
         return_pandas_categorical=False,
     ):
-
         self.dtype_include = dtype_include
         self.dtype_exclude = dtype_exclude
         self.pattern = pattern
         self.exclude_cols = exclude_cols
         self.output_dtype = output_dtype
         self.handle_unknown = handle_unknown
         self.unknown_value = unknown_value
@@ -457,15 +456,14 @@
         self,
         bin_features="all",
         n_bins=10,
         boost_params=None,
         raw=False,
         task="regression",
     ):
-
         if (boost_params is not None) & (not isinstance(boost_params, dict)):
             raise TypeError("boost_kwargs should be a dictionary")
 
         self.bin_features = bin_features
         self.n_bins = n_bins
         self.boost_params = {}
         self.raw = raw
```

### Comparing `arfs-1.0.6/src/arfs/sampling.py` & `arfs-1.0.7/src/arfs/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,26 +218,18 @@
     weight_cat = weight[cat_features]
     weight_num = weight[np.logical_not(cat_features)]
 
     out = np.zeros((x_n_rows, y_n_rows), dtype=np.float32)
 
     weight_sum = weight.sum()
 
-    X_cat = Z_cat[
-        x_index,
-    ]
-    X_num = Z_num[
-        x_index,
-    ]
-    Y_cat = Z_cat[
-        y_index,
-    ]
-    Y_num = Z_num[
-        y_index,
-    ]
+    X_cat = Z_cat[x_index,]
+    X_num = Z_num[x_index,]
+    Y_cat = Z_cat[y_index,]
+    Y_num = Z_num[y_index,]
 
     # print(X_cat,X_num,Y_cat,Y_num)
 
     for i in range(x_n_rows):
         j_start = i
         if x_n_rows != y_n_rows:
             j_start = 0
```

### Comparing `arfs-1.0.6/src/arfs/utils.py` & `arfs-1.0.7/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/src/arfs.egg-info/PKG-INFO` & `arfs-1.0.7/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 1.0.6
+Version: 1.0.7
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-1.0.6/src/arfs.egg-info/SOURCES.txt` & `arfs-1.0.7/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/tests/test_allrelevant.py` & `arfs-1.0.7/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-1.0.6/tests/test_featselect.py` & `arfs-1.0.7/tests/test_featselect.py`

 * *Files identical despite different names*

