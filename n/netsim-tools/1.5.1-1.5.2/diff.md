# Comparing `tmp/netsim-tools-1.5.1.tar.gz` & `tmp/netsim-tools-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim-tools-1.5.1.tar", last modified: Sun Apr  2 11:35:17 2023, max compression
+gzip compressed data, was "netsim-tools-1.5.2.tar", last modified: Thu Apr 27 06:48:34 2023, max compression
```

## Comparing `netsim-tools-1.5.1.tar` & `netsim-tools-1.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-02 11:35:17.689239 netsim-tools-1.5.1/
--rw-r--r--   0 pipi       (501) staff       (20)      493 2023-04-02 11:35:17.689125 netsim-tools-1.5.1/PKG-INFO
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-02 11:35:17.688987 netsim-tools-1.5.1/netsim_tools.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)      493 2023-04-02 11:35:17.000000 netsim-tools-1.5.1/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)      187 2023-04-02 11:35:17.000000 netsim-tools-1.5.1/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-02 11:35:17.000000 netsim-tools-1.5.1/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       18 2023-04-02 11:35:17.000000 netsim-tools-1.5.1/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-02 11:35:17.000000 netsim-tools-1.5.1/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-04-02 11:35:17.689271 netsim-tools-1.5.1/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1292 2023-04-02 11:32:00.000000 netsim-tools-1.5.1/setup.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:34.957301 netsim-tools-1.5.2/
+-rw-r--r--   0 pipi       (501) staff       (20)      493 2023-04-27 06:48:34.957178 netsim-tools-1.5.2/PKG-INFO
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:34.957032 netsim-tools-1.5.2/netsim_tools.egg-info/
+-rw-r--r--   0 pipi       (501) staff       (20)      493 2023-04-27 06:48:34.000000 netsim-tools-1.5.2/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)      187 2023-04-27 06:48:34.000000 netsim-tools-1.5.2/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-27 06:48:34.000000 netsim-tools-1.5.2/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       18 2023-04-27 06:48:34.000000 netsim-tools-1.5.2/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-27 06:48:34.000000 netsim-tools-1.5.2/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       38 2023-04-27 06:48:34.957337 netsim-tools-1.5.2/setup.cfg
+-rw-r--r--   0 pipi       (501) staff       (20)     1292 2023-04-27 06:46:29.000000 netsim-tools-1.5.2/setup.py
```

### Comparing `netsim-tools-1.5.1/setup.py` & `netsim-tools-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
 
 sys.path.append('..')
 
-version="1.5.1"
+version="1.5.2"
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
   author="Ivan Pepelnjak",
   author_email="ip@ipspace.net",
```

