# Comparing `tmp/hestia-earth-utils-0.9.1.tar.gz` & `tmp/hestia-earth-utils-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hestia-earth-utils-0.9.1.tar", last modified: Tue Aug 10 08:41:48 2021, max compression
+gzip compressed data, was "dist/hestia-earth-utils-0.9.2.tar", last modified: Thu Aug 12 08:17:47 2021, max compression
```

## Comparing `hestia-earth-utils-0.9.1.tar` & `hestia-earth-utils-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-10 08:41:48.000000 hestia-earth-utils-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     1563 2021-08-10 08:41:48.000000 hestia-earth-utils-0.9.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-10 08:41:48.000000 hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1563 2021-08-10 08:41:47.000000 hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2021-08-10 08:41:47.000000 hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-10 08:41:47.000000 hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-08-10 08:41:47.000000 hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       66 2021-08-10 08:41:47.000000 hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1005 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-10 08:41:48.000000 hestia-earth-utils-0.9.1/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-10 08:41:48.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/
--rw-rw-rw-   0 root         (0) root         (0)      641 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/request.py
--rw-rw-rw-   0 root         (0) root         (0)     3655 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/date.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/_s3_client.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/api.py
--rw-rw-rw-   0 root         (0) root         (0)     3776 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/model.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/lookup.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/hestia_earth/utils/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2021-08-10 08:41:33.000000 hestia-earth-utils-0.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-10 08:41:48.000000 hestia-earth-utils-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1563 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1563 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      526 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      641 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/_s3_client.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3776 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/hestia_earth/utils/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2021-08-12 08:17:33.000000 hestia-earth-utils-0.9.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-12 08:17:47.000000 hestia-earth-utils-0.9.2/setup.cfg
```

### Comparing `hestia-earth-utils-0.9.1/PKG-INFO` & `hestia-earth-utils-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-utils
-Version: 0.9.1
+Version: 0.9.2
 Summary: Hestia's utils library
 Home-page: https://gitlab.com/hestia-earth/hestia-utils
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL-3.0-or-later
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/PKG-INFO` & `hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-utils
-Version: 0.9.1
+Version: 0.9.2
 Summary: Hestia's utils library
 Home-page: https://gitlab.com/hestia-earth/hestia-utils
 Author: Hestia Team
 Author-email: guillaumeroyer.mail@gmail.com
 License: GPL-3.0-or-later
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-utils-0.9.1/hestia_earth_utils.egg-info/SOURCES.txt` & `hestia-earth-utils-0.9.2/hestia_earth_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/setup.py` & `hestia-earth-utils-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/request.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/request.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/tools.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/date.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/date.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/_s3_client.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/_s3_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/api.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/api.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/model.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/model.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/hestia_earth/utils/lookup.py` & `hestia-earth-utils-0.9.2/hestia_earth/utils/lookup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-utils-0.9.1/README.md` & `hestia-earth-utils-0.9.2/README.md`

 * *Files identical despite different names*

