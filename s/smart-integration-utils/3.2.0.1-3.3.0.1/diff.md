# Comparing `tmp/smart-integration-utils-3.2.0.1.tar.gz` & `tmp/smart-integration-utils-3.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart-integration-utils-3.2.0.1.tar", last modified: Wed Oct 26 09:43:50 2022, max compression
+gzip compressed data, was "smart-integration-utils-3.3.0.1.tar", last modified: Thu Apr 27 11:27:46 2023, max compression
```

## Comparing `smart-integration-utils-3.2.0.1.tar` & `smart-integration-utils-3.3.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-10-26 09:43:50.201665 smart-integration-utils-3.2.0.1/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2022-10-26 09:43:50.201665 smart-integration-utils-3.2.0.1/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    11362 2022-10-25 11:05:32.000000 smart-integration-utils-3.2.0.1/README.md
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-10-26 09:43:50.201665 smart-integration-utils-3.2.0.1/integration_utils/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       46 2022-10-26 09:43:42.000000 smart-integration-utils-3.2.0.1/integration_utils/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1818 2022-10-25 12:44:54.000000 smart-integration-utils-3.2.0.1/integration_utils/comparison.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      814 2022-10-25 12:44:54.000000 smart-integration-utils-3.2.0.1/integration_utils/exceptions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      912 2022-10-25 11:05:32.000000 smart-integration-utils-3.2.0.1/integration_utils/fields.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7867 2022-10-25 11:05:32.000000 smart-integration-utils-3.2.0.1/integration_utils/filters.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4640 2022-10-26 09:43:42.000000 smart-integration-utils-3.2.0.1/integration_utils/mixins.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3333 2022-10-25 12:44:54.000000 smart-integration-utils-3.2.0.1/integration_utils/pagination.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1970 2022-10-25 11:05:32.000000 smart-integration-utils-3.2.0.1/integration_utils/serializers.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7266 2022-10-25 11:05:32.000000 smart-integration-utils-3.2.0.1/integration_utils/services.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    14281 2022-10-26 07:44:24.000000 smart-integration-utils-3.2.0.1/integration_utils/tools.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3341 2022-10-25 11:05:32.000000 smart-integration-utils-3.2.0.1/integration_utils/utils.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4668 2022-10-25 12:44:54.000000 smart-integration-utils-3.2.0.1/integration_utils/views.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2022-10-26 09:43:50.201665 smart-integration-utils-3.2.0.1/setup.cfg
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      535 2022-10-25 14:02:55.000000 smart-integration-utils-3.2.0.1/setup.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-10-26 09:43:50.201665 smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2022-10-26 09:43:50.000000 smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      607 2022-10-26 09:43:50.000000 smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2022-10-26 09:43:50.000000 smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      104 2022-10-26 09:43:50.000000 smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/requires.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2022-10-26 09:43:50.000000 smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/top_level.txt
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 11:27:46.526996 smart-integration-utils-3.3.0.1/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-04-27 11:27:46.526996 smart-integration-utils-3.3.0.1/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    11362 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.1/README.md
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 11:27:46.526996 smart-integration-utils-3.3.0.1/integration_utils/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       46 2023-04-27 11:27:36.000000 smart-integration-utils-3.3.0.1/integration_utils/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1818 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.1/integration_utils/comparison.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      814 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.1/integration_utils/exceptions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      912 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.1/integration_utils/fields.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7867 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.1/integration_utils/filters.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4708 2023-04-27 11:27:36.000000 smart-integration-utils-3.3.0.1/integration_utils/mixins.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3333 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.1/integration_utils/pagination.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1970 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.1/integration_utils/serializers.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7266 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.1/integration_utils/services.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    14497 2023-04-27 11:27:36.000000 smart-integration-utils-3.3.0.1/integration_utils/tools.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3341 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.1/integration_utils/utils.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4668 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.1/integration_utils/views.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-04-27 11:27:46.526996 smart-integration-utils-3.3.0.1/setup.cfg
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      535 2022-10-25 14:02:55.000000 smart-integration-utils-3.3.0.1/setup.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 11:27:46.526996 smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-04-27 11:27:46.000000 smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      607 2023-04-27 11:27:46.000000 smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-04-27 11:27:46.000000 smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      104 2023-04-27 11:27:46.000000 smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/requires.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-04-27 11:27:46.000000 smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/top_level.txt
```

### Comparing `smart-integration-utils-3.2.0.1/README.md` & `smart-integration-utils-3.3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/comparison.py` & `smart-integration-utils-3.3.0.1/integration_utils/comparison.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/exceptions.py` & `smart-integration-utils-3.3.0.1/integration_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/fields.py` & `smart-integration-utils-3.3.0.1/integration_utils/fields.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/filters.py` & `smart-integration-utils-3.3.0.1/integration_utils/filters.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/mixins.py` & `smart-integration-utils-3.3.0.1/integration_utils/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     if hasattr(settings, 'IS_BOX_APP') and settings.IS_BOX_APP:
         url = f'{settings.AUTH_URL}'
         header_param = 'Authorization'
     else:
         url = f'{url}api/check-platform/'
         header_param = 'executetoken'
+    ssl_verify: bool = True
 
     def get_user_info(
         self, request, **kwargs
     ):  # **kwargs for old versions compatibility
         if 'token' in request.GET and "platform_id" in request.GET:
             token = unquote(request.GET["token"])
         elif 'HTTP_AUTHORIZATION' in request.META and "platform_id" in request.GET:
@@ -36,14 +37,15 @@
             raise PermissionDenied(
                 {"status": "error", "message": "you don't have permission to access"}
             )
         try:
             response = requests.get(
                 f"{self.url}?platform_id={request.GET['platform_id']}",
                 headers={self.header_param: token},
+                verify=self.ssl_verify,
             )
         except requests.ConnectionError:
             raise PermissionDenied(
                 {"status": "error", "message": "Authorization failed."}
             )
 
         if response.status_code != 200:
```

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/pagination.py` & `smart-integration-utils-3.3.0.1/integration_utils/pagination.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/serializers.py` & `smart-integration-utils-3.3.0.1/integration_utils/serializers.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/services.py` & `smart-integration-utils-3.3.0.1/integration_utils/services.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/tools.py` & `smart-integration-utils-3.3.0.1/integration_utils/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,52 +57,56 @@
     while switcher[0] == True:
         try:
             yield inner(iterator, max_value, switcher)
         except StopIteration:
             return None
 
 
-def get_smart_token(platform: str) -> str:
+def get_smart_token(platform: str, verify: bool = True) -> str:
     """
     :param platform: str (prod or dev)
     :return: str
     """
     if hasattr(settings, 'IS_BOX_APP') and settings.IS_BOX_APP:
         r = requests.post(
             settings.AUTH_TOKEN_URL,
             json={
                 'username': settings.ADMIN_USERNAME,
                 'password': settings.ADMIN_USER_PASSWORD,
             },
+            verify=verify,
         ).json()
         return r['access']['value']
     else:
         url = f'{DASHBOARD_URL}api/smart_tokens/?platform_id={platform}'
         token = settings.EXECUTE_TOKEN
         try:
-            r = requests.get(url, headers={"executetoken": token}).json()
+            r = requests.get(url, headers={"executetoken": token}, verify=verify).json()
         except (requests.ConnectionError, json.JSONDecodeError):
             return 'error'
         return r['token']
 
 
 def get_integration_info(
-    platform: str, integration_id: int, token: Optional[str] = None
+    platform: str,
+    integration_id: int,
+    token: Optional[str] = None,
+    verify: bool = True,
 ) -> dict:
     if hasattr(settings, 'IS_BOX_APP') and settings.IS_BOX_APP:
         headers = {"Authorization": settings.AUTH_TOKEN}
         integration_url = f'{DASHBOARD_URL}/integrations/{integration_id}'
     else:
         if not token:
-            token = get_smart_token(platform)
+            token = get_smart_token(platform, verify)
         config_url = f'{DASHBOARD_URL}api/get_config_url/?platform_id={platform}'
-        dash_response = requests.get(f'{config_url}').json()
+        dash_response = requests.get(f'{config_url}', verify=verify).json()
         headers = {"Authorization": token}
         integration_url = f'{dash_response["config_url"]}{integration_id}/'
-    integration = requests.get(integration_url, headers=headers).json()
+    integration = requests.get(integration_url, headers=headers, verify=verify).json()
     return integration
 
 
 def delete_file(filename: str):
     os.remove(filename)
 
 
@@ -220,32 +224,36 @@
 
 def chunk_by_items(items: list, step: int):
     """Yield successive n-sized chunks from l."""
     for i in range(0, len(items), step):
         yield items[i : i + step]
 
 
-def get_full_integrations(platform: str, service_code: str) -> list:
+def get_full_integrations(
+    platform: str,
+    service_code: str,
+    verify: bool = True,
+) -> list:
     """
     :param platform: str (prod or dev)
     :param service_code: str (code from integration config)
     :return: list (list of integrations)
     """
     token = get_smart_token(platform)
     url = f'{DASHBOARD_URL}api/get_config_url/'
-    dash_response = requests.get(f'{url}?platform_id={platform}').json()
+    dash_response = requests.get(f'{url}?platform_id={platform}', verify=verify).json()
     headers = {"Authorization": token}
 
     config_url = f'{dash_response["config_url"]}?type__code={service_code}&all=1'
     # print(config_url)
 
-    configs = requests.get(config_url, headers=headers).json()
+    configs = requests.get(config_url, headers=headers, verify=verify).json()
     results = configs["results"]
     while configs["next"]:
-        configs = requests.get(configs["next"], headers=headers).json()
+        configs = requests.get(configs["next"], headers=headers, verify=verify).json()
         results.extend(configs["results"])
     return results
 
 
 def check_entities_equal(
     db_entity: Any, new_entity: Any, exclude_fields: Union[list, tuple, None] = None
 ) -> bool:
```

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/utils.py` & `smart-integration-utils-3.3.0.1/integration_utils/utils.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/integration_utils/views.py` & `smart-integration-utils-3.3.0.1/integration_utils/views.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/setup.py` & `smart-integration-utils-3.3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.2.0.1/smart_integration_utils.egg-info/SOURCES.txt` & `smart-integration-utils-3.3.0.1/smart_integration_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

