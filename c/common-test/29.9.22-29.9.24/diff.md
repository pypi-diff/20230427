# Comparing `tmp/common-test-29.9.22.tar.gz` & `tmp/common-test-29.9.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.22.tar", last modified: Mon Apr 24 05:36:33 2023, max compression
+gzip compressed data, was "common-test-29.9.24.tar", last modified: Thu Apr 27 05:56:13 2023, max compression
```

## Comparing `common-test-29.9.22.tar` & `common-test-29.9.24.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.574927 common-test-29.9.22/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-24 05:36:33.575057 common-test-29.9.22/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.548661 common-test-29.9.22/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.22/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.550206 common-test-29.9.22/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.22/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.22/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.22/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.22/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.555089 common-test-29.9.22/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.22/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.22/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.22/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.22/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.556773 common-test-29.9.22/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.22/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.22/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.559783 common-test-29.9.22/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.22/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17498 2023-04-24 05:17:14.000000 common-test-29.9.22/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.22/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.562447 common-test-29.9.22/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.22/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.22/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.565445 common-test-29.9.22/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.22/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11930 2023-04-24 05:17:14.000000 common-test-29.9.22/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.22/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.566063 common-test-29.9.22/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.22/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.22/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.568243 common-test-29.9.22/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.22/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.22/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.572376 common-test-29.9.22/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.22/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.22/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.22/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3908 2023-04-23 08:05:34.000000 common-test-29.9.22/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    11219 2023-04-24 05:18:09.000000 common-test-29.9.22/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.22/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.22/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.574618 common-test-29.9.22/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-24 05:36:33.575783 common-test-29.9.22/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-04-24 05:34:13.000000 common-test-29.9.22/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.145079 common-test-29.9.24/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-27 05:56:13.145620 common-test-29.9.24/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.106168 common-test-29.9.24/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.24/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.108386 common-test-29.9.24/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.24/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.24/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.24/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.24/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.111274 common-test-29.9.24/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.24/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.24/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.24/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.24/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.112285 common-test-29.9.24/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.24/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.24/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.114844 common-test-29.9.24/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.24/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17498 2023-04-24 05:17:14.000000 common-test-29.9.24/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.24/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.119747 common-test-29.9.24/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.24/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.24/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.24/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.125156 common-test-29.9.24/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.24/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11776 2023-04-27 05:55:54.000000 common-test-29.9.24/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.24/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.24/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.126164 common-test-29.9.24/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.24/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.24/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.130190 common-test-29.9.24/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.24/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.24/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.140271 common-test-29.9.24/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.24/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.24/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.24/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3908 2023-04-23 08:05:34.000000 common-test-29.9.24/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    11215 2023-04-24 05:43:36.000000 common-test-29.9.24/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.24/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.24/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.24/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-27 05:56:13.143609 common-test-29.9.24/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-27 05:56:12.000000 common-test-29.9.24/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-27 05:56:13.147838 common-test-29.9.24/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-04-27 05:55:54.000000 common-test-29.9.24/setup.py
```

### Comparing `common-test-29.9.22/PKG-INFO` & `common-test-29.9.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.22
+Version: 29.9.24
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.22/common/autotest/base_requests.py` & `common-test-29.9.24/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/autotest/handle_allure.py` & `common-test-29.9.24/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/autotest/handle_assert.py` & `common-test-29.9.24/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/common/api_driver.py` & `common-test-29.9.24/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/common/constant.py` & `common-test-29.9.24/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/common/test.py` & `common-test-29.9.24/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/config/config.py` & `common-test-29.9.24/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/data/data_process.py` & `common-test-29.9.24/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/data/handle_common.py` & `common-test-29.9.24/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/db/handle_db.py` & `common-test-29.9.24/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/db/handle_db_batch.py` & `common-test-29.9.24/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/db/handle_mysqldb.py` & `common-test-29.9.24/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/db/handle_oracle.py` & `common-test-29.9.24/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/db/handle_sqlserver.py` & `common-test-29.9.24/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/file/ReadFile.py` & `common-test-29.9.24/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/file/handle_excel.py` & `common-test-29.9.24/common/file/handle_excel.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,18 +207,14 @@
     data_file = adjust_path_data(data_file)
     data_list = []  # 新建个空列表，来存储所有的数据
     wb = xlrd.open_workbook(data_file)  # 打开excel
     sh = wb.sheet_by_name(sheet)  # 获取工作簿
     # 获取标题行数据
     #header = sh.row_values(0)
     # 跳过标题行，从第二行开始取数据
-    _mysql = None
-    if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-        _config = {'key': 'traffic', 'env': 'test'}
-        _mysql = MysqlDB(_config)
     for row in range(_index, sh.nrows):
         d = dict()
         # 将标题和每行数据组装成字典
         for col in range(0, sh.ncols):
             # 获取指定单元格数据(行，列)
             cell_data = sh.cell_value(row, col)
             ctype = sh.cell(row, col).ctype
@@ -238,16 +234,14 @@
                 temp['_sheetName'] = sheet
             else:
                 temp = d
                 temp['_excelPath'] = data_file
                 temp['_sheetName'] = sheet
             print_info(f'添加单个参数化用例数据: {temp}')
             data_list.append(temp)
-        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            _mysql.close()
         print_info(f'用例参数化数据: {data_list}')
     return data_list
 
 
 
 def check_excel_data(testdata:dict, _mysql, _filter, _checkData):
     if _checkData:
@@ -256,24 +250,28 @@
         if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
             return True
         if DataProcess.isNotNull(casename) == False or DataProcess.isNotNull(caseNo) == False:
             return False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)) and _mysql is not None:
             cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
             _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and casename='{casename}'"
+            _mysql = MysqlDB({'key': 'traffic', 'env': 'test'})
             _info = _mysql.execute(_sql).fetchall()
             if len(_info) < 1:
                 _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and caseid='{caseNo}'"
                 _info = _mysql.execute(_sql).fetchall()
+
             if len(_info) < 1:
+                _mysql.close()
                 return False
             else:
                 _temp = _info[0]
                 logger.info(f"执行参数化用例编号:{_temp['caseid']} 用例名称：{_temp['casename']}  运行ID:{_temp['caserunid']} ")
                 print_info(f'执行参数化测试数据: {testdata}')
+                _mysql.close()
                 return True
         if testdata[Constant.CASE_STATUS].strip() == '否':
             return False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
             if testdata[Constant.CASE_TITLE] in eval(get_system_key(Constant.TEST_CASE_NAME_LIST)):
                 return True
             else:
```

### Comparing `common-test-29.9.22/common/file/handle_file.py` & `common-test-29.9.24/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/file/handle_reques.py` & `common-test-29.9.24/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/file/handle_system.py` & `common-test-29.9.24/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/file/handle_yaml.py` & `common-test-29.9.24/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/mq/handle_rabbit.py` & `common-test-29.9.24/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plat/ATF_platform.py` & `common-test-29.9.24/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plat/jenkin_platform.py` & `common-test-29.9.24/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plat/jira_platform.py` & `common-test-29.9.24/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plat/mysql_platform.py` & `common-test-29.9.24/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plat/service_platform.py` & `common-test-29.9.24/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/allure_plugin.py` & `common-test-29.9.24/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/assert_plugin.py` & `common-test-29.9.24/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/atf_plugin.py` & `common-test-29.9.24/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/data_bus.py` & `common-test-29.9.24/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/data_plugin.py` & `common-test-29.9.24/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/file_plugin.py` & `common-test-29.9.24/common/plugin/file_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
                 _flag = False
         return _flag
 
 
 
 if __name__ == '__main__':
     _xml=FilePlugin.excel_to_dict("data.xls",sheet="Sheet1",_filter={'需求名称':'bocc上传提交'})
-    print(_xml[0].get('$上传文件')[2].get('用例编号'))
+    print(_xml[0].get('上传文件').get('用例编号'))
```

### Comparing `common-test-29.9.22/common/plugin/hooks_plugin.py` & `common-test-29.9.24/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/pytest_playwright.py` & `common-test-29.9.24/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common/plugin/pytest_plugin.py` & `common-test-29.9.24/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common_test.egg-info/PKG-INFO` & `common-test-29.9.24/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.22
+Version: 29.9.24
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.22/common_test.egg-info/SOURCES.txt` & `common-test-29.9.24/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/common_test.egg-info/requires.txt` & `common-test-29.9.24/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.22/setup.py` & `common-test-29.9.24/setup.py`

 * *Files identical despite different names*

