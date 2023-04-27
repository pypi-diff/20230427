# Comparing `tmp/methodism-0.0.4.tar.gz` & `tmp/methodism-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.0.4.tar", last modified: Thu Apr 27 12:18:15 2023, max compression
+gzip compressed data, was "methodism-0.0.5.tar", last modified: Thu Apr 27 12:22:10 2023, max compression
```

## Comparing `methodism-0.0.4.tar` & `methodism-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:18:15.337525 methodism-0.0.4/
--rw-rw-rw-   0        0        0     2881 2023-04-27 12:18:15.353178 methodism-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2399 2023-04-27 08:27:37.000000 methodism-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:18:15.323960 methodism-0.0.4/base/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.4/base/__init__.py
--rw-rw-rw-   0        0        0     3559 2023-04-27 07:18:17.000000 methodism-0.0.4/base/costumizing.py
--rw-rw-rw-   0        0        0      708 2023-04-26 06:02:02.000000 methodism-0.0.4/base/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.4/base/error_messages.py
--rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.4/base/helper.py
--rw-rw-rw-   0        0        0     3493 2023-04-27 12:17:14.000000 methodism-0.0.4/base/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:18:15.337525 methodism-0.0.4/methodism.egg-info/
--rw-rw-rw-   0        0        0     2881 2023-04-27 12:18:15.000000 methodism-0.0.4/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-27 12:18:15.000000 methodism-0.0.4/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:18:15.000000 methodism-0.0.4/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 12:18:15.000000 methodism-0.0.4/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-04-27 12:17:23.000000 methodism-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-04-27 12:18:15.353178 methodism-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 12:22:10.542565 methodism-0.0.5/
+-rw-rw-rw-   0        0        0     2881 2023-04-27 12:22:10.542565 methodism-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2399 2023-04-27 08:27:37.000000 methodism-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 12:22:10.526535 methodism-0.0.5/base/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.5/base/__init__.py
+-rw-rw-rw-   0        0        0     3559 2023-04-27 07:18:17.000000 methodism-0.0.5/base/costumizing.py
+-rw-rw-rw-   0        0        0      708 2023-04-26 06:02:02.000000 methodism-0.0.5/base/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.5/base/error_messages.py
+-rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.5/base/helper.py
+-rw-rw-rw-   0        0        0     3492 2023-04-27 12:21:39.000000 methodism-0.0.5/base/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:22:10.542565 methodism-0.0.5/methodism.egg-info/
+-rw-rw-rw-   0        0        0     2881 2023-04-27 12:22:10.000000 methodism-0.0.5/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-27 12:22:10.000000 methodism-0.0.5/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:22:10.000000 methodism-0.0.5/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 12:22:10.000000 methodism-0.0.5/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-04-27 12:21:39.000000 methodism-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-04-27 12:22:10.542565 methodism-0.0.5/setup.cfg
```

### Comparing `methodism-0.0.4/PKG-INFO` & `methodism-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.4
+Version: 0.0.5
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.0.4/README.md` & `methodism-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `methodism-0.0.4/base/costumizing.py` & `methodism-0.0.5/base/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.4/base/decors.py` & `methodism-0.0.5/base/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.4/base/error_messages.py` & `methodism-0.0.5/base/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.4/base/helper.py` & `methodism-0.0.5/base/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.4/base/main.py` & `methodism-0.0.5/base/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     response_funk = custom_response  # must be funk(status, data, method ,message) return dict {}
 
     @method_and_params_checker
     def post(self, requests, *args, **kwargs):
         method = requests.data.get("method")
         params = requests.data.get("params")
         headers = requests.headers
-        if AllowAny not in self.permission_classes and method not in self.not_auth_methods:
+        if AllowAny not in self.permission_classes or method not in self.not_auth_methods:
             authorization = headers.get(self.auth_headers, '')
             pattern = re_compile(self.token_key + r" (.+)")
 
             if not pattern.match(authorization):
                 return Response(self.response_funk(status=False, method=method, message=MESSAGE['NotAuthenticated']))
             input_token = pattern.findall(authorization)[0]
```

### Comparing `methodism-0.0.4/methodism.egg-info/PKG-INFO` & `methodism-0.0.5/methodism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.4
+Version: 0.0.5
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.0.4/pyproject.toml` & `methodism-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.0.4/setup.cfg` & `methodism-0.0.5/setup.cfg`

 * *Files identical despite different names*

