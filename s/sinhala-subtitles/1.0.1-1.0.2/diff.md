# Comparing `tmp/sinhala_subtitles-1.0.1.tar.gz` & `tmp/sinhala_subtitles-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinhala_subtitles-1.0.1.tar", last modified: Thu Apr 27 03:30:29 2023, max compression
+gzip compressed data, was "sinhala_subtitles-1.0.2.tar", last modified: Thu Apr 27 03:42:59 2023, max compression
```

## Comparing `sinhala_subtitles-1.0.1.tar` & `sinhala_subtitles-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 03:30:29.980455 sinhala_subtitles-1.0.1/
--rw-rw-rw-   0        0        0     2913 2023-04-27 03:30:29.979453 sinhala_subtitles-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2023-04-27 03:07:14.000000 sinhala_subtitles-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 03:30:29.981456 sinhala_subtitles-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-04-27 03:29:07.000000 sinhala_subtitles-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:30:29.883454 sinhala_subtitles-1.0.1/sinhala_subtitles/
--rw-rw-rw-   0        0        0     2599 2023-04-27 02:32:34.000000 sinhala_subtitles-1.0.1/sinhala_subtitles/__init__.py
--rw-rw-rw-   0        0        0     3976 2023-04-27 02:28:05.000000 sinhala_subtitles-1.0.1/sinhala_subtitles/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:30:29.975458 sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/
--rw-rw-rw-   0        0        0     2913 2023-04-27 03:30:29.000000 sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-27 03:30:29.000000 sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 03:30:29.000000 sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-27 03:30:29.000000 sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-27 03:30:29.000000 sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 03:42:59.382456 sinhala_subtitles-1.0.2/
+-rw-rw-rw-   0        0        0     2888 2023-04-27 03:42:59.380455 sinhala_subtitles-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2358 2023-04-27 03:30:47.000000 sinhala_subtitles-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 03:42:59.382456 sinhala_subtitles-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      775 2023-04-27 03:42:26.000000 sinhala_subtitles-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:42:59.357458 sinhala_subtitles-1.0.2/sinhala_subtitles/
+-rw-rw-rw-   0        0        0     2599 2023-04-27 02:32:34.000000 sinhala_subtitles-1.0.2/sinhala_subtitles/__init__.py
+-rw-rw-rw-   0        0        0     3976 2023-04-27 02:28:05.000000 sinhala_subtitles-1.0.2/sinhala_subtitles/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-27 03:42:59.377455 sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     2888 2023-04-27 03:42:59.000000 sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-27 03:42:59.000000 sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 03:42:59.000000 sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-27 03:42:59.000000 sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-27 03:42:59.000000 sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/top_level.txt
```

### Comparing `sinhala_subtitles-1.0.1/PKG-INFO` & `sinhala_subtitles-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: sinhala_subtitles
-Version: 1.0.1
+Version: 1.0.2
 Summary: This Python library is designed to make downloading Sinhala subtitles for TV series and movies easy. To use it, simply install the library using pip and import it into your Python script.
 Home-page: 
 Author: Gavindu Tharaka
 Author-email: gavi.tharaka@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 
 # Sinhala Subtitles Downloader
 
 This Python library makes it easy to download Sinhala subtitles for TV series and movies. It currently supports two websites, Baiscope and Cineru.
 
 ## Installation
 
 You can install the library using pip:
 ```cmd
-pip install sinhala-subtitles
+pip install sinhala_subtitles
 ```
 
 
 ## Usage
 
 To use the library, simply import it and call one of the following functions:
```

### Comparing `sinhala_subtitles-1.0.1/README.md` & `sinhala_subtitles-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This Python library makes it easy to download Sinhala subtitles for TV series and movies. It currently supports two websites, Baiscope and Cineru.
 
 ## Installation
 
 You can install the library using pip:
 ```cmd
-pip install sinhala-subtitles
+pip install sinhala_subtitles
 ```
 
 
 ## Usage
 
 To use the library, simply import it and call one of the following functions:
```

### Comparing `sinhala_subtitles-1.0.1/setup.py` & `sinhala_subtitles-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sinhala_subtitles",
-    version="1.0.1",
+    version="1.0.2",
     author="Gavindu Tharaka",
     author_email="gavi.tharaka@gmail.com",
     description="This Python library is designed to make downloading Sinhala subtitles for TV series and movies easy. To use it, simply install the library using pip and import it into your Python script.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=["sinhala_subtitles"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.10',
     install_requires=['bs4'],
 )
```

### Comparing `sinhala_subtitles-1.0.1/sinhala_subtitles/__init__.py` & `sinhala_subtitles-1.0.2/sinhala_subtitles/__init__.py`

 * *Files identical despite different names*

### Comparing `sinhala_subtitles-1.0.1/sinhala_subtitles/functions.py` & `sinhala_subtitles-1.0.2/sinhala_subtitles/functions.py`

 * *Files identical despite different names*

### Comparing `sinhala_subtitles-1.0.1/sinhala_subtitles.egg-info/PKG-INFO` & `sinhala_subtitles-1.0.2/sinhala_subtitles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: sinhala-subtitles
-Version: 1.0.1
+Version: 1.0.2
 Summary: This Python library is designed to make downloading Sinhala subtitles for TV series and movies easy. To use it, simply install the library using pip and import it into your Python script.
 Home-page: 
 Author: Gavindu Tharaka
 Author-email: gavi.tharaka@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 
 # Sinhala Subtitles Downloader
 
 This Python library makes it easy to download Sinhala subtitles for TV series and movies. It currently supports two websites, Baiscope and Cineru.
 
 ## Installation
 
 You can install the library using pip:
 ```cmd
-pip install sinhala-subtitles
+pip install sinhala_subtitles
 ```
 
 
 ## Usage
 
 To use the library, simply import it and call one of the following functions:
```

