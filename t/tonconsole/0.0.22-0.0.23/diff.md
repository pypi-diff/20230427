# Comparing `tmp/tonconsole-0.0.22.tar.gz` & `tmp/tonconsole-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconsole-0.0.22.tar", last modified: Thu Apr 27 09:35:48 2023, max compression
+gzip compressed data, was "tonconsole-0.0.23.tar", last modified: Thu Apr 27 09:44:19 2023, max compression
```

## Comparing `tonconsole-0.0.22.tar` & `tonconsole-0.0.23.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.139819 tonconsole-0.0.22/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-04-27 08:03:37.000000 tonconsole-0.0.22/LICENSE
--rw-rw-r--   0 ness      (1000) ness      (1000)      582 2023-04-27 09:35:48.139819 tonconsole-0.0.22/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)      136 2023-04-27 08:06:09.000000 tonconsole-0.0.22/README.md
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-27 09:35:48.139819 tonconsole-0.0.22/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      749 2023-04-27 09:35:34.000000 tonconsole-0.0.22/setup.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.135820 tonconsole-0.0.22/tonconsole/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-27 08:22:40.000000 tonconsole-0.0.22/tonconsole/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.139819 tonconsole-0.0.22/tonconsole/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-26 08:31:05.000000 tonconsole-0.0.22/tonconsole/tonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.139819 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1037 2023-04-18 02:22:36.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1699 2023-04-27 09:35:34.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.139819 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-18 02:18:29.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3464 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      512 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2678 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/nfts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      559 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      997 2023-04-27 08:10:42.000000 tonconsole-0.0.22/tonconsole/tonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.139819 tonconsole-0.0.22/tonconsole/tonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1744 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      469 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      327 2023-04-27 08:23:22.000000 tonconsole-0.0.22/tonconsole/tonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-04-18 02:03:45.000000 tonconsole-0.0.22/tonconsole/tonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-04-18 01:03:47.000000 tonconsole-0.0.22/tonconsole/tonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2955 2023-04-18 09:06:47.000000 tonconsole-0.0.22/tonconsole/tonapi/schema/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-04-11 17:45:48.000000 tonconsole-0.0.22/tonconsole/tonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:35:48.139819 tonconsole-0.0.22/tonconsole.egg-info/
--rw-rw-r--   0 ness      (1000) ness      (1000)      582 2023-04-27 09:35:48.000000 tonconsole-0.0.22/tonconsole.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)      852 2023-04-27 09:35:48.000000 tonconsole-0.0.22/tonconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-04-27 09:35:48.000000 tonconsole-0.0.22/tonconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       47 2023-04-27 09:35:48.000000 tonconsole-0.0.22/tonconsole.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       11 2023-04-27 09:35:48.000000 tonconsole-0.0.22/tonconsole.egg-info/top_level.txt
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-04-27 08:03:37.000000 tonconsole-0.0.23/LICENSE
+-rw-rw-r--   0 ness      (1000) ness      (1000)      582 2023-04-27 09:44:19.570738 tonconsole-0.0.23/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)      136 2023-04-27 08:06:09.000000 tonconsole-0.0.23/README.md
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-27 09:44:19.570738 tonconsole-0.0.23/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      749 2023-04-27 09:44:14.000000 tonconsole-0.0.23/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/tonconsole/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-27 08:22:40.000000 tonconsole-0.0.23/tonconsole/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/tonconsole/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-26 08:31:05.000000 tonconsole-0.0.23/tonconsole/tonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1037 2023-04-18 02:22:36.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1699 2023-04-27 09:37:49.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-18 02:18:29.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3464 2023-04-27 08:23:22.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      512 2023-04-27 08:23:22.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2678 2023-04-27 08:23:22.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/nfts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      618 2023-04-27 09:43:34.000000 tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      997 2023-04-27 08:10:42.000000 tonconsole-0.0.23/tonconsole/tonapi/exceptions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/tonconsole/tonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1744 2023-04-27 08:23:22.000000 tonconsole-0.0.23/tonconsole/tonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      469 2023-04-27 08:23:22.000000 tonconsole-0.0.23/tonconsole/tonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      327 2023-04-27 08:23:22.000000 tonconsole-0.0.23/tonconsole/tonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-04-18 02:03:45.000000 tonconsole-0.0.23/tonconsole/tonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-04-18 01:03:47.000000 tonconsole-0.0.23/tonconsole/tonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2955 2023-04-18 09:06:47.000000 tonconsole-0.0.23/tonconsole/tonapi/schema/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-04-11 17:45:48.000000 tonconsole-0.0.23/tonconsole/tonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 09:44:19.570738 tonconsole-0.0.23/tonconsole.egg-info/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      582 2023-04-27 09:44:19.000000 tonconsole-0.0.23/tonconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)      852 2023-04-27 09:44:19.000000 tonconsole-0.0.23/tonconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-04-27 09:44:19.000000 tonconsole-0.0.23/tonconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       47 2023-04-27 09:44:19.000000 tonconsole-0.0.23/tonconsole.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       11 2023-04-27 09:44:19.000000 tonconsole-0.0.23/tonconsole.egg-info/top_level.txt
```

### Comparing `tonconsole-0.0.22/LICENSE` & `tonconsole-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/PKG-INFO` & `tonconsole-0.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconsole
-Version: 0.0.22
+Version: 0.0.23
 Summary: Connecting businesses to the TON ecosystem.
 Home-page: https://github.com/nessshon/tonconsole/
 Author: nessshon
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tonconsole-0.0.22/setup.py` & `tonconsole-0.0.23/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tonconsole",
-    version="0.0.22",
+    version="0.0.23",
     author="nessshon",
     description="Connecting businesses to the TON ecosystem.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nessshon/tonconsole/",
     packages=setuptools.find_packages(exclude="tonconsole"),
     python_requires='>=3.10',
```

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/__init__.py` & `tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/client.py` & `tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         params = params.copy() if params is not None else {}
 
         async with aiohttp.ClientSession(headers=self.__headers) as session:
             async with await session.get(f"{self.__base_url}{method}",
                                          params=params,
                                          ) as response:
                 response_json = await response.json()
-                error = response_json.get('error', response_json)
+                error = response_json.get('Error', response_json)
 
                 match response.status:
                     case 200:
                         return response_json
                     case 400:
                         raise TONAPIBadRequestError(error)
                     case 401:
```

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/accounts.py` & `tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/jettons.py` & `tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/jettons.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/async_tonapi/methods/nfts.py` & `tonconsole-0.0.23/tonconsole/tonapi/async_tonapi/methods/nfts.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/exceptions.py` & `tonconsole-0.0.23/tonconsole/tonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/schema/__init__.py` & `tonconsole-0.0.23/tonconsole/tonapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/schema/jettons.py` & `tonconsole-0.0.23/tonconsole/tonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/schema/nft.py` & `tonconsole-0.0.23/tonconsole/tonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/schema/traces.py` & `tonconsole-0.0.23/tonconsole/tonapi/schema/traces.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole/tonapi/utils.py` & `tonconsole-0.0.23/tonconsole/tonapi/utils.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.22/tonconsole.egg-info/PKG-INFO` & `tonconsole-0.0.23/tonconsole.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconsole
-Version: 0.0.22
+Version: 0.0.23
 Summary: Connecting businesses to the TON ecosystem.
 Home-page: https://github.com/nessshon/tonconsole/
 Author: nessshon
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tonconsole-0.0.22/tonconsole.egg-info/SOURCES.txt` & `tonconsole-0.0.23/tonconsole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

