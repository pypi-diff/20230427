# Comparing `tmp/currensees-1.0.9.tar.gz` & `tmp/currensees-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/currensees-1.0.9.tar", last modified: Sat Apr 22 19:10:34 2023, max compression
+gzip compressed data, was "dist/currensees-1.1.0.tar", last modified: Thu Apr 27 04:02:45 2023, max compression
```

## Comparing `currensees-1.0.9.tar` & `currensees-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-22 19:10:34.497223 currensees-1.0.9/
--rw-r--r--   0 finn       (501) staff       (20)     6299 2023-04-22 19:10:34.497521 currensees-1.0.9/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3174 2023-04-22 19:08:57.000000 currensees-1.0.9/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-22 19:10:34.491913 currensees-1.0.9/currensees/
--rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.0.9/currensees/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.0.9/currensees/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      755 2023-04-22 18:24:20.000000 currensees-1.0.9/currensees/convert.py
--rw-r--r--   0 finn       (501) staff       (20)      709 2023-04-22 18:21:27.000000 currensees-1.0.9/currensees/convert_all.py
--rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-22 18:45:05.000000 currensees-1.0.9/currensees/currencies.py
--rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.0.9/currensees/daily_average.py
--rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-22 19:03:02.000000 currensees-1.0.9/currensees/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-22 18:46:05.000000 currensees-1.0.9/currensees/margins_spreads.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-22 19:09:45.000000 currensees-1.0.9/currensees/version.py
--rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.0.9/currensees/weekly_average.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-22 19:10:34.496671 currensees-1.0.9/currensees.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     6299 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-22 19:10:19.000000 currensees-1.0.9/currensees.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-22 19:10:34.000000 currensees-1.0.9/currensees.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-22 19:10:34.498349 currensees-1.0.9/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-22 19:09:45.000000 currensees-1.0.9/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-27 04:02:45.005945 currensees-1.1.0/
+-rw-r--r--   0 finn       (501) staff       (20)     7001 2023-04-27 04:02:45.006277 currensees-1.1.0/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3685 2023-04-27 04:01:36.000000 currensees-1.1.0/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-27 04:02:45.002859 currensees-1.1.0/currensees/
+-rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.1.0/currensees/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.1.0/currensees/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      755 2023-04-22 18:24:20.000000 currensees-1.1.0/currensees/convert.py
+-rw-r--r--   0 finn       (501) staff       (20)      709 2023-04-22 18:21:27.000000 currensees-1.1.0/currensees/convert_all.py
+-rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-22 18:45:05.000000 currensees-1.1.0/currensees/currencies.py
+-rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.1.0/currensees/daily_average.py
+-rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-22 19:03:02.000000 currensees-1.1.0/currensees/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-27 03:54:01.000000 currensees-1.1.0/currensees/margins_spreads.py
+-rw-r--r--   0 finn       (501) staff       (20)      974 2023-04-27 03:54:25.000000 currensees-1.1.0/currensees/performances.py
+-rw-r--r--   0 finn       (501) staff       (20)      939 2023-04-27 03:56:19.000000 currensees-1.1.0/currensees/signals.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-27 03:58:19.000000 currensees-1.1.0/currensees/version.py
+-rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.1.0/currensees/weekly_average.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-27 04:02:45.005424 currensees-1.1.0/currensees.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     7001 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      528 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-27 04:02:30.000000 currensees-1.1.0/currensees.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-27 04:02:45.006911 currensees-1.1.0/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-27 03:58:19.000000 currensees-1.1.0/setup.py
```

### Comparing `currensees-1.0.9/PKG-INFO` & `currensees-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -53,14 +53,16 @@
             from currensees.currencies import Currencies
             from currensees.historical import Historical
             from currensees.convert import Convert
             from currensees.convert_all import ConvertAll
             from currensees.daily_average import DailyAverage
             from currensees.weekly_average import WeeklyAverage
             from currensees.margins_spreads import MarginsSpreads
+            from currensees.performances import Performances
+            from currensees.signals import Signals
         
             # Authenticate and log in
             auth = Auth()
             username = "your_username"
             password = "your_password"
         
             result = auth.login(username, password)
@@ -102,14 +104,29 @@
             result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
             print("Margins and spreads:", result)
         
             uuid = "margins_spreads_uuid"
             result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
             print("Margins and spreads for currency:", result)
         
+            performances = Performances(auth.headers)
+            result = performances.get_performances(username)
+            print("Performances:", result)
+        
+            uuid = "performance_uuid"
+            result = performances.get_performance(uuid, username)
+            print("Performance:", result)
+        
+            signals = Signals(auth.headers)
+            result = signals.get_signals(username)
+            print("Signals:", result)
+        
+            uuid = "signal_uuid"
+            result = signals.get_signal(uuid, username)
+            print("Signal:", result)
         
         Setting up Currency API Account
         -------------------------------
         
         Subscribe here for a `user account`_.
         
         .. _user account: https://moatsystems.com/currency-api/
```

### Comparing `currensees-1.0.9/README.md` & `currensees-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from currensees.currencies import Currencies
 from currensees.historical import Historical
 from currensees.convert import Convert
 from currensees.convert_all import ConvertAll
 from currensees.daily_average import DailyAverage
 from currensees.weekly_average import WeeklyAverage
 from currensees.margins_spreads import MarginsSpreads
+from currensees.performances import Performances
+from currensees.signals import Signals
 
 # Authenticate and log in
 auth = Auth()
 username = "your_username"
 password = "your_password"
 
 result = auth.login(username, password)
@@ -80,14 +82,30 @@
 margins_spreads = MarginsSpreads(auth.headers)
 result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
 print("Margins and spreads:", result)
 
 uuid = "margins_spreads_uuid"
 result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
 print("Margins and spreads for currency:", result)
+
+performances = Performances(auth.headers)
+result = performances.get_performances(username)
+print("Performances:", result)
+
+uuid = "performance_uuid"
+result = performances.get_performance(uuid, username)
+print("Performance:", result)
+
+signals = Signals(auth.headers)
+result = signals.get_signals(username)
+print("Signals:", result)
+
+uuid = "signal_uuid"
+result = signals.get_signal(uuid, username)
+print("Signal:", result)
 ```
 
 ## Setting up Currency API Account
 
 Subscribe here for a [user account](https://moatsystems.com/currency-api/).
```

### Comparing `currensees-1.0.9/currensees/auth.py` & `currensees-1.1.0/currensees/auth.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees/convert.py` & `currensees-1.1.0/currensees/convert.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees/convert_all.py` & `currensees-1.1.0/currensees/convert_all.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees/currencies.py` & `currensees-1.1.0/currensees/currencies.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees/historical.py` & `currensees-1.1.0/currensees/historical.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees/margins_spreads.py` & `currensees-1.1.0/currensees/margins_spreads.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees/weekly_average.py` & `currensees-1.1.0/currensees/weekly_average.py`

 * *Files identical despite different names*

### Comparing `currensees-1.0.9/currensees.egg-info/PKG-INFO` & `currensees-1.1.0/currensees.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -53,14 +53,16 @@
             from currensees.currencies import Currencies
             from currensees.historical import Historical
             from currensees.convert import Convert
             from currensees.convert_all import ConvertAll
             from currensees.daily_average import DailyAverage
             from currensees.weekly_average import WeeklyAverage
             from currensees.margins_spreads import MarginsSpreads
+            from currensees.performances import Performances
+            from currensees.signals import Signals
         
             # Authenticate and log in
             auth = Auth()
             username = "your_username"
             password = "your_password"
         
             result = auth.login(username, password)
@@ -102,14 +104,29 @@
             result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
             print("Margins and spreads:", result)
         
             uuid = "margins_spreads_uuid"
             result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
             print("Margins and spreads for currency:", result)
         
+            performances = Performances(auth.headers)
+            result = performances.get_performances(username)
+            print("Performances:", result)
+        
+            uuid = "performance_uuid"
+            result = performances.get_performance(uuid, username)
+            print("Performance:", result)
+        
+            signals = Signals(auth.headers)
+            result = signals.get_signals(username)
+            print("Signals:", result)
+        
+            uuid = "signal_uuid"
+            result = signals.get_signal(uuid, username)
+            print("Signal:", result)
         
         Setting up Currency API Account
         -------------------------------
         
         Subscribe here for a `user account`_.
         
         .. _user account: https://moatsystems.com/currency-api/
```

### Comparing `currensees-1.0.9/setup.py` & `currensees-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "currensees"
-VERSION = "1.0.9"
+VERSION = "1.1.0"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

