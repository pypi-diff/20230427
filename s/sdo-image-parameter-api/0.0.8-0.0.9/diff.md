# Comparing `tmp/sdo_image_parameter_api-0.0.8.tar.gz` & `tmp/sdo_image_parameter_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdo_image_parameter_api-0.0.8.tar", last modified: Thu Apr 27 00:50:07 2023, max compression
+gzip compressed data, was "sdo_image_parameter_api-0.0.9.tar", last modified: Thu Apr 27 00:52:34 2023, max compression
```

## Comparing `sdo_image_parameter_api-0.0.8.tar` & `sdo_image_parameter_api-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 00:50:07.477312 sdo_image_parameter_api-0.0.8/
--rw-rw-rw-   0        0        0     1089 2023-04-24 19:02:43.000000 sdo_image_parameter_api-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3407 2023-04-27 00:50:07.477312 sdo_image_parameter_api-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2630 2023-04-26 23:07:31.000000 sdo_image_parameter_api-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 00:50:07.477312 sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-04-27 00:50:07.000000 sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-04-27 00:50:07.000000 sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 00:50:07.000000 sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-27 00:50:07.000000 sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-27 00:50:07.000000 sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 00:50:07.477312 sdo_image_parameter_api-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-04-27 00:49:51.000000 sdo_image_parameter_api-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 00:50:07.446037 sdo_image_parameter_api-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 00:50:07.477312 sdo_image_parameter_api-0.0.8/src/sdo_image_parameter_api/
--rw-rw-rw-   0        0        0        0 2023-04-24 18:59:15.000000 sdo_image_parameter_api-0.0.8/src/sdo_image_parameter_api/__init__.py
--rw-rw-rw-   0        0        0    17256 2023-04-26 22:44:33.000000 sdo_image_parameter_api-0.0.8/src/sdo_image_parameter_api/image_methods.py
+drwxrwxrwx   0        0        0        0 2023-04-27 00:52:34.334098 sdo_image_parameter_api-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2023-04-24 19:02:43.000000 sdo_image_parameter_api-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3407 2023-04-27 00:52:34.334098 sdo_image_parameter_api-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2630 2023-04-26 23:07:31.000000 sdo_image_parameter_api-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 00:52:34.318500 sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-04-27 00:52:34.000000 sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-04-27 00:52:34.000000 sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 00:52:34.000000 sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-27 00:52:34.000000 sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2023-04-27 00:52:34.000000 sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 00:52:34.334098 sdo_image_parameter_api-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1846 2023-04-27 00:52:14.000000 sdo_image_parameter_api-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 00:52:34.287239 sdo_image_parameter_api-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 00:52:34.318500 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/
+-rw-rw-rw-   0        0        0        0 2023-04-24 18:59:15.000000 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/__init__.py
+-rw-rw-rw-   0        0        0    17256 2023-04-26 22:44:33.000000 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/image_methods.py
+drwxrwxrwx   0        0        0        0 2023-04-27 00:52:34.318500 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/util/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:48:49.000000 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/util/__init__.py
+-rw-rw-rw-   0        0        0     3033 2023-03-09 20:48:49.000000 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/util/constants.py
+-rw-rw-rw-   0        0        0     2121 2023-04-26 22:40:21.000000 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/util/converters.py
+-rw-rw-rw-   0        0        0     3294 2023-04-26 22:44:41.000000 sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/util/validators.py
```

### Comparing `sdo_image_parameter_api-0.0.8/LICENSE` & `sdo_image_parameter_api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdo_image_parameter_api-0.0.8/PKG-INFO` & `sdo_image_parameter_api-0.0.9/sdo_image_parameter_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sdo_image_parameter_api
-Version: 0.0.8
+Name: sdo-image-parameter-api
+Version: 0.0.9
 Summary: A toolkit for accessing solar image data
 Home-page: https://bitbucket.org/ds4350-image-param-api-rm/solar-image-api/src/main/
 Author: Ruqayyah Muse
 Author-email: ruqayyahmuse@gmail.com
 Maintainer: Ruqayyah Muse
 Maintainer-email: ruqayyahmuse@gmail.com
 License: MIT
```

### Comparing `sdo_image_parameter_api-0.0.8/README.md` & `sdo_image_parameter_api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sdo_image_parameter_api-0.0.8/sdo_image_parameter_api.egg-info/PKG-INFO` & `sdo_image_parameter_api-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sdo-image-parameter-api
-Version: 0.0.8
+Name: sdo_image_parameter_api
+Version: 0.0.9
 Summary: A toolkit for accessing solar image data
 Home-page: https://bitbucket.org/ds4350-image-param-api-rm/solar-image-api/src/main/
 Author: Ruqayyah Muse
 Author-email: ruqayyahmuse@gmail.com
 Maintainer: Ruqayyah Muse
 Maintainer-email: ruqayyahmuse@gmail.com
 License: MIT
```

### Comparing `sdo_image_parameter_api-0.0.8/setup.py` & `sdo_image_parameter_api-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 
 # pckges = find_packages(where="src")
 # pckges = find_packages()
 
 # ------------- SETUP ---------------
 setup(
     name="sdo_image_parameter_api",
-    version="0.0.8",
+    version="0.0.9",
     author="Ruqayyah Muse",
     author_email="ruqayyahmuse@gmail.com",
     url="https://bitbucket.org/ds4350-image-param-api-rm/solar-image-api"
         "/src/main/",
     maintainer='Ruqayyah Muse',
     maintainer_email="ruqayyahmuse@gmail.com",
     description="A toolkit for accessing solar image data",
     long_description=readme,
     long_description_content_type='text/markdown',
-    packages=['src/sdo_image_parameter_api'],
+    packages=['src/sdo_image_parameter_api',
+              'src/sdo_image_parameter_api/util'],
     package_data={'.': ['requirements.txt']},
     install_requires=install_requires,
     include_package_data=True,
     license='MIT',
     keywords=['sun', 'sdo', 'solar images', 'parameters'],
     project_urls={
         'Source': "https://bitbucket.org/ds4350-image-param-api-rm/solar"
```

### Comparing `sdo_image_parameter_api-0.0.8/src/sdo_image_parameter_api/image_methods.py` & `sdo_image_parameter_api-0.0.9/src/sdo_image_parameter_api/image_methods.py`

 * *Files identical despite different names*

