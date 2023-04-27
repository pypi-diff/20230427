# Comparing `tmp/timecalculator-1.2.0.tar.gz` & `tmp/timecalculator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timecalculator-1.2.0.tar", last modified: Thu Apr 27 17:01:25 2023, max compression
+gzip compressed data, was "timecalculator-1.2.1.tar", last modified: Thu Apr 27 17:03:06 2023, max compression
```

## Comparing `timecalculator-1.2.0.tar` & `timecalculator-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:01:25.051694 timecalculator-1.2.0/
--rw-rw-rw-   0        0        0     1062 2023-04-27 13:33:04.000000 timecalculator-1.2.0/LICENCE.txt
--rw-rw-rw-   0        0        0     3505 2023-04-27 17:01:25.049693 timecalculator-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2980 2023-04-27 16:57:39.000000 timecalculator-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 17:01:25.051694 timecalculator-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-04-27 17:01:09.000000 timecalculator-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:01:25.013124 timecalculator-1.2.0/timecalculator/
--rw-rw-rw-   0        0        0     2080 2023-04-27 13:33:04.000000 timecalculator-1.2.0/timecalculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:01:25.048693 timecalculator-1.2.0/timecalculator.egg-info/
--rw-rw-rw-   0        0        0     3505 2023-04-27 17:01:24.000000 timecalculator-1.2.0/timecalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-04-27 17:01:24.000000 timecalculator-1.2.0/timecalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:01:24.000000 timecalculator-1.2.0/timecalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 17:01:24.000000 timecalculator-1.2.0/timecalculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 17:03:06.329852 timecalculator-1.2.1/
+-rw-rw-rw-   0        0        0     1062 2023-04-27 13:33:04.000000 timecalculator-1.2.1/LICENCE.txt
+-rw-rw-rw-   0        0        0     3506 2023-04-27 17:03:06.326852 timecalculator-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2981 2023-04-27 17:02:54.000000 timecalculator-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 17:03:06.329852 timecalculator-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-04-27 17:03:01.000000 timecalculator-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:03:06.298625 timecalculator-1.2.1/timecalculator/
+-rw-rw-rw-   0        0        0     2080 2023-04-27 13:33:04.000000 timecalculator-1.2.1/timecalculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:03:06.325852 timecalculator-1.2.1/timecalculator.egg-info/
+-rw-rw-rw-   0        0        0     3506 2023-04-27 17:03:06.000000 timecalculator-1.2.1/timecalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-04-27 17:03:06.000000 timecalculator-1.2.1/timecalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 17:03:06.000000 timecalculator-1.2.1/timecalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 17:03:06.000000 timecalculator-1.2.1/timecalculator.egg-info/top_level.txt
```

### Comparing `timecalculator-1.2.0/LICENCE.txt` & `timecalculator-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `timecalculator-1.2.0/PKG-INFO` & `timecalculator-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timecalculator
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for converting time units to seconds
 Home-page: https://github.com/Xyndra/Timecalculator
 Author: Xyndra
 Author-email: sammy@deutschergamingserver.de
 License: MIT
 Keywords: time,calculator
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,16 @@
 
 Once you have a TimeCalculator object, you can use the `to_seconds` method to convert any time unit to seconds. The `to_seconds` method takes two arguments: `time_value` and `time_unit`. The `time_value` argument is the value you want to convert, and the `time_unit` argument is the unit of the value, expressed in seconds.
 
 Here's a simple example of how to use the `to_seconds` method to convert 5 minutes to seconds:
 
 ```
 
-minutes = 5 total_seconds = tc.to_seconds(minutes, tc.MINUTE)
+minutes = 5
+total_seconds = tc.to_seconds(minutes, tc.MINUTE)
 print(f"{minutes} minutes is {total_seconds} seconds")
 
 ```
 
 In this example, we pass the value `5` and the `MINUTE` constant to the `to_seconds` method to convert the time to seconds. The resulting value is stored in the `total_seconds` variable. Finally, we print out the result.
 
 The output of this code will be:
```

### Comparing `timecalculator-1.2.0/README.md` & `timecalculator-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
 Once you have a TimeCalculator object, you can use the `to_seconds` method to convert any time unit to seconds. The `to_seconds` method takes two arguments: `time_value` and `time_unit`. The `time_value` argument is the value you want to convert, and the `time_unit` argument is the unit of the value, expressed in seconds.
 
 Here's a simple example of how to use the `to_seconds` method to convert 5 minutes to seconds:
 
 ```
 
-minutes = 5 total_seconds = tc.to_seconds(minutes, tc.MINUTE)
+minutes = 5
+total_seconds = tc.to_seconds(minutes, tc.MINUTE)
 print(f"{minutes} minutes is {total_seconds} seconds")
 
 ```
 
 In this example, we pass the value `5` and the `MINUTE` constant to the `to_seconds` method to convert the time to seconds. The resulting value is stored in the `total_seconds` variable. Finally, we print out the result.
 
 The output of this code will be:
```

### Comparing `timecalculator-1.2.0/setup.py` & `timecalculator-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Operating System :: Microsoft :: Windows :: Windows 10",
 ]
 
 setup(
     name="timecalculator",
-    version="1.2.0",
+    version="1.2.1",
     packages=find_packages(),
     description="A Python package for converting time units to seconds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Xyndra",
     author_email="sammy@deutschergamingserver.de",
     license="MIT",
```

### Comparing `timecalculator-1.2.0/timecalculator/__init__.py` & `timecalculator-1.2.1/timecalculator/__init__.py`

 * *Files identical despite different names*

### Comparing `timecalculator-1.2.0/timecalculator.egg-info/PKG-INFO` & `timecalculator-1.2.1/timecalculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timecalculator
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for converting time units to seconds
 Home-page: https://github.com/Xyndra/Timecalculator
 Author: Xyndra
 Author-email: sammy@deutschergamingserver.de
 License: MIT
 Keywords: time,calculator
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,16 @@
 
 Once you have a TimeCalculator object, you can use the `to_seconds` method to convert any time unit to seconds. The `to_seconds` method takes two arguments: `time_value` and `time_unit`. The `time_value` argument is the value you want to convert, and the `time_unit` argument is the unit of the value, expressed in seconds.
 
 Here's a simple example of how to use the `to_seconds` method to convert 5 minutes to seconds:
 
 ```
 
-minutes = 5 total_seconds = tc.to_seconds(minutes, tc.MINUTE)
+minutes = 5
+total_seconds = tc.to_seconds(minutes, tc.MINUTE)
 print(f"{minutes} minutes is {total_seconds} seconds")
 
 ```
 
 In this example, we pass the value `5` and the `MINUTE` constant to the `to_seconds` method to convert the time to seconds. The resulting value is stored in the `total_seconds` variable. Finally, we print out the result.
 
 The output of this code will be:
```

