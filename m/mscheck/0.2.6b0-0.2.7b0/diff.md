# Comparing `tmp/mscheck-0.2.6b0.tar.gz` & `tmp/mscheck-0.2.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscheck-0.2.6b0.tar", last modified: Thu Apr 27 20:21:02 2023, max compression
+gzip compressed data, was "mscheck-0.2.7b0.tar", last modified: Thu Apr 27 20:50:10 2023, max compression
```

## Comparing `mscheck-0.2.6b0.tar` & `mscheck-0.2.7b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:21:02.199739 mscheck-0.2.6b0/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-27 20:21:02.199739 mscheck-0.2.6b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:21:02.199739 mscheck-0.2.6b0/mscheck/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/mscheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/mscheck/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/mscheck/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/mscheck/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/mscheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:21:02.199739 mscheck-0.2.6b0/mscheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-27 20:21:02.000000 mscheck-0.2.6b0/mscheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 20:21:02.000000 mscheck-0.2.6b0/mscheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 20:21:02.000000 mscheck-0.2.6b0/mscheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 20:21:02.000000 mscheck-0.2.6b0/mscheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 20:21:02.000000 mscheck-0.2.6b0/mscheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 20:21:02.203739 mscheck-0.2.6b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:21:02.199739 mscheck-0.2.6b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-27 20:21:01.000000 mscheck-0.2.6b0/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.741527 mscheck-0.2.7b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-27 20:50:10.741527 mscheck-0.2.7b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.737527 mscheck-0.2.7b0/mscheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/mscheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/mscheck/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/mscheck/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/mscheck/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/mscheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.741527 mscheck-0.2.7b0/mscheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-27 20:50:10.000000 mscheck-0.2.7b0/mscheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 20:50:10.000000 mscheck-0.2.7b0/mscheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 20:50:10.000000 mscheck-0.2.7b0/mscheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 20:50:10.000000 mscheck-0.2.7b0/mscheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 20:50:10.000000 mscheck-0.2.7b0/mscheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 20:50:10.741527 mscheck-0.2.7b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:10.741527 mscheck-0.2.7b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-27 20:50:09.000000 mscheck-0.2.7b0/tests/test_spectrum.py
```

### Comparing `mscheck-0.2.6b0/PKG-INFO` & `mscheck-0.2.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d73 6368  : 2.1.Name: msch
 00000020: 6563 6b0a 5665 7273 696f 6e3a 2030 2e32  eck.Version: 0.2
-00000030: 2e36 6230 0a53 756d 6d61 7279 3a20 4175  .6b0.Summary: Au
+00000030: 2e37 6230 0a53 756d 6d61 7279 3a20 4175  .7b0.Summary: Au
 00000040: 746f 204d 5320 6d61 7373 2063 6865 636b  to MS mass check
 00000050: 6572 0a48 6f6d 652d 7061 6765 3a20 6874  er.Home-page: ht
 00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000070: 2f57 617a 746f 6d2f 6d73 6368 6563 6b0a  /Waztom/mscheck.
 00000080: 4175 7468 6f72 3a20 5761 7272 656e 2054  Author: Warren T
 00000090: 686f 6d70 736f 6e0a 4175 7468 6f72 2d65  hompson.Author-e
 000000a0: 6d61 696c 3a20 7761 7a74 6f6d 4067 6d61  mail: waztom@gma
```

### Comparing `mscheck-0.2.6b0/README.md` & `mscheck-0.2.7b0/README.md`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.6b0/mscheck/analyse.py` & `mscheck-0.2.7b0/mscheck/analyse.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.6b0/mscheck/report.py` & `mscheck-0.2.7b0/mscheck/report.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.6b0/mscheck/spectrum.py` & `mscheck-0.2.7b0/mscheck/spectrum.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.6b0/mscheck/utils.py` & `mscheck-0.2.7b0/mscheck/utils.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.6b0/mscheck.egg-info/PKG-INFO` & `mscheck-0.2.7b0/mscheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d73 6368  : 2.1.Name: msch
 00000020: 6563 6b0a 5665 7273 696f 6e3a 2030 2e32  eck.Version: 0.2
-00000030: 2e36 6230 0a53 756d 6d61 7279 3a20 4175  .6b0.Summary: Au
+00000030: 2e37 6230 0a53 756d 6d61 7279 3a20 4175  .7b0.Summary: Au
 00000040: 746f 204d 5320 6d61 7373 2063 6865 636b  to MS mass check
 00000050: 6572 0a48 6f6d 652d 7061 6765 3a20 6874  er.Home-page: ht
 00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000070: 2f57 617a 746f 6d2f 6d73 6368 6563 6b0a  /Waztom/mscheck.
 00000080: 4175 7468 6f72 3a20 5761 7272 656e 2054  Author: Warren T
 00000090: 686f 6d70 736f 6e0a 4175 7468 6f72 2d65  hompson.Author-e
 000000a0: 6d61 696c 3a20 7761 7a74 6f6d 4067 6d61  mail: waztom@gma
```

### Comparing `mscheck-0.2.6b0/setup.py` & `mscheck-0.2.7b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     long_description_content_type="text/markdown",
     license="MIT",
     install_requires=[
         "rdkit",
         "matplotlib",
         "scipy",
         "svgutils",
-        "pyopenms-nightly",
+        "pyopenms",
     ],
-    dependency_links=["https://pypi.cs.uni-tuebingen.de/simple/pyopenms-nightly/"],
+    dependency_links=["https://pypi.cs.uni-tuebingen.de/simple/pyopenms/"],
     packages=find_packages(),
     url="https://github.com/Waztom/mscheck",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

### Comparing `mscheck-0.2.6b0/tests/test_analyse.py` & `mscheck-0.2.7b0/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.6b0/tests/test_spectrum.py` & `mscheck-0.2.7b0/tests/test_spectrum.py`

 * *Files identical despite different names*

