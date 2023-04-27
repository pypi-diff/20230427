# Comparing `tmp/locate_pixelcolor_cythonmulti-0.11.tar.gz` & `tmp/locate_pixelcolor_cythonmulti-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_cythonmulti-0.11.tar", last modified: Thu Apr 27 17:30:48 2023, max compression
+gzip compressed data, was "locate_pixelcolor_cythonmulti-0.12.tar", last modified: Thu Apr 27 17:32:04 2023, max compression
```

## Comparing `locate_pixelcolor_cythonmulti-0.11.tar` & `locate_pixelcolor_cythonmulti-0.12.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:30:48.648089 locate_pixelcolor_cythonmulti-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-27 17:30:41.000000 locate_pixelcolor_cythonmulti-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      423 2023-04-27 17:30:37.000000 locate_pixelcolor_cythonmulti-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0    10368 2023-04-27 17:30:48.648089 locate_pixelcolor_cythonmulti-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     9635 2023-04-26 03:22:56.000000 locate_pixelcolor_cythonmulti-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 17:30:48.643103 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/LICENSE
--rw-rw-rw-   0        0        0     3521 2023-04-27 17:25:35.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/README.md
--rw-rw-rw-   0        0        0     1539 2023-04-27 17:07:33.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/__init__.py
--rw-rw-rw-   0        0        0   129024 2023-04-27 16:57:08.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/colorsearchcythonmulti.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     1048 2023-04-27 16:56:34.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/colorsearchcythonmulti.pyx
--rw-rw-rw-   0        0        0      508 2023-04-27 16:57:30.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/colorsearchcythonmultisetup.py
--rw-rw-rw-   0        0        0       25 2023-04-27 17:30:47.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/requirements.txt
--rw-rw-rw-   0        0        0    49970 2023-04-27 17:30:47.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-27 17:30:48.647092 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/
--rw-rw-rw-   0        0        0    10368 2023-04-27 17:30:48.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-04-27 17:30:48.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:30:48.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-27 17:30:48.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-27 17:30:48.000000 locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-27 17:30:48.649087 locate_pixelcolor_cythonmulti-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-04-27 17:30:47.000000 locate_pixelcolor_cythonmulti-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:32:04.289455 locate_pixelcolor_cythonmulti-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-27 17:31:53.000000 locate_pixelcolor_cythonmulti-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      423 2023-04-27 17:31:52.000000 locate_pixelcolor_cythonmulti-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     4246 2023-04-27 17:32:04.289455 locate_pixelcolor_cythonmulti-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3521 2023-04-27 17:25:35.000000 locate_pixelcolor_cythonmulti-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 17:32:04.284468 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/LICENSE
+-rw-rw-rw-   0        0        0     3521 2023-04-27 17:25:35.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/README.md
+-rw-rw-rw-   0        0        0     1539 2023-04-27 17:07:33.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/__init__.py
+-rw-rw-rw-   0        0        0   129024 2023-04-27 16:57:08.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/colorsearchcythonmulti.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0     1048 2023-04-27 16:56:34.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/colorsearchcythonmulti.pyx
+-rw-rw-rw-   0        0        0      508 2023-04-27 16:57:30.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/colorsearchcythonmultisetup.py
+-rw-rw-rw-   0        0        0       25 2023-04-27 17:32:03.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/requirements.txt
+-rw-rw-rw-   0        0        0    49970 2023-04-27 17:32:03.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-27 17:32:04.288466 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/
+-rw-rw-rw-   0        0        0     4246 2023-04-27 17:32:04.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-04-27 17:32:04.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 17:32:04.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-27 17:32:04.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-27 17:32:04.000000 locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-27 17:32:04.290452 locate_pixelcolor_cythonmulti-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-04-27 17:32:03.000000 locate_pixelcolor_cythonmulti-0.12/setup.py
```

### Comparing `locate_pixelcolor_cythonmulti-0.11/LICENSE.rst` & `locate_pixelcolor_cythonmulti-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/LICENSE` & `locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/LICENSE`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/README.md` & `locate_pixelcolor_cythonmulti-0.12/README.md`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/__init__.py` & `locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/__init__.py`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/colorsearchcythonmulti.pyx` & `locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/colorsearchcythonmulti.pyx`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti/thirdparty.json` & `locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti/thirdparty.json`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/locate_pixelcolor_cythonmulti.egg-info/SOURCES.txt` & `locate_pixelcolor_cythonmulti-0.12/locate_pixelcolor_cythonmulti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cythonmulti-0.11/setup.py` & `locate_pixelcolor_cythonmulti-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Compiled Cython Code (parallel) - Detects colors in images 5-10 x faster than Numpy'''
 
 # Setting up
 setup(
     name="locate_pixelcolor_cythonmulti",
     version=VERSION,
     license='MIT',
```

