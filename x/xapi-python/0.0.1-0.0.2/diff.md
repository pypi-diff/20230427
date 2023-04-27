# Comparing `tmp/xapi-python-0.0.1.tar.gz` & `tmp/xapi-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.0.1.tar", last modified: Tue Apr 25 12:50:19 2023, max compression
+gzip compressed data, was "xapi-python-0.0.2.tar", last modified: Thu Apr 27 06:57:11 2023, max compression
```

## Comparing `xapi-python-0.0.1.tar` & `xapi-python-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-25 12:50:19.717937 xapi-python-0.0.1/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.0.1/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5923 2023-04-25 12:50:19.717937 xapi-python-0.0.1/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5127 2023-04-25 11:16:58.000000 xapi-python-0.0.1/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)      496 2023-04-25 12:47:51.000000 xapi-python-0.0.1/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-25 12:50:19.717937 xapi-python-0.0.1/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)      712 2023-04-25 11:24:12.000000 xapi-python-0.0.1/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-25 12:50:19.707937 xapi-python-0.0.1/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      940 2023-04-25 12:20:21.000000 xapi-python-0.0.1/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-25 12:50:19.717937 xapi-python-0.0.1/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      303 2023-04-24 14:59:09.000000 xapi-python-0.0.1/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1679 2023-04-25 08:25:05.000000 xapi-python-0.0.1/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.0.1/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      200 2023-04-24 12:09:22.000000 xapi-python-0.0.1/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-24 15:09:27.000000 xapi-python-0.0.1/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3115 2023-04-24 13:51:23.000000 xapi-python-0.0.1/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1104 2023-04-25 10:53:24.000000 xapi-python-0.0.1/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-25 12:50:19.717937 xapi-python-0.0.1/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5923 2023-04-25 12:50:19.000000 xapi-python-0.0.1/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      312 2023-04-25 12:50:19.000000 xapi-python-0.0.1/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-25 12:50:19.000000 xapi-python-0.0.1/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-25 12:50:19.000000 xapi-python-0.0.1/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.0.2/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-27 06:57:11.094159 xapi-python-0.0.2/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5591 2023-04-26 13:10:27.000000 xapi-python-0.0.2/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1075 2023-04-27 06:52:41.000000 xapi-python-0.0.2/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-04-27 06:57:11.094159 xapi-python-0.0.2/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1011 2023-04-27 06:53:55.000000 xapi-python-0.0.2/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5636 2023-04-27 06:31:53.000000 xapi-python-0.0.2/tests/test_connect.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.0.2/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.0.2/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-26 11:04:33.000000 xapi-python-0.0.2/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-04-27 06:12:53.000000 xapi-python-0.0.2/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2041 2023-04-27 06:06:45.000000 xapi-python-0.0.2/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.0.2/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      200 2023-04-24 12:09:22.000000 xapi-python-0.0.2/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-26 08:53:56.000000 xapi-python-0.0.2/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-26 09:47:15.000000 xapi-python-0.0.2/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1104 2023-04-26 06:51:38.000000 xapi-python-0.0.2/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-04-27 06:57:11.094159 xapi-python-0.0.2/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7880 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-04-27 06:57:11.000000 xapi-python-0.0.2/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.0.1/LICENSE` & `xapi-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.1/PKG-INFO` & `xapi-python-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-Metadata-Version: 2.1
-Name: xapi-python
-Version: 0.0.1
-Summary: The xStation5 API Python library
-Home-page: https://github.com/pawelkn/xapi-python
-Author: Paweł Knioła
-Author-email: Paweł Knioła <pawel.kn@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Keywords: python trading websocket trading-api forex xapi forex-trading exchange-api forex-data xstation5 xtb xopenhub forex-api xopenhub-api xtb-api xstation-api x-trade-brokers bfbcapital xstation
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # xStation5 API Python Library
 
-[![Test xapi-python](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml/badge.svg)](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml)
+[![Test xapi-python](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml/badge.svg)](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml) [![PyPi](https://img.shields.io/pypi/v/xapi-python.svg)](https://pypi.python.org/pypi/xapi-python/) [![Downloads](https://img.shields.io/pypi/dm/xapi-python)](https://pypi.python.org/pypi/xapi-python/) [![Codecov](https://codecov.io/gh/pawelkn/xapi-python/branch/master/graph/badge.svg)](https://codecov.io/gh/pawelkn/xapi-python/)
 
 The xStation5 API Python library provides a simple and easy-to-use API for interacting with the xStation5 trading platform. With this library, you can connect to the xStation5 platform, retrieve market data, and execute trades.
 
 This library may be used for [BFB Capital](https://bfb.capital) and [XTB](https://www.xtb.com) xStation5 accounts.
 
 API documentation: <http://developers.xstore.pro/documentation>
 
@@ -45,26 +27,27 @@
 Here is an example of how to use the xAPI library to connect to the xStation5 platform:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     try:
         # Create a new xAPI object and connect to the xStation5 platform
-        x = await xapi.connect(**credentials)
+        async with await xapi.connect(**CREDENTIALS) as x:
+            pass
 
     except xapi.LoginFailed as e:
         print(f"Log in failed: {e}")
 
     except xapi.ConnectionClosed as e:
         print(f"Connection closed: {e}")
 
@@ -77,34 +60,33 @@
 Here is an example of how to subscribe to market data using the xAPI library:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     while True:
         try:
-            x = await xapi.connect(**credentials)
-
-            # Subscribe for the current price of BITCOIN and ETHEREUM
-            await x.stream.getTickPrices("BITCOIN")
-            await x.stream.getTickPrices("ETHEREUM")
-
-            # Listen for coming price ticks
-            async for message in x.stream.listen():
-                print(message['data'])
+            async with await xapi.connect(**CREDENTIALS) as x:
+                # Subscribe for the current price of BITCOIN and ETHEREUM
+                await x.stream.getTickPrices("BITCOIN")
+                await x.stream.getTickPrices("ETHEREUM")
+
+                # Listen for coming price ticks
+                async for message in x.stream.listen():
+                    print(message['data'])
 
         except xapi.LoginFailed as e:
             print(f"Log in failed: {e}")
             return
 
         except xapi.ConnectionClosed as e:
             print(f"Connection closed: {e}, reconnecting ...")
@@ -122,39 +104,38 @@
 
 ```python
 import asyncio
 import xapi
 from xapi import TradeCmd, TradeType, TradeStatus
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     try:
-        x = await xapi.connect(**credentials)
-
-        # Open a new trade for BITCOIN
-        response = await x.socket.tradeTransaction(
-            symbol="BITCOIN",
-            cmd=TradeCmd.BUY_LIMIT,
-            type=TradeType.OPEN,
-            price=10.00,
-            volume=1
-        )
-
-        if response['status'] == True:
-            print("Transaction sent to market")
-        else:
-            print("Failed to trade a transaction", response)
+        async with await xapi.connect(**CREDENTIALS) as x:
+            # Open a new trade for BITCOIN
+            response = await x.socket.tradeTransaction(
+                symbol="BITCOIN",
+                cmd=TradeCmd.BUY_LIMIT,
+                type=TradeType.OPEN,
+                price=10.00,
+                volume=1
+            )
+
+            if response['status'] == True:
+                print("Transaction sent to market")
+            else:
+                print("Failed to trade a transaction", response)
 
     except xapi.LoginFailed as e:
         print(f"Log in failed: {e}")
 
     except xapi.ConnectionClosed as e:
         print(f"Connection closed: {e}")
 
@@ -171,23 +152,23 @@
 ### credentials.json
 
 ```json
 {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
-    "type": "demo",
-    "safe": true
+    "type": "real",
+    "safe": false
 }
 ```
 
 Once you have created the _credentials.json_ file, you can run an example using the following command:
 
 ```shell
-python3 examples/get-balance.py
+python3 examples/get-margin-level.py
 ```
 
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xapi-python-0.0.1/README.md` & `xapi-python-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,54 @@
+Metadata-Version: 2.1
+Name: xapi-python
+Version: 0.0.2
+Summary: The xStation5 API Python library
+Home-page: https://github.com/pawelkn/xapi-python
+Author: Paweł Knioła
+Author-email: Paweł Knioła <pawel.kn@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Paweł Knioła
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/pawelkn/xapi-python
+Project-URL: Bug Tracker, https://github.com/pawelkn/xapi-python/issues
+Keywords: python,trading,websocket,trading-api,forex,xapi,forex-trading,exchange-api,forex-data,xstation5,xtb,xopenhub,forex-api,xopenhub-api,xtb-api,xstation-api,x-trade-brokers,bfbcapital,xstation
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # xStation5 API Python Library
 
-[![Test xapi-python](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml/badge.svg)](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml)
+[![Test xapi-python](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml/badge.svg)](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml) [![PyPi](https://img.shields.io/pypi/v/xapi-python.svg)](https://pypi.python.org/pypi/xapi-python/) [![Downloads](https://img.shields.io/pypi/dm/xapi-python)](https://pypi.python.org/pypi/xapi-python/) [![Codecov](https://codecov.io/gh/pawelkn/xapi-python/branch/master/graph/badge.svg)](https://codecov.io/gh/pawelkn/xapi-python/)
 
 The xStation5 API Python library provides a simple and easy-to-use API for interacting with the xStation5 trading platform. With this library, you can connect to the xStation5 platform, retrieve market data, and execute trades.
 
 This library may be used for [BFB Capital](https://bfb.capital) and [XTB](https://www.xtb.com) xStation5 accounts.
 
 API documentation: <http://developers.xstore.pro/documentation>
 
@@ -27,26 +71,27 @@
 Here is an example of how to use the xAPI library to connect to the xStation5 platform:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     try:
         # Create a new xAPI object and connect to the xStation5 platform
-        x = await xapi.connect(**credentials)
+        async with await xapi.connect(**CREDENTIALS) as x:
+            pass
 
     except xapi.LoginFailed as e:
         print(f"Log in failed: {e}")
 
     except xapi.ConnectionClosed as e:
         print(f"Connection closed: {e}")
 
@@ -59,34 +104,33 @@
 Here is an example of how to subscribe to market data using the xAPI library:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     while True:
         try:
-            x = await xapi.connect(**credentials)
-
-            # Subscribe for the current price of BITCOIN and ETHEREUM
-            await x.stream.getTickPrices("BITCOIN")
-            await x.stream.getTickPrices("ETHEREUM")
-
-            # Listen for coming price ticks
-            async for message in x.stream.listen():
-                print(message['data'])
+            async with await xapi.connect(**CREDENTIALS) as x:
+                # Subscribe for the current price of BITCOIN and ETHEREUM
+                await x.stream.getTickPrices("BITCOIN")
+                await x.stream.getTickPrices("ETHEREUM")
+
+                # Listen for coming price ticks
+                async for message in x.stream.listen():
+                    print(message['data'])
 
         except xapi.LoginFailed as e:
             print(f"Log in failed: {e}")
             return
 
         except xapi.ConnectionClosed as e:
             print(f"Connection closed: {e}, reconnecting ...")
@@ -104,39 +148,38 @@
 
 ```python
 import asyncio
 import xapi
 from xapi import TradeCmd, TradeType, TradeStatus
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     try:
-        x = await xapi.connect(**credentials)
-
-        # Open a new trade for BITCOIN
-        response = await x.socket.tradeTransaction(
-            symbol="BITCOIN",
-            cmd=TradeCmd.BUY_LIMIT,
-            type=TradeType.OPEN,
-            price=10.00,
-            volume=1
-        )
-
-        if response['status'] == True:
-            print("Transaction sent to market")
-        else:
-            print("Failed to trade a transaction", response)
+        async with await xapi.connect(**CREDENTIALS) as x:
+            # Open a new trade for BITCOIN
+            response = await x.socket.tradeTransaction(
+                symbol="BITCOIN",
+                cmd=TradeCmd.BUY_LIMIT,
+                type=TradeType.OPEN,
+                price=10.00,
+                volume=1
+            )
+
+            if response['status'] == True:
+                print("Transaction sent to market")
+            else:
+                print("Failed to trade a transaction", response)
 
     except xapi.LoginFailed as e:
         print(f"Log in failed: {e}")
 
     except xapi.ConnectionClosed as e:
         print(f"Connection closed: {e}")
 
@@ -153,23 +196,23 @@
 ### credentials.json
 
 ```json
 {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
-    "type": "demo",
-    "safe": true
+    "type": "real",
+    "safe": false
 }
 ```
 
 Once you have created the _credentials.json_ file, you can run an example using the following command:
 
 ```shell
-python3 examples/get-balance.py
+python3 examples/get-margin-level.py
 ```
 
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xapi-python-0.0.1/setup.py` & `xapi-python-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,20 @@
     author_email='pawel.kn@gmail.com',
     description='The xStation5 API Python library',
     long_description=open('README.md', encoding='utf-8').read(),
     license='MIT',
     keywords='python trading websocket trading-api forex xapi forex-trading exchange-api forex-data xstation5 xtb xopenhub forex-api xopenhub-api xtb-api xstation-api x-trade-brokers bfbcapital xstation',
     url='https://github.com/pawelkn/xapi-python',
     classifiers=[
-        "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.0.1",
+    version="0.0.2",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.0.1/xapi/connection.py` & `xapi-python-0.0.2/xapi/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 from .exceptions import ConnectionClosed
 
-import websockets
+import websockets.client
+import websockets.exceptions
 import asyncio
 import json
 
-class Connection:
+class Connection():
     def __init__(self):
         self.safe = False
+        self._conn = None
 
     async def connect(self, url):
         try:
-            self.__conn = await websockets.connect(url, close_timeout=0)
+            self._conn = await websockets.client.connect(url, close_timeout=0)
 
         except asyncio.exceptions.TimeoutError:
             raise ConnectionClosed("Connection timed out")
 
         except ConnectionRefusedError:
             raise ConnectionClosed("Connection refused")
 
     async def disconnect(self):
         try:
-            await self.__conn.close()
+            if self._conn:
+                await self._conn.close()
 
-        except NameError:
+        except websockets.exceptions.ConnectionClosed:
             pass
 
+        self._conn = None
+
     async def listen(self):
         try:
-            async for message in self.__conn:
-                yield json.loads(message)
-
-        except NameError:
-            raise ConnectionClosed("Not connected")
+            if self._conn:
+                async for message in self._conn:
+                    yield json.loads(message)
+            else:
+                raise ConnectionClosed("Not connected")
 
-        except websockets.ConnectionClosed:
+        except websockets.exceptions.ConnectionClosed:
+            self._conn = None
             raise ConnectionClosed("Connection unexpectedly closed")
 
     async def _request(self, command):
         try:
-            await self.__conn.send(json.dumps(command))
+            if self._conn:
+                await self._conn.send(json.dumps(command))
+            else:
+                raise ConnectionClosed("Not connected")
 
-        except NameError:
-            raise ConnectionClosed("Not connected")
-
-        except websockets.ConnectionClosed:
+        except websockets.exceptions.ConnectionClosed:
+            self._conn = None
             raise ConnectionClosed("Connection unexpectedly closed")
 
     async def _response(self):
         try:
-            response = await self.__conn.recv()
-            return json.loads(response)
-
-        except NameError:
-            raise ConnectionClosed("Not connected")
+            if self._conn:
+                response = await self._conn.recv()
+                return json.loads(response)
+            else:
+                raise ConnectionClosed("Not connected")
 
-        except websockets.ConnectionClosed:
+        except websockets.exceptions.ConnectionClosed:
+            self._conn = None
             raise ConnectionClosed("Connection unexpectedly closed")
 
     async def _transaction(self, command):
         await self._request(command)
         return await self._response()
```

### Comparing `xapi-python-0.0.1/xapi/enums.py` & `xapi-python-0.0.2/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.1/xapi/socket.py` & `xapi-python-0.0.2/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.1/xapi/stream.py` & `xapi-python-0.0.2/xapi/stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,20 +61,14 @@
         })
 
     async def stopProfits(self):
         return await self._request({
             "command": "stopProfits"
         })
 
-    async def stopTickPrices(self, symbol: str):
-        return await self._request({
-            "command": "stopTickPrices",
-            "symbol": symbol
-        })
-
     async def getTickPrices(self, symbol: str, minArrivalTime: int = 0, maxLevel: int = 2):
         return await self._request({
             "command": "getTickPrices",
             "streamSessionId": self.streamSessionId,
             "symbol": symbol,
             "minArrivalTime": minArrivalTime,
             "maxLevel": maxLevel
```

### Comparing `xapi-python-0.0.1/xapi/xapi.py` & `xapi-python-0.0.2/xapi/xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.0.1/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.0.2/xapi_python.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,54 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Keywords: python trading websocket trading-api forex xapi forex-trading exchange-api forex-data xstation5 xtb xopenhub forex-api xopenhub-api xtb-api xstation-api x-trade-brokers bfbcapital xstation
-Classifier: Programming Language :: Python :: 3
+License: MIT License
+        
+        Copyright (c) 2023 Paweł Knioła
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/pawelkn/xapi-python
+Project-URL: Bug Tracker, https://github.com/pawelkn/xapi-python/issues
+Keywords: python,trading,websocket,trading-api,forex,xapi,forex-trading,exchange-api,forex-data,xstation5,xtb,xopenhub,forex-api,xopenhub-api,xtb-api,xstation-api,x-trade-brokers,bfbcapital,xstation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xStation5 API Python Library
 
-[![Test xapi-python](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml/badge.svg)](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml)
+[![Test xapi-python](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml/badge.svg)](https://github.com/pawelkn/xapi-python/actions/workflows/test-xapi-python.yml) [![PyPi](https://img.shields.io/pypi/v/xapi-python.svg)](https://pypi.python.org/pypi/xapi-python/) [![Downloads](https://img.shields.io/pypi/dm/xapi-python)](https://pypi.python.org/pypi/xapi-python/) [![Codecov](https://codecov.io/gh/pawelkn/xapi-python/branch/master/graph/badge.svg)](https://codecov.io/gh/pawelkn/xapi-python/)
 
 The xStation5 API Python library provides a simple and easy-to-use API for interacting with the xStation5 trading platform. With this library, you can connect to the xStation5 platform, retrieve market data, and execute trades.
 
 This library may be used for [BFB Capital](https://bfb.capital) and [XTB](https://www.xtb.com) xStation5 accounts.
 
 API documentation: <http://developers.xstore.pro/documentation>
 
@@ -45,26 +71,27 @@
 Here is an example of how to use the xAPI library to connect to the xStation5 platform:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     try:
         # Create a new xAPI object and connect to the xStation5 platform
-        x = await xapi.connect(**credentials)
+        async with await xapi.connect(**CREDENTIALS) as x:
+            pass
 
     except xapi.LoginFailed as e:
         print(f"Log in failed: {e}")
 
     except xapi.ConnectionClosed as e:
         print(f"Connection closed: {e}")
 
@@ -77,34 +104,33 @@
 Here is an example of how to subscribe to market data using the xAPI library:
 
 ```python
 import asyncio
 import xapi
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     while True:
         try:
-            x = await xapi.connect(**credentials)
-
-            # Subscribe for the current price of BITCOIN and ETHEREUM
-            await x.stream.getTickPrices("BITCOIN")
-            await x.stream.getTickPrices("ETHEREUM")
-
-            # Listen for coming price ticks
-            async for message in x.stream.listen():
-                print(message['data'])
+            async with await xapi.connect(**CREDENTIALS) as x:
+                # Subscribe for the current price of BITCOIN and ETHEREUM
+                await x.stream.getTickPrices("BITCOIN")
+                await x.stream.getTickPrices("ETHEREUM")
+
+                # Listen for coming price ticks
+                async for message in x.stream.listen():
+                    print(message['data'])
 
         except xapi.LoginFailed as e:
             print(f"Log in failed: {e}")
             return
 
         except xapi.ConnectionClosed as e:
             print(f"Connection closed: {e}, reconnecting ...")
@@ -122,39 +148,38 @@
 
 ```python
 import asyncio
 import xapi
 from xapi import TradeCmd, TradeType, TradeStatus
 
 # Replace these values with your own credentials
-credentials = {
+CREDENTIALS = {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
     "type": "real",
     "safe": False
 }
 
 async def main():
     try:
-        x = await xapi.connect(**credentials)
-
-        # Open a new trade for BITCOIN
-        response = await x.socket.tradeTransaction(
-            symbol="BITCOIN",
-            cmd=TradeCmd.BUY_LIMIT,
-            type=TradeType.OPEN,
-            price=10.00,
-            volume=1
-        )
-
-        if response['status'] == True:
-            print("Transaction sent to market")
-        else:
-            print("Failed to trade a transaction", response)
+        async with await xapi.connect(**CREDENTIALS) as x:
+            # Open a new trade for BITCOIN
+            response = await x.socket.tradeTransaction(
+                symbol="BITCOIN",
+                cmd=TradeCmd.BUY_LIMIT,
+                type=TradeType.OPEN,
+                price=10.00,
+                volume=1
+            )
+
+            if response['status'] == True:
+                print("Transaction sent to market")
+            else:
+                print("Failed to trade a transaction", response)
 
     except xapi.LoginFailed as e:
         print(f"Log in failed: {e}")
 
     except xapi.ConnectionClosed as e:
         print(f"Connection closed: {e}")
 
@@ -171,23 +196,23 @@
 ### credentials.json
 
 ```json
 {
     "accountId": "<your_client_id>",
     "password": "<your_password>",
     "host": "ws.xtb.com",
-    "type": "demo",
-    "safe": true
+    "type": "real",
+    "safe": false
 }
 ```
 
 Once you have created the _credentials.json_ file, you can run an example using the following command:
 
 ```shell
-python3 examples/get-balance.py
+python3 examples/get-margin-level.py
 ```
 
 ## Unit Tests
 
 This will run all of the unit tests in the tests directory:
 
 ```shell
```

