# Comparing `tmp/smart-manage-app-client-0.1.0b0.tar.gz` & `tmp/smart-manage-app-client-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart-manage-app-client-0.1.0b0.tar", last modified: Thu Jul 21 07:40:19 2022, max compression
+gzip compressed data, was "smart-manage-app-client-0.2.0b0.tar", last modified: Thu Apr 27 14:18:14 2023, max compression
```

## Comparing `smart-manage-app-client-0.1.0b0.tar` & `smart-manage-app-client-0.2.0b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-07-21 07:40:19.889774 smart-manage-app-client-0.1.0b0/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      199 2022-07-21 07:40:19.889774 smart-manage-app-client-0.1.0b0/PKG-INFO
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)     1669 2020-10-28 10:29:41.000000 smart-manage-app-client-0.1.0b0/README.md
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-07-21 07:40:19.885774 smart-manage-app-client-0.1.0b0/manage_app_client/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      126 2022-01-28 12:31:09.000000 smart-manage-app-client-0.1.0b0/manage_app_client/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4940 2022-07-21 07:39:49.000000 smart-manage-app-client-0.1.0b0/manage_app_client/client.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4408 2022-01-28 12:35:03.000000 smart-manage-app-client-0.1.0b0/manage_app_client/decorator.py
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)      800 2020-10-22 10:33:16.000000 smart-manage-app-client-0.1.0b0/manage_app_client/settings.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1687 2022-07-21 07:39:49.000000 smart-manage-app-client-0.1.0b0/manage_app_client/tools.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3494 2022-07-21 07:32:41.000000 smart-manage-app-client-0.1.0b0/manage_app_client/utils.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2022-07-21 07:40:19.889774 smart-manage-app-client-0.1.0b0/setup.cfg
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      215 2022-07-21 07:39:49.000000 smart-manage-app-client-0.1.0b0/setup.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-07-21 07:40:19.889774 smart-manage-app-client-0.1.0b0/smart_manage_app_client.egg-info/
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)      199 2022-07-21 07:40:19.000000 smart-manage-app-client-0.1.0b0/smart_manage_app_client.egg-info/PKG-INFO
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)      425 2022-07-21 07:40:19.000000 smart-manage-app-client-0.1.0b0/smart_manage_app_client.egg-info/SOURCES.txt
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)        1 2022-07-21 07:40:19.000000 smart-manage-app-client-0.1.0b0/smart_manage_app_client.egg-info/dependency_links.txt
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)       41 2022-07-21 07:40:19.000000 smart-manage-app-client-0.1.0b0/smart_manage_app_client.egg-info/requires.txt
--rw-r--r--   0 bzdv      (1000) bzdv      (1000)       18 2022-07-21 07:40:19.000000 smart-manage-app-client-0.1.0b0/smart_manage_app_client.egg-info/top_level.txt
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 14:18:14.909699 smart-manage-app-client-0.2.0b0/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       69 2023-04-27 14:18:14.909699 smart-manage-app-client-0.2.0b0/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1669 2022-10-25 13:12:40.000000 smart-manage-app-client-0.2.0b0/README.md
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 14:18:14.909699 smart-manage-app-client-0.2.0b0/manage_app_client/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      126 2022-10-25 13:12:40.000000 smart-manage-app-client-0.2.0b0/manage_app_client/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5291 2023-04-27 14:16:09.000000 smart-manage-app-client-0.2.0b0/manage_app_client/client.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4762 2023-04-27 14:14:19.000000 smart-manage-app-client-0.2.0b0/manage_app_client/decorator.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      800 2023-04-27 14:12:49.000000 smart-manage-app-client-0.2.0b0/manage_app_client/settings.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1780 2023-04-27 14:17:45.000000 smart-manage-app-client-0.2.0b0/manage_app_client/tools.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3494 2022-10-25 13:12:40.000000 smart-manage-app-client-0.2.0b0/manage_app_client/utils.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-04-27 14:18:14.909699 smart-manage-app-client-0.2.0b0/setup.cfg
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      215 2023-04-27 14:16:15.000000 smart-manage-app-client-0.2.0b0/setup.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 14:18:14.909699 smart-manage-app-client-0.2.0b0/smart_manage_app_client.egg-info/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       69 2023-04-27 14:18:14.000000 smart-manage-app-client-0.2.0b0/smart_manage_app_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      425 2023-04-27 14:18:14.000000 smart-manage-app-client-0.2.0b0/smart_manage_app_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-04-27 14:18:14.000000 smart-manage-app-client-0.2.0b0/smart_manage_app_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       41 2023-04-27 14:18:14.000000 smart-manage-app-client-0.2.0b0/smart_manage_app_client.egg-info/requires.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-04-27 14:18:14.000000 smart-manage-app-client-0.2.0b0/smart_manage_app_client.egg-info/top_level.txt
```

### Comparing `smart-manage-app-client-0.1.0b0/README.md` & `smart-manage-app-client-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `smart-manage-app-client-0.1.0b0/manage_app_client/client.py` & `smart-manage-app-client-0.2.0b0/manage_app_client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 import logging
 from typing import Optional
 from requests import post, ConnectionError
 
 logger = logging.getLogger('manage_app_client')
 
 
-def _request(url: str, data: dict, headers: dict) -> bool:
+def _request(
+    url: str,
+    data: dict,
+    headers: dict,
+    ssl_verify: bool = True,
+) -> bool:
     """Requests helper
 
     Args:
         url (str): manage system url
         data (dict): event data or exceptio data
         headers (dict): auth headers
 
     Returns:
         bool: True if success else False
     """
     try:
-        r = post(url, json=data, headers=headers)
+        r = post(url, json=data, headers=headers, verify=ssl_verify)
         if r.status_code > 204:
             warnings.warn(
                 f'Invalid response status: {r.status_code}, check Manage app settings'
             )
             return False
         return True
     except ConnectionError as e:
@@ -60,14 +65,15 @@
 
     def push_event(
         self,
         definition: dict,
         start_time: str,
         status: bool = False,
         description: Optional[str] = None,
+        ssl_verify: bool = True,
     ) -> bool:
         """Push event data
 
         Args:
             definition (dict): definition of event
             status (bool, optional): finisth status. Defaults to False.
 
@@ -92,24 +98,26 @@
         else:
             data["start_time"] = start_time
             data["finish_time"] = None
         return _request(
             f'{self.system_url}api/events/?system_id={self.system_id}',
             data=data,
             headers=headers,
+            ssl_verify=ssl_verify,
         )
 
     def push_exception(
         self,
         definition: dict,
         description: str,
         start_time: str,
         is_auth: bool = False,
         trb: Optional[str] = None,
         platform_id: str = 'prod',
+        ssl_verify: bool = True,
     ) -> bool:
         """Push error
 
         Args:
             definition (str): like {"integration_id": 13, "selection": 2310}
             description (str): ZeroDivizionError
             is_auth (bool, optional): [description]. Defaults to False.
@@ -131,24 +139,25 @@
             "title": name,
             "description": description,
             "definition": definition,
             "traceback": trb if trb else description,
             "date_time": start_time,
             "is_auth": is_auth,
         }
-        _request(exception_url, data=data, headers=headers)
+        _request(exception_url, data=data, headers=headers, ssl_verify=ssl_verify)
         return True
 
     def log_exception(
         self,
         definition: dict,
         description: str,
         is_auth: bool = False,
         trb: Optional[str] = None,
         platform_id: str = 'prod',
+        ssl_verify: bool = True,
     ) -> bool:
         """Puth to errors enpoint
 
         Args:
             definition (str): event definition
             trb (Optional[str], optional): traceback. Defaults to None.
 
@@ -157,13 +166,20 @@
         """
         dt = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         self.push_event(
             definition=definition,
             start_time=dt,
             status=True,
             description=description,
+            ssl_verify=ssl_verify,
         )
         if self.debug:
             return False
         return self.push_exception(
-            definition, description, dt, is_auth, trb, platform_id
+            definition,
+            description,
+            dt,
+            is_auth,
+            trb,
+            platform_id,
+            ssl_verify=ssl_verify,
         )
```

### Comparing `smart-manage-app-client-0.1.0b0/manage_app_client/decorator.py` & `smart-manage-app-client-0.2.0b0/manage_app_client/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,38 +18,41 @@
     def __init__(
         self,
         function: Callable,
         keys: Optional[Union[list, str, None]] = None,
         list_value: Optional[str] = None,
         iter_key: Optional[str] = None,
         description: Optional[str] = None,
+        ssl_verify: bool = True,
         *args,
         **kwargs
     ):
         self.function = function
         self.keys = keys
         self.list_value = list_value
         self.iter_key = iter_key
         self.args = args
         self.kwargs = kwargs
         self.description = description
+        self.ssl_verify = ssl_verify
 
     def execution(self, definition: dict, timestamp: str, *args, **kwargs) -> Any:
         init_kwargs = {
             "system_id": os.environ.get("MANAGE_SYSTEM_ID", ""),
             "system_url": os.environ.get("MANAGE_SYSTEM_URL", ""),
             "token": os.environ.get("MANAGE_SYSTEM_TOKEN", ""),
             "debug": os.environ.get("MANAGE_SYSTEM_DEBUG", '0'),
         }
         client = ManageClient(**init_kwargs)
         client.push_event(
             definition=definition,
             start_time=timestamp,
             status=False,
             description=self.description,
+            ssl_verify=self.ssl_verify,
         )
         # print(pushed)
         try:
             args = _check_lambda_args(args)
             if args or kwargs:
                 func_result = self.function(*args, **kwargs)
             else:
@@ -62,14 +65,15 @@
                 definition=definition, description=str(exc_description), trb=t
             )
         client.push_event(
             definition=definition,
             start_time=timestamp,
             status=True,
             description=self.description,
+            ssl_verify=self.ssl_verify,
         )
         return func_result
 
     def push(self, list_: bool = False, *args, **kwargs):
         definition = {}
         var_names = self.function.__code__.co_varnames
         try:
@@ -94,39 +98,48 @@
         except IndexError:
             pass
         timestamp = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         return self.execution(definition, timestamp, *args, **kwargs)
 
 
 def event(
-    keys: Optional[Union[list, str, None]] = None, description: Optional[str] = None
+    keys: Optional[Union[list, str, None]] = None,
+    description: Optional[str] = None,
+    ssl_verify: bool = True,
 ):
     def decorator(function: Callable, *args, **kwargs):
         def push_function_results(*args, **kwargs):
-            executor = __Executor(function=function, keys=keys, description=description)
+            executor = __Executor(
+                function=function,
+                keys=keys,
+                description=description,
+                ssl_verify=ssl_verify,
+            )
             return executor.push(False, *args, **kwargs)
 
         return push_function_results
 
     return decorator
 
 
 def list_value_event(
     keys: Union[str, list],
     list_value: str,
     iter_key: str,
     description: Optional[str] = None,
+    ssl_verify: bool = True,
 ) -> Any:
     def decorator(function, *args, **kwargs):
         def push_function_results(*args, **kwargs):
             executor = __Executor(
                 function=function,
                 keys=keys,
                 list_value=list_value,
                 iter_key=iter_key,
                 description=description,
+                ssl_verify=ssl_verify,
             )
             return executor.push(True, *args, **kwargs)
 
         return push_function_results
 
     return decorator
```

### Comparing `smart-manage-app-client-0.1.0b0/manage_app_client/settings.py` & `smart-manage-app-client-0.2.0b0/manage_app_client/settings.py`

 * *Files identical despite different names*

### Comparing `smart-manage-app-client-0.1.0b0/manage_app_client/tools.py` & `smart-manage-app-client-0.2.0b0/manage_app_client/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def log_exception(
     definition: dict,
     description: str,
     trb: Optional[str] = None,
     function_name: str = '',
     is_auth: bool = False,
     platform_id: str = 'prod',
+    ssl_verify: bool = True,
 ) -> bool:
     """Log error helper
 
     Args:
         definition (dict): dict definiton
         description (str): exception str
         trb (Optional[str], optional): full traceback. Defaults to None.
@@ -32,15 +33,20 @@
     }
     client = ManageClient(**init_kwargs)
     if not trb:
         trb = str(traceback.format_exc()).replace(
             'func_result = function', function_name
         )
     return client.log_exception(
-        definition, description, trb=trb, is_auth=is_auth, platform_id=platform_id
+        definition,
+        description,
+        trb=trb,
+        is_auth=is_auth,
+        platform_id=platform_id,
+        ssl_verify=ssl_verify,
     )
 
 
 def run(function: Callable[..., Any], **kwargs) -> Any:
     """
     function must be a top level function, not class method, and not decorated function
     """
```

### Comparing `smart-manage-app-client-0.1.0b0/manage_app_client/utils.py` & `smart-manage-app-client-0.2.0b0/manage_app_client/utils.py`

 * *Files identical despite different names*

