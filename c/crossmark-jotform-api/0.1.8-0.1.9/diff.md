# Comparing `tmp/crossmark-jotform-api-0.1.8.tar.gz` & `tmp/crossmark-jotform-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.1.8.tar", last modified: Thu Apr 27 06:42:02 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.1.9.tar", last modified: Thu Apr 27 07:04:10 2023, max compression
```

## Comparing `crossmark-jotform-api-0.1.8.tar` & `crossmark-jotform-api-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 06:42:02.984498 crossmark-jotform-api-0.1.8/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2159 2023-04-27 06:42:02.982505 crossmark-jotform-api-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.8/README.md
--rw-rw-rw-   0        0        0      789 2023-04-27 06:41:40.000000 crossmark-jotform-api-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 06:42:02.984498 crossmark-jotform-api-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 06:42:02.963497 crossmark-jotform-api-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 06:42:02.970499 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12022 2023-04-27 06:39:53.000000 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-27 06:42:02.980498 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2159 2023-04-27 06:42:02.000000 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-27 06:42:02.000000 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 06:42:02.000000 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-27 06:42:02.000000 crossmark-jotform-api-0.1.8/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.637871 crossmark-jotform-api-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2159 2023-04-27 07:04:10.635866 crossmark-jotform-api-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.9/README.md
+-rw-rw-rw-   0        0        0      789 2023-04-27 07:03:06.000000 crossmark-jotform-api-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:04:10.637871 crossmark-jotform-api-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.617869 crossmark-jotform-api-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.625869 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12041 2023-04-27 07:03:35.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:04:10.633866 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2159 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-27 07:04:10.000000 crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.1.8/LICENSE` & `crossmark-jotform-api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.1.8/PKG-INFO` & `crossmark-jotform-api-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.1.8/pyproject.toml` & `crossmark-jotform-api-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.1.8/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.1.9/src/crossmark_jotform_api/jotForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import ABC
 import requests
 from datetime import datetime
 from urllib.parse import quote
-import time
 
 
 class JotForm(ABC):
     def __init__(self, api_key, form_id, timeout=30, debug=False):
         self.update_timestamp = datetime.now().timestamp()
         self.api_key = api_key
         self.form_id = form_id
@@ -133,15 +132,16 @@
         else:
             self.url += "&" + key + "=" + value
 
     def _sort_submission_data_by_id(self):
         '''
             Sorts the submission data by id
         '''
-        sorted_tuples = sorted(self.submission_data.items(), key=lambda x: x[1].id, reverse=True)
+        sorted_tuples = sorted(self.submission_data.items(),
+                               key=lambda x: x[1].id, reverse=True)
         sorted_dict = {k: v for k, v in sorted_tuples}
         self.submission_data = sorted_dict
 
     def set_data(self):
         self.data = requests.get(self.url, timeout=self.timeout).json()
         count = self.data['resultSet']['count']
         self.submission_data.update(
```

### Comparing `crossmark-jotform-api-0.1.8/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.1.9/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

