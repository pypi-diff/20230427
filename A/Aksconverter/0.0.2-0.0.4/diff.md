# Comparing `tmp/Aksconverter-0.0.2.tar.gz` & `tmp/Aksconverter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aksconverter-0.0.2.tar", last modified: Thu Apr 27 15:59:30 2023, max compression
+gzip compressed data, was "Aksconverter-0.0.4.tar", last modified: Thu Apr 27 16:07:46 2023, max compression
```

## Comparing `Aksconverter-0.0.2.tar` & `Aksconverter-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-27 15:59:30.577884 Aksconverter-0.0.2/
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-27 15:59:30.577305 Aksconverter-0.0.2/Aksconverter.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)      686 2023-04-27 15:59:30.000000 Aksconverter-0.0.2/Aksconverter.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      296 2023-04-27 15:59:30.000000 Aksconverter-0.0.2/Aksconverter.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-04-27 15:59:30.000000 Aksconverter-0.0.2/Aksconverter.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       28 2023-04-27 15:59:30.000000 Aksconverter-0.0.2/Aksconverter.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       77 2023-04-26 07:11:04.000000 Aksconverter-0.0.2/CHANGELOG.txt
--rw-r--r--   0 akshay     (501) staff       (20)     1101 2023-04-27 15:15:18.000000 Aksconverter-0.0.2/LICENCE.txt
--rw-r--r--   0 akshay     (501) staff       (20)       25 2023-04-26 06:35:28.000000 Aksconverter-0.0.2/MANIFEST.in
--rw-r--r--   0 akshay     (501) staff       (20)      686 2023-04-27 15:59:30.577779 Aksconverter-0.0.2/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      132 2023-04-27 15:17:29.000000 Aksconverter-0.0.2/README.txt
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-27 15:59:30.577522 Aksconverter-0.0.2/aksconverter_properties_pkg/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2023-04-26 07:32:40.000000 Aksconverter-0.0.2/aksconverter_properties_pkg/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)      357 2023-04-27 15:58:09.000000 Aksconverter-0.0.2/aksconverter_properties_pkg/aksconverter_properties.py
--rw-r--r--   0 akshay     (501) staff       (20)       38 2023-04-27 15:59:30.577917 Aksconverter-0.0.2/setup.cfg
--rw-r--r--   0 akshay     (501) staff       (20)      663 2023-04-27 15:52:05.000000 Aksconverter-0.0.2/setup.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-27 16:07:46.395717 Aksconverter-0.0.4/
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-27 16:07:46.395104 Aksconverter-0.0.4/Aksconverter.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)      686 2023-04-27 16:07:46.000000 Aksconverter-0.0.4/Aksconverter.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      296 2023-04-27 16:07:46.000000 Aksconverter-0.0.4/Aksconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-04-27 16:07:46.000000 Aksconverter-0.0.4/Aksconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       28 2023-04-27 16:07:46.000000 Aksconverter-0.0.4/Aksconverter.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       77 2023-04-26 07:11:04.000000 Aksconverter-0.0.4/CHANGELOG.txt
+-rw-r--r--   0 akshay     (501) staff       (20)     1101 2023-04-27 15:15:18.000000 Aksconverter-0.0.4/LICENCE.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       25 2023-04-26 06:35:28.000000 Aksconverter-0.0.4/MANIFEST.in
+-rw-r--r--   0 akshay     (501) staff       (20)      686 2023-04-27 16:07:46.395599 Aksconverter-0.0.4/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      132 2023-04-27 15:17:29.000000 Aksconverter-0.0.4/README.txt
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-04-27 16:07:46.395326 Aksconverter-0.0.4/aksconverter_properties_pkg/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2023-04-26 07:32:40.000000 Aksconverter-0.0.4/aksconverter_properties_pkg/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)      390 2023-04-27 16:05:35.000000 Aksconverter-0.0.4/aksconverter_properties_pkg/aksconverter_properties.py
+-rw-r--r--   0 akshay     (501) staff       (20)       38 2023-04-27 16:07:46.395755 Aksconverter-0.0.4/setup.cfg
+-rw-r--r--   0 akshay     (501) staff       (20)      663 2023-04-27 16:07:41.000000 Aksconverter-0.0.4/setup.py
```

### Comparing `Aksconverter-0.0.2/Aksconverter.egg-info/PKG-INFO` & `Aksconverter-0.0.4/Aksconverter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aksconverter
-Version: 0.0.2
+Version: 0.0.4
 Summary: A very currency calculator
 Home-page: 
 Author: Akshat Joshi
 Author-email: x22137696@student.ncirl.ie
 License: MIT
 Keywords: Currency Calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Aksconverter-0.0.2/LICENCE.txt` & `Aksconverter-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `Aksconverter-0.0.2/PKG-INFO` & `Aksconverter-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aksconverter
-Version: 0.0.2
+Version: 0.0.4
 Summary: A very currency calculator
 Home-page: 
 Author: Akshat Joshi
 Author-email: x22137696@student.ncirl.ie
 License: MIT
 Keywords: Currency Calculator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Aksconverter-0.0.2/setup.py` & `Aksconverter-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.8'
 ]
  
 setup(
   name='Aksconverter',
-  version='0.0.2',
+  version='0.0.4',
   description='A very currency calculator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Akshat Joshi',
   author_email='x22137696@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
```

