# Comparing `tmp/pandasflow-0.4.2.tar.gz` & `tmp/pandasflow-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.4.2.tar", last modified: Wed Apr 26 15:21:29 2023, max compression
+gzip compressed data, was "pandasflow-0.4.3.tar", last modified: Thu Apr 27 15:26:41 2023, max compression
```

## Comparing `pandasflow-0.4.2.tar` & `pandasflow-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.913318 pandasflow-0.4.2/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.2/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-26 15:21:29.913318 pandasflow-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.900862 pandasflow-0.4.2/pandasflow/
--rw-rw-rw-   0        0        0      296 2023-04-26 15:21:24.000000 pandasflow-0.4.2/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.904851 pandasflow-0.4.2/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.2/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.2/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      441 2023-04-26 15:12:42.000000 pandasflow-0.4.2/pandasflow/get_import.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.906847 pandasflow-0.4.2/pandasflow/metrics/
--rw-rw-rw-   0        0        0      120 2023-04-26 14:24:20.000000 pandasflow-0.4.2/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.2/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.2/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.2/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.907843 pandasflow-0.4.2/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.2/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.910236 pandasflow-0.4.2/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.2/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.2/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.2/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.903854 pandasflow-0.4.2/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-26 15:21:29.000000 pandasflow-0.4.2/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2023-04-26 15:21:29.000000 pandasflow-0.4.2/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:21:29.000000 pandasflow-0.4.2/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-26 15:21:29.000000 pandasflow-0.4.2/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-26 15:21:29.000000 pandasflow-0.4.2/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 15:21:29.913318 pandasflow-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:29.913318 pandasflow-0.4.2/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.2/test/__init__.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.2/test/split_tvt_test.py
--rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.4.2/test/test_get_column_name.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.2/test/test_lloss_up.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.2/test/test_mean_error.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.2/test/test_split_tt.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.972189 pandasflow-0.4.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.3/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-27 15:26:41.972189 pandasflow-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.961214 pandasflow-0.4.3/pandasflow/
+-rw-rw-rw-   0        0        0      294 2023-04-27 15:23:21.000000 pandasflow-0.4.3/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.965203 pandasflow-0.4.3/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.3/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.3/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      355 2023-04-27 14:33:43.000000 pandasflow-0.4.3/pandasflow/get_import.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.967198 pandasflow-0.4.3/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      168 2023-04-27 14:37:44.000000 pandasflow-0.4.3/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1180 2023-04-27 15:22:37.000000 pandasflow-0.4.3/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.3/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.3/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.3/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.967198 pandasflow-0.4.3/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.3/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.969194 pandasflow-0.4.3/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.3/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.3/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.3/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.964206 pandasflow-0.4.3/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-27 15:26:41.000000 pandasflow-0.4.3/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 15:26:41.973187 pandasflow-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:26:41.972189 pandasflow-0.4.3/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.3/test/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.3/test/split_tvt_test.py
+-rw-rw-rw-   0        0        0      734 2023-04-27 14:51:02.000000 pandasflow-0.4.3/test/test_conf_mat.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.3/test/test_lloss_up.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.3/test/test_mean_error.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.3/test/test_split_tt.py
```

### Comparing `pandasflow-0.4.2/LICENCE` & `pandasflow-0.4.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/PKG-INFO` & `pandasflow-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.2
+Version: 0.4.3
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.2/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.4.3/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/pandasflow/metrics/lloss_up.py` & `pandasflow-0.4.3/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/pandasflow/reset_mi.py` & `pandasflow-0.4.3/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/pandasflow/split/train_test.py` & `pandasflow-0.4.3/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/pandasflow/split/train_valid_test.py` & `pandasflow-0.4.3/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.4.3/pandasflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.2
+Version: 0.4.3
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.2/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.4.3/pandasflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
 pandasflow/dev/__init__.py
 pandasflow/dev/err_mean_diff.py
 pandasflow/metrics/__init__.py
+pandasflow/metrics/conf_mat.py
 pandasflow/metrics/lloss_up.py
 pandasflow/metrics/mean_error.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
 test/split_tvt_test.py
-test/test_get_column_name.py
+test/test_conf_mat.py
 test/test_lloss_up.py
 test/test_mean_error.py
 test/test_split_tt.py
```

### Comparing `pandasflow-0.4.2/setup.py` & `pandasflow-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/test/split_tvt_test.py` & `pandasflow-0.4.3/test/split_tvt_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.2/test/test_lloss_up.py` & `pandasflow-0.4.3/test/test_lloss_up.py`

 * *Files identical despite different names*

