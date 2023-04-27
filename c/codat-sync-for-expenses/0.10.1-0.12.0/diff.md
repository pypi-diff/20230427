# Comparing `tmp/codat-sync-for-expenses-0.10.1.tar.gz` & `tmp/codat-sync-for-expenses-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.10.1.tar", last modified: Tue Apr 18 08:14:46 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.12.0.tar", last modified: Wed Apr 26 15:09:57 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.10.1.tar` & `codat-sync-for-expenses-0.12.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.869395 codat-sync-for-expenses-0.10.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-18 08:14:46.869395 codat-sync-for-expenses-0.10.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1725 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:14:46.869395 codat-sync-for-expenses-0.10.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.845394 codat-sync-for-expenses-0.10.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.849394 codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-18 08:14:46.000000 codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-18 08:14:46.000000 codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:14:46.000000 codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 08:14:46.000000 codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 08:14:46.000000 codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.853395 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4374 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4441 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.857395 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.861395 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      847 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1238 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.869395 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5737 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1144 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5421 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4857 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/integrationtype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2154 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1615 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2036 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3968 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:14:46.869395 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-18 08:14:32.000000 codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.801787 codat-sync-for-expenses-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:09:57.801787 codat-sync-for-expenses-0.12.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4374 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4441 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      847 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1238 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5737 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5421 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4859 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/integrationtype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2154 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1615 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2036 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3968 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.10.1/setup.py` & `codat-sync-for-expenses-0.12.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.10.1",
+    version="0.12.0",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi==2022.12.07",
+        "certifi==2022.12.7",
         "charset-normalizer==2.1.1",
         "dataclasses-json-speakeasy==0.5.8",
         "idna==3.3",
         "marshmallow==3.17.1",
         "marshmallow-enum==1.5.1",
         "mypy-extensions==0.4.3",
         "packaging==21.3",
```

### Comparing `codat-sync-for-expenses-0.10.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/connections.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/expenses.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import bankaccount as shared_bankaccount
-from ..shared import customer as shared_customer
-from ..shared import supplier as shared_supplier
+from ..shared import recordref as shared_recordref
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CompanyConfiguration:
-    r"""Success"""
+class ExpenseTransactionLine:
     
-    bank_account: Optional[shared_bankaccount.BankAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccount'), 'exclude': lambda f: f is None }})  
-    customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer'), 'exclude': lambda f: f is None }})  
-    supplier: Optional[shared_supplier.Supplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplier'), 'exclude': lambda f: f is None }})  
+    account_ref: shared_recordref.RecordRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef') }})  
+    net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
+    r"""Amount of the line, exclusive of tax."""  
+    tax_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount') }})
+    r"""Amount of tax for the line."""  
+    tax_rate_ref: Optional[shared_recordref.RecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})  
+    tracking_refs: Optional[list[shared_recordref.RecordRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingRefs'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpenseTransaction:
     
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
     r"""Currency the transaction was recorded in."""  
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Your unique idenfier for the transaction."""  
+    r"""Your unique identifier for the transaction."""  
     issue_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issueDate') }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
```

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import recordref as shared_recordref
+from ..shared import hallink as shared_hallink
+from ..shared import transactionmetadata as shared_transactionmetadata
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ExpenseTransactionLine:
+class TransactionMetadataListLinks:
     
-    account_ref: shared_recordref.RecordRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef') }})  
-    net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
-    r"""Amount of the line, exclusive of tax."""  
-    tax_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount') }})
-    r"""Amount of tax for the line."""  
-    tax_rate_ref: Optional[shared_recordref.RecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})  
-    tracking_refs: Optional[list[shared_recordref.RecordRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingRefs'), 'exclude': lambda f: f is None }})  
+    current: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})  
+    self_: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})  
+    next: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})  
+    previous: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})  
+    
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class TransactionMetadataList:
+    r"""Success"""
+    
+    links: TransactionMetadataListLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.10.1"
-    _gen_version: str = "2.18.1"
+    _sdk_version: str = "0.12.0"
+    _gen_version: str = "2.22.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync_status.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/transaction_status.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.10.1/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

