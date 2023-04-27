# Comparing `tmp/orthanc_tools-0.8.4.tar.gz` & `tmp/orthanc_tools-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc_tools-0.8.4.tar", last modified: Wed Apr 12 08:49:44 2023, max compression
+gzip compressed data, was "orthanc_tools-0.8.7.tar", last modified: Thu Apr 27 17:23:35 2023, max compression
```

## Comparing `orthanc_tools-0.8.4.tar` & `orthanc_tools-0.8.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.212294 orthanc_tools-0.8.4/orthanc_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/orthanc_tools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/old_files_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/time_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_series_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_worklist_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_cloner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_folder_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_test_db_populator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/pacs_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/orthanc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/release-notes.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/tests/test_3_orthancs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/tests/test_old_files_deleter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.935842 orthanc_tools-0.8.7/orthanc_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.935842 orthanc_tools-0.8.7/orthanc_tools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/old_files_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/time_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_series_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_worklist_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_cloner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_folder_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_test_db_populator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/pacs_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.935842 orthanc_tools-0.8.7/orthanc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/tests/test_3_orthancs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/tests/test_old_files_deleter.py
```

### Comparing `orthanc_tools-0.8.4/LICENSE.txt` & `orthanc_tools-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/PKG-INFO` & `orthanc_tools-0.8.7/orthanc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: orthanc_tools
-Version: 0.8.4
+Name: orthanc-tools
+Version: 0.8.7
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.4/README.md` & `orthanc_tools-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/__init__.py` & `orthanc_tools-0.8.7/orthanc_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/helpers/old_files_deleter.py` & `orthanc_tools-0.8.7/orthanc_tools/helpers/old_files_deleter.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/helpers/scheduler.py` & `orthanc_tools-0.8.7/orthanc_tools/helpers/scheduler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/helpers/time_out.py` & `orthanc_tools-0.8.7/orthanc_tools/helpers/time_out.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/helpers/timer.py` & `orthanc_tools-0.8.7/orthanc_tools/helpers/timer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/__init__.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_client.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_error.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_error.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_parser.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_validator.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_validator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_parser.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_series_builder.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_series_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_server.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_server.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_worklist_parser.py` & `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_worklist_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/orthanc_cloner.py` & `orthanc_tools-0.8.7/orthanc_tools/orthanc_cloner.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/orthanc_comparator.py` & `orthanc_tools-0.8.7/orthanc_tools/orthanc_comparator.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,18 +89,17 @@
                     remote_match = [r for r in remote_studies if r.dicom_id == local_study.dicom_id]
                     study_summary = f"{local_study.patient_main_dicom_tags.get('PatientID')} - {local_study.patient_main_dicom_tags.get('PatientName')} - {local_study.main_dicom_tags.get('StudyDescription')}"
 
                     if len(remote_match) == 0 and not self._ignore_missing_on_modality:
                         logger.warning(f"WARNING {str(current_date)}, study missing on modality: {study_summary}")
                         if self._transfer_missing_to_modality:
                             logger.warning(f"WARNING {str(current_date)}, transferring study to modality: {study_summary}")
-                            self._api_client.modalities.store(
+                            self._api_client.modalities.send(
                                 target_modality=self._modality,
-                                resources_ids=local_study.orthanc_id,
-                                synchronous=True
+                                resources_ids=local_study.orthanc_id
                             )
                     elif len(remote_match) > 1:
                         logger.warning(f"WARNING {str(current_date)}, study found multiple times on modality: {study_summary}")
                     elif len(remote_match) == 1:
                         if self._level in ['Series', 'Instance']:
                             self.compare_study(orthanc_id=local_study.orthanc_id, dicom_id=local_study.dicom_id, study_summary=study_summary)
                 except Exception as ex:
@@ -151,18 +150,17 @@
             for local_serie in local_series:
                 local_dicom_id = local_serie.get('MainDicomTags').get('SeriesInstanceUID')
                 remote_match = [r for r in remote_series if r.dicom_id == local_dicom_id]
                 if len(remote_match) == 0 and not self._ignore_missing_on_modality:
                     logger.warning(f"WARNING STUDY {study_summary}, series missing from modality: {local_dicom_id}")
                     if self._transfer_missing_to_modality:
                         logger.warning(f"WARNING STUDY {study_summary}, transferring series to modality: {local_dicom_id}")
-                        self._api_client.modalities.store(
+                        self._api_client.modalities.send(
                             target_modality=self._modality,
-                            resources_ids=local_serie.get('ID'),
-                            synchronous=True
+                            resources_ids=local_serie.get('ID')
                         )
                 elif len(remote_match) > 1:
                     logger.warning(f"WARNING STUDY {study_summary}, series found multiple times on modality: {local_dicom_id}")
                 elif len(remote_match) == 1:
                     series_summary = f"{local_dicom_id} (from STUDY {study_summary})"
                     if self._level in ['Instance']:
                         self.compare_series(
@@ -212,18 +210,17 @@
                     local_dicom_id = local_instance.get('MainDicomTags').get('SOPInstanceUID')
                     remote_match = [r for r in remote_instances if r.dicom_id == local_dicom_id]
 
                     if len(remote_match) == 0 and not self._ignore_missing_on_modality:
                         logger.warning(f"WARNING SERIES {series_summary}, instance missing from modality: {local_dicom_id}")
                         if self._transfer_missing_to_modality:
                             logger.warning(f"WARNING SERIES {series_summary}, transferring instance to modality: {local_dicom_id}")
-                            self._api_client.modalities.store(
+                            self._api_client.modalities.send(
                                 target_modality=self._modality,
-                                resources_ids=local_instance.get('ID'),
-                                synchronous=True
+                                resources_ids=local_instance.get('ID')
                             )
                             success_count += 1
                     elif len(remote_match) > 1:
                         logger.warning(f"WARNING SERIES {series_summary}, instance found multiple times on modality: {local_dicom_id}")
                 except:
                     failure_count += 1
```

### Comparing `orthanc_tools-0.8.4/orthanc_tools/orthanc_folder_importer.py` & `orthanc_tools-0.8.7/orthanc_tools/orthanc_folder_importer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/orthanc_forwarder.py` & `orthanc_tools-0.8.7/orthanc_tools/orthanc_forwarder.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,16 +317,15 @@
                 target_modality=destination.destination,
                 resources_ids=instances_set.instances_ids
             )
         elif destination.forwarder_mode == ForwarderMode.DICOM_SERIES_BY_SERIES:
             for s in instances_set.series_ids:
                 self._source.modalities.send(
                     target_modality=destination.destination,
-                    resources_ids=instances_set.get_instances_ids(series_id=s),
-                    synchronous=True
+                    resources_ids=instances_set.get_instances_ids(series_id=s)
                 )
         elif destination.forwarder_mode == ForwarderMode.DICOM_WEB:
             for s in instances_set.series_ids:
                 self._source.dicomweb_servers.send(
                     target_server=destination.destination,
                     resources_ids=instances_set.get_instances_ids(series_id=s)
                 )
```

### Comparing `orthanc_tools-0.8.4/orthanc_tools/orthanc_monitor.py` & `orthanc_tools-0.8.7/orthanc_tools/orthanc_monitor.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/orthanc_tools/orthanc_test_db_populator.py` & `orthanc_tools-0.8.7/orthanc_tools/orthanc_test_db_populator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,25 @@
     """
     Populates an Orthanc with a test DB
     """
 
     def __init__(self,
                  api_client: OrthancApiClient,
                  studies_count: int,
+                 series_count: int = None,                  # to force the number of series in a study
+                 instances_count: int = None,               # to force the number of instances in a study
                  random_seed: int = None,                   # to make the generation repeatable
                  from_study_date: datetime.date = datetime.date(2000, 1, 1),     # StudyDate for generated studies
                  to_study_date: datetime.date = datetime.date(2022, 4, 21)        # StudyDate for generated studies
                  ):
 
         self._api_client = api_client
         self._studies_count = studies_count
+        self._series_count = series_count
+        self._instances_count = instances_count
         self._random_seed = random_seed
         self._patient_counter = 1
         self._from_study_date = from_study_date
         self._to_study_date = to_study_date
 
     def generate_patient_tags(self, tags: object) -> object:
         # generate a pseudo patient
@@ -111,20 +115,26 @@
             if random.randint(0, 10) > 7:  # change patients every now and then
                 tags = self.generate_patient_tags(tags)
 
             tags = self.generate_study_tags(tags, study_counter)
 
             logger.info(f"-created study {tags['StudyDescription']}")
 
-            series_count = random.randint(1, 6)
+            if self._series_count is not None:
+                series_count = self._series_count
+            else:
+                series_count = random.randint(1, 6)
             for series_counter in range(0, series_count):
                 tags = self.generate_series_tags(tags, series_counter, study_counter)
 
                 if tags["Modality"] in ["MR", "CT"]:
-                    instances_count = random.randint(50, 150)
+                    if self._instances_count is not None:
+                        instances_count = self._instances_count
+                    else:
+                        instances_count = random.randint(50, 150)
                 else:
                     instances_count = 1
 
                 logger.info(f"--created series {tags['Modality']} with {instances_count} instances")
 
                 for instance_counter in range(0, instances_count):
                     tags = self.generate_instance_tags(tags, instance_counter, series_counter, study_counter)
```

### Comparing `orthanc_tools-0.8.4/orthanc_tools/pacs_migrator.py` & `orthanc_tools-0.8.7/orthanc_tools/pacs_migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,15 @@
 
             if self.source_is_orthanc:
                 try:
                     logger.info(f"C-Store study {message.orthanc_id} from orthanc to destination modality {self._destination_modality}")
                     # move the study from orthanc to the target modality
                     self._api_client.modalities.send(
                         target_modality=self._destination_modality,
-                        resources_ids=message.orthanc_id,
-                        synchronous=True
+                        resources_ids=message.orthanc_id
                     )
 
                     if self._delete_from_source:
                         self._api_client.studies.delete(
                             orthanc_id=message.orthanc_id
                         )
                 except Exception as ex:
@@ -154,15 +153,15 @@
 
             self._messages.task_done()  # tell the queue the item has been processed
 
         logger.debug(f"Processing thread {worker_thread_id} stopped")
 
     def push_message(self, message: Message):
         if self._scheduler:
-            self._scheduler.wait_right_time_to_run(logger=logger)
+            self._scheduler.wait_right_time_to_run()
 
         self._messages.put(message)
 
 
     def execute(self):
         if self._is_running:
             raise RuntimeError("Migrator is already running")
```

### Comparing `orthanc_tools-0.8.4/orthanc_tools.egg-info/PKG-INFO` & `orthanc_tools-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: orthanc-tools
-Version: 0.8.4
+Name: orthanc_tools
+Version: 0.8.7
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.4/orthanc_tools.egg-info/SOURCES.txt` & `orthanc_tools-0.8.7/orthanc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.4/release-notes.md` & `orthanc_tools-0.8.7/release-notes.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v 0.8.6
+=======
+
+- `OrthancTestDbPopulator`: new feature: number of series/instances
+
+v 0.8.5
+=======
+
+- `PacsMigrator`: fix push_message method
+
 v 0.8.4
 =======
 
 - `OrthancForwarder`: added error logs + retry in case of ConnectionError
 - `OrthancForwarder`: removed `worker_threads_count` that was not used anymore
 
 v 0.8.3
```

### Comparing `orthanc_tools-0.8.4/setup.py` & `orthanc_tools-0.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.8.4',  # Required
+    version='0.8.7',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python Orthanc Tools',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -126,15 +126,15 @@
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
         'requests',
-        'orthanc-api-client>=0.11.8',
+        'orthanc-api-client>=0.12.2',
         'pydicom>=2.3.1',
         'hl7==0.4.2',
         'six'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
```

### Comparing `orthanc_tools-0.8.4/tests/test_3_orthancs.py` & `orthanc_tools-0.8.7/tests/test_3_orthancs.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,29 @@
         populator_b = OrthancTestDbPopulator(api_client=self.ob, studies_count=2, random_seed=42)
 
         populator_a.execute()
         populator_b.execute()
 
         self.assertEqual(self.oa.instances.get_all_ids(), self.ob.instances.get_all_ids())
 
+    def test_populator_repeatability_with_forced_quantities(self):
+        self.oa.delete_all_content()
+        self.ob.delete_all_content()
+
+        populator_a = OrthancTestDbPopulator(api_client=self.oa, studies_count=2, random_seed=42, series_count=1, instances_count=1)
+        populator_b = OrthancTestDbPopulator(api_client=self.ob, studies_count=2, random_seed=42, series_count=1, instances_count=1)
+
+        populator_a.execute()
+        populator_b.execute()
+
+        a_ids = self.oa.instances.get_all_ids()
+        b_ids = self.ob.instances.get_all_ids()
+        self.assertEqual(a_ids, b_ids)
+        self.assertEqual(len(a_ids), 2)
+
 
     def test_monitor_recovery(self):
         with tempfile.TemporaryDirectory() as temp_dir:
             persist_status_path = os.path.join(temp_dir, 'seq.txt')
 
             processed_resources = []
```

### Comparing `orthanc_tools-0.8.4/tests/test_old_files_deleter.py` & `orthanc_tools-0.8.7/tests/test_old_files_deleter.py`

 * *Files identical despite different names*

