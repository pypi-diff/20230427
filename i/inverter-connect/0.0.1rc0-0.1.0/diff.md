# Comparing `tmp/inverter-connect-0.0.1rc0.tar.gz` & `tmp/inverter-connect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.0.1rc0.tar", last modified: Fri Apr 21 07:05:50 2023, max compression
+gzip compressed data, was "inverter-connect-0.1.0.tar", last modified: Thu Apr 27 17:09:26 2023, max compression
```

## Comparing `inverter-connect-0.0.1rc0.tar` & `inverter-connect-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,68 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.0.1rc0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.0.1rc0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.0.1rc0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.0.1rc0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     8702 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     8285 2023-04-21 06:59:46.000000 inverter-connect-0.0.1rc0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      151 2023-04-21 07:01:32.000000 inverter-connect-0.0.1rc0/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    11354 2023-04-21 06:40:55.000000 inverter-connect-0.0.1rc0/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7905 2023-04-21 07:03:09.000000 inverter-connect-0.0.1rc0/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      136 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2885 2023-04-20 19:38:44.000000 inverter-connect-0.0.1rc0/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2367 2023-04-21 07:03:09.000000 inverter-connect-0.0.1rc0/inverter/definitions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      239 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-20 19:23:21.000000 inverter-connect-0.0.1rc0/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     1369 2023-04-20 19:23:05.000000 inverter-connect-0.0.1rc0/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.0.1rc0/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.0.1rc0/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2135 2023-04-21 06:50:23.000000 inverter-connect-0.0.1rc0/inverter/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.0.1rc0/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-21 07:02:38.000000 inverter-connect-0.0.1rc0/inverter/utilities/modbus_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     8702 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      928 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      249 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-21 07:05:50.000000 inverter-connect-0.0.1rc0/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4675 2023-04-21 06:59:46.000000 inverter-connect-0.0.1rc0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    50878 2023-04-19 06:56:45.000000 inverter-connect-0.0.1rc0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     2307 2023-04-19 06:56:45.000000 inverter-connect-0.0.1rc0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-21 07:05:50.837658 inverter-connect-0.0.1rc0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.1.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.1.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.377880 inverter-connect-0.1.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-19 06:56:31.000000 inverter-connect-0.1.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.1.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     9457 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     9043 2023-04-27 16:51:26.000000 inverter-connect-0.1.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3047 2023-04-20 19:23:05.000000 inverter-connect-0.1.0/cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.377880 inverter-connect-0.1.0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-04-27 16:57:57.000000 inverter-connect-0.1.0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.1.0/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3753 2023-04-27 16:10:03.000000 inverter-connect-0.1.0/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    17570 2023-04-27 17:05:44.000000 inverter-connect-0.1.0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)      276 2023-04-23 15:55:16.000000 inverter-connect-0.1.0/inverter/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8893 2023-04-27 16:18:50.000000 inverter-connect-0.1.0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.1.0/inverter/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.1.0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.1.0/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.1.0/inverter/exceptions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/test_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/tests/test_doctests.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.1.0/inverter/mqtt4homeassistant/utilities/string_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2460 2023-04-24 09:00:54.000000 inverter-connect-0.1.0/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.1.0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.1.0/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.1.0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.1.0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.1.0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2314 2023-04-20 19:36:47.000000 inverter-connect-0.1.0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2135 2023-04-21 06:50:23.000000 inverter-connect-0.1.0/inverter/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.1.0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      458 2023-04-27 17:06:47.000000 inverter-connect-0.1.0/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.1.0/inverter/utilities/credentials.py
+-rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.1.0/inverter/utilities/log_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.1.0/inverter/utilities/modbus_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     9457 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1544 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       52 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      259 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-04-27 17:09:26.000000 inverter-connect-0.1.0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4731 2023-04-27 15:42:09.000000 inverter-connect-0.1.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    50591 2023-04-27 17:07:50.000000 inverter-connect-0.1.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-04-27 17:07:31.000000 inverter-connect-0.1.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-04-27 17:09:26.381880 inverter-connect-0.1.0/setup.cfg
```

### Comparing `inverter-connect-0.0.1rc0/.github/workflows/tests.yml` & `inverter-connect-0.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1rc0/PKG-INFO` & `inverter-connect-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.0.1rc0
+Version: 0.1.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # inverter
 
-[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect-connect/actions/workflows/tests.yml)
+[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/LICENSE)
+[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 ## screenshots
 
@@ -56,22 +56,28 @@
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
 │ coverage                    Run and show coverage.                                               │
+│ debug-settings              Display (anonymized) MQTT server username and password               │
 │ fix-code-style              Fix code style of all inverter source code files via darker          │
 │ install                     Run pip-sync and install 'inverter' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ print-at-commands           Print one or more AT command values from Inverter.                   │
 │ print-values                Print all known register values from Inverter, e.g.:                 │
 │ publish                     Build and upload this project to PyPi                                │
+│ publish-loop                Publish current data via MQTT (endless loop)                         │
+│ read-register               Read register(s) from the inverter                                   │
 │ safety                      Run safety check against current requirements files                  │
+│ set-time                    Set current date time in the inverter device.                        │
+│ store-settings              Store MQTT server settings.                                          │
 │ test                        Run unittests                                                        │
+│ test-mqtt-connection        Test connection to MQTT Server                                       │
 │ tox                         Run tox                                                              │
 │ update                      Update "requirements*.txt" dependencies files                        │
 │ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
@@ -137,7 +143,10 @@
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
+## various links
+
+* Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.0.1rc0/README.md` & `inverter-connect-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # inverter
 
-[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect-connect/actions/workflows/tests.yml)
+[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/LICENSE)
+[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 ## screenshots
 
@@ -44,22 +44,28 @@
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
 │ coverage                    Run and show coverage.                                               │
+│ debug-settings              Display (anonymized) MQTT server username and password               │
 │ fix-code-style              Fix code style of all inverter source code files via darker          │
 │ install                     Run pip-sync and install 'inverter' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ print-at-commands           Print one or more AT command values from Inverter.                   │
 │ print-values                Print all known register values from Inverter, e.g.:                 │
 │ publish                     Build and upload this project to PyPi                                │
+│ publish-loop                Publish current data via MQTT (endless loop)                         │
+│ read-register               Read register(s) from the inverter                                   │
 │ safety                      Run safety check against current requirements files                  │
+│ set-time                    Set current date time in the inverter device.                        │
+│ store-settings              Store MQTT server settings.                                          │
 │ test                        Run unittests                                                        │
+│ test-mqtt-connection        Test connection to MQTT Server                                       │
 │ tox                         Run tox                                                              │
 │ update                      Update "requirements*.txt" dependencies files                        │
 │ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
@@ -125,7 +131,10 @@
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
+## various links
+
+* Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.0.1rc0/cli.py` & `inverter-connect-0.1.0/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1rc0/inverter/.github/workflows/tests.yml` & `inverter-connect-0.1.0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1rc0/inverter/connection.py` & `inverter-connect-0.1.0/inverter/connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,22 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 import socket
 import time
 
+from inverter.config import Config
+from inverter.constants import AT_READ_FUNC_NUMBER, AT_WRITE_FUNC_NUMBER, ERROR_STR_NO_DATA
 from inverter.definitions import Parameter
+from inverter.exceptions import CrcError, ModbusNoData, ModbusNoHexData, ParseModbusValueError, ReadTimeout
 
 
 logger = logging.getLogger(__name__)
 
-ERROR_STR_NO_DATA = 'no data'
-
-
-class ModbusNoData(KeyError):
-    """
-    Modbus register value is: 'no data' == ERROR_STR_NO_DATA
-    """
-
-    pass
-
-
-@dataclasses.dataclass
-class Config:
-    host: str
-    port: int = 48899
-    pause: float = 0.1
-    timeout: int = 5
-    debug: bool = False
-    init_cmd: bytes = b'WIFIKIT-214028-READ'
-
 
 @dataclasses.dataclass
 class InverterInfo:
     ip: str
     mac: str
     serial: int
 
@@ -65,16 +48,16 @@
     try:
         parsed_value = parser_func(
             data_hex=data_hex,
             scale=parameter.scale,
             offset=parameter.offset,
             lookup=parameter.lookup,
         )
-    except ValueError as err:
-        raise ValueError(f'Parser error with {response=} {parameter=}: {err}')
+    except (ValueError, AssertionError) as err:
+        raise ParseModbusValueError(f'Parser error with {response=} {parameter=}: {err}')
     logger.debug(f'{parsed_value=}')
     result = ModbusReadResult(parameter=parameter, response=response, parsed_value=parsed_value)
     logger.debug('%s', result)
     return result
 
 
 def modbus_crc(data):
@@ -103,20 +86,22 @@
     request_data.extend(start_register.to_bytes(2, 'big'))
     request_data.extend(length.to_bytes(2, 'big'))
     crc = modbus_crc(request_data)
     request_data.extend(crc.to_bytes(2, 'little'))
     return request_data
 
 
-def parameter2modbus_at_command(start_register: int, length: int) -> str:
+def parameter2modbus_at_command(start_register: int, length: int, modbus_function: int) -> str:
     """
-    >>> parameter2modbus_at_command(start_register=0x0056, length=1)
+    >>> parameter2modbus_at_command(start_register=0x0056, length=1, modbus_function=3)
     'INVDATA=8,010300560001641a'
     """
-    request_data = get_business_field(start_register=start_register, length=length, slave_id=1, modbus_function=3)
+    request_data = get_business_field(
+        start_register=start_register, length=length, slave_id=1, modbus_function=modbus_function
+    )
     cmd_length = len(request_data)
     at_command = f'INVDATA={cmd_length},{request_data.hex()}'
     return at_command
 
 
 def parse_response(data: bytes) -> RawModBusResponse:
     """
@@ -144,23 +129,23 @@
     if data == ERROR_STR_NO_DATA:
         raise ModbusNoData
 
     try:
         data_bytes = bytes.fromhex(data)
     except ValueError as err:
         logger.warning(f'Value error with {data=}: {err}')
-        raise ModbusNoData
+        raise ModbusNoHexData(data=data)
 
     logger.debug(f'{data_bytes=}')
 
     calculated_crc = modbus_crc(data_bytes[:-2])
     calculated_crc = calculated_crc.to_bytes(2, 'little')
     got_crc = data_bytes[-2:]
     if got_crc != calculated_crc:
-        raise AssertionError(f'{got_crc.hex()=} {calculated_crc.hex()=} from {data=}')
+        raise CrcError(f'{got_crc.hex()=} {calculated_crc.hex()=} from {data=}')
 
     length = data_bytes[2]
     data = data_bytes[3:-2]
     assert len(data) == length, f'Data is not {length=}: {data=}'
 
     result = ModbusResponse(
         slave_id=data_bytes[0],
@@ -203,15 +188,15 @@
 
         if self.config.debug:
             print('recv', end='...', flush=True)
 
         try:
             data = self.sock.recv(buffer_size)
         except TimeoutError as err:
-            raise TimeoutError(f'Get no response from {self.config.host}: {err}')
+            raise ReadTimeout(f'Get no response from {self.config.host}: {err}')
         if self.config.debug:
             print(f'{data}', flush=True)
 
         return data
 
     def at_command(self, command: str, buffer_size=1024):
         assert not command.startswith('AT+'), f'Remove "AT+" prefix from: {command=}'
@@ -242,26 +227,56 @@
     def init_inventer(self):
         data = self.recv_command(command=self.config.init_cmd)
         self.send(command=b'+ok')
         data = data.decode()
         data = data.split(',')
         return InverterInfo(ip=data[0], mac=data[1], serial=int(data[2]))
 
-    def read(self, *, parameter: Parameter) -> ModbusReadResult:
+    def read(self, *, start_register: int, length: int) -> ModbusResponse:
         if self.config.debug:
-            print(parameter)
-        command = parameter2modbus_at_command(start_register=parameter.start_register, length=parameter.length)
+            print(f'Read {length} value(s) from {start_register=!r}')
+
+        command = parameter2modbus_at_command(
+            start_register=start_register,
+            length=length,
+            modbus_function=AT_READ_FUNC_NUMBER,
+        )
         if self.config.debug:
             print(f'AT command: {command}')
 
         data: str = self.cleaned_at_command(command=command)
-
         try:
             response: ModbusResponse = parse_modbus_response(data=data)
-        except ValueError as err:
-            raise ValueError(f'parse error: {data=}: {err}')
+        except ParseModbusValueError as err:
+            raise ParseModbusValueError(f'parse error: {data=}: {err}')
+        return response
+
+    def read_paremeter(self, *, parameter: Parameter) -> ModbusReadResult:
+        if self.config.debug:
+            print(parameter)
+
+        try:
+            response: ModbusResponse = self.read(
+                start_register=parameter.start_register,
+                length=parameter.length,
+            )
         except ModbusNoData:
             # Modbus register value is: b'no data'
             result = ModbusReadResult(parameter=parameter, parsed_value='no data')
         else:
             result: ModbusReadResult = make_modbus_result(response=response, parameter=parameter)
         return result
+
+    def write(self, *, address: int, values: list[int, ...]):
+        if self.config.debug:
+            print(f'Write {" ".join(hex(value) for value in values)} to {hex(address)}')
+
+        command = parameter2modbus_at_command(
+            start_register=address,
+            length=len(values),
+            modbus_function=AT_WRITE_FUNC_NUMBER,
+        )
+        if self.config.debug:
+            print(f'AT command: {command}')
+
+        data: str = self.cleaned_at_command(command=command)
+        return data
```

### Comparing `inverter-connect-0.0.1rc0/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.1.0/inverter/definitions/deye_2mppt.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
       scale: 0.1
       rule: 1
       registers: [0x006F]
       icon: 'mdi:solar-power'
 
     - name: "PV1 Current"
       class: "current"
+      state_class: "measurement"
       uom: "A"
       scale: 0.1
       rule: 1
       registers: [0x006E]
       icon: 'mdi:solar-power'
 
     - name: "PV2 Current"
```

### Comparing `inverter-connect-0.0.1rc0/inverter/definitions.py` & `inverter-connect-0.1.0/inverter/definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from __future__ import annotations
 
 import dataclasses
+from collections.abc import Iterable
+from typing import Callable
 
 import yaml
 from bx_py_utils.dict_utils import pluck
 from bx_py_utils.path import assert_is_file
 
 from inverter.constants import BASE_PATH
 from inverter.utilities.modbus_converter import debug_converter, parse_number, parse_string, parse_swapped_number
 
 
 @dataclasses.dataclass
 class Parameter:
     start_register: int
     length: int
     group: str
-    name: str
-    unit: str
-    scale: float | int
-    parser: callable
+    name: str  # e.g.: "PV1 Voltage" / "PV1 Current" / "Daily Production" etc.
+    device_class: str  # e.g.: "voltage" / "current" / "energy" etc.
+    state_class: str | None  # e.g.: "measurement" / "total" / "total_increasing" etc.
+    unit: str  # e.g.: "V" / "A" / "kWh" etc.
+    scale: float | int  # e.g.: 1 / 0.1
+    parser: Callable
     offset: int | None = None
     lookup: dict | None = None
 
 
 rule2converter = {
     1: parse_number,
     3: parse_swapped_number,
@@ -42,15 +46,15 @@
     """
     >>> convert_lookup([{'key': 2, 'value': 'Normal'},{'key': 3, 'value': 'Warning'}])
     {2: 'Normal', 3: 'Warning'}
     """
     return {entry['key']: entry['value'] for entry in raw_lookup}
 
 
-def get_parameter(yaml_filename, debug=False):
+def get_parameter(yaml_filename, debug=False) -> Iterable[Parameter]:
     data = get_definition(yaml_filename)
     parameters = []
     for group_data in data:
         group_name = group_data['group']
         for item in group_data['items']:
             # example = {
             #     'name': 'PV1 Voltage',
@@ -61,24 +65,25 @@
             #     'rule': 1,
             #     'registers': [109],
             #     'icon': 'mdi:solar-power',
             # }
             rule = item['rule']
             registers = item['registers']
 
-            parameter_kwargs = pluck(item, keys=['name', 'scale', 'offset'])
+            parameter_kwargs = pluck(item, keys=['name', 'state_class', 'scale', 'offset'])
             if lookup := item.get('lookup'):
                 lookup = convert_lookup(lookup)
 
             converter_func = rule2converter.get(rule, debug_converter)
 
             parameter = Parameter(
                 start_register=registers[0],
                 length=len(registers),
                 group=group_name,
                 lookup=lookup,
                 unit=item['uom'],
                 parser=converter_func,
+                device_class=item['class'],
                 **parameter_kwargs,
             )
             parameters.append(parameter)
     return parameters
```

### Comparing `inverter-connect-0.0.1rc0/inverter/tests/test_connect.py` & `inverter-connect-0.1.0/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1rc0/inverter/tests/test_definitions.py` & `inverter-connect-0.1.0/inverter/tests/test_definitions.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         self.assertEqual(
             example,
             Parameter(
                 start_register=109,
                 length=1,
                 group='solar',
                 name='PV1 Voltage',
+                device_class='voltage',
+                state_class='measurement',
                 unit='V',
                 scale=0.1,
                 parser=example.parser,
                 offset=None,
                 lookup=None,
             ),
         )
```

### Comparing `inverter-connect-0.0.1rc0/inverter/tests/test_project_setup.py` & `inverter-connect-0.1.0/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1rc0/inverter/tests/test_readme.py` & `inverter-connect-0.1.0/inverter/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.0.1rc0/inverter/utilities/modbus_converter.py` & `inverter-connect-0.1.0/inverter/utilities/modbus_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         number = number - offset
         logger.debug(f'{number=}')
 
     logger.debug(f'{number=} {scale=}')
     number = number * scale
     logger.debug(f'{number=}')
 
-    result = round(number, 1)
+    result = round(number, 2)
     logger.debug(f'{result=}')
     return result
 
 
 def parse_number(*, data_hex: str, scale: int | float, offset: int = None, lookup: dict = None):
     """
     >>> parse_number(data_hex='0938', scale=0.1)
```

### Comparing `inverter-connect-0.0.1rc0/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.1.0/inverter_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.0.1rc0
+Version: 0.1.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # inverter
 
-[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect-connect/actions/workflows/tests.yml)
+[![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/pyproject.toml)
-[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect-connect/blob/main/LICENSE)
+[![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
+[![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
 
 Get information from Deye Microinverter
 
 The whole thing is just a learning exercise for now. We will see.
 
 ## screenshots
 
@@ -56,22 +56,28 @@
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
 │ coverage                    Run and show coverage.                                               │
+│ debug-settings              Display (anonymized) MQTT server username and password               │
 │ fix-code-style              Fix code style of all inverter source code files via darker          │
 │ install                     Run pip-sync and install 'inverter' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ print-at-commands           Print one or more AT command values from Inverter.                   │
 │ print-values                Print all known register values from Inverter, e.g.:                 │
 │ publish                     Build and upload this project to PyPi                                │
+│ publish-loop                Publish current data via MQTT (endless loop)                         │
+│ read-register               Read register(s) from the inverter                                   │
 │ safety                      Run safety check against current requirements files                  │
+│ set-time                    Set current date time in the inverter device.                        │
+│ store-settings              Store MQTT server settings.                                          │
 │ test                        Run unittests                                                        │
+│ test-mqtt-connection        Test connection to MQTT Server                                       │
 │ tox                         Run tox                                                              │
 │ update                      Update "requirements*.txt" dependencies files                        │
 │ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
@@ -137,7 +143,10 @@
 * https://github.com/StephanJoubert/home_assistant_solarman
 
 The included definitions yaml files are from:
 
 https://github.com/StephanJoubert/home_assistant_solarman/tree/main/custom_components/solarman/inverter_definitions
 
 
+## various links
+
+* Discussion: https://www.photovoltaikforum.com/thread/201065-inverter-connect-daten-vom-deye-wechselrichter-per-python-abrufen/ (de)
```

### Comparing `inverter-connect-0.0.1rc0/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.1.0/inverter_connect.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,28 +8,45 @@
 requirements.txt
 .github/workflows/tests.yml
 inverter/.editorconfig
 inverter/.flake8
 inverter/.gitignore
 inverter/__init__.py
 inverter/__main__.py
+inverter/api.py
+inverter/config.py
 inverter/connection.py
 inverter/constants.py
 inverter/definitions.py
+inverter/exceptions.py
+inverter/publish_loop.py
 inverter/.github/workflows/tests.yml
 inverter/cli/__init__.py
 inverter/cli/cli_app.py
 inverter/definitions/deye_2mppt.yaml
+inverter/mqtt4homeassistant/__init__.py
+inverter/mqtt4homeassistant/converter.py
+inverter/mqtt4homeassistant/data_classes.py
+inverter/mqtt4homeassistant/mqtt.py
+inverter/mqtt4homeassistant/tests/__init__.py
+inverter/mqtt4homeassistant/tests/test_converter.py
+inverter/mqtt4homeassistant/tests/test_doctests.py
+inverter/mqtt4homeassistant/utilities/__init__.py
+inverter/mqtt4homeassistant/utilities/string_utils.py
 inverter/tests/__init__.py
+inverter/tests/test_api.py
 inverter/tests/test_connect.py
 inverter/tests/test_definitions.py
 inverter/tests/test_doctests.py
 inverter/tests/test_project_setup.py
 inverter/tests/test_readme.py
 inverter/utilities/__init__.py
+inverter/utilities/cli.py
+inverter/utilities/credentials.py
+inverter/utilities/log_setup.py
 inverter/utilities/modbus_converter.py
 inverter_connect.egg-info/PKG-INFO
 inverter_connect.egg-info/SOURCES.txt
 inverter_connect.egg-info/dependency_links.txt
 inverter_connect.egg-info/entry_points.txt
 inverter_connect.egg-info/requires.txt
 inverter_connect.egg-info/top_level.txt
```

### Comparing `inverter-connect-0.0.1rc0/pyproject.toml` & `inverter-connect-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'inverter-connect@jensdiemer.de'}
 ]
 requires-python = ">=3.9,<4"
 dependencies = [
+    "paho-mqtt",  # https://pypi.org/project/paho-mqtt/
     "pyyaml",  # https://github.com/yaml/pyyaml
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
 ]
 [project.optional-dependencies]
```

### Comparing `inverter-connect-0.0.1rc0/requirements.dev.txt` & `inverter-connect-0.1.0/requirements.dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 astor==0.8.1 \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
     --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
     # via flynt
 autopep8==2.0.2 \
     --hash=sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1 \
     --hash=sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
 black==23.3.0 \
     --hash=sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5 \
     --hash=sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915 \
@@ -55,15 +55,15 @@
     --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
     --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
     # via pip-tools
 bx-py-utils==80 \
     --hash=sha256:34c4f5e4e1199014a83139aa4285a85f84274a982f9a9a8eae056fd9848a42f7 \
     --hash=sha256:59f3d641c516fdf75d47ea86cd84fe6405d07fc7761074dcbbb967b6962dcc09
     # via
-    #   inverter (pyproject.toml)
+    #   inverter-connect (pyproject.toml)
     #   manageprojects
 cachetools==5.3.0 \
     --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
     --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
     # via tox
 certifi==2022.12.7 \
     --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
@@ -220,23 +220,23 @@
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via
     #   black
     #   cookiecutter
-    #   inverter (pyproject.toml)
+    #   inverter-connect (pyproject.toml)
     #   manageprojects
     #   pip-tools
     #   rich-click
     #   safety
 codespell==2.2.4 \
     --hash=sha256:0b4620473c257d9cde1ff8998b26b2bb209a35c2b7489f5dc3436024298ce83a \
     --hash=sha256:7d984b8130108e6f82524b7d09f8b7bf2fb1e398c5d4b37d9e2bd310145b3e29
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
 cookiecutter==2.1.1 \
     --hash=sha256:9f3ab027cec4f70916e28f03470bdb41e637a3ad354b4d65c765d93aad160022 \
     --hash=sha256:f3982be8d9c53dac1261864013fdec7f83afd2e42ede6f6dd069c5e149c540d5
@@ -289,15 +289,15 @@
     --hash=sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4 \
     --hash=sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22 \
     --hash=sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd \
     --hash=sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1 \
     --hash=sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910 \
     --hash=sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859 \
     --hash=sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 cryptography==40.0.2 \
     --hash=sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440 \
     --hash=sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288 \
     --hash=sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b \
     --hash=sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958 \
     --hash=sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b \
     --hash=sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d \
@@ -314,15 +314,15 @@
     --hash=sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99 \
     --hash=sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e \
     --hash=sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9
     # via secretstorage
 darker[color,flynt,isort]==1.7.1 \
     --hash=sha256:cf4173be4ad2982e5b2ebab7e08bd0d27173f2459ec1b1cf66aec9290da80cce \
     --hash=sha256:d72126418194871aeaf1e8aa620ad06edc5472848bef71c4d393c22b65571878
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
 docutils==0.19 \
     --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
     --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
@@ -330,36 +330,36 @@
 dparse==0.6.2 \
     --hash=sha256:8097076f1dd26c377f30d4745e6ec18fef42f3bf493933b842ac5bafad8c345f \
     --hash=sha256:d45255bda21f998bc7ddf2afd5e62505ba6134756ba2d42a84c56b0826614dfe
     # via safety
 editorconfig==0.12.3 \
     --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
     --hash=sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1
-    # via inverter (pyproject.toml)
-filelock==3.11.0 \
-    --hash=sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37 \
-    --hash=sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318
+    # via inverter-connect (pyproject.toml)
+filelock==3.12.0 \
+    --hash=sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9 \
+    --hash=sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0 \
     --hash=sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7 \
     --hash=sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 flynt==0.77 \
     --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
     --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
     # via darker
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
-importlib-metadata==6.4.1 \
-    --hash=sha256:63ace321e24167d12fbb176b6015f4dbe06868c54a2af4f15849586afb9027fd \
-    --hash=sha256:eb1a7933041f0f85c94cd130258df3fb0dec060ad8c1c9318892ef4192c47ce1
+importlib-metadata==6.6.0 \
+    --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
+    --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
     # via
     #   keyring
     #   twine
 isort==5.12.0 \
     --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
     --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
     # via darker
@@ -386,15 +386,15 @@
 keyring==23.13.1 \
     --hash=sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd \
     --hash=sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678
     # via twine
 manageprojects==0.9.10 \
     --hash=sha256:5f6aac8e660cc8bc72548afbc300be8d3096f4afd715e1549a4bebedba105c75 \
     --hash=sha256:be59603525d1f27519bd65717d5dcfe4d81eb75c34df71bb86a3fc4fbe15f0b5
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 markdown-it-py==2.2.0 \
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via rich
 markupsafe==2.1.2 \
     --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
     --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
@@ -482,15 +482,15 @@
     --hash=sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950 \
     --hash=sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937 \
     --hash=sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394 \
     --hash=sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6 \
     --hash=sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602 \
     --hash=sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1 \
     --hash=sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
 packaging==23.1 \
@@ -499,29 +499,32 @@
     # via
     #   black
     #   build
     #   dparse
     #   pyproject-api
     #   safety
     #   tox
+paho-mqtt==1.6.1 \
+    --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
+    # via inverter-connect (pyproject.toml)
 pathspec==0.11.1 \
     --hash=sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687 \
     --hash=sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293
     # via black
 pip-tools==6.13.0 \
     --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
     --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 pkginfo==1.9.6 \
     --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
     --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
     # via twine
-platformdirs==3.2.0 \
-    --hash=sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08 \
-    --hash=sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e
+platformdirs==3.5.0 \
+    --hash=sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4 \
+    --hash=sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335
     # via
     #   black
     #   tox
     #   virtualenv
 pluggy==1.0.0 \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
@@ -537,50 +540,42 @@
     --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
     # via cffi
 pyflakes==3.0.1 \
     --hash=sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf \
     --hash=sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd
     # via
     #   flake8
-    #   inverter (pyproject.toml)
-pygments==2.15.0 \
-    --hash=sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094 \
-    --hash=sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500
+    #   inverter-connect (pyproject.toml)
+pygments==2.15.1 \
+    --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
+    --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via
     #   darker
     #   readme-renderer
     #   rich
 pyproject-api==1.5.1 \
     --hash=sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9 \
     --hash=sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43
     # via tox
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via build
-pyserial==3.5 \
-    --hash=sha256:3c77e014170dfffbd816e6ffc205e9842efb10be9f58ec16d3e8675b4925cddb \
-    --hash=sha256:c4451db6ba391ca6ca299fb3ec7bae67a5c55dde170964c7a14ceefec02f2cf0
-    # via umodbus
-pysolarmanv5==2.4.0 \
-    --hash=sha256:04af419c44a1f61179128fc8ffeb831c5794add189ca54a7ce6deaa6d304412c \
-    --hash=sha256:7a2a87fcc3245f5063e9797149fb82b01625ecf593e30899098fa951e4c01a5a
-    # via inverter (pyproject.toml)
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via arrow
 python-slugify==8.0.1 \
     --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
     --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
     # via cookiecutter
-pyupgrade==3.3.1 \
-    --hash=sha256:3b93641963df022d605c78aeae4b5956a5296ea24701eafaef9c487527b77e60 \
-    --hash=sha256:f88bce38b0ba92c2a9a5063c8629e456e8d919b67d2d42c7ecab82ff196f9813
-    # via inverter (pyproject.toml)
+pyupgrade==3.3.2 \
+    --hash=sha256:bcfed63d38811809f179fd269dec246680b0aaa5bbe662b535826e5fa2275219 \
+    --hash=sha256:c05b82c911934b3a638b29f48f48dc6e0ef6c57c55ec36f2b41ae9dbf6711b4b
+    # via inverter-connect (pyproject.toml)
 pyyaml==6.0 \
     --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
     --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
     --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
     --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
     --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
     --hash=sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4 \
@@ -614,48 +609,50 @@
     --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
     --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
     --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
     --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
     --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
     --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
     --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
-    # via cookiecutter
+    # via
+    #   cookiecutter
+    #   inverter-connect (pyproject.toml)
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.28.2 \
-    --hash=sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa \
-    --hash=sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf
+requests==2.29.0 \
+    --hash=sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b \
+    --hash=sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059
     # via
     #   cookiecutter
     #   requests-toolbelt
     #   safety
     #   twine
 requests-toolbelt==0.10.1 \
     --hash=sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7 \
     --hash=sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d
     # via twine
 rfc3986==2.0.0 \
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
     # via twine
-rich==13.3.4 \
-    --hash=sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a \
-    --hash=sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b
+rich==13.3.5 \
+    --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
+    --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
     # via
-    #   inverter (pyproject.toml)
+    #   inverter-connect (pyproject.toml)
     #   manageprojects
     #   rich-click
     #   twine
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
-    #   inverter (pyproject.toml)
+    #   inverter-connect (pyproject.toml)
     #   manageprojects
 ruamel-yaml==0.17.21 \
     --hash=sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7 \
     --hash=sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af
     # via safety
 ruamel-yaml-clib==0.2.7 \
     --hash=sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e \
@@ -694,15 +691,15 @@
     --hash=sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0 \
     --hash=sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646 \
     --hash=sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38
     # via ruamel-yaml
 safety==2.3.4 \
     --hash=sha256:6224dcd9b20986a2b2c5e7acfdfba6bca42bb11b2783b24ed04f32317e5167ea \
     --hash=sha256:b9e74e794e82f54d11f4091c5d820c4d2d81de9f953bf0b4f33ac8bc402ae72c
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
     --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
     # via keyring
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
@@ -727,48 +724,44 @@
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   autopep8
     #   black
     #   build
     #   flynt
-    #   inverter (pyproject.toml)
+    #   inverter-connect (pyproject.toml)
     #   mypy
     #   pyproject-api
     #   pyproject-hooks
     #   tox
-tomlkit==0.11.7 \
-    --hash=sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c \
-    --hash=sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d
+tomlkit==0.11.8 \
+    --hash=sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171 \
+    --hash=sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3
     # via manageprojects
-tox==4.4.12 \
-    --hash=sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e \
-    --hash=sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b
-    # via inverter (pyproject.toml)
+tox==4.5.1 \
+    --hash=sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56 \
+    --hash=sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046
+    # via inverter-connect (pyproject.toml)
 twine==4.0.2 \
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
-    # via inverter (pyproject.toml)
+    # via inverter-connect (pyproject.toml)
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via mypy
-umodbus==1.0.4 \
-    --hash=sha256:26bbbeff02d6d8a3e29bb0f9d9044c672d55fc1687afe4297a2f7d68175103a7 \
-    --hash=sha256:aab3e61488d8bef638466687b360192ddf046a23b61a9ba3734b4f48d31efe16
-    # via pysolarmanv5
 urllib3==1.26.15 \
     --hash=sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305 \
     --hash=sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42
     # via
     #   requests
     #   twine
-virtualenv==20.21.0 \
-    --hash=sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc \
-    --hash=sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68
+virtualenv==20.22.0 \
+    --hash=sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3 \
+    --hash=sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a
     # via tox
 webencodings==0.5.1 \
     --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
     --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
     # via bleach
 wheel==0.40.0 \
     --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
@@ -776,17 +769,17 @@
     # via pip-tools
 zipp==3.15.0 \
     --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
     --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.1 \
-    --hash=sha256:408539897ee535dbfb83a153f7bc4d620f990d8bd44a52a986efc0b4d330d34a \
-    --hash=sha256:64b1d4528e491aa835ec6ece0c1ac40ce6ab6d886e60740f6519db44b2e9634d
+pip==23.1.2 \
+    --hash=sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba \
+    --hash=sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18
     # via pip-tools
-setuptools==67.6.1 \
-    --hash=sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a \
-    --hash=sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078
+setuptools==67.7.2 \
+    --hash=sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b \
+    --hash=sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990
     # via
     #   pip-tools
     #   safety
```

