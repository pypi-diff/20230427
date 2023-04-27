# Comparing `tmp/pyTibber-0.9.8.tar.gz` & `tmp/pyTibber-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyTibber-0.9.8.tar", last modified: Fri Mar 15 13:51:14 2019, max compression
+gzip compressed data, was "dist/pyTibber-0.9.9.tar", last modified: Thu Mar 21 09:01:22 2019, max compression
```

## Comparing `pyTibber-0.9.8.tar` & `pyTibber-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-15 13:51:14.000000 pyTibber-0.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1630 2019-03-15 13:50:28.000000 pyTibber-0.9.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      975 2019-03-15 13:50:28.000000 pyTibber-0.9.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-15 13:51:14.000000 pyTibber-0.9.8/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-15 13:51:14.000000 pyTibber-0.9.8/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5959 2019-03-15 13:50:28.000000 pyTibber-0.9.8/test/test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2019-03-15 13:50:28.000000 pyTibber-0.9.8/License.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-15 13:50:28.000000 pyTibber-0.9.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2563 2019-03-15 13:51:14.000000 pyTibber-0.9.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-15 13:51:14.000000 pyTibber-0.9.8/pyTibber.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-03-15 13:51:14.000000 pyTibber-0.9.8/pyTibber.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-03-15 13:51:14.000000 pyTibber-0.9.8/pyTibber.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2563 2019-03-15 13:51:14.000000 pyTibber-0.9.8/pyTibber.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-15 13:51:14.000000 pyTibber-0.9.8/pyTibber.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-03-15 13:51:14.000000 pyTibber-0.9.8/pyTibber.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-15 13:51:14.000000 pyTibber-0.9.8/tibber/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18109 2019-03-15 13:50:28.000000 pyTibber-0.9.8/tibber/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-21 09:01:22.000000 pyTibber-0.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1610 2019-03-21 09:00:37.000000 pyTibber-0.9.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      975 2019-03-21 09:00:37.000000 pyTibber-0.9.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-21 09:01:22.000000 pyTibber-0.9.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-21 09:01:22.000000 pyTibber-0.9.9/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5959 2019-03-21 09:00:37.000000 pyTibber-0.9.9/test/test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2019-03-21 09:00:37.000000 pyTibber-0.9.9/License.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-21 09:00:37.000000 pyTibber-0.9.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2543 2019-03-21 09:01:22.000000 pyTibber-0.9.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-21 09:01:22.000000 pyTibber-0.9.9/pyTibber.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-03-21 09:01:22.000000 pyTibber-0.9.9/pyTibber.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-03-21 09:01:22.000000 pyTibber-0.9.9/pyTibber.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2543 2019-03-21 09:01:22.000000 pyTibber-0.9.9/pyTibber.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-21 09:01:22.000000 pyTibber-0.9.9/pyTibber.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-03-21 09:01:22.000000 pyTibber-0.9.9/pyTibber.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-21 09:01:22.000000 pyTibber-0.9.9/tibber/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18147 2019-03-21 09:00:37.000000 pyTibber-0.9.9/tibber/__init__.py
```

### Comparing `pyTibber-0.9.8/README.md` & `pyTibber-0.9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 home.sync_update_price_info()
 
 print(home.current_price_info)
 
 tibber_connection.sync_close_connection()
 ```
 
-The library is used as part of Home Assitant: [https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py](https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py)
+The library is used as part of Home Assitant: [https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/tibber](https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/tibber)
```

#### html2text {}

```diff
@@ -10,10 +10,10 @@
 developer.tibber.com/) to get your API token. ## Install ``` pip3 install
 pyTibber ``` ## Example: ```python import tibber tibber_connection =
 tibber.Tibber() # access_token=YOUR_TOKEN tibber_connection.sync_update_info()
 print(tibber_connection.name) home = tibber_connection.get_homes()[0]
 home.sync_update_info() print(home.address1) home.sync_update_price_info()
 print(home.current_price_info) tibber_connection.sync_close_connection() ```
 The library is used as part of Home Assitant: [https://github.com/home-
-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py]
-(https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/
-components/sensor/tibber.py)
+assistant/home-assistant/tree/dev/homeassistant/components/tibber](https://
+github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/
+tibber)
```

### Comparing `pyTibber-0.9.8/setup.py` & `pyTibber-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name = 'pyTibber',
     packages = ['tibber'],
     install_requires=['gql>=0.1.0', 'aiohttp>=3.0.6',
                       'async_timeout>=1.4.0', 'websockets>=6.0',
                       'graphql-subscription-manager>=0.2.7'],
-    version='0.9.8',
+    version='0.9.9',
     description='A python3 library to communicate with Tibber',
     long_description=long_description,
     python_requires='>=3.5.3',
     author='Daniel Hoyer Iversen',
     author_email='mail@dahoiv.net',
     url='https://github.com/Danielhiversen/pyTibber',
     license="MIT",
```

### Comparing `pyTibber-0.9.8/test/test.py` & `pyTibber-0.9.9/test/test.py`

 * *Files identical despite different names*

### Comparing `pyTibber-0.9.8/License.txt` & `pyTibber-0.9.9/License.txt`

 * *Files identical despite different names*

### Comparing `pyTibber-0.9.8/PKG-INFO` & `pyTibber-0.9.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyTibber
-Version: 0.9.8
+Version: 0.9.9
 Summary: A python3 library to communicate with Tibber
 Home-page: https://github.com/Danielhiversen/pyTibber
 Author: Daniel Hoyer Iversen
 Author-email: mail@dahoiv.net
 License: MIT
 Description: # pyTibber 
         [![Build Status](https://travis-ci.org/Danielhiversen/pyTibber.svg?branch=master)](https://travis-ci.org/Danielhiversen/pyTibber)
@@ -45,15 +45,15 @@
         home.sync_update_price_info()
         
         print(home.current_price_info)
         
         tibber_connection.sync_close_connection()
         ```
         
-        The library is used as part of Home Assitant: [https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py](https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py)
+        The library is used as part of Home Assitant: [https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/tibber](https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/tibber)
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.2 Name: pyTibber Version: 0.9.8 Summary: A python3 library
+Metadata-Version: 1.2 Name: pyTibber Version: 0.9.9 Summary: A python3 library
 to communicate with Tibber Home-page: https://github.com/Danielhiversen/
 pyTibber Author: Daniel Hoyer Iversen Author-email: mail@dahoiv.net License:
 MIT Description: # pyTibber [![Build Status](https://travis-ci.org/
 Danielhiversen/pyTibber.svg?branch=master)](https://travis-ci.org/
 Danielhiversen/pyTibber) [![Coverage Status](https://coveralls.io/repos/github/
 Danielhiversen/pyTibber/badge.svg?branch=master)](https://coveralls.io/github/
 Danielhiversen/pyTibber?branch=master) [![PyPI version](https://badge.fury.io/
@@ -13,15 +13,14 @@
 [developer.tibber.com/](https://developer.tibber.com/) to get your API token.
 ## Install ``` pip3 install pyTibber ``` ## Example: ```python import tibber
 tibber_connection = tibber.Tibber() # access_token=YOUR_TOKEN
 tibber_connection.sync_update_info() print(tibber_connection.name) home =
 tibber_connection.get_homes()[0] home.sync_update_info() print(home.address1)
 home.sync_update_price_info() print(home.current_price_info)
 tibber_connection.sync_close_connection() ``` The library is used as part of
-Home Assitant: [https://github.com/home-assistant/home-assistant/blob/dev/
-homeassistant/components/sensor/tibber.py](https://github.com/home-assistant/
-home-assistant/blob/dev/homeassistant/components/sensor/tibber.py) Platform:
-UNKNOWN Classifier: Intended Audience :: Developers Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Home Automation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5.3
+Home Assitant: [https://github.com/home-assistant/home-assistant/tree/dev/
+homeassistant/components/tibber](https://github.com/home-assistant/home-
+assistant/tree/dev/homeassistant/components/tibber) Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Home Automation Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Requires-Python: >=3.5.3
```

### Comparing `pyTibber-0.9.8/pyTibber.egg-info/PKG-INFO` & `pyTibber-0.9.9/pyTibber.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyTibber
-Version: 0.9.8
+Version: 0.9.9
 Summary: A python3 library to communicate with Tibber
 Home-page: https://github.com/Danielhiversen/pyTibber
 Author: Daniel Hoyer Iversen
 Author-email: mail@dahoiv.net
 License: MIT
 Description: # pyTibber 
         [![Build Status](https://travis-ci.org/Danielhiversen/pyTibber.svg?branch=master)](https://travis-ci.org/Danielhiversen/pyTibber)
@@ -45,15 +45,15 @@
         home.sync_update_price_info()
         
         print(home.current_price_info)
         
         tibber_connection.sync_close_connection()
         ```
         
-        The library is used as part of Home Assitant: [https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py](https://github.com/home-assistant/home-assistant/blob/dev/homeassistant/components/sensor/tibber.py)
+        The library is used as part of Home Assitant: [https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/tibber](https://github.com/home-assistant/home-assistant/tree/dev/homeassistant/components/tibber)
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.2 Name: pyTibber Version: 0.9.8 Summary: A python3 library
+Metadata-Version: 1.2 Name: pyTibber Version: 0.9.9 Summary: A python3 library
 to communicate with Tibber Home-page: https://github.com/Danielhiversen/
 pyTibber Author: Daniel Hoyer Iversen Author-email: mail@dahoiv.net License:
 MIT Description: # pyTibber [![Build Status](https://travis-ci.org/
 Danielhiversen/pyTibber.svg?branch=master)](https://travis-ci.org/
 Danielhiversen/pyTibber) [![Coverage Status](https://coveralls.io/repos/github/
 Danielhiversen/pyTibber/badge.svg?branch=master)](https://coveralls.io/github/
 Danielhiversen/pyTibber?branch=master) [![PyPI version](https://badge.fury.io/
@@ -13,15 +13,14 @@
 [developer.tibber.com/](https://developer.tibber.com/) to get your API token.
 ## Install ``` pip3 install pyTibber ``` ## Example: ```python import tibber
 tibber_connection = tibber.Tibber() # access_token=YOUR_TOKEN
 tibber_connection.sync_update_info() print(tibber_connection.name) home =
 tibber_connection.get_homes()[0] home.sync_update_info() print(home.address1)
 home.sync_update_price_info() print(home.current_price_info)
 tibber_connection.sync_close_connection() ``` The library is used as part of
-Home Assitant: [https://github.com/home-assistant/home-assistant/blob/dev/
-homeassistant/components/sensor/tibber.py](https://github.com/home-assistant/
-home-assistant/blob/dev/homeassistant/components/sensor/tibber.py) Platform:
-UNKNOWN Classifier: Intended Audience :: Developers Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Home Automation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5.3
+Home Assitant: [https://github.com/home-assistant/home-assistant/tree/dev/
+homeassistant/components/tibber](https://github.com/home-assistant/home-
+assistant/tree/dev/homeassistant/components/tibber) Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Home Automation Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Requires-Python: >=3.5.3
```

### Comparing `pyTibber-0.9.8/tibber/__init__.py` & `pyTibber-0.9.9/tibber/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,14 +508,15 @@
         document = gql(
             """
             subscription{
               liveMeasurement(homeId:"%s"){
                 timestamp
                 power
                 powerProduction
+                accumulatedProduction
                 accumulatedConsumption
                 accumulatedCost
                 currency
                 minPower
                 averagePower
                 maxPower
                 voltagePhase1
```

