# Comparing `tmp/codat-sync-for-expenses-0.12.0.tar.gz` & `tmp/codat-sync-for-expenses-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.12.0.tar", last modified: Wed Apr 26 15:09:57 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.13.0.tar", last modified: Thu Apr 27 12:36:41 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.12.0.tar` & `codat-sync-for-expenses-0.13.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.801787 codat-sync-for-expenses-0.12.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:09:57.801787 codat-sync-for-expenses-0.12.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 15:09:57.000000 codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4374 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4441 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.793787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      847 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1238 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5737 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5421 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4859 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/integrationtype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2154 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1615 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2036 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3968 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:09:57.797787 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-26 15:09:36.000000 codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.721711 codat-sync-for-expenses-0.13.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 12:36:41.721711 codat-sync-for-expenses-0.13.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:36:41.721711 codat-sync-for-expenses-0.13.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.713712 codat-sync-for-expenses-0.13.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.713712 codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 12:36:41.000000 codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-27 12:36:41.000000 codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:36:41.000000 codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 12:36:41.000000 codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 12:36:41.000000 codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.713712 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4374 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4441 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.713712 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.717712 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.721711 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5711 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5408 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4851 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1329 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/integrationtype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      569 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2148 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2418 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1611 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2027 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3968 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:36:41.721711 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-27 12:36:24.000000 codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.12.0/PKG-INFO` & `codat-sync-for-expenses-0.13.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.12.0
+Version: 0.13.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.12.0/README.md` & `codat-sync-for-expenses-0.13.0/README.md`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/setup.py` & `codat-sync-for-expenses-0.13.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.12.0",
+    version="0.13.0",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.12.0
+Version: 0.13.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.13.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/connections.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/expenses.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 from ..shared import createexpenseresponse as shared_createexpenseresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateExpenseDatasetRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
-    create_expense_request: Optional[shared_createexpenserequest.CreateExpenseRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
+    create_expense_request: Optional[shared_createexpenserequest.CreateExpenseRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+
     
 
 @dataclasses.dataclass
 class CreateExpenseDatasetResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     create_expense_response: Optional[shared_createexpenseresponse.CreateExpenseResponse] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""OK"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 from ..shared import dataconnection as shared_dataconnection
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreatePartnerExpenseConnectionRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     
 
 @dataclasses.dataclass
 class CreatePartnerExpenseConnectionResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     data_connection: Optional[shared_dataconnection.DataConnection] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 from ..shared import companyconfiguration as shared_companyconfiguration
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetCompanyConfigurationRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     
 
 @dataclasses.dataclass
 class GetCompanyConfigurationResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 from ..shared import companysyncstatus as shared_companysyncstatus
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLastSuccessfulSyncRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     
 
 @dataclasses.dataclass
 class GetLastSuccessfulSyncResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 from ..shared import companysyncstatus as shared_companysyncstatus
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLatestSyncRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     
 
 @dataclasses.dataclass
 class GetLatestSyncResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 from ..shared import mappingoptions as shared_mappingoptions
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetMappingOptionsRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     
 
 @dataclasses.dataclass
 class GetMappingOptionsResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     mapping_options: Optional[shared_mappingoptions.MappingOptions] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 from ..shared import companysyncstatus as shared_companysyncstatus
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSyncByIDRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-    r"""Unique identifier for a sync."""  
+
+    r"""Unique identifier for a sync."""
     
 
 @dataclasses.dataclass
 class GetSyncByIDResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,30 @@
 from ..shared import transactionmetadata as shared_transactionmetadata
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSyncTransactionRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-    r"""Unique identifier for a sync."""  
+
+    r"""Unique identifier for a sync."""
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionId', 'style': 'simple', 'explode': False }})
-    r"""The unique identifier for your SMB's transaction."""  
+
+    r"""The unique identifier for your SMB's transaction."""
     
 
 @dataclasses.dataclass
 class GetSyncTransactionResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
     transaction_metadata: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None)
-    r"""Success"""  
+
+    r"""Success"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,29 @@
 from ..shared import syncinitiated as shared_syncinitiated
 from typing import Optional
 
 
 @dataclasses.dataclass
 class IntiateSyncRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
-    post_sync: Optional[shared_postsync.PostSync] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
+    post_sync: Optional[shared_postsync.PostSync] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+
     
 
 @dataclasses.dataclass
 class IntiateSyncResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     codat_error_message: Optional[shared_codaterrormessage.CodatErrorMessage] = dataclasses.field(default=None)
-    r"""If model is incorrect"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""If model is incorrect"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
     sync_initiated: Optional[shared_syncinitiated.SyncInitiated] = dataclasses.field(default=None)
-    r"""Returns the newly created SyncId"""  
+
+    r"""Returns the newly created SyncId"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 from ..shared import transactionmetadatalist as shared_transactionmetadatalist
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSyncTransactionsRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-    r"""Unique identifier for a sync."""  
+
+    r"""Unique identifier for a sync."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
     
 
 @dataclasses.dataclass
 class ListSyncTransactionsResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
     transaction_metadata_list: Optional[shared_transactionmetadatalist.TransactionMetadataList] = dataclasses.field(default=None)
-    r"""Success"""  
+
+    r"""Success"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 from ..shared import companysyncstatus as shared_companysyncstatus
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSyncsRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     
 
 @dataclasses.dataclass
 class ListSyncsResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     company_sync_statuses: Optional[list[shared_companysyncstatus.CompanySyncStatus]] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,29 @@
 from ..shared import companyconfiguration as shared_companyconfiguration
 from typing import Optional
 
 
 @dataclasses.dataclass
 class SaveCompanyConfigurationRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
-    company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
+    company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+
     
 
 @dataclasses.dataclass
 class SaveCompanyConfigurationResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     codat_error_message: Optional[shared_codaterrormessage.CodatErrorMessage] = dataclasses.field(default=None)
-    r"""Bad Request"""  
+
+    r"""Bad Request"""
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""Success"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,31 +6,41 @@
 from ..shared import attachment as shared_attachment
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UploadAttachmentRequestBody:
     
-    content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})  
-    request_body: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'requestBody' }})  
+    content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})
+
+    request_body: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'requestBody' }})
+
     
 
 @dataclasses.dataclass
 class UploadAttachmentRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-    r"""Unique identifier for a sync."""  
+
+    r"""Unique identifier for a sync."""
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionId', 'style': 'simple', 'explode': False }})
-    r"""The unique identifier for your SMB's transaction."""  
-    request_body: Optional[UploadAttachmentRequestBody] = dataclasses.field(default=None, metadata={'multipart_form': { 'file': True }, 'request': { 'media_type': 'multipart/form-data' }})  
+
+    r"""The unique identifier for your SMB's transaction."""
+    request_body: Optional[UploadAttachmentRequestBody] = dataclasses.field(default=None, metadata={'multipart_form': { 'file': True }, 'request': { 'media_type': 'multipart/form-data' }})
+
     
 
 @dataclasses.dataclass
 class UploadAttachmentResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
+    content_type: str = dataclasses.field()
+
+    status_code: int = dataclasses.field()
+
     attachment: Optional[shared_attachment.Attachment] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+
+    r"""OK"""
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,22 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountMappingInfo:
     
     account_type: Optional[AccountMappingInfoAccountTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
-    r"""Type of the account."""  
+
+    r"""Type of the account."""
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    r"""Currency of the account."""  
+
+    r"""Currency of the account."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier of account."""  
+
+    r"""Unique identifier of account."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name of the account as it appears in the companies accounting software."""  
+
+    r"""Name of the account as it appears in the companies accounting software."""
     valid_transaction_types: Optional[list[AccountMappingInfoValidTransactionTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
-    r"""Supported transaction types for the account."""  
+
+    r"""Supported transaction types for the account."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,13 +9,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Attachment:
     r"""OK"""
     
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-    r"""Unique ID of company in Codat"""  
+
+    r"""Unique ID of company in Codat"""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier of attachment"""  
+
+    r"""Unique identifier of attachment"""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier of transaction"""  
+
+    r"""Unique identifier of transaction"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BankAccount:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""The id of the account from which purchases are made"""  
+
+    r"""The id of the account from which purchases are made"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,59 +7,85 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidationErrors:
     
-    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})  
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})  
-    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})  
-    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})  
+    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
+
+    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
+
+    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
+
+    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
+
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidationInternals:
     
-    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})  
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})  
-    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})  
-    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})  
+    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
+
+    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
+
+    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
+
+    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
+
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidationWarnings:
     
-    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})  
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})  
-    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})  
-    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})  
+    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
+
+    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
+
+    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
+
+    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
+
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidation:
     
-    errors: Optional[list[CodatErrorMessageValidationErrors]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})  
-    has_errors: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasErrors'), 'exclude': lambda f: f is None }})  
-    has_internals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasInternals'), 'exclude': lambda f: f is None }})  
-    has_warnings: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasWarnings'), 'exclude': lambda f: f is None }})  
-    internals: Optional[list[CodatErrorMessageValidationInternals]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('internals'), 'exclude': lambda f: f is None }})  
-    warnings: Optional[list[CodatErrorMessageValidationWarnings]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})  
+    errors: Optional[list[CodatErrorMessageValidationErrors]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
+
+    has_errors: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasErrors'), 'exclude': lambda f: f is None }})
+
+    has_internals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasInternals'), 'exclude': lambda f: f is None }})
+
+    has_warnings: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasWarnings'), 'exclude': lambda f: f is None }})
+
+    internals: Optional[list[CodatErrorMessageValidationInternals]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('internals'), 'exclude': lambda f: f is None }})
+
+    warnings: Optional[list[CodatErrorMessageValidationWarnings]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})
+
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessage:
     r"""Bad Request"""
     
-    can_be_retried: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('canBeRetried'), 'exclude': lambda f: f is None }})  
-    correlation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('correlationId'), 'exclude': lambda f: f is None }})  
-    detailed_error_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailedErrorCode'), 'exclude': lambda f: f is None }})  
-    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})  
-    inner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inner'), 'exclude': lambda f: f is None }})  
-    service: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service'), 'exclude': lambda f: f is None }})  
-    status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})  
-    validation: Optional[CodatErrorMessageValidation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})  
+    can_be_retried: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('canBeRetried'), 'exclude': lambda f: f is None }})
+
+    correlation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('correlationId'), 'exclude': lambda f: f is None }})
+
+    detailed_error_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailedErrorCode'), 'exclude': lambda f: f is None }})
+
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+
+    inner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inner'), 'exclude': lambda f: f is None }})
+
+    service: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service'), 'exclude': lambda f: f is None }})
+
+    status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
+
+    validation: Optional[CodatErrorMessageValidation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,11 +10,14 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompanyConfiguration:
     r"""Success"""
     
-    bank_account: shared_bankaccount.BankAccount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccount') }})  
-    customer: shared_customer.Customer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})  
-    supplier: shared_supplier.Supplier = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplier') }})  
+    bank_account: shared_bankaccount.BankAccount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccount') }})
+
+    customer: shared_customer.Customer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})
+
+    supplier: shared_supplier.Supplier = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplier') }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,36 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompanySyncStatus:
     r"""Success"""
     
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for your SMB in Codat."""  
+
+    r"""Unique identifier for your SMB in Codat."""
     data_pushed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataPushed'), 'exclude': lambda f: f is None }})
-    r"""Boolean of whether the sync resulted in data being pushed."""  
+
+    r"""Boolean of whether the sync resulted in data being pushed."""
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    r"""Error message of the sync."""  
+
+    r"""Error message of the sync."""
     sync_exception_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncExceptionMessage'), 'exclude': lambda f: f is None }})
-    r"""Exception message of the sync."""  
+
+    r"""Exception message of the sync."""
     sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier of the sync."""  
+
+    r"""Unique identifier of the sync."""
     sync_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatus'), 'exclude': lambda f: f is None }})
-    r"""Text status of the sync."""  
+
+    r"""Text status of the sync."""
     sync_status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatusCode'), 'exclude': lambda f: f is None }})
-    r"""Status code of the sync."""  
+
+    r"""Status code of the sync."""
     sync_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncUtc'), 'exclude': lambda f: f is None }})
+
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -42,9 +50,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """  
+    """
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateExpenseRequest:
     
-    items: Optional[list[shared_expensetransaction.ExpenseTransaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})  
+    items: Optional[list[shared_expensetransaction.ExpenseTransaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateExpenseResponse:
     r"""OK"""
     
     dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetId'), 'exclude': lambda f: f is None }})
-    r"""Unique id of dataset created"""  
+
+    r"""Unique id of dataset created"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/customer.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Customer:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""id of the customer for all income related activities to be associated to."""  
+
+    r"""id of the customer for all income related activities to be associated to."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnection:
     r"""A connection represents the link between a `company` and a source of data."""
     
     created: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created') }})
+
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -39,33 +40,45 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """  
+    """
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique identifier for a company's data connection."""  
+
+    r"""Unique identifier for a company's data connection."""
     integration_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
-    r"""A Codat ID representing the integration."""  
+
+    r"""A Codat ID representing the integration."""
     integration_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationKey') }})
-    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""  
-    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})  
-    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})  
+
+    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""
+    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})
+
+    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})
+
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
+
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
     source_type: DataConnectionSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    r"""The type of platform of the connection."""  
+
+    r"""The type of platform of the connection."""
     status: shared_dataconnectionstatus_enum.DataConnectionStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""The current authorization status of the data connection."""  
-    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})  
-    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})  
-    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})  
+
+    r"""The current authorization status of the data connection."""
+    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})
+
+    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})
+
+    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})
+
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
+
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -77,9 +90,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """  
+    """
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnectionError:
     
     errored_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('erroredOnUtc'), 'exclude': lambda f: f is None }})
+
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -27,12 +28,15 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """  
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
-    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})  
-    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})  
+    """
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
+
+    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
+
+    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,21 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpenseTransaction:
     
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
-    r"""Currency the transaction was recorded in."""  
+
+    r"""Currency the transaction was recorded in."""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Your unique identifier for the transaction."""  
+
+    r"""Your unique identifier for the transaction."""
     issue_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issueDate') }})
+
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -44,18 +47,20 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """  
+    """
     type: ExpenseTransactionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""The type of transaction."""  
+
+    r"""The type of transaction."""
     currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
+
     r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
     
     Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
     
     Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
     
     For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
@@ -71,15 +76,18 @@
     ## Examples with base currency of USD
     
     | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
     | :--------------- | :------------- | :------------ | :------------------------- |
     | **GBP**          | £20            | 1.277         | $25.54                     |
     | **EUR**          | €20            | 1.134         | $22.68                     |
     | **RUB**          | ₽20            | 0.015         | $0.30                      |
-    """  
+    """
     lines: Optional[list[shared_expensetransactionline.ExpenseTransactionLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
-    r"""Array of transaction lines."""  
+
+    r"""Array of transaction lines."""
     merchant_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('merchantName'), 'exclude': lambda f: f is None }})
-    r"""Name of the merchant where the purchase took place"""  
+
+    r"""Name of the merchant where the purchase took place"""
     notes: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
-    r"""Any private, company notes about the transaction."""  
+
+    r"""Any private, company notes about the transaction."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpenseTransactionLine:
     
-    account_ref: shared_recordref.RecordRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef') }})  
+    account_ref: shared_recordref.RecordRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef') }})
+
     net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
-    r"""Amount of the line, exclusive of tax."""  
+
+    r"""Amount of the line, exclusive of tax."""
     tax_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount') }})
-    r"""Amount of tax for the line."""  
-    tax_rate_ref: Optional[shared_recordref.RecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})  
-    tracking_refs: Optional[list[shared_recordref.RecordRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingRefs'), 'exclude': lambda f: f is None }})  
+
+    r"""Amount of tax for the line."""
+    tax_rate_ref: Optional[shared_recordref.RecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})
+
+    tracking_refs: Optional[list[shared_recordref.RecordRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingRefs'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class HalLink:
     
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})  
+    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class MappingOptions:
     r"""Success"""
     
     accounts: Optional[list[shared_accountmappinginfo.AccountMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-    r"""Array of available accounts for mapping."""  
+
+    r"""Array of available accounts for mapping."""
     expense_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expenseProvider'), 'exclude': lambda f: f is None }})
-    r"""Name of the expense integration."""  
+
+    r"""Name of the expense integration."""
     tax_rates: Optional[list[shared_taxratemappinginfo.TaxRateMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
-    r"""Array of available tax rates for mapping."""  
+
+    r"""Array of available tax rates for mapping."""
     tracking_categories: Optional[list[shared_trackingcategorymappinginfo.TrackingCategoryMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategories'), 'exclude': lambda f: f is None }})
-    r"""Array of available tracking categories for mapping."""  
+
+    r"""Array of available tracking categories for mapping."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostSync:
     
-    dataset_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetIds'), 'exclude': lambda f: f is None }})  
+    dataset_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetIds'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RecordRef:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""identifier of linked reference from mapping options."""  
+
+    r"""identifier of linked reference from mapping options."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Supplier:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""id of the supplier for all purchases to be associated to"""  
+
+    r"""id of the supplier for all purchases to be associated to"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SyncInitiated:
     r"""Returns the newly created SyncId"""
     
-    sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncId'), 'exclude': lambda f: f is None }})  
+    sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncId'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,25 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TaxRateMappingInfo:
     
     code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
-    r"""Code for the tax rate from the accounting platform."""  
+
+    r"""Code for the tax rate from the accounting platform."""
     effective_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('effectiveTaxRate'), 'exclude': lambda f: f is None }})
-    r"""Effective tax rate."""  
+
+    r"""Effective tax rate."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier of tax rate."""  
+
+    r"""Unique identifier of tax rate."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name of the tax rate in the accounting platform."""  
+
+    r"""Name of the tax rate in the accounting platform."""
     total_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalTaxRate'), 'exclude': lambda f: f is None }})
-    r"""Total (not compounded) sum of the components of a tax rate."""  
+
+    r"""Total (not compounded) sum of the components of a tax rate."""
     valid_transaction_types: Optional[list[TaxRateMappingInfoValidTransactionTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
-    r"""Supported transaction types for the account."""  
+
+    r"""Supported transaction types for the account."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackingCategoryMappingInfo:
     
     has_children: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasChildren'), 'exclude': lambda f: f is None }})
-    r"""Boolean of whether the tracking category has child categories."""  
+
+    r"""Boolean of whether the tracking category has child categories."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier of the tracking category."""  
+
+    r"""Unique identifier of the tracking category."""
     modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -31,13 +34,15 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """  
+    """
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name of the tracking category as it appears in the accounting software."""  
+
+    r"""Name of the tracking category as it appears in the accounting software."""
     parent_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentId'), 'exclude': lambda f: f is None }})
-    r"""ID of the parent tracking category"""  
+
+    r"""ID of the parent tracking category"""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadata:
     
     integration_type: Optional[shared_integrationtype_enum.IntegrationTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationType'), 'exclude': lambda f: f is None }})
-    r"""Type of transaction that has been processed e.g. Expense or Bank Feed."""  
+
+    r"""Type of transaction that has been processed e.g. Expense or Bank Feed."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-    r"""Metadata such as validation errors or the resulting record created in the accounting software."""  
+
+    r"""Metadata such as validation errors or the resulting record created in the accounting software."""
     status: Optional[shared_transactionstatus_enum.TransactionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""Status of the transaction."""  
+
+    r"""Status of the transaction."""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
-    r"""Your unique idenfier of the transaction."""  
+
+    r"""Your unique idenfier of the transaction."""
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,33 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadataListLinks:
     
-    current: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})  
-    self_: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})  
-    next: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})  
-    previous: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})  
+    current: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
+
+    self_: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
+
+    next: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+
+    previous: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadataList:
     r"""Success"""
     
-    links: TransactionMetadataListLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
-    results: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
+    links: TransactionMetadataListLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
+
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
+
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
+
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
+
+    results: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.12.0"
-    _gen_version: str = "2.22.0"
+    _sdk_version: str = "0.13.0"
+    _gen_version: str = "2.23.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/sync_status.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/transaction_status.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.12.0/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.13.0/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

