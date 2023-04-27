# Comparing `tmp/RobertCommonDriver-0.1.38.tar.gz` & `tmp/RobertCommonDriver-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.38.tar", last modified: Mon Apr 17 09:35:37 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.39.tar", last modified: Thu Apr 27 02:24:54 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.38.tar` & `RobertCommonDriver-0.1.39.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.648023 RobertCommonDriver-0.1.38/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.38/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.38/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2023-04-17 09:35:37.648023 RobertCommonDriver-0.1.38/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.38/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.584677 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-14 13:23:29.000000 RobertCommonDriver-0.1.38/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.584677 RobertCommonDriver-0.1.38/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.38/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.585677 RobertCommonDriver-0.1.38/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.597677 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     4980 2022-12-01 08:57:24.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.615893 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    62987 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    62779 2023-04-17 09:22:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566042 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    33721 2023-04-14 08:37:47.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18312 2023-04-13 03:18:43.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    62003 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    23955 2023-04-14 09:08:35.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43387 2023-04-13 08:35:41.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51617 2023-04-13 08:22:42.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41508 2023-04-13 08:32:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32748 2023-04-14 09:33:24.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44632 2023-04-14 09:40:13.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-04-17 09:35:37.648960 RobertCommonDriver-0.1.38/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-04-17 09:35:17.000000 RobertCommonDriver-0.1.38/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.616893 RobertCommonDriver-0.1.38/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.38/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.617892 RobertCommonDriver-0.1.38/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.38/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.628894 RobertCommonDriver-0.1.38/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.646964 RobertCommonDriver-0.1.38/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22764 2023-04-13 09:16:01.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0     9711 2023-04-14 08:35:25.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3646 2023-04-14 09:02:11.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     7609 2023-04-14 09:31:32.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.797557 RobertCommonDriver-0.1.39/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.39/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.39/MANIFEST.in
+-rw-rw-rw-   0        0        0     1744 2023-04-27 02:24:54.797557 RobertCommonDriver-0.1.39/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.39/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.723381 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0     1744 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.39/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.724700 RobertCommonDriver-0.1.39/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.39/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.725706 RobertCommonDriver-0.1.39/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.740725 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     4980 2022-12-01 08:57:24.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.760893 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    62987 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    62781 2023-04-26 10:00:30.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566042 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    33803 2023-04-25 09:57:11.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18368 2023-04-27 02:18:02.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    62003 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24090 2023-04-24 09:50:15.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43387 2023-04-13 08:35:41.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51617 2023-04-13 08:22:42.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41508 2023-04-13 08:32:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32748 2023-04-14 09:33:24.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44632 2023-04-14 09:40:13.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-04-27 02:24:54.797557 RobertCommonDriver-0.1.39/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-04-27 02:24:37.000000 RobertCommonDriver-0.1.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.762066 RobertCommonDriver-0.1.39/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.39/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.763074 RobertCommonDriver-0.1.39/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.39/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.776646 RobertCommonDriver-0.1.39/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.795048 RobertCommonDriver-0.1.39/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22764 2023-04-13 09:16:01.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    13461 2023-04-26 06:02:28.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3667 2023-04-24 09:44:00.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     7609 2023-04-14 09:31:32.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.38/LICENSE` & `RobertCommonDriver-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/PKG-INFO` & `RobertCommonDriver-0.1.39/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.38
+Version: 0.1.39
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.38/README.md` & `RobertCommonDriver-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.38
+Version: 0.1.39
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
             pass
         return bacnet_device
 
     def control(self, status: bool = True):
         self.logging(content=f"control({status})", pos=self.stack_pos)
         if status is True:
             enable_sleeping()
-            run(spin=self.bacnet_cmd_interval, sigterm=None, sigusr1=None)
+            run(spin=self.bacnet_cmd_interval/5, sigterm=None, sigusr1=None)
         else:
             stop()
 
     def discover(self, low_device_id: Optional[int] = None, high_device_id: Optional[int] = None, target_address: Optional[str] = None) -> bool:
         request = WhoIsRequest()
         if low_device_id is not None:
             request.deviceInstanceRangeLowLimit = low_device_id
```

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_modbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,15 @@
 
     def _combine_read_unit(self, modbus_unit, modbus_read_units: dict):
         read_units = modbus_read_units.get(modbus_unit.__str__())
         if read_units is not None:
             if modbus_unit.get_modbus_start == (read_units[-1].get_modbus_end + 1):
                 if read_units[-1].get_modbus_end - read_units[-1].get_modbus_start + 1 >= self.configs.get('multi_read', 100):  # 超过连读上限
                     read_units[-1].set_full_flag()
+                    modbus_read_units[modbus_unit.__str__()].append(modbus_unit)
                 else:
                     read_units[-1].set_modbus_end(modbus_unit.get_modbus_end)
             elif modbus_unit.get_modbus_start == read_units[-1].get_modbus_end:
                 read_units[-1].set_modbus_end(modbus_unit.get_modbus_end)
             else:
                 modbus_read_units[modbus_unit.__str__()].append(modbus_unit)
         else:
```

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_obix.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             'bool': lambda x: x.lower() == "true",
             'real': float,
             'enum': self._enum_value_handler,
         }
 
     def exit(self):
         self.exit_flag = True
-
+        self._del_watch()
         self.reinit()
 
     @classmethod
     def template(cls, mode: int, type: str, lan: str) -> List[Dict[str, Any]]:
         templates = []
         if type == 'point':
             templates.extend([
@@ -240,14 +240,15 @@
 
                     self._set_reltime()
 
                 self._add_points(items)
 
             self._pool_refresh()
         except Exception as e:
+            self._del_watch()
             self.logging(content=f"obix read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
             for item in items:
                 self.update_device(self.configs.get('url'), item, **self.gen_read_write_result(False, e.__str__()))
 
     def get_value(self, name: str, url: str, type: str):
         try:
             [result, value] = self.get_device_property(self.configs.get('url'), url, [self.get_read_quality, self.get_read_result])
```

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcua.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,17 @@
         except:
             pass
         try:
             if self.client:
                 self.client.disconnect()
         except:
             pass
+        self.subs = []
         self.client = None
+        self.devices = {}
 
     def _get_sub(self):
         if self.sub is None:
             sub = self._get_client().create_subscription(self.configs.get('subscript_interval', 500), self.SubHandler(callbacks={'datachange_notification': self._datachange_notification}))
             self.sub = sub
         return self.sub
 
@@ -387,14 +389,15 @@
     def _release_server(self):
         try:
             if self.server is not None:
                 self.server.stop()
         except Exception as e:
             pass
         self.server = None
+        self.server_node_folder = {}
 
     def _create_folder(self, server, paths: Union[str, list]):
         root_folder = self.server_node_folder[self.configs.get('root', 'Robert')]
         if isinstance(paths, list):
             for index, folder in enumerate(paths):
                 self._create_folder(server, '/'.join(paths[:index+1]))
         elif isinstance(paths, str):
@@ -414,26 +417,26 @@
                     node_path = object.get('point_name')
 
                 paths = node_path.replace('\\', '/').split('/')
                 folder = self.server_node_folder.get(root)
                 try:
                     if len(paths) > 1:     # 创建子目录
                         folder = self._create_folder(self._get_server(), paths[:-1])
-                    self.server_nodes[node_id] = folder.add_variable(node_id, paths[-1], IOTBaseCommon.format_value(object.get('point_value')))
+                    self.server_nodes[node_id] = folder.add_variable(node_id, ua.QualifiedName(paths[-1]), ua.DataValue(IOTBaseCommon.format_value(object.get('point_value'))))
                     self.server_nodes[node_id].set_writable()
                     self.logging(content=f"create object: {node_path}({node_id})", pos=self.stack_pos)
                 except Exception as e:
                     self.logging(content=f"create object: {node_path}({node_id}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _refresh_objects(self, objects: List[IOTSimulateObject]):
         for object in objects:
             node_id = object.get('point_node_id')
             if node_id in self.server_nodes.keys():
                 try:
-                    self.server_nodes[node_id].set_value(IOTBaseCommon.format_value(object.get('point_value')))
+                    self.server_nodes[node_id].set_value(ua.DataValue(IOTBaseCommon.format_value(object.get('point_value'))))
                 except Exception as e:
                     self.logging(content=f"refresh object({node_id}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _cert_to_string(self, der):
         if not der:
             return 'no certificate'
         try:
```

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/setup.py` & `RobertCommonDriver-0.1.39/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.38'
-DATE = '2023-04-17'
+VERSION = '0.1.39'
+DATE = '2023-04-27'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,46 @@
     # 轮询全部
     while True:
         dict_result_scrap = modbus_driver.read()
         print(dict_result_scrap)
         time.sleep(2)
 
 
+def test_read1():
+    #配置项
+    dict_config = {
+                        'multi_read': 1,                             # 批量读取个数
+                        'cmd_interval': 0.3,                         # 命令间隔
+                        'time_out': 5                                 # 超时时间
+                    }
+    #点表
+    dict_point = {}
+    dict_point['modbus_0'] = {'point_writable': True, 'point_name': 'modbus_0', 'point_device_address': '192.168.1.184/502',  'point_slave_id': 1, 'point_fun_code': 3, 'point_address': 0, 'point_data_type': 18, 'point_data_length': 2, 'point_scale':'1'}
+    dict_point['modbus_1'] = {'point_writable': True, 'point_name': 'modbus_1', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 2, 'point_data_type': 18, 'point_data_length': 2, 'point_scale': '1'}
+    dict_point['modbus_2'] = {'point_writable': True, 'point_name': 'modbus_2', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 4, 'point_data_type': 18, 'point_data_length': 2, 'point_scale': '1'}
+
+    dict_point['signed'] = {'point_writable': True, 'point_name': 'signed', 'point_device_address': '192.168.1.172/502',  'point_slave_id': 2, 'point_fun_code': 3, 'point_address': 0, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['unsigned'] = {'point_writable': True, 'point_name': 'unsigned', 'point_device_address': '192.168.1.172/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 1, 'point_data_type': 6, 'point_data_length': 1, 'point_scale': '1'}
+    dict_point['bit'] = {'point_writable': True, 'point_name': 'bit', 'point_device_address': '192.168.1.172/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 2, 'point_data_type': 8, 'point_data_length': 1, 'point_scale': '1'}
+    dict_point['long'] = {'point_writable': True, 'point_name': 'long', 'point_device_address': '192.168.1.172/502',  'point_slave_id': 2, 'point_fun_code': 3, 'point_address': 4, 'point_data_type': 12, 'point_data_length': 2, 'point_scale':'1'}
+    dict_point['long_rev'] = {'point_writable': True, 'point_name': 'long_rev', 'point_device_address': '192.168.1.172/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 6, 'point_data_type': 12, 'point_data_order': 2, 'point_data_length': 2, 'point_scale': '1'}
+    dict_point['float'] = {'point_writable': True, 'point_name': 'float', 'point_device_address': '192.168.1.172/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 10, 'point_data_type': 18, 'point_data_length': 2, 'point_scale': '1'}
+    dict_point['float_rev'] = {'point_writable': True, 'point_name': 'float_rev', 'point_device_address': '192.168.1.172/502',  'point_slave_id': 2, 'point_fun_code': 3, 'point_address': 12, 'point_data_type': 18, 'point_data_order': 2, 'point_data_length': 2, 'point_scale':'1'}
+    dict_point['double'] = {'point_writable': True, 'point_name': 'double', 'point_device_address': '192.168.1.172/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 16, 'point_data_type': 20, 'point_data_length': 4, 'point_scale': '1'}
+    dict_point['double_rev'] = {'point_writable': True, 'point_name': 'double_rev', 'point_device_address': '192.168.1.172/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 24, 'point_data_type': 20, 'point_data_order': 2, 'point_data_length': 4, 'point_scale': '1'}
+
+    modbus_driver = IOTModbus(configs=dict_config, points=dict_point)
+    modbus_driver.logging(call_logging=logging_print)
+    # 轮询全部
+    while True:
+        dict_result_scrap = modbus_driver.read()
+        print(dict_result_scrap)
+        time.sleep(2)
+
+
 def test_write():
     # 配置项
     dict_config = {
         'multi_read': 100,  # 批量读取个数
         'cmd_interval': 0.3,  # 命令间隔
         'time_out': 5  # 超时时间
     }
@@ -90,9 +122,9 @@
     while True:
         #for name, point in dict_point.items():
         #    point['point_value'] = random.randint(1, 100)
         client.simulate(points=dict_point)
         time.sleep(10)
 
 
-test_read()
+test_read1()
```

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     dict_config = {
         'endpoint': 'opc.tcp://0.0.0.0:4841/freeopcua/server/',
         'name': 'Robert OPC UA Server',  #
         'root': 'Robert1'
     }
 
     dict_point = {}
-    dict_point['opcua1'] = {'point_writable': True, 'point_name': 'opcua1', 'point_node_id': 'ns=2;i=1000', 'point_node_path': '', 'point_scale': '1'}
-    dict_point['opcua'] = {'point_writable': True, 'point_name': 'opcua2', 'point_node_id': 'ns=2;i=1001', 'point_node_path': 'group2/group3/point2', 'point_scale': '1'}
+    dict_point['opcua1'] = {'point_writable': True, 'point_name': 'opcua1', 'point_node_id': 'ns=2;s=ModbusOPC.OPC1.qeq', 'point_node_path': '', 'point_scale': '1'}
+    dict_point['opcua'] = {'point_writable': True, 'point_name': 'opcua2', 'point_node_id': 'ns=2;s=通道1.qwq', 'point_node_path': 'group2/group3/point2', 'point_scale': '1'}
 
     client = IOTOPCUA(configs=dict_config, points=dict_point)
     client.logging(call_logging=logging_print)
     while True:
         for name, point in dict_point.items():
             point['point_value'] = f"{random.randint(1, 100)}"
         client.simulate(points=dict_point)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

