# Comparing `tmp/swiftshadow-0.1.2.tar.gz` & `tmp/swiftshadow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.1.2.tar", last modified: Tue Apr 25 10:50:21 2023, max compression
+gzip compressed data, was "swiftshadow-0.2.0.tar", last modified: Thu Apr 27 09:54:34 2023, max compression
```

## Comparing `swiftshadow-0.1.2.tar` & `swiftshadow-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.1.2/LICENSE` & `swiftshadow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.2/PKG-INFO` & `swiftshadow-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.1.2
+Version: 0.2.0
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swiftshadow-0.1.2/README.md` & `swiftshadow-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.2/setup.py` & `swiftshadow-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
     url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=VERSION.get("__version__", "0.1.2"),
+    version=VERSION.get("__version__", "0.2.0"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.1.2/swiftshadow/constants.py` & `swiftshadow-0.2.0/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.2/swiftshadow/helpers.py` & `swiftshadow-0.2.0/swiftshadow/helpers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.2/swiftshadow/providers.py` & `swiftshadow-0.2.0/swiftshadow/providers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.2/swiftshadow/swiftshadow.py` & `swiftshadow-0.2.0/swiftshadow/swiftshadow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from requests import get
 from random import choice
 from datetime import datetime, timezone, timedelta
 from pickle import dump, load
 from swiftshadow.helpers import log
 from swiftshadow.providers import Proxyscrape, Scrapingant
+import swiftshadow.cache as cache
 
 
 class Proxy:
     def __init__(
         self,
         countries: list = [],
         protocol: str = "http",
@@ -40,15 +41,15 @@
                 Proxies are sourced from **Proxyscrape** and **Scrapingant** websites which are freely available and validated locally.
         """
         self.countries = [i.upper() for i in countries]
         self.protocol = protocol
         self.maxProxies = maxProxies
         self.autoRotate = autoRotate
         self.cachePeriod = cachePeriod
-        self.updateProxyList()
+        self.update()
 
     def checkIp(self, ip, cc, protocol):
         if (ip[1] == cc or cc == None) and ip[2] == protocol:
             proxy = {ip[2]: ip[0]}
             try:
                 oip = get(f"{protocol}://ipinfo.io/ip", proxies=proxy).text
             except:
@@ -56,43 +57,32 @@
             if oip.count(".") == 3 and oip != self.mip:
                 return True
             else:
                 return False
         else:
             return False
 
-    def checkCache(self, latest, cache=datetime.now(timezone.utc)):
-        expiry = latest + timedelta(minutes=self.cachePeriod)
-        live = cache - latest
-        dead = expiry - cache
-        limit = float(self.cachePeriod)
-        if live.seconds / 60 < limit and dead.seconds / 60 < limit:
-            cacheValid = True
-        else:
-            cacheValid = False
-        return cacheValid
-
-    def updateProxyList(self):
+    def update(self):
         try:
             with open(".swiftshadow.dat", "rb") as file:
                 data = load(file)
-                self.latest = data[0]
-                cacheState = self.checkCache(self.latest)
-            if cacheState:
+                self.expiry = data[0]
+                expired = cache.checkExpiry(self.expiry)
+            if not expired:
                 log(
                     "info",
-                    f"{datetime.now(timezone.utc).time()} Loaded proxies from cache",
+                    f"Loaded proxies from cache",
                 )
                 self.proxies = data[1]
                 self.current = self.proxies[0]
                 return
             else:
                 log(
                     "info",
-                    f"{datetime.now(timezone.utc).time()} Cache expired. Updating cache...",
+                    f"Cache expired. Updating cache...",
                 )
         except FileNotFoundError:
             log("error", "No cache found. Cache will be created after update")
 
         self.proxies = []
         self.proxies.extend(Proxyscrape(self.maxProxies, self.countries, self.protocol))
         if len(self.proxies) != self.maxProxies:
@@ -102,36 +92,44 @@
         if len(self.proxies) == 0:
             log(
                 "warn",
                 "No proxies found for current settings. To prevent runtime error updating the proxy list again.",
             )
             self.update()
         with open(".swiftshadow.dat", "wb") as file:
-            dump([datetime.now(timezone.utc), self.proxies], file)
+            dump([cache.getExpiry(self.cachePeriod), self.proxies], file)
         self.current = self.proxies[0]
 
     def rotate(self):
         """
         Rotate the current proxy.
 
         Sets the current proxy to a random one from available proxies and also validates cache.
 
         Note:
                 Function only for manual rotation. If `autoRotate` is set to `True` then no need to call this function.
         """
-        if not self.checkCache(self.latest):
+        if cache.checkExpiry(self.expiry):
             self.update()
         self.current = choice(self.proxies)
 
     def proxy(self):
         """
         Returns a proxy dict.
 
         Returns:
                 proxyDict (dict):A proxy dict of format `{protocol:address}`
         """
-        if not self.checkCache(self.latest):
+        if cache.checkExpiry(self.expiry):
             self.update()
         if self.autoRotate == True:
             return choice(self.proxies)
         else:
             return self.current
+
+
+from time import sleep
+
+a = Proxy(cachePeriod=1, maxProxies=1)
+while True:
+    print(a.proxy())
+    sleep(1)
```

### Comparing `swiftshadow-0.1.2/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-0.2.0/swiftshadow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.1.2
+Version: 0.2.0
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

