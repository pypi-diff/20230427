# Comparing `tmp/tonconsole-0.0.1.tar.gz` & `tmp/tonconsole-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconsole-0.0.1.tar", last modified: Thu Apr 27 08:13:53 2023, max compression
+gzip compressed data, was "tonconsole-0.0.2.tar", last modified: Thu Apr 27 08:24:09 2023, max compression
```

## Comparing `tonconsole-0.0.1.tar` & `tonconsole-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:13:53.583683 tonconsole-0.0.1/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-04-27 08:03:37.000000 tonconsole-0.0.1/LICENSE
--rw-rw-r--   0 ness      (1000) ness      (1000)      581 2023-04-27 08:13:53.583683 tonconsole-0.0.1/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)      136 2023-04-27 08:06:09.000000 tonconsole-0.0.1/README.md
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-27 08:13:53.583683 tonconsole-0.0.1/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      744 2023-04-27 08:12:16.000000 tonconsole-0.0.1/setup.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:13:53.579683 tonconsole-0.0.1/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-26 08:31:05.000000 tonconsole-0.0.1/tonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:13:53.579683 tonconsole-0.0.1/tonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1037 2023-04-18 02:22:36.000000 tonconsole-0.0.1/tonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1649 2023-04-27 08:11:48.000000 tonconsole-0.0.1/tonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:13:53.579683 tonconsole-0.0.1/tonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-18 02:18:29.000000 tonconsole-0.0.1/tonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3398 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      490 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2656 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/async_tonapi/methods/nfts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      537 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      997 2023-04-27 08:10:42.000000 tonconsole-0.0.1/tonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:13:53.583683 tonconsole-0.0.1/tonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1733 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      458 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      316 2023-04-27 08:02:02.000000 tonconsole-0.0.1/tonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-04-18 02:03:45.000000 tonconsole-0.0.1/tonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-04-18 01:03:47.000000 tonconsole-0.0.1/tonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2955 2023-04-18 09:06:47.000000 tonconsole-0.0.1/tonapi/schema/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-04-11 17:45:48.000000 tonconsole-0.0.1/tonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:13:53.583683 tonconsole-0.0.1/tonconsole.egg-info/
--rw-rw-r--   0 ness      (1000) ness      (1000)      581 2023-04-27 08:13:53.000000 tonconsole-0.0.1/tonconsole.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)      653 2023-04-27 08:13:53.000000 tonconsole-0.0.1/tonconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-04-27 08:13:53.000000 tonconsole-0.0.1/tonconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       47 2023-04-27 08:13:53.000000 tonconsole-0.0.1/tonconsole.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        7 2023-04-27 08:13:53.000000 tonconsole-0.0.1/tonconsole.egg-info/top_level.txt
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.451875 tonconsole-0.0.2/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-04-27 08:03:37.000000 tonconsole-0.0.2/LICENSE
+-rw-rw-r--   0 ness      (1000) ness      (1000)      581 2023-04-27 08:24:09.451875 tonconsole-0.0.2/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)      136 2023-04-27 08:06:09.000000 tonconsole-0.0.2/README.md
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-27 08:24:09.451875 tonconsole-0.0.2/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      748 2023-04-27 08:23:49.000000 tonconsole-0.0.2/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.447875 tonconsole-0.0.2/tonconsole/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-27 08:22:40.000000 tonconsole-0.0.2/tonconsole/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.447875 tonconsole-0.0.2/tonconsole/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-04-26 08:31:05.000000 tonconsole-0.0.2/tonconsole/tonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.447875 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1037 2023-04-18 02:22:36.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1704 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.447875 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-04-18 02:18:29.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3464 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      512 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2678 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/nfts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      559 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      997 2023-04-27 08:10:42.000000 tonconsole-0.0.2/tonconsole/tonapi/exceptions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.451875 tonconsole-0.0.2/tonconsole/tonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1744 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      469 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      327 2023-04-27 08:23:22.000000 tonconsole-0.0.2/tonconsole/tonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-04-18 02:03:45.000000 tonconsole-0.0.2/tonconsole/tonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-04-18 01:03:47.000000 tonconsole-0.0.2/tonconsole/tonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2955 2023-04-18 09:06:47.000000 tonconsole-0.0.2/tonconsole/tonapi/schema/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-04-11 17:45:48.000000 tonconsole-0.0.2/tonconsole/tonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-04-27 08:24:09.447875 tonconsole-0.0.2/tonconsole.egg-info/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      581 2023-04-27 08:24:09.000000 tonconsole-0.0.2/tonconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)      852 2023-04-27 08:24:09.000000 tonconsole-0.0.2/tonconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-04-27 08:24:09.000000 tonconsole-0.0.2/tonconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       47 2023-04-27 08:24:09.000000 tonconsole-0.0.2/tonconsole.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       11 2023-04-27 08:24:09.000000 tonconsole-0.0.2/tonconsole.egg-info/top_level.txt
```

### Comparing `tonconsole-0.0.1/LICENSE` & `tonconsole-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/PKG-INFO` & `tonconsole-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconsole
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connecting businesses to the TON ecosystem.
 Home-page: https://github.com/nessshon/tonconsole/
 Author: nessshon
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tonconsole-0.0.1/setup.py` & `tonconsole-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tonconsole",
-    version="0.0.1",
+    version="0.0.2",
     author="nessshon",
     description="Connecting businesses to the TON ecosystem.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nessshon/tonconsole/",
-    packages=setuptools.find_packages(exclude="tonapi"),
+    packages=setuptools.find_packages(exclude="tonconsole"),
     python_requires='>=3.10',
     install_requires=[
         "aiohttp>=3.8.3",
         "libscrc>=1.8.1",
         "pydantic>=1.10.4",
     ],
     classifiers=[
```

### Comparing `tonconsole-0.0.1/tonapi/async_tonapi/__init__.py` & `tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/tonapi/async_tonapi/client.py` & `tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import aiohttp
 
-from tonapi.exceptions import (TONAPIError,
-                               TONAPINotFoundError,
-                               TONAPIBadRequestError,
-                               TONAPIUnauthorizedError,
-                               TONAPIInternalServerError)
+from tonconsole.tonapi.exceptions import (TONAPIError,
+                                          TONAPINotFoundError,
+                                          TONAPIBadRequestError,
+                                          TONAPIUnauthorizedError,
+                                          TONAPIInternalServerError)
 
 
 class AsyncTonapiClient:
 
     def __init__(self, api_key: str, testnet: bool = False):
         self._api_key = api_key
         self._testnet = testnet
```

### Comparing `tonconsole-0.0.1/tonapi/async_tonapi/methods/accounts.py` & `tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/accounts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from tonapi.async_tonapi.client import AsyncTonapiClient
+from tonconsole.tonapi.async_tonapi.client import AsyncTonapiClient
 
-from tonapi.schema.accounts import Account
-from tonapi.schema.domains import DomainNames
-from tonapi.schema.jettons import JettonsBalances
-from tonapi.schema.nft import NftItems
-from tonapi.schema.traces import TraceIds
+from tonconsole.tonapi.schema.accounts import Account
+from tonconsole.tonapi.schema.domains import DomainNames
+from tonconsole.tonapi.schema.jettons import JettonsBalances
+from tonconsole.tonapi.schema.nft import NftItems
+from tonconsole.tonapi.schema.traces import TraceIds
 
 
 class AccountMethod(AsyncTonapiClient):
 
     async def get_info(self, account_id: str) -> Account:
         """
         Get human-friendly information about an account without low-level details.
```

### Comparing `tonconsole-0.0.1/tonapi/async_tonapi/methods/nfts.py` & `tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/nfts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from tonapi.async_tonapi.client import AsyncTonapiClient
+from tonconsole.tonapi.async_tonapi.client import AsyncTonapiClient
 
-from tonapi.schema.nft import NftCollections, NftCollection, NftItems, NftItem
+from tonconsole.tonapi.schema.nft import NftCollections, NftCollection, NftItems, NftItem
 
 
 class NftMethod(AsyncTonapiClient):
 
     async def get_collections(self, limit: int = 15, offset: int = 0) -> NftCollections:
         """
         Get NFT collections.
```

### Comparing `tonconsole-0.0.1/tonapi/async_tonapi/methods/traces.py` & `tonconsole-0.0.2/tonconsole/tonapi/async_tonapi/methods/traces.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from tonapi.async_tonapi import AsyncTonapiClient
+from tonconsole.tonapi.async_tonapi import AsyncTonapiClient
 
-from tonapi.schema.traces import Trace
+from tonconsole.tonapi.schema.traces import Trace
 
 
 class TraceMethod(AsyncTonapiClient):
 
     async def get_trace(self, trace_id: str) -> Trace:
         """
         Get the trace by trace ID or hash of any transaction in trace.
```

### Comparing `tonconsole-0.0.1/tonapi/exceptions.py` & `tonconsole-0.0.2/tonconsole/tonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/tonapi/schema/__init__.py` & `tonconsole-0.0.2/tonconsole/tonapi/schema/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import BaseModel
 
-from tonapi.utils import nano_to_amount, raw_to_userfriendly
+from tonconsole.tonapi.utils import nano_to_amount, raw_to_userfriendly
 
 
 class Address(BaseModel):
     __root__: str
 
     def __str__(self) -> str:
         return self.__root__
```

### Comparing `tonconsole-0.0.1/tonapi/schema/jettons.py` & `tonconsole-0.0.2/tonconsole/tonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/tonapi/schema/nft.py` & `tonconsole-0.0.2/tonconsole/tonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/tonapi/schema/traces.py` & `tonconsole-0.0.2/tonconsole/tonapi/schema/traces.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/tonapi/utils.py` & `tonconsole-0.0.2/tonconsole/tonapi/utils.py`

 * *Files identical despite different names*

### Comparing `tonconsole-0.0.1/tonconsole.egg-info/PKG-INFO` & `tonconsole-0.0.2/tonconsole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconsole
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connecting businesses to the TON ecosystem.
 Home-page: https://github.com/nessshon/tonconsole/
 Author: nessshon
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

