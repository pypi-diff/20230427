# Comparing `tmp/visualtest_python-1.3.0-py3-none-any.whl.zip` & `tmp/visualtest_python-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20518 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1129 b- defN 23-Apr-26 16:58 sbvt/__init__.py
+Zip file size: 20523 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1129 b- defN 23-Apr-27 18:10 sbvt/__init__.py
 -rw-r--r--  2.0 unx     9114 b- defN 23-Apr-26 16:54 sbvt/api.py
 -rw-r--r--  2.0 unx    34618 b- defN 23-Apr-26 16:54 sbvt/browser.py
 -rw-r--r--  2.0 unx     5981 b- defN 22-Sep-26 14:39 sbvt/imagetools.py
 -rw-r--r--  2.0 unx      548 b- defN 22-Sep-26 14:39 sbvt/timer.py
--rw-r--r--  2.0 unx    11181 b- defN 23-Apr-26 16:54 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      869 b- defN 23-Apr-27 15:15 visualtest_python-1.3.0.dist-info/RECORD
-11 files, 68486 bytes uncompressed, 19060 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx    11191 b- defN 23-Apr-27 18:10 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      869 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/RECORD
+11 files, 68496 bytes uncompressed, 19065 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.3.0.dist-info/LICENSE
+Filename: visualtest_python-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.3.0.dist-info/METADATA
+Filename: visualtest_python-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.3.0.dist-info/WHEEL
+Filename: visualtest_python-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.3.0.dist-info/top_level.txt
+Filename: visualtest_python-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.3.0.dist-info/RECORD
+Filename: visualtest_python-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,14 +1,14 @@
 import logging
 import os.path
 
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 logPath = 'logs'
 if not os.path.exists(logPath):
     os.makedirs(logPath)
 
 # By generating a new logger as 'vt' we don't affect global logging from other packages
 # Each logger created in our package should be a child by prefacing with 'vt.childname'
```

## sbvt/visualtest.py

```diff
@@ -227,15 +227,15 @@
             if not isinstance(options['freezePage'], bool):
                 raise Exception(f'freezePage must be of type "bool"')
 
         if 'element' in options:
             screenshotResult = self.browser.takeElementScreenshot(filePath, options)
             imageType = 'element'
         elif 'viewport' in options and options['viewport'] == True:
-            result = self.browser.takeViewportScreenshot(filePath, options)
+            screenshotResult = self.browser.takeViewportScreenshot(filePath, options)
             imageType = 'viewport'
         else:
             if 'lazyload' in options:
                 if type(options['lazyload']) != int or options['lazyload'] < 0 or options['lazyload'] > 10000:
                     raise Exception('"lazyload" value must be an integer between 0 and 10000 ms!')
 
             screenshotResult = self.browser.takeFullpageScreenshot(filePath, options)
```

## Comparing `visualtest_python-1.3.0.dist-info/LICENSE` & `visualtest_python-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.3.0.dist-info/METADATA` & `visualtest_python-1.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `visualtest_python-1.3.0.dist-info/RECORD` & `visualtest_python-1.3.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-sbvt/__init__.py,sha256=2r35CuXc9Fnkdlc1BrxcY70WQUsZCxgtgYChni57Wp4,1129
+sbvt/__init__.py,sha256=yDlWl36LFXFnYp-wdUMtppagx-HtDzdO9IAO6_bhFJ8,1129
 sbvt/api.py,sha256=BS6nFHtzhfKmYAYcJXvYHmsAlAibNgTRUe4s4Hg8Eyw,9114
 sbvt/browser.py,sha256=IrA2nBhsxk5MODqsFCj51Mx3yOySY74jaoWZ5SPnC9s,34618
 sbvt/imagetools.py,sha256=6z4MA2Wfet8jMlTlKTU68JXSADXNj78fOXQhl7f_ONQ,5981
 sbvt/timer.py,sha256=ciQJQUYSTChdIbsLiYiEzPa6yw8YwSqaeWc7DU4gSrE,548
-sbvt/visualtest.py,sha256=shoeT1Z1aWYZ_WztlX_H1Pw8e6stsZBwt3N_NF15qFc,11181
-visualtest_python-1.3.0.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
-visualtest_python-1.3.0.dist-info/METADATA,sha256=MsEPiwlbBJTQk1I6Qkrj_2b15BXk60eWu65oTq5oZg8,3876
-visualtest_python-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-visualtest_python-1.3.0.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
-visualtest_python-1.3.0.dist-info/RECORD,,
+sbvt/visualtest.py,sha256=2bKP3hKA4sA4Tvv57PGvT7RgjPIzfewVh5Gy2uLPhXk,11191
+visualtest_python-1.3.1.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
+visualtest_python-1.3.1.dist-info/METADATA,sha256=aVmgWh-RNUqCtKoymgIdWx2UTSb5Hph-EtCujciutt0,3876
+visualtest_python-1.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+visualtest_python-1.3.1.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
+visualtest_python-1.3.1.dist-info/RECORD,,
```

