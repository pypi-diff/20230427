# Comparing `tmp/oauth2-client-1.4.0.tar.gz` & `tmp/oauth2-client-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oauth2-client-1.4.0.tar", last modified: Fri Apr 14 08:57:25 2023, max compression
+gzip compressed data, was "dist/oauth2-client-1.4.1.tar", last modified: Thu Apr 27 21:01:42 2023, max compression
```

## Comparing `oauth2-client-1.4.0.tar` & `oauth2-client-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/
--rw-rw-r--   0 root         (0) root         (0)    11347 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       38 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7870 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7184 2023-02-02 15:04:57.000000 oauth2-client-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/main/oauth2_client/
--rw-rw-r--   0 root         (0) root         (0)       22 2023-04-14 08:49:18.000000 oauth2-client-1.4.0/main/oauth2_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12958 2023-04-14 08:48:55.000000 oauth2-client-1.4.0/main/oauth2_client/credentials_manager.py
--rw-rw-r--   0 root         (0) root         (0)     2324 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/main/oauth2_client/http_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7870 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:55:11.000000 oauth2-client-1.4.0/oauth2_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/oauth2_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       15 2022-12-03 11:03:06.000000 oauth2-client-1.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 08:57:25.000000 oauth2-client-1.4.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1567 2023-02-02 14:51:28.000000 oauth2-client-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/
+-rw-rw-r--   0 root         (0) root         (0)    11347 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       38 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7184 2023-02-02 15:04:57.000000 oauth2-client-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/main/oauth2_client/
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-04-27 21:00:33.000000 oauth2-client-1.4.1/main/oauth2_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13047 2023-04-27 21:00:22.000000 oauth2-client-1.4.1/main/oauth2_client/credentials_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2324 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/main/oauth2_client/http_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1567 2023-02-02 14:51:28.000000 oauth2-client-1.4.1/setup.py
```

### Comparing `oauth2-client-1.4.0/LICENSE` & `oauth2-client-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.4.0/PKG-INFO` & `oauth2-client-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-client
-Version: 1.4.0
+Version: 1.4.1
 Summary: A client library for OAuth2
 Home-page: http://github.com/antechrestos/OAuth2Client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `oauth2-client-1.4.0/README.rst` & `oauth2-client-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.4.0/main/oauth2_client/credentials_manager.py` & `oauth2-client-1.4.1/main/oauth2_client/credentials_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 
     def _token_request(self, request_parameters: dict, refresh_token_mandatory: bool):
         headers = self._token_request_headers(request_parameters['grant_type'])
         if self.service_information.auth:
             headers['Authorization'] = 'Basic %s' % self.service_information.auth
         else:
             request_parameters["client_id"] = self.service_information.client_id
+            request_parameters["client_secret"] = self.service_information.client_secret
         response = requests.post(self.service_information.token_service,
                                  data=request_parameters,
                                  headers=headers,
                                  proxies=self.proxies,
                                  verify=self.service_information.verify)
         if response.status_code != HTTPStatus.OK.value:
             CredentialManager._handle_bad_response(response)
```

### Comparing `oauth2-client-1.4.0/main/oauth2_client/http_server.py` & `oauth2-client-1.4.1/main/oauth2_client/http_server.py`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.4.0/oauth2_client.egg-info/PKG-INFO` & `oauth2-client-1.4.1/oauth2_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-client
-Version: 1.4.0
+Version: 1.4.1
 Summary: A client library for OAuth2
 Home-page: http://github.com/antechrestos/OAuth2Client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `oauth2-client-1.4.0/setup.py` & `oauth2-client-1.4.1/setup.py`

 * *Files identical despite different names*

