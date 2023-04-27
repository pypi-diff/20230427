# Comparing `tmp/salamenc-1.2.tar.gz` & `tmp/salamenc-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salamenc-1.2.tar", last modified: Mon Apr 24 23:47:46 2023, max compression
+gzip compressed data, was "salamenc-1.3.tar", last modified: Thu Apr 27 14:27:47 2023, max compression
```

## Comparing `salamenc-1.2.tar` & `salamenc-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-24 23:47:46.479004 salamenc-1.2/
--rw-rw----   0 root         (0) everybody  (9997)     1061 2022-07-07 15:21:40.000000 salamenc-1.2/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     2055 2023-04-24 23:47:46.439004 salamenc-1.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1448 2023-04-24 23:45:55.000000 salamenc-1.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-24 23:47:46.319004 salamenc-1.2/salamenc/
--rw-rw----   0 root         (0) everybody  (9997)       23 2023-04-24 23:39:13.000000 salamenc-1.2/salamenc/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    23109 2023-04-24 23:27:59.000000 salamenc-1.2/salamenc/salamenc.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-24 23:47:46.419004 salamenc-1.2/salamenc.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2055 2023-04-24 23:47:45.000000 salamenc-1.2/salamenc.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      196 2023-04-24 23:47:46.000000 salamenc-1.2/salamenc.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-24 23:47:45.000000 salamenc-1.2/salamenc.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-04-24 23:47:45.000000 salamenc-1.2/salamenc.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-24 23:47:46.479004 salamenc-1.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1162 2023-04-24 23:46:11.000000 salamenc-1.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-27 14:27:47.457928 salamenc-1.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1061 2022-07-07 15:21:40.000000 salamenc-1.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     2055 2023-04-27 14:27:47.427928 salamenc-1.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1448 2023-04-24 23:45:55.000000 salamenc-1.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-27 14:27:47.307928 salamenc-1.3/salamenc/
+-rw-rw----   0 root         (0) everybody  (9997)       23 2023-04-27 14:23:11.000000 salamenc-1.3/salamenc/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2167 2023-04-27 14:25:36.000000 salamenc-1.3/salamenc/salamenc.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-27 14:27:47.407928 salamenc-1.3/salamenc.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2055 2023-04-27 14:27:46.000000 salamenc-1.3/salamenc.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      196 2023-04-27 14:27:47.000000 salamenc-1.3/salamenc.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-27 14:27:46.000000 salamenc-1.3/salamenc.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-04-27 14:27:46.000000 salamenc-1.3/salamenc.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-27 14:27:47.457928 salamenc-1.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1162 2023-04-27 14:22:46.000000 salamenc-1.3/setup.py
```

### Comparing `salamenc-1.2/LICENSE` & `salamenc-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `salamenc-1.2/PKG-INFO` & `salamenc-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salamenc
-Version: 1.2
+Version: 1.3
 Summary: For developers Encrypt tools
 Home-page: https://t.me/T5B55
 Author: salammzere3
 Author-email: salamhunter@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: salamenc
 Classifier: Development Status :: 1 - Planning
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salamenc Version: 1.2 Summary: For developers
+Metadata-Version: 2.1 Name: salamenc Version: 1.3 Summary: For developers
 Encrypt tools Home-page: https://t.me/T5B55 Author: salammzere3 Author-email:
 salamhunter@gmail.com Project-URL: Bug Tracker, https://github.com/pypa/
 sampleproject/issues Keywords: salamenc Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `salamenc-1.2/README.md` & `salamenc-1.3/README.md`

 * *Files identical despite different names*

### Comparing `salamenc-1.2/salamenc.egg-info/PKG-INFO` & `salamenc-1.3/salamenc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salamenc
-Version: 1.2
+Version: 1.3
 Summary: For developers Encrypt tools
 Home-page: https://t.me/T5B55
 Author: salammzere3
 Author-email: salamhunter@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: salamenc
 Classifier: Development Status :: 1 - Planning
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salamenc Version: 1.2 Summary: For developers
+Metadata-Version: 2.1 Name: salamenc Version: 1.3 Summary: For developers
 Encrypt tools Home-page: https://t.me/T5B55 Author: salammzere3 Author-email:
 salamhunter@gmail.com Project-URL: Bug Tracker, https://github.com/pypa/
 sampleproject/issues Keywords: salamenc Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `salamenc-1.2/setup.py` & `salamenc-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = "\n" + fh.read()
 
 
 setup(
 
     name="salamenc",
     
-    version="1.2",
+    version="1.3",
     
     author="salammzere3",
     
     author_email="salamhunter@gmail.com",
     
     description = ("For developers Encrypt tools"),
```

