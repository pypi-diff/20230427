# Comparing `tmp/CollabConnector-0.1.1682611691.tar.gz` & `tmp/CollabConnector-0.1.1682611733.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CollabConnector-0.1.1682611691.tar", last modified: Thu Apr 27 16:08:22 2023, max compression
+gzip compressed data, was "CollabConnector-0.1.1682611733.tar", last modified: Thu Apr 27 16:09:03 2023, max compression
```

## Comparing `CollabConnector-0.1.1682611691.tar` & `CollabConnector-0.1.1682611733.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.558669 CollabConnector-0.1.1682611691/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1682611691/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-04-27 16:08:22.559301 CollabConnector-0.1.1682611691/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1682611691/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1682611691/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-04-27 16:08:22.562781 CollabConnector-0.1.1682611691/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.098200 CollabConnector-0.1.1682611691/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.122283 CollabConnector-0.1.1682611691/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.134113 CollabConnector-0.1.1682611691/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2582 2023-02-22 19:34:55.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.137828 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.139638 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10783 2023-02-22 19:35:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.141405 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/AXL.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.145276 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Add/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Add/Add.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Add/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.149001 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Do/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Do/Do.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Do/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.154739 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Get/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Get/Get.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Get/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.158395 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/List/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/List/List.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/List/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.160504 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Remove/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Remove/Remove.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Remove/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.165541 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Update/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Update/Update.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Update/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.107375 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.176019 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.203188 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.233187 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.259223 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.286602 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.346288 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.360511 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.439105 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.447775 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.467494 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.484200 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.505257 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.521590 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20618 2023-01-24 14:18:53.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13354 2023-04-27 16:07:31.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.524845 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.526325 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.527747 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.531333 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.532966 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2098 2023-02-22 19:35:33.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.534418 CollabConnector-0.1.1682611691/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15080 2023-02-22 19:34:48.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.535936 CollabConnector-0.1.1682611691/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3525 2023-02-22 19:35:10.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.537419 CollabConnector-0.1.1682611691/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1682611691/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1682611691/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.541000 CollabConnector-0.1.1682611691/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.544616 CollabConnector-0.1.1682611691/src/CollabConnector/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30949 2023-02-22 19:35:02.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.548174 CollabConnector-0.1.1682611691/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8550 2023-02-22 19:34:41.000000 CollabConnector-0.1.1682611691/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.557803 CollabConnector-0.1.1682611691/src/CollabConnector/Webex/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Webex/CallControl.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9267 2022-10-26 14:42:05.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Webex/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Webex/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     7728 2022-10-28 12:24:36.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611691/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1682611691/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:08:22.131193 CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-04-27 16:08:22.000000 CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4444 2023-04-27 16:08:22.000000 CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-04-27 16:08:22.000000 CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-04-27 16:08:22.000000 CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-04-27 16:08:22.000000 CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.359966 CollabConnector-0.1.1682611733/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1682611733/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-04-27 16:09:03.360554 CollabConnector-0.1.1682611733/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1682611733/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1682611733/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-04-27 16:09:03.362008 CollabConnector-0.1.1682611733/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.114640 CollabConnector-0.1.1682611733/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.133379 CollabConnector-0.1.1682611733/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.138313 CollabConnector-0.1.1682611733/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2582 2023-02-22 19:34:55.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.139798 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.141475 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10783 2023-02-22 19:35:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.143622 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/AXL.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.146225 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Add/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Add/Add.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Add/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.148178 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Do/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Do/Do.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Do/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.150771 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Get/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Get/Get.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Get/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.153268 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/List/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/List/List.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/List/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.155614 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Remove/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Remove/Remove.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Remove/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.158119 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Update/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Update/Update.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Update/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.122000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.163840 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.178837 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.195544 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.214036 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.230242 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.265225 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.270107 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.288290 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.293137 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.305738 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.316677 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.329459 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.339324 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20618 2023-01-24 14:18:53.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13353 2023-04-27 16:08:41.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.340747 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.342106 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.343636 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.345700 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.347158 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2098 2023-02-22 19:35:33.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.348573 CollabConnector-0.1.1682611733/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15080 2023-02-22 19:34:48.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.349992 CollabConnector-0.1.1682611733/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3525 2023-02-22 19:35:10.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.351439 CollabConnector-0.1.1682611733/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1682611733/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1682611733/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.352713 CollabConnector-0.1.1682611733/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.354116 CollabConnector-0.1.1682611733/src/CollabConnector/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30949 2023-02-22 19:35:02.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.355497 CollabConnector-0.1.1682611733/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8550 2023-02-22 19:34:41.000000 CollabConnector-0.1.1682611733/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.359111 CollabConnector-0.1.1682611733/src/CollabConnector/Webex/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Webex/CallControl.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9267 2022-10-26 14:42:05.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Webex/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Webex/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     7728 2022-10-28 12:24:36.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1682611733/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1682611733/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-04-27 16:09:03.136867 CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-04-27 16:09:03.000000 CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4444 2023-04-27 16:09:03.000000 CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-04-27 16:09:03.000000 CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-04-27 16:09:03.000000 CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-04-27 16:09:03.000000 CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `CollabConnector-0.1.1682611691/LICENSE` & `CollabConnector-0.1.1682611733/LICENSE`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/PKG-INFO` & `CollabConnector-0.1.1682611733/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1682611691
+Version: 0.1.1682611733
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1682611691/README.md` & `CollabConnector-0.1.1682611733/README.md`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/setup.cfg` & `CollabConnector-0.1.1682611733/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1682611691
+version = 0.1.1682611733
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CER/CER.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AST/AST.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/AXL.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Add/Add.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Add/Add.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Do/Do.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Do/Do.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Get/Get.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Get/Get.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/List/List.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/List/List.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Remove/Remove.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Remove/Remove.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/Update/Update.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/Update/Update.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CDR/CDR.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/CUCM.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/CUCM.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             return False
 
     # Function to query SQL via AXL API to CUCM
     def query(self, sql_statement):
         if self.version:
             version = self.version
         else:
-            version = "11.0"
+            version = "8.5"
         result_dict = []
         row_info = ["", None, None]
         newsql_statement = sql_statement
         while row_info[1] is None or int(row_info[1]) > len(result_dict):
             if re.search("select", sql_statement.lower()):
                 execute_sql = "executeSQLQuery"
             else:
```

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/DIME/DIME.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Logs/Logs.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Risport/Risport.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCM/UDS/UDS.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/CUCX/CUCX.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/Expressway/Expressway.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/IOS/IOS.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/PAWS/PAWS.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/Phone/Phone.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/UCCX/UCCX.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/Webex/CallControl.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/Webex/CallControl.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/Webex/ContactCenter.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/Webex/ContactCenter.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/Webex/OutputStyle.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/Webex/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector/Webex/Webex.py` & `CollabConnector-0.1.1682611733/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/PKG-INFO` & `CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1682611691
+Version: 0.1.1682611733
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1682611691/src/CollabConnector.egg-info/SOURCES.txt` & `CollabConnector-0.1.1682611733/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

