# Comparing `tmp/sar_handler-0.1.0.tar.gz` & `tmp/sar_handler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sar_handler-0.1.0.tar", last modified: Thu Apr 27 08:56:36 2023, max compression
+gzip compressed data, was "sar_handler-0.1.2.tar", last modified: Thu Apr 27 10:49:07 2023, max compression
```

## Comparing `sar_handler-0.1.0.tar` & `sar_handler-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:56:36.405187 sar_handler-0.1.0/
--rw-rw-rw-   0        0        0      203 2023-04-27 08:56:36.404187 sar_handler-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-27 07:59:22.000000 sar_handler-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 08:56:36.388188 sar_handler-0.1.0/sar_handler/
--rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.0/sar_handler/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-27 08:24:14.000000 sar_handler-0.1.0/sar_handler/first_func.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:56:36.401202 sar_handler-0.1.0/sar_handler.egg-info/
--rw-rw-rw-   0        0        0      203 2023-04-27 08:56:36.000000 sar_handler-0.1.0/sar_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-27 08:56:36.000000 sar_handler-0.1.0/sar_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 08:56:36.000000 sar_handler-0.1.0/sar_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 08:56:36.000000 sar_handler-0.1.0/sar_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 08:56:36.000000 sar_handler-0.1.0/sar_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 08:56:36.405187 sar_handler-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-27 08:40:27.000000 sar_handler-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:49:07.532773 sar_handler-0.1.2/
+-rw-rw-rw-   0        0        0      203 2023-04-27 10:49:07.532773 sar_handler-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-27 07:59:22.000000 sar_handler-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 10:49:07.519776 sar_handler-0.1.2/sar_handler/
+-rw-rw-rw-   0        0        0     9353 2023-03-07 18:48:04.000000 sar_handler-0.1.2/sar_handler/FC_Classifier.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:07:11.000000 sar_handler-0.1.2/sar_handler/__init__.py
+-rw-rw-rw-   0        0        0     4268 2023-04-27 09:32:47.000000 sar_handler-0.1.2/sar_handler/assistive_funcs.py
+-rw-rw-rw-   0        0        0      918 2022-10-11 07:49:15.000000 sar_handler-0.1.2/sar_handler/check_validity_of_values.py
+-rw-rw-rw-   0        0        0     4381 2023-03-01 10:44:04.000000 sar_handler-0.1.2/sar_handler/csv_dataloader.py
+-rw-rw-rw-   0        0        0     9321 2023-03-01 09:31:44.000000 sar_handler-0.1.2/sar_handler/dataset_creator.py
+-rw-rw-rw-   0        0        0    10185 2023-04-27 10:17:07.000000 sar_handler-0.1.2/sar_handler/fastaniso.py
+-rw-rw-rw-   0        0        0     3445 2023-02-26 12:09:17.000000 sar_handler-0.1.2/sar_handler/image_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:49:07.530772 sar_handler-0.1.2/sar_handler.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 10:49:07.000000 sar_handler-0.1.2/sar_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:49:07.533774 sar_handler-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      609 2023-04-27 10:39:07.000000 sar_handler-0.1.2/setup.py
```

