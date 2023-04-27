# Comparing `tmp/qtaf-5.6.1.tar.gz` & `tmp/qtaf-5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtaf-5.6.1.tar", last modified: Sat Apr 22 12:16:41 2023, max compression
+gzip compressed data, was "qtaf-5.6.2.tar", last modified: Thu Apr 27 09:08:34 2023, max compression
```

## Comparing `qtaf-5.6.1.tar` & `qtaf-5.6.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.808263 qtaf-5.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-22 12:16:25.000000 qtaf-5.6.1/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 12:16:25.000000 qtaf-5.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-22 12:16:41.808263 qtaf-5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-22 12:16:25.000000 qtaf-5.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-22 12:16:25.000000 qtaf-5.6.1/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.800263 qtaf-5.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-22 12:16:25.000000 qtaf-5.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta-manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.800263 qtaf-5.6.1/qta_statics/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/TestReport.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/TestResult.xsl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-04-22 12:16:25.000000 qtaf-5.6.1/qta_statics/qta-report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.804263 qtaf-5.6.1/qtaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-22 12:16:41.000000 qtaf-5.6.1/qtaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-22 12:16:25.000000 qtaf-5.6.1/qtaf_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-22 12:16:25.000000 qtaf-5.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:16:41.808263 qtaf-5.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-22 12:16:25.000000 qtaf-5.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.808263 qtaf-5.6.1/testbase/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/datadrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/exlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    33826 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    35361 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/testresult.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-04-22 12:16:25.000000 qtaf-5.6.1/testbase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 12:16:41.000000 qtaf-5.6.1/testbase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:16:41.808263 qtaf-5.6.1/tuia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/_tif.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/accessible.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/filedialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/gfcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/qpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/qpathparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/remoteprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/uiacontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/webcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/wincontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-22 12:16:25.000000 qtaf-5.6.1/tuia/wintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 12:16:39.000000 qtaf-5.6.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:34.981925 qtaf-5.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-27 09:08:22.000000 qtaf-5.6.2/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 09:08:22.000000 qtaf-5.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-27 09:08:34.981925 qtaf-5.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-27 09:08:22.000000 qtaf-5.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-27 09:08:22.000000 qtaf-5.6.2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:34.973925 qtaf-5.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 09:08:22.000000 qtaf-5.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-27 09:08:22.000000 qtaf-5.6.2/qta-manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:34.973925 qtaf-5.6.2/qta_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-27 09:08:22.000000 qtaf-5.6.2/qta_statics/TestReport.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-27 09:08:22.000000 qtaf-5.6.2/qta_statics/TestResult.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:22.000000 qtaf-5.6.2/qta_statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-04-27 09:08:22.000000 qtaf-5.6.2/qta_statics/qta-report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:34.977925 qtaf-5.6.2/qtaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-27 09:08:34.000000 qtaf-5.6.2/qtaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-27 09:08:34.000000 qtaf-5.6.2/qtaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:08:34.000000 qtaf-5.6.2/qtaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 09:08:34.000000 qtaf-5.6.2/qtaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 09:08:34.000000 qtaf-5.6.2/qtaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 09:08:34.000000 qtaf-5.6.2/qtaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-27 09:08:22.000000 qtaf-5.6.2/qtaf_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 09:08:22.000000 qtaf-5.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:08:34.981925 qtaf-5.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-27 09:08:22.000000 qtaf-5.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:34.981925 qtaf-5.6.2/testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/datadrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/exlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-04-27 09:08:22.000000 qtaf-5.6.2/testbase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 09:08:34.000000 qtaf-5.6.2/testbase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:08:34.981925 qtaf-5.6.2/tuia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/_tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/accessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/filedialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/gfcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/qpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/qpathparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/remoteprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/uiacontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/webcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/wincontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-27 09:08:22.000000 qtaf-5.6.2/tuia/wintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 09:08:32.000000 qtaf-5.6.2/version.txt
```

### Comparing `qtaf-5.6.1/LICENSE.TXT` & `qtaf-5.6.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/PKG-INFO` & `qtaf-5.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.1
+Version: 5.6.2
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.1/README.md` & `qtaf-5.6.2/README.md`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/__main__.py` & `qtaf-5.6.2/__main__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/qta-manage.py` & `qtaf-5.6.2/qta-manage.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/qta_statics/TestReport.xsl` & `qtaf-5.6.2/qta_statics/TestReport.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/qta_statics/TestResult.xsl` & `qtaf-5.6.2/qta_statics/TestResult.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/qta_statics/qta-report.html` & `qtaf-5.6.2/qta_statics/qta-report.html`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/qtaf.egg-info/PKG-INFO` & `qtaf-5.6.2/qtaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.1
+Version: 5.6.2
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.1/qtaf.egg-info/SOURCES.txt` & `qtaf-5.6.2/qtaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/qtaf_settings.py` & `qtaf-5.6.2/qtaf_settings.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/setup.py` & `qtaf-5.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/__init__.py` & `qtaf-5.6.2/testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/assertion.py` & `qtaf-5.6.2/testbase/assertion.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/conf.py` & `qtaf-5.6.2/testbase/conf.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/context.py` & `qtaf-5.6.2/testbase/context.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/datadrive.py` & `qtaf-5.6.2/testbase/datadrive.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/dist.py` & `qtaf-5.6.2/testbase/dist.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/exlib.py` & `qtaf-5.6.2/testbase/exlib.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/loader.py` & `qtaf-5.6.2/testbase/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,17 +108,19 @@
                     )
             elif isinstance(obj, type):
                 if issubclass(obj, TestCase):
                     testcases += self._load_from_class(
                         obj, data_key, exclude_data_keys, parameters
                     )
                 elif issubclass(obj, TestSuite):
-                    testcases += self._load_from_testsuite(
-                        obj, data_key, exclude_data_keys, parameters
-                    )
+                    if not self._filter_testcase(obj):
+                        tests = self._load_from_testsuite(
+                            obj, data_key, exclude_data_keys, parameters
+                        )
+                        testcases.append(obj(tests))  # append testsuite to testcase list
 
         # 过滤掉重复的用例
         testcase_dict = OrderedDict()
         for testcase in testcases:
             testcase_dict[testcase.test_name] = testcase
 
         return list(testcase_dict.values())
@@ -188,21 +190,32 @@
         )
 
     def _is_testsuite_class(self, obj):
         """是否是测试用例套类
 
         :returns bool - 是否为用例套类
         """
-        return isinstance(obj, type) and issubclass(obj, TestSuite)
+        return (
+            isinstance(obj, type)
+            and issubclass(obj, TestSuite)
+            and obj is not TestSuite
+        )
 
     def _walk_package_error(self, modulename):
         """walk_packages错误回调"""
         self._module_errs[modulename] = traceback.format_exc()
 
-    def _load_from_package(self, pkg, data_key=None, exclude_data_key=None, attrs=None):
+    def _load_from_package(
+        self,
+        pkg,
+        data_key=None,
+        exclude_data_key=None,
+        attrs=None,
+        ignore_testsuite=False,
+    ):
         """从一个python包加载测试用例
 
         :param pkg: Python包
         :type pkg: ModuleType
         :returns list - 测试用例对象列表
         """
         tests = []
@@ -214,33 +227,48 @@
             try:
                 __import__(modulename)
                 tests += self._load_from_module(
                     sys.modules[modulename],
                     data_key,
                     exclude_data_key=exclude_data_key,
                     attrs=None,
+                    ignore_testsuite=ignore_testsuite,
                 )
             except Exception:  # pylint: disable=broad-except
                 self._module_errs[modulename] = traceback.format_exc()
         return tests
 
-    def _load_from_module(self, mod, data_key=None, exclude_data_key=None, attrs=None):
+    def _load_from_module(
+        self,
+        mod,
+        data_key=None,
+        exclude_data_key=None,
+        attrs=None,
+        ignore_testsuite=False,
+    ):
         """从一个python模块加载测试用例
 
         :param mod: Python模块
         :type mod: ModuleType
         :returns list - 测试用例对象列表
         """
         tests = []
         for name in dir(mod):
             obj = getattr(mod, name)
             if self._is_testcase_class(obj):
                 tests += self._load_from_class(
                     obj, data_key, exclude_data_key=exclude_data_key, attrs=attrs
                 )
+            elif self._is_testsuite_class(obj) and not ignore_testsuite:
+                if not self._filter_testcase(obj):
+                    testcases = self._load_from_testsuite(
+                        obj, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                    )
+                    tests.append(obj(testcases))
+
         if hasattr(mod, "__qtaf_seq_tests__"):  # 测试用例需要顺序执行
             seqdef = mod.__qtaf_seq_tests__
             if not isinstance(seqdef, list):
                 raise TypeError("__qtaf_seq_tests__必须为list类型")
             if len(seqdef) == 0:
                 raise ValueError("__qtaf_seq_tests__必须至少包含一个测试用例")
             for it in seqdef:
@@ -270,26 +298,44 @@
         tests = []
         for test in cls.testcases:
             if isinstance(test, str):
                 test = self._load(test)
             if not isinstance(test, type):
                 if hasattr(test, "__path__"):
                     tests += self._load_from_package(
-                        test, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                        test,
+                        data_key,
+                        exclude_data_key=exclude_data_key,
+                        attrs=attrs,
+                        ignore_testsuite=True,
                     )
                 else:
                     tests += self._load_from_module(
-                        test, data_key, exclude_data_key=exclude_data_key, attrs=attrs
+                        test,
+                        data_key,
+                        exclude_data_key=exclude_data_key,
+                        attrs=attrs,
+                        ignore_testsuite=True,
                     )
             else:
                 tests += self._load_from_class(
                     test, data_key, exclude_data_key=exclude_data_key, attrs=attrs
                 )
 
-        return [cls([it for it in tests if not cls.filter(it)])]
+        return [it for it in tests if not cls.filter(it)]
+
+    def _filter_testcase(self, test):
+        if not self._filter:
+            return False
+        filter_reason = self._filter(test)
+        if filter_reason:
+            self._filtered_tests[test] = filter_reason
+            return True
+        else:
+            return False
 
     def _load_from_class(self, cls, data_key=None, exclude_data_key=None, attrs=None):
         """加载用例类
 
         :param cls: Python类
         :type cls: Type
         :returns list - 测试用例对象列表
@@ -308,24 +354,15 @@
                 ] = traceback.format_exc()
             else:
                 if len(tests) == 0:
                     tests = [cls(attrs=attrs)]
         else:
             tests = [cls(attrs=attrs)]
 
-        if self._filter:
-            final_tests = []
-            for it in tests:
-                filter_reason = self._filter(it)
-                if filter_reason:
-                    self._filtered_tests[it] = filter_reason
-                else:
-                    final_tests.append(it)
-            tests = final_tests
-        return tests
+        return [it for it in tests if not self._filter_testcase(it)]
 
 
 class TestDataLoader(object):
     """测试数据加载器"""
 
     MODULE_NAME = "testbase.loader.testdata"
```

### Comparing `qtaf-5.6.1/testbase/logger.py` & `qtaf-5.6.2/testbase/logger.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/management.py` & `qtaf-5.6.2/testbase/management.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from testbase import project
 from testbase.conf import settings
 from testbase.version import version
 from testbase.exlib import ExLibManager
 from testbase.dist import DistGenerator, VirtuelEnv
 from testbase.loader import TestLoader
 from testbase.testcase import TestCasePriority, TestCaseStatus, TestCase
+from testbase.testsuite import TestSuite
 from testbase.runner import TestCaseSettings
 from testbase.report import test_list_types
 from testbase.types import runner_types, report_types, resmgr_backend_types
 from testbase.util import codecs_open, path_exists
 
 
 class ArgumentParser(object):
@@ -522,15 +523,15 @@
         choices=test_list_types.keys(),
     )
 
     def execute(self, args):
         if not args.tests:
             logger.info("no test set specified")
             return 1
-        shows = args.shows or ["filtered", "error", "normal"]
+        shows = args.shows or ["filtered", "error", "normal", "testsuite"]
         priorities = args.priorities or [
             TestCase.EnumPriority.Normal,
             TestCase.EnumPriority.High,
         ]
         status = args.status or [TestCase.EnumStatus.Ready]
 
         test_conf = TestCaseSettings(
@@ -541,14 +542,19 @@
             owners=args.owners,
             tags=args.tags,
             excluded_tags=args.excluded_tags,
         )
 
         loader = TestLoader(test_conf.filter)
         tests = loader.load(test_conf.names)
+        testsuites = []
+        for test in tests[:]:
+            if isinstance(test, TestSuite):
+                testsuites.append(test)
+                tests.remove(test)
 
         test_list_output = test_list_types[args.output_type](args.output_file)
 
         if "filtered" in shows:
             filtered_tests = loader.get_filtered_tests_with_reason().items()
             sorted_filtered_tests = sorted(filtered_tests, key=lambda x: x[0].test_name)
             test_list_output.output_filtered_tests(sorted_filtered_tests)
@@ -557,14 +563,18 @@
             sorted_tests = sorted(tests, key=lambda x: x.test_name)
             test_list_output.output_normal_tests(sorted_tests)
 
         if "error" in shows:
             error_tests = loader.get_last_errors().items()
             sorted_error_tests = sorted(error_tests, key=lambda x: x[0])
             test_list_output.output_error_tests(sorted_error_tests)
+
+        if "testsuite" in shows:
+            test_list_output.output_testsuites(testsuites)
+
         test_list_output.end_output()
 
 
 class RunPlan(Command):
     """执行测试计划"""
 
     name = "runplan"
```

### Comparing `qtaf-5.6.1/testbase/plan.py` & `qtaf-5.6.2/testbase/plan.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/project.py` & `qtaf-5.6.2/testbase/project.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/report.py` & `qtaf-5.6.2/testbase/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1043,14 +1043,17 @@
 
     def output_filtered_tests(self, filtered_tests):
         raise NotImplementedError
 
     def output_error_tests(self, error_tests):
         raise NotImplementedError
 
+    def output_testsuites(self, testsuites):
+        raise NotImplementedError
+
     def end_output(self):
         if self._close_fd:
             self._fd.close()
 
 
 class StreamTestListOutput(TestListOutputBase):
     """stream output"""
@@ -1075,14 +1078,22 @@
         self._output_func("\n======================")
         self._output_func("%s error tests:" % len(error_tests))
         self._output_func("======================")
         for test_name, error in error_tests:
             test_info = 'cannot load test "%s"' % test_name + ", error:\n" + error
             self._output_func(test_info)
 
+    def output_testsuites(self, testsuites):
+        self._output_func("\n======================")
+        self._output_func("%s testsuites:" % len(testsuites))
+        self._output_func("======================")
+        for testsuite in testsuites:
+            test_info = self.stream_format_test(testsuite)
+            self._output_func(test_info)
+
     def stream_format_test(self, test):
         desc = "%s/%s" % (test.priority, test.status)
         test_info = "%-12s " % desc
         test_info += "timeout=%-3s " % test.timeout
         test_info += "%-10s " % test.owner
         test_info += "%s" % test.test_name
         return test_info
```

### Comparing `qtaf-5.6.1/testbase/resource.py` & `qtaf-5.6.2/testbase/resource.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/retry.py` & `qtaf-5.6.2/testbase/retry.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/runner.py` & `qtaf-5.6.2/testbase/runner.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/serialization.py` & `qtaf-5.6.2/testbase/serialization.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/test.py` & `qtaf-5.6.2/testbase/test.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/testcase.py` & `qtaf-5.6.2/testbase/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/testresult.py` & `qtaf-5.6.2/testbase/testresult.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/testsuite.py` & `qtaf-5.6.2/testbase/testsuite.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         :type testresult_factory: ITestResultFactory
         :param stop_on_failure: 是否遇到失败用例停止执行
         :type stop_on_failure: bool
 
         :return TestResult/TestResultCollection - 测试结果
         """
         passed = True
-        results = []
+        results = [testresult]
         for it in testsuite:
             case_result = self._run_test(testsuite, it, testresult_factory, testresult)
             passed &= case_result.passed
             results.append(case_result)
             if not passed and stop_on_failure:
                 break
         return TestResultCollection(results, passed)
@@ -272,15 +272,15 @@
         :type testresult_factory: ITestResultFactory
         :param concurrency: 并发数
         :type concurrency: int
 
         :return TestResult/TestResultCollection - 测试结果
         """
         tests_queue = collections.deque([it for it in testsuite])
-        results = []
+        results = [testresult]
         threads = []
         lock = threading.Lock()
         for _ in range(concurrency):
             thread = threading.Thread(
                 target=self._run_test_from_queue,
                 args=(
                     testsuite,
@@ -314,15 +314,15 @@
         """
         if not isinstance(testsuite, TestSuite):
             raise ValueError("Invalid testsuite type: %s" % type(testsuite))
         testresult = testresult_factory.create(testsuite)
         testresult.begin_test(testsuite)
         testresult.begin_step("pre_test")
         testsuite.init_test(testresult)
-        result = TestResultCollection([], False)
+        result = TestResultCollection([testresult], False)
         try:
             testsuite.pre_test()
         except:
             self._log_testsuite_error(
                 testsuite,
                 testresult,
                 "pre_test run failed: \n%s" % traceback.format_exc(),
@@ -365,29 +365,32 @@
     EnumPriority = TestCase.EnumPriority
     EnumStatus = TestCase.EnumStatus
 
     class EnumExecMode(object):
         Parallel = "parallel"
         Sequential = "sequential"
 
+    owner = None
+    priority = None
+    status = None
+    timeout = None
     testcases = []
     testcase_filter = {}
     exec_mode = EnumExecMode.Sequential
     stop_on_failure = True
     concurrency = 1
 
     def __init__(self, testcases):
         self.case_runner = TestSuiteCaseRunner(
             self.exec_mode,
             stop_on_failure=self.stop_on_failure,
             concurrency=self.concurrency,
         )
         self.__testcases = testcases
-        self.__testresult = None
-        self.__testresults = None
+        self.__testresults = []
         self.__current_stage = ""
 
     def __iter__(self):
         for it in self.__testcases:
             yield it
 
     def __len__(self):
@@ -411,23 +414,27 @@
 
     @property
     def test_result(self):
         """测试套结果
 
         :return: TestResult
         """
-        return self.__testresult
+        if self.__testresults:
+            return self.__testresults[0]
+        return None
 
     @property
     def test_results(self):
         """测试用例结果
 
         :return: TestResultCollection
         """
-        return self.__testresults
+        if len(self.__testresults) > 1:
+            return self.__testresults[1:]
+        return []
 
     @property
     def current_stage(self):
         return self.__current_stage
 
     @current_stage.setter
     def current_stage(self, value):
@@ -457,14 +464,15 @@
             and isinstance(owner_list, list)
             and testcase.owner not in owner_list
         ):
             return True
         tag_list = cls.testcase_filter.get("tags", [])
         if (
             tag_list
+            and hasattr(testcase, "tags")
             and isinstance(tag_list, list)
             and set(tag_list).isdisjoint(testcase.tags)
         ):
             return True
         exclude_tag_list = cls.testcase_filter.get("exclude_tags", [])
         if (
             exclude_tag_list
@@ -506,15 +514,15 @@
 
     def init_test(self, testresult):
         """初始化测试套。慎用此函数，尽量将初始化放到pre_test里。
 
         :param testresult: 测试结果
         :type testresult: TestResult
         """
-        self.__testresult = testresult
+        self.__testresults.append(testresult)
 
     def pre_test(self):
         pass
 
     def post_test(self):
         pass
```

### Comparing `qtaf-5.6.1/testbase/types.py` & `qtaf-5.6.2/testbase/types.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/testbase/util.py` & `qtaf-5.6.2/testbase/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/__init__.py` & `qtaf-5.6.2/tuia/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/_tif.py` & `qtaf-5.6.2/tuia/_tif.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/accessible.py` & `qtaf-5.6.2/tuia/accessible.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/app.py` & `qtaf-5.6.2/tuia/app.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/control.py` & `qtaf-5.6.2/tuia/control.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/env.py` & `qtaf-5.6.2/tuia/env.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/exceptions.py` & `qtaf-5.6.2/tuia/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/filedialog.py` & `qtaf-5.6.2/tuia/filedialog.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/gfcontrols.py` & `qtaf-5.6.2/tuia/gfcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/keyboard.py` & `qtaf-5.6.2/tuia/keyboard.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/mouse.py` & `qtaf-5.6.2/tuia/mouse.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/qpath.py` & `qtaf-5.6.2/tuia/qpath.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/qpathparser.py` & `qtaf-5.6.2/tuia/qpathparser.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/remoteprocessing.py` & `qtaf-5.6.2/tuia/remoteprocessing.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/testcase.py` & `qtaf-5.6.2/tuia/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/uiacontrols.py` & `qtaf-5.6.2/tuia/uiacontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/util.py` & `qtaf-5.6.2/tuia/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/webcontrols.py` & `qtaf-5.6.2/tuia/webcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/wincontrols.py` & `qtaf-5.6.2/tuia/wincontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.1/tuia/wintypes.py` & `qtaf-5.6.2/tuia/wintypes.py`

 * *Files identical despite different names*

