# Comparing `tmp/culturalconformity-0.0.4.tar.gz` & `tmp/culturalconformity-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culturalconformity-0.0.4.tar", last modified: Wed Apr 26 07:43:39 2023, max compression
+gzip compressed data, was "culturalconformity-0.0.6.tar", last modified: Wed Apr 26 22:39:41 2023, max compression
```

## Comparing `culturalconformity-0.0.4.tar` & `culturalconformity-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 07:43:39.079377 culturalconformity-0.0.4/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 07:43:39.079213 culturalconformity-0.0.4/PKG-INFO
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 07:43:39.078327 culturalconformity-0.0.4/culturalconformity/
--rw-r--r--   0 kaledadenton   (501) staff       (20)       41 2023-04-26 07:24:23.000000 culturalconformity-0.0.4/culturalconformity/__init__.py
--rw-r--r--   0 kaledadenton   (501) staff       (20)      997 2023-04-26 07:41:47.000000 culturalconformity-0.0.4/culturalconformity/frq_over_time.py
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 07:43:39.079024 culturalconformity-0.0.4/culturalconformity.egg-info/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 07:43:39.000000 culturalconformity-0.0.4/culturalconformity.egg-info/PKG-INFO
--rw-r--r--   0 kaledadenton   (501) staff       (20)      243 2023-04-26 07:43:39.000000 culturalconformity-0.0.4/culturalconformity.egg-info/SOURCES.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 07:43:39.000000 culturalconformity-0.0.4/culturalconformity.egg-info/dependency_links.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       19 2023-04-26 07:43:39.000000 culturalconformity-0.0.4/culturalconformity.egg-info/top_level.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 07:43:39.079435 culturalconformity-0.0.4/setup.cfg
--rw-r--r--   0 kaledadenton   (501) staff       (20)      976 2023-04-26 07:43:36.000000 culturalconformity-0.0.4/setup.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 22:39:41.013348 culturalconformity-0.0.6/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 22:39:41.013082 culturalconformity-0.0.6/PKG-INFO
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 22:39:41.012306 culturalconformity-0.0.6/culturalconformity/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       80 2023-04-26 22:39:28.000000 culturalconformity-0.0.6/culturalconformity/__init__.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)     3922 2023-04-26 22:38:29.000000 culturalconformity-0.0.6/culturalconformity/frq_over_time.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)     7139 2023-04-26 22:39:28.000000 culturalconformity-0.0.6/culturalconformity/interactive.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 22:39:41.012876 culturalconformity-0.0.6/culturalconformity.egg-info/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/PKG-INFO
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      277 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/SOURCES.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/dependency_links.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       19 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/top_level.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 22:39:41.013428 culturalconformity-0.0.6/setup.cfg
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      976 2023-04-26 22:36:54.000000 culturalconformity-0.0.6/setup.py
```

### Comparing `culturalconformity-0.0.4/setup.py` & `culturalconformity-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.6'
 DESCRIPTION = 'Simulations of conformity, anti-conformity, and unbiased frequency-dependent transmission'
 # LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
     name="culturalconformity",
     version=VERSION,
```

