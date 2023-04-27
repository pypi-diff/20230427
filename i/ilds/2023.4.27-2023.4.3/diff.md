# Comparing `tmp/ilds-2023.4.27.tar.gz` & `tmp/ilds-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ilds-2023.4.27.tar", last modified: Thu Apr 27 08:17:53 2023, max compression
+gzip compressed data, was "dist\ilds-2023.4.3.tar", last modified: Mon Apr  3 10:59:19 2023, max compression
```

## Comparing `ilds-2023.4.27.tar` & `ilds-2023.4.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:17:53.000000 ilds-2023.4.27/
-drwxrwxrwx   0        0        0        0 2023-04-27 08:17:53.000000 ilds-2023.4.27/ilds/
--rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.4.27/ilds/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:17:53.000000 ilds-2023.4.27/ilds/django/
--rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.4.27/ilds/django/admin.py
--rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.4.27/ilds/django/import_export.py
--rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.4.27/ilds/django/model.py
--rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.4.27/ilds/django/user.py
--rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.4.27/ilds/django/util.py
--rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.4.27/ilds/django/__init__.py
--rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.4.27/ilds/everything.py
--rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.4.27/ilds/excel_xlrd.py
--rw-rw-rw-   0        0        0     7970 2022-10-19 09:11:30.000000 ilds-2023.4.27/ilds/excel_xlsx.py
--rw-rw-rw-   0        0        0    26848 2023-04-03 10:59:15.000000 ilds-2023.4.27/ilds/file.py
--rw-rw-rw-   0        0        0     1530 2023-04-10 12:39:32.000000 ilds-2023.4.27/ilds/json.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:17:53.000000 ilds-2023.4.27/ilds/lib/
--rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.4.27/ilds/lib/browsercookie.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:17:53.000000 ilds-2023.4.27/ilds/lib/configobj/
--rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.4.27/ilds/lib/configobj/validate.py
--rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.4.27/ilds/lib/configobj/_version.py
--rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.4.27/ilds/lib/configobj/__init__.py
--rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.4.27/ilds/lib/hexdump.py
--rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.4.27/ilds/lib/__init__.py
--rw-rw-rw-   0        0        0    15494 2021-10-24 10:49:44.000000 ilds-2023.4.27/ilds/match_data.py
--rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.4.27/ilds/md.py
--rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.4.27/ilds/md5summer.py
--rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.4.27/ilds/mycsv.py
--rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.4.27/ilds/net.py
--rw-rw-rw-   0        0        0    10403 2023-04-27 08:17:50.000000 ilds-2023.4.27/ilds/pd.py
--rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.4.27/ilds/spider.py
--rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.4.27/ilds/time.py
--rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.4.27/ilds/util.py
--rw-rw-rw-   0        0        0       23 2023-04-27 07:31:28.000000 ilds-2023.4.27/ilds/versions.py
--rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.4.27/ilds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:17:53.000000 ilds-2023.4.27/ilds.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-27 08:17:52.000000 ilds-2023.4.27/ilds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1317 2023-04-27 08:17:52.000000 ilds-2023.4.27/ilds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-04-27 08:17:52.000000 ilds-2023.4.27/ilds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      708 2023-04-27 08:17:52.000000 ilds-2023.4.27/ilds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 08:17:52.000000 ilds-2023.4.27/ilds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1317 2023-04-27 08:17:53.000000 ilds-2023.4.27/PKG-INFO
--rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.4.27/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-27 08:17:53.000000 ilds-2023.4.27/setup.cfg
--rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.4.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/
+-rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.4.3/ilds/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/django/
+-rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.4.3/ilds/django/admin.py
+-rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.4.3/ilds/django/import_export.py
+-rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.4.3/ilds/django/model.py
+-rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.4.3/ilds/django/user.py
+-rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.4.3/ilds/django/util.py
+-rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.4.3/ilds/django/__init__.py
+-rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.4.3/ilds/everything.py
+-rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.4.3/ilds/excel_xlrd.py
+-rw-rw-rw-   0        0        0     7970 2022-10-19 09:11:30.000000 ilds-2023.4.3/ilds/excel_xlsx.py
+-rw-rw-rw-   0        0        0    26848 2023-04-03 10:59:15.000000 ilds-2023.4.3/ilds/file.py
+-rw-rw-rw-   0        0        0     1530 2021-09-26 05:15:22.000000 ilds-2023.4.3/ilds/json.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/lib/
+-rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.4.3/ilds/lib/browsercookie.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/lib/configobj/
+-rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/validate.py
+-rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/_version.py
+-rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/__init__.py
+-rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.4.3/ilds/lib/hexdump.py
+-rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.4.3/ilds/lib/__init__.py
+-rw-rw-rw-   0        0        0    15494 2021-10-24 10:49:44.000000 ilds-2023.4.3/ilds/match_data.py
+-rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.4.3/ilds/md.py
+-rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.4.3/ilds/md5summer.py
+-rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.4.3/ilds/mycsv.py
+-rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.4.3/ilds/net.py
+-rw-rw-rw-   0        0        0     7906 2023-04-03 10:59:05.000000 ilds-2023.4.3/ilds/pd.py
+-rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.4.3/ilds/spider.py
+-rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.4.3/ilds/time.py
+-rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.4.3/ilds/util.py
+-rw-rw-rw-   0        0        0       22 2023-04-03 10:59:05.000000 ilds-2023.4.3/ilds/versions.py
+-rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.4.3/ilds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1316 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      708 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1316 2023-04-03 10:59:19.000000 ilds-2023.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.4.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-03 10:59:19.000000 ilds-2023.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.4.3/setup.py
```

### Comparing `ilds-2023.4.27/ilds/cmd.py` & `ilds-2023.4.3/ilds/cmd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/django/admin.py` & `ilds-2023.4.3/ilds/django/admin.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/django/import_export.py` & `ilds-2023.4.3/ilds/django/import_export.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/django/model.py` & `ilds-2023.4.3/ilds/django/model.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/django/user.py` & `ilds-2023.4.3/ilds/django/user.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/django/util.py` & `ilds-2023.4.3/ilds/django/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/everything.py` & `ilds-2023.4.3/ilds/everything.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/excel_xlrd.py` & `ilds-2023.4.3/ilds/excel_xlrd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/excel_xlsx.py` & `ilds-2023.4.3/ilds/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/file.py` & `ilds-2023.4.3/ilds/file.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/json.py` & `ilds-2023.4.3/ilds/json.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/lib/browsercookie.py` & `ilds-2023.4.3/ilds/lib/browsercookie.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/lib/configobj/validate.py` & `ilds-2023.4.3/ilds/lib/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/lib/configobj/__init__.py` & `ilds-2023.4.3/ilds/lib/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/lib/hexdump.py` & `ilds-2023.4.3/ilds/lib/hexdump.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/match_data.py` & `ilds-2023.4.3/ilds/match_data.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/md.py` & `ilds-2023.4.3/ilds/md.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/md5summer.py` & `ilds-2023.4.3/ilds/md5summer.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/mycsv.py` & `ilds-2023.4.3/ilds/mycsv.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/net.py` & `ilds-2023.4.3/ilds/net.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/spider.py` & `ilds-2023.4.3/ilds/spider.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/time.py` & `ilds-2023.4.3/ilds/time.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds/util.py` & `ilds-2023.4.3/ilds/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/ilds.egg-info/PKG-INFO` & `ilds-2023.4.3/ilds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.4.27
+Version: 2023.4.3
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.4.27/ilds.egg-info/SOURCES.txt` & `ilds-2023.4.3/ilds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.27/PKG-INFO` & `ilds-2023.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.4.27
+Version: 2023.4.3
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.4.27/setup.py` & `ilds-2023.4.3/setup.py`

 * *Files identical despite different names*

