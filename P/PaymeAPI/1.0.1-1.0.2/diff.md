# Comparing `tmp/PaymeAPI-1.0.1.tar.gz` & `tmp/PaymeAPI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaymeAPI-1.0.1.tar", last modified: Thu Apr 27 17:43:10 2023, max compression
+gzip compressed data, was "PaymeAPI-1.0.2.tar", last modified: Thu Apr 27 18:50:07 2023, max compression
```

## Comparing `PaymeAPI-1.0.1.tar` & `PaymeAPI-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:43:10.040863 PaymeAPI-1.0.1/
--rw-rw-rw-   0        0        0     1082 2023-04-27 16:52:25.000000 PaymeAPI-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      351 2023-04-27 17:43:10.038863 PaymeAPI-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 17:43:10.037863 PaymeAPI-1.0.1/PaymeAPI.egg-info/
--rw-rw-rw-   0        0        0      351 2023-04-27 17:43:09.000000 PaymeAPI-1.0.1/PaymeAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-04-27 17:43:09.000000 PaymeAPI-1.0.1/PaymeAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:43:09.000000 PaymeAPI-1.0.1/PaymeAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 17:43:09.000000 PaymeAPI-1.0.1/PaymeAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      693 2023-04-27 17:13:18.000000 PaymeAPI-1.0.1/README.md
--rw-rw-rw-   0        0        0     2793 2023-04-27 17:43:05.000000 PaymeAPI-1.0.1/payme.py
--rw-rw-rw-   0        0        0       42 2023-04-27 17:43:10.040863 PaymeAPI-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      435 2023-04-27 17:39:37.000000 PaymeAPI-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:50:07.408962 PaymeAPI-1.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-04-27 16:52:25.000000 PaymeAPI-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      351 2023-04-27 18:50:07.407962 PaymeAPI-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 18:50:07.406963 PaymeAPI-1.0.2/PaymeAPI.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 18:50:07.000000 PaymeAPI-1.0.2/PaymeAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2793 2023-04-27 17:43:05.000000 PaymeAPI-1.0.2/PaymeAPI.py
+-rw-rw-rw-   0        0        0      699 2023-04-27 18:48:41.000000 PaymeAPI-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:50:07.408962 PaymeAPI-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-04-27 18:49:51.000000 PaymeAPI-1.0.2/setup.py
```

### Comparing `PaymeAPI-1.0.1/LICENSE` & `PaymeAPI-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PaymeAPI-1.0.1/README.md` & `PaymeAPI-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 <pre lang="bash">
 pip install PaymeAPI
 </pre>
 
 
 <h1>Usage</h1>
 
-To use PaymeAPI, first import the <code>PaymeAPI</code> class from the <code>payme</code> package:
+To use PaymeAPI, first import the <code>PaymeAPI</code> class from the <code>PaymeAPI</code> package:
 
 <pre lang="python">
 # Import lib
-from payme import Payme
+from PaymeAPI import Payme
 # Create a client instance with your card ID
 client = Payme(mycard=' ')
 
 # Call the create method to create a payment
 response = client.create(summ=10000, desc='Test Payment')
 
 check_id = response['result']['id']
```

### Comparing `PaymeAPI-1.0.1/payme.py` & `PaymeAPI-1.0.2/PaymeAPI.py`

 * *Files identical despite different names*

