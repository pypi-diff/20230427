# Comparing `tmp/petprep_hmc-0.0.1.tar.gz` & `tmp/petprep_hmc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petprep_hmc-0.0.1.tar", last modified: Tue Apr 18 20:13:23 2023, max compression
+gzip compressed data, was "petprep_hmc-0.0.3.tar", last modified: Thu Apr 27 11:15:43 2023, max compression
```

## Comparing `petprep_hmc-0.0.1.tar` & `petprep_hmc-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 20:13:23.219249 petprep_hmc-0.0.1/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.1/LICENSE
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-04-18 20:13:23.219074 petprep_hmc-0.0.1/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     2381 2023-04-18 11:38:07.000000 petprep_hmc-0.0.1/README.md
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 20:13:23.218008 petprep_hmc-0.0.1/petprep_hmc/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.1/petprep_hmc/__init__.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 20:13:23.218876 petprep_hmc-0.0.1/petprep_hmc.egg-info/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-04-18 20:13:23.000000 petprep_hmc-0.0.1/petprep_hmc.egg-info/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      224 2023-04-18 20:13:23.000000 petprep_hmc-0.0.1/petprep_hmc.egg-info/SOURCES.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-04-18 20:13:23.000000 petprep_hmc-0.0.1/petprep_hmc.egg-info/dependency_links.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      403 2023-04-18 20:13:23.000000 petprep_hmc-0.0.1/petprep_hmc.egg-info/requires.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-04-18 20:13:23.000000 petprep_hmc-0.0.1/petprep_hmc.egg-info/top_level.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-04-18 20:13:23.219307 petprep_hmc-0.0.1/setup.cfg
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1554 2023-04-18 20:12:46.000000 petprep_hmc-0.0.1/setup.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-27 11:15:43.322815 petprep_hmc-0.0.3/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.3/LICENSE
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-04-27 11:15:43.322628 petprep_hmc-0.0.3/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     4023 2023-04-27 11:08:27.000000 petprep_hmc-0.0.3/README.md
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-27 11:15:43.321621 petprep_hmc-0.0.3/petprep_hmc/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.3/petprep_hmc/__init__.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-04-27 11:15:43.322405 petprep_hmc-0.0.3/petprep_hmc.egg-info/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      224 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/SOURCES.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/dependency_links.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      403 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/requires.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-04-27 11:15:43.000000 petprep_hmc-0.0.3/petprep_hmc.egg-info/top_level.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-04-27 11:15:43.322865 petprep_hmc-0.0.3/setup.cfg
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1554 2023-04-27 11:15:38.000000 petprep_hmc-0.0.3/setup.py
```

### Comparing `petprep_hmc-0.0.1/LICENSE` & `petprep_hmc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.1/PKG-INFO` & `petprep_hmc-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep_hmc
-Version: 0.0.1
+Version: 0.0.3
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.1/petprep_hmc.egg-info/PKG-INFO` & `petprep_hmc-0.0.3/petprep_hmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep-hmc
-Version: 0.0.1
+Version: 0.0.3
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.1/setup.py` & `petprep_hmc-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="petprep_hmc",
-    version="0.0.1",
+    version="0.0.3",
     description='PETPrep Head Motion Correction Workflow',
     author='Martin Norgaard',
     author_email='martin.noergaard@di.ku.dk',
     url='https://github.com/mnoergaard/petprep_hmc',
     packages=find_packages(),
     install_requires=[
         "click==8.1.3",
```

