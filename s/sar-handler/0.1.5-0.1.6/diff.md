# Comparing `tmp/sar_handler-0.1.5.tar.gz` & `tmp/sar_handler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sar_handler-0.1.5.tar", last modified: Thu Apr 27 12:23:43 2023, max compression
+gzip compressed data, was "sar_handler-0.1.6.tar", last modified: Thu Apr 27 13:02:57 2023, max compression
```

## Comparing `sar_handler-0.1.5.tar` & `sar_handler-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:23:43.468683 sar_handler-0.1.5/
--rw-rw-rw-   0        0        0     1057 2023-04-27 11:30:14.000000 sar_handler-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      511 2023-04-27 12:23:43.467682 sar_handler-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-27 10:58:50.000000 sar_handler-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:23:43.455681 sar_handler-0.1.5/sar_handler/
--rw-rw-rw-   0        0        0     9353 2023-03-07 18:48:04.000000 sar_handler-0.1.5/sar_handler/FC_Classifier.py
--rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.5/sar_handler/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-04-27 12:20:24.000000 sar_handler-0.1.5/sar_handler/assistive_funcs.py
--rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.5/sar_handler/check_validity_of_values.py
--rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.5/sar_handler/csv_dataloader.py
--rw-rw-rw-   0        0        0     9324 2023-04-27 12:20:58.000000 sar_handler-0.1.5/sar_handler/dataset_creator.py
--rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.5/sar_handler/fastaniso.py
--rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.5/sar_handler/image_processing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:23:43.466682 sar_handler-0.1.5/sar_handler.egg-info/
--rw-rw-rw-   0        0        0      511 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 12:23:43.000000 sar_handler-0.1.5/sar_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 12:23:43.469682 sar_handler-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-27 12:22:30.000000 sar_handler-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:02:57.495122 sar_handler-0.1.6/
+-rw-rw-rw-   0        0        0     1057 2023-04-27 11:30:14.000000 sar_handler-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      511 2023-04-27 13:02:57.494117 sar_handler-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-27 10:58:50.000000 sar_handler-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 13:02:57.454121 sar_handler-0.1.6/sar_handler/
+-rw-rw-rw-   0        0        0      143 2023-04-27 12:58:27.000000 sar_handler-0.1.6/sar_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:02:57.493117 sar_handler-0.1.6/sar_handler.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-04-27 13:02:57.000000 sar_handler-0.1.6/sar_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-04-27 13:02:57.000000 sar_handler-0.1.6/sar_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:02:57.000000 sar_handler-0.1.6/sar_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 13:02:57.000000 sar_handler-0.1.6/sar_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 13:02:57.000000 sar_handler-0.1.6/sar_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:02:57.496118 sar_handler-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2023-04-27 12:59:26.000000 sar_handler-0.1.6/setup.py
```

### Comparing `sar_handler-0.1.5/LICENSE` & `sar_handler-0.1.6/LICENSE`

 * *Files identical despite different names*

