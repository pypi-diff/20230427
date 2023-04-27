# Comparing `tmp/pyPhases-1.1.8.tar.gz` & `tmp/pyPhases-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhases-1.1.8.tar", last modified: Thu Feb 16 11:56:36 2023, max compression
+gzip compressed data, was "pyPhases-1.1.9.tar", last modified: Tue Feb 21 07:20:39 2023, max compression
```

## Comparing `pyPhases-1.1.8.tar` & `pyPhases-1.1.9.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.169405 pyPhases-1.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-02-16 11:56:18.000000 pyPhases-1.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-02-16 11:56:18.000000 pyPhases-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4666 2023-02-16 11:56:36.169405 pyPhases-1.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4180 2023-02-16 11:56:18.000000 pyPhases-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.153404 pyPhases-1.1.8/pyPhases/
--rw-rw-rw-   0 root         (0) root         (0)     3045 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/Data.py
--rw-rw-rw-   0 root         (0) root         (0)     3189 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/Phase.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/PluginAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/Project.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-02-16 11:56:20.000000 pyPhases-1.1.8/pyPhases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.155404 pyPhases-1.1.8/pyPhases/decorator/
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/decorator/Decorator.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/decorator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.156404 pyPhases-1.1.8/pyPhases/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/exporter/DataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/exporter/PickleExporter.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.158404 pyPhases-1.1.8/pyPhases/test/
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/test/MockLogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/test/TestCase.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/test/TestCaseIntegration.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/test/TestRun.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.160404 pyPhases-1.1.8/pyPhases/util/
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/BatchProgress.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/EventBus.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/Logger.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/Optionizable.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1775 2023-02-16 11:56:18.000000 pyPhases-1.1.8/pyPhases/util/pdict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.154404 pyPhases-1.1.8/pyPhases.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4666 2023-02-16 11:56:36.000000 pyPhases-1.1.8/pyPhases.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1488 2023-02-16 11:56:36.000000 pyPhases-1.1.8/pyPhases.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 11:56:36.000000 pyPhases-1.1.8/pyPhases.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-16 11:56:36.000000 pyPhases-1.1.8/pyPhases.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-16 11:56:36.000000 pyPhases-1.1.8/pyPhases.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-16 11:56:18.000000 pyPhases-1.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-16 11:56:36.169405 pyPhases-1.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-02-16 11:56:20.000000 pyPhases-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.161404 pyPhases-1.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.162404 pyPhases-1.1.8/tests/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1932 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/test/test_BaseTest.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/test/test_IntegrationTest.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/test/test_TestRun.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/test_acceptance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.166405 pyPhases-1.1.8/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5184 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_BatchProgress.py
--rw-rw-rw-   0 root         (0) root         (0)     6054 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Data.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_DataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Decorator.py
--rw-rw-rw-   0 root         (0) root         (0)      964 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_EventBus.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Loggermock.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Optionizable.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Phase.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_PluginAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    16555 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_Project.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_csvlogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_exporter_pickleexporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/unit/test_pdict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 11:56:36.168405 pyPhases-1.1.8/tests/util/
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/util/ExporterTestHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/util/PhaseGenerator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-16 11:56:18.000000 pyPhases-1.1.8/tests/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.377918 pyPhases-1.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-02-21 07:20:22.000000 pyPhases-1.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-02-21 07:20:22.000000 pyPhases-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-02-21 07:20:39.377918 pyPhases-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4180 2023-02-21 07:20:22.000000 pyPhases-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.360916 pyPhases-1.1.9/pyPhases/
+-rw-rw-rw-   0 root         (0) root         (0)     3045 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/Data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/Phase.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/PluginAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-02-21 07:20:23.000000 pyPhases-1.1.9/pyPhases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.362916 pyPhases-1.1.9/pyPhases/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/decorator/Decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/decorator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.363916 pyPhases-1.1.9/pyPhases/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/exporter/DataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/exporter/PickleExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.365917 pyPhases-1.1.9/pyPhases/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/MockLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/Mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/TestCase.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/TestCaseIntegration.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/TestRun.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.367917 pyPhases-1.1.9/pyPhases/util/
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/BatchProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/EventBus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/Optionizable.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/pdict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.361916 pyPhases-1.1.9/pyPhases.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-21 07:20:22.000000 pyPhases-1.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-21 07:20:39.377918 pyPhases-1.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-02-21 07:20:23.000000 pyPhases-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.368917 pyPhases-1.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.370917 pyPhases-1.1.9/tests/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_BaseTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_IntegrationTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_Mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_TestRun.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test_acceptance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.375917 pyPhases-1.1.9/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_BatchProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)     6054 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_DataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)      964 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_EventBus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Loggermock.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Optionizable.py
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Phase.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_PluginAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    16555 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3838 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_csvlogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_exporter_pickleexporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_pdict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.376917 pyPhases-1.1.9/tests/util/
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/util/ExporterTestHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/util/PhaseGenerator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/util/__init__.py
```

### Comparing `pyPhases-1.1.8/LICENSE` & `pyPhases-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/PKG-INFO` & `pyPhases-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhases
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt/pyPhases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhases-1.1.8/README.md` & `pyPhases-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/Data.py` & `pyPhases-1.1.9/pyPhases/Data.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/Phase.py` & `pyPhases-1.1.9/pyPhases/Phase.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/Project.py` & `pyPhases-1.1.9/pyPhases/Project.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/decorator/Decorator.py` & `pyPhases-1.1.9/pyPhases/decorator/Decorator.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/exporter/DataExporter.py` & `pyPhases-1.1.9/pyPhases/exporter/DataExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/exporter/PickleExporter.py` & `pyPhases-1.1.9/pyPhases/exporter/PickleExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/test/MockLogger.py` & `pyPhases-1.1.9/pyPhases/test/MockLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/test/TestCase.py` & `pyPhases-1.1.9/pyPhases/test/TestCase.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/test/TestRun.py` & `pyPhases-1.1.9/pyPhases/test/TestRun.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/util/BatchProgress.py` & `pyPhases-1.1.9/pyPhases/util/BatchProgress.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/util/CSVLogger.py` & `pyPhases-1.1.9/pyPhases/util/CSVLogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,9 +41,9 @@
     def getRowsAsDict(self):
         return self.getRowsReader(csv.DictReader, removeHeader=False)
 
     def getRowsAsList(self):
         return self.getRowsReader(csv.reader)
 
     def getLastRow(self):
-        rows = self.getRows()
+        rows = self.getRowsAsDict()
         return rows[-1]
```

### Comparing `pyPhases-1.1.8/pyPhases/util/EventBus.py` & `pyPhases-1.1.9/pyPhases/util/EventBus.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/util/Logger.py` & `pyPhases-1.1.9/pyPhases/util/Logger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/util/Optionizable.py` & `pyPhases-1.1.9/pyPhases/util/Optionizable.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases/util/pdict.py` & `pyPhases-1.1.9/pyPhases/util/pdict.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/pyPhases.egg-info/PKG-INFO` & `pyPhases-1.1.9/pyPhases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhases
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt/pyPhases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhases-1.1.8/pyPhases.egg-info/SOURCES.txt` & `pyPhases-1.1.9/pyPhases.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pyPhases.egg-info/top_level.txt
 pyPhases/decorator/Decorator.py
 pyPhases/decorator/__init__.py
 pyPhases/exporter/DataExporter.py
 pyPhases/exporter/PickleExporter.py
 pyPhases/exporter/__init__.py
 pyPhases/test/MockLogger.py
+pyPhases/test/Mocks.py
 pyPhases/test/TestCase.py
 pyPhases/test/TestCaseIntegration.py
 pyPhases/test/TestRun.py
 pyPhases/test/__init__.py
 pyPhases/util/BatchProgress.py
 pyPhases/util/CSVLogger.py
 pyPhases/util/EventBus.py
@@ -31,14 +32,15 @@
 pyPhases/util/__init__.py
 pyPhases/util/pdict.py
 tests/__init__.py
 tests/test_acceptance.py
 tests/test/__init__.py
 tests/test/test_BaseTest.py
 tests/test/test_IntegrationTest.py
+tests/test/test_Mocks.py
 tests/test/test_TestRun.py
 tests/unit/__init__.py
 tests/unit/test_BatchProgress.py
 tests/unit/test_Data.py
 tests/unit/test_DataExporter.py
 tests/unit/test_Decorator.py
 tests/unit/test_EventBus.py
```

### Comparing `pyPhases-1.1.8/setup.py` & `pyPhases-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhases",
-    version="v1.1.8"[1:],
+    version="v1.1.9"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt/pyPhases",
     packages=setuptools.find_packages(exclude="tests"),
```

### Comparing `pyPhases-1.1.8/tests/test/test_BaseTest.py` & `pyPhases-1.1.9/tests/test/test_BaseTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# from pyPhases.exporter.ObjectExporter import ObjectExporter
-# import pyPhases
-
-
 from pyPhases.Project import ConfigNotFoundException
-from tests.util.PhaseGenerator import PhaseGenerator
 from pyPhases.test.TestCase import TestCase
+from tests.util.PhaseGenerator import PhaseGenerator
 
 
 class TestBaseTest(TestCase):
     phase = TestCase.project.phases[0]
     isPrepared = False
 
     def config(self):
         return {"option1": 1, "c1": "o"}
 
-    def defaultConfig(self):
-        return {**PhaseGenerator.completeConfig(), **self.config()}
-
     def testSetProject(self):
         self.assertIsNotNone(self.project)
         self.assertEqual("testProject", self.project.name)
 
     def testConfig(self):
         self.assertEqual(self.getConfig("p1"), 1)
         self.assertEqual(self.getConfig("p2"), 2)
```

### Comparing `pyPhases-1.1.8/tests/test/test_IntegrationTest.py` & `pyPhases-1.1.9/tests/test/test_IntegrationTest.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/test/test_TestRun.py` & `pyPhases-1.1.9/tests/test/test_TestRun.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_BatchProgress.py` & `pyPhases-1.1.9/tests/unit/test_BatchProgress.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_Data.py` & `pyPhases-1.1.9/tests/unit/test_Data.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_DataExporter.py` & `pyPhases-1.1.9/tests/unit/test_DataExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_EventBus.py` & `pyPhases-1.1.9/tests/unit/test_EventBus.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_Logger.py` & `pyPhases-1.1.9/tests/unit/test_Logger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_Loggermock.py` & `pyPhases-1.1.9/tests/unit/test_Loggermock.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_Optionizable.py` & `pyPhases-1.1.9/tests/unit/test_Optionizable.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_Phase.py` & `pyPhases-1.1.9/tests/unit/test_Phase.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_PluginAdapter.py` & `pyPhases-1.1.9/tests/unit/test_PluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_Project.py` & `pyPhases-1.1.9/tests/unit/test_Project.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_csvlogger.py` & `pyPhases-1.1.9/tests/unit/test_csvlogger.py`

 * *Files 14% similar despite different names*

```diff
@@ -101,7 +101,22 @@
         self.assertListEqual(rows[0], list(row.values()))
         self.assertListEqual(rows[1], list(row2.values()))
 
     def test_getRows_empty(self):
         rows = self.logger.getRowsAsList()
         self.assertEqual(len(rows), 0)
         self.assertEqual(rows, [])
+
+    def test_getLastRow(self):
+        self.logger.cleanCsv()
+
+        row = {"col1": "val1", "col2": "val2"}
+        self.logger.addCsvRow(row)
+
+        lastRow = self.logger.getLastRow()
+        self.assertDictEqual(lastRow, row)
+
+        # Add another row and check that it was added
+        row2 = {"col1": "val3", "col2": "val4"}
+        self.logger.addCsvRow(row2)
+        lastRow = self.logger.getLastRow()
+        self.assertDictEqual(lastRow, row2)
```

### Comparing `pyPhases-1.1.8/tests/unit/test_exporter_pickleexporter.py` & `pyPhases-1.1.9/tests/unit/test_exporter_pickleexporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/unit/test_pdict.py` & `pyPhases-1.1.9/tests/unit/test_pdict.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/util/ExporterTestHelper.py` & `pyPhases-1.1.9/tests/util/ExporterTestHelper.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.8/tests/util/PhaseGenerator.py` & `pyPhases-1.1.9/tests/util/PhaseGenerator.py`

 * *Files identical despite different names*

