# Comparing `tmp/st_common_data-0.2.6.1.tar.gz` & `tmp/st_common_data-0.2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common_data-0.2.6.1.tar", last modified: Tue Apr 18 06:55:35 2023, max compression
+gzip compressed data, was "st_common_data-0.2.6.2.tar", last modified: Thu Apr 27 07:13:33 2023, max compression
```

## Comparing `st_common_data-0.2.6.1.tar` & `st_common_data-0.2.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.6.1/LICENCE
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.6.1/README.md
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.6.1/pyproject.toml
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/setup.cfg
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-04-18 06:51:07.000000 st_common_data-0.2.6.1/st_common_data/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/auth/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.6.1/st_common_data/auth/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.6.1/st_common_data/auth/apps.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     9561 2023-04-18 06:48:02.000000 st_common_data-0.2.6.1/st_common_data/auth/django_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.6.1/st_common_data/auth/fastapi_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/auth/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/auth/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.6.1/st_common_data/auth/views.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    30488 2023-02-16 13:38:13.000000 st_common_data-0.2.6.1/st_common_data/datum.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.6.1/st_common_data/nyse_holidays.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/pagination.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/trading_accounts/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0001_initial.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/models.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.6.1/st_common_data/trading_accounts/views.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data/utils/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.6.1/st_common_data/utils/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.6.1/st_common_data/utils/common.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-18 06:55:35.862700 st_common_data-0.2.6.1/st_common_data.egg-info/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/SOURCES.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/dependency_links.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-04-18 06:55:35.000000 st_common_data-0.2.6.1/st_common_data.egg-info/top_level.txt
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.6.2/LICENCE
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.6.2/README.md
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.6.2/pyproject.toml
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/setup.cfg
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.685906 st_common_data-0.2.6.2/st_common_data/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-04-25 17:01:18.000000 st_common_data-0.2.6.2/st_common_data/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/st_common_data/auth/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.6.2/st_common_data/auth/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.6.2/st_common_data/auth/apps.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-25 17:38:18.000000 st_common_data-0.2.6.2/st_common_data/auth/django_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.6.2/st_common_data/auth/fastapi_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/auth/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/auth/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.6.2/st_common_data/auth/views.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    30488 2023-02-16 13:38:13.000000 st_common_data-0.2.6.2/st_common_data/datum.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.6.2/st_common_data/nyse_holidays.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/pagination.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/st_common_data/trading_accounts/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/0001_initial.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/models.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.6.2/st_common_data/trading_accounts/views.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.689906 st_common_data-0.2.6.2/st_common_data/utils/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.6.2/st_common_data/utils/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.6.2/st_common_data/utils/common.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-27 07:13:33.685906 st_common_data-0.2.6.2/st_common_data.egg-info/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-27 07:13:33.000000 st_common_data-0.2.6.2/st_common_data.egg-info/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-04-27 07:13:33.000000 st_common_data-0.2.6.2/st_common_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-04-27 07:13:33.000000 st_common_data-0.2.6.2/st_common_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-04-27 07:13:33.000000 st_common_data-0.2.6.2/st_common_data.egg-info/top_level.txt
```

### Comparing `st_common_data-0.2.6.1/LICENCE` & `st_common_data-0.2.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/PKG-INFO` & `st_common_data-0.2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.6.1
+Version: 0.2.6.2
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.6.1/README.md` & `st_common_data-0.2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/setup.cfg` & `st_common_data-0.2.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/auth/django_auth.py` & `st_common_data-0.2.6.2/st_common_data/auth/django_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
 class Auth0Authentication(authentication.BaseAuthentication):
     """
     An authentication plugin that authenticates requests through a JSON web
     token provided in a request header.
     """
     www_authenticate_realm = 'api'
+    auth0_api_audience = settings.AUTH0_API_AUDIENCE
 
     def authenticate(self, request):
         header = self.get_header(request)
         if header is None:
             return None
 
         raw_token = self.get_raw_token(header)
@@ -99,22 +100,21 @@
 
         rsa_key = jwks.get_rsa_key(unverified_header["kid"])
         try:
             claims = jwt.decode(
                 raw_token,
                 rsa_key,
                 algorithms=["RS256"],
-                audience=settings.AUTH0_API_AUDIENCE,
+                audience=self.auth0_api_audience,
                 issuer=f'https://{settings.AUTH0_DOMAIN}/')
         except jwt.ExpiredSignatureError:
             raise AuthenticationFailed(
                 detail='Token is expired')
         except jwt.JWTClaimsError:
-            raise AuthenticationFailed(
-                detail='Incorrect claims, please check the audience and issuer')
+            return None  # try another authentication instance
         except Exception:
             raise AuthenticationFailed(
                 detail='Unable to parse authentication header')
 
         user = self.get_user(claims)
         if not user:
             return None
@@ -181,14 +181,29 @@
     def get_user(self, claims):
         if 'azp' in claims and claims['azp'] == settings.AUTH0_SERVICE_CLIENT_ID:
             return ServiceUser()
         else:
             return None
 
 
+class Auth0CAPServiceAuthentication(Auth0ServiceAuthentication):
+    """
+    An authentication plugin for service auth (for CAP api).
+    """
+    auth0_api_audience = settings.AUTH0_CAP_API_AUDIENCE
+
+
+class Auth0CAPAuthentication(Auth0Authentication):
+    """
+    An authentication plugin that authenticates requests through a JSON web
+    token provided in a request header (for CAP api).
+    """
+    auth0_api_audience = settings.AUTH0_CAP_API_AUDIENCE
+
+
 class ServiceAuth0Token(metaclass=SingletonMeta):
     """
     Auth0 token from service app for machine-to-machine communication (between services)
     """
     TOKEN_FILENAME = SERVICE_TOKEN_FILENAME
 
     def __init__(self,
```

### Comparing `st_common_data-0.2.6.1/st_common_data/auth/fastapi_auth.py` & `st_common_data-0.2.6.2/st_common_data/auth/fastapi_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/auth/views.py` & `st_common_data-0.2.6.2/st_common_data/auth/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/datum.py` & `st_common_data-0.2.6.2/st_common_data/datum.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/nyse_holidays.py` & `st_common_data-0.2.6.2/st_common_data/nyse_holidays.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0001_initial.py` & `st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py` & `st_common_data-0.2.6.2/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/trading_accounts/models.py` & `st_common_data-0.2.6.2/st_common_data/trading_accounts/models.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/trading_accounts/views.py` & `st_common_data-0.2.6.2/st_common_data/trading_accounts/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data/utils/common.py` & `st_common_data-0.2.6.2/st_common_data/utils/common.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.6.1/st_common_data.egg-info/PKG-INFO` & `st_common_data-0.2.6.2/st_common_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-common-data
-Version: 0.2.6.1
+Version: 0.2.6.2
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.6.1/st_common_data.egg-info/SOURCES.txt` & `st_common_data-0.2.6.2/st_common_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

