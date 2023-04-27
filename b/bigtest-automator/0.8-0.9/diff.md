# Comparing `tmp/bigtest_automator-0.8.tar.gz` & `tmp/bigtest_automator-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtest_automator-0.8.tar", last modified: Mon Apr 24 10:56:39 2023, max compression
+gzip compressed data, was "bigtest_automator-0.9.tar", last modified: Thu Apr 27 04:25:06 2023, max compression
```

## Comparing `bigtest_automator-0.8.tar` & `bigtest_automator-0.9.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.841570 bigtest_automator-0.8/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-24 10:56:39.841429 bigtest_automator-0.8/PKG-INFO
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.837599 bigtest_automator-0.8/bigtest_automator.egg-info/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/PKG-INFO
--rw-r--r--   0 shantharamp   (502) staff       (20)      871 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/SOURCES.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/dependency_links.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       61 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/entry_points.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/requires.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/top_level.txt
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.838474 bigtest_automator-0.8/core_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.8/core_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     7023 2023-04-24 10:55:23.000000 bigtest_automator-0.8/core_utils/generate_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.8/core_utils/run_scp.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.8/core_utils/run_vmstat.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.8/core_utils/take_awr_snapshot.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.838952 bigtest_automator-0.8/entrypoint/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:17:21.000000 bigtest_automator-0.8/entrypoint/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1784 2023-04-24 10:34:12.000000 bigtest_automator-0.8/entrypoint/initialize.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      713 2023-04-24 10:51:17.000000 bigtest_automator-0.8/entrypoint/main_class.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.839606 bigtest_automator-0.8/internal_db_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.8/internal_db_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1234 2023-04-24 10:34:58.000000 bigtest_automator-0.8/internal_db_management/db_ops.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.8/internal_db_management/get_server_details.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1132 2023-04-24 10:35:59.000000 bigtest_automator-0.8/internal_db_management/pwd_handler.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.840018 bigtest_automator-0.8/oracle_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.8/oracle_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.8/oracle_utils/oracle_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.8/oracle_utils/remote_oracle_db_connector.py
--rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-24 10:56:39.841628 bigtest_automator-0.8/setup.cfg
--rw-r--r--   0 shantharamp   (502) staff       (20)      670 2023-04-24 10:56:29.000000 bigtest_automator-0.8/setup.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.840448 bigtest_automator-0.8/temp/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.8/temp/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.8/temp/initiator.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.8/temp/playground.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.841123 bigtest_automator-0.8/ui_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.8/ui_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.8/ui_management/dynamic_logger.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.8/ui_management/grid.py
--rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.8/ui_management/tk_page_layouts.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.297685 bigtest_automator-0.9/
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1077 2023-04-26 15:20:07.000000 bigtest_automator-0.9/LICENSE
+-rw-r--r--   0 shantharamp   (502) staff       (20)       26 2023-04-27 04:10:40.000000 bigtest_automator-0.9/MANIFEST.in
+-rw-r--r--   0 shantharamp   (502) staff       (20)      405 2023-04-27 04:25:06.297532 bigtest_automator-0.9/PKG-INFO
+-rw-r--r--   0 shantharamp   (502) staff       (20)      110 2023-04-26 15:20:07.000000 bigtest_automator-0.9/README.md
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.292891 bigtest_automator-0.9/bigtest_automator.egg-info/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      405 2023-04-27 04:25:06.000000 bigtest_automator-0.9/bigtest_automator.egg-info/PKG-INFO
+-rw-r--r--   0 shantharamp   (502) staff       (20)      901 2023-04-27 04:25:06.000000 bigtest_automator-0.9/bigtest_automator.egg-info/SOURCES.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-27 04:25:06.000000 bigtest_automator-0.9/bigtest_automator.egg-info/dependency_links.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       61 2023-04-27 04:25:06.000000 bigtest_automator-0.9/bigtest_automator.egg-info/entry_points.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-27 04:25:06.000000 bigtest_automator-0.9/bigtest_automator.egg-info/requires.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-27 04:25:06.000000 bigtest_automator-0.9/bigtest_automator.egg-info/top_level.txt
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.294158 bigtest_automator-0.9/core_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-26 15:21:53.000000 bigtest_automator-0.9/core_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     7023 2023-04-26 15:21:53.000000 bigtest_automator-0.9/core_utils/generate_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-26 15:21:53.000000 bigtest_automator-0.9/core_utils/run_scp.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-26 15:21:53.000000 bigtest_automator-0.9/core_utils/run_vmstat.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-26 15:21:53.000000 bigtest_automator-0.9/core_utils/take_awr_snapshot.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.294730 bigtest_automator-0.9/entrypoint/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-26 15:21:53.000000 bigtest_automator-0.9/entrypoint/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1784 2023-04-26 15:21:53.000000 bigtest_automator-0.9/entrypoint/initialize.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      713 2023-04-26 15:21:53.000000 bigtest_automator-0.9/entrypoint/main_class.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.295489 bigtest_automator-0.9/internal_db_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-26 15:21:53.000000 bigtest_automator-0.9/internal_db_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1234 2023-04-26 15:21:53.000000 bigtest_automator-0.9/internal_db_management/db_ops.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-26 15:21:53.000000 bigtest_automator-0.9/internal_db_management/get_server_details.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1132 2023-04-26 15:21:53.000000 bigtest_automator-0.9/internal_db_management/pwd_handler.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.296005 bigtest_automator-0.9/oracle_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-26 15:21:53.000000 bigtest_automator-0.9/oracle_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-26 15:21:53.000000 bigtest_automator-0.9/oracle_utils/oracle_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-26 15:21:53.000000 bigtest_automator-0.9/oracle_utils/remote_oracle_db_connector.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-27 04:25:06.297732 bigtest_automator-0.9/setup.cfg
+-rw-r--r--   0 shantharamp   (502) staff       (20)      733 2023-04-27 04:23:44.000000 bigtest_automator-0.9/setup.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.296531 bigtest_automator-0.9/temp/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-26 15:21:53.000000 bigtest_automator-0.9/temp/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      456 2023-04-26 15:21:53.000000 bigtest_automator-0.9/temp/initiator.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-26 15:21:53.000000 bigtest_automator-0.9/temp/playground.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-27 04:25:06.297212 bigtest_automator-0.9/ui_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-26 15:21:53.000000 bigtest_automator-0.9/ui_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-26 15:21:53.000000 bigtest_automator-0.9/ui_management/dynamic_logger.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-26 15:21:53.000000 bigtest_automator-0.9/ui_management/grid.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-26 15:21:53.000000 bigtest_automator-0.9/ui_management/tk_page_layouts.py
```

### Comparing `bigtest_automator-0.8/bigtest_automator.egg-info/SOURCES.txt` & `bigtest_automator-0.9/bigtest_automator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+LICENSE
+MANIFEST.in
+README.md
 setup.py
 bigtest_automator.egg-info/PKG-INFO
 bigtest_automator.egg-info/SOURCES.txt
 bigtest_automator.egg-info/dependency_links.txt
 bigtest_automator.egg-info/entry_points.txt
 bigtest_automator.egg-info/requires.txt
 bigtest_automator.egg-info/top_level.txt
```

### Comparing `bigtest_automator-0.8/core_utils/generate_awr.py` & `bigtest_automator-0.9/core_utils/generate_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/core_utils/run_scp.py` & `bigtest_automator-0.9/core_utils/run_scp.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/core_utils/run_vmstat.py` & `bigtest_automator-0.9/core_utils/run_vmstat.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/core_utils/take_awr_snapshot.py` & `bigtest_automator-0.9/core_utils/take_awr_snapshot.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/entrypoint/initialize.py` & `bigtest_automator-0.9/entrypoint/initialize.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/entrypoint/main_class.py` & `bigtest_automator-0.9/entrypoint/main_class.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/internal_db_management/db_ops.py` & `bigtest_automator-0.9/internal_db_management/db_ops.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/internal_db_management/get_server_details.py` & `bigtest_automator-0.9/internal_db_management/get_server_details.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/internal_db_management/pwd_handler.py` & `bigtest_automator-0.9/internal_db_management/pwd_handler.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/oracle_utils/oracle_awr.py` & `bigtest_automator-0.9/oracle_utils/oracle_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/oracle_utils/remote_oracle_db_connector.py` & `bigtest_automator-0.9/oracle_utils/remote_oracle_db_connector.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/setup.py` & `bigtest_automator-0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bigtest_automator',
-    version='0.8',
+    version='0.9',
     author='Shantharam Puranik M',
     author_email='shantharam.puranik@ellucian.com',
     description='A small tool that helps to run and collect performance related metrics such as VMSTAT and AWR. Highly specific to my ORG, might not be useful for general public. SORRY! - Noob.',
+    url="https://github.com/mspuranika/bigtest-automator.git",
     packages=find_packages(),
     install_requires=[
         'scp',
         'paramiko',
         'oracledb'
     ],
     entry_points={
```

### Comparing `bigtest_automator-0.8/temp/playground.py` & `bigtest_automator-0.9/temp/playground.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.8/ui_management/tk_page_layouts.py` & `bigtest_automator-0.9/ui_management/tk_page_layouts.py`

 * *Files identical despite different names*

