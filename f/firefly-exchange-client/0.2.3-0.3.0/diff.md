# Comparing `tmp/firefly_exchange_client-0.2.3.tar.gz` & `tmp/firefly_exchange_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.2.3.tar", last modified: Wed Apr 26 08:22:20 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.3.0.tar", last modified: Thu Apr 27 09:39:21 2023, max compression
```

## Comparing `firefly_exchange_client-0.2.3.tar` & `firefly_exchange_client-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.000588 firefly_exchange_client-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    32136 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 08:22:20.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.337369 firefly_exchange_client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:39:21.337369 firefly_exchange_client-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-27 09:39:08.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:39:21.333369 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 09:39:21.000000 firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.2.3/LICENSE` & `firefly_exchange_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/PKG-INFO` & `firefly_exchange_client-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.2.3
+Version: 0.3.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.2.3/README.md` & `firefly_exchange_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/pyproject.toml` & `firefly_exchange_client-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.2.3"
+version = "0.3.0"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/api_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,18 @@
                 url, 
                 params=query, 
                 headers={'Authorization': 'Bearer {}'.format(self.auth_token)})
         else:
             response = await self.client.get(url, params=query)
 
         try:
-            return await response.json()
+            if response.status != 503: #checking for service unavailitbility 
+                return await response.json()
+            else:
+               return response
         except:
             raise Exception("Error while getting {}: {}".format(url, response))
         
     async def post(self, service_url, data, auth_required=False):
         """
             Makes a POST request and returns the results
             Inputs:
@@ -46,20 +49,23 @@
         url = self._create_url(service_url)
         response = None
 
         if auth_required:
             response = await self.client.post(
                 url=url, 
                 data=data, 
-                headers={'Authorization': 'Bearer {}'.format(self.auth_token)})
+                headers={'Authorization': 'Bearer {}'.format(self.auth_token),'Content-type': 'application/json'})
         else:
             response = await self.client.post(url=url, data=data)
 
         try:
-            return await response.json()
+            if response.status != 503: #checking for service unavailitbility 
+                return await response.json()
+            else:
+               return response
         except:
             raise Exception("Error while posting to {}: {}".format(url, response))
         
     async def delete(self,service_url, data, auth_required=False):
         """
             Makes a DELETE request and returns the results
             Inputs:
```

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from .api_service import APIService
 from .contracts import Contracts
 from .order_signer import OrderSigner
 from .onboarding_signer import OnboardingSigner
 from .utilities import *
 from .constants import TIME, SERVICE_URLS
 from .interfaces import *
@@ -15,14 +16,15 @@
 class FireflyClient:
     def __init__(self, are_terms_accepted, network, private_key):
         self.are_terms_accepted = are_terms_accepted
         self.network = network
         self.w3 = self._connect_w3(self.network["url"])
         self.account = Account.from_key(private_key)
         self.apis = APIService(self.network["apiGateway"])
+        self.dmsApi = APIService(self.network["dmsURL"])
         self.socket = Sockets(self.network["socketURL"])
         self.webSocketClient = WebsocketClient(self.network["webSocketURL"])
         self.contracts = Contracts()
         self.order_signers = {}
         self.onboarding_signer = OnboardingSigner()
         
             
@@ -39,14 +41,15 @@
         # contracts pertaining to markets
         for k, v in self.contracts.contract_addresses.items():
             if 'PERP' in k:
                 self.add_contract(name="Perpetual",address=v["Perpetual"], market=k)
 
         if user_onboarding:
             self.apis.auth_token = await self.onboard_user()
+            self.dmsApi.auth_token = self.apis.auth_token
             self.socket.set_token(self.apis.auth_token)
             self.webSocketClient.set_token(self.apis.auth_token)
 
 
     async def onboard_user(self, token:str=None):
         """
             On boards the user address and returns user authentication token.
@@ -785,14 +788,57 @@
             if symbol.value==i["symbol"]:
                 return int(from_wei(int(i["selectedLeverage"]), "ether"))    
 
         # default leverage on system is 3
         # todo fetch from exchange info route
         return 3
 
+    async def get_cancel_on_disconnect_timer(self, params:GetCancelOnDisconnectTimerRequest=None):
+        """
+            Returns a list of the user's countDowns for provided market symbol,
+            Inputs:
+                - symbol(MARKET_SYMBOLS): (Optional) market symbol to get user market cancel_on_disconnect timer for, not providing it would return all the active countDown timers for each market.  
+                - parentAddress (str):(Optional) Only provided by a sub account
+            Returns:
+                - GetCountDownsResponse:
+                    - countDowns: object with provided market symbol and respective countDown timer
+                    - timestamp
+        """
+        
+        params = extract_enums(params, ["symbol"])
+        response = await self.dmsApi.get(
+            SERVICE_URLS["USER"]["CANCEL_ON_DISCONNECT"],
+            params,
+            auth_required=True
+        )
+        # check for service unavailibility
+        if hasattr(response, 'status') and response.status == 503:
+            raise Exception("Cancel on Disconnect (dead-mans-switch) feature is currently unavailable")
+            
+        return response
+    
+    async def reset_cancel_on_disconnect_timer(self, params:PostTimerAttributes):
+        """
+            Returns PostTimerResponse containing accepted and failed countdowns, and the next page number
+            Inputs:
+                - params(PostTimerAttributes): params required to fetch funding history  
+            Returns:
+                - PostTimerResponse: 
+                    - acceptedToReset: array with symbols for which timer was reset successfully
+                    - failedReset: aray with symbols for whcih timer failed to reset 
+        """
+        response = await self.dmsApi.post(
+            SERVICE_URLS["USER"]["CANCEL_ON_DISCONNECT"],
+            json.dumps(params),
+            auth_required=True   
+        )
+        # check for service unavailibility
+        if hasattr(response, 'status') and response.status == 503:
+             raise Exception("Cancel on Disconnect (dead-mans-switch) feature is currently unavailable")
+        return response
        
     ## Internal methods
     def _get_order_signer(self,symbol:MARKET_SYMBOLS=None):
         """
             Returns the order signer for the specified symbol, else returns a dictionary of symbol -> order signer
             Inputs:
                 - symbol(MARKET_SYMBOLS): the symbol to get order signer for, optional
```

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "onboardingUrl": "https://dev.firefly.exchange",
   },
 
   "TESTNET_ARBITRUM": {
     "url": "https://goerli-rollup.arbitrum.io/rpc",
     "chainId": 421613,
     "apiGateway": "https://dapi.api.arbitrum-staging.firefly.exchange",
+    "dmsURL": "https://api.arbitrum-staging.firefly.exchange/dead-man-switch",
     "socketURL": "wss://dapi.api.arbitrum-staging.firefly.exchange",
     "webSocketURL": "wss://notifications.api.arbitrum-staging.firefly.exchange",
     "onboardingUrl": "https://testnet.firefly.exchange",
   },
 
   "MAINNET_BOBA": {
     "url": "https://bobabeam.boba.network/",
@@ -23,14 +24,15 @@
     "socketURL": "wss://dapi.firefly.exchange",
     "onboardingUrl": "https://trade.firefly.exchange",
   },
   "MAINNET_ARBITRUM": {
     "url": "https://arb1.arbitrum.io/rpc/",
     "chainId": 42161,
     "apiGateway": "https://dapi.api.arbitrum-prod.firefly.exchange",
+    "dmsURL": "https://api.arbitrum-prod.firefly.exchange/dead-man-switch",
     "socketURL": "wss://dapi.api.arbitrum-prod.firefly.exchange",
     "webSocketURL": "wss://notifications.api.arbitrum-prod.firefly.exchange",
     "onboardingUrl": "https://trade-arb.firefly.exchange",
   },
 }
 
 
@@ -85,14 +87,15 @@
     "ORDERS": "/orders",
     "ACCOUNT": "/account",
     "USER_TRANSACTION_HISTORY": "/userTransactionHistory",
     "AUTHORIZE": "/authorize",
     "ADJUST_LEVERAGE": "/account/adjustLeverage",
     "FUND_GAS": "/account/fundGas",
     "FUNDING_HISTORY": "/userFundingHistory",
+    "CANCEL_ON_DISCONNECT": "/dms-countdown"
   },
   "ORDERS": {
     "ORDERS": "/orders",
     "ORDERS_HASH": "/orders/hash",
   },
 }
```

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,8 +161,31 @@
   side: ORDER_SIDE # BUY/SELL
   blockNumber: int # transaction block number
   isPositionPositive: bool # is position LONG or SHORT
 
 class GetFundingHistoryResponse(TypedDict):
   isMoreDataAvailable: bool # boolean indicating if there is more data available
   nextCursor: int # next page number
-  data: List[FundingHistoryResponse]
+  data: List[FundingHistoryResponse]
+
+class CountDown(TypedDict):
+  symbol: str
+  count: int
+class GetCancelOnDisconnectTimerRequest(TypedDict):
+  symbol: MARKET_SYMBOLS  # will fetch Cancel On Disconnect Timer of provided market
+  parentAddress: str # (optional) should be provided by a sub account 
+
+class PostTimerAttributes(TypedDict):
+  countDowns: List[CountDown]
+  parentAddress: str 
+
+class FailedCountDownResetResponse(TypedDict):
+  symbol: str
+  reason: str
+
+class PostTimerResponse(TypedDict):
+  acceptedToReset: List[str]
+  failedReset: List[FailedCountDownResetResponse]
+
+
+
+
```

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/sockets.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly-exchange-client
-Version: 0.2.3
+Version: 0.3.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.3.0/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

