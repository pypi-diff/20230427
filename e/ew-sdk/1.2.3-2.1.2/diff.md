# Comparing `tmp/ew-sdk-1.2.3.tar.gz` & `tmp/ew-sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ew-sdk-1.2.3.tar", last modified: Thu Apr 27 11:21:28 2023, max compression
+gzip compressed data, was "ew-sdk-2.1.2.tar", last modified: Thu Apr 27 10:06:34 2023, max compression
```

## Comparing `ew-sdk-1.2.3.tar` & `ew-sdk-2.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.081828 ew-sdk-1.2.3/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-27 11:21:28.081828 ew-sdk-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2562 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.071828 ew-sdk-1.2.3/apimaticcalculator/
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/apimaticcalculator_client.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.073828 ew-sdk-1.2.3/apimaticcalculator/controllers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/controllers/simple_calculator_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.074828 ew-sdk-1.2.3/apimaticcalculator/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.077828 ew-sdk-1.2.3/apimaticcalculator/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.078828 ew-sdk-1.2.3/apimaticcalculator/models/
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/models/operation_type_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.079828 ew-sdk-1.2.3/apimaticcalculator/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/apimaticcalculator/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:21:28.081828 ew-sdk-1.2.3/ew_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-27 11:21:28.000000 ew-sdk-1.2.3/ew_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-27 11:21:28.000000 ew-sdk-1.2.3/ew_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:21:28.000000 ew-sdk-1.2.3/ew_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-27 11:21:28.000000 ew-sdk-1.2.3/ew_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 11:21:28.000000 ew-sdk-1.2.3/ew_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-27 11:21:01.000000 ew-sdk-1.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-27 11:21:28.082828 ew-sdk-1.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.528054 ew-sdk-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-27 10:06:34.528054 ew-sdk-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.509053 ew-sdk-2.1.2/apimaticcalculator/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/apimaticcalculator_client.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.511053 ew-sdk-2.1.2/apimaticcalculator/controllers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/controllers/simple_calculator_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.511053 ew-sdk-2.1.2/apimaticcalculator/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.517053 ew-sdk-2.1.2/apimaticcalculator/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.521053 ew-sdk-2.1.2/apimaticcalculator/models/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/models/operation_type_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.522053 ew-sdk-2.1.2/apimaticcalculator/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/apimaticcalculator/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:06:34.528054 ew-sdk-2.1.2/ew_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-27 10:06:34.000000 ew-sdk-2.1.2/ew_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-27 10:06:34.000000 ew-sdk-2.1.2/ew_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 10:06:34.000000 ew-sdk-2.1.2/ew_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-27 10:06:34.000000 ew-sdk-2.1.2/ew_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 10:06:34.000000 ew-sdk-2.1.2/ew_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-27 10:05:48.000000 ew-sdk-2.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-27 10:06:34.530054 ew-sdk-2.1.2/setup.cfg
```

### Comparing `ew-sdk-1.2.3/LICENSE` & `ew-sdk-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/README.md` & `ew-sdk-2.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.10`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install ew-sdk==1.2.3
+pip install ew-sdk==2.1.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/ew-sdk/1.2.3
+https://pypi.python.org/pypi/ew-sdk/2.1.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
```

### Comparing `ew-sdk-1.2.3/apimaticcalculator/api_helper.py` & `ew-sdk-2.1.2/apimaticcalculator/api_helper.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/apimaticcalculator_client.py` & `ew-sdk-2.1.2/apimaticcalculator/apimaticcalculator_client.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/configuration.py` & `ew-sdk-2.1.2/apimaticcalculator/configuration.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/controllers/base_controller.py` & `ew-sdk-2.1.2/apimaticcalculator/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/controllers/simple_calculator_controller.py` & `ew-sdk-2.1.2/apimaticcalculator/controllers/simple_calculator_controller.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/exceptions/api_exception.py` & `ew-sdk-2.1.2/apimaticcalculator/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/http/http_request.py` & `ew-sdk-2.1.2/apimaticcalculator/http/http_request.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/http/http_response.py` & `ew-sdk-2.1.2/apimaticcalculator/http/http_response.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/apimaticcalculator/models/operation_type_enum.py` & `ew-sdk-2.1.2/apimaticcalculator/models/operation_type_enum.py`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/ew_sdk.egg-info/SOURCES.txt` & `ew-sdk-2.1.2/ew_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ew-sdk-1.2.3/pyproject.toml` & `ew-sdk-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "ew-sdk"
 description = "few"
-version = "1.2.3"
+version = "2.1.2"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "ewqf", email = "qw2@g.com"}]
 urls = {}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
```

