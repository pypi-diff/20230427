# Comparing `tmp/codat-sync-for-commerce-0.10.0.tar.gz` & `tmp/codat-sync-for-commerce-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-commerce-0.10.0.tar", last modified: Thu Apr 27 12:36:22 2023, max compression
+gzip compressed data, was "codat-sync-for-commerce-0.9.0.tar", last modified: Wed Apr 26 15:03:44 2023, max compression
```

## Comparing `codat-sync-for-commerce-0.10.0.tar` & `codat-sync-for-commerce-0.9.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.321572 codat-sync-for-commerce-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-27 12:36:22.321572 codat-sync-for-commerce-0.10.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3066 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:36:22.321572 codat-sync-for-commerce-0.10.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.305572 codat-sync-for-commerce-0.10.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.305572 codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-27 12:36:22.000000 codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-27 12:36:22.000000 codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:36:22.000000 codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 12:36:22.000000 codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 12:36:22.000000 codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.309572 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8903 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/company_management.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3852 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.309572 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.309572 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/create_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      920 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/create_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_integration_branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_sync_flow_url.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_visible_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1605 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/list_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1753 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/list_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1626 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/list_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/request_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1012 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/set_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/update_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.321572 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/accountoption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/brandingbutton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/brandingimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/brandinglogo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1727 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/configaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1341 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5396 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/createcompany.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2692 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/datatypefeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/daterange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/featurestate_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/featuretype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/fees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/feessupplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/groupinglevels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/groupingperiod.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/halref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/imagereference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3215 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/invoicelevelselection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      880 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/invoicestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1041 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/localization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/newpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/newtaxrates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/option.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2191 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/sales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/sourcetype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/supportedfeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      561 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/syncflowurl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3844 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/syncsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1432 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/synctolatestargs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/taxrateamount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/taxratemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/updateconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      612 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/visibleaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8928 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/sync_flow_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:22.321572 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-27 12:36:11.000000 codat-sync-for-commerce-0.10.0/src/codatsynccommerce/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3066 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.155307 codat-sync-for-commerce-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.155307 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8903 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/company_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3852 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      926 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      827 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_integration_branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_flow_url.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_visible_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1634 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/set_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1021 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/accountoption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1455 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingbutton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandinglogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5409 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/createcompany.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2694 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/datatypefeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2503 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/daterange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/featurestate_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/featuretype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/fees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/feessupplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupinglevels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupingperiod.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/halref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/imagereference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3226 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelevelselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/localization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1870 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newtaxrates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      764 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/option.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sourcetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/supportedfeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncflowurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/synctolatestargs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxrateamount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxratemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/updateconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/visibleaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8928 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync_flow_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/utils.py
```

### Comparing `codat-sync-for-commerce-0.10.0/PKG-INFO` & `codat-sync-for-commerce-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-commerce
-Version: 0.10.0
+Version: 0.9.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-commerce-0.10.0/README.md` & `codat-sync-for-commerce-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/setup.py` & `codat-sync-for-commerce-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-commerce",
-    version="0.10.0",
+    version="0.9.0",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/PKG-INFO` & `codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-commerce
-Version: 0.10.0
+Version: 0.9.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt` & `codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/company_management.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/company_management.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/integrations.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/integrations.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/__init__.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/create_company.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import company as shared_company
+from ..shared import localization as shared_localization
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateCompanyResponse:
+class GetConfigTextSyncFlowResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    company: Optional[shared_company.Company] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/create_connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,20 @@
 from ..shared import connection as shared_connection
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateConnectionRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
-    request_body: Optional[str] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[str] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class CreateConnectionResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import localization as shared_localization
+from ..shared import configuration as shared_configuration
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetConfigTextSyncFlowResponse:
+class GetConfigurationRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
 
+@dataclasses.dataclass
+class GetConfigurationResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/set_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,21 @@
 import dataclasses
 import requests as requests_http
 from ..shared import configuration as shared_configuration
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetConfigurationRequest:
+class SetConfigurationRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class GetConfigurationResponse:
+class SetConfigurationResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_integration_branding.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_integration_branding.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,19 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetIntegrationBrandingRequest:
     
     platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
-
-    r"""PlatformKey"""
+    r"""PlatformKey"""  
     
 
 @dataclasses.dataclass
 class GetIntegrationBrandingResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     branding: Optional[shared_branding.Branding] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_sync_flow_url.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import syncflowurl as shared_syncflowurl
+from ..shared import daterange as shared_daterange
+from ..shared import syncsummary as shared_syncsummary
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetSyncFlowURLRequest:
+class RequestSyncForDateRangeRequest:
     
-    accounting_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountingKey', 'style': 'simple', 'explode': False }})
-
-    r"""Accounting platform key"""
-    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})
-
-    r"""Commerce platform key"""
-    merchant_identifier: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'merchantIdentifier', 'style': 'form', 'explode': True }})
-
-    r"""Identifier for your merchant, can be the merchant name or Codat company id."""
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    date_range: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
-class GetSyncFlowURLResponse:
+class RequestSyncForDateRangeResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
-    sync_flow_url: Optional[shared_syncflowurl.SyncFlowURL] = dataclasses.field(default=None)
-
-    r"""Success"""
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_sync_status.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_company.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import company as shared_company
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetSyncStatusRequest:
+class CreateCompanyResponse:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
-    
-
-@dataclasses.dataclass
-class GetSyncStatusResponse:
-    
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    company: Optional[shared_company.Company] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/get_visible_accounts.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_visible_accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,20 @@
 from ..shared import visibleaccounts as shared_visibleaccounts
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetVisibleAccountsRequest:
     
-    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
-
-    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
-
+    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})  
+    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetVisibleAccountsResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
-
-    r"""Success"""
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/list_companies.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_companies.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,33 +7,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListCompaniesRequest:
     
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
 class ListCompaniesResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     companies: Optional[shared_companies.Companies] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/list_connections.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,27 @@
 from ..shared import connections as shared_connections
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListConnectionsRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
 class ListConnectionsResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     connections: Optional[shared_connections.Connections] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/list_integrations.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_integrations.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListIntegrationsRequest:
     
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
 class ListIntegrationsResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     integrations: Optional[shared_integrations.Integrations] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/request_sync.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,20 @@
 from ..shared import synctolatestargs as shared_synctolatestargs
 from typing import Optional
 
 
 @dataclasses.dataclass
 class RequestSyncRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
-    sync_to_latest_args: Optional[shared_synctolatestargs.SyncToLatestArgs] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    sync_to_latest_args: Optional[shared_synctolatestargs.SyncToLatestArgs] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class RequestSyncResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
-
-    r"""Success"""
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import daterange as shared_daterange
-from ..shared import syncsummary as shared_syncsummary
+from ..shared import visibleaccounts as shared_visibleaccounts
 from typing import Optional
 
 
 @dataclasses.dataclass
-class RequestSyncForDateRangeRequest:
+class UpdateVisibleAccountsSyncFlowRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
-    date_range: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
+    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})  
+    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
-class RequestSyncForDateRangeResponse:
+class UpdateVisibleAccountsSyncFlowResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
-    sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
-
-    r"""Success"""
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,13 @@
 from ..shared import localization as shared_localization
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UpdateConfigTextSyncFlowResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/update_connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,28 +7,21 @@
 from ..shared import updateconnection as shared_updateconnection
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UpdateConnectionRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-
-    update_connection: Optional[shared_updateconnection.UpdateConnection] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    update_connection: Optional[shared_updateconnection.UpdateConnection] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class UpdateConnectionResponse:
     
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
-
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/option.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import visibleaccounts as shared_visibleaccounts
+from codatsynccommerce import utils
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UpdateVisibleAccountsSyncFlowRequest:
+class Option:
     
-    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})
-
-    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
-    
-
-@dataclasses.dataclass
-class UpdateVisibleAccountsSyncFlowResponse:
-    
-    content_type: str = dataclasses.field()
-
-    status_code: int = dataclasses.field()
-
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
-    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
-
-    r"""Success"""
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for the option."""  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Name value of the option."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/__init__.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/accountoption.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/accountoption.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountOption:
     
     classification: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('classification'), 'exclude': lambda f: f is None }})
-
-    r"""Classification of the type of G/L account."""
+    r"""Classification of the type of G/L account."""  
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
-    r"""Identifier for the account, unique for the company."""
+    r"""Identifier for the account, unique for the company."""  
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-
-    r"""Name of the account."""
+    r"""Name of the account."""  
     nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-
-    r"""Reference given to each nominal account for a business. It ensures money is allocated to the correct account. This code isn't a unique identifier in the Codat system."""
+    r"""Reference given to each nominal account for a business. It ensures money is allocated to the correct account. This code isn't a unique identifier in the Codat system."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/branding.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/branding.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,13 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Branding:
     r"""Success"""
     
     button: Optional[shared_brandingbutton.BrandingButton] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('button'), 'exclude': lambda f: f is None }})
-
-    r"""Button branding references."""
+    r"""Button branding references."""  
     logo: Optional[shared_brandinglogo.BrandingLogo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logo'), 'exclude': lambda f: f is None }})
-
-    r"""Logo branding references."""
+    r"""Logo branding references."""  
     source_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId'), 'exclude': lambda f: f is None }})
-
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/brandingbutton.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingbutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingButton:
     r"""Button branding references."""
     
-    default: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})
-
-    hover: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hover'), 'exclude': lambda f: f is None }})
-
+    default: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})  
+    hover: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hover'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/brandingimage.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingImage:
     
     image: Optional[shared_imagereference.ImageReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('image'), 'exclude': lambda f: f is None }})
-
-    r"""Image reference."""
+    r"""Image reference."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/brandinglogo.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandinglogo.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingLogo:
     r"""Logo branding references."""
     
-    full: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('full'), 'exclude': lambda f: f is None }})
-
-    square: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('square'), 'exclude': lambda f: f is None }})
-
+    full: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('full'), 'exclude': lambda f: f is None }})  
+    square: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('square'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/companies.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import company as shared_company
+from ..shared import connection as shared_connection
 from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Companies:
+class Connections:
     r"""Success"""
     
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-
-    results: Optional[list[shared_company.Company]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
-
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/company.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/company.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Company:
     r"""A company in Codat represent a small or medium sized business, whose data you wish to share"""
     
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-
-    r"""Unique identifier for your SMB in Codat."""
+    r"""Unique identifier for your SMB in Codat."""  
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
-    r"""The name of the company"""
+    r"""The name of the company"""  
     redirect: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirect') }})
-
-    r"""The `redirect` [Link URL](https://docs.codat.io/auth-flow/authorize-hosted-link) enabling the customer to start their auth flow journey for the company."""
+    r"""The `redirect` [Link URL](https://docs.codat.io/auth-flow/authorize-hosted-link) enabling the customer to start their auth flow journey for the company."""  
     created: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -39,24 +35,20 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    created_by_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdByUserName'), 'exclude': lambda f: f is None }})
-
-    data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})
-
+    """  
+    created_by_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdByUserName'), 'exclude': lambda f: f is None }})  
+    data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})  
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-
-    r"""Additional information about the company. This can be used to store foreign IDs, references, etc."""
+    r"""Additional information about the company. This can be used to store foreign IDs, references, etc."""  
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -68,11 +60,10 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
-
+    """  
+    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/configaccount.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configaccount.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConfigAccount:
     r"""G/L account object for configuration."""
     
     account_options: Optional[list[shared_accountoption.AccountOption]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Object containing account options."""
+    r"""Object containing account options."""  
     description_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptionText'), 'exclude': lambda f: f is None }})
-
-    r"""Descriprtive text for sales configuration section."""
+    r"""Descriprtive text for sales configuration section."""  
     label_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('labelText'), 'exclude': lambda f: f is None }})
-
-    r"""Label text for sales configuration section."""
+    r"""Label text for sales configuration section."""  
     required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})
-
-    r"""Required section to be configured for sync."""
+    r"""Required section to be configured for sync."""  
     selected_account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedAccountId'), 'exclude': lambda f: f is None }})
-
-    r"""Selected account id from the list of available accounts."""
+    r"""Selected account id from the list of available accounts."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,16 +12,12 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Configuration:
     r"""Success"""
     
-    fees: Optional[shared_fees.Fees] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fees'), 'exclude': lambda f: f is None }})
-
-    new_payments: Optional[shared_newpayments.NewPayments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newPayments'), 'exclude': lambda f: f is None }})
-
-    payments: Optional[shared_payments.Payments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payments'), 'exclude': lambda f: f is None }})
-
-    sales: Optional[shared_sales.Sales] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})
-
+    fees: Optional[shared_fees.Fees] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fees'), 'exclude': lambda f: f is None }})  
+    new_payments: Optional[shared_newpayments.NewPayments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newPayments'), 'exclude': lambda f: f is None }})  
+    payments: Optional[shared_payments.Payments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payments'), 'exclude': lambda f: f is None }})  
+    sales: Optional[shared_sales.Sales] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Connection:
     r"""A connection represents the link between a `company` and a source of data."""
     
     created: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created') }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -40,45 +39,33 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """  
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-
-    r"""Unique identifier for a company's data connection."""
+    r"""Unique identifier for a company's data connection."""  
     integration_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
-
-    r"""A Codat ID representing the integration."""
+    r"""A Codat ID representing the integration."""  
     integration_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationKey') }})
-
-    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""
-    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})
-
-    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})
-
+    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""  
+    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})  
+    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})  
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
     source_type: ConnectionSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    r"""The type of platform of the connection."""
+    r"""The type of platform of the connection."""  
     status: shared_dataconnectionstatus_enum.DataConnectionStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-
-    r"""The current authorization status of the data connection."""
-    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})
-
-    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})
-
-    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})
-
+    r"""The current authorization status of the data connection."""  
+    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})  
+    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})  
+    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})  
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -90,9 +77,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/connections.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integrations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import connection as shared_connection
+from ..shared import integration as shared_integration
 from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Connections:
+class Integrations:
     r"""Success"""
     
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-
-    results: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
-
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/createcompany.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/createcompany.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,10 +7,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateCompany:
     
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
-    r"""Name of the company in Codat with a partner-commerce data connection."""
+    r"""Name of the company in Codat with a partner-commerce data connection."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/customer.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Customer:
     
     customer_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerOptions'), 'exclude': lambda f: f is None }})
-
-    r"""List of customer options from the list of customer records on the accounting software."""
+    r"""List of customer options from the list of customer records on the accounting software."""  
     selected_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedCustomerId'), 'exclude': lambda f: f is None }})
-
-    r"""Selected customer id from the list of customer records on the accounting software."""
+    r"""Selected customer id from the list of customer records on the accounting software."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/dataconnectionerror.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionerror.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnectionError:
     
     errored_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('erroredOnUtc'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -28,15 +27,12 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-
-    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-
-    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
-
+    """  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})  
+    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/datatypefeature.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/datatypefeature.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,13 +55,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataTypeFeature:
     r"""Describes support for a given datatype and associated operations"""
     
-    supported_features: list[shared_supportedfeature.SupportedFeature] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supportedFeatures') }})
-
+    supported_features: list[shared_supportedfeature.SupportedFeature] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supportedFeatures') }})  
     data_type: Optional[DataTypeFeatureDataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-
-    r"""Available Data types"""
+    r"""Available Data types"""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/daterange.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/daterange.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DateRange:
     
     finish: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('finish'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -28,17 +27,16 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """  
     start: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -50,9 +48,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/fees.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/fees.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,12 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Fees:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-
-    fees_supplier: Optional[shared_feessupplier.FeesSupplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feesSupplier'), 'exclude': lambda f: f is None }})
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    fees_supplier: Optional[shared_feessupplier.FeesSupplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feesSupplier'), 'exclude': lambda f: f is None }})  
     sync_fees: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncFees'), 'exclude': lambda f: f is None }})
-
-    r"""Boolean indicator to enable syncing fees."""
+    r"""Boolean indicator to enable syncing fees."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/feessupplier.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/feessupplier.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,13 +9,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class FeesSupplier:
     
     selected_supplier_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedSupplierId'), 'exclude': lambda f: f is None }})
-
-    r"""Selected supplier id from the list of supplier records on the accounting software."""
+    r"""Selected supplier id from the list of supplier records on the accounting software."""  
     supplier_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierOptions'), 'exclude': lambda f: f is None }})
-
-    r"""List of supplier options from the list of supplier records on the accounting software."""
+    r"""List of supplier options from the list of supplier records on the accounting software."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/grouping.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Grouping:
     
-    grouping_levels: Optional[shared_groupinglevels.GroupingLevels] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingLevels'), 'exclude': lambda f: f is None }})
-
-    grouping_period: Optional[shared_groupingperiod.GroupingPeriod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriod'), 'exclude': lambda f: f is None }})
-
+    grouping_levels: Optional[shared_groupinglevels.GroupingLevels] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingLevels'), 'exclude': lambda f: f is None }})  
+    grouping_period: Optional[shared_groupingperiod.GroupingPeriod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriod'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/groupinglevels.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupinglevels.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GroupingLevels:
     
-    invoice_level: Optional[shared_invoicelevelselection.InvoiceLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLevel'), 'exclude': lambda f: f is None }})
-
-    invoice_line_level: Optional[shared_invoicelinelevelselection.InvoiceLineLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLineLevel'), 'exclude': lambda f: f is None }})
-
+    invoice_level: Optional[shared_invoicelevelselection.InvoiceLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLevel'), 'exclude': lambda f: f is None }})  
+    invoice_line_level: Optional[shared_invoicelinelevelselection.InvoiceLineLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLineLevel'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/groupingperiod.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupingperiod.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GroupingPeriod:
     
     grouping_period_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriodOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Array of grouping period options."""
+    r"""Array of grouping period options."""  
     selected_grouping_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupingPeriod'), 'exclude': lambda f: f is None }})
-
-    r"""Grouping period i.e. Daily sales."""
+    r"""Grouping period i.e. Daily sales."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/halref.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/halref.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,9 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class HalRef:
     
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
-
+    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/imagereference.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/imagereference.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,11 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ImageReference:
     r"""Image reference."""
     
     alt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alt'), 'exclude': lambda f: f is None }})
-
-    r"""Alternative text when image is not available."""
+    r"""Alternative text when image is not available."""  
     src: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('src'), 'exclude': lambda f: f is None }})
-
-    r"""Source URL for image."""
+    r"""Source URL for image."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/integration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,34 +11,23 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Integration:
     r"""An integration that Codat supports"""
     
     enabled: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('enabled') }})
-
-    r"""Whether this integration is enabled for your customers to use"""
+    r"""Whether this integration is enabled for your customers to use"""  
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-
-    r"""A unique 4-letter key to represent a platform in each integration. View [accounting](https://docs.codat.io/integrations/accounting/accounting-platform-keys), [banking](https://docs.codat.io/integrations/banking/banking-platform-keys), and [commerce](https://docs.codat.io/integrations/commerce/commerce-platform-keys) platform keys."""
-    logo_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logoUrl') }})
-
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
-    data_provided_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataProvidedBy'), 'exclude': lambda f: f is None }})
-
-    datatype_features: Optional[list[shared_datatypefeature.DataTypeFeature]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datatypeFeatures'), 'exclude': lambda f: f is None }})
-
+    r"""A unique 4-letter key to represent a platform in each integration. View [accounting](https://docs.codat.io/integrations/accounting/accounting-platform-keys), [banking](https://docs.codat.io/integrations/banking/banking-platform-keys), and [commerce](https://docs.codat.io/integrations/commerce/commerce-platform-keys) platform keys."""  
+    logo_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logoUrl') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    data_provided_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataProvidedBy'), 'exclude': lambda f: f is None }})  
+    datatype_features: Optional[list[shared_datatypefeature.DataTypeFeature]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datatypeFeatures'), 'exclude': lambda f: f is None }})  
     integration_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
-
-    r"""A Codat ID representing the integration."""
-    is_beta: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBeta'), 'exclude': lambda f: f is None }})
-
-    is_offline_connector: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isOfflineConnector'), 'exclude': lambda f: f is None }})
-
+    r"""A Codat ID representing the integration."""  
+    is_beta: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBeta'), 'exclude': lambda f: f is None }})  
+    is_offline_connector: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isOfflineConnector'), 'exclude': lambda f: f is None }})  
     source_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId'), 'exclude': lambda f: f is None }})
-
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
     source_type: Optional[shared_sourcetype_enum.SourceTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType'), 'exclude': lambda f: f is None }})
-
-    r"""The type of platform of the connection."""
+    r"""The type of platform of the connection."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/integrations.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/links.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import integration as shared_integration
-from ..shared import links as shared_links
+from ..shared import halref as shared_halref
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Integrations:
-    r"""Success"""
+class Links:
     
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-
-    results: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
-
+    current: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})  
+    self_: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})  
+    next: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})  
+    previous: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/invoicelevelselection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelevelselection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InvoiceLevelSelection:
     
     group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Options for grouping sales."""
+    r"""Options for grouping sales."""  
     selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Selected array of grouping options."""
+    r"""Selected array of grouping options."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/companies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import company as shared_company
+from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineLevelSelection:
+class Companies:
+    r"""Success"""
     
-    group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Options for grouping on invoice lines."""
-    selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Invoice line level selection."""
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_company.Company]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/invoicestatus.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicestatus.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,13 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InvoiceStatus:
     
     invoice_status_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatusOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Options for invoice statuses."""
+    r"""Options for invoice statuses."""  
     selected_invoice_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedInvoiceStatus'), 'exclude': lambda f: f is None }})
-
-    r"""Selected option for invoice status for invoice to be synced."""
+    r"""Selected option for invoice status for invoice to be synced."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/links.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/localization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import halref as shared_halref
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Links:
+class Localization:
     
-    current: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
-
-    self_: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
-
-    next: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-
-    previous: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-
+    required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})  
+    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
+    r"""Value of the property."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/localization.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxrateamount.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Localization:
+class TaxRateAmount:
     
-    required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})
-
-    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
-
-    r"""Value of the property."""
+    selected_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedTaxRateId'), 'exclude': lambda f: f is None }})
+    r"""Selected tax rate id from the list of tax rates on the accounting software."""  
+    tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateOptions'), 'exclude': lambda f: f is None }})
+    r"""Array of tax rate options object."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/newpayments.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/payments.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class NewPayments:
+class Payments:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
     sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
-
-    r"""Boolean indicator for syncing payments."""
+    r"""Boolean indicator for syncing sales."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/newtaxrates.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newtaxrates.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,17 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class NewTaxRates:
     
     accounting_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountingTaxRateOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Array of accounting tax rate options."""
+    r"""Array of accounting tax rate options."""  
     commerce_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commerceTaxRateOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Array of tax component options."""
+    r"""Array of tax component options."""  
     default_zero_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultZeroTaxRateOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Default zero tax rate selected for sync."""
+    r"""Default zero tax rate selected for sync."""  
     selected_default_zero_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedDefaultZeroTaxRateId'), 'exclude': lambda f: f is None }})
-
-    r"""Default tax rate selected for sync."""
+    r"""Default tax rate selected for sync."""  
     tax_rate_mappings: Optional[list[shared_taxratemapping.TaxRateMapping]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateMappings'), 'exclude': lambda f: f is None }})
-
-    r"""Array of tax component to rate mapppings."""
+    r"""Array of tax component to rate mapppings."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/option.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncflowurl.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Option:
+class SyncFlowURL:
+    r"""Success"""
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
-    r"""Unique identifier for the option."""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-
-    r"""Name value of the option."""
+    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
+    r"""Sync flow URL."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/payments.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newpayments.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Payments:
+class NewPayments:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
     sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
-
-    r"""Boolean indicator for syncing sales."""
+    r"""Boolean indicator for syncing payments."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/sales.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sales.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,16 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Sales:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-
-    grouping: Optional[shared_grouping.Grouping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping'), 'exclude': lambda f: f is None }})
-
-    invoice_status: Optional[shared_invoicestatus.InvoiceStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatus'), 'exclude': lambda f: f is None }})
-
-    new_tax_rates: Optional[shared_newtaxrates.NewTaxRates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newTaxRates'), 'exclude': lambda f: f is None }})
-
-    sales_customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesCustomer'), 'exclude': lambda f: f is None }})
-
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    grouping: Optional[shared_grouping.Grouping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping'), 'exclude': lambda f: f is None }})  
+    invoice_status: Optional[shared_invoicestatus.InvoiceStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatus'), 'exclude': lambda f: f is None }})  
+    new_tax_rates: Optional[shared_newtaxrates.NewTaxRates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newTaxRates'), 'exclude': lambda f: f is None }})  
+    sales_customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesCustomer'), 'exclude': lambda f: f is None }})  
     sync_sales: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncSales'), 'exclude': lambda f: f is None }})
-
-    r"""Boolean indicator for syncing sales."""
-    tax_rates: Optional[dict[str, shared_taxrateamount.TaxRateAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
-
+    r"""Boolean indicator for syncing sales."""  
+    tax_rates: Optional[dict[str, shared_taxrateamount.TaxRateAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/supportedfeature.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/supportedfeature.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,12 +8,10 @@
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SupportedFeature:
     
-    feature_state: shared_featurestate_enum.FeatureStateEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureState') }})
-
-    feature_type: shared_featuretype_enum.FeatureTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureType') }})
-
+    feature_state: shared_featurestate_enum.FeatureStateEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureState') }})  
+    feature_type: shared_featuretype_enum.FeatureTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureType') }})
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/syncflowurl.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/visibleaccounts.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SyncFlowURL:
+class VisibleAccounts:
     r"""Success"""
     
-    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
-
-    r"""Sync flow URL."""
+    visible_accounts: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('visibleAccounts'), 'exclude': lambda f: f is None }})
+    r"""Visible accounts on sync flow."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/syncsummary.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncsummary.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,41 +11,31 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SyncSummary:
     r"""Success"""
     
     commerce_sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commerceSyncId'), 'exclude': lambda f: f is None }})
-
-    r"""Unique identifier for the sync in Codat."""
+    r"""Unique identifier for the sync in Codat."""  
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-
-    r"""Unique identifier for your SMB in Codat."""
+    r"""Unique identifier for your SMB in Codat."""  
     data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})
-
-    r"""Array of containing objects data connection information for the company."""
+    r"""Array of containing objects data connection information for the company."""  
     data_pushed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataPushed'), 'exclude': lambda f: f is None }})
-
-    r"""Boolean indicator for data being pushed during a sync operation."""
+    r"""Boolean indicator for data being pushed during a sync operation."""  
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-
-    r"""Friendly error message for the sync operation."""
-    sync_date_range_utc: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncDateRangeUtc'), 'exclude': lambda f: f is None }})
-
+    r"""Friendly error message for the sync operation."""  
+    sync_date_range_utc: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncDateRangeUtc'), 'exclude': lambda f: f is None }})  
     sync_exception_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncExceptionMessage'), 'exclude': lambda f: f is None }})
-
-    r"""Exception message for the sync operation."""
+    r"""Exception message for the sync operation."""  
     sync_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatus'), 'exclude': lambda f: f is None }})
-
-    r"""Status of the sync of the company data. This is linked to status code."""
+    r"""Status of the sync of the company data. This is linked to status code."""  
     sync_status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatusCode'), 'exclude': lambda f: f is None }})
-
-    r"""Numerical status code sync of the company data."""
+    r"""Numerical status code sync of the company data."""  
     sync_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncUtc'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -57,9 +47,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/synctolatestargs.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/synctolatestargs.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SyncToLatestArgs:
     
     sync_to: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncTo'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -28,9 +27,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/taxrateamount.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TaxRateAmount:
+class InvoiceLineLevelSelection:
     
-    selected_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedTaxRateId'), 'exclude': lambda f: f is None }})
-
-    r"""Selected tax rate id from the list of tax rates on the accounting software."""
-    tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateOptions'), 'exclude': lambda f: f is None }})
-
-    r"""Array of tax rate options object."""
+    group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
+    r"""Options for grouping on invoice lines."""  
+    selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
+    r"""Invoice line level selection."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/taxratemapping.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxratemapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TaxRateMapping:
     
     selected_accounting_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedAccountingTaxRateId'), 'exclude': lambda f: f is None }})
-
-    r"""Selected tax rate id from the list of tax rates on the accounting software."""
+    r"""Selected tax rate id from the list of tax rates on the accounting software."""  
     selected_commerce_tax_rate_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedCommerceTaxRateIds'), 'exclude': lambda f: f is None }})
-
-    r"""Selected tax component id from the list of tax components on the commerce software."""
+    r"""Selected tax component id from the list of tax components on the commerce software."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/models/shared/updateconnection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/updateconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UpdateConnection:
     
     status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-
-    r"""The current authorization status of the data connection."""
+    r"""The current authorization status of the data connection."""
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/sdk.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     sync_flow_preferences: SyncFlowPreferences
     r"""Configure preferences for any given Sync for Commerce company using sync flow."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.10.0"
-    _gen_version: str = "2.23.0"
+    _sdk_version: str = "0.9.0"
+    _gen_version: str = "2.22.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/sync.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/sync_flow_preferences.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync_flow_preferences.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/utils/retries.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.10.0/src/codatsynccommerce/utils/utils.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/utils.py`

 * *Files identical despite different names*

