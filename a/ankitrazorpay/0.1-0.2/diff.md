# Comparing `tmp/ankitrazorpay-0.1.tar.gz` & `tmp/ankitrazorpay-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ankitrazorpay-0.1.tar", last modified: Wed Apr 19 10:10:06 2023, max compression
+gzip compressed data, was "ankitrazorpay-0.2.tar", last modified: Thu Apr 27 09:11:46 2023, max compression
```

## Comparing `ankitrazorpay-0.1.tar` & `ankitrazorpay-0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 ankit.das   (503) admin       (80)        0 2023-04-19 10:10:06.552760 ankitrazorpay-0.1/
--rw-r--r--   0 ankit.das   (503) admin       (80)      547 2023-04-19 10:10:06.552483 ankitrazorpay-0.1/PKG-INFO
-drwxr-xr-x   0 ankit.das   (503) admin       (80)        0 2023-04-19 10:10:06.552044 ankitrazorpay-0.1/ankitrazorpay.egg-info/
--rw-r--r--   0 ankit.das   (503) admin       (80)      547 2023-04-19 10:10:06.000000 ankitrazorpay-0.1/ankitrazorpay.egg-info/PKG-INFO
--rw-r--r--   0 ankit.das   (503) admin       (80)      156 2023-04-19 10:10:06.000000 ankitrazorpay-0.1/ankitrazorpay.egg-info/SOURCES.txt
--rw-r--r--   0 ankit.das   (503) admin       (80)        1 2023-04-19 10:10:06.000000 ankitrazorpay-0.1/ankitrazorpay.egg-info/dependency_links.txt
--rw-r--r--   0 ankit.das   (503) admin       (80)        1 2023-04-19 10:10:06.000000 ankitrazorpay-0.1/ankitrazorpay.egg-info/top_level.txt
--rw-r--r--   0 ankit.das   (503) admin       (80)       38 2023-04-19 10:10:06.552877 ankitrazorpay-0.1/setup.cfg
--rw-r--r--   0 ankit.das   (503) admin       (80)      665 2023-04-18 08:53:46.000000 ankitrazorpay-0.1/setup.py
+drwxr-xr-x   0 ankit.das   (503) admin       (80)        0 2023-04-27 09:11:46.858905 ankitrazorpay-0.2/
+-rw-r--r--   0 ankit.das   (503) admin       (80)     2097 2023-04-27 09:11:46.858662 ankitrazorpay-0.2/PKG-INFO
+-rw-r--r--   0 ankit.das   (503) admin       (80)     1509 2023-04-19 14:10:01.000000 ankitrazorpay-0.2/README.md
+drwxr-xr-x   0 ankit.das   (503) admin       (80)        0 2023-04-27 09:11:46.858174 ankitrazorpay-0.2/ankitrazorpay.egg-info/
+-rw-r--r--   0 ankit.das   (503) admin       (80)     2097 2023-04-27 09:11:46.000000 ankitrazorpay-0.2/ankitrazorpay.egg-info/PKG-INFO
+-rw-r--r--   0 ankit.das   (503) admin       (80)      166 2023-04-27 09:11:46.000000 ankitrazorpay-0.2/ankitrazorpay.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit.das   (503) admin       (80)        1 2023-04-27 09:11:46.000000 ankitrazorpay-0.2/ankitrazorpay.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit.das   (503) admin       (80)        1 2023-04-27 09:11:46.000000 ankitrazorpay-0.2/ankitrazorpay.egg-info/top_level.txt
+-rw-r--r--   0 ankit.das   (503) admin       (80)       38 2023-04-27 09:11:46.858959 ankitrazorpay-0.2/setup.cfg
+-rw-r--r--   0 ankit.das   (503) admin       (80)      823 2023-04-27 09:11:37.000000 ankitrazorpay-0.2/setup.py
```

