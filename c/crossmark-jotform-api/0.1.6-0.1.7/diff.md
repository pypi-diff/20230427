# Comparing `tmp/crossmark-jotform-api-0.1.6.tar.gz` & `tmp/crossmark-jotform-api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.1.6.tar", last modified: Thu Apr 27 03:53:00 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.1.7.tar", last modified: Thu Apr 27 03:57:06 2023, max compression
```

## Comparing `crossmark-jotform-api-0.1.6.tar` & `crossmark-jotform-api-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 03:53:00.377478 crossmark-jotform-api-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2159 2023-04-27 03:53:00.377478 crossmark-jotform-api-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.6/README.md
--rw-rw-rw-   0        0        0      789 2023-04-27 03:44:12.000000 crossmark-jotform-api-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 03:53:00.377478 crossmark-jotform-api-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 03:53:00.351489 crossmark-jotform-api-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 03:53:00.371123 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    11405 2023-04-27 03:43:49.000000 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:53:00.377478 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2159 2023-04-27 03:53:00.000000 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-27 03:53:00.000000 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 03:53:00.000000 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-27 03:53:00.000000 crossmark-jotform-api-0.1.6/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 03:57:06.124745 crossmark-jotform-api-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2159 2023-04-27 03:57:06.123713 crossmark-jotform-api-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.7/README.md
+-rw-rw-rw-   0        0        0      789 2023-04-27 03:56:45.000000 crossmark-jotform-api-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 03:57:06.124745 crossmark-jotform-api-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 03:57:06.105480 crossmark-jotform-api-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 03:57:06.112694 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    11384 2023-04-27 03:56:40.000000 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:57:06.121775 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2159 2023-04-27 03:57:06.000000 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-27 03:57:06.000000 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 03:57:06.000000 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-27 03:57:06.000000 crossmark-jotform-api-0.1.7/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.1.6/LICENSE` & `crossmark-jotform-api-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.1.6/PKG-INFO` & `crossmark-jotform-api-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.1.6/pyproject.toml` & `crossmark-jotform-api-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.1.6/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.1.7/src/crossmark_jotform_api/jotForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from abc import ABC
 import requests
 from datetime import datetime
 from urllib.parse import quote
 
 
 class JotForm(ABC):
-    version = 1.2
-
     def __init__(self, api_key, form_id, timeout=30):
         self.update_timestamp = datetime.now().timestamp()
         self.api_key = api_key
         self.form_id = form_id
         self.url = "https://api.jotform.com/form/" + form_id + \
             "/submissions?limit=1000&apiKey=" + api_key
         self.set_url_param("offset", "0")
```

### Comparing `crossmark-jotform-api-0.1.6/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.1.7/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

