# Comparing `tmp/aggdirect_route_estimation_calculator-0.3.tar.gz` & `tmp/aggdirect_route_estimation_calculator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggdirect_route_estimation_calculator-0.3.tar", last modified: Wed Apr 26 07:13:23 2023, max compression
+gzip compressed data, was "aggdirect_route_estimation_calculator-0.4.tar", last modified: Thu Apr 27 07:42:02 2023, max compression
```

## Comparing `aggdirect_route_estimation_calculator-0.3.tar` & `aggdirect_route_estimation_calculator-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:05:23.000000 aggdirect_route_estimation_calculator-0.3/LICENSE
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/PKG-INFO
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1463 2023-04-25 14:10:26.000000 aggdirect_route_estimation_calculator-0.3/README.md
-drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-26 07:13:23.376789 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator/
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      925 2023-04-26 07:09:17.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator/__init__.py
-drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/PKG-INFO
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      380 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/SOURCES.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        1 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/dependency_links.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        9 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/requires.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-04-26 07:13:23.000000 aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator.egg-info/top_level.txt
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-04-26 07:13:23.380789 aggdirect_route_estimation_calculator-0.3/setup.cfg
--rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1074 2023-04-26 07:09:12.000000 aggdirect_route_estimation_calculator-0.3/setup.py
+drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-27 07:42:02.493060 aggdirect_route_estimation_calculator-0.4/
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        0 2023-03-10 07:05:23.000000 aggdirect_route_estimation_calculator-0.4/LICENSE
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-04-27 07:42:02.493060 aggdirect_route_estimation_calculator-0.4/PKG-INFO
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1463 2023-04-25 14:10:26.000000 aggdirect_route_estimation_calculator-0.4/README.md
+drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-27 07:42:02.493060 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator/
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      913 2023-04-27 07:40:20.000000 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator/__init__.py
+drwxrwxr-x   0 chinmoy   (1000) chinmoy   (1000)        0 2023-04-27 07:42:02.493060 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator.egg-info/
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      504 2023-04-27 07:42:02.000000 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator.egg-info/PKG-INFO
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)      380 2023-04-27 07:42:02.000000 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        1 2023-04-27 07:42:02.000000 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)        9 2023-04-27 07:42:02.000000 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator.egg-info/requires.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-04-27 07:42:02.000000 aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator.egg-info/top_level.txt
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)       38 2023-04-27 07:42:02.493060 aggdirect_route_estimation_calculator-0.4/setup.cfg
+-rw-rw-r--   0 chinmoy   (1000) chinmoy   (1000)     1074 2023-04-27 07:40:28.000000 aggdirect_route_estimation_calculator-0.4/setup.py
```

### Comparing `aggdirect_route_estimation_calculator-0.3/README.md` & `aggdirect_route_estimation_calculator-0.4/README.md`

 * *Files identical despite different names*

### Comparing `aggdirect_route_estimation_calculator-0.3/aggdirect_route_estimation_calculator/__init__.py` & `aggdirect_route_estimation_calculator-0.4/aggdirect_route_estimation_calculator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     def estimated_distance(self, required_unit="M"):
         required_unit = required_unit.upper()
         unit = {"M":[0.000621371, "Miles"], "K":[0.001,"Kilometer"], "T":[1, "Meter"]}
         return f"{str(round(self.__response['routes'][0]['distance'] * unit.get(required_unit)[0], 2))} {unit.get(required_unit)[1]}"
     
     
     def get_path(self):
-        return ";".join([f'{l[0] * 0.1},{l[1] * 0.1}' for l in polyline.decode(self.__response['routes'][0]['geometry'])])
+        return ";".join([f'{l[0]},{l[1]}' for l in polyline.decode(self.__response['routes'][0]['geometry'])])
```

### Comparing `aggdirect_route_estimation_calculator-0.3/setup.py` & `aggdirect_route_estimation_calculator-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name = 'aggdirect_route_estimation_calculator',         # How you named your package folder (MyLib)
     packages = ['aggdirect_route_estimation_calculator'],
-    version = '0.3',
+    version = '0.4',
     description = 'Route Estimation Calculator functions',
     author = 'Chinmoy Das',
     author_email = '',
     url = '',   # Provide either the link to your github or to your website
     keywords = ['Route Estimation Calculator', 'Route Calculator' , 'AGGDIRECT'],   # Keywords that define your package best
     install_requires=['polyline'],
     classifiers=[
```

