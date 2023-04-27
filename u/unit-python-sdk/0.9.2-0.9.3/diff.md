# Comparing `tmp/unit-python-sdk-0.9.2.tar.gz` & `tmp/unit-python-sdk-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit-python-sdk-0.9.2.tar", last modified: Tue Mar  1 13:16:01 2022, max compression
+gzip compressed data, was "dist/unit-python-sdk-0.9.3.tar", last modified: Wed Mar  9 08:23:57 2022, max compression
```

## Comparing `unit-python-sdk-0.9.2.tar` & `unit-python-sdk-0.9.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 elroie     (501) staff       (20)        0 2022-03-01 13:16:01.254168 unit-python-sdk-0.9.2/
--rw-r--r--   0 elroie     (501) staff       (20)      800 2022-03-01 13:16:01.254295 unit-python-sdk-0.9.2/PKG-INFO
--rw-r--r--   0 elroie     (501) staff       (20)       39 2021-11-03 13:43:10.538771 unit-python-sdk-0.9.2/setup.cfg
--rw-r--r--   0 elroie     (501) staff       (20)      995 2022-03-01 13:07:49.892086 unit-python-sdk-0.9.2/setup.py
-drwxr-xr-x   0 elroie     (501) staff       (20)        0 2022-03-01 13:16:01.239706 unit-python-sdk-0.9.2/unit/
--rw-r--r--   0 elroie     (501) staff       (20)     2654 2021-12-15 13:23:28.756821 unit-python-sdk-0.9.2/unit/__init__.py
-drwxr-xr-x   0 elroie     (501) staff       (20)        0 2022-03-01 13:16:01.246752 unit-python-sdk-0.9.2/unit/api/
--rw-r--r--   0 elroie     (501) staff       (20)        0 2021-11-03 15:05:14.032619 unit-python-sdk-0.9.2/unit/api/__init__.py
--rw-r--r--   0 elroie     (501) staff       (20)      804 2022-03-01 13:05:54.342936 unit-python-sdk-0.9.2/unit/api/account_end_of_day_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     3621 2022-03-01 13:05:54.343334 unit-python-sdk-0.9.2/unit/api/account_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1501 2021-12-15 13:23:28.757563 unit-python-sdk-0.9.2/unit/api/api_token_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1820 2022-03-01 13:05:54.343676 unit-python-sdk-0.9.2/unit/api/applicationForm_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     2882 2022-01-19 16:26:22.804214 unit-python-sdk-0.9.2/unit/api/application_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1317 2022-03-01 13:05:54.343971 unit-python-sdk-0.9.2/unit/api/atmLocation_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     2390 2022-03-01 13:05:54.344286 unit-python-sdk-0.9.2/unit/api/authorization_request_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1331 2022-03-01 13:05:54.344682 unit-python-sdk-0.9.2/unit/api/authorization_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     2002 2021-12-19 12:27:47.002234 unit-python-sdk-0.9.2/unit/api/base_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)      809 2021-12-15 13:23:28.760244 unit-python-sdk-0.9.2/unit/api/bill_pay_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     5571 2022-03-01 13:05:54.345044 unit-python-sdk-0.9.2/unit/api/card_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     2934 2022-03-01 13:05:54.345435 unit-python-sdk-0.9.2/unit/api/counterparty_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1338 2021-11-03 15:05:14.035414 unit-python-sdk-0.9.2/unit/api/customerToken_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1795 2022-03-01 13:05:54.345983 unit-python-sdk-0.9.2/unit/api/customer_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1410 2022-03-01 13:05:54.346229 unit-python-sdk-0.9.2/unit/api/event_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)      697 2021-11-24 09:28:43.225446 unit-python-sdk-0.9.2/unit/api/fee_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)      705 2021-11-24 09:28:43.225634 unit-python-sdk-0.9.2/unit/api/institution_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     2224 2022-03-01 13:05:54.346407 unit-python-sdk-0.9.2/unit/api/payment_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)      889 2021-11-24 09:28:43.226111 unit-python-sdk-0.9.2/unit/api/returnAch_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1729 2022-03-01 13:05:54.346591 unit-python-sdk-0.9.2/unit/api/statement_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     1988 2022-03-01 13:05:54.346855 unit-python-sdk-0.9.2/unit/api/transaction_resource.py
--rw-r--r--   0 elroie     (501) staff       (20)     3250 2022-03-01 13:05:54.347143 unit-python-sdk-0.9.2/unit/api/webhook_resource.py
-drwxr-xr-x   0 elroie     (501) staff       (20)        0 2022-03-01 13:16:01.253366 unit-python-sdk-0.9.2/unit/models/
--rw-r--r--   0 elroie     (501) staff       (20)     8988 2022-03-01 13:05:54.347801 unit-python-sdk-0.9.2/unit/models/__init__.py
--rw-r--r--   0 elroie     (501) staff       (20)     8965 2022-03-01 13:05:54.348199 unit-python-sdk-0.9.2/unit/models/account.py
--rw-r--r--   0 elroie     (501) staff       (20)     1620 2022-03-01 13:05:54.348540 unit-python-sdk-0.9.2/unit/models/account_end_of_day.py
--rw-r--r--   0 elroie     (501) staff       (20)     1687 2021-12-15 13:23:28.765181 unit-python-sdk-0.9.2/unit/models/api_token.py
--rw-r--r--   0 elroie     (501) staff       (20)    10792 2022-03-01 13:05:54.348911 unit-python-sdk-0.9.2/unit/models/application.py
--rw-r--r--   0 elroie     (501) staff       (20)     4275 2022-03-01 13:05:54.349275 unit-python-sdk-0.9.2/unit/models/applicationForm.py
--rw-r--r--   0 elroie     (501) staff       (20)     1350 2021-12-15 13:20:58.794064 unit-python-sdk-0.9.2/unit/models/atm_location.py
--rw-r--r--   0 elroie     (501) staff       (20)     3261 2022-03-01 13:05:54.349579 unit-python-sdk-0.9.2/unit/models/authorization.py
--rw-r--r--   0 elroie     (501) staff       (20)     4417 2022-03-01 13:05:54.349927 unit-python-sdk-0.9.2/unit/models/authorization_request.py
--rw-r--r--   0 elroie     (501) staff       (20)      568 2021-12-15 13:20:58.794982 unit-python-sdk-0.9.2/unit/models/bill_pay.py
--rw-r--r--   0 elroie     (501) staff       (20)    18105 2022-03-01 13:05:54.350335 unit-python-sdk-0.9.2/unit/models/card.py
--rw-r--r--   0 elroie     (501) staff       (20)    17505 2022-03-01 13:05:54.350751 unit-python-sdk-0.9.2/unit/models/codecs.py
--rw-r--r--   0 elroie     (501) staff       (20)     5100 2022-03-01 13:05:54.351129 unit-python-sdk-0.9.2/unit/models/counterparty.py
--rw-r--r--   0 elroie     (501) staff       (20)     6208 2022-03-01 13:05:54.351811 unit-python-sdk-0.9.2/unit/models/customer.py
--rw-r--r--   0 elroie     (501) staff       (20)     2863 2022-01-19 16:26:22.807044 unit-python-sdk-0.9.2/unit/models/customerToken.py
--rw-r--r--   0 elroie     (501) staff       (20)    19231 2022-03-01 13:05:54.352256 unit-python-sdk-0.9.2/unit/models/event.py
--rw-r--r--   0 elroie     (501) staff       (20)     1654 2021-12-15 13:23:28.768478 unit-python-sdk-0.9.2/unit/models/fee.py
--rw-r--r--   0 elroie     (501) staff       (20)      740 2021-12-15 13:20:58.797471 unit-python-sdk-0.9.2/unit/models/institution.py
--rw-r--r--   0 elroie     (501) staff       (20)    12767 2022-03-01 13:05:54.352649 unit-python-sdk-0.9.2/unit/models/payment.py
--rw-r--r--   0 elroie     (501) staff       (20)      763 2021-12-15 13:23:28.769135 unit-python-sdk-0.9.2/unit/models/returnAch.py
--rw-r--r--   0 elroie     (501) staff       (20)     1646 2022-03-01 13:05:54.352934 unit-python-sdk-0.9.2/unit/models/statement.py
--rw-r--r--   0 elroie     (501) staff       (20)    24184 2022-03-01 13:07:34.486018 unit-python-sdk-0.9.2/unit/models/transaction.py
--rw-r--r--   0 elroie     (501) staff       (20)     2843 2022-03-01 13:05:54.353833 unit-python-sdk-0.9.2/unit/models/webhook.py
-drwxr-xr-x   0 elroie     (501) staff       (20)        0 2022-03-01 13:16:01.254094 unit-python-sdk-0.9.2/unit/utils/
--rw-r--r--   0 elroie     (501) staff       (20)        0 2021-11-03 15:05:14.042071 unit-python-sdk-0.9.2/unit/utils/__init__.py
--rw-r--r--   0 elroie     (501) staff       (20)      241 2021-11-03 15:05:14.042368 unit-python-sdk-0.9.2/unit/utils/date_utils.py
+drwxr-xr-x   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:57.000000 unit-python-sdk-0.9.3/
+-rw-r--r--   0 asaf       (501) staff       (20)      800 2022-03-09 08:23:57.000000 unit-python-sdk-0.9.3/PKG-INFO
+drwxr-xr-x   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:57.000000 unit-python-sdk-0.9.3/unit/
+-rw-r--r--   0 asaf       (501) staff       (20)     2654 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/__init__.py
+drwxr-xr-x   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:57.000000 unit-python-sdk-0.9.3/unit/utils/
+-rw-r--r--   0 asaf       (501) staff       (20)      241 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/utils/date_utils.py
+-rw-r--r--   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/utils/__init__.py
+drwxr-xr-x   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:57.000000 unit-python-sdk-0.9.3/unit/models/
+-rw-r--r--   0 asaf       (501) staff       (20)     1620 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/account_end_of_day.py
+-rw-r--r--   0 asaf       (501) staff       (20)    19231 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/event.py
+-rw-r--r--   0 asaf       (501) staff       (20)      568 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/bill_pay.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1350 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/atm_location.py
+-rw-r--r--   0 asaf       (501) staff       (20)     4275 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/applicationForm.py
+-rw-r--r--   0 asaf       (501) staff       (20)      740 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/institution.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2863 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/customerToken.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2843 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/webhook.py
+-rw-r--r--   0 asaf       (501) staff       (20)     5100 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/counterparty.py
+-rw-r--r--   0 asaf       (501) staff       (20)    24184 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/transaction.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1646 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/statement.py
+-rw-r--r--   0 asaf       (501) staff       (20)    17505 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/codecs.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1687 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/api_token.py
+-rw-r--r--   0 asaf       (501) staff       (20)     8987 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/__init__.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1654 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/fee.py
+-rw-r--r--   0 asaf       (501) staff       (20)    18105 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/card.py
+-rw-r--r--   0 asaf       (501) staff       (20)    10792 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/application.py
+-rw-r--r--   0 asaf       (501) staff       (20)     3261 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/authorization.py
+-rw-r--r--   0 asaf       (501) staff       (20)     6208 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/customer.py
+-rw-r--r--   0 asaf       (501) staff       (20)      763 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/returnAch.py
+-rw-r--r--   0 asaf       (501) staff       (20)    12767 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/payment.py
+-rw-r--r--   0 asaf       (501) staff       (20)     4417 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/authorization_request.py
+-rw-r--r--   0 asaf       (501) staff       (20)     8965 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/models/account.py
+drwxr-xr-x   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:57.000000 unit-python-sdk-0.9.3/unit/api/
+-rw-r--r--   0 asaf       (501) staff       (20)      804 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/account_end_of_day_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2882 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/application_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1410 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/event_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1795 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/customer_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2002 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/base_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2224 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/payment_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)        0 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/__init__.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1338 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/customerToken_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1988 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/transaction_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1820 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/applicationForm_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)      705 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/institution_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)      809 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/bill_pay_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2390 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/authorization_request_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1317 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/atmLocation_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     3250 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/webhook_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     2934 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/counterparty_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1729 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/statement_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)      889 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/returnAch_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1501 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/api_token_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     3621 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/account_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     5571 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/card_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)     1331 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/authorization_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)      697 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/unit/api/fee_resource.py
+-rw-r--r--   0 asaf       (501) staff       (20)      995 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/setup.py
+-rw-r--r--   0 asaf       (501) staff       (20)       39 2022-03-09 08:23:36.000000 unit-python-sdk-0.9.3/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `unit-python-sdk-0.9.2/PKG-INFO` & `unit-python-sdk-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unit-python-sdk
-Version: 0.9.2
+Version: 0.9.3
 Summary: This library provides a python wrapper to http://unit.co API. See https://docs.unit.co/
 Home-page: https://github.com/unit-finance/unit-python-sdk
 Author: unit.co
 Author-email: dev@unit.co
 License: Mozilla Public License 2.0
 Download-URL: https://github.com/unit-finance/unit-python-sdk.git
 Description: UNKNOWN
```

### Comparing `unit-python-sdk-0.9.2/setup.py` & `unit-python-sdk-0.9.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='unit-python-sdk',
     packages=['unit', 'unit.api', 'unit.models', 'unit.utils'],
-    version='0.9.2',
+    version='0.9.3',
     license='Mozilla Public License 2.0',
     description='This library provides a python wrapper to http://unit.co API. See https://docs.unit.co/',
     author='unit.co',
     author_email='dev@unit.co',
     url='https://github.com/unit-finance/unit-python-sdk',
     download_url='https://github.com/unit-finance/unit-python-sdk.git',
     keywords=['unit', 'finance', 'banking',
```

### Comparing `unit-python-sdk-0.9.2/unit/__init__.py` & `unit-python-sdk-0.9.3/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/account_end_of_day_resource.py` & `unit-python-sdk-0.9.3/unit/api/account_end_of_day_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/account_resource.py` & `unit-python-sdk-0.9.3/unit/api/account_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/api_token_resource.py` & `unit-python-sdk-0.9.3/unit/api/api_token_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/applicationForm_resource.py` & `unit-python-sdk-0.9.3/unit/api/applicationForm_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/application_resource.py` & `unit-python-sdk-0.9.3/unit/api/application_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/atmLocation_resource.py` & `unit-python-sdk-0.9.3/unit/api/atmLocation_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/authorization_request_resource.py` & `unit-python-sdk-0.9.3/unit/api/authorization_request_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/authorization_resource.py` & `unit-python-sdk-0.9.3/unit/api/authorization_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/base_resource.py` & `unit-python-sdk-0.9.3/unit/api/base_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/bill_pay_resource.py` & `unit-python-sdk-0.9.3/unit/api/bill_pay_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/card_resource.py` & `unit-python-sdk-0.9.3/unit/api/card_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/counterparty_resource.py` & `unit-python-sdk-0.9.3/unit/api/counterparty_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/customerToken_resource.py` & `unit-python-sdk-0.9.3/unit/api/customerToken_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/customer_resource.py` & `unit-python-sdk-0.9.3/unit/api/customer_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/event_resource.py` & `unit-python-sdk-0.9.3/unit/api/event_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/fee_resource.py` & `unit-python-sdk-0.9.3/unit/api/fee_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/institution_resource.py` & `unit-python-sdk-0.9.3/unit/api/institution_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/payment_resource.py` & `unit-python-sdk-0.9.3/unit/api/payment_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/returnAch_resource.py` & `unit-python-sdk-0.9.3/unit/api/returnAch_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/statement_resource.py` & `unit-python-sdk-0.9.3/unit/api/statement_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/transaction_resource.py` & `unit-python-sdk-0.9.3/unit/api/transaction_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/api/webhook_resource.py` & `unit-python-sdk-0.9.3/unit/api/webhook_resource.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/__init__.py` & `unit-python-sdk-0.9.3/unit/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         self.state = state
         self.postal_code = postal_code
         self.country = country
 
     @staticmethod
     def from_json_api(data: Dict):
         return Address(data.get("street"), data.get("city"), data.get("state"),
-                data.get("postal_code"), data.get("country"), data.get("street2", None))
+                data.get("postalCode"), data.get("country"), data.get("street2", None))
 
 
 class Phone(object):
     def __init__(self, country_code: str, number: str):
         self.country_code = country_code
         self.number = number
```

### Comparing `unit-python-sdk-0.9.2/unit/models/account.py` & `unit-python-sdk-0.9.3/unit/models/account.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/account_end_of_day.py` & `unit-python-sdk-0.9.3/unit/models/account_end_of_day.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/api_token.py` & `unit-python-sdk-0.9.3/unit/models/api_token.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/application.py` & `unit-python-sdk-0.9.3/unit/models/application.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/applicationForm.py` & `unit-python-sdk-0.9.3/unit/models/applicationForm.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/atm_location.py` & `unit-python-sdk-0.9.3/unit/models/atm_location.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/authorization.py` & `unit-python-sdk-0.9.3/unit/models/authorization.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/authorization_request.py` & `unit-python-sdk-0.9.3/unit/models/authorization_request.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/bill_pay.py` & `unit-python-sdk-0.9.3/unit/models/bill_pay.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/card.py` & `unit-python-sdk-0.9.3/unit/models/card.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/codecs.py` & `unit-python-sdk-0.9.3/unit/models/codecs.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/counterparty.py` & `unit-python-sdk-0.9.3/unit/models/counterparty.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/customer.py` & `unit-python-sdk-0.9.3/unit/models/customer.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/customerToken.py` & `unit-python-sdk-0.9.3/unit/models/customerToken.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/event.py` & `unit-python-sdk-0.9.3/unit/models/event.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/fee.py` & `unit-python-sdk-0.9.3/unit/models/fee.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/institution.py` & `unit-python-sdk-0.9.3/unit/models/institution.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/payment.py` & `unit-python-sdk-0.9.3/unit/models/payment.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/returnAch.py` & `unit-python-sdk-0.9.3/unit/models/returnAch.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/statement.py` & `unit-python-sdk-0.9.3/unit/models/statement.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/transaction.py` & `unit-python-sdk-0.9.3/unit/models/transaction.py`

 * *Files identical despite different names*

### Comparing `unit-python-sdk-0.9.2/unit/models/webhook.py` & `unit-python-sdk-0.9.3/unit/models/webhook.py`

 * *Files identical despite different names*

