# Comparing `tmp/PaymeAPI-1.0.2.tar.gz` & `tmp/PaymeAPI-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaymeAPI-1.0.2.tar", last modified: Thu Apr 27 18:50:07 2023, max compression
+gzip compressed data, was "PaymeAPI-1.0.3.tar", last modified: Thu Apr 27 19:10:31 2023, max compression
```

## Comparing `PaymeAPI-1.0.2.tar` & `PaymeAPI-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 18:50:07.408962 PaymeAPI-1.0.2/
--rw-rw-rw-   0        0        0     1082 2023-04-27 16:52:25.000000 PaymeAPI-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      351 2023-04-27 18:50:07.407962 PaymeAPI-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 18:50:07.406963 PaymeAPI-1.0.2/PaymeAPI.egg-info/
--rw-rw-rw-   0        0        0      351 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2793 2023-04-27 17:43:05.000000 PaymeAPI-1.0.2/PaymeAPI.py
--rw-rw-rw-   0        0        0      699 2023-04-27 18:48:41.000000 PaymeAPI-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 18:50:07.408962 PaymeAPI-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-04-27 18:49:51.000000 PaymeAPI-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:10:31.657874 PaymeAPI-1.0.3/
+-rw-rw-rw-   0        0        0      373 2023-04-27 19:10:31.654877 PaymeAPI-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 19:10:31.618875 PaymeAPI-1.0.3/PaymeAPI/
+-rw-rw-rw-   0        0        0       20 2023-04-27 19:06:17.000000 PaymeAPI-1.0.3/PaymeAPI/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-04-27 19:04:13.000000 PaymeAPI-1.0.3/PaymeAPI/payme.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:10:31.647876 PaymeAPI-1.0.3/PaymeAPI.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-04-27 19:10:31.000000 PaymeAPI-1.0.3/PaymeAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-04-27 19:10:31.000000 PaymeAPI-1.0.3/PaymeAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 19:10:31.000000 PaymeAPI-1.0.3/PaymeAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 19:10:31.000000 PaymeAPI-1.0.3/PaymeAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      699 2023-04-27 18:48:41.000000 PaymeAPI-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 19:10:31.658875 PaymeAPI-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-04-27 19:09:40.000000 PaymeAPI-1.0.3/setup.py
```

### Comparing `PaymeAPI-1.0.2/PaymeAPI.py` & `PaymeAPI-1.0.3/PaymeAPI/payme.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
                                                                                      
 # :copyright: (c) 2022-2023 by Amore.
 # :license: MIT, see LICENSE for more details.
 
                       
 import requests
 
+__all__ = ["Payme"]
+
 class Payme:
     headers = {'device': '6Fk1rB', 'user-agent': 'Mozilla/57.36'}
 
     def __init__(self, mycard):
         self.mycard = mycard
 
     def create(self, summ, desc):
```

### Comparing `PaymeAPI-1.0.2/README.md` & `PaymeAPI-1.0.3/README.md`

 * *Files identical despite different names*

