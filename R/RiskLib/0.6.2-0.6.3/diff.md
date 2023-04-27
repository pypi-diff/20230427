# Comparing `tmp/RiskLib-0.6.2.tar.gz` & `tmp/RiskLib-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLib-0.6.2.tar", last modified: Thu Apr 27 20:30:27 2023, max compression
+gzip compressed data, was "RiskLib-0.6.3.tar", last modified: Thu Apr 27 20:55:30 2023, max compression
```

## Comparing `RiskLib-0.6.2.tar` & `RiskLib-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:30:27.146678 RiskLib-0.6.2/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:30:27.146481 RiskLib-0.6.2/PKG-INFO
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:30:27.145039 RiskLib-0.6.2/RiskLib/
--rw-r--r--   0 ma_qh      (501) staff       (20)    16423 2023-04-27 19:06:43.000000 RiskLib-0.6.2/RiskLib/Option.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.2/RiskLib/VaR.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      333 2023-04-27 19:29:52.000000 RiskLib-0.6.2/RiskLib/__init__.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.2/RiskLib/calculation.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.2/RiskLib/cov_matrix.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.2/RiskLib/linear_regression.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      999 2023-04-27 19:11:39.000000 RiskLib-0.6.2/RiskLib/optimal_portfolio.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     8112 2023-04-27 20:29:57.000000 RiskLib-0.6.2/RiskLib/risk_parity.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     5261 2023-04-27 19:31:14.000000 RiskLib-0.6.2/RiskLib/simulation.py
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:30:27.146220 RiskLib-0.6.2/RiskLib.egg-info/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:30:27.000000 RiskLib-0.6.2/RiskLib.egg-info/PKG-INFO
--rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 20:30:27.000000 RiskLib-0.6.2/RiskLib.egg-info/SOURCES.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 20:30:27.000000 RiskLib-0.6.2/RiskLib.egg-info/dependency_links.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 20:30:27.000000 RiskLib-0.6.2/RiskLib.egg-info/requires.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 20:30:27.000000 RiskLib-0.6.2/RiskLib.egg-info/top_level.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 20:30:27.146732 RiskLib-0.6.2/setup.cfg
--rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 20:30:20.000000 RiskLib-0.6.2/setup.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:55:30.634112 RiskLib-0.6.3/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:55:30.633889 RiskLib-0.6.3/PKG-INFO
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:55:30.632375 RiskLib-0.6.3/RiskLib/
+-rw-r--r--   0 ma_qh      (501) staff       (20)    16423 2023-04-27 19:06:43.000000 RiskLib-0.6.3/RiskLib/Option.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.3/RiskLib/VaR.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      333 2023-04-27 19:29:52.000000 RiskLib-0.6.3/RiskLib/__init__.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.3/RiskLib/calculation.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.3/RiskLib/cov_matrix.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.3/RiskLib/linear_regression.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      999 2023-04-27 19:11:39.000000 RiskLib-0.6.3/RiskLib/optimal_portfolio.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     8088 2023-04-27 20:55:07.000000 RiskLib-0.6.3/RiskLib/risk_parity.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5261 2023-04-27 19:31:14.000000 RiskLib-0.6.3/RiskLib/simulation.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 20:55:30.633411 RiskLib-0.6.3/RiskLib.egg-info/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 20:55:30.000000 RiskLib-0.6.3/RiskLib.egg-info/PKG-INFO
+-rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 20:55:30.000000 RiskLib-0.6.3/RiskLib.egg-info/SOURCES.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 20:55:30.000000 RiskLib-0.6.3/RiskLib.egg-info/dependency_links.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 20:55:30.000000 RiskLib-0.6.3/RiskLib.egg-info/requires.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 20:55:30.000000 RiskLib-0.6.3/RiskLib.egg-info/top_level.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 20:55:30.634177 RiskLib-0.6.3/setup.cfg
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 20:55:25.000000 RiskLib-0.6.3/setup.py
```

### Comparing `RiskLib-0.6.2/RiskLib/Option.py` & `RiskLib-0.6.3/RiskLib/Option.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.2/RiskLib/calculation.py` & `RiskLib-0.6.3/RiskLib/calculation.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.2/RiskLib/cov_matrix.py` & `RiskLib-0.6.3/RiskLib/cov_matrix.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.2/RiskLib/linear_regression.py` & `RiskLib-0.6.3/RiskLib/linear_regression.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.2/RiskLib/optimal_portfolio.py` & `RiskLib-0.6.3/RiskLib/optimal_portfolio.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.2/RiskLib/risk_parity.py` & `RiskLib-0.6.3/RiskLib/risk_parity.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,18 +119,18 @@
     attrib = pd.DataFrame(ffReturns * (factorWeights * carinoK[:, np.newaxis]), columns=factors)
     attrib["Alpha"] = residReturn * carinoK
 
     # Set up a DataFrame for output.
     Attribution = pd.DataFrame({"Value": ["TotalReturn", "Return Attribution"]})
 
     
-    newFactors = list(upFfData.columns)
+    newFactors = factors[:]
     newFactors.append('Alpha')
 
-    ss = list(upFfData.columns)
+    ss = factors[:]
     ss.append('Alpha')
     ss.append('Portfolio')
 
     # Loop over the factors
     for s in ss:
         # Total Stock return over the period
         tr = np.exp(np.sum(np.log(upFfData[s] + 1))) - 1
```

### Comparing `RiskLib-0.6.2/RiskLib/simulation.py` & `RiskLib-0.6.3/RiskLib/simulation.py`

 * *Files identical despite different names*

