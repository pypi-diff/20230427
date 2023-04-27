# Comparing `tmp/RiskLib-0.6.0.tar.gz` & `tmp/RiskLib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLib-0.6.0.tar", last modified: Thu Apr 27 20:23:14 2023, max compression
+gzip compressed data, was "RiskLib-0.6.1.tar", last modified: Thu Apr 27 20:25:47 2023, max compression
```

## Comparing `RiskLib-0.6.0.tar` & `RiskLib-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:23:14.902953 RiskLib-0.6.0/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:23:14.902763 RiskLib-0.6.0/PKG-INFO
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:23:14.901471 RiskLib-0.6.0/RiskLib/
--rw-r--r--   0 ma_qh      (501) staff       (20)    16423 2023-04-27 19:06:43.000000 RiskLib-0.6.0/RiskLib/Option.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.0/RiskLib/VaR.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      333 2023-04-27 19:29:52.000000 RiskLib-0.6.0/RiskLib/__init__.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.0/RiskLib/calculation.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.0/RiskLib/cov_matrix.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.0/RiskLib/linear_regression.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      999 2023-04-27 19:11:39.000000 RiskLib-0.6.0/RiskLib/optimal_portfolio.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     8053 2023-04-27 20:22:43.000000 RiskLib-0.6.0/RiskLib/risk_parity.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     5261 2023-04-27 19:31:14.000000 RiskLib-0.6.0/RiskLib/simulation.py
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:23:14.902544 RiskLib-0.6.0/RiskLib.egg-info/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:23:14.000000 RiskLib-0.6.0/RiskLib.egg-info/PKG-INFO
--rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 20:23:14.000000 RiskLib-0.6.0/RiskLib.egg-info/SOURCES.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 20:23:14.000000 RiskLib-0.6.0/RiskLib.egg-info/dependency_links.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 20:23:14.000000 RiskLib-0.6.0/RiskLib.egg-info/requires.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 20:23:14.000000 RiskLib-0.6.0/RiskLib.egg-info/top_level.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 20:23:14.903005 RiskLib-0.6.0/setup.cfg
--rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 20:22:49.000000 RiskLib-0.6.0/setup.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:25:47.200350 RiskLib-0.6.1/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:25:47.200146 RiskLib-0.6.1/PKG-INFO
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:25:47.199076 RiskLib-0.6.1/RiskLib/
+-rw-r--r--   0 ma_qh      (501) staff       (20)    16423 2023-04-27 19:06:43.000000 RiskLib-0.6.1/RiskLib/Option.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.1/RiskLib/VaR.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      333 2023-04-27 19:29:52.000000 RiskLib-0.6.1/RiskLib/__init__.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.1/RiskLib/calculation.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.1/RiskLib/cov_matrix.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.1/RiskLib/linear_regression.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      999 2023-04-27 19:11:39.000000 RiskLib-0.6.1/RiskLib/optimal_portfolio.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     8051 2023-04-27 20:25:16.000000 RiskLib-0.6.1/RiskLib/risk_parity.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5261 2023-04-27 19:31:14.000000 RiskLib-0.6.1/RiskLib/simulation.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:25:47.199875 RiskLib-0.6.1/RiskLib.egg-info/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:25:47.000000 RiskLib-0.6.1/RiskLib.egg-info/PKG-INFO
+-rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 20:25:47.000000 RiskLib-0.6.1/RiskLib.egg-info/SOURCES.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 20:25:47.000000 RiskLib-0.6.1/RiskLib.egg-info/dependency_links.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 20:25:47.000000 RiskLib-0.6.1/RiskLib.egg-info/requires.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 20:25:47.000000 RiskLib-0.6.1/RiskLib.egg-info/top_level.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 20:25:47.200408 RiskLib-0.6.1/setup.cfg
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 20:25:27.000000 RiskLib-0.6.1/setup.py
```

### Comparing `RiskLib-0.6.0/RiskLib/Option.py` & `RiskLib-0.6.1/RiskLib/Option.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.0/RiskLib/calculation.py` & `RiskLib-0.6.1/RiskLib/calculation.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.0/RiskLib/cov_matrix.py` & `RiskLib-0.6.1/RiskLib/cov_matrix.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.0/RiskLib/linear_regression.py` & `RiskLib-0.6.1/RiskLib/linear_regression.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.0/RiskLib/optimal_portfolio.py` & `RiskLib-0.6.1/RiskLib/optimal_portfolio.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.0/RiskLib/risk_parity.py` & `RiskLib-0.6.1/RiskLib/risk_parity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 from scipy.optimize import minimize
 
-def expost_attribution_1(w, upReturns):
+def expost_attribution(w, upReturns):
     _stocks = list(upReturns.columns)
     n = upReturns.shape[0]
     pReturn = np.empty(n)
     weights = np.empty((n, len(w)))
     lastW = np.copy(w)
     matReturns = upReturns[_stocks].values
```

### Comparing `RiskLib-0.6.0/RiskLib/simulation.py` & `RiskLib-0.6.1/RiskLib/simulation.py`

 * *Files identical despite different names*

