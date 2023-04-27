# Comparing `tmp/ckanext-harvest-basket-1.3.5.tar.gz` & `tmp/ckanext-harvest-basket-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-harvest-basket-1.3.5.tar", last modified: Wed Jan 25 09:57:09 2023, max compression
+gzip compressed data, was "ckanext-harvest-basket-1.3.6.tar", last modified: Thu Apr 27 13:26:01 2023, max compression
```

## Comparing `ckanext-harvest-basket-1.3.5.tar` & `ckanext-harvest-basket-1.3.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    34500 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/LICENSE
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      213 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/MANIFEST.in
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2418 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/PKG-INFO
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1869 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/README.md
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      221 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/__init__.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/auth/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      227 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/auth/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      661 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/auth/get.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/logic/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      174 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/logic/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1862 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/logic/get.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/css/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      879 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/css/harvest_basket.css
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.280647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/js/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     3786 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/js/harvest_basket.js
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      325 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/webassets.yml
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      619 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     8522 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/arcgis_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     8338 2023-01-25 09:56:10.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/base_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2341 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/ckan_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     8079 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/dkan_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     6559 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/junar_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     8971 2023-01-04 14:28:22.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/ods_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)    14430 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/socrata_harvester.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      781 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/templates/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      228 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/templates/base.html
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/templates/source/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2355 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/templates/source/new_source_form.html
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/tests/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/tests/__init__.py
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1399 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/tests/test_plugin.py
-drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     2418 2023-01-25 09:57:09.000000 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/PKG-INFO
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     1415 2023-01-25 09:57:09.000000 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/SOURCES.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        1 2023-01-25 09:57:09.000000 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/dependency_links.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      552 2023-01-25 09:57:09.000000 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/entry_points.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-01-25 09:57:09.000000 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/namespace_packages.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-01-25 09:57:09.000000 ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/top_level.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)       66 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.5/requirements.txt
--rw-rw-r--   0 cherry    (1000) cherry    (1000)      777 2023-01-25 09:57:09.284647 ckanext-harvest-basket-1.3.5/setup.cfg
--rw-rw-r--   0 cherry    (1000) cherry    (1000)     4210 2023-01-25 09:55:12.000000 ckanext-harvest-basket-1.3.5/setup.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.037452 ckanext-harvest-basket-1.3.6/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)    34500 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/LICENSE
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      213 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/MANIFEST.in
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2418 2023-04-27 13:26:01.037452 ckanext-harvest-basket-1.3.6/PKG-INFO
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1869 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/README.md
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      221 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/auth/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      227 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/auth/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      661 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/auth/get.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/logic/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      174 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/logic/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1862 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/logic/get.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/css/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      879 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/css/harvest_basket.css
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/js/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3786 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/js/harvest_basket.js
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      325 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/webassets.yml
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      619 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     8522 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/arcgis_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     8338 2023-04-27 13:23:49.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/base_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2341 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/ckan_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     8079 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/dkan_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     6559 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/junar_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     9596 2023-04-27 13:23:52.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/ods_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)    14430 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/socrata_harvester.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      781 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/plugin.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/templates/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      228 2023-02-21 08:17:21.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/templates/base.html
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/templates/source/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2355 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/templates/source/new_source_form.html
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.033452 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/tests/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/tests/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1399 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/tests/test_plugin.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-27 13:26:01.037452 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2418 2023-04-27 13:26:01.000000 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/PKG-INFO
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1415 2023-04-27 13:26:01.000000 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/SOURCES.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        1 2023-04-27 13:26:01.000000 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/dependency_links.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      552 2023-04-27 13:26:01.000000 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/entry_points.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-04-27 13:26:01.000000 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-04-27 13:26:01.000000 ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/top_level.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       66 2022-08-02 08:25:34.000000 ckanext-harvest-basket-1.3.6/requirements.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      777 2023-04-27 13:26:01.037452 ckanext-harvest-basket-1.3.6/setup.cfg
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     4210 2023-04-27 13:23:57.000000 ckanext-harvest-basket-1.3.6/setup.py
```

### Comparing `ckanext-harvest-basket-1.3.5/LICENSE` & `ckanext-harvest-basket-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/PKG-INFO` & `ckanext-harvest-basket-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-harvest-basket
-Version: 1.3.5
+Version: 1.3.6
 Summary: A bunch of custom harvesters for ckanext-harvest
 Home-page: https://github.com/mutantsan/ckanext-harvest-basket
 Author: Alexandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN harvest harvester
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-harvest-basket-1.3.5/README.md` & `ckanext-harvest-basket-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/auth/get.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/auth/get.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/action/logic/get.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/action/logic/get.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/css/harvest_basket.css` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/css/harvest_basket.css`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/assets/js/harvest_basket.js` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/assets/js/harvest_basket.js`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/__init__.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/arcgis_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/arcgis_harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/base_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/base_harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/ckan_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/ckan_harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/dkan_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/dkan_harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/junar_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/junar_harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/ods_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/ods_harvester.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+import mimetypes
 import logging
 import json
-from typing import Iterable, Any
+from typing import Any
 from urllib.parse import urljoin, urlencode
 
 import ckan.plugins.toolkit as tk
 from ckan.lib.navl.validators import unicode_safe
 
 from ckanext.harvest.model import HarvestObject
 from ckanext.harvest.harvesters.ckanharvester import SearchError
@@ -160,20 +161,33 @@
                 resource = {}
                 url = urljoin(
                     source_url, offset.format(pkg_data["origin_id"], att["id"])
                 )
 
                 resource["package_id"] = pkg_data["id"]
                 resource["url"] = url
-                resource["format"] = (att["url"].split(".")[-1]).upper()
+                resource["format"] = self._guess_attachment_format(att)
                 resource["name"] = att.get("title", "")
 
                 resources.append(resource)
         return resources
 
+    def _guess_attachment_format(self, attachment: dict[str, str]) -> str:
+        """The attachment doesn't have a format field, only mimetype. So we
+        could try to guess a format by mimetype. If it's not here, use a url
+        and try to parse format from it (it could end with something like
+        `attachment_name.pdf`"""
+        mimetype: str | None = attachment.get("mimetype")
+        if mimetype:
+            dot_format: str | None = mimetypes.guess_extension(mimetype)
+            if dot_format:
+                return dot_format.strip(".")
+
+        return (attachment["url"].split(".")[-1]).upper()
+
     def fetch_stage(self, harvest_object):
         self._set_config(harvest_object.source.config)
         source_url = self._get_src_url(harvest_object)
         package_dict = json.loads(harvest_object.content)
         self._pre_map_stage(package_dict, source_url)
         harvest_object.content = json.dumps(package_dict)
         return True
```

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/harvesters/socrata_harvester.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/harvesters/socrata_harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/plugin.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/templates/source/new_source_form.html` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/templates/source/new_source_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext/harvest_basket/tests/test_plugin.py` & `ckanext-harvest-basket-1.3.6/ckanext/harvest_basket/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/PKG-INFO` & `ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-harvest-basket
-Version: 1.3.5
+Version: 1.3.6
 Summary: A bunch of custom harvesters for ckanext-harvest
 Home-page: https://github.com/mutantsan/ckanext-harvest-basket
 Author: Alexandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN harvest harvester
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/SOURCES.txt` & `ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/ckanext_harvest_basket.egg-info/entry_points.txt` & `ckanext-harvest-basket-1.3.6/ckanext_harvest_basket.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/setup.cfg` & `ckanext-harvest-basket-1.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-harvest-basket-1.3.5/setup.py` & `ckanext-harvest-basket-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 setup(
     name="""ckanext-harvest-basket""",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version="1.3.5",
+    version="1.3.6",
     description="""A bunch of custom harvesters for ckanext-harvest""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/mutantsan/ckanext-harvest-basket",
     # Author details
     author="""Alexandr Cherniavskyi""",
```

