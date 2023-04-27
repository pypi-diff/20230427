# Comparing `tmp/mask2bbox-0.0.1.tar.gz` & `tmp/mask2bbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.1.tar", last modified: Thu Apr 27 12:53:50 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.2.tar", last modified: Thu Apr 27 13:36:32 2023, max compression
```

## Comparing `mask2bbox-0.0.1.tar` & `mask2bbox-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.503103 mask2bbox-0.0.1/
--rw-r--r--   0 miguelibarra   (501) staff       (20)    35149 2023-04-27 12:24:53.000000 mask2bbox-0.0.1/LICENSE.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       56 2023-04-27 12:51:38.000000 mask2bbox-0.0.1/MANIFEST.in
--rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 12:53:50.502956 mask2bbox-0.0.1/PKG-INFO
--rw-r--r--   0 miguelibarra   (501) staff       (20)      420 2023-04-27 12:31:34.000000 mask2bbox-0.0.1/README.md
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.501842 mask2bbox-0.0.1/mask2bbox.egg-info/
--rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 miguelibarra   (501) staff       (20)      389 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)        1 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       19 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       14 2023-04-27 12:53:50.000000 mask2bbox-0.0.1/mask2bbox.egg-info/top_level.txt
--rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 12:53:50.503142 mask2bbox-0.0.1/setup.cfg
--rw-r--r--   0 miguelibarra   (501) staff       (20)      832 2023-04-27 12:49:03.000000 mask2bbox-0.0.1/setup.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.501965 mask2bbox-0.0.1/src/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.1/src/__init__.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.502318 mask2bbox-0.0.1/src/mask2bbox/
--rw-r--r--   0 miguelibarra   (501) staff       (20)     2019 2023-04-27 11:50:58.000000 mask2bbox-0.0.1/src/mask2bbox/BBoxes.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.1/src/mask2bbox/__init__.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)     1808 2023-04-27 12:36:32.000000 mask2bbox-0.0.1/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.502513 mask2bbox-0.0.1/tests/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:42:54.000000 mask2bbox-0.0.1/tests/__init__.py
-drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:53:50.502755 mask2bbox-0.0.1/tests/test_mask2bbox/
--rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:43:28.000000 mask2bbox-0.0.1/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 miguelibarra   (501) staff       (20)      120 2023-04-27 12:47:29.000000 mask2bbox-0.0.1/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.676257 mask2bbox-0.0.2/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)    35149 2023-04-27 12:24:53.000000 mask2bbox-0.0.2/LICENSE.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       56 2023-04-27 12:51:38.000000 mask2bbox-0.0.2/MANIFEST.in
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 13:36:32.676117 mask2bbox-0.0.2/PKG-INFO
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      420 2023-04-27 12:31:34.000000 mask2bbox-0.0.2/README.md
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 13:36:32.676296 mask2bbox-0.0.2/setup.cfg
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      818 2023-04-27 13:30:33.000000 mask2bbox-0.0.2/setup.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.674542 mask2bbox-0.0.2/src/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.2/src/__init__.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.674850 mask2bbox-0.0.2/src/mask2bbox/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)     2019 2023-04-27 11:50:58.000000 mask2bbox-0.0.2/src/mask2bbox/BBoxes.py
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-25 13:07:57.000000 mask2bbox-0.0.2/src/mask2bbox/__init__.py
+-rw-r--r--   0 miguelibarra   (501) staff       (20)     1808 2023-04-27 12:36:32.000000 mask2bbox-0.0.2/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.675587 mask2bbox-0.0.2/src/mask2bbox.egg-info/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      949 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      409 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        1 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       38 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 miguelibarra   (501) staff       (20)       19 2023-04-27 13:36:32.000000 mask2bbox-0.0.2/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.675730 mask2bbox-0.0.2/tests/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:42:54.000000 mask2bbox-0.0.2/tests/__init__.py
+drwxr-xr-x   0 miguelibarra   (501) staff       (20)        0 2023-04-27 13:36:32.675940 mask2bbox-0.0.2/tests/test_mask2bbox/
+-rw-r--r--   0 miguelibarra   (501) staff       (20)        0 2023-04-27 12:43:28.000000 mask2bbox-0.0.2/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 miguelibarra   (501) staff       (20)      127 2023-04-27 13:29:49.000000 mask2bbox-0.0.2/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.1/LICENSE.txt` & `mask2bbox-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.1/PKG-INFO` & `mask2bbox-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mask2bbox-0.0.1/mask2bbox.egg-info/PKG-INFO` & `mask2bbox-0.0.2/src/mask2bbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mask2bbox-0.0.1/setup.py` & `mask2bbox-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.1",
+    version="0.0.2",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
-    packages=["src/mask2bbox"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     long_description=long_description,
     long_description_content_type="text/markdown",
+    install_requires = [
+        "numpy",
+        "scikit-image"
+    ],
     extras_require={
         "dev": ["pytest>=3.7"],
     },
 )
 
-install_requires = [
-    "numpy",
-    "scikit-image"
-]
```

### Comparing `mask2bbox-0.0.1/src/mask2bbox/BBoxes.py` & `mask2bbox-0.0.2/src/mask2bbox/BBoxes.py`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.1/src/mask2bbox/mask2bbox.py` & `mask2bbox-0.0.2/src/mask2bbox/mask2bbox.py`

 * *Files identical despite different names*

