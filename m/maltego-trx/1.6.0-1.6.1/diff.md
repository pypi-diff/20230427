# Comparing `tmp/maltego-trx-1.6.0.tar.gz` & `tmp/maltego-trx-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maltego-trx-1.6.0.tar", last modified: Wed Aug 10 12:09:46 2022, max compression
+gzip compressed data, was "maltego-trx-1.6.1.tar", last modified: Thu Apr 27 14:53:06 2023, max compression
```

## Comparing `maltego-trx-1.6.0.tar` & `maltego-trx-1.6.1.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/
--rw-r--r--   0 vsts      (1001) docker     (121)     1068 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)    18239 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    17942 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/maltego_trx/
--rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1435 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/commands.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8631 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/decorator_registry.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3178 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/entities.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1302 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14762 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/maltego.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7614 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/mtz.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6180 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/oauth.py
--rw-r--r--   0 vsts      (1001) docker     (121)      248 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/overlays.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1945 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/registry.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2482 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/maltego_trx/template_dir/
--rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/Dockerfile
--rw-r--r--   0 vsts      (1001) docker     (121)      145 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/docker-compose.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      622 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (121)      400 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/project.py
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       46 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/settings.csv
--rw-r--r--   0 vsts      (1001) docker     (121)      614 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/settings.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/maltego_trx/template_dir/transforms/
--rw-r--r--   0 vsts      (1001) docker     (121)     1015 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/transforms/DNSToIP.py
--rw-r--r--   0 vsts      (1001) docker     (121)      690 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/transforms/GreetPerson.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1208 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/transforms/GreetPersonLocalized.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2288 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/transforms/OverlayExample.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/transforms/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      693 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/template_dir/transforms.csv
--rw-r--r--   0 vsts      (1001) docker     (121)      428 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/transform.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4923 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/maltego_trx/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/maltego_trx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)    18239 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1152 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       76 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       73 2022-08-10 12:09:46.000000 maltego-trx-1.6.0/maltego_trx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-08-10 12:09:46.643213 maltego-trx-1.6.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     1270 2022-08-10 12:09:35.000000 maltego-trx-1.6.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 14:53:06.749280 maltego-trx-1.6.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1068 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)    18342 2023-04-27 14:53:06.749280 maltego-trx-1.6.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    18020 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 14:53:06.745280 maltego-trx-1.6.1/maltego_trx/
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1435 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9258 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/decorator_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3178 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/entities.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1302 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/handler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14762 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/maltego.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7614 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/mtz.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6180 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/oauth.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      248 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/overlays.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1945 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2482 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 14:53:06.749280 maltego-trx-1.6.1/maltego_trx/template_dir/
+-rw-r--r--   0 vsts      (1001) docker     (122)      651 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/Dockerfile
+-rw-r--r--   0 vsts      (1001) docker     (122)      145 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/docker-compose.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      622 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/project.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/settings.csv
+-rw-r--r--   0 vsts      (1001) docker     (122)      614 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/settings.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 14:53:06.749280 maltego-trx-1.6.1/maltego_trx/template_dir/transforms/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1015 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/transforms/DNSToIP.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      690 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/transforms/GreetPerson.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1208 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/transforms/GreetPersonLocalized.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/transforms/OverlayExample.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/transforms/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      693 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/template_dir/transforms.csv
+-rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/transform.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4873 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/maltego_trx/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 14:53:06.745280 maltego-trx-1.6.1/maltego_trx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18342 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1266 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       73 2023-04-27 14:53:06.000000 maltego-trx-1.6.1/maltego_trx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-04-27 14:53:06.749280 maltego-trx-1.6.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-27 14:53:06.749280 maltego-trx-1.6.1/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3624 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/tests/test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10238 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/tests/test_decorator_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/tests/test_mtz.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      767 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/tests/test_property_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6085 2023-04-27 14:52:58.000000 maltego-trx-1.6.1/tests/test_xml.py
```

### Comparing `maltego-trx-1.6.0/LICENSE` & `maltego-trx-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/PKG-INFO` & `maltego-trx-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: maltego-trx
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python library used to develop Maltego transforms
 Home-page: https://github.com/paterva/maltego-trx/
 Author: Maltego Staff
 Author-email: support@maltego.com
 License: MIT
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Maltego TRX Python Library
 
-[![Runs with Python3.6 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml)
-[![PyTest with Python3.6 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml)
+[![Runs with Python3.8 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml)
+[![PyTest with Python3.8 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml)
 [![Sonatype Jake](https://github.com/paterva/maltego-trx/actions/workflows/sonatype-jack.yml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/sonatype-jack.yml)
 
 ## Release Notes
 
+__1.6.1__: Update cryptography and Flask dependency and deprecate Python 3.7
+
 __1.6.0__: Automatically generate am `.mtz` for your local transforms
 
 __1.5.2__: Add logging output for invalid / missing params in xml serialization
 
 __1.5.1__: Add ignored files to starter and use README for pypi
 
 __1.5.0__: XML Serialization via `ElementTree` instead of string interpolation
@@ -29,15 +32,15 @@
 
 __1.4.0 + 1.4.1:__ Both versions are incompatible with python3.7 and lower.
 
 __1.4.2__: Fixed python3.6 incompatibility
 
 ## Getting Started
 
-_Note: Support for Python 2 has been officially discontinued as of July 2021. Please use Python 3.6 or higher to use
+_Note: Support for Python 2 has been officially discontinued as of July 2021. Please use Python 3.8 or higher to use
 up-to-date versions of Maltego TRX._
 
 To install the trx library run the following command:
 
 ``` bash
 pip install maltego-trx
 ```
```

### Comparing `maltego-trx-1.6.0/README.md` & `maltego-trx-1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Maltego TRX Python Library
 
-[![Runs with Python3.6 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml)
-[![PyTest with Python3.6 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml)
+[![Runs with Python3.8 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml)
+[![PyTest with Python3.8 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml)
 [![Sonatype Jake](https://github.com/paterva/maltego-trx/actions/workflows/sonatype-jack.yml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/sonatype-jack.yml)
 
 ## Release Notes
 
+__1.6.1__: Update cryptography and Flask dependency and deprecate Python 3.7
+
 __1.6.0__: Automatically generate am `.mtz` for your local transforms
 
 __1.5.2__: Add logging output for invalid / missing params in xml serialization
 
 __1.5.1__: Add ignored files to starter and use README for pypi
 
 __1.5.0__: XML Serialization via `ElementTree` instead of string interpolation
@@ -18,15 +20,15 @@
 
 __1.4.0 + 1.4.1:__ Both versions are incompatible with python3.7 and lower.
 
 __1.4.2__: Fixed python3.6 incompatibility
 
 ## Getting Started
 
-_Note: Support for Python 2 has been officially discontinued as of July 2021. Please use Python 3.6 or higher to use
+_Note: Support for Python 2 has been officially discontinued as of July 2021. Please use Python 3.8 or higher to use
 up-to-date versions of Maltego TRX._
 
 To install the trx library run the following command:
 
 ``` bash
 pip install maltego-trx
 ```
```

### Comparing `maltego-trx-1.6.0/maltego_trx/commands.py` & `maltego-trx-1.6.1/maltego_trx/commands.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/decorator_registry.py` & `maltego-trx-1.6.1/maltego_trx/decorator_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,26 @@
     escape_csv_fields,
     export_as_csv,
     serialize_bool,
     name_to_path,
     serialize_xml,
 )
 
-TRANSFORMS_CSV_HEADER = (
+LEGACY_TRANSFORMS_CSV_HEADER = (
     "Owner,Author,Disclaimer,Description,Version,"
     "Name,UIName,URL,entityName,"
     "oAuthSettingId,transformSettingIDs,seedIDs"
 )
+
+TRANSFORMS_CSV_HEADER = (
+    "Owner,Author,Disclaimer,Description,Version,"
+    "Name,UIName,URL,entityName,"
+    "oAuthSettingId,transformSettingIDs,seedIDs,outputEntities"
+)
+
 SETTINGS_CSV_HEADER = "Name,Type,Display,DefaultValue,Optional,Popup"
 
 
 @dataclass(frozen=True)
 class TransformSet:
     name: str
     description: str
@@ -123,15 +130,15 @@
             if transform_set:
                 self.transform_sets[transform_set].append(cleaned_transform_name)
 
             return transform_callable
 
         return decorated
 
-    def _create_transforms_config(self) -> Iterable[str]:
+    def _create_transforms_config(self, include_output_entities: bool = True) -> Iterable[str]:
         global_settings_full_names = [gs.id for gs in self.global_settings]
 
         for transform_name, transform_meta in self.transform_metas.items():
             meta_settings = [
                 setting.id
                 for setting in self.transform_settings.get(transform_name, [])
             ]
@@ -145,30 +152,38 @@
                 transform_name,
                 transform_meta.display_name + self.display_name_suffix,
                 os.path.join(self.host_url, "run", transform_name),
                 transform_meta.input_entity,
                 ";".join(self.oauth_settings_id),
                 # combine global and transform scoped settings
                 ";".join(chain(meta_settings, global_settings_full_names)),
-                ";".join(self.seed_ids),
+                ";".join(self.seed_ids)
             ]
 
+            if include_output_entities:
+                transform_row.append(";".join(transform_meta.output_entities))
+
             escaped_fields = escape_csv_fields(*transform_row)
             yield ",".join(escaped_fields)
 
     def write_transforms_config(
-        self, config_path: str = "./transforms.csv", csv_line_limit: int = 100
+        self, config_path: str = "./transforms.csv", csv_line_limit: int = 100, include_output_entities: bool = True
     ):
         """Exports the collected transform metadata as a csv-file to config_path"""
 
-        csv_lines = self._create_transforms_config()
+        csv_lines = self._create_transforms_config(include_output_entities=include_output_entities)
 
-        export_as_csv(
-            TRANSFORMS_CSV_HEADER, tuple(csv_lines), config_path, csv_line_limit
-        )
+        if not include_output_entities:
+            export_as_csv(
+                LEGACY_TRANSFORMS_CSV_HEADER, tuple(csv_lines), config_path, csv_line_limit
+            )
+        else:
+            export_as_csv(
+                TRANSFORMS_CSV_HEADER, tuple(csv_lines), config_path, csv_line_limit
+            )
 
     def _create_settings_config(self) -> Iterable[str]:
         chained_settings = chain(
             self.global_settings, *list(self.transform_settings.values())
         )
         unique_settings: Iterable[TransformSetting] = filter_unique(
             lambda s: s.name, chained_settings
```

### Comparing `maltego-trx-1.6.0/maltego_trx/entities.py` & `maltego-trx-1.6.1/maltego_trx/entities.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/handler.py` & `maltego-trx-1.6.1/maltego_trx/handler.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/maltego.py` & `maltego-trx-1.6.1/maltego_trx/maltego.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/mtz.py` & `maltego-trx-1.6.1/maltego_trx/mtz.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/oauth.py` & `maltego-trx-1.6.1/maltego_trx/oauth.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/registry.py` & `maltego-trx-1.6.1/maltego_trx/registry.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/server.py` & `maltego-trx-1.6.1/maltego_trx/server.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/Dockerfile` & `maltego-trx-1.6.1/maltego_trx/template_dir/Dockerfile`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/extensions.py` & `maltego-trx-1.6.1/maltego_trx/template_dir/extensions.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/settings.py` & `maltego-trx-1.6.1/maltego_trx/template_dir/settings.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/transforms/DNSToIP.py` & `maltego-trx-1.6.1/maltego_trx/template_dir/transforms/DNSToIP.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/transforms/GreetPerson.py` & `maltego-trx-1.6.1/maltego_trx/template_dir/transforms/GreetPerson.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/transforms/GreetPersonLocalized.py` & `maltego-trx-1.6.1/maltego_trx/template_dir/transforms/GreetPersonLocalized.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/transforms/OverlayExample.py` & `maltego-trx-1.6.1/maltego_trx/template_dir/transforms/OverlayExample.py`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/template_dir/transforms.csv` & `maltego-trx-1.6.1/maltego_trx/template_dir/transforms.csv`

 * *Files identical despite different names*

### Comparing `maltego-trx-1.6.0/maltego_trx/utils.py` & `maltego-trx-1.6.1/maltego_trx/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import re
 import sys
 import warnings
 from typing import TypeVar, Callable, Hashable, Iterable, Generator, Sequence
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 
-from six import text_type, binary_type
-
 logger = logging.getLogger("maltego-trx")
 
 
 def name_to_path(name):
     # Convert function name to a URL path
     path = name.replace("_", "-")
     return path.lower()
@@ -35,20 +33,20 @@
     :param val: the variable we want unicode encoded
     :return: val {Byte/Unicode}
     """
     return force_encoding(val, 'ascii')
 
 
 def force_encoding(val, encoding):
-    if type(val) == text_type:
+    if isinstance(val, str):
         return val.encode(encoding, 'replace').decode(encoding, 'replace')
-    elif type(val) == binary_type:
+    elif isinstance(val, bytes):
         return val.decode(encoding, 'replace')
     else:
-        return text_type(val).encode(encoding, 'replace').decode(encoding, 'replace')
+        return str(val).encode(encoding, 'replace').decode(encoding, 'replace')
 
 
 def remove_invalid_xml_chars(val):
     """
     Remove characters which aren't allowed in XML.
     :param val:
     :return:
```

### Comparing `maltego-trx-1.6.0/maltego_trx.egg-info/PKG-INFO` & `maltego-trx-1.6.1/maltego_trx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: maltego-trx
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python library used to develop Maltego transforms
 Home-page: https://github.com/paterva/maltego-trx/
 Author: Maltego Staff
 Author-email: support@maltego.com
 License: MIT
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Maltego TRX Python Library
 
-[![Runs with Python3.6 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml)
-[![PyTest with Python3.6 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml)
+[![Runs with Python3.8 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-boot-check.yaml)
+[![PyTest with Python3.8 - Python3.10](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/pythonx-pytest.yaml)
 [![Sonatype Jake](https://github.com/paterva/maltego-trx/actions/workflows/sonatype-jack.yml/badge.svg)](https://github.com/paterva/maltego-trx/actions/workflows/sonatype-jack.yml)
 
 ## Release Notes
 
+__1.6.1__: Update cryptography and Flask dependency and deprecate Python 3.7
+
 __1.6.0__: Automatically generate am `.mtz` for your local transforms
 
 __1.5.2__: Add logging output for invalid / missing params in xml serialization
 
 __1.5.1__: Add ignored files to starter and use README for pypi
 
 __1.5.0__: XML Serialization via `ElementTree` instead of string interpolation
@@ -29,15 +32,15 @@
 
 __1.4.0 + 1.4.1:__ Both versions are incompatible with python3.7 and lower.
 
 __1.4.2__: Fixed python3.6 incompatibility
 
 ## Getting Started
 
-_Note: Support for Python 2 has been officially discontinued as of July 2021. Please use Python 3.6 or higher to use
+_Note: Support for Python 2 has been officially discontinued as of July 2021. Please use Python 3.8 or higher to use
 up-to-date versions of Maltego TRX._
 
 To install the trx library run the following command:
 
 ``` bash
 pip install maltego-trx
 ```
```

### Comparing `maltego-trx-1.6.0/maltego_trx.egg-info/SOURCES.txt` & `maltego-trx-1.6.1/maltego_trx.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -29,8 +29,13 @@
 maltego_trx/template_dir/settings.csv
 maltego_trx/template_dir/settings.py
 maltego_trx/template_dir/transforms.csv
 maltego_trx/template_dir/transforms/DNSToIP.py
 maltego_trx/template_dir/transforms/GreetPerson.py
 maltego_trx/template_dir/transforms/GreetPersonLocalized.py
 maltego_trx/template_dir/transforms/OverlayExample.py
-maltego_trx/template_dir/transforms/__init__.py
+maltego_trx/template_dir/transforms/__init__.py
+tests/test.py
+tests/test_decorator_registry.py
+tests/test_mtz.py
+tests/test_property_mapping.py
+tests/test_xml.py
```

### Comparing `maltego-trx-1.6.0/setup.py` & `maltego-trx-1.6.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,32 +2,27 @@
 from maltego_trx import VERSION
 
 with open("README.md", "r") as readme_md:
     long_description = readme_md.read()
 
 setup(
     name='maltego-trx',
+    python_requires='>=3.8.0',
     version=VERSION,
     description='Python library used to develop Maltego transforms',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/paterva/maltego-trx/',
     author='Maltego Staff',
     author_email='support@maltego.com',
     license='MIT',
     install_requires=[
-        'flask>=1',
-        'six>=1',
-        'cryptography==3.3.2'  # pinned for now as newer versions require setuptools_rust
+        'flask>=2.2.0',
+        'cryptography>=39.0.1'
     ],
-    extras_require={
-        ':python_version == "3.6"': [
-            'dataclasses',
-        ],
-    },
     packages=[
         'maltego_trx',
         'maltego_trx/template_dir',
         'maltego_trx/template_dir/transforms',
     ],
     package_data={
         'maltego_trx/template_dir': [
```

