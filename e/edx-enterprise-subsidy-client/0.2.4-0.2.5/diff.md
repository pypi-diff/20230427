# Comparing `tmp/edx-enterprise-subsidy-client-0.2.4.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.2.4.tar", last modified: Wed Mar 29 19:41:50 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.2.5.tar", last modified: Thu Apr 27 13:45:29 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.2.4.tar` & `edx-enterprise-subsidy-client-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 19:41:50.180304 edx-enterprise-subsidy-client-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8139 2023-03-29 19:41:50.180304 edx-enterprise-subsidy-client-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 19:41:50.176304 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6740 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 19:41:50.180304 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8139 2023-03-29 19:41:50.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-03-29 19:41:50.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 19:41:50.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 19:41:50.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-03-29 19:41:50.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-29 19:41:50.000000 edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 19:41:50.180304 edx-enterprise-subsidy-client-0.2.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-03-29 19:41:50.180304 edx-enterprise-subsidy-client-0.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-03-29 19:41:44.000000 edx-enterprise-subsidy-client-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:45:29.177497 edx-enterprise-subsidy-client-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8273 2023-04-27 13:45:29.177497 edx-enterprise-subsidy-client-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:45:29.177497 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6784 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:45:29.177497 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8273 2023-04-27 13:45:29.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-27 13:45:29.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 13:45:29.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 13:45:29.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-27 13:45:29.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 13:45:29.000000 edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:45:29.177497 edx-enterprise-subsidy-client-0.2.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-27 13:45:29.181497 edx-enterprise-subsidy-client-0.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 13:45:29.177497 edx-enterprise-subsidy-client-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-27 13:45:23.000000 edx-enterprise-subsidy-client-0.2.5/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.2.4/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.2.5/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
-None.
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[0.2.5]
+*******
+* feat: redemption metadata.
 
 [0.2.4]
 *******
 * fix: don't directly access a status code on a failed response for logging.
 
 [0.2.3]
 *******
```

### Comparing `edx-enterprise-subsidy-client-0.2.4/LICENSE` & `edx-enterprise-subsidy-client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.4/LICENSE.txt` & `edx-enterprise-subsidy-client-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.4/PKG-INFO` & `edx-enterprise-subsidy-client-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -219,15 +219,21 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
-None.
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[0.2.5]
+*******
+* feat: redemption metadata.
 
 [0.2.4]
 *******
 * fix: don't directly access a status code on a failed response for logging.
 
 [0.2.3]
 *******
```

### Comparing `edx-enterprise-subsidy-client-0.2.4/README.rst` & `edx-enterprise-subsidy-client-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,23 +147,24 @@
         """
         response = self.client.get(
             self.TRANSACTIONS_ENDPOINT + f'{transaction_uuid}/'
         )
         response.raise_for_status()
         return response.json()
 
-    def create_subsidy_transaction(self, subsidy_uuid, lms_user_id, content_key, subsidy_access_policy_uuid):
+    def create_subsidy_transaction(self, subsidy_uuid, lms_user_id, content_key, subsidy_access_policy_uuid, metadata):
         """
         TODO: add docstring.
         """
         request_payload = {
             'subsidy_uuid': str(subsidy_uuid),
             'learner_id': lms_user_id,
             'content_key': content_key,
             'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
+            'metadata': metadata,
         }
         response = self.client.post(
             self.TRANSACTIONS_ENDPOINT,
             json=request_payload,
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -219,15 +219,21 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
-None.
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+[0.2.5]
+*******
+* feat: redemption metadata.
 
 [0.2.4]
 *******
 * fix: don't directly access a status code on a failed response for logging.
 
 [0.2.3]
 *******
```

### Comparing `edx-enterprise-subsidy-client-0.2.4/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.2.5/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 edx_enterprise_subsidy_client.egg-info/PKG-INFO
 edx_enterprise_subsidy_client.egg-info/SOURCES.txt
 edx_enterprise_subsidy_client.egg-info/dependency_links.txt
 edx_enterprise_subsidy_client.egg-info/not-zip-safe
 edx_enterprise_subsidy_client.egg-info/requires.txt
 edx_enterprise_subsidy_client.egg-info/top_level.txt
 requirements/base.in
-requirements/constraints.txt
+requirements/constraints.txt
+tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.2.4/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.2.5/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.4/setup.py` & `edx-enterprise-subsidy-client-0.2.5/setup.py`

 * *Files identical despite different names*

