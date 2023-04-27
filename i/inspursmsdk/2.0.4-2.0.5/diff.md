# Comparing `tmp/inspursmsdk-2.0.4.tar.gz` & `tmp/inspursmsdk-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspursmsdk-2.0.4.tar", last modified: Thu Apr 27 08:55:10 2023, max compression
+gzip compressed data, was "dist/inspursmsdk-2.0.5.tar", last modified: Thu Apr 27 09:11:58 2023, max compression
```

## Comparing `inspursmsdk-2.0.4.tar` & `inspursmsdk-2.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/
--rw-r--r--   0 root         (0) root         (0)      991 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      888 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49060 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    20338 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   306678 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11954 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18131 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54444 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84520 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81800 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46175 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   360127 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   360290 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    65986 2023-04-27 08:53:48.000000 inspursmsdk-2.0.4/inspur_sm_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    43783 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)   743806 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   631511 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    17358 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16476 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   259774 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)    45791 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14793 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15217 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59696 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47127 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   120002 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:47.000000 inspursmsdk-2.0.4/inspur_sm_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4652 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-04-27 08:53:46.000000 inspursmsdk-2.0.4/inspur_sm_sdk/util/parameterConversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/inspursmsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-04-27 08:55:09.000000 inspursmsdk-2.0.4/inspursmsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2598 2023-04-27 08:55:09.000000 inspursmsdk-2.0.4/inspursmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 08:55:09.000000 inspursmsdk-2.0.4/inspursmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-27 08:55:09.000000 inspursmsdk-2.0.4/inspursmsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-27 08:55:09.000000 inspursmsdk-2.0.4/inspursmsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/ism.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 08:55:10.000000 inspursmsdk-2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2023-04-27 08:53:49.000000 inspursmsdk-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)      991 2023-04-27 08:53:49.000000 inspursmsdk-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-27 08:53:49.000000 inspursmsdk-2.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-27 08:53:49.000000 inspursmsdk-2.0.5/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49338 2023-04-27 09:11:35.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    20338 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   306678 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11954 2023-04-27 08:53:49.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2023-04-27 08:53:49.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18131 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54444 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84520 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81800 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46175 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   360127 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   360290 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    65986 2023-04-27 08:53:48.000000 inspursmsdk-2.0.5/inspur_sm_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/conf/
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/conf/NF5180M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/conf/NF5280M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/conf/SA5112M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/conf/SA5212M5.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    43783 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)   743806 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   631511 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    17358 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   259774 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)    45791 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14793 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59696 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47127 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   120002 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:47.000000 inspursmsdk-2.0.5/inspur_sm_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-04-27 08:53:46.000000 inspursmsdk-2.0.5/inspur_sm_sdk/util/parameterConversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspursmsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspursmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspursmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspursmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspursmsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/inspursmsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-04-27 09:11:26.000000 inspursmsdk-2.0.5/ism.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 09:11:58.000000 inspursmsdk-2.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-04-27 08:53:49.000000 inspursmsdk-2.0.5/setup.py
```

### Comparing `inspursmsdk-2.0.4/MANIFEST.in` & `inspursmsdk-2.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/PKG-INFO` & `inspursmsdk-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.0.4
+Version: 2.0.5
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/IpmiFunc.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/IpmiFunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1282,24 +1282,34 @@
     return sendRawByIpmi(client, cmd)
 
 
 def setBootOptions(client, bootType, timeLines):
     cmd = 'chassis bootdev ' + bootType
     if timeLines is not None and timeLines == 'persistent':
         cmd = cmd + ' options=' + timeLines
-    return sendRawByIpmi(client, cmd)
+    result = __getCmd_type(client, cmd, 'readline')
+    if result['code'] != 0:
+        return result
+    cmd_str = result['data']
+    if 'Set Boot Device to' not in cmd_str:
+        res['code'] = -1
+        res['data'] = 'Failure: ' + cmd_str
+        return res
+    res['code'] = 0
+    res['data'] = 'Success'
+    return res
 
 
 def sendRawByIpmi(client, raw):
     res = {}
     result = __getCmd_type(client, raw, 'readline')
     if result['code'] != 0:
         return result
     cmd_str = result['data']
-    if 'Set Boot Device to' not in cmd_str:
+    if cmd_str != '\n':
         res['code'] = -1
         res['data'] = 'Failure: ' + cmd_str
         return res
     res['code'] = 0
     res['data'] = 'Success'
     return res
```

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/biosPostEventStr.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/commonInfoStr.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/eventLogString.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/sensorEventStr.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/M5Log/showSensorDesc.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/M5Log/showSensorDesc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/RedfishFunc.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/RestFunc.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/RestFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/backup.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/A7.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF3180A6.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF3280A6.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5468A5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/NF5488A5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/command/restore.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/conf/NF5180M5.yml` & `inspursmsdk-2.0.5/inspur_sm_sdk/conf/NF5180M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/conf/NF5280M5.yml` & `inspursmsdk-2.0.5/inspur_sm_sdk/conf/NF5280M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/conf/SA5112M5.yml` & `inspursmsdk-2.0.5/inspur_sm_sdk/conf/SA5112M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/conf/SA5212M5.yml` & `inspursmsdk-2.0.5/inspur_sm_sdk/conf/SA5212M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/Base.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/Base.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonA5.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonA6.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonA7.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM5.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM6.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM6_41401.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM6_41401.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM6_4140a.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/CommonM7.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/CommonM7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/I24M6.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/IBase.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5180M5.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5_435.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/NF5280M5_436.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/NS5160M6.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/ResEntity.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/ResEntity.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/interface/SA5212M5Impl.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/interface/SA5212M5Impl.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/route/route.yml` & `inspursmsdk-2.0.5/inspur_sm_sdk/route/route.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/HostTypeJudge.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/HostTypeJudge.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/RedfishClient.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/RegularCheckUtil.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/RequestClient.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/configUtil.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/fileUtil.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspur_sm_sdk/util/parameterConversion.py` & `inspursmsdk-2.0.5/inspur_sm_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/inspursmsdk.egg-info/PKG-INFO` & `inspursmsdk-2.0.5/inspursmsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.0.4
+Version: 2.0.5
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.0.4/inspursmsdk.egg-info/SOURCES.txt` & `inspursmsdk-2.0.5/inspursmsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.0.4/ism.py` & `inspursmsdk-2.0.5/ism.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     ISM_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inspursmsdk-2.0.4/setup.py` & `inspursmsdk-2.0.5/setup.py`

 * *Files identical despite different names*

