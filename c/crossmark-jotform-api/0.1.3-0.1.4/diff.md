# Comparing `tmp/crossmark-jotform-api-0.1.3.tar.gz` & `tmp/crossmark-jotform-api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.1.3.tar", last modified: Wed Apr 26 20:42:37 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.1.4.tar", last modified: Thu Apr 27 02:33:20 2023, max compression
```

## Comparing `crossmark-jotform-api-0.1.3.tar` & `crossmark-jotform-api-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:42:37.853663 crossmark-jotform-api-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2159 2023-04-26 20:42:37.852668 crossmark-jotform-api-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.3/README.md
--rw-rw-rw-   0        0        0      789 2023-04-26 20:42:08.000000 crossmark-jotform-api-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 20:42:37.854664 crossmark-jotform-api-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 20:42:37.835663 crossmark-jotform-api-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:42:37.841661 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    11325 2023-04-26 20:41:16.000000 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:42:37.850661 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2159 2023-04-26 20:42:37.000000 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-26 20:42:37.000000 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:42:37.000000 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-26 20:42:37.000000 crossmark-jotform-api-0.1.3/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 02:33:20.800457 crossmark-jotform-api-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2159 2023-04-27 02:33:20.799458 crossmark-jotform-api-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-26 20:32:45.000000 crossmark-jotform-api-0.1.4/README.md
+-rw-rw-rw-   0        0        0      789 2023-04-27 02:30:24.000000 crossmark-jotform-api-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 02:33:20.800457 crossmark-jotform-api-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 02:33:20.779457 crossmark-jotform-api-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 02:33:20.786459 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    11373 2023-04-27 02:31:43.000000 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:33:20.796458 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2159 2023-04-27 02:33:20.000000 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-27 02:33:20.000000 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 02:33:20.000000 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-27 02:33:20.000000 crossmark-jotform-api-0.1.4/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.1.3/LICENSE` & `crossmark-jotform-api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.1.3/PKG-INFO` & `crossmark-jotform-api-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.1.3/pyproject.toml` & `crossmark-jotform-api-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.1.3/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.1.4/src/crossmark_jotform_api/jotForm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 from datetime import datetime
 from urllib.parse import quote
 
 
 class JotForm(ABC):
     version = 1.2
 
-    def __init__(self, api_key, form_id):
+    def __init__(self, api_key, form_id, timeout=30):
         self.update_timestamp = datetime.now().timestamp()
         self.api_key = api_key
         self.form_id = form_id
         self.url = "https://api.jotform.com/form/" + form_id + \
             "/submissions?limit=1000&apiKey=" + api_key
         self.set_url_param("offset", "0")
         self.submission_ids = []
         self.submission_data = {}
         self.updating_process = False
         self.submission_count = 0
         self.submissions = []
         self.submission_data["submissions"] = {}
         self.set_data()
+        self.timeout = timeout
 
     def __set_submission_data(self, submission_data):
         submissions_dict = {}
         for i in submission_data:
             submissions_dict[i["id"]] = jotFormSubmission(i)
         return submissions_dict
 
@@ -44,15 +45,15 @@
 
     def get_submission_answers(self, submission_id):
         self.update()
         return self.submission_data["submissions"][submission_id].answers
 
     def get_submission_by_request(self, submission_id):
         requests.get("https://api.jotform.com/submission/" +
-                     submission_id + "?apiKey=" + self.api_key, timeout=15)
+                     submission_id + "?apiKey=" + self.api_key, self.timeout)
 
     def get_submission(self, submission_id):
         self.update()
         return self.submission_data["submissions"][submission_id]
 
     def get_submission_id_by_text(self, text):
         self.update()
@@ -103,15 +104,15 @@
             submission_answers_by_question_id[answer["id"]] = answer["answer"]
 
     def update_submission_answer(self, submission_id, answer_id, answer):
         self.update()
         query = f'submission[{answer_id}]={answer}'
         # &submission[{rsrEmailFieldId}]={email}&submission[{actionerSupervisorEmailField}]={actionerSupervisorEmail.lower()}&submission[{actionerSupervisorNameField}]={actionerSupervisorName.lower()}'
         url = f"https://api.jotform.com/submission/{submission_id}?apiKey={self.api_key}&{query}"
-        response = requests.request("POST", url, timeout=15)
+        response = requests.request("POST", url, self.timeout)
         if response.status_code == 200:
             return True
         else:
             return False
 
     def set_url_param(self, key, value):
         value = str(value)
@@ -122,15 +123,15 @@
                 if key in params[i]:
                     params[i] = key + "=" + value
             self.url = "&".join(params)
         else:
             self.url += "&" + key + "=" + value
 
     def set_data(self):
-        self.data = requests.get(self.url, timeout=15).json()
+        self.data = requests.get(self.url, self.timeout).json()
         count = self.data['resultSet']['count']
         self.submission_count += count
         self.submission_data["submissions"].update(
             self.__set_submission_data(
                 self.data['content']
             )
         )
@@ -144,27 +145,27 @@
         query = quote(f'''{{"q221:matches:answer":"{case_id}"}}''')
         url = f"https://api.jotform.com/form/{self.form_id}/submissions?apiKey={self.api_key}&filter={query}"
         response = requests.get(url)
         if response.status_code != 200:
             return None
         _json = response.json()
         return _json
-    
+
     def set_new_submission(self, submission):
         self.submission_data["submissions"].update(
             self.__set_submission_data(
                 [submission]
             )
         )
         self.submission_count += 1
         self.submission_ids.append(submission['id'])
 
     def get_form(self):
         url = f"https://api.jotform.com/form/{self.form_id}?apiKey={self.api_key}"
-        response = requests.request("GET", url, timeout=15)
+        response = requests.request("GET", url, self.timeout)
         if response.status_code == 200:
             return response.json()
         else:
             return None
 
     def get_submissions_count(self):
         form = self.get_form()
```

### Comparing `crossmark-jotform-api-0.1.3/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.1.4/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

