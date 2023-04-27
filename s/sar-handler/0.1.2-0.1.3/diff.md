# Comparing `tmp/sar_handler-0.1.2.tar.gz` & `tmp/sar_handler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sar_handler-0.1.2.tar", last modified: Thu Apr 27 10:49:07 2023, max compression
+gzip compressed data, was "sar_handler-0.1.3.tar", last modified: Thu Apr 27 11:00:02 2023, max compression
```

## Comparing `sar_handler-0.1.2.tar` & `sar_handler-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 10:49:07.532773 sar_handler-0.1.2/
--rw-rw-rw-   0        0        0      203 2023-04-27 10:49:07.532773 sar_handler-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-27 07:59:22.000000 sar_handler-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 10:49:07.519776 sar_handler-0.1.2/sar_handler/
--rw-rw-rw-   0        0        0     9353 2023-03-07 18:48:04.000000 sar_handler-0.1.2/sar_handler/FC_Classifier.py
--rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.2/sar_handler/__init__.py
--rw-rw-rw-   0        0        0     4268 2023-04-27 09:32:47.000000 sar_handler-0.1.2/sar_handler/assistive_funcs.py
--rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.2/sar_handler/check_validity_of_values.py
--rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.2/sar_handler/csv_dataloader.py
--rw-rw-rw-   0        0        0     9321 2023-03-01 09:31:44.000000 sar_handler-0.1.2/sar_handler/dataset_creator.py
--rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.2/sar_handler/fastaniso.py
--rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.2/sar_handler/image_processing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 10:49:07.530772 sar_handler-0.1.2/sar_handler.egg-info/
--rw-rw-rw-   0        0        0      203 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 10:49:07.533774 sar_handler-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      609 2023-04-27 10:39:07.000000 sar_handler-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:00:02.938172 sar_handler-0.1.3/
+-rw-rw-rw-   0        0        0      203 2023-04-27 11:00:02.938172 sar_handler-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-27 10:58:50.000000 sar_handler-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 11:00:02.915172 sar_handler-0.1.3/sar_handler/
+-rw-rw-rw-   0        0        0     9353 2023-03-07 18:48:04.000000 sar_handler-0.1.3/sar_handler/FC_Classifier.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.3/sar_handler/__init__.py
+-rw-rw-rw-   0        0        0     4268 2023-04-27 09:32:47.000000 sar_handler-0.1.3/sar_handler/assistive_funcs.py
+-rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.3/sar_handler/check_validity_of_values.py
+-rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.3/sar_handler/csv_dataloader.py
+-rw-rw-rw-   0        0        0     9321 2023-03-01 09:31:44.000000 sar_handler-0.1.3/sar_handler/dataset_creator.py
+-rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.3/sar_handler/fastaniso.py
+-rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.3/sar_handler/image_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:00:02.937173 sar_handler-0.1.3/sar_handler.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-04-27 11:00:02.000000 sar_handler-0.1.3/sar_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-27 11:00:02.000000 sar_handler-0.1.3/sar_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:00:02.000000 sar_handler-0.1.3/sar_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 11:00:02.000000 sar_handler-0.1.3/sar_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 11:00:02.000000 sar_handler-0.1.3/sar_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 11:00:02.939172 sar_handler-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      609 2023-04-27 10:59:30.000000 sar_handler-0.1.3/setup.py
```

### Comparing `sar_handler-0.1.2/sar_handler/FC_Classifier.py` & `sar_handler-0.1.3/sar_handler/FC_Classifier.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/sar_handler/assistive_funcs.py` & `sar_handler-0.1.3/sar_handler/assistive_funcs.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/sar_handler/check_validity_of_values.py` & `sar_handler-0.1.3/sar_handler/check_validity_of_values.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/sar_handler/csv_dataloader.py` & `sar_handler-0.1.3/sar_handler/csv_dataloader.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/sar_handler/dataset_creator.py` & `sar_handler-0.1.3/sar_handler/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/sar_handler/fastaniso.py` & `sar_handler-0.1.3/sar_handler/fastaniso.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/sar_handler/image_processing.py` & `sar_handler-0.1.3/sar_handler/image_processing.py`

 * *Files identical despite different names*

### Comparing `sar_handler-0.1.2/setup.py` & `sar_handler-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='sar_handler',
     packages=find_packages(include=['sar_handler']),
-    version='0.1.2',
+    version='0.1.3',
     description='Handler SAR images',
     author='Felecort',
     # author_email="@gmail.com",
     url="https://github.com/Felecort/SAR_Handler",
     license='MIT',
     install_requires=["numpy",
                       "Pillow",
```

