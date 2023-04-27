# Comparing `tmp/RiskLib-0.6.4.tar.gz` & `tmp/RiskLib-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLib-0.6.4.tar", last modified: Thu Apr 27 21:17:29 2023, max compression
+gzip compressed data, was "RiskLib-0.6.5.tar", last modified: Thu Apr 27 21:30:37 2023, max compression
```

## Comparing `RiskLib-0.6.4.tar` & `RiskLib-0.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:17:29.916836 RiskLib-0.6.4/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 21:17:29.916640 RiskLib-0.6.4/PKG-INFO
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:17:29.915532 RiskLib-0.6.4/RiskLib/
--rw-r--r--   0 ma_qh      (501) staff       (20)    16423 2023-04-27 19:06:43.000000 RiskLib-0.6.4/RiskLib/Option.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.4/RiskLib/VaR.py
--rw-r--r--   0 ma_qh      (501) staff       (20)      204 2023-04-27 21:16:35.000000 RiskLib-0.6.4/RiskLib/__init__.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.4/RiskLib/calculation.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.4/RiskLib/cov_matrix.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.4/RiskLib/linear_regression.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     1011 2023-04-27 21:14:16.000000 RiskLib-0.6.4/RiskLib/optimal_portfolio.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     8088 2023-04-27 20:59:27.000000 RiskLib-0.6.4/RiskLib/risk_parity.py
--rw-r--r--   0 ma_qh      (501) staff       (20)     5261 2023-04-27 19:31:14.000000 RiskLib-0.6.4/RiskLib/simulation.py
-drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:17:29.916440 RiskLib-0.6.4/RiskLib.egg-info/
--rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 21:17:29.000000 RiskLib-0.6.4/RiskLib.egg-info/PKG-INFO
--rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 21:17:29.000000 RiskLib-0.6.4/RiskLib.egg-info/SOURCES.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 21:17:29.000000 RiskLib-0.6.4/RiskLib.egg-info/dependency_links.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 21:17:29.000000 RiskLib-0.6.4/RiskLib.egg-info/requires.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 21:17:29.000000 RiskLib-0.6.4/RiskLib.egg-info/top_level.txt
--rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 21:17:29.916894 RiskLib-0.6.4/setup.cfg
--rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 21:16:58.000000 RiskLib-0.6.4/setup.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:30:37.749954 RiskLib-0.6.5/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 21:30:37.749762 RiskLib-0.6.5/PKG-INFO
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:30:37.748590 RiskLib-0.6.5/RiskLib/
+-rw-r--r--   0 ma_qh      (501) staff       (20)    16468 2023-04-27 21:30:12.000000 RiskLib-0.6.5/RiskLib/Option.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      317 2023-04-27 18:51:46.000000 RiskLib-0.6.5/RiskLib/VaR.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)      204 2023-04-27 21:16:35.000000 RiskLib-0.6.5/RiskLib/__init__.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1865 2023-04-27 19:26:45.000000 RiskLib-0.6.5/RiskLib/calculation.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     7874 2023-04-27 18:39:32.000000 RiskLib-0.6.5/RiskLib/cov_matrix.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1534 2023-04-27 18:42:16.000000 RiskLib-0.6.5/RiskLib/linear_regression.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     1011 2023-04-27 21:14:16.000000 RiskLib-0.6.5/RiskLib/optimal_portfolio.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     8088 2023-04-27 20:59:27.000000 RiskLib-0.6.5/RiskLib/risk_parity.py
+-rw-r--r--   0 ma_qh      (501) staff       (20)     5261 2023-04-27 19:31:14.000000 RiskLib-0.6.5/RiskLib/simulation.py
+drwxr-xr-x   0 ma_qh      (501) staff       (20)        0 2023-04-27 21:30:37.749515 RiskLib-0.6.5/RiskLib.egg-info/
+-rw-r--r--   0 ma_qh      (501) staff       (20)      116 2023-04-27 21:30:37.000000 RiskLib-0.6.5/RiskLib.egg-info/PKG-INFO
+-rw-r--r--   0 ma_qh      (501) staff       (20)      363 2023-04-27 21:30:37.000000 RiskLib-0.6.5/RiskLib.egg-info/SOURCES.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        1 2023-04-27 21:30:37.000000 RiskLib-0.6.5/RiskLib.egg-info/dependency_links.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       19 2023-04-27 21:30:37.000000 RiskLib-0.6.5/RiskLib.egg-info/requires.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)        8 2023-04-27 21:30:37.000000 RiskLib-0.6.5/RiskLib.egg-info/top_level.txt
+-rw-r--r--   0 ma_qh      (501) staff       (20)       38 2023-04-27 21:30:37.750008 RiskLib-0.6.5/setup.cfg
+-rw-r--r--   0 ma_qh      (501) staff       (20)      235 2023-04-27 21:30:21.000000 RiskLib-0.6.5/setup.py
```

### Comparing `RiskLib-0.6.4/RiskLib/Option.py` & `RiskLib-0.6.5/RiskLib/Option.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,22 +171,23 @@
         return carry_rho
 
     
     def greeks(self):
         """
         Calculates and returns all the greeks of the option as a dictionary.
         """
+        value = self.price()
         delta = self.delta()
         gamma = self.gamma()
         vega = self.vega()
         theta = self.theta()
         rho = self.rho()
         carry_rho = self.carry_rho()
         
-        return {'Delta': delta, 'Gamma': gamma, 'Vega': vega, 'Theta': theta, 'Rho': rho, "Carry Rho": carry_rho}
+        return {'Value': value, 'Delta': delta, 'Gamma': gamma, 'Vega': vega, 'Theta': theta, 'Rho': rho, "Carry Rho": carry_rho}
     
 
 
 def binomial_tree_american_continous(S0, K, T, r, q, sigma, N=200, option_type='call'):
     dt = T/N
     u = np.exp(sigma*np.sqrt(dt))
     d = 1/u
```

### Comparing `RiskLib-0.6.4/RiskLib/calculation.py` & `RiskLib-0.6.5/RiskLib/calculation.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.4/RiskLib/cov_matrix.py` & `RiskLib-0.6.5/RiskLib/cov_matrix.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.4/RiskLib/linear_regression.py` & `RiskLib-0.6.5/RiskLib/linear_regression.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.4/RiskLib/optimal_portfolio.py` & `RiskLib-0.6.5/RiskLib/optimal_portfolio.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.4/RiskLib/risk_parity.py` & `RiskLib-0.6.5/RiskLib/risk_parity.py`

 * *Files identical despite different names*

### Comparing `RiskLib-0.6.4/RiskLib/simulation.py` & `RiskLib-0.6.5/RiskLib/simulation.py`

 * *Files identical despite different names*

