# Comparing `tmp/vartests-0.2.1.tar.gz` & `tmp/vartests-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vartests-0.2.1.tar", max compression
+gzip compressed data, was "vartests-0.2.2.tar", max compression
```

## Comparing `vartests-0.2.1.tar` & `vartests-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3582 2023-03-29 01:12:16.214555 vartests-0.2.1/README.md
--rw-r--r--   0        0        0      530 2023-03-29 01:14:24.982432 vartests-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      131 2023-03-29 01:12:16.219280 vartests-0.2.1/src/vartests/__init__.py
--rw-r--r--   0        0        0    11666 2023-03-29 01:32:32.094164 vartests-0.2.1/src/vartests/vartests.py
--rw-r--r--   0        0        0       66 2023-03-29 01:14:12.982560 vartests-0.2.1/src/vartests/version.py
--rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 vartests-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3582 2023-04-27 00:55:29.260672 vartests-0.2.2/README.md
+-rw-r--r--   0        0        0      530 2023-04-27 01:06:41.361926 vartests-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-04-27 00:55:29.263511 vartests-0.2.2/src/vartests/__init__.py
+-rw-r--r--   0        0        0    11868 2023-04-27 01:14:22.130791 vartests-0.2.2/src/vartests/vartests.py
+-rw-r--r--   0        0        0       66 2023-04-27 00:59:38.774798 vartests-0.2.2/src/vartests/version.py
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 vartests-0.2.2/PKG-INFO
```

### Comparing `vartests-0.2.1/README.md` & `vartests-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vartests-0.2.1/pyproject.toml` & `vartests-0.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vartests"
-version = "0.2.1"
+version = "0.2.2"
 description = "Statistic tests for Value at Risk (VaR) Models."
 authors = ["Rafael Rodrigues <rafael.rafarod@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rafa-rod/vartests.git"
 
 [tool.poetry.dependencies]
```

### Comparing `vartests-0.2.1/src/vartests/vartests.py` & `vartests-0.2.2/src/vartests/vartests.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,29 +276,32 @@
             answer (dict):           statistics and decision of the test
     """
     if not isinstance(pnl, pd.DataFrame):
         raise ValueError("Input must be dataframe.")
 
     print("Normalizing returns...")
     conditional_vol, conditional_mean = pd.DataFrame(), pd.DataFrame()
-    for t in tqdm(range(pnl.shape[0] - volatility_window + 1)):
+    for t in tqdm(range(pnl.shape[0] - volatility_window)):
         am = arch.arch_model(
             pnl[(t) : (volatility_window + t)],
             vol="GARCH",
             dist="normal",
             rescale=False,
         ).fit(disp="off")
         cond_vol = am.forecast(horizon=1, reindex=False).variance.apply(np.sqrt)
         cond_mean = am.forecast(horizon=1, reindex=False).mean
         conditional_vol = pd.concat([conditional_vol, cond_vol])
         conditional_mean = pd.concat([conditional_mean, cond_mean])
 
-    ret_padr = (pnl.values - conditional_mean.values) / conditional_vol.values
+    #standardized returns with inconditional mean and forecasted condicitional volatility
+    ret_padr = (pnl[volatility_window:].values.flatten() - pnl[volatility_window:].mean().values[0]) / conditional_vol.values.flatten()
 
     zeta = stats.norm.ppf(stats.norm.cdf(ret_padr))
+    zeta[zeta == np.inf] = 0
+    zeta[zeta == -np.inf] = 0
 
     alpha = 1 - var_conf_level
     significance = 1 - conf_level
 
     def objective(x):
         # pars[0] => media
         # pars[1] => vol incondicional
```

### Comparing `vartests-0.2.1/PKG-INFO` & `vartests-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vartests
-Version: 0.2.1
+Version: 0.2.2
 Summary: Statistic tests for Value at Risk (VaR) Models.
 Home-page: https://github.com/rafa-rod/vartests.git
 License: MIT
 Author: Rafael Rodrigues
 Author-email: rafael.rafarod@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vartests Version: 0.2.1 Summary: Statistic tests
+Metadata-Version: 2.1 Name: vartests Version: 0.2.2 Summary: Statistic tests
 for Value at Risk (VaR) Models. Home-page: https://github.com/rafa-rod/
 vartests.git License: MIT Author: Rafael Rodrigues Author-email:
 rafael.rafarod@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: arch
```

