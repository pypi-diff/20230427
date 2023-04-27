# Comparing `tmp/crossmark-jotform-api-0.1.1.tar.gz` & `tmp/crossmark-jotform-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.1.1.tar", last modified: Tue Apr 25 07:14:46 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.1.2.tar", last modified: Wed Apr 26 20:33:09 2023, max compression
```

## Comparing `crossmark-jotform-api-0.1.1.tar` & `crossmark-jotform-api-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 07:14:46.761909 crossmark-jotform-api-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1896 2023-04-25 07:14:46.760912 crossmark-jotform-api-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-04-25 07:13:15.000000 crossmark-jotform-api-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 07:14:46.761909 crossmark-jotform-api-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 07:14:46.743915 crossmark-jotform-api-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 07:14:46.748911 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    10452 2023-04-25 07:12:52.000000 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-25 07:14:46.758910 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     1896 2023-04-25 07:14:46.000000 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-25 07:14:46.000000 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 07:14:46.000000 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-25 07:14:46.000000 crossmark-jotform-api-0.1.1/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 20:33:09.259594 crossmark-jotform-api-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2159 2023-04-26 20:33:09.258594 crossmark-jotform-api-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.2/README.md
+-rw-rw-rw-   0        0        0      789 2023-04-26 20:30:41.000000 crossmark-jotform-api-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 20:33:09.259594 crossmark-jotform-api-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 20:33:09.242594 crossmark-jotform-api-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 20:33:09.249599 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    10745 2023-04-26 20:30:37.000000 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:33:09.256596 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2159 2023-04-26 20:33:09.000000 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-26 20:33:09.000000 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:33:09.000000 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 20:33:09.000000 crossmark-jotform-api-0.1.2/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.1.1/LICENSE` & `crossmark-jotform-api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.1.1/PKG-INFO` & `crossmark-jotform-api-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,7 +26,13 @@
 Project-URL: Bug Tracker, https://github.com/mirkan1/crossmark-jotform-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# jotform api library for python
+specilized for jotform api and crossmark needs
+
+# updates
+- 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
```

### Comparing `crossmark-jotform-api-0.1.1/pyproject.toml` & `crossmark-jotform-api-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.1.1/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.1.2/src/crossmark_jotform_api/jotForm.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,23 @@
             )
         )
         if count == self.data['resultSet']['limit']:
             self.set_url_param(
                 "offset", self.data['resultSet']['offset'] + count)
             return self.set_data()
         self.get_submission_ids()
+    
+    def set_new_submission(self, submission):
+        self.submission_data["submissions"].update(
+            self.__set_submission_data(
+                [submission]
+            )
+        )
+        self.submission_count += 1
+        self.submission_ids.append(submission['id'])
 
     def get_form(self):
         url = f"https://api.jotform.com/form/{self.form_id}?apiKey={self.api_key}"
         response = requests.request("GET", url, timeout=15)
         if response.status_code == 200:
             return response.json()
         else:
```

### Comparing `crossmark-jotform-api-0.1.1/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.1.2/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,7 +26,13 @@
 Project-URL: Bug Tracker, https://github.com/mirkan1/crossmark-jotform-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# jotform api library for python
+specilized for jotform api and crossmark needs
+
+# updates
+- 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
```

