# Comparing `tmp/Uname_sridhar-0.0.4.tar.gz` & `tmp/Uname_sridhar-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Uname_sridhar-0.0.4.tar", last modified: Sun Apr  9 02:24:26 2023, max compression
+gzip compressed data, was "Uname_sridhar-0.0.5.tar", last modified: Thu Apr 27 01:40:44 2023, max compression
```

## Comparing `Uname_sridhar-0.0.4.tar` & `Uname_sridhar-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      594 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      271 2023-04-09 02:23:20.000000 Uname_sridhar-0.0.4/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      594 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      236 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       46 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        5 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/top_level.txt
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/main/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 01:42:29.000000 Uname_sridhar-0.0.4/main/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1318 2023-04-09 01:42:30.000000 Uname_sridhar-0.0.4/main/main.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      633 2023-04-09 02:24:05.000000 Uname_sridhar-0.0.4/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-27 01:40:44.917998 Uname_sridhar-0.0.5/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      600 2023-04-27 01:40:44.917998 Uname_sridhar-0.0.5/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      271 2023-04-09 02:23:20.000000 Uname_sridhar-0.0.5/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-27 01:40:44.917998 Uname_sridhar-0.0.5/Uname_sridhar.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      600 2023-04-27 01:40:44.000000 Uname_sridhar-0.0.5/Uname_sridhar.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      236 2023-04-27 01:40:44.000000 Uname_sridhar-0.0.5/Uname_sridhar.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-27 01:40:44.000000 Uname_sridhar-0.0.5/Uname_sridhar.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       46 2023-04-27 01:40:44.000000 Uname_sridhar-0.0.5/Uname_sridhar.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        5 2023-04-27 01:40:44.000000 Uname_sridhar-0.0.5/Uname_sridhar.egg-info/top_level.txt
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-27 01:40:44.917998 Uname_sridhar-0.0.5/main/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 01:42:29.000000 Uname_sridhar-0.0.5/main/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1318 2023-04-09 01:42:30.000000 Uname_sridhar-0.0.5/main/main.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-27 01:40:44.917998 Uname_sridhar-0.0.5/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      639 2023-04-27 01:39:57.000000 Uname_sridhar-0.0.5/setup.py
```

### Comparing `Uname_sridhar-0.0.4/main/main.py` & `Uname_sridhar-0.0.5/main/main.py`

 * *Files identical despite different names*

### Comparing `Uname_sridhar-0.0.4/setup.py` & `Uname_sridhar-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Uname_sridhar',
-    version='0.0.4',
+    version='0.0.5',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
-    description='Get Information About Current Linux Kernel With Python',
+    description='Get Information About  Linux Kernel with the help of  Python',
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/package_uname_command',
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'Uname_cli=main.main:main',
```

