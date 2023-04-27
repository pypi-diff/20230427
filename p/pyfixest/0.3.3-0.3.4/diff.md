# Comparing `tmp/pyfixest-0.3.3.tar.gz` & `tmp/pyfixest-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.3.3.tar", max compression
+gzip compressed data, was "pyfixest-0.3.4.tar", max compression
```

## Comparing `pyfixest-0.3.3.tar` & `pyfixest-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.3.3/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.3.3/pyfixest/__init__.py
--rw-r--r--   0        0        0     9613 2023-03-21 20:34:46.351334 pyfixest-0.3.3/pyfixest/feols.py
--rw-r--r--   0        0        0    19850 2023-03-29 20:38:16.132175 pyfixest-0.3.3/pyfixest/fixest.py
--rw-r--r--   0        0        0    14183 2023-03-28 21:31:50.654617 pyfixest-0.3.3/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     1089 2023-03-28 21:31:50.660731 pyfixest-0.3.3/pyfixest/utils.py
--rw-r--r--   0        0        0      534 2023-03-28 21:31:50.661844 pyfixest-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1763 2023-03-16 21:08:28.608240 pyfixest-0.3.3/readme.md
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 pyfixest-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.3.4/pyfixest/__init__.py
+-rw-r--r--   0        0        0     9613 2023-03-21 20:34:46.351334 pyfixest-0.3.4/pyfixest/feols.py
+-rw-r--r--   0        0        0    22639 2023-04-01 14:20:37.440084 pyfixest-0.3.4/pyfixest/fixest.py
+-rw-r--r--   0        0        0    14183 2023-03-28 21:31:50.654617 pyfixest-0.3.4/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     1089 2023-03-28 21:31:50.660731 pyfixest-0.3.4/pyfixest/utils.py
+-rw-r--r--   0        0        0      516 2023-04-01 14:31:11.186077 pyfixest-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1763 2023-03-16 21:08:28.608240 pyfixest-0.3.4/readme.md
+-rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 pyfixest-0.3.4/setup.py
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pyfixest-0.3.4/PKG-INFO
```

### Comparing `pyfixest-0.3.3/LICENSE.md` & `pyfixest-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.3.3/pyfixest/feols.py` & `pyfixest-0.3.4/pyfixest/feols.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.3.3/pyfixest/fixest.py` & `pyfixest-0.3.4/pyfixest/fixest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import pyhdfe
 import re
 
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
+from matplotlib import pyplot as plt
+from matplotlib.pyplot import cm
 
-from typing import Any, Union, Dict, Optional
+from typing import Any, Union, Dict, Optional, List, Tuple
 from scipy.stats import norm
 from formulaic import model_matrix
 
-from plotnine import ggplot, aes, geom_errorbar, geom_point, theme_bw, ylab, xlab, geom_hline, position_dodge
-
 from pyfixest.feols import Feols
 from pyfixest.FormulaParser import FixestFormulaParser, _flatten_list
 
 
 class Fixest:
 
     def __init__(self, data: pd.DataFrame) -> None:
@@ -35,26 +34,22 @@
     def _clean_fe(self, fval):
 
         fval_list = fval.split("+")
 
         # find interacted fixed effects via "^"
         interacted_fes = [
             x for x in fval_list if len(x.split('^')) > 1]
-        regular_fes = [x for x in fval_list if len(x.split('^')) == 1]
 
         for x in interacted_fes:
             vars = x.split("^")
             self.data[x] = self.data[vars].apply(lambda x: '^'.join(
                 x.dropna().astype(str)) if x.notna().all() else np.nan, axis=1)
 
-        #for x in regular_fes:
-        #    self.data[x] = self.data[x].astype(str)
-
         fe = self.data[fval_list]
-        # all fes to ints
+        # all fes to factors / categories
         fe = fe.apply(lambda x: pd.factorize(x)[0])
 
         fe_na = fe.isna().any(axis=1)
         fe = fe.to_numpy()
 
         return fe, fe_na
 
@@ -63,28 +58,29 @@
 
         '''
         demean all regressions for a specification of fixed effects
 
         Args:
             fval: A specification of fixed effects. String. E.g. X4 or
                 "X3 + X2"
+            ivars: the interacted variables
+            drop_ref: the reference category for the interacted variables.
         '''
 
         YX_dict = dict()
         na_dict = dict()
 
         if fval != "0":
             fe, fe_na = self._clean_fe(fval)
             fe_na = list(fe_na[fe_na == True])
         else:
             fe = None
             fe_na = None
 
         dict2fe = self.fml_dict2.get(fval)
-        #na_index_dict_fe = self.na_index_dict.get(fval)
 
         # create lookup table with NA index key
         # for each regression, check if lookup table already
         # populated with "demeaned" data for some (or all)
         # variables of the model. if demeaned variable for
         # NA key already exists -> use it. else rerun demeaning
         # algorithm
@@ -111,54 +107,51 @@
 
                 Y, X = model_matrix(fml, self.data)
                 na_index = list(set(range(0, self.data.shape[0])) - set(Y.index))
 
                 if self.ivars is not None:
                     if drop_ref is not None:
                         X = X.drop(drop_ref, axis=1)
-                        
+
                 dep_varnames = list(Y.columns)
                 co_varnames = list(X.columns)
                 var_names = list(dep_varnames) + list(co_varnames)
 
                 if self.ivars is not None:
                     self.icovars = [s for s in co_varnames if s.startswith(
                         ivars[0]) and s.endswith(ivars[1])]
                 else:
-                    self.icovars = None                
-              
+                    self.icovars = None
+
                 Y = Y.to_numpy()
                 X = X.to_numpy()
 
                 # variant 1: if there are fixed effects to be projected out
                 if fe is not None:
                     na_index = (na_index + fe_na)
                     fe2 = np.delete(fe, na_index, axis = 0)
                     # drop intercept
                     X = X[:, 1:]
                     co_varnames.remove("Intercept")
                     var_names.remove("Intercept")
 
-                    print("var_names", var_names)
-
                     # check if variables have already been demeaned
                     Y = np.delete(Y, fe_na, axis = 0)
                     X = np.delete(X, fe_na, axis = 0)
                     YX = np.concatenate([Y,X], axis = 1)
 
                     na_index_str = ','.join(str(x) for x in na_index)
 
                     # check if looked dict has data for na_index
                     if lookup_demeaned_data.get(na_index_str) is not None:
                         # get data out of lookup table: list of [algo, data]
                         algorithm, YX_demeaned_old = lookup_demeaned_data.get(na_index_str)
 
                         # get not yet demeaned covariates
                         var_diff_names = list(set(var_names) - set(YX_demeaned_old.columns))[0]
-                        print("var_diff_names", var_diff_names)
                         var_diff_index = list(var_names).index(var_diff_names)
                         var_diff = YX[:,var_diff_index]
                         if var_diff.ndim == 1:
                             var_diff = var_diff.reshape(len(var_diff), 1)
 
 
                         YX_demean_new = algorithm.residualize(var_diff)
@@ -166,15 +159,14 @@
                         YX_demeaned = pd.DataFrame(YX_demeaned)
 
                         YX_demeaned.columns = list(YX_demeaned_old.columns) + [var_diff_names]
 
 
                     else:
                         # not data demeaned yet for NA combination
-                        #YX = np.concatenate([Y, X], axis=1)
                         algorithm = pyhdfe.create(ids=fe2, residualize_method='map')
                         YX_demeaned = algorithm.residualize(YX)
                         YX_demeaned = pd.DataFrame(YX_demeaned)
                         YX_demeaned.columns = list(dep_varnames) + list(co_varnames)
 
                     lookup_demeaned_data[na_index_str] = [algorithm, YX_demeaned]
 
@@ -233,41 +225,39 @@
         fxst_fml._transform_fml_dict()
 
         self.fml_dict = fxst_fml.fml_dict
         self.var_dict = fxst_fml.var_dict
         self.fml_dict2 = fxst_fml.fml_dict2
         self.ivars = fxst_fml.ivars
 
-        #self._get_na_index()
-
         # get all fixed effects combinations
         fixef_keys = list(self.var_dict.keys())
-        
+
         if self.ivars is not None:
 
             if list(self.ivars.keys())[0] is not None:
                 ref = list(self.ivars.keys())[0]
                 ivars = self.ivars[ref]
                 drop_ref = ivars[0] + "[T." + ref + "]" + ":" + ivars[1]
             else:
                 ivars = self.ivars[None]
                 drop_ref = None
-                
+
             # type checking
             i0_type = self.data[ivars[0]].dtype
             i1_type = self.data[ivars[1]].dtype
             if not i0_type in ['category', "O"]:
                 raise ValueError("Column " + ivars[0] + " is not of type 'O' or 'category', which is required in the first position of i(). Instead it is of type " + i0_type.name + ". If a reference level is set, it is required that the variable in the first position of 'i()' is of type 'O' or 'category'.")
             if not i1_type in ['int64', 'float64', 'int32', 'float32']:
                 raise ValueError("Column " + ivars[1] + " is not of type 'int' or 'float', which is required in the second position of i(). Instead it is of type " + i1_type.name + ". If a reference level is set, iti is required that the variable in the second position of 'i()' is of type 'int' or 'float'.")
 
         else:
             ivars = None
             drop_ref = None
-            
+
 
 
         self.dropped_data_dict = dict()
         self.demeaned_data_dict = dict()
 
         for _, fval in enumerate(fixef_keys):
             self.demeaned_data_dict[fval], self.dropped_data_dict[fval] = self.demean(fval, ivars, drop_ref)
@@ -409,20 +399,24 @@
             print('')
             print('### Fixed-effects:', fe)
             print('Dep. var.:', depvar)
             print('')
             print(df.to_string(index=False))
             print('---')
 
-    def iplot(self, alpha = 0.05):
+    def iplot(self, alpha: float = 0.05, figsize: tuple = (10, 10), yintercept: Union[int, str, None] = None, xintercept: Union[int, str, None] = None, rotate_xticks: int = 0) -> None:
+
         '''
         Plot model coefficients with confidence intervals for variable interactions specified via the `i()` syntax.
 
         Args:
             alpha: float, optional. The significance level for the confidence intervals. Default is 0.05.
+            figsize: tuple, optional. The size of the figure. Default is (10, 10).
+            yintercept: int or str (for a categorical x axis). The value at which to draw a horizontal line.
+            xintercept: int or str (for a categorical y axis). The value at which to draw a vertical line.
 
         Returns:
             None
         '''
 
         ivars = self.icovars
 
@@ -440,59 +434,25 @@
             ivars.remove("Intercept")
 
         df = self.tidy()
 
         df = df[df.coefnames.isin(ivars)]
         models = df.index.unique()
 
-        df_list = []
-
-        for model in models:
-
-            df_model = df.xs(model)
-            coef = df_model["Estimate"].values
-            conf_l = coef - df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
-            conf_u = coef + df_model["Std. Error"].values  * norm.ppf(1 - alpha / 2)
-            coefnames = df_model["coefnames"].values.tolist()
-
-            coefnames = [(i) for string in coefnames for i in re.findall(
-                r'\[T\.([\d\.\-]+)\]', string)]
-
-            if ref is not None:
-                coef = np.append(coef, 0)
-                conf_l = np.append(conf_l, 0)
-                conf_u = np.append(conf_u, 0)
-                coefnames = np.append(coefnames, ref)
-
-            df_dict = {
-                'coef': coef,
-                'conf_l': conf_l,
-                'conf_u': conf_u,
-                'coefnames': coefnames,
-                'model': model
-            }
-
-            df_list.append(pd.DataFrame(df_dict))
-
-        df_all = pd.concat(df_list, axis=0)
-
-        iplot = (
-            ggplot(df_all, aes(x='coefnames', y='coef', color='model', group = 'model')) +
-            geom_point(position = position_dodge(0.5)) +
-            geom_errorbar(aes(x='coefnames', ymin='conf_l', ymax='conf_u'), position = position_dodge(0.5)) +
-            theme_bw() +
-            ylab('Estimate') +
-            xlab(list(self.ivars.values())[0][0]) +
-            geom_hline(yintercept=0, color="blue", linetype="dotted")
+        _coefplot(
+            models = models,
+            figsize = figsize,
+            alpha = alpha,
+            yintercept = yintercept,
+            xintercept = xintercept,
+            df = df,
+            is_iplot = True
         )
 
-
-        return iplot
-
-    def coefplot(self, alpha = 0.05, figsize=(5, 2), yintercept=0, figtitle=None, figtext=None):
+    def coefplot(self, alpha: float = 0.05, figsize: tuple = (5, 2), yintercept: int = 0, figtitle: str = None, figtext: str = None, rotate_xticks: int = 0) -> None:
         '''
         Plot estimation results. The plot() method is only defined for single regressions.
 
         Args:
             alpha (float): the significance level for the confidence intervals. Default is 0.05.
             figsize (tuple): the size of the figure. Default is (5, 2).
             yintercept (float): the value of the y-intercept. Default is 0.
@@ -500,36 +460,124 @@
             figtext (str): the text at the bottom of the figure. Default is None.
 
         Returns:
             None
 
         '''
 
-        n_models = len(self.tidy().index.unique())
+        df = self.tidy()
+        models = df.index.unique()
 
-        if n_models > 1:
-            raise ValueError(
-                "The plot() method is only defined for single regressions.")
+        _coefplot(
+            models = models,
+            figsize = figsize,
+            alpha = alpha,
+            yintercept = yintercept,
+            xintercept = None,
+            df = df,
+            is_iplot = False,
+            rotate_xticks=rotate_xticks
+        )
 
-        df = self.tidy()
-        coef = df["Estimate"].values
-        se = df["Std. Error"].values  * norm.ppf(1 - alpha / 2)
-        coefnames = df["coefnames"].values.tolist()
-
-        plt.figure(figsize=figsize)
-        plt.errorbar(coefnames, coef, yerr=se, fmt='.', capsize=5)
-        plt.ylabel("Estimate")
 
-        if figtitle is not None:
-            plt.title(figtitle)
 
-        if figtext is not None:
-            plt.figtext(0.5, -0.1, figtext, ha='center', fontsize=10)
 
-        if yintercept is not None:
-            plt.axhline(y=yintercept, color='red', linestyle='--')
+def _coefplot(models: List, df: pd.DataFrame, figsize: Tuple[int, int], alpha: float, yintercept: Optional[int] = None,
+              xintercept: Optional[int] = None, is_iplot: bool = False,
+              rotate_xticks: float = 0) -> None:
+    """
+        Plot model coefficients with confidence intervals.
 
-        return plt
+        Args:
+            models (list): A list of fitted models.
+            figsize (tuple): The size of the figure.
+            alpha (float): The significance level for the confidence intervals.
+            yintercept (int or None): The value at which to draw a horizontal line on the plot.
+            xintercept (int or None): The value at which to draw a vertical line on the plot.
+            df (pandas.DataFrame): The dataframe containing the data used for the model fitting.
+            is_iplot (bool): If True, plot variable interactions specified via the `i()` syntax.
+            rotate_xticks (float): The angle in degrees to rotate the xticks labels. Default is 0 (no rotation).
+
+        Returns:
+        None
+    """
 
+    if len(models) > 1:
 
+        fig, ax = plt.subplots(len(models), gridspec_kw={'hspace': 0.5}, figsize=figsize)
+        fig.suptitle("iplot")
+
+        for x, model in enumerate(models):
+
+            df_model = df.xs(model)
+            coef = df_model["Estimate"].values
+            conf_l = coef - df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
+            conf_u = coef + df_model["Std. Error"].values  * norm.ppf(1 - alpha / 2)
+            coefnames = df_model["coefnames"].values.tolist()
+
+            # could be moved out of the for loop, as the same ivars for all
+            # models.
+
+            if is_iplot == True:
+                coefnames = [(i) for string in coefnames for i in re.findall(
+                    r'\[T\.([\d\.\-]+)\]', string)]
+
+            # in the future: add reference category
+            #if ref is not None:
+            #    coef = np.append(coef, 0)
+            #    conf_l = np.append(conf_l, 0)
+            #    conf_u = np.append(conf_u, 0)
+            #    coefnames = np.append(coefnames, ref)
+
+            ax[x].scatter(coefnames,coef, color= "b", alpha = 0.8)
+            ax[x].scatter(coefnames,conf_u, color = "b", alpha = 0.8, marker = "_", s = 100)
+            ax[x].scatter(coefnames,conf_l, color = "b", alpha = 0.8, marker = "_", s = 100)
+            ax[x].vlines(coefnames, ymin=conf_l, ymax=conf_u, color= "b", alpha = 0.8)
+            if yintercept is not None:
+                ax[x].axhline(yintercept, color='red', linestyle='--', alpha = 0.5)
+            if xintercept is not None:
+                ax[x].axvline(xintercept, color='red', linestyle='--', alpha = 0.5)
+            ax[x].set_ylabel('Coefficients')
+            ax[x].set_title(model)
+            ax[x].tick_params(axis='x', rotation=rotate_xticks)
+
+    else:
+
+        fig, ax = plt.subplots(figsize=figsize)
+        fig.suptitle("iplot")
+
+        model = models[0]
+
+        df_model = df.xs(model)
+        coef = df_model["Estimate"].values
+        conf_l = coef - df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
+        conf_u = coef + df_model["Std. Error"].values  * norm.ppf(1 - alpha / 2)
+        coefnames = df_model["coefnames"].values.tolist()
+
+        if is_iplot == True:
+            coefnames = [(i) for string in coefnames for i in re.findall(
+                r'\[T\.([\d\.\-]+)\]', string)]
+
+        # in the future: add reference category
+        #if ref is not None:
+        #    coef = np.append(coef, 0)
+        #    conf_l = np.append(conf_l, 0)
+        #    conf_u = np.append(conf_u, 0)
+        #    coefnames = np.append(coefnames, ref)
+
+                #c = next(color)
+
+        ax.scatter(coefnames,coef, color= "b", alpha = 0.8)
+        ax.scatter(coefnames,conf_u, color = "b", alpha = 0.8, marker = "_", s = 100)
+        ax.scatter(coefnames,conf_l, color = "b", alpha = 0.8, marker = "_", s = 100)
+        ax.vlines(coefnames, ymin=conf_l, ymax=conf_u, color= "b", alpha = 0.8)
+        if yintercept is not None:
+            ax.axhline(yintercept, color='red', linestyle='--', alpha = 0.5)
+        if xintercept is not None:
+            ax.axvline(xintercept, color='red', linestyle='--', alpha = 0.5)
+        ax.set_ylabel('Coefficients')
+        ax.set_title(model)
+        ax.tick_params(axis='x', rotation=rotate_xticks)
 
 
+        plt.show()
+        plt.close()
```

### Comparing `pyfixest-0.3.3/pyfixest/FormulaParser.py` & `pyfixest-0.3.4/pyfixest/FormulaParser.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.3.3/pyfixest/utils.py` & `pyfixest-0.3.4/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.3.3/pyproject.toml` & `pyfixest-0.3.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.3.3"
+version = "0.3.4"
 description = "Draft package for high dimensional fixed effect OLS estimation"
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python=">=3.8,<3.11"
 pandas = "^1.5.1"
 numpy = "^1.2"
 matplotlib = "^3.7"
 PyHDFE = "^0.1.1"
 scipy = "^1.9.0"
 formulaic = "^0.3.0"
 pytest="^7.2.0"
-plotnine="^0.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyfixest-0.3.3/readme.md` & `pyfixest-0.3.4/readme.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.3.3/PKG-INFO` & `pyfixest-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.3.3
+Version: 0.3.4
 Summary: Draft package for high dimensional fixed effect OLS estimation
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyHDFE (>=0.1.1,<0.2.0)
 Requires-Dist: formulaic (>=0.3.0,<0.4.0)
 Requires-Dist: matplotlib (>=3.7,<4.0)
 Requires-Dist: numpy (>=1.2,<2.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
-Requires-Dist: plotnine (>=0.10,<0.11)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## PyFixest
 
 <?xml version="1.0" encoding="UTF-8"?>
```

