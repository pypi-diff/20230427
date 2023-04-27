# Comparing `tmp/i2a_oauth2_api_client-2.0.9.tar.gz` & `tmp/i2a_oauth2_api_client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2a_oauth2_api_client-2.0.9.tar", last modified: Wed Jun 22 08:48:20 2022, max compression
+gzip compressed data, was "/home/bartlomiej/workspace/i2a-oauth-sdk/python_sdk/dist/.tmp-ztb42_ti/i2a_oauth2_api_client-3.0.1.tar", last modified: Thu Apr 27 13:59:49 2023, max compression
```

## Comparing `i2a_oauth2_api_client-2.0.9.tar` & `i2a_oauth2_api_client-3.0.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 admn      (1000) admn      (1000)        0 2022-06-22 08:48:20.943948 i2a_oauth2_api_client-2.0.9/
--rw-rw-r--   0 admn      (1000) admn      (1000)     1061 2022-06-22 08:46:09.000000 i2a_oauth2_api_client-2.0.9/LICENSE.txt
--rw-rw-r--   0 admn      (1000) admn      (1000)      818 2022-06-22 08:48:20.943948 i2a_oauth2_api_client-2.0.9/PKG-INFO
--rw-rw-r--   0 admn      (1000) admn      (1000)      433 2022-06-22 08:46:09.000000 i2a_oauth2_api_client-2.0.9/README.md
-drwxrwxr-x   0 admn      (1000) admn      (1000)        0 2022-06-22 08:48:20.943948 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client/
--rw-rw-r--   0 admn      (1000) admn      (1000)        0 2022-06-22 08:46:09.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client/__init__.py
--rw-rw-r--   0 admn      (1000) admn      (1000)    17032 2022-06-22 08:48:07.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client/client.py
--rw-rw-r--   0 admn      (1000) admn      (1000)       73 2022-06-22 08:46:09.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client/enums.py
--rw-rw-r--   0 admn      (1000) admn      (1000)      213 2022-06-22 08:46:55.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client/exceptions.py
-drwxrwxr-x   0 admn      (1000) admn      (1000)        0 2022-06-22 08:48:20.943948 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/
--rw-rw-r--   0 admn      (1000) admn      (1000)      818 2022-06-22 08:48:20.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 admn      (1000) admn      (1000)      387 2022-06-22 08:48:20.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 admn      (1000) admn      (1000)        1 2022-06-22 08:48:20.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 admn      (1000) admn      (1000)       17 2022-06-22 08:48:20.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/requires.txt
--rw-rw-r--   0 admn      (1000) admn      (1000)       22 2022-06-22 08:48:20.000000 i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/top_level.txt
--rw-rw-r--   0 admn      (1000) admn      (1000)       38 2022-06-22 08:48:20.943948 i2a_oauth2_api_client-2.0.9/setup.cfg
--rw-rw-r--   0 admn      (1000) admn      (1000)      758 2022-06-22 08:48:07.000000 i2a_oauth2_api_client-2.0.9/setup.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 13:59:49.979980 i2a_oauth2_api_client-3.0.1/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1061 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.1/LICENSE.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      818 2023-04-27 13:59:49.979980 i2a_oauth2_api_client-3.0.1/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      433 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.1/README.md
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 13:59:49.979980 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    23257 2023-04-25 12:18:20.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/client.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       73 2023-03-29 13:29:15.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/enums.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      270 2023-04-21 15:04:34.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/exceptions.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      936 2023-04-25 14:11:11.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/types.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1050 2023-04-13 10:07:54.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/validators.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 13:59:49.979980 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      818 2023-04-27 13:59:49.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      475 2023-04-27 13:59:49.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2023-04-27 13:59:49.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       17 2023-04-27 13:59:49.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/requires.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       22 2023-04-27 13:59:49.000000 i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/top_level.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2023-04-27 13:59:49.979980 i2a_oauth2_api_client-3.0.1/setup.cfg
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      787 2023-04-27 13:59:00.000000 i2a_oauth2_api_client-3.0.1/setup.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-04-27 13:59:49.979980 i2a_oauth2_api_client-3.0.1/tests/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1917 2023-04-21 15:10:26.000000 i2a_oauth2_api_client-3.0.1/tests/test_client.py
```

### Comparing `i2a_oauth2_api_client-2.0.9/LICENSE.txt` & `i2a_oauth2_api_client-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2a_oauth2_api_client-2.0.9/PKG-INFO` & `i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: i2a_oauth2_api_client
-Version: 2.0.9
+Name: i2a-oauth2-api-client
+Version: 3.0.1
 Summary: Sdk for i2a oauth2 api
 Download-URL: https://pypi.org/project/i2a_oauth2_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Oauth2 Client,I2A Oauth2 Api,I2A Oauth2,Python 3,I2A Oauth2 Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client/client.py` & `i2a_oauth2_api_client-3.0.1/i2a_oauth2_api_client/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,101 @@
 import requests
 import os
 from urllib.parse import urljoin
 
 from i2a_oauth2_api_client.exceptions import I2AOauth2ClientException
 from i2a_oauth2_api_client.enums import Environment
+from i2a_oauth2_api_client.types import MeData, TokenData, Page, AppLessS2SI2IdentityData
+from i2a_oauth2_api_client.validators import client_call, server_to_server_call, app_less_server_to_server_call
 
 
 class I2AOauth2Client:
-
     I2A_OAUTH2_API_QA_SERVER_URL = 'https://oauth2-qa.i2asolutions.com'
     I2A_OAUTH2_API_PROD_SERVER_URL = 'https://oauth2.i2asolutions.com'
     I2A_OAUTH2_API_ROOT_PATH = '/api/v2'
 
-    def __init__(self, client_id, client_secret, environment=Environment.QA):
+    def __init__(
+            self,
+            client_id: str = None,
+            client_secret: str = None,
+            user_group_secret: str = None,
+            app_less_secret: str = None,
+            server_name: str = None,
+            environment=Environment.QA
+    ):
         assert isinstance(environment, Environment)
 
         if environment is Environment.QA:
             self.__url = self.I2A_OAUTH2_API_QA_SERVER_URL
         elif environment is Environment.PROD:
             self.__url = self.I2A_OAUTH2_API_PROD_SERVER_URL
         else:
             raise NotImplementedError
 
         self.__environment = environment
         self.__client_id = client_id
         self.__client_secret = client_secret
+        self.__user_group_secret = user_group_secret
+        self.__app_less_secret = app_less_secret
+        self.__server_name = server_name
 
         self.headers = {
-            "Client-Id": self.__client_id
+            "Client-Id": self.__client_id,
+            "Application-User-Group-Secret": self.__user_group_secret,
         }
         self.server_to_server_headers = {
             "Client-Id": self.__client_id,
-            "Client-Secret": self.__client_secret
+            "Client-Secret": self.__client_secret,
+            "Application-User-Group-Secret": self.__user_group_secret,
+        }
+        self.app_less_server_to_server_headers = {
+            "Server-Secret": self.__app_less_secret,
+            "User-Agent": self.__server_name
         }
 
     @property
     def client_id(self):
         return self.__client_id
 
     @property
     def client_secret(self):
         return self.__client_secret
 
     @property
+    def user_group_secret(self):
+        return self.__user_group_secret
+
+    @property
+    def app_less_secret(self):
+        return self.__app_less_secret
+
+    @property
+    def server_name(self):
+        return self.__server_name
+
+    @property
     def url(self):
         return self.__url
 
     @property
     def environment(self):
         return self.__environment
 
+    @client_call
     def ping(self):
         url = self._get_full_url('ping/')
         response = requests.get(url, headers=self.headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Ping attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def register(
             self, email, password1, password2, first_name=None, last_name=None
     ):
         url = self._get_full_url('application-users/register/')
         data = {
             "username": email,
             "password1": password1,
@@ -78,56 +110,60 @@
         if response.status_code == 201:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Register attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
-    def get_token(self, email, password):
+    @client_call
+    def get_token(self, email, password) -> TokenData:
         url = self._get_full_url('auth/token/')
         data = {
             "grant_type": "password",
             "username": email,
             "password": password
         }
         response = requests.post(url, json=data, headers=self.headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Get token attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def refresh_token(self, refresh_token):
         url = self._get_full_url('auth/token/')
         data = {
             "grant_type": "refresh_token",
             "refresh_token": refresh_token
         }
         response = requests.post(url, json=data, headers=self.headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Refresh token attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def revoke_token(self, token):
         url = self._get_full_url('auth/revoke-token/')
         data = {
             "token": token,
         }
         response = requests.post(url, json=data, headers=self.headers)
         if response.status_code == 204:
             return
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Revoke token attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def convert_token(self, backend, social_app_token):
         url = self._get_full_url('auth/convert-token/')
         data = {
             "grant_type": "convert_token",
             "backend": backend,
             "token": social_app_token
         }
@@ -135,39 +171,42 @@
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Convert token attempt at {url} has failed failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
-    def get_me(self, token):
+    @client_call
+    def get_me(self, token) -> MeData:
         url = self._get_full_url('application-users/me/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
 
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Get me attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def get_my_application_user(self, token):
         url = self._get_full_url('application-users/my-application-user/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Get me attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def password_change(self, token, old_password, new_password1, new_password2):
         url = self._get_full_url('application-users/password-change/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
         data = {
             "old_password": old_password,
             "new_password1": new_password1,
@@ -177,38 +216,41 @@
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Password change attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def deactivate_account(self, token):
         url = self._get_full_url('application-users/deactivate-account/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
         response = requests.delete(url, headers=headers)
         if response.status_code == 204:
             return
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Deactivate account attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def delete_account(self, token):
         url = self._get_full_url('application-users/delete-account/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
         response = requests.delete(url, headers=headers)
         if response.status_code == 204:
             return
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Delete account attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def add_new_identity(self, token, email, password1, password2, first_name=None, last_name=None):
         url = self._get_full_url('add-new-identity/username-and-password/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
         data = {
             "username": email,
             "password1": password1,
@@ -223,14 +265,15 @@
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Add new identity attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @client_call
     def add_new_social_app_identity(self, token, backend, social_app_token):
         url = self._get_full_url('add-new-identity/social-app/')
         headers = self.headers.copy()
         headers['Authorization'] = f"Bearer {token}"
         data = {
             "client_id": self.client_id,
             "client_secret": self.client_secret,
@@ -245,24 +288,26 @@
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Add new social app identity attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_ping(self):
         url = self._get_full_url('server-to-server/ping/')
         response = requests.get(url, headers=self.server_to_server_headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Server to server ping attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_register(self, email, password1, password2, first_name=None, last_name=None):
         url = self._get_full_url('server-to-server/application-users/register/')
         data = {
             "username": email,
             "password1": password1,
             "password2": password2,
         }
@@ -275,38 +320,41 @@
         if response.status_code == 201:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(f'Server to server register attempt at {url} has failed for unknown reason.')
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_get_application_users(self):
         url = self._get_full_url('server-to-server/application-users/')
         response = requests.get(url, headers=self.server_to_server_headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server get application users attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_get_application_user(self, i2a_identifier):
         url = self._get_full_url(f'server-to-server/application-users/{i2a_identifier}/')
         response = requests.get(url, headers=self.server_to_server_headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server get application user attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_password_reset_request(self, email):
         url = self._get_full_url('server-to-server/application-users/password-reset-request/')
         data = {
             "username": email
         }
         response = requests.post(url, json=data, headers=self.server_to_server_headers)
         if response.status_code == 200:
@@ -314,14 +362,15 @@
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server password reset request attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_password_reset(self, code, new_password1, new_password2):
         url = self._get_full_url('server-to-server/application-users/password-reset/')
         data = {
             "code": str(code),
             "new_password1": new_password1,
             "new_password2": new_password2
         }
@@ -331,14 +380,15 @@
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server ot server password reset attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_password_reset_code_check(self, code):
         url = self._get_full_url('server-to-server/application-users/password-reset-code-check/')
         data = {
             "code": str(code)
         }
         response = requests.post(url, json=data, headers=self.server_to_server_headers)
         if response.status_code == 200:
@@ -346,14 +396,15 @@
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server password reset code check attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_username_change(self, old_email, new_email):
         url = self._get_full_url('server-to-server/application-users/username-change/')
         data = {
             "old_username": old_email,
             "new_username": new_email
         }
         response = requests.post(url, json=data, headers=self.server_to_server_headers)
@@ -362,45 +413,154 @@
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server username change attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_delete_account(self, i2a_identifier):
         url = self._get_full_url(f'server-to-server/application-users/delete-account/{i2a_identifier}/')
         response = requests.delete(url, headers=self.server_to_server_headers)
         if response.status_code == 204:
             return
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server delete account attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_get_application_user_groups(self):
         url = self._get_full_url(f'server-to-server/application-user-groups/')
         response = requests.delete(url, headers=self.server_to_server_headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server get application user groups attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @server_to_server_call
     def server_to_server_get_application_user_group(self, application_user_group_id):
         url = self._get_full_url(f'server-to-server/application-user-groups/{application_user_group_id}/')
         response = requests.delete(url, headers=self.server_to_server_headers)
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 500:
             raise I2AOauth2ClientException(
                 f'Server to server get application user group attempt at {url} has failed for unknown reason.'
             )
         else:
             raise I2AOauth2ClientException(data=response.json())
 
+    @app_less_server_to_server_call
+    def app_less_server_to_server_get_user_identity_details(
+        self, username: str, clients_ids: list[str], groups_identifiers: list[str]
+    ) -> AppLessS2SI2IdentityData:
+        url = self._get_full_url(f'server-to-server/app-less/users_identities/{username}/')
+        response = requests.get(url, headers=self.app_less_server_to_server_headers, params={
+            "clients_ids": clients_ids,
+            "groups_identifiers": groups_identifiers
+        })
+        if response.status_code == 200:
+            return response.json()
+        elif response.status_code == 500:
+            raise I2AOauth2ClientException(
+                f'App less Server to server get application user group attempt at {url} has failed for unknown reason.'
+            )
+        else:
+            raise I2AOauth2ClientException(data=response.json())
+
+    @app_less_server_to_server_call
+    def app_less_server_to_server_get_user_identity_list(
+        self, clients_ids: list[str], groups_identifiers: list[str],
+        page: int = 1, page_size: int = 25
+    ) -> Page[AppLessS2SI2IdentityData]:
+        url = self._get_full_url(f'server-to-server/app-less/users_identities/')
+        response = requests.get(url, headers=self.app_less_server_to_server_headers, params={
+            "clients_ids": clients_ids,
+            "groups_identifiers": groups_identifiers,
+            "page": page,
+            "page_size": page_size
+        })
+        if response.status_code == 200:
+            return response.json()
+        elif response.status_code == 500:
+            raise I2AOauth2ClientException(
+                f'App less Server to server get application user group attempt at {url} has failed for unknown reason.'
+            )
+        else:
+            raise I2AOauth2ClientException(data=response.json())
+
+    @app_less_server_to_server_call
+    def app_less_add_existing_identity_to_applications_groups(
+        self,
+        clients_ids: list[str], groups_identifiers: list[str],
+        to_groups_by_secrets: list[str], username
+    ) -> dict:
+        url = self._get_full_url(
+            f'server-to-server/app-less/users_identities/{username}/register_in_apps_using_identity/'
+        )
+        response = requests.post(
+            url,
+            headers=self.app_less_server_to_server_headers,
+            json={
+               "groups_secrets": to_groups_by_secrets
+            },
+            params={
+                "clients_ids": clients_ids,
+                "groups_identifiers": groups_identifiers,
+            }
+        )
+        if response.status_code == 201:
+            return response.json()
+        if response.status_code == 400:
+            raise I2AOauth2ClientException(data=response.json())
+        if response.status_code == 404:
+            raise I2AOauth2ClientException("Object does not exists.")
+        elif response.status_code == 500:
+            raise I2AOauth2ClientException(
+                f'App less Server to server get application user group attempt at {url} has failed for unknown reason.'
+            )
+        else:
+            raise I2AOauth2ClientException(data=response.json())
+
+    @app_less_server_to_server_call
+    def app_less_create_new_identity_in_applications_groups(
+            self,
+            to_groups_by_secrets: list[str],
+            username_email: str, password1: str, password2: str, first_name: str, last_name: str
+    ) -> dict:
+        url = self._get_full_url(
+            f'server-to-server/app-less/users_identities/create_identity_and_register_in_apps/'
+        )
+        response = requests.post(
+            url,
+            headers=self.app_less_server_to_server_headers,
+            json={
+                "groups_secrets": to_groups_by_secrets,
+                "password1": password1,
+                "password2": password1,
+                "first_name": first_name,
+                "last_name": last_name,
+                "username_email": username_email
+            },
+        )
+        if response.status_code == 201:
+            return response.json()
+        if response.status_code == 400:
+            raise I2AOauth2ClientException(data=response.json())
+        if response.status_code == 404:
+            raise I2AOauth2ClientException("Object does not exists.")
+        elif response.status_code == 500:
+            raise I2AOauth2ClientException(
+                f'App less Server to server get application user group attempt at {url} has failed for unknown reason.'
+            )
+        else:
+            raise I2AOauth2ClientException(data=response.json())
+
     def _get_full_url(self, resource_path):
         return urljoin(self.__url, os.path.join(self.I2A_OAUTH2_API_ROOT_PATH, resource_path))
```

### Comparing `i2a_oauth2_api_client-2.0.9/i2a_oauth2_api_client.egg-info/PKG-INFO` & `i2a_oauth2_api_client-3.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: i2a-oauth2-api-client
-Version: 2.0.9
+Name: i2a_oauth2_api_client
+Version: 3.0.1
 Summary: Sdk for i2a oauth2 api
 Download-URL: https://pypi.org/project/i2a_oauth2_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Oauth2 Client,I2A Oauth2 Api,I2A Oauth2,Python 3,I2A Oauth2 Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_oauth2_api_client-2.0.9/setup.py` & `i2a_oauth2_api_client-3.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='i2a_oauth2_api_client',
-    version='2.0.9',
+    version='3.0.1',
     description='Sdk for i2a oauth2 api',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     author='i2a Solutions Inc.',
     author_email='msyta@i2asolutions.com',
     keywords=['I2A Oauth2 Client', 'I2A Oauth2 Api', 'I2A Oauth2', 'Python 3', 'I2A Oauth2 Api SDK'],
     # url='',
-    download_url='https://pypi.org/project/i2a_oauth2_api_client/'
+    download_url='https://pypi.org/project/i2a_oauth2_api_client/',
 )
 
 install_requires = [
     'requests>=2.26.0',
 ]
 
 if __name__ == '__main__':
```

