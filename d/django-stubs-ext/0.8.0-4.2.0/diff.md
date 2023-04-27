# Comparing `tmp/django-stubs-ext-0.8.0.tar.gz` & `tmp/django-stubs-ext-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-ext-0.8.0.tar", last modified: Thu Mar 16 14:11:48 2023, max compression
+gzip compressed data, was "django-stubs-ext-4.2.0.tar", last modified: Thu Apr 27 12:47:35 2023, max compression
```

## Comparing `django-stubs-ext-0.8.0.tar` & `django-stubs-ext-4.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-03-16 14:11:48.351247 django-stubs-ext-0.8.0/
--rw-r--r--   0 marti     (1000) marti      (121)     3619 2023-03-16 14:11:48.351247 django-stubs-ext-0.8.0/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-03-16 14:11:48.351247 django-stubs-ext-0.8.0/django_stubs_ext/
--rw-r--r--   0 marti     (1000) marti      (121)      535 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/django_stubs_ext/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      620 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/django_stubs_ext/aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)      693 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/django_stubs_ext/annotations.py
--rw-r--r--   0 marti     (1000) marti      (121)     3660 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/django_stubs_ext/patch.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/django_stubs_ext/py.typed
--rw-r--r--   0 marti     (1000) marti      (121)      266 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/django_stubs_ext/types.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-03-16 14:11:48.351247 django-stubs-ext-0.8.0/django_stubs_ext.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     3619 2023-03-16 14:11:48.000000 django-stubs-ext-0.8.0/django_stubs_ext.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)      460 2023-03-16 14:11:48.000000 django-stubs-ext-0.8.0/django_stubs_ext.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-03-16 14:11:48.000000 django-stubs-ext-0.8.0/django_stubs_ext.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)       25 2023-03-16 14:11:48.000000 django-stubs-ext-0.8.0/django_stubs_ext.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       17 2023-03-16 14:11:48.000000 django-stubs-ext-0.8.0/django_stubs_ext.egg-info/top_level.txt
--rw-r--r--   0 marti     (1000) marti      (121)       80 2023-03-16 14:11:48.351247 django-stubs-ext-0.8.0/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 17:23:10.000000 django-stubs-ext-0.8.0/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-03-16 14:11:48.351247 django-stubs-ext-0.8.0/tests/
--rw-r--r--   0 marti     (1000) marti      (121)      169 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/tests/test_aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)     3957 2023-03-15 16:53:32.000000 django-stubs-ext-0.8.0/tests/test_monkeypatching.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/
+-rw-r--r--   0 marti     (1000) marti      (121)     3658 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/django_stubs_ext/
+-rw-r--r--   0 marti     (1000) marti      (121)      535 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)      620 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/aliases.py
+-rw-r--r--   0 marti     (1000) marti      (121)      693 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/annotations.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3660 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/patch.py
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/py.typed
+-rw-r--r--   0 marti     (1000) marti      (121)      266 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/types.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)     3658 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)      460 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       25 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       17 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/top_level.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       80 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     1808 2023-04-27 12:45:58.000000 django-stubs-ext-4.2.0/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/tests/
+-rw-r--r--   0 marti     (1000) marti      (121)      169 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/tests/test_aliases.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3957 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/tests/test_monkeypatching.py
```

### Comparing `django-stubs-ext-0.8.0/PKG-INFO` & `django-stubs-ext-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 0.8.0
+Version: 4.2.0
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -20,14 +20,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: ../LICENSE.txt
 
 # Extensions and monkey-patching for django-stubs
 
 [![Build Status](https://travis-ci.com/typeddjango/django-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/django-stubs)
```

### Comparing `django-stubs-ext-0.8.0/README.md` & `django-stubs-ext-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-0.8.0/django_stubs_ext/__init__.py` & `django-stubs-ext-4.2.0/django_stubs_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-0.8.0/django_stubs_ext/aliases.py` & `django-stubs-ext-4.2.0/django_stubs_ext/aliases.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-0.8.0/django_stubs_ext/annotations.py` & `django-stubs-ext-4.2.0/django_stubs_ext/annotations.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-0.8.0/django_stubs_ext/patch.py` & `django-stubs-ext-4.2.0/django_stubs_ext/patch.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-0.8.0/django_stubs_ext.egg-info/PKG-INFO` & `django-stubs-ext-4.2.0/django_stubs_ext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 0.8.0
+Version: 4.2.0
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -20,14 +20,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: ../LICENSE.txt
 
 # Extensions and monkey-patching for django-stubs
 
 [![Build Status](https://travis-ci.com/typeddjango/django-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/django-stubs)
```

### Comparing `django-stubs-ext-0.8.0/setup.py` & `django-stubs-ext-4.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,19 @@
     readme = f.read()
 
 dependencies = [
     "django",
     "typing-extensions",
 ]
 
+# NB! For clarity, keep version major.minor.patch in sync with django-stubs.
+# It's fine to skip django-stubs-ext releases, but when doing a release, update this to newest django-stubs version.
 setup(
     name="django-stubs-ext",
-    version="0.8.0",
+    version="4.2.0",
     description="Monkey-patching and extensions for django-stubs",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/typeddjango/django-stubs",
     author="Simula Proxy",
     author_email="3nki.nam.shub@gmail.com",
@@ -39,12 +41,13 @@
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
     ],
     project_urls={
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
 )
```

### Comparing `django-stubs-ext-0.8.0/tests/test_monkeypatching.py` & `django-stubs-ext-4.2.0/tests/test_monkeypatching.py`

 * *Files identical despite different names*

