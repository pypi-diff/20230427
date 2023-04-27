# Comparing `tmp/Avalara-23.3.1.tar.gz` & `tmp/Avalara-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Avalara-23.3.1.tar", last modified: Wed Mar 29 23:14:28 2023, max compression
+gzip compressed data, was "Avalara-23.4.1.tar", last modified: Thu Apr 27 21:54:20 2023, max compression
```

## Comparing `Avalara-23.3.1.tar` & `Avalara-23.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:14:28.440049 Avalara-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-29 23:14:26.000000 Avalara-23.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-03-29 23:14:28.440049 Avalara-23.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-03-29 23:14:26.000000 Avalara-23.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 23:14:28.440049 Avalara-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-29 23:14:26.000000 Avalara-23.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:14:28.436048 Avalara-23.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:14:28.436048 Avalara-23.3.1/src/Avalara.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-03-29 23:14:28.000000 Avalara-23.3.1/src/Avalara.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-29 23:14:28.000000 Avalara-23.3.1/src/Avalara.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 23:14:28.000000 Avalara-23.3.1/src/Avalara.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-29 23:14:28.000000 Avalara-23.3.1/src/Avalara.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-29 23:14:28.000000 Avalara-23.3.1/src/Avalara.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:14:28.440049 Avalara-23.3.1/src/avalara/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/_str_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/ava_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   722779 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/client_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/transaction_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-03-29 23:14:26.000000 Avalara-23.3.1/src/avalara/transaction_builder_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:54:20.823486 Avalara-23.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 21:54:15.000000 Avalara-23.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-04-27 21:54:20.823486 Avalara-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-27 21:54:15.000000 Avalara-23.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:54:20.823486 Avalara-23.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-27 21:54:15.000000 Avalara-23.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:54:20.819486 Avalara-23.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:54:20.819486 Avalara-23.4.1/src/Avalara.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-04-27 21:54:20.000000 Avalara-23.4.1/src/Avalara.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 21:54:20.000000 Avalara-23.4.1/src/Avalara.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:54:20.000000 Avalara-23.4.1/src/Avalara.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 21:54:20.000000 Avalara-23.4.1/src/Avalara.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 21:54:20.000000 Avalara-23.4.1/src/Avalara.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:54:20.823486 Avalara-23.4.1/src/avalara/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/_str_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/ava_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   723675 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/client_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/transaction_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-27 21:54:15.000000 Avalara-23.4.1/src/avalara/transaction_builder_methods.py
```

### Comparing `Avalara-23.3.1/LICENSE.txt` & `Avalara-23.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Avalara-23.3.1/PKG-INFO` & `Avalara-23.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Avalara
-Version: 23.3.1
+Version: 23.4.1
 Summary: Avalara Tax Python SDK.
 Home-page: https://github.com/avadev/AvaTax-REST-V2-Python-SDK
 Author: Han Bao, Adrienne Karnoski, Robert Bronson, Philip Werner, Genevieve Conty
 Author-email: han.bao@avalara.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `Avalara-23.3.1/README.md` & `Avalara-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Avalara-23.3.1/setup.py` & `Avalara-23.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pkg_description = ''
 with open('README.md') as f:
     pkg_description = f.read()
 
 
 setup(
     name='Avalara',
-    version='23.3.1',
+    version='23.4.1',
     url='https://github.com/avadev/AvaTax-REST-V2-Python-SDK',
     package_dir={'': 'src'},
     packages=['avalara'],
     author='Han Bao, Adrienne Karnoski, Robert Bronson, Philip Werner, Genevieve Conty',
     author_email='han.bao@avalara.com',
     description='Avalara Tax Python SDK.',
     long_description=pkg_description,
```

### Comparing `Avalara-23.3.1/src/Avalara.egg-info/PKG-INFO` & `Avalara-23.4.1/src/Avalara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Avalara
-Version: 23.3.1
+Version: 23.4.1
 Summary: Avalara Tax Python SDK.
 Home-page: https://github.com/avadev/AvaTax-REST-V2-Python-SDK
 Author: Han Bao, Adrienne Karnoski, Robert Bronson, Philip Werner, Genevieve Conty
 Author-email: han.bao@avalara.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `Avalara-23.3.1/src/avalara/_str_version.py` & `Avalara-23.4.1/src/avalara/_str_version.py`

 * *Files identical despite different names*

### Comparing `Avalara-23.3.1/src/avalara/ava_logger.py` & `Avalara-23.4.1/src/avalara/ava_logger.py`

 * *Files identical despite different names*

### Comparing `Avalara-23.3.1/src/avalara/client.py` & `Avalara-23.4.1/src/avalara/client.py`

 * *Files identical despite different names*

### Comparing `Avalara-23.3.1/src/avalara/client_methods.py` & `Avalara-23.4.1/src/avalara/client_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     
       :param id_ [int] The ID of the account you wish to update.
       :param model [ResetLicenseKeyModel] A request confirming that you wish to reset the license key of this account.
       :return LicenseKeyModel
     """
     def account_reset_license_key(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/resetlicensekey'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Activate an account by accepting terms and conditions
@@ -52,15 +52,15 @@
     
       :param id_ [int] The ID of the account to activate
       :param model [ActivateAccountModel] The activation request
       :return AccountModel
     """
     def activate_account(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/activate'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve audit history for an account.
@@ -72,26 +72,26 @@
       You can learn more about valid time zone designators at https://en.wikipedia.org/wiki/ISO_8601#Time_zone_designators.
       This API enforces limits to the amount of data retrieved. These limits are subject to change.
       * You may request data from a maximum of a one-hour time period.
       * The amount of data and number of API calls returned by this API are limited and may be adjusted at any time.
       * Old records may be migrated out of immediately available storage. To request older data, please contact your account manager.
       * New records must migrate to available storage before they can be retrieved. You may need to wait a period of time before newly created records can be fetched.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the account you wish to audit.
       :param start [datetime] The start datetime of audit history you with to retrieve, e.g. "2018-06-08T17:00:00Z". Defaults to the past 15 minutes.
       :param end [datetime] The end datetime of audit history you with to retrieve, e.g. "2018-06-08T17:15:00Z. Defaults to the current time. Maximum of an hour after the start time.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :return FetchResult
     """
     def audit_account(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/audit'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create license key for this account
@@ -108,15 +108,15 @@
     
       :param id_ [int] The ID of the account you wish to update.
       :param model [AccountLicenseKeyModel] 
       :return LicenseKeyModel
     """
     def create_license_key(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/licensekey'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete license key for this account by license key name
@@ -129,37 +129,37 @@
     
       :param id_ [int] The ID of the account you wish to update.
       :param licensekeyname [string] The license key name you wish to update.
       :return ErrorDetail
     """
     def delete_license_key(self, id_, licensekeyname):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/accounts/{}/licensekey/{}'.format(self.base_url, id_, licensekeyname),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single account
     
     Get the account object identified by this URL.
       You may use the '$include' parameter to fetch additional nested data:
       * Subscriptions
       * Users
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the account to retrieve
       :param include [string] A comma separated list of special fetch options
       :return AccountModel
     """
     def get_account(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get configuration settings for this account
@@ -170,58 +170,58 @@
       Avalara internal software configuration values; to store your own account-level settings, please
       create a new category name that begins with `X-`, for example, `X-MyCustomCategory`.
       Account settings are permanent settings that cannot be deleted. You can set the value of an
       account setting to null if desired.
       Avalara-based account settings for `TaxServiceConfig` and `AddressServiceConfig` affect your account's
       tax calculation and address resolution, and should only be changed with care.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param id_ [int] 
       :return AccountConfigurationModel
     """
     def get_account_configuration(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/configuration'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve license key by license key name
     
     ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the account to retrieve
       :param licensekeyname [string] The ID of the account to retrieve
       :return AccountLicenseKeyModel
     """
     def get_license_key(self, id_, licensekeyname):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/licensekey/{}'.format(self.base_url, id_, licensekeyname),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all license keys for this account
     
     Gets list of all the license keys used by the account.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the account to retrieve
       :return AccountLicenseKeyModel
     """
     def get_license_keys(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/licensekeys'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all accounts
@@ -231,26 +231,26 @@
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * Subscriptions
       * Users
       For more information about filtering in REST, please see the documentation at http://developer.avalara.com/avatax/filtering-in-rest/ .
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param include [string] A comma separated list of objects to fetch underneath this account. Any object with a URL path underneath this account can be fetched by specifying its name.
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* subscriptions, users
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_accounts(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Change configuration settings for this account
@@ -269,15 +269,15 @@
     
       :param id_ [int] 
       :param model [AccountConfigurationModel] 
       :return AccountConfigurationModel
     """
     def set_account_configuration(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/configuration'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve geolocation information for a specified address
@@ -304,15 +304,15 @@
       :param postalCode [string] Postal Code / Zip Code
       :param country [string] Two character ISO 3166 Country Code (see /api/v2/definitions/countries for a full list)
       :param textCase [TextCase] selectable text case for address validation (See TextCase::* for a list of allowable values)
       :return AddressResolutionModel
     """
     def resolve_address(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/addresses/resolve'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve geolocation information for a specified address
@@ -328,15 +328,15 @@
       * This API depends on the following active services:*Required* (all): AutoAddress.
     
       :param model [AddressValidationInfo] The address to resolve
       :return AddressResolutionModel
     """
     def resolve_address_post(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/addresses/resolve'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a lookup file for a company
@@ -346,15 +346,15 @@
       :param accountId [int] The ID of the account for the company
       :param companyId [int] The ID of the company for which the lookup file is to be created
       :param model [AdvancedRuleLookupFileModel] The lookup file you wish to create
       :return AdvancedRuleLookupFileModel
     """
     def create_company_lookup_file(self, accountId, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/advancedrules/accounts/{}/companies/{}/lookupFiles'.format(self.base_url, accountId, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a lookup file
@@ -363,15 +363,15 @@
     
       :param accountId [int] The ID of the account for the company the lookup file is for
       :param id_ [string] The unique ID/GUID for the company lookup file to be deleted
       :return ErrorDetail
     """
     def delete_lookup_file(self, accountId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/advancedrules/accounts/{}/lookupFiles/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get the lookup files for a company
@@ -380,15 +380,15 @@
     
       :param accountId [int] The account ID for the company
       :param companyId [int] The ID of the company for which to retrieve lookup files
       :return FetchResult
     """
     def get_company_lookup_files(self, accountId, companyId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/advancedrules/accounts/{}/companies/{}/lookupFiles'.format(self.base_url, accountId, companyId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get a lookup file for an accountId and companyLookupFileId
@@ -397,15 +397,15 @@
     
       :param accountId [int] The ID of the account for the lookup file
       :param id_ [string] The unique ID/GUID of the company lookup file to return
       :return AdvancedRuleLookupFileModel
     """
     def get_lookup_file(self, accountId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/advancedrules/accounts/{}/lookupFiles/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a lookup file
@@ -415,15 +415,15 @@
       :param accountId [int] The ID of the account for the company the lookup file is for
       :param id_ [string] The unique ID/GUID of the company lookup file to be updated
       :param model [AdvancedRuleLookupFileModel] The new values to update the lookup file
       :return AdvancedRuleLookupFileModel
     """
     def update_lookup_file(self, accountId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/advancedrules/accounts/{}/lookupFiles/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new AvaFileForm
@@ -435,15 +435,15 @@
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param model [AvaFileFormModel] The AvaFileForm you wish to create.
       :return AvaFileFormModel
     """
     def create_ava_file_forms(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/avafileforms'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single AvaFileForm
@@ -454,15 +454,15 @@
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param id_ [int] The ID of the AvaFileForm you wish to delete.
       :return ErrorDetail
     """
     def delete_ava_file_form(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/avafileforms/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single AvaFileForm
@@ -473,15 +473,15 @@
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param id_ [int] The primary key of this AvaFileForm
       :return AvaFileFormModel
     """
     def get_ava_file_form(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/avafileforms/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all AvaFileForms
@@ -496,15 +496,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_ava_file_forms(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/avafileforms'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a AvaFileForm
@@ -517,15 +517,15 @@
     
       :param id_ [int] The ID of the AvaFileForm you wish to update
       :param model [AvaFileFormModel] The AvaFileForm model you wish to update.
       :return AvaFileFormModel
     """
     def update_ava_file_form(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/avafileforms/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Cancel an in progress batch
@@ -544,15 +544,15 @@
     
       :param companyId [int] The ID of the company that owns this batch.
       :param id_ [int] The ID of the batch to cancel.
       :return BatchModel
     """
     def cancel_batch(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/batches/{}/cancel'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new batch
@@ -577,15 +577,15 @@
     
       :param companyId [int] The ID of the company that owns this batch.
       :param model [BatchModel] The batch you wish to create.
       :return BatchModel
     """
     def create_batches(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/batches'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new transaction batch
@@ -609,15 +609,15 @@
     
       :param companyId [int] The ID of the company that owns this batch.
       :param model [CreateTransactionBatchRequestModel] The transaction batch you wish to create.
       :return CreateTransactionBatchResponseModel
     """
     def create_transaction_batch(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/batches/transactions'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single batch
@@ -635,15 +635,15 @@
     
       :param companyId [int] The ID of the company that owns this batch.
       :param id_ [int] The ID of the batch to delete.
       :return ErrorDetail
     """
     def delete_batch(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/batches/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Download a single batch file
@@ -655,15 +655,15 @@
       :param companyId [int] The ID of the company that owns this batch
       :param batchId [int] The ID of the batch object
       :param id_ [int] The primary key of this batch file object
       :return String
     """
     def download_batch(self, companyId, batchId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/batches/{}/files/{}/attachment'.format(self.base_url, companyId, batchId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single batch
@@ -685,15 +685,15 @@
     
       :param companyId [int] The ID of the company that owns this batch
       :param id_ [int] The primary key of this batch
       :return BatchModel
     """
     def get_batch(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/batches/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all batches for this company
@@ -723,15 +723,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_batches_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/batches'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all batches
@@ -758,15 +758,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_batches(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/batches'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a CertExpress invitation
@@ -790,15 +790,15 @@
       :param companyId [int] The unique ID number of the company that will record certificates
       :param customerCode [string] The number of the customer where the request is sent to
       :param model [CreateCertExpressInvitationModel] the requests to send out to customers
       :return CertExpressInvitationStatusModel
     """
     def create_cert_express_invitation(self, companyId, customerCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/customers/{}/certexpressinvites'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single CertExpress invitation
@@ -823,15 +823,15 @@
       :param customerCode [string] The number of the customer where the request is sent to
       :param id_ [int] The unique ID number of this CertExpress invitation
       :param include [string] OPTIONAL: A comma separated list of special fetch options. No options are defined at this time.
       :return CertExpressInvitationModel
     """
     def get_cert_express_invitation(self, companyId, customerCode, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/customers/{}/certexpressinvites/{}'.format(self.base_url, companyId, customerCode, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List CertExpress invitations
@@ -858,15 +858,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_cert_express_invitations(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certexpressinvites'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create certificates for this company
@@ -894,15 +894,15 @@
       :param companyId [int] The ID number of the company recording this certificate
       :param preValidatedExemptionReason [boolean] If set to true, the certificate will bypass the human verification process.
       :param model [CertificateModel] Certificates to be created
       :return CertificateModel
     """
     def create_certificates(self, companyId, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Revoke and delete a certificate
@@ -923,15 +923,15 @@
     
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :return ErrorDetail
     """
     def delete_certificate(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/certificates/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Download an image for this certificate
@@ -955,15 +955,15 @@
       :param id_ [int] The unique ID number of this certificate
       :param page [int] If you choose `$type`=`Jpeg`, you must specify which page number to retrieve.
       :param type [CertificatePreviewType] The data format in which to retrieve the certificate image (See CertificatePreviewType::* for a list of allowable values)
       :return String
     """
     def download_certificate_image(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certificates/{}/attachment'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single certificate
@@ -988,15 +988,15 @@
       :param companyId [int] The ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param include [string] OPTIONAL: A comma separated list of special fetch options. You can specify one or more of the following:      * customers - Retrieves the list of customers linked to the certificate.   * po_numbers - Retrieves all PO numbers tied to the certificate.   * attributes - Retrieves all attributes applied to the certificate.
       :return CertificateModel
     """
     def get_certificate(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certificates/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Check a company's exemption certificate status.
@@ -1012,15 +1012,15 @@
       * This API depends on the following active services:*Required* (all): AvaTaxPro.
     
       :param companyId [int] The company ID to check
       :return ProvisionStatusModel
     """
     def get_certificate_setup(self, companyId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certificates/setup'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Link attributes to a certificate
@@ -1043,15 +1043,15 @@
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param model [CertificateAttributeModel] The list of attributes to link to this certificate.
       :return FetchResult
     """
     def link_attributes_to_certificate(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates/{}/attributes/link'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Link customers to a certificate
@@ -1075,15 +1075,15 @@
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param model [LinkCustomersModel] The list of customers needed be added to the Certificate for exemption
       :return FetchResult
     """
     def link_customers_to_certificate(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates/{}/customers/link'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all attributes applied to this certificate
@@ -1105,15 +1105,15 @@
     
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :return FetchResult
     """
     def list_attributes_for_certificate(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certificates/{}/attributes'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List customers linked to this certificate
@@ -1136,15 +1136,15 @@
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param include [string] OPTIONAL: A comma separated list of special fetch options.   No options are currently available when fetching customers.
       :return FetchResult
     """
     def list_customers_for_certificate(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certificates/{}/customers'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all certificates for a company
@@ -1172,15 +1172,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_certificates(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certificates'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Request setup of exemption certificates for this company.
@@ -1197,15 +1197,15 @@
       * This API depends on the following active services:*Required* (all): AvaTaxPro.
     
       :param companyId [int] 
       :return ProvisionStatusModel
     """
     def request_certificate_setup(self, companyId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates/setup'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Unlink attributes from a certificate
@@ -1228,15 +1228,15 @@
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param model [CertificateAttributeModel] The list of attributes to unlink from this certificate.
       :return FetchResult
     """
     def unlink_attributes_from_certificate(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates/{}/attributes/unlink'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Unlink customers from a certificate
@@ -1261,15 +1261,15 @@
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param model [LinkCustomersModel] The list of customers to unlink from this certificate
       :return FetchResult
     """
     def unlink_customers_from_certificate(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates/{}/customers/unlink'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single certificate
@@ -1290,15 +1290,15 @@
       :param companyId [int] The ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param model [CertificateModel] The new certificate object that will replace the existing one
       :return CertificateModel
     """
     def update_certificate(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/certificates/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Upload an image or PDF attachment for this certificate
@@ -1321,15 +1321,15 @@
       :param companyId [int] The unique ID number of the company that recorded this certificate
       :param id_ [int] The unique ID number of this certificate
       :param file [String] The exemption certificate file you wanted to upload. Accepted formats are: PDF, JPEG, TIFF, PNG.
       :return string
     """
     def upload_certificate_image(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/certificates/{}/attachment'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Checks whether the integration being used to set up this company and run transactions onto this company is compliant to all requirements.
@@ -1353,22 +1353,22 @@
       12. All documents have same ItemCodes, descriptions and taxCodes.
       13. Less than 2 addresses used across all documents.
       14. Whether locationCode was used in documents.
       15. Account with AvaGlobal subscription and no documents have VATBuyerId.
       16. Any document has currencyCode not being USD for accounts with AvaGlobal subscription.
       17. All documents have countryCode used for accounts with AvaGlobal subscription.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the company to check if its integration is certified.
       :return string
     """
     def certify_integration(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/certify'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Change the filing status of this company
@@ -1379,23 +1379,23 @@
       requested filing calendars prior to beginning filing tax returns on behalf of this company.
       The following changes may be requested through this API:
       * If a company is in `NotYetFiling` status, the customer may request this be changed to `FilingRequested`.
       * Avalara compliance team members may change a company from `FilingRequested` to `FirstFiling`.
       * Avalara compliance team members may change a company from `FirstFiling` to `Active`.
       All other status changes must be requested through the Avalara customer support team.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] 
       :param model [FilingStatusChangeModel] 
       :return string
     """
     def change_filing_status(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/filingstatus'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Quick setup for a company with a single physical address
@@ -1414,15 +1414,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, CompanyAdmin, CSPTester, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param model [CompanyInitializationModel] Information about the company you wish to create.
       :return CompanyModel
     """
     def company_initialize(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/initialize'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create new companies
@@ -1435,15 +1435,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, CompanyAdmin, CSPTester, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param model [CompanyModel] Either a single company object or an array of companies to create
       :return CompanyModel
     """
     def create_companies(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Add parameters to a company.
@@ -1459,15 +1459,15 @@
     
       :param companyId [int] The ID of the company that owns this company parameter.
       :param model [CompanyParameterDetailModel] The company parameters you wish to create.
       :return CompanyParameterDetailModel
     """
     def create_company_parameters(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/parameters'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Request managed returns funding setup for a company
@@ -1480,25 +1480,25 @@
       be sent either via email or via an embedded HTML widget.
       When the funding configuration is submitted to Avalara, it will be reviewed by treasury team members
       before approval.
       This API records that an ambedded HTML funding setup widget was activated.
       This API requires a subscription to Avalara Managed Returns or SST Certified Service Provider.
       ### Security Policies
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The unique identifier of the company
       :param businessUnit [POABusinessUnit] The company's business unit (See POABusinessUnit::* for a list of allowable values)
       :param subscriptionType [POASubscriptionType] The company's subscription type (See POASubscriptionType::* for a list of allowable values)
       :param model [FundingInitiateModel] The funding initialization request
       :return FundingStatusModel
     """
     def create_funding_request(self, id_, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/funding/setup'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single company
@@ -1508,15 +1508,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, CompanyAdmin, CSPTester, FirmAdmin, SSTAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] The ID of the company you wish to delete.
       :return ErrorDetail
     """
     def delete_company(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single company parameter
@@ -1530,60 +1530,60 @@
     
       :param companyId [int] The company id
       :param id_ [int] The parameter id
       :return ErrorDetail
     """
     def delete_company_parameter(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/parameters/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Check the funding configuration of a company
     
     This API is available by invitation only.
       Requires a subscription to Avalara Managed Returns or SST Certified Service Provider.
       Returns the funding configuration of the requested company.
       .
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param companyId [int] The unique identifier of the company
       :return FundingConfigurationModel
     """
     def funding_configuration_by_company(self, companyId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/funding/configuration'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Check the funding configuration of a company
     
     This API is available by invitation only.
       Requires a subscription to Avalara Managed Returns or SST Certified Service Provider.
       Returns the funding configuration of the requested company.
       .
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param companyId [int] The unique identifier of the company
       :param currency [string] The currency of the funding. USD and CAD are the only valid currencies
       :return FundingConfigurationModel
     """
     def funding_configurations_by_company_and_currency(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/funding/configurations'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single company
@@ -1597,23 +1597,23 @@
        * Nexus
        * Settings
        * TaxCodes
        * TaxRules
        * UPC
        * Parameters
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the company to retrieve.
       :param include [string] OPTIONAL: A comma separated list of special fetch options.      * Child objects - Specify one or more of the following to retrieve objects related to each company: "Contacts", "FilingCalendars", "Items", "Locations", "Nexus", "TaxCodes", "NonReportingChildren" or "TaxRules".   * Deleted objects - Specify "FetchDeleted" to retrieve information about previously deleted objects.
       :return CompanyModel
     """
     def get_company(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get configuration settings for this company
@@ -1624,44 +1624,44 @@
       Avalara internal software configuration values; to store your own company-level settings, please
       create a new category name that begins with `X-`, for example, `X-MyCustomCategory`.
       Company settings are permanent settings that cannot be deleted. You can set the value of a
       company setting to null if desired and if the particular setting supports it.
       Avalara-based company settings for `AvaCertServiceConfig` affect your company's exemption certificate
       processing, and should be changed with care.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param id_ [int] 
       :return CompanyConfigurationModel
     """
     def get_company_configuration(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/configuration'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single company parameter
     
     Retrieves a single parameter of a company.
       Some companies can be taxed and reported differently depending on the properties of the company, such as IsPrimaryAddress. In AvaTax, these tax-affecting properties are called "parameters".
       A parameter added to a company will be used by default in tax calculation but will not show on the transaction line referencing the company.
       A company location parameter specified on a transaction line will override a company parameter if they share the same parameter name.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] 
       :param id_ [int] 
       :return CompanyParameterDetailModel
     """
     def get_company_parameter_detail(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/parameters/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get this company's filing status
@@ -1674,46 +1674,46 @@
       * `NoReporting` - This company is not configured to report tax returns; instead, it reports through a parent company.
       * `NotYetFiling` - This company has not yet begun filing tax returns through Avalara's Managed Returns Service.
       * `FilingRequested` - The company has requested to begin filing tax returns, but Avalara's compliance team has not yet begun filing.
       * `FirstFiling` - The company has recently filing tax returns and is in a new status.
       * `Active` - The company is currently active and is filing tax returns via Avalara Managed Returns.
       * `Inactive` - The company is currently inactive.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] 
       :return string
     """
     def get_filing_status(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/filingstatus'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get ACH entry detail report for company and period
     
     This API is available by invitation only.
       Requires a subscription to Avalara Managed Returns or SST Certified Service Provider.
       Returns a list of ACH entry details for the given company and period.
       Each object in the result is an ach entry trace record for a payment made on behalf of this company.
       ### Security Policies
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The unique identifier of the company
       :param periodyear [int] The period year
       :param periodmonth [int] The period month
       :return ACHEntryDetailModel
     """
     def list_a_c_h_entry_details_for_company(self, id_, periodyear, periodmonth):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/paymentdetails/{}/{}'.format(self.base_url, id_, periodyear, periodmonth),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve parameters for a company
@@ -1721,66 +1721,66 @@
     Retrieve all parameters of a company.
       Some companies can be taxed and reported differently depending on the properties of the company, such as IsPrimaryAddress. In AvaTax, these tax-affecting properties are called "parameters".
       A parameter added to a company will be used by default in tax calculation but will not show on the transaction line referencing the company.
       A company location parameter specified on a transaction line will override a company parameter if they share the same parameter name.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The company id
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* name, unit
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_company_parameter_details(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/parameters'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Check managed returns funding status for a company
     
     This API is available by invitation only.
       Requires a subscription to Avalara Managed Returns or SST Certified Service Provider.
       Returns a list of funding setup requests and their current status.
       Each object in the result is a request that was made to setup or adjust funding status for this company.
       ### Security Policies
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The unique identifier of the company
       :return FundingStatusModel
     """
     def list_funding_requests_by_company(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/funding'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a list of MRS Companies with account
     
     This API is available by invitation only.
       Get a list of companies with an active MRS service.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :return FetchResult
     """
     def list_mrs_companies(self):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/mrs'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all companies
@@ -1796,26 +1796,26 @@
       * Nexus
       * Settings
       * TaxCodes
       * TaxRules
       * UPC
       * Parameters
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param include [string] A comma separated list of objects to fetch underneath this company. Any object with a URL path underneath this company can be fetched by specifying its name.
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* IsFein, contacts, items, locations, nexus, settings, taxCodes, taxRules, upcs, nonReportingChildCompanies, exemptCerts, parameters, supplierandcustomers
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_companies(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Change configuration settings for this company
@@ -1834,15 +1834,15 @@
     
       :param id_ [int] 
       :param model [CompanyConfigurationModel] 
       :return CompanyConfigurationModel
     """
     def set_company_configuration(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/configuration'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single company
@@ -1859,15 +1859,15 @@
     
       :param id_ [int] The ID of the company you wish to update.
       :param model [CompanyModel] The company object you wish to update.
       :return CompanyModel
     """
     def update_company(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a company parameter
@@ -1882,61 +1882,36 @@
       :param companyId [int] The company id.
       :param id_ [int] The company parameter id
       :param model [CompanyParameterDetailModel] The company parameter object you wish to update.
       :return CompanyParameterDetailModel
     """
     def update_company_parameter_detail(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/parameters/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
-    Retrieve jurisdiction rate information for tax authority
-    
-    This API is available by invitation only.
-      ### Security Policies
-      * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
-    
-      :param taxAuthorityId [int] Used to limit the jurisdictions returned.
-      :param effectiveDate [datetime] Used to limit the jurisdictions returned.
-      :param endDate [datetime] Used to limit the jurisdictions returned.
-      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
-      :param include [string] A comma separated list of objects to fetch underneath this jurisdiction.
-      :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
-      :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
-      :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
-      :return ComplianceJurisdictionRateModel
-    """
-    def query_tax_authority_jurisdiction_rates(self, include=None):
-        if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
-        return requests.get('{}/api/v2/compliance/taxauthorityjurisdictionrates'.format(self.base_url),
-                               auth=self.auth, headers=self.client_header, params=include, 
-                               timeout=self.timeout_limit if self.timeout_limit else 1200)
-    r"""
-    Swagger Name: AvaTaxClient
-    
     Create a new contact
     
     Create one or more new contact objects.
       A 'contact' is a person associated with a company who is designated to handle certain responsibilities of
       a tax collecting and filing entity.
       ### Security Policies
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, CompanyAdmin, CSPTester, FirmAdmin, SSTAdmin, TechnicalSupportAdmin.
     
       :param companyId [int] The ID of the company that owns this contact.
       :param model [ContactModel] The contacts you wish to create.
       :return ContactModel
     """
     def create_contacts(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/contacts'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single contact
@@ -1947,15 +1922,15 @@
     
       :param companyId [int] The ID of the company that owns this contact.
       :param id_ [int] The ID of the contact you wish to delete.
       :return ErrorDetail
     """
     def delete_contact(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/contacts/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single contact
@@ -1968,15 +1943,15 @@
     
       :param companyId [int] The ID of the company for this contact
       :param id_ [int] The primary key of this contact
       :return ContactModel
     """
     def get_contact(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/contacts/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve contacts for this company
@@ -1992,15 +1967,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_contacts_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/contacts'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all contacts
@@ -2017,15 +1992,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_contacts(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/contacts'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single contact
@@ -2041,15 +2016,15 @@
       :param companyId [int] The ID of the company that this contact belongs to.
       :param id_ [int] The ID of the contact you wish to update
       :param model [ContactModel] The contact you wish to update.
       :return ContactModel
     """
     def update_contact(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/contacts/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create customers for this company
@@ -2072,15 +2047,15 @@
     
       :param companyId [int] The unique ID number of the company that recorded this customer
       :param model [CustomerModel] The list of customer objects to be created
       :return CustomerModel
     """
     def create_customers(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/customers'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a customer record
@@ -2101,15 +2076,15 @@
     
       :param companyId [int] The unique ID number of the company that recorded this customer
       :param customerCode [string] The unique code representing this customer
       :return CustomerModel
     """
     def delete_customer(self, companyId, customerCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/customers/{}'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single customer
@@ -2135,15 +2110,15 @@
       :param companyId [int] The unique ID number of the company that recorded this customer
       :param customerCode [string] The unique code representing this customer
       :param include [string] Specify optional additional objects to include in this fetch request
       :return CustomerModel
     """
     def get_customer(self, companyId, customerCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/customers/{}'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Link attributes to a customer
@@ -2167,15 +2142,15 @@
       :param companyId [int] The unique ID number of the company that recorded the provided customer
       :param customerCode [string] The unique code representing the current customer
       :param model [CustomerAttributeModel] The list of attributes to link to the customer.
       :return FetchResult
     """
     def link_attributes_to_customer(self, companyId, customerCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/customers/{}/attributes/link'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Link certificates to a customer
@@ -2197,15 +2172,15 @@
       :param companyId [int] The unique ID number of the company that recorded this customer
       :param customerCode [string] The unique code representing this customer
       :param model [LinkCertificatesModel] The list of certificates to link to this customer
       :return FetchResult
     """
     def link_certificates_to_customer(self, companyId, customerCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/customers/{}/certificates/link'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Link two customer records together
@@ -2227,15 +2202,15 @@
       :param companyId [int] The unique ID number of the company defining customers.
       :param code [string] The code of the bill-to customer to link.
       :param model [LinkCustomersModel] A list of information about ship-to customers to link to this bill-to customer.
       :return CustomerModel
     """
     def link_ship_to_customers_to_bill_customer(self, companyId, code, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/customers/billto/{}/shipto/link'.format(self.base_url, companyId, code),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a customer's attributes
@@ -2258,15 +2233,15 @@
     
       :param companyId [int] The unique ID number of the company that recorded the provided customer
       :param customerCode [string] The unique code representing the current customer
       :return FetchResult
     """
     def list_attributes_for_customer(self, companyId, customerCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/customers/{}/attributes'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List certificates linked to a customer
@@ -2292,15 +2267,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_certificates_for_customer(self, companyId, customerCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/customers/{}/certificates'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List valid certificates for a location
@@ -2325,15 +2300,15 @@
       :param customerCode [string] The unique code representing this customer
       :param country [string] Search for certificates matching this country. Uses the ISO 3166 two character country code.
       :param region [string] Search for certificates matching this region. Uses the ISO 3166 two or three character state, region, or province code.
       :return ExemptionStatusModel
     """
     def list_valid_certificates_for_customer(self, companyId, customerCode, country, region):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/customers/{}/certificates/{}/{}'.format(self.base_url, companyId, customerCode, country, region),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all customers for this company
@@ -2361,15 +2336,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_customers(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/customers'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Unlink attributes from a customer
@@ -2393,15 +2368,15 @@
       :param companyId [int] The unique ID number of the company that recorded the customer
       :param customerCode [string] The unique code representing the current customer
       :param model [CustomerAttributeModel] The list of attributes to unlink from the customer.
       :return FetchResult
     """
     def unlink_attributes_from_customer(self, companyId, customerCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/customers/{}/attributes/unlink'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Unlink certificates from a customer
@@ -2423,15 +2398,15 @@
       :param companyId [int] The unique ID number of the company that recorded this customer
       :param customerCode [string] The unique code representing this customer
       :param model [LinkCertificatesModel] The list of certificates to link to this customer
       :return FetchResult
     """
     def unlink_certificates_from_customer(self, companyId, customerCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/customers/{}/certificates/unlink'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single customer
@@ -2453,15 +2428,15 @@
       :param companyId [int] The unique ID number of the company that recorded this customer
       :param customerCode [string] The unique code representing this customer
       :param model [CustomerModel] The new customer model that will replace the existing record at this URL
       :return CustomerModel
     """
     def update_customer(self, companyId, customerCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/customers/{}'.format(self.base_url, companyId, customerCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create and store new datasources for the respective companies.
@@ -2473,15 +2448,15 @@
     
       :param companyId [int] The id of the company you which to create the datasources
       :param model [DataSourceModel] 
       :return DataSourceModel
     """
     def create_data_sources(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/datasources'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a datasource by datasource id for a company.
@@ -2493,82 +2468,82 @@
     
       :param companyId [int] The id of the company the datasource belongs to.
       :param id_ [int] The id of the datasource you wish to delete.
       :return ErrorDetail
     """
     def delete_data_source(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/datasources/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get data source by data source id
     
     Retrieve the data source by its unique ID number.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Required* (all): AvaTaxPro, BasicReturns.
     
       :param companyId [int] 
       :param id_ [int] data source id
       :return DataSourceModel
     """
     def get_data_source_by_id(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/datasources/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all datasources for this company
     
     Gets multiple datasource objects for a given company.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Required* (all): AvaTaxPro, BasicReturns.
     
       :param companyId [int] The id of the company you wish to retrieve the datasources.
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* isEnabled, isSynced, isAuthorized, name, externalState
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_data_sources(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/datasources'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all datasources
     
     Get multiple datasource objects across all companies.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Required* (all): AvaTaxPro, BasicReturns.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* isEnabled, isSynced, isAuthorized, name, externalState
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_data_sources(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/datasources'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a datasource identified by id for a company
@@ -2581,15 +2556,15 @@
       :param companyId [int] The id of the company the datasource belongs to.
       :param id_ [int] The id of the datasource you wish to delete.
       :param model [DataSourceModel] 
       :return DataSourceModel
     """
     def update_data_source(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/datasources/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Lists all parents of an HS Code.
@@ -2606,15 +2581,15 @@
     
       :param country [string] The name or code of the destination country.
       :param hsCode [string] The partial or full HS Code for which you would like to view all of the parents.
       :return FetchResult
     """
     def get_cross_border_code(self, country, hsCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/crossborder/{}/{}/hierarchy'.format(self.base_url, country, hsCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Test whether a form supports online login verification
@@ -2627,15 +2602,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def get_login_verifier_by_form(self, form, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/filingcalendars/loginverifiers/{}'.format(self.base_url, form),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all market place locations.
@@ -2646,15 +2621,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_all_marketplace_locations(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/listallmarketplacelocations'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of the AvaFile Forms available
@@ -2668,15 +2643,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_ava_file_forms(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/avafileforms'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List certificate attributes used by a company
@@ -2692,15 +2667,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_certificate_attributes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/certificateattributes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List the certificate exempt reasons defined by a company
@@ -2715,15 +2690,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_certificate_exempt_reasons(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/certificateexemptreasons'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List certificate exposure zones used by a company
@@ -2738,15 +2713,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_certificate_exposure_zones(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/certificateexposurezones'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported usage of extra parameters for classification of a item.
@@ -2759,15 +2734,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_classification_parameters_usage(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/classification/parametersusage'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of communications service types
@@ -2779,15 +2754,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_communications_service_types(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/communications/transactiontypes/{}/servicetypes'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of communications transactiontypes
@@ -2799,15 +2774,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_communications_transaction_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/communications/transactiontypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of communications transaction/service type pairs
@@ -2819,15 +2794,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_communications_t_s_pairs(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/communications/tspairs'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all ISO 3166 countries
@@ -2840,15 +2815,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_countries(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/countries'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List certificate exposure zones used by a company
@@ -2864,15 +2839,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_cover_letters(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/coverletters'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Lists the next level of HS Codes given a destination country and HS Code prefix.
@@ -2892,15 +2867,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_cross_border_codes(self, country, hsCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/crossborder/{}/{}'.format(self.base_url, country, hsCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List top level HS Code Sections.
@@ -2913,15 +2888,15 @@
       ### Security Policies
       * This API depends on the following active services:*Required* (all): AvaTaxGlobal.
     
       :return FetchResult
     """
     def list_cross_border_sections(self):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/crossborder/sections'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all ISO 4217 currencies supported by AvaTax.
@@ -2934,15 +2909,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_currencies(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/currencies'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported entity use codes
@@ -2957,15 +2932,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_entity_use_codes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/entityusecodes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported filing frequencies.
@@ -2977,37 +2952,37 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_filing_frequencies(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/filingfrequencies'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List jurisdictions based on the filter provided
     
     Returns a list of all Avalara-supported taxing jurisdictions.
       This API allows you to examine all Avalara-supported jurisdictions. You can filter your search by supplying
       SQL-like query for fetching only the ones you concerned about. For example: effectiveDate > '2016-01-01'
       The rate, salesRate, and useRate fields are not available on the JurisdictionModels returned by this API.
     
-      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* rate, salesRate, signatureCode, useRate
+      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* rate, salesRate, signatureCode, useRate, isAcm, isSst
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_jurisdictions(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/jurisdictions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List jurisdictions near a specific address
@@ -3029,15 +3004,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_jurisdictions_by_address(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/jurisdictionsnearaddress'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List jurisdictions based on the provided taxTypeId, taxSubTypeId, country, and rateTypeId
@@ -3057,15 +3032,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_jurisdictions_by_rate_type_tax_type_mapping(self, country, taxTypeId, taxSubTypeId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/jurisdictions/countries/{}/taxtypes/{}/taxsubtypes/{}'.format(self.base_url, country, taxTypeId, taxSubTypeId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List jurisdiction types based on the provided taxTypeId, taxSubTypeId, country, and rateTypeId
@@ -3076,15 +3051,15 @@
       :param taxTypeId [string] The taxtype for which you want to retrieve the jurisdiction information
       :param taxSubTypeId [string] The taxsubtype for which you want to retrieve the jurisdiction information
       :param rateTypeId [string] The ratetype for which you want to retrieve the jurisdiction information
       :return string
     """
     def list_jurisdiction_types_by_rate_type_tax_type_mapping(self, country, taxTypeId, taxSubTypeId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/jurisdictionTypes/countries/{}/taxtypes/{}/taxsubtypes/{}'.format(self.base_url, country, taxTypeId, taxSubTypeId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list of questions that are required for a tax location
@@ -3109,15 +3084,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_location_questions_by_address(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/locationquestions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all forms where logins can be verified automatically
@@ -3130,15 +3105,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_login_verifiers(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/filingcalendars/loginverifiers'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list of locations for a marketplace.
@@ -3149,15 +3124,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_marketplace_locations(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/marketplacelocations'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported nexus for all countries and regions.
@@ -3169,15 +3144,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexus'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all nexus that apply to a specific address.
@@ -3199,15 +3174,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_by_address(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexus/byaddress'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported nexus for a country.
@@ -3220,15 +3195,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_by_country(self, country, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexus/{}'.format(self.base_url, country),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported nexus for a country and region.
@@ -3242,15 +3217,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_by_country_and_region(self, country, region, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexus/{}/{}'.format(self.base_url, country, region),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List nexus related to a tax form
@@ -3267,15 +3242,15 @@
       * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param formCode [string] The form code that we are looking up the nexus for
       :return NexusByTaxFormModel
     """
     def list_nexus_by_form_code(self, formCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexus/byform/{}'.format(self.base_url, formCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported nexus for a tax type group.
@@ -3288,15 +3263,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_by_tax_type_group(self, taxTypeGroup, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexus/bytaxtypegroup/{}'.format(self.base_url, taxTypeGroup),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of nexus tax type groups
@@ -3308,15 +3283,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_tax_type_groups(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/nexustaxtypegroups'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice customer funding options.
@@ -3328,15 +3303,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_customer_funding_options(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticecustomerfundingoptions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice customer types.
@@ -3348,15 +3323,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_customer_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticecustomertypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice filing types.
@@ -3368,15 +3343,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_filingtypes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticefilingtypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice priorities.
@@ -3388,15 +3363,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_priorities(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticepriorities'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice reasons.
@@ -3408,15 +3383,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_reasons(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticereasons'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice responsibility ids
@@ -3428,15 +3403,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_responsibilities(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticeresponsibilities'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice root causes
@@ -3448,15 +3423,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_root_causes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticerootcauses'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice statuses.
@@ -3468,15 +3443,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_statuses(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticestatuses'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax notice types.
@@ -3488,15 +3463,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notice_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/noticetypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported extra parameters for creating transactions.
@@ -3509,21 +3484,41 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_parameters(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/parameters'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
+    Retrieve the list of Avalara-supported parameters based on account subscriptions.
+    
+    Returns the list of Avalara-supported parameters based on account subscriptions.
+    
+      :param accountId [int] The ID of the account to retrieve the parameters.
+      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* serviceTypes, regularExpression, values
+      :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
+      :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
+      :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
+      :return FetchResult
+    """
+    def list_parameters_by_account(self, accountId, include=None):
+        if ('X-Avalara-Client' in self.client_header): 
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
+        return requests.get('{}/api/v2/definitions/accounts/{}/parameters'.format(self.base_url, accountId),
+                               auth=self.auth, headers=self.client_header, params=include, 
+                               timeout=self.timeout_limit if self.timeout_limit else 1200)
+    r"""
+    Swagger Name: AvaTaxClient
+    
     Retrieve the parameters by companyCode and itemCode.
     
     Returns the list of parameters based on the company's service types and the item code.
       Ignores nexus if a service type is configured in the 'IgnoreNexusForServiceTypes' configuration section.
       Ignores nexus for the AvaAlcohol service type.
       NOTE: If your company code or item code contains any of these characters /, +, ? or a space, please use the following encoding before making a request:
       * Replace '/' with '\_-ava2f-\_' For example: 'Company/Code' becomes 'Company_-ava2f-_Code'
@@ -3543,15 +3538,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_parameters_by_item(self, companyCode, itemCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/parameters/byitem/{}/{}'.format(self.base_url, companyCode, itemCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported usage of extra parameters for creating transactions.
@@ -3564,15 +3559,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_parameters_usage(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/parametersusage'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported permissions
@@ -3582,15 +3577,15 @@
     
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :return FetchResult
     """
     def list_permissions(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/permissions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported postal codes.
@@ -3601,15 +3596,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_postal_codes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/postalcodes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all customs duty programs recognized by AvaTax
@@ -3626,15 +3621,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_preferred_programs(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/preferredprograms'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all available product classification systems.
@@ -3648,15 +3643,15 @@
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :param countryCode [string] If not null, return all records with this code.
       :return FetchResult
     """
     def list_product_classification_systems(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/productclassificationsystems'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all product classification systems available to a company based on its nexus.
@@ -3677,15 +3672,15 @@
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :param countryCode [string] If not null, return all records with this code.
       :return FetchResult
     """
     def list_product_classification_systems_by_company(self, companyCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/productclassificationsystems/bycompany/{}'.format(self.base_url, companyCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of rate types for each country
@@ -3698,15 +3693,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_rate_types_by_country(self, country, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/countries/{}/ratetypes'.format(self.base_url, country),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list of rate types by country, TaxType and by TaxSubType
@@ -3721,15 +3716,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_rate_types_by_country_tax_type_tax_sub_type(self, country, taxTypeId, taxSubTypeId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/countries/{}/taxtypes/{}/taxsubtypes/{}/ratetypes'.format(self.base_url, country, taxTypeId, taxSubTypeId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all ISO 3166 regions
@@ -3742,15 +3737,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_regions(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/regions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all ISO 3166 regions for a country
@@ -3764,15 +3759,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_regions_by_country(self, country, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/countries/{}/regions'.format(self.base_url, country),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list of applicable regions by country tax type, tax sub type, and rate type for a given JurisdictionTypeId
@@ -3790,15 +3785,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_regions_by_country_and_tax_type_and_tax_sub_type_and_rate_type(self, companyId, country, taxTypeId, taxSubTypeId, rateTypeId, jurisdictionTypeId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/companies/{}/countries/{}/regions/taxtypes/{}/taxsubtypes/{}/rateTypeId/{}/jurisdictionTypeId/{}'.format(self.base_url, companyId, country, taxTypeId, taxSubTypeId, rateTypeId, jurisdictionTypeId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported resource file types
@@ -3810,15 +3805,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_resource_file_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/resourcefiletypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported usage of parameters used for returns.
@@ -3831,15 +3826,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_returns_parameters_usage(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/returns/parametersusage'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported permissions
@@ -3852,37 +3847,37 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_security_roles(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/securityroles'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported subscription types
     
     Returns the full list of Avalara-supported subscription types.
       This API is intended to be useful for identifying which features you have added to your account.
       You may always contact Avalara's sales department for information on available products or services.
       You cannot change your subscriptions directly through the API.
     
-      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
+      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* taxTypeGroupIdSK
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_subscription_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/subscriptiontypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list all tags supported by avalara
@@ -3893,15 +3888,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tags(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/tags'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax authorities.
@@ -3913,15 +3908,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_authorities(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxauthorities'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported forms for each tax authority.
@@ -3935,15 +3930,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_authority_forms(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxauthorityforms'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax authority types.
@@ -3955,40 +3950,40 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_authority_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxauthoritytypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax codes.
     
     Retrieves the list of Avalara-supported system tax codes.
       A 'TaxCode' represents a uniquely identified type of product, good, or service.
       Avalara supports correct tax rates and taxability rules for all TaxCodes in all supported jurisdictions.
       If you identify your products by tax code in your 'Create Transacion' API calls, Avalara will correctly calculate tax rates and
       taxability rules for this product in all supported jurisdictions.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_codes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxcodes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported tax code types.
@@ -3999,15 +3994,15 @@
     
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :return TaxCodeTypesModel
     """
     def list_tax_code_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxcodetypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of the Tax Forms available
@@ -4019,15 +4014,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_forms(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxforms'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of tax sub types
@@ -4039,15 +4034,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_sub_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxsubtypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of tax sub types by Country and TaxType
@@ -4062,15 +4057,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_sub_types_by_country_and_tax_type(self, country, taxTypeId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxsubtypes/countries/{}/taxtypes/{}'.format(self.base_url, country, taxTypeId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of tax sub types by jurisdiction code and region
@@ -4084,15 +4079,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_sub_types_by_jurisdiction_and_region(self, jurisdictionCode, region, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxsubtypes/{}/{}'.format(self.base_url, jurisdictionCode, region),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of tax type groups
@@ -4104,15 +4099,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_type_groups(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxtypegroups'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list of applicable TaxTypes
@@ -4124,15 +4119,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_types_by_nexus_and_country(self, country, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/taxtypes/countries/{}'.format(self.base_url, country),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the list of applicable UnitOfBasis
@@ -4146,15 +4141,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_unit_of_basis_by_country_and_tax_type_and_tax_sub_type_and_rate_type(self, country, taxTypeId, taxSubTypeId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/unitofbasis/countries/{}/taxtypes/{}/taxsubtypes/{}'.format(self.base_url, country, taxTypeId, taxSubTypeId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all defined units of measurement
@@ -4166,15 +4161,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_unit_of_measurement(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/definitions/unitofmeasurements'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create one or more DistanceThreshold objects
@@ -4188,15 +4183,15 @@
     
       :param companyId [int] The unique ID number of the company that owns this DistanceThreshold
       :param model [CompanyDistanceThresholdModel] The DistanceThreshold object or objects you wish to create.
       :return CompanyDistanceThresholdModel
     """
     def create_distance_threshold(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/distancethresholds'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single DistanceThreshold object
@@ -4210,15 +4205,15 @@
     
       :param companyId [int] The unique ID number of the company that owns this DistanceThreshold
       :param id_ [int] The unique ID number of the DistanceThreshold object you wish to delete.
       :return ErrorDetail
     """
     def delete_distance_threshold(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/distancethresholds/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single DistanceThreshold
@@ -4232,15 +4227,15 @@
     
       :param companyId [int] The ID of the company that owns this DistanceThreshold object
       :param id_ [int] The unique ID number referring to this DistanceThreshold object
       :return CompanyDistanceThresholdModel
     """
     def get_distance_threshold(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/distancethresholds/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all DistanceThresholds for this company.
@@ -4258,15 +4253,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_distance_thresholds(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/distancethresholds'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all DistanceThreshold objects
@@ -4285,15 +4280,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_distance_thresholds(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/distancethresholds'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a DistanceThreshold object
@@ -4310,55 +4305,55 @@
       :param companyId [int] The unique ID number of the company that owns this DistanceThreshold object.
       :param id_ [int] The unique ID number of the DistanceThreshold object to replace.
       :param model [CompanyDistanceThresholdModel] The new DistanceThreshold object to store.
       :return CompanyDistanceThresholdModel
     """
     def update_distance_threshold(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/distancethresholds/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new eCommerce token.
     
     Creates a new eCommerce token.
       This API is used to create a new eCommerce token. An eCommerce token is required in order to launch the CertCapture eCommerce plugin. Create a token for each of your CertCapture customers.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The company ID that will be issued this certificate.
       :param model [CreateECommerceTokenInputModel] 
       :return ECommerceTokenOutputModel
     """
     def create_e_commerce_token(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/ecommercetokens'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Refresh an eCommerce token.
     
     Refresh an eCommerce token.
       CertCapture eCommerce tokens expire after one hour. This API is used to refresh an eCommerce token that is about to expire. This API can only be used with active tokens. If your token has expired, you must generate a new one.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The company ID that the refreshed certificate belongs to.
       :param model [RefreshECommerceTokenInputModel] 
       :return FetchResult
     """
     def refresh_e_commerce_token(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/ecommercetokens'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Approves linkage to a firm for a client account
@@ -4368,15 +4363,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] 
       :return FirmClientLinkageOutputModel
     """
     def approve_firm_client_linkage(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/firmclientlinkages/{}/approve'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Request a new FirmClient account and create an approved linkage to it
@@ -4392,15 +4387,15 @@
       * This API requires one of the following user roles: FirmAdmin, Registrar, SiteAdmin, SystemAdmin.
     
       :param model [NewFirmClientAccountRequestModel] Information about the account you wish to create.
       :return FirmClientLinkageOutputModel
     """
     def create_and_link_new_firm_client_account(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/firmclientlinkages/createandlinkclient'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Links a firm account with the client account
@@ -4410,15 +4405,15 @@
       * This API requires one of the following user roles: BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param model [FirmClientLinkageInputModel] FirmClientLinkageInputModel
       :return FirmClientLinkageOutputModel
     """
     def create_firm_client_linkage(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/firmclientlinkages'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a linkage
@@ -4428,51 +4423,51 @@
       * This API requires one of the following user roles: BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] 
       :return ErrorDetail
     """
     def delete_firm_client_linkage(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/firmclientlinkages/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get linkage between a firm and client by id
     
     This API enables the firm admins/firm users to request the linkage of a firm account and a client account.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] 
       :return FirmClientLinkageOutputModel
     """
     def get_firm_client_linkage(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/firmclientlinkages/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List client linkages for a firm or client
     
     This API enables the firm or account users to request the associated linkages to the account.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* firmAccountName, clientAccountName
       :return FetchResult
     """
     def list_firm_client_linkage(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/firmclientlinkages'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Rejects linkage to a firm for a client account
@@ -4482,15 +4477,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] 
       :return FirmClientLinkageOutputModel
     """
     def reject_firm_client_linkage(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/firmclientlinkages/{}/reject'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Reset linkage status between a client and firm back to requested
@@ -4500,15 +4495,15 @@
       * This API requires one of the following user roles: BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] 
       :return FirmClientLinkageOutputModel
     """
     def reset_firm_client_linkage(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/firmclientlinkages/{}/reset'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Revokes previously approved linkage to a firm for a client account
@@ -4518,15 +4513,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] 
       :return FirmClientLinkageOutputModel
     """
     def revoke_firm_client_linkage(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/firmclientlinkages/{}/revoke'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     FREE API - Request a free trial of AvaTax
@@ -4542,15 +4537,15 @@
       * This API may be called without providing authentication credentials.
     
       :param model [FreeTrialRequestModel] Required information to provision a free trial account.
       :return NewAccountModel
     """
     def request_free_trial(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/freetrials/request'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Request the javascript for a funding setup widget
@@ -4564,25 +4559,25 @@
       When the funding configuration is submitted to Avalara, it will be reviewed by treasury team members
       before approval.
       This API returns back the actual javascript code to insert into your application to render the
       JavaScript funding setup widget inline.
       Use the 'methodReturn.javaScript' return value to insert this widget into your HTML page.
       This API requires a subscription to Avalara Managed Returns or SST Certified Service Provider.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param id_ [int] The unique ID number of this funding request
       :param businessUnit [POABusinessUnit] The company's business unit (See POABusinessUnit::* for a list of allowable values)
       :param subscriptionType [POASubscriptionType] The company's subscription type (See POASubscriptionType::* for a list of allowable values)
       :return FundingStatusModel
     """
     def activate_funding_request(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/fundingrequests/{}/widget'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve status about a funding setup request
@@ -4604,15 +4599,15 @@
       :param id_ [int] The unique ID number of this funding request
       :param businessUnit [POABusinessUnit] The company's business unit (See POABusinessUnit::* for a list of allowable values)
       :param subscriptionType [POASubscriptionType] The company's subscription type (See POASubscriptionType::* for a list of allowable values)
       :return FundingStatusModel
     """
     def funding_request_status(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/fundingrequests/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete all classifications for an item
@@ -4625,15 +4620,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param itemId [int] The ID of the item you wish to delete the classifications.
       :return ErrorDetail
     """
     def batch_delete_item_classifications(self, companyId, itemId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}/classifications'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete all parameters for an item
@@ -4647,15 +4642,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param itemId [int] The ID of the item you wish to delete the parameters.
       :return ErrorDetail
     """
     def batch_delete_item_parameters(self, companyId, itemId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}/parameters'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Bulk upload items from a product catalog
@@ -4672,15 +4667,15 @@
     
       :param companyId [int] The ID of the company that owns this items.
       :param model [ItemBulkUploadInputModel] The items you wish to upload.
       :return ItemBulkUploadOutputModel
     """
     def bulk_upload_items(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/items/upload'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Add classifications to an item.
@@ -4695,15 +4690,15 @@
       :param companyId [int] The company id.
       :param itemId [int] The item id.
       :param model [ItemClassificationInputModel] The item classifications you wish to create.
       :return ItemClassificationOutputModel
     """
     def create_item_classifications(self, companyId, itemId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/items/{}/classifications'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Add parameters to an item.
@@ -4720,15 +4715,15 @@
       :param companyId [int] The ID of the company that owns this item parameter.
       :param itemId [int] The item id.
       :param model [ItemParameterModel] The item parameters you wish to create.
       :return ItemParameterModel
     """
     def create_item_parameters(self, companyId, itemId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/items/{}/parameters'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new item
@@ -4745,15 +4740,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param model [ItemModel] The item you wish to create.
       :return ItemModel
     """
     def create_items(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/items'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create tags for a item
@@ -4766,15 +4761,15 @@
       :param companyId [int] The ID of the company that defined these items
       :param itemId [int] The ID of the item as defined by the company that owns this tag.
       :param model [ItemTagDetailInputModel] Tags you wish to associate with the Item
       :return ItemTagDetailOutputModel
     """
     def create_item_tags(self, companyId, itemId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/items/{}/tags'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new tax code classification request
@@ -4788,15 +4783,15 @@
     
       :param companyId [int] The ID of the company that creates this request.
       :param model [ItemTaxCodeClassificationRequestInputModel] The request you wish to create.
       :return ItemTaxCodeClassificationRequestOutputModel
     """
     def create_tax_code_classification_request(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/classificationrequests/taxcode'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single item
@@ -4818,15 +4813,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param itemCode [string] The code of the item you want to delete.
       :return ErrorDetail
     """
     def delete_catalogue_item(self, companyId, itemCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/itemcatalogue/{}'.format(self.base_url, companyId, itemCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single item
@@ -4843,15 +4838,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param id_ [int] The ID of the item you wish to delete.
       :return ErrorDetail
     """
     def delete_item(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single item classification.
@@ -4865,15 +4860,15 @@
       :param companyId [int] The company id.
       :param itemId [int] The item id.
       :param id_ [int] The item classification id.
       :return ErrorDetail
     """
     def delete_item_classification(self, companyId, itemId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}/classifications/{}'.format(self.base_url, companyId, itemId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single item parameter
@@ -4888,15 +4883,15 @@
       :param companyId [int] The company id
       :param itemId [int] The item id
       :param id_ [int] The parameter id
       :return ErrorDetail
     """
     def delete_item_parameter(self, companyId, itemId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}/parameters/{}'.format(self.base_url, companyId, itemId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete item tag by id
@@ -4909,15 +4904,15 @@
       :param companyId [int] The ID of the company that defined these items
       :param itemId [int] The ID of the item as defined by the company that owns this tag.
       :param itemTagDetailId [int] The ID of the item tag detail you wish to delete.
       :return ErrorDetail
     """
     def delete_item_tag(self, companyId, itemId, itemTagDetailId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}/tags/{}'.format(self.base_url, companyId, itemId, itemTagDetailId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete all item tags
@@ -4929,15 +4924,15 @@
     
       :param companyId [int] The ID of the company that defined these items.
       :param itemId [int] The ID of the item as defined by the company that owns this tag.
       :return ErrorDetail
     """
     def delete_item_tags(self, companyId, itemId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/items/{}/tags'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get status of classification requests of a company
@@ -4956,15 +4951,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def get_classification_status(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/classificationrequests/taxcode'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single item
@@ -4981,15 +4976,15 @@
       :param companyId [int] The ID of the company that owns this item object
       :param id_ [int] The primary key of this item
       :param include [string] A comma separated list of additional data to retrieve.
       :return ItemModel
     """
     def get_item(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single item classification.
@@ -5003,15 +4998,15 @@
       :param companyId [int] The company id.
       :param itemId [int] The item id.
       :param id_ [int] The item classification id.
       :return ItemClassificationOutputModel
     """
     def get_item_classification(self, companyId, itemId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/classifications/{}'.format(self.base_url, companyId, itemId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single item parameter
@@ -5026,15 +5021,15 @@
       :param companyId [int] The company id
       :param itemId [int] The item id
       :param id_ [int] The parameter id
       :return ItemParameterModel
     """
     def get_item_parameter(self, companyId, itemId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/parameters/{}'.format(self.base_url, companyId, itemId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve tags for an item
@@ -5049,15 +5044,15 @@
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* tagName
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :return FetchResult
     """
     def get_item_tags(self, companyId, itemId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/tags'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve premium classification for a company's item based on its ItemCode and SystemCode.
@@ -5077,15 +5072,15 @@
       :param companyId [int] The ID of the company that owns this item object
       :param itemCode [string] The ItemCode of the item for which you want to retrieve premium classification
       :param systemCode [string] The SystemCode for which you want to retrieve premium classification
       :return ItemPremiumClassificationOutputModel
     """
     def get_premium_classification(self, companyId, itemCode, systemCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/premiumClassification/{}'.format(self.base_url, companyId, itemCode, systemCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get tax code recommendations
@@ -5103,15 +5098,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def get_tax_code_recommendations(self, companyId, requestId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/classificationrequests/taxcode/{}/recommendations'.format(self.base_url, companyId, requestId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve Restrictions for Item by CountryOfImport
@@ -5134,15 +5129,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_import_restrictions(self, companyId, itemCode, countryOfImport, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/restrictions/import/{}'.format(self.base_url, companyId, itemCode, countryOfImport),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve classifications for an item.
@@ -5161,15 +5156,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_item_classifications(self, companyId, itemId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/classifications'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve parameters for an item
@@ -5189,15 +5184,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_item_parameters(self, companyId, itemId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/{}/parameters'.format(self.base_url, companyId, itemId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve items for this company
@@ -5226,15 +5221,15 @@
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :param tagName [string] Tag Name on the basis of which you want to filter Items
       :return FetchResult
     """
     def list_items_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all items
@@ -5255,15 +5250,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_items(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/items'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all items associated with given tag
@@ -5286,15 +5281,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_items_by_tag(self, companyId, tag, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/items/bytags/{}'.format(self.base_url, companyId, tag),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create or update items from a product catalog.
@@ -5309,15 +5304,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param model [ItemCatalogueInputModel] The items you want to create or update.
       :return ItemCatalogueOutputModel
     """
     def sync_item_catalogue(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/itemcatalogue'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Sync items from a product catalog
@@ -5336,15 +5331,15 @@
     
       :param companyId [int] The ID of the company that owns this item.
       :param model [SyncItemsRequestModel] The request object.
       :return SyncItemsResponseModel
     """
     def sync_items(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/items/sync'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single item
@@ -5364,15 +5359,15 @@
       :param companyId [int] The ID of the company that this item belongs to.
       :param id_ [int] The ID of the item you wish to update
       :param model [ItemModel] The item object you wish to update.
       :return ItemModel
     """
     def update_item(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/items/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update an item classification.
@@ -5388,15 +5383,15 @@
       :param itemId [int] The item id.
       :param id_ [int] The item classification id.
       :param model [ItemClassificationInputModel] The item object you wish to update.
       :return ItemClassificationOutputModel
     """
     def update_item_classification(self, companyId, itemId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/items/{}/classifications/{}'.format(self.base_url, companyId, itemId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update an item parameter
@@ -5412,15 +5407,15 @@
       :param itemId [int] The item id
       :param id_ [int] The item parameter id
       :param model [ItemParameterModel] The item object you wish to update.
       :return ItemParameterModel
     """
     def update_item_parameter(self, companyId, itemId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/items/{}/parameters/{}'.format(self.base_url, companyId, itemId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create one or more overrides
@@ -5435,15 +5430,15 @@
     
       :param accountId [int] The ID of the account that owns this override
       :param model [JurisdictionOverrideModel] The jurisdiction override objects to create
       :return JurisdictionOverrideModel
     """
     def create_jurisdiction_overrides(self, accountId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/jurisdictionoverrides'.format(self.base_url, accountId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single override
@@ -5454,15 +5449,15 @@
     
       :param accountId [int] The ID of the account that owns this override
       :param id_ [int] The ID of the override you wish to delete
       :return ErrorDetail
     """
     def delete_jurisdiction_override(self, accountId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/accounts/{}/jurisdictionoverrides/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single override
@@ -5477,15 +5472,15 @@
     
       :param accountId [int] The ID of the account that owns this override
       :param id_ [int] The primary key of this override
       :return JurisdictionOverrideModel
     """
     def get_jurisdiction_override(self, accountId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/jurisdictionoverrides/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve overrides for this account
@@ -5506,15 +5501,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_jurisdiction_overrides_by_account(self, accountId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/jurisdictionoverrides'.format(self.base_url, accountId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all overrides
@@ -5534,15 +5529,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_jurisdiction_overrides(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/jurisdictionoverrides'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single jurisdictionoverride
@@ -5554,15 +5549,15 @@
       :param accountId [int] The ID of the account that this jurisdictionoverride belongs to.
       :param id_ [int] The ID of the jurisdictionoverride you wish to update
       :param model [JurisdictionOverrideModel] The jurisdictionoverride object you wish to update.
       :return JurisdictionOverrideModel
     """
     def update_jurisdiction_override(self, accountId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/accounts/{}/jurisdictionoverrides/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Add parameters to a location.
@@ -5579,15 +5574,15 @@
       :param companyId [int] The ID of the company that owns this location parameter.
       :param locationId [int] The location id.
       :param model [LocationParameterModel] The location parameters you wish to create.
       :return LocationParameterModel
     """
     def create_location_parameters(self, companyId, locationId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/locations/{}/parameters'.format(self.base_url, companyId, locationId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new location
@@ -5598,15 +5593,15 @@
     
       :param companyId [int] The ID of the company that owns this location.
       :param model [LocationModel] The location you wish to create.
       :return LocationModel
     """
     def create_locations(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/locations'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single location
@@ -5617,15 +5612,15 @@
     
       :param companyId [int] The ID of the company that owns this location.
       :param id_ [int] The ID of the location you wish to delete.
       :return ErrorDetail
     """
     def delete_location(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/locations/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single location parameter
@@ -5640,15 +5635,15 @@
       :param companyId [int] The company id
       :param locationId [int] The location id
       :param id_ [int] The parameter id
       :return ErrorDetail
     """
     def delete_location_parameter(self, companyId, locationId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/locations/{}/parameters/{}'.format(self.base_url, companyId, locationId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single location
@@ -5658,47 +5653,47 @@
       Many taxing authorities require that you define a list of all locations where your company does business.
       These locations may require additional custom configuration or tax registration with these authorities.
       For more information on metadata requirements, see the '/api/v2/definitions/locationquestions' API.
       You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * LocationSettings
       * parameters
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The ID of the company that owns this location
       :param id_ [int] The primary key of this location
       :param include [string] A comma separated list of additional data to retrieve.
       :return LocationModel
     """
     def get_location(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/locations/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single company location parameter
     
     Retrieve a single location parameter.
       Some locations can be taxed differently depending on the properties of that location. In AvaTax, these tax-affecting properties are called "parameters".
       A parameter added to a location will be used by default in tax calculation but will not show on the transaction line referencing the location.
       A parameter specified on a transaction line will override a location parameter if they share the same parameter name.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The company id
       :param locationId [int] The location id
       :param id_ [int] The parameter id
       :return LocationParameterModel
     """
     def get_location_parameter(self, companyId, locationId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/locations/{}/parameters/{}'.format(self.base_url, companyId, locationId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve parameters for a location
@@ -5706,27 +5701,27 @@
     List parameters for a location.
       Some locations can be taxed differently depending on the properties of that location. In AvaTax, these tax-affecting properties are called "parameters".
       A parameter added to a location will be used by default in tax calculation but will not show on the transaction line referencing the location.
       A parameter specified on a transaction line will override a location parameter if they share the same parameter name.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The company id
       :param locationId [int] The ID of the location
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* name, unit
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_location_parameters(self, companyId, locationId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/locations/{}/parameters'.format(self.base_url, companyId, locationId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve locations for this company
@@ -5738,27 +5733,27 @@
       For more information on metadata requirements, see the '/api/v2/definitions/locationquestions' API.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * LocationSettings
       * parameters
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The ID of the company that owns these locations
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* isMarketplaceOutsideUsa, settings, parameters
       :param include [string] A comma separated list of additional data to retrieve.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_locations_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/locations'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all locations
@@ -5770,26 +5765,26 @@
       For more information on metadata requirements, see the '/api/v2/definitions/locationquestions' API.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * LocationSettings
       * parameters
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* isMarketplaceOutsideUsa, settings, parameters
       :param include [string] A comma separated list of additional data to retrieve. You may specify `LocationSettings` to retrieve location settings.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_locations(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/locations'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single location
@@ -5803,15 +5798,15 @@
       :param companyId [int] The ID of the company that this location belongs to.
       :param id_ [int] The ID of the location you wish to update
       :param model [LocationModel] The location you wish to update.
       :return LocationModel
     """
     def update_location(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/locations/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a location parameter
@@ -5827,36 +5822,36 @@
       :param locationId [int] The location id
       :param id_ [int] The location parameter id
       :param model [LocationParameterModel] The location parameter object you wish to update.
       :return LocationParameterModel
     """
     def update_location_parameter(self, companyId, locationId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/locations/{}/parameters/{}'.format(self.base_url, companyId, locationId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Validate the location against local requirements
     
     Returns validation information for this location.
       This API call is intended to compare this location against the currently known taxing authority rules and regulations,
       and provide information about what additional work is required to completely setup this location.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param companyId [int] The ID of the company that owns this location
       :param id_ [int] The primary key of this location
       :return LocationValidationModel
     """
     def validate_location(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/locations/{}/validate'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Adjust a MultiDocument transaction
@@ -5882,15 +5877,15 @@
       :param type [DocumentType] The transaction type for this MultiDocument transaction (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [AdjustMultiDocumentModel] The adjust request you wish to execute
       :return MultiDocumentModel
     """
     def adjust_multi_document_transaction(self, code, type, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/multidocument/{}/type/{}/adjust'.format(self.base_url, code, type),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get audit information about a MultiDocument transaction
@@ -5919,15 +5914,15 @@
     
       :param code [string] The transaction code for this MultiDocument transaction
       :param type [DocumentType] The transaction type for this MultiDocument transaction (See DocumentType::* for a list of allowable values)
       :return AuditMultiDocumentModel
     """
     def audit_multi_document_transaction(self, code, type):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/transactions/multidocument/{}/type/{}/audit'.format(self.base_url, code, type),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Commit a MultiDocument transaction
@@ -5949,15 +5944,15 @@
       * This API depends on the following active services:*Required* (all): AvaTaxPro.
     
       :param model [CommitMultiDocumentModel] The commit request you wish to execute
       :return MultiDocumentModel
     """
     def commit_multi_document_transaction(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/multidocument/commit'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new MultiDocument transaction
@@ -5999,15 +5994,15 @@
     
       :param include [string] Specifies objects to include in the response after transaction is created
       :param model [CreateMultiDocumentModel] the multi document transaction model
       :return MultiDocumentModel
     """
     def create_multi_document_transaction(self, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/multidocument'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a MultiDocument transaction
@@ -6035,15 +6030,15 @@
       :param code [string] The multidocument code to retrieve
       :param type [DocumentType] The transaction type to retrieve (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in the response after transaction is created
       :return MultiDocumentModel
     """
     def get_multi_document_transaction_by_code_and_type(self, code, type, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/transactions/multidocument/{}/type/{}'.format(self.base_url, code, type),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a MultiDocument transaction by ID
@@ -6077,15 +6072,15 @@
     
       :param id_ [int] The unique ID number of the MultiDocument transaction to retrieve
       :param include [string] Specifies objects to include in the response after transaction is created
       :return MultiDocumentModel
     """
     def get_multi_document_transaction_by_id(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/transactions/multidocument/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all MultiDocument transactions
@@ -6120,15 +6115,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_multi_document_transactions(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/transactions/multidocument'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a refund for a MultiDocument transaction
@@ -6175,15 +6170,15 @@
       :param type [DocumentType] The type of this MultiDocument transaction (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in the response after transaction is created
       :param model [RefundTransactionModel] Information about the refund to create
       :return MultiDocumentModel
     """
     def refund_multi_document_transaction(self, code, type, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/multidocument/{}/type/{}/refund'.format(self.base_url, code, type),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Verify a MultiDocument transaction
@@ -6204,15 +6199,15 @@
       * This API depends on the following active services:*Required* (all): AvaTaxPro.
     
       :param model [VerifyMultiDocumentModel] Information from your accounting system to verify against this MultiDocument transaction as it is stored in AvaTax
       :return MultiDocumentModel
     """
     def verify_multi_document_transaction(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/multidocument/verify'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Void a MultiDocument transaction
@@ -6237,15 +6232,15 @@
       :param code [string] The transaction code for this MultiDocument transaction
       :param type [DocumentType] The transaction type for this MultiDocument transaction (See DocumentType::* for a list of allowable values)
       :param model [VoidTransactionModel] The void request you wish to execute
       :return MultiDocumentModel
     """
     def void_multi_document_transaction(self, code, type, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/multidocument/{}/type/{}/void'.format(self.base_url, code, type),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new nexus
@@ -6269,15 +6264,15 @@
     
       :param companyId [int] The ID of the company that owns this nexus.
       :param model [NexusModel] The nexus you wish to create.
       :return NexusModel
     """
     def create_nexus(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/nexus'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Add parameters to a nexus.
@@ -6294,15 +6289,15 @@
       :param companyId [int] The ID of the company that owns this nexus parameter.
       :param nexusId [int] The nexus id.
       :param model [NexusParameterDetailModel] The nexus parameters you wish to create.
       :return NexusParameterDetailModel
     """
     def create_nexus_parameters(self, companyId, nexusId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/nexus/{}/parameters'.format(self.base_url, companyId, nexusId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Creates nexus for a list of addresses.
@@ -6323,15 +6318,15 @@
     
       :param companyId [int] The ID of the company that will own this nexus.
       :param model [DeclareNexusByAddressModel] The nexus you wish to create.
       :return NexusByAddressModel
     """
     def declare_nexus_by_address(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/nexus/byaddress'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single nexus
@@ -6348,15 +6343,15 @@
       :param companyId [int] The ID of the company that owns this nexus.
       :param id_ [int] The ID of the nexus you wish to delete.
       :param cascadeDelete [boolean] If true, deletes all the child nexus if they exist along with parent nexus
       :return ErrorDetail
     """
     def delete_nexus(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/nexus/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single nexus parameter
@@ -6371,15 +6366,15 @@
       :param companyId [int] The company id
       :param nexusId [int] The nexus id
       :param id_ [int] The parameter id
       :return ErrorDetail
     """
     def delete_nexus_parameter(self, companyId, nexusId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/nexus/{}/parameters/{}'.format(self.base_url, companyId, nexusId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete all parameters for an nexus
@@ -6393,15 +6388,15 @@
     
       :param companyId [int] The ID of the company that owns this nexus.
       :param nexusId [int] The ID of the nexus you wish to delete the parameters.
       :return ErrorDetail
     """
     def delete_nexus_parameters(self, companyId, nexusId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/nexus/{}/parameters'.format(self.base_url, companyId, nexusId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single nexus
@@ -6418,15 +6413,15 @@
       :param companyId [int] The ID of the company that owns this nexus object
       :param id_ [int] The primary key of this nexus
       :param include [string] 
       :return NexusModel
     """
     def get_nexus(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/nexus/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List company nexus related to a tax form
@@ -6446,15 +6441,15 @@
       :param companyId [int] The ID of the company that owns this nexus object
       :param formCode [string] The form code that we are looking up the nexus for
       :param include [string] 
       :return NexusByTaxFormModel
     """
     def get_nexus_by_form_code(self, companyId, formCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/nexus/byform/{}'.format(self.base_url, companyId, formCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single nexus parameter
@@ -6469,15 +6464,15 @@
       :param companyId [int] The company id
       :param nexusId [int] The nexus id
       :param id_ [int] The parameter id
       :return NexusParameterDetailModel
     """
     def get_nexus_parameter(self, companyId, nexusId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/nexus/{}/parameters/{}'.format(self.base_url, companyId, nexusId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve nexus for this company
@@ -6499,15 +6494,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/nexus'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve nexus for this company By TaxTypeGroup
@@ -6530,15 +6525,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_by_company_and_tax_type_group(self, companyId, taxTypeGroup, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/nexus/byTaxTypeGroup/{}'.format(self.base_url, companyId, taxTypeGroup),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve parameters for a nexus
@@ -6558,15 +6553,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_nexus_parameters(self, companyId, nexusId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/nexus/{}/parameters'.format(self.base_url, companyId, nexusId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all nexus
@@ -6587,15 +6582,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_nexus(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/nexus'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single nexus
@@ -6620,15 +6615,15 @@
       :param companyId [int] The ID of the company that this nexus belongs to.
       :param id_ [int] The ID of the nexus you wish to update
       :param model [NexusModel] The nexus object you wish to update.
       :return NexusModel
     """
     def update_nexus(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/nexus/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update an nexus parameter
@@ -6644,15 +6639,15 @@
       :param nexusId [int] The nexus id
       :param id_ [int] The nexus parameter id
       :param model [NexusParameterDetailModel] The nexus object you wish to update.
       :return NexusParameterDetailModel
     """
     def update_nexus_parameter(self, companyId, nexusId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/nexus/{}/parameters/{}'.format(self.base_url, companyId, nexusId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Creates a new tax notice responsibility type.
@@ -6663,15 +6658,15 @@
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param model [CreateNoticeResponsibilityTypeModel] The responsibility type to create
       :return NoticeResponsibilityModel
     """
     def create_notice_responsibility_type(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/notices/responsibilities'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Creates a new tax notice root cause type.
@@ -6682,15 +6677,15 @@
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param model [CreateNoticeRootCauseTypeModel] The root cause type to create
       :return NoticeRootCauseModel
     """
     def create_notice_root_cause_type(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/notices/rootcauses'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a tax notice responsibility type.
@@ -6700,15 +6695,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, CompanyAdmin, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPTester, FirmAdmin, FirmUser, SSTAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param responsibilityId [int] The unique ID of the responsibility type
       :return ErrorDetail
     """
     def delete_notice_responsibility_type(self, responsibilityId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/notices/responsibilities/{}'.format(self.base_url, responsibilityId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a tax notice root cause type.
@@ -6718,15 +6713,15 @@
       * This API requires one of the following user roles: AccountAdmin, BatchServiceAdmin, CompanyAdmin, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPTester, FirmAdmin, FirmUser, SSTAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param rootCauseId [int] The unique ID of the root cause type
       :return ErrorDetail
     """
     def delete_notice_root_cause_type(self, rootCauseId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/notices/rootcauses/{}'.format(self.base_url, rootCauseId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Mark a single notification as dismissed.
@@ -6738,22 +6733,22 @@
       An example of a notification would be a message about new software, or a change to AvaTax that may
       affect you, or a potential issue with your company's tax profile.
       When you dismiss a notification, the notification will track the user and time when it was
       dismissed. You can then later review which employees of your company dismissed notifications to
       determine if they were resolved appropriately.
       A Global notification with null accountId and companyId cannot be dismissed and will expire within a given time span.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The id of the notification you wish to mark as dismissed.
       :return NotificationModel
     """
     def dismiss_notification(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/notifications/{}/dismiss'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single notification.
@@ -6761,22 +6756,22 @@
     Retrieve a single notification by its unique ID number.
       A notification is a message from Avalara that may have relevance to your business. You may want
       to regularly review notifications and then dismiss them when you are certain that you have addressed
       any relevant concerns raised by this notification.
       An example of a notification would be a message about new software, or a change to AvaTax that may
       affect you, or a potential issue with your company's tax profile.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The id of the notification to retrieve.
       :return NotificationModel
     """
     def get_notification(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/notifications/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all notifications.
@@ -6786,25 +6781,25 @@
       to regularly review notifications and then dismiss them when you are certain that you have addressed
       any relevant concerns raised by this notification.
       An example of a notification would be a message about new software, or a change to AvaTax that may
       affect you, or a potential issue with your company's tax profile.
       You may search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_notifications(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/notifications'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Request a new Avalara account
@@ -6826,15 +6821,15 @@
       * This API is available by invitation only. To request access to this feature, please speak to a business development manager and request access to [Provisioning:RequestNewAccount].
     
       :param model [NewAccountRequestModel] Information about the account you wish to create and the selected product offerings.
       :return NewAccountModel
     """
     def request_new_account(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/request'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Request a new entitilement to an existing customer
@@ -6848,15 +6843,15 @@
     
       :param id_ [int] The avatax account id of the customer
       :param offer [string] The offer to be added to an already existing customer
       :return OfferModel
     """
     def request_new_entitlement(self, id_, offer):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/entitlements/{}'.format(self.base_url, id_, offer),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new account
@@ -6869,15 +6864,15 @@
       * This API requires one of the following user roles: BatchServiceAdmin, FirmAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param model [AccountModel] The account you wish to create.
       :return AccountModel
     """
     def create_account(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create new notifications.
@@ -6896,15 +6891,15 @@
       * This API is available by invitation only. To request access to this feature, please speak to a business development manager and request access to [NotificationsAPI:Create].
     
       :param model [NotificationModel] The notifications you wish to create.
       :return NotificationModel
     """
     def create_notifications(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/notifications'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create Avalara-supported subscription (ServiceTypes)
@@ -6919,15 +6914,15 @@
       * This API requires one of the following user roles: BatchServiceAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param model [SubscriptionTypeModel] The subscription type object you wish to create.
       :return SubscriptionTypeModel
     """
     def create_service_types(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/servicetypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new subscription
@@ -6941,15 +6936,15 @@
     
       :param accountId [int] The ID of the account that owns this subscription.
       :param model [SubscriptionModel] The subscription you wish to create.
       :return SubscriptionModel
     """
     def create_subscriptions(self, accountId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/subscriptions'.format(self.base_url, accountId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single account
@@ -6962,15 +6957,15 @@
       * This API requires the user role SystemAdmin.
     
       :param id_ [int] The ID of the account you wish to delete.
       :return ErrorDetail
     """
     def delete_account(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/accounts/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single notification.
@@ -6987,15 +6982,15 @@
       * This API is available by invitation only. To request access to this feature, please speak to a business development manager and request access to [NotificationsAPI:Create].
     
       :param id_ [int] The id of the notification you wish to delete.
       :return ErrorDetail
     """
     def delete_notification(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/notifications/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single Subscription (ServiceTypes) object
@@ -7008,15 +7003,15 @@
       * This API requires one of the following user roles: BatchServiceAdmin, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin.
     
       :param id_ [int] The unique ID number of the Subscription object you wish to delete.
       :return ErrorDetail
     """
     def delete_service_type(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/servicetypes/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single subscription
@@ -7029,15 +7024,15 @@
     
       :param accountId [int] The ID of the account that owns this subscription.
       :param id_ [int] The ID of the subscription you wish to delete.
       :return ErrorDetail
     """
     def delete_subscription(self, accountId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/accounts/{}/subscriptions/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve the full list of Avalara-supported subscription (ServiceTypes)
@@ -7047,23 +7042,23 @@
       Returns the full list of Avalara-supported subscription types.
       This API is intended to be useful for identifying which features you have added to your account.
       You may always contact Avalara's sales department for information on available products or services.
       You cannot change your subscriptions/service directly through the API.
       ### Security Policies
       * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
-      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
+      :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* taxTypeGroupIdSK
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_service_types(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/servicetypes/servicetypes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Reset a user's password programmatically
@@ -7080,15 +7075,15 @@
       :param userId [int] The unique ID of the user whose password will be changed
       :param isUndoMigrateRequest [boolean] If user's password was migrated to AI, undo this.
       :param model [SetPasswordModel] The new password for this user
       :return string
     """
     def reset_password(self, userId, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/passwords/{}/reset'.format(self.base_url, userId),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single account
@@ -7101,15 +7096,15 @@
     
       :param id_ [int] The ID of the account you wish to update.
       :param model [AccountModel] The account object you wish to update.
       :return AccountModel
     """
     def update_account(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/accounts/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single notification.
@@ -7127,15 +7122,15 @@
     
       :param id_ [int] The id of the notification you wish to update.
       :param model [NotificationModel] The notification object you wish to update.
       :return NotificationModel
     """
     def update_notification(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/notifications/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update existing Avalara-supported subscription (ServiceTypes)
@@ -7150,15 +7145,15 @@
     
       :param id_ [int] The unique ID number of the existing subscription type object to replace.
       :param model [SubscriptionTypeModel] The subscription type object to update.
       :return SubscriptionTypeModel
     """
     def update_service_type(self, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/servicetypes/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single subscription
@@ -7176,15 +7171,15 @@
       :param accountId [int] The ID of the account that this subscription belongs to.
       :param id_ [int] The ID of the subscription you wish to update
       :param model [SubscriptionModel] The subscription you wish to update.
       :return SubscriptionModel
     """
     def update_subscription(self, accountId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/accounts/{}/subscriptions/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Download a report
@@ -7203,15 +7198,15 @@
       * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param id_ [int] The unique ID number of this report
       :return String
     """
     def download_report(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/reports/{}/attachment'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single report
@@ -7226,15 +7221,15 @@
       This API call returns information about any report type.
     
       :param id_ [int] The unique ID number of the report to retrieve
       :return ReportModel
     """
     def get_report(self, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/reports/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Initiate an ExportDocumentLine report task
@@ -7258,15 +7253,15 @@
     
       :param companyId [int] The unique ID number of the company to report on.
       :param model [ExportDocumentLineModel] Options that may be configured to customize the report.
       :return ReportModel
     """
     def initiate_export_document_line_report(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/reports/exportdocumentline/initiate'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all report tasks for account
@@ -7286,15 +7281,15 @@
       :param pageKey [string] Provide a page key to retrieve the next page of results.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :return FetchResult
     """
     def list_reports(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/reports'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new setting
@@ -7315,15 +7310,15 @@
     
       :param companyId [int] The ID of the company that owns this setting.
       :param model [SettingModel] The setting you wish to create.
       :return SettingModel
     """
     def create_settings(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/settings'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single setting
@@ -7341,15 +7336,15 @@
     
       :param companyId [int] The ID of the company that owns this setting.
       :param id_ [int] The ID of the setting you wish to delete.
       :return ErrorDetail
     """
     def delete_setting(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/settings/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single setting
@@ -7359,23 +7354,23 @@
       about a company. Your integration or connector could use this data storage to keep track of
       preference information, reminders, or any other storage that would need to persist even if
       the customer uninstalls your application.
       A setting can refer to any type of data you need to remember about this company object.
       When creating this object, you may define your own `set`, `name`, and `value` parameters.
       To define your own values, please choose a `set` name that begins with `X-` to indicate an extension.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param companyId [int] The ID of the company that owns this setting
       :param id_ [int] The primary key of this setting
       :return SettingModel
     """
     def get_setting(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/settings/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all settings for this company
@@ -7387,27 +7382,27 @@
       the customer uninstalls your application.
       A setting can refer to any type of data you need to remember about this company object.
       When creating this object, you may define your own `set`, `name`, and `value` parameters.
       To define your own values, please choose a `set` name that begins with `X-` to indicate an extension.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param companyId [int] The ID of the company that owns these settings
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* modifiedDate, ModifiedUserId
       :param include [string] A comma separated list of additional data to retrieve.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_settings_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/settings'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all settings
@@ -7419,26 +7414,26 @@
       the customer uninstalls your application.
       A setting can refer to any type of data you need to remember about this company object.
       When creating this object, you may define your own `set`, `name`, and `value` parameters.
       To define your own values, please choose a `set` name that begins with `X-` to indicate an extension.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* modifiedDate, ModifiedUserId
       :param include [string] A comma separated list of additional data to retrieve.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_settings(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/settings'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single setting
@@ -7459,15 +7454,15 @@
       :param companyId [int] The ID of the company that this setting belongs to.
       :param id_ [int] The ID of the setting you wish to update
       :param model [SettingModel] The setting you wish to update.
       :return SettingModel
     """
     def update_setting(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/settings/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single subscription
@@ -7480,15 +7475,15 @@
     
       :param accountId [int] The ID of the account that owns this subscription
       :param id_ [int] The primary key of this subscription
       :return SubscriptionModel
     """
     def get_subscription(self, accountId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/subscriptions/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve subscriptions for this account
@@ -7506,15 +7501,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_subscriptions_by_account(self, accountId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/subscriptions'.format(self.base_url, accountId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all subscriptions
@@ -7531,15 +7526,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_subscriptions(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/subscriptions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new tax code
@@ -7554,15 +7549,15 @@
     
       :param companyId [int] The ID of the company that owns this tax code.
       :param model [TaxCodeModel] The tax code you wish to create.
       :return TaxCodeModel
     """
     def create_tax_codes(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/taxcodes'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single tax code
@@ -7573,38 +7568,38 @@
     
       :param companyId [int] The ID of the company that owns this tax code.
       :param id_ [int] The ID of the tax code you wish to delete.
       :return ErrorDetail
     """
     def delete_tax_code(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/taxcodes/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single tax code
     
     Get the taxcode object identified by this URL.
       A 'TaxCode' represents a uniquely identified type of product, good, or service.
       Avalara supports correct tax rates and taxability rules for all TaxCodes in all supported jurisdictions.
       If you identify your products by tax code in your 'Create Transacion' API calls, Avalara will correctly calculate tax rates and
       taxability rules for this product in all supported jurisdictions.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param companyId [int] The ID of the company that owns this tax code
       :param id_ [int] The primary key of this tax code
       :return TaxCodeModel
     """
     def get_tax_code(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/taxcodes/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve tax codes for this company
@@ -7613,27 +7608,27 @@
       A 'TaxCode' represents a uniquely identified type of product, good, or service.
       Avalara supports correct tax rates and taxability rules for all TaxCodes in all supported jurisdictions.
       If you identify your products by tax code in your 'Create Transacion' API calls, Avalara will correctly calculate tax rates and
       taxability rules for this product in all supported jurisdictions.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param companyId [int] The ID of the company that owns these tax codes
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
       :param include [string] A comma separated list of additional data to retrieve.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_codes_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/taxcodes'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all tax codes
@@ -7642,26 +7637,26 @@
       A 'TaxCode' represents a uniquely identified type of product, good, or service.
       Avalara supports correct tax rates and taxability rules for all TaxCodes in all supported jurisdictions.
       If you identify your products by tax code in your 'Create Transacion' API calls, Avalara will correctly calculate tax rates and
       taxability rules for this product in all supported jurisdictions.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, CSPAdmin, CSPTester, ECMAccountUser, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser.
     
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).
       :param include [string] A comma separated list of additional data to retrieve.
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_tax_codes(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/taxcodes'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single tax code
@@ -7679,15 +7674,15 @@
       :param companyId [int] The ID of the company that this tax code belongs to.
       :param id_ [int] The ID of the tax code you wish to update
       :param model [TaxCodeModel] The tax code you wish to update.
       :return TaxCodeModel
     """
     def update_tax_code(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/taxcodes/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Build a multi-location tax content file
@@ -7706,23 +7701,23 @@
       then use `CreateItems()` to create an item that uses the custom tax code.
       This data file can be customized for specific partner devices and usage conditions.
       The result of this API is the file you requested in the format you requested using the `responseType` field.
       This API builds the file on demand, and is limited to files with no more than 7500 scenarios. To build a tax content
       file for a single location at a time, please use `BuildTaxContentFileForLocation`.
       NOTE: This API does not work for Tennessee tax holiday scenarios.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Required* (all): AvaTaxPro.
     
       :param model [PointOfSaleDataRequestModel] Parameters about the desired file format and report format, specifying which company, locations and TaxCodes to include.
       :return String
     """
     def build_tax_content_file(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/pointofsaledata/build'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Build a tax content file for a single location
@@ -7741,28 +7736,28 @@
       then use `CreateItems()` to create an item that uses the custom tax code.
       This data file can be customized for specific partner devices and usage conditions.
       The result of this API is the file you requested in the format you requested using the `responseType` field.
       This API builds the file on demand, and is limited to files with no more than 7500 scenarios. To build a tax content
       file for a multiple locations in a single file, please use `BuildTaxContentFile`.
       NOTE: This API does not work for Tennessee tax holiday scenarios.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Required* (all): AvaTaxPro.
     
       :param companyId [int] The ID number of the company that owns this location.
       :param id_ [int] The ID number of the location to retrieve point-of-sale data.
       :param date [datetime] The date for which point-of-sale data would be calculated (today by default)
       :param format [PointOfSaleFileType] The format of the file (JSON by default) (See PointOfSaleFileType::* for a list of allowable values)
       :param partnerId [PointOfSalePartnerId] If specified, requests a custom partner-formatted version of the file. (See PointOfSalePartnerId::* for a list of allowable values)
       :param includeJurisCodes [boolean] When true, the file will include jurisdiction codes in the result.
       :return String
     """
     def build_tax_content_file_for_location(self, companyId, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/locations/{}/pointofsaledata'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Download a file listing tax rates by postal code
@@ -7797,23 +7792,23 @@
       * CITY_USE_TAX - The city component of the use tax rate.
       * TOTAL_SALES_TAX - The total tax rate for sales tax for this postal code. This value may not equal the sum of the state/county/city due to special tax jurisdiction rules.
       * TOTAL_USE_TAX - The total tax rate for use tax for this postal code. This value may not equal the sum of the state/county/city due to special tax jurisdiction rules.
       * TAX_SHIPPING_ALONE - This column contains 'Y' if shipping is taxable.
       * TAX_SHIPPING_AND_HANDLING_TOGETHER - This column contains 'Y' if shipping and handling are taxable when sent together.
       For more detailed tax content, please use the `BuildTaxContentFile` API which allows usage of exact items and exact locations.
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param date [datetime] The date for which point-of-sale data would be calculated (today by default). Example input: 2016-12-31
       :param region [string] A two character region code which limits results to a specific region.
       :return String
     """
     def download_tax_rates_by_zip_code(self, date, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/taxratesbyzipcode/download/{}'.format(self.base_url, date),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Sales tax rates for a specified address
@@ -7842,15 +7837,15 @@
       :param region [string] Name or ISO 3166 code identifying the region within the country.     This field supports many different region identifiers:   * Two and three character ISO 3166 region codes   * Fully spelled out names of the region in ISO supported languages   * Common alternative spellings for many regions     For a full list of all supported codes and names, please see the Definitions API `ListRegions`.
       :param postalCode [string] The postal code of the location.
       :param country [string] Name or ISO 3166 code identifying the country.     This field supports many different country identifiers:   * Two character ISO 3166 codes   * Three character ISO 3166 codes   * Fully spelled out names of the country in ISO supported languages   * Common alternative spellings for many countries     For a full list of all supported codes and names, please see the Definitions API `ListCountries`.
       :return TaxRateModel
     """
     def tax_rates_by_address(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/taxrates/byaddress'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Sales tax rates for a specified country and postal code. This API is only available for US postal codes.
@@ -7875,15 +7870,15 @@
     
       :param country [string] Name or ISO 3166 code identifying the country.     This field supports many different country identifiers:   * Two character ISO 3166 codes   * Three character ISO 3166 codes   * Fully spelled out names of the country in ISO supported languages   * Common alternative spellings for many countries     For a full list of all supported codes and names, please see the Definitions API `ListCountries`.
       :param postalCode [string] The postal code of the location.
       :return TaxRateModel
     """
     def tax_rates_by_postal_code(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/taxrates/bypostalcode'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new tax rule
@@ -7903,15 +7898,15 @@
     
       :param companyId [int] The ID of the company that owns this tax rule.
       :param model [TaxRuleModel] The tax rule you wish to create.
       :return TaxRuleModel
     """
     def create_tax_rules(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/taxrules'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single tax rule
@@ -7931,15 +7926,15 @@
     
       :param companyId [int] The ID of the company that owns this tax rule.
       :param id_ [int] The ID of the tax rule you wish to delete.
       :return ErrorDetail
     """
     def delete_tax_rule(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/taxrules/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single tax rule
@@ -7959,15 +7954,15 @@
     
       :param companyId [int] The ID of the company that owns this tax rule
       :param id_ [int] The primary key of this tax rule
       :return TaxRuleModel
     """
     def get_tax_rule(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/taxrules/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve tax rules for this company
@@ -7993,15 +7988,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_tax_rules(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/taxrules'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all tax rules
@@ -8026,15 +8021,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_tax_rules(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/taxrules'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single tax rule
@@ -8055,15 +8050,15 @@
       :param companyId [int] The ID of the company that this tax rule belongs to.
       :param id_ [int] The ID of the tax rule you wish to update
       :param model [TaxRuleModel] The tax rule you wish to update.
       :return TaxRuleModel
     """
     def update_tax_rule(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/taxrules/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Add lines to an existing unlocked transaction
@@ -8090,15 +8085,15 @@
     
       :param include [string] Specifies objects to include in the response after transaction is created
       :param model [AddTransactionLineModel] information about the transaction and lines to be added
       :return TransactionModel
     """
     def add_lines(self, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/transactions/lines/add'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Correct a previously created transaction
@@ -8135,15 +8130,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to adjust. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [AdjustTransactionModel] The adjustment you wish to make
       :return TransactionModel
     """
     def adjust_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/adjust'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get audit information about a transaction
@@ -8172,15 +8167,15 @@
     
       :param companyCode [string] The code identifying the company that owns this transaction
       :param transactionCode [string] The code identifying the transaction
       :return AuditTransactionModel
     """
     def audit_transaction(self, companyCode, transactionCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/transactions/{}/audit'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Get audit information about a transaction
@@ -8210,15 +8205,15 @@
       :param companyCode [string] The code identifying the company that owns this transaction
       :param transactionCode [string] The code identifying the transaction
       :param documentType [DocumentType] The document type of the original transaction (See DocumentType::* for a list of allowable values)
       :return AuditTransactionModel
     """
     def audit_transaction_with_type(self, companyCode, transactionCode, documentType):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/transactions/{}/types/{}/audit'.format(self.base_url, companyCode, transactionCode, documentType),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Lock a set of documents
@@ -8233,15 +8228,15 @@
       * This API depends on the following active services:*Returns* (at least one of): Mrs, MRSComplianceManager, AvaTaxCsp.*Firm Managed* (for accounts managed by a firm): ARA, ARAManaged.
     
       :param model [BulkLockTransactionModel] bulk lock request
       :return BulkLockTransactionResult
     """
     def bulk_lock_transaction(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/lock'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Change a transaction's code
@@ -8277,15 +8272,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to change document code. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [ChangeTransactionCodeModel] The code change request you wish to execute
       :return TransactionModel
     """
     def change_transaction_code(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/changecode'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Commit a transaction for reporting
@@ -8319,15 +8314,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to commit. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [CommitTransactionModel] The commit request you wish to execute
       :return TransactionModel
     """
     def commit_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/commit'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create or adjust a transaction
@@ -8363,15 +8358,15 @@
     
       :param include [string] Specifies objects to include in the response after transaction is created
       :param model [CreateOrAdjustTransactionModel] The transaction you wish to create or adjust
       :return TransactionModel
     """
     def create_or_adjust_transaction(self, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/createoradjust'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new transaction
@@ -8412,15 +8407,15 @@
     
       :param include [string] Specifies objects to include in the response after transaction is created
       :param model [CreateTransactionModel] The transaction you wish to create
       :return TransactionModel
     """
     def create_transaction(self, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/transactions/create'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Remove lines from an existing unlocked transaction
@@ -8444,15 +8439,15 @@
     
       :param include [string] Specifies objects to include in the response after transaction is created
       :param model [RemoveTransactionLineModel] information about the transaction and lines to be removed
       :return TransactionModel
     """
     def delete_lines(self, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/transactions/lines/delete'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Fetches the Variance data generated for all the transactions done by Company.
@@ -8462,15 +8457,15 @@
       * This API depends on the following active services:*Required* (all): AvaTaxPro, BasicReturns.
     
       :param companyCode [string] 
       :return VarianceResponseModel
     """
     def get_all_variance_report_by_company_code(self, companyCode):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/AllVariance'.format(self.base_url, companyCode),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single transaction by code
@@ -8503,15 +8498,15 @@
       :param transactionCode [string] The transaction code to retrieve
       :param documentType [DocumentType] (Optional): The document type of the transaction to retrieve (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :return TransactionModel
     """
     def get_transaction_by_code(self, companyCode, transactionCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/transactions/{}'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single transaction by code
@@ -8532,15 +8527,15 @@
       :param transactionCode [string] The transaction code to retrieve
       :param documentType [DocumentType] The transaction type to retrieve (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :return TransactionModel
     """
     def get_transaction_by_code_and_type(self, companyCode, transactionCode, documentType, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/transactions/{}/types/{}'.format(self.base_url, companyCode, transactionCode, documentType),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single transaction by ID
@@ -8563,15 +8558,15 @@
     
       :param id_ [int] The unique ID number of the transaction to retrieve
       :param include [string] Specifies objects to include in this fetch call
       :return TransactionModel
     """
     def get_transaction_by_id(self, id_, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/transactions/{}'.format(self.base_url, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Fetches the Variance data generated for particular Company by transaction ID
@@ -8582,15 +8577,15 @@
     
       :param companyCode [string] 
       :param transactionId [string] 
       :return VarianceResponseModel
     """
     def get_variance_report_by_company_code_by_transaction_id(self, companyCode, transactionId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/transactions/{}/variance'.format(self.base_url, companyCode, transactionId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all transactions
@@ -8628,15 +8623,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_transactions_by_company(self, companyCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/transactions'.format(self.base_url, companyCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Lock a single transaction
@@ -8672,15 +8667,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to lock. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [LockTransactionModel] The lock request you wish to execute
       :return TransactionModel
     """
     def lock_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/lock'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a refund for a transaction
@@ -8726,15 +8721,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to refund. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param useTaxDateOverride [boolean] (Optional): If set to true, processes refund using taxDateOverride rather than taxAmountOverride (Note: taxAmountOverride is not allowed for SST states).
       :param model [RefundTransactionModel] Information about the refund to create
       :return TransactionModel
     """
     def refund_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/refund'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Perform multiple actions on a transaction
@@ -8768,15 +8763,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to settle. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [SettleTransactionModel] The data from an external system to reconcile against AvaTax
       :return TransactionModel
     """
     def settle_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/settle'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Uncommit a transaction for reporting
@@ -8807,15 +8802,15 @@
       :param transactionCode [string] The transaction code to Uncommit
       :param documentType [DocumentType] (Optional): The document type of the transaction to Uncommit. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :return TransactionModel
     """
     def uncommit_transaction(self, companyCode, transactionCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/uncommit'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Unvoids a transaction
@@ -8844,15 +8839,15 @@
       :param transactionCode [string] The transaction code to commit
       :param documentType [DocumentType] (Optional): The document type of the transaction to commit. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :return TransactionModel
     """
     def unvoid_transaction(self, companyCode, transactionCode, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/unvoid'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Generates the Variance report which will capture the difference between "Tax Calculated by Avalara" Vs "Actual Tax" paid at custom clearance at line / header level.
@@ -8863,15 +8858,15 @@
     
       :param companyCode [string] 
       :param model [VarianceRequestModel] 
       :return VarianceResponseModel
     """
     def variance_report(self, companyCode, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/variance'.format(self.base_url, companyCode),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Verify a transaction
@@ -8905,15 +8900,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to verify. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [VerifyTransactionModel] The data from an external system to reconcile against AvaTax
       :return TransactionModel
     """
     def verify_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/verify'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Void a transaction
@@ -8948,15 +8943,15 @@
       :param documentType [DocumentType] (Optional): The document type of the transaction to void. If not provided, the default is SalesInvoice. (See DocumentType::* for a list of allowable values)
       :param include [string] Specifies objects to include in this fetch call
       :param model [VoidTransactionModel] The void request you wish to execute. To void a transaction the code must be set to 'DocVoided'
       :return TransactionModel
     """
     def void_transaction(self, companyCode, transactionCode, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/transactions/{}/void'.format(self.base_url, companyCode, transactionCode),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create a new UPC
@@ -8969,15 +8964,15 @@
     
       :param companyId [int] The ID of the company that owns this UPC.
       :param model [UPCModel] The UPC you wish to create.
       :return UPCModel
     """
     def create_u_p_cs(self, companyId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/upcs'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single UPC
@@ -8989,15 +8984,15 @@
     
       :param companyId [int] The ID of the company that owns this UPC.
       :param id_ [int] The ID of the UPC you wish to delete.
       :return ErrorDetail
     """
     def delete_u_p_c(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/upcs/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single UPC
@@ -9010,15 +9005,15 @@
     
       :param companyId [int] The ID of the company that owns this UPC
       :param id_ [int] The primary key of this UPC
       :return UPCModel
     """
     def get_u_p_c(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/upcs/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve UPCs for this company
@@ -9037,15 +9032,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_u_p_cs_by_company(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/upcs'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all UPCs
@@ -9063,15 +9058,15 @@
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_u_p_cs(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/upcs'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single UPC
@@ -9087,15 +9082,15 @@
       :param companyId [int] The ID of the company that this UPC belongs to.
       :param id_ [int] The ID of the UPC you wish to update
       :param model [UPCModel] The UPC you wish to update.
       :return UPCModel
     """
     def update_u_p_c(self, companyId, id_, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/companies/{}/upcs/{}'.format(self.base_url, companyId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a User Defined Field by User Defined Field id for a company.
@@ -9107,35 +9102,35 @@
     
       :param companyId [int] The id of the company the User Defined Field belongs to.
       :param id_ [int] The id of the User Defined Field you wish to delete.
       :return ErrorDetail
     """
     def delete_user_defined_field(self, companyId, id_):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/companies/{}/userdefinedfields/{}'.format(self.base_url, companyId, accountId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     
     
     ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
       * This API depends on the following active services:*Required* (all): AvaTaxPro, BasicReturns.
     
       :param companyId [int] 
       :param udfType [UserDefinedFieldType] Document or Line level UDF (See UserDefinedFieldType::* for a list of allowable values)
       :param allowDefaults [boolean] If true this will add defaulted UDFs to the list that are not named yet
       :return FetchResult
     """
     def list_user_defined_fields_by_company_id(self, companyId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/companies/{}/userdefinedfields'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a User Defined Field identified by id for a company
@@ -9148,15 +9143,15 @@
       :param companyId [int] The id of the company the user defined field belongs to.
       :param id [int] 
       :param model [CompanyUserDefinedFieldModel] 
       :return CompanyUserDefinedFieldModel
     """
     def update_user_defined_field(self, companyId, model, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/companies/{}/userdefinedfields'.format(self.base_url, companyId),
                                auth=self.auth, headers=self.client_header, params=include, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Change Password
@@ -9170,15 +9165,15 @@
       * This API requires one of the following user roles: AccountAdmin, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPTester, FirmAdmin, FirmUser, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param model [PasswordChangeModel] An object containing your current password and the new password.
       :return string
     """
     def change_password(self, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/passwords'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Create new users
@@ -9194,15 +9189,15 @@
     
       :param accountId [int] The unique ID number of the account where these users will be created.
       :param model [UserModel] The user or array of users you wish to create.
       :return UserModel
     """
     def create_users(self, accountId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.post('{}/api/v2/accounts/{}/users'.format(self.base_url, accountId),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Delete a single user
@@ -9216,38 +9211,38 @@
     
       :param id_ [int] The ID of the user you wish to delete.
       :param accountId [int] The accountID of the user you wish to delete.
       :return ErrorDetail
     """
     def delete_user(self, id_, accountId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.delete('{}/api/v2/accounts/{}/users/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve a single user
     
     Get the user object identified by this URL.
       A user represents one person with access privileges to make API calls and work with a specific account.
        You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * FetchDeleted
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the user to retrieve.
       :param accountId [int] The accountID of the user you wish to get.
       :param include [string] Optional fetch commands.
       :return UserModel
     """
     def get_user(self, id_, accountId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/users/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all entitlements for a single user
@@ -9262,23 +9257,23 @@
        credentials for this user.
       * If the 'accessLevel' field within entitlements is 'None', the call will fail.
       * If the 'accessLevel' field within entitlements is 'SingleCompany' or 'SingleAccount', the call will fail if the companies
        table does not contain the ID number 12345.
       * If the 'permissions' array within entitlements does not contain 'AccountSvc.CompanySave', the call will fail.
       For a full list of defined permissions, please use '/api/v2/definitions/permissions' .
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param id_ [int] The ID of the user to retrieve.
       :param accountId [int] The accountID of the user you wish to get.
       :return UserEntitlementModel
     """
     def get_user_entitlements(self, id_, accountId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/users/{}/entitlements'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve users for this account
@@ -9288,27 +9283,27 @@
       When an API is called using a legacy AvaTax License Key, the API log entry is recorded as being performed by a special user attached to that license key.
       By default, this API will not return a listing of license key users. Users with registrar-level security may call this API to list license key users.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * FetchDeleted
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param accountId [int] The accountID of the user you wish to list.
       :param include [string] Optional fetch commands.
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* SuppressNewUserEmail
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def list_users_by_account(self, accountId, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/accounts/{}/users'.format(self.base_url, accountId),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Retrieve all users
@@ -9319,26 +9314,26 @@
       When an API is called using a legacy AvaTax License Key, the API log entry is recorded as being performed by a special user attached to that license key.
       By default, this API will not return a listing of license key users. Users with registrar-level security may call this API to list license key users.
       Search for specific objects using the criteria in the `$filter` parameter; full documentation is available on [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/) .
       Paginate your results using the `$top`, `$skip`, and `$orderby` parameters.
       You may specify one or more of the following values in the `$include` parameter to fetch additional nested data, using commas to separate multiple values:
       * FetchDeleted
       ### Security Policies
-      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
+      * This API requires one of the following user roles: AccountAdmin, AccountOperator, AccountUser, BatchServiceAdmin, CompanyAdmin, CompanyUser, Compliance Root User, ComplianceAdmin, ComplianceUser, CSPAdmin, CSPTester, ECMAccountUser, ECMCompanyUser, FirmAdmin, FirmUser, ProStoresOperator, Registrar, SiteAdmin, SSTAdmin, SystemAdmin, SystemOperator, TechnicalSupportAdmin, TechnicalSupportUser, TreasuryAdmin, TreasuryUser.
     
       :param include [string] Optional fetch commands.
       :param filter [string] A filter statement to identify specific records to retrieve. For more information on filtering, see [Filtering in REST](http://developer.avalara.com/avatax/filtering-in-rest/).<br />*Not filterable:* SuppressNewUserEmail
       :param top [int] If nonzero, return no more than this number of results. Used with `$skip` to provide pagination for large datasets. Unless otherwise specified, the maximum number of records that can be returned from an API call is 1,000 records.
       :param skip [int] If nonzero, skip this number of results before returning data. Used with `$top` to provide pagination for large datasets.
       :param orderBy [string] A comma separated list of sort statements in the format `(fieldname) [ASC|DESC]`, for example `id ASC`.
       :return FetchResult
     """
     def query_users(self, include=None):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/users'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=include, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Update a single user
@@ -9353,15 +9348,15 @@
       :param id_ [int] The ID of the user you wish to update.
       :param accountId [int] The accountID of the user you wish to update.
       :param model [UserModel] The user object you wish to update.
       :return UserModel
     """
     def update_user(self, id_, accountId, model):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.put('{}/api/v2/accounts/{}/users/{}'.format(self.base_url, accountId, id_),
                                auth=self.auth, headers=self.client_header, json=model, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Checks if the current user is subscribed to a specific service
@@ -9374,15 +9369,15 @@
       specific features of AvaTax.
     
       :param serviceTypeId [string] The service to check
       :return SubscriptionModel
     """
     def get_my_subscription(self, serviceTypeId):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/utilities/subscriptions/{}'.format(self.base_url, serviceTypeId),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     List all services to which the current user is subscribed
@@ -9394,15 +9389,15 @@
       or subscription to provide useful information to the current user as to whether they are entitled to use
       specific features of AvaTax.
     
       :return FetchResult
     """
     def list_my_subscriptions(self):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/utilities/subscriptions'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxClient
     
     Tests connectivity and version of the service
@@ -9423,15 +9418,15 @@
       ### Security Policies
       * This API may be called without providing authentication credentials.
     
       :return PingResultModel
     """
     def ping(self):
         if ('X-Avalara-Client' in self.client_header): 
-            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.3.1")   
+            self.client_header['X-Avalara-Client']=self.client_id.replace("API_VERSION","23.4.1")   
         return requests.get('{}/api/v2/utilities/ping'.format(self.base_url),
                                auth=self.auth, headers=self.client_header, params=None, 
                                timeout=self.timeout_limit if self.timeout_limit else 1200)
     r"""
     Swagger Name: AvaTaxBeverageClient
     
     Fetches a previously stored age verification response.
```

### Comparing `Avalara-23.3.1/src/avalara/transaction_builder.py` & `Avalara-23.4.1/src/avalara/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `Avalara-23.3.1/src/avalara/transaction_builder_methods.py` & `Avalara-23.4.1/src/avalara/transaction_builder_methods.py`

 * *Files identical despite different names*

