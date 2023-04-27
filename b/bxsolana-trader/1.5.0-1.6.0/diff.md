# Comparing `tmp/bxsolana-trader-1.5.0.tar.gz` & `tmp/bxsolana-trader-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxsolana-trader-1.5.0.tar", last modified: Tue Mar 14 21:55:23 2023, max compression
+gzip compressed data, was "bxsolana-trader-1.6.0.tar", last modified: Thu Apr 27 20:19:29 2023, max compression
```

## Comparing `bxsolana-trader-1.5.0.tar` & `bxsolana-trader-1.6.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.588193 bxsolana-trader-1.5.0/
--rw-r--r--   0 aspin      (501) staff       (20)     1071 2022-09-13 19:43:40.000000 bxsolana-trader-1.5.0/LICENSE
--rw-r--r--   0 aspin      (501) staff       (20)     4400 2023-03-14 21:55:23.588273 bxsolana-trader-1.5.0/PKG-INFO
--rw-r--r--   0 aspin      (501) staff       (20)     2919 2023-02-20 23:04:33.000000 bxsolana-trader-1.5.0/README.md
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.576603 bxsolana-trader-1.5.0/bxsolana/
--rw-r--r--   0 aspin      (501) staff       (20)      280 2023-01-10 20:47:33.000000 bxsolana-trader-1.5.0/bxsolana/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.579387 bxsolana-trader-1.5.0/bxsolana/examples/
--rw-r--r--   0 aspin      (501) staff       (20)      672 2023-01-10 20:47:33.000000 bxsolana-trader-1.5.0/bxsolana/examples/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)      617 2023-02-21 21:35:54.000000 bxsolana-trader-1.5.0/bxsolana/examples/constants.py
--rw-r--r--   0 aspin      (501) staff       (20)     2638 2022-12-21 21:25:04.000000 bxsolana-trader-1.5.0/bxsolana/examples/order_lifecycle.py
--rw-r--r--   0 aspin      (501) staff       (20)     6862 2023-01-10 20:47:33.000000 bxsolana-trader-1.5.0/bxsolana/examples/order_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)    11562 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/examples/request_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)     3002 2023-03-14 19:51:28.000000 bxsolana-trader-1.5.0/bxsolana/examples/stream_utils.py
--rw-r--r--   0 aspin      (501) staff       (20)     5638 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/examples/transaction_request_utils.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.581744 bxsolana-trader-1.5.0/bxsolana/provider/
--rw-r--r--   0 aspin      (501) staff       (20)      582 2022-10-10 22:32:15.000000 bxsolana-trader-1.5.0/bxsolana/provider/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)    10174 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/provider/base.py
--rw-r--r--   0 aspin      (501) staff       (20)      970 2023-02-20 23:04:33.000000 bxsolana-trader-1.5.0/bxsolana/provider/constants.py
--rw-r--r--   0 aspin      (501) staff       (20)     2946 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/provider/grpc.py
--rw-r--r--   0 aspin      (501) staff       (20)    26895 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/provider/http.py
--rw-r--r--   0 aspin      (501) staff       (20)      947 2023-03-06 23:02:29.000000 bxsolana-trader-1.5.0/bxsolana/provider/http_error.py
--rw-r--r--   0 aspin      (501) staff       (20)     3888 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/provider/ws.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.582736 bxsolana-trader-1.5.0/bxsolana/transaction/
--rw-r--r--   0 aspin      (501) staff       (20)      593 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/bxsolana/transaction/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     2361 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/transaction/memo.py
--rw-r--r--   0 aspin      (501) staff       (20)     2402 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/bxsolana/transaction/signing.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.583546 bxsolana-trader-1.5.0/bxsolana_trader.egg-info/
--rw-r--r--   0 aspin      (501) staff       (20)     4400 2023-03-14 21:55:23.000000 bxsolana-trader-1.5.0/bxsolana_trader.egg-info/PKG-INFO
--rw-r--r--   0 aspin      (501) staff       (20)     1138 2023-03-14 21:55:23.000000 bxsolana-trader-1.5.0/bxsolana_trader.egg-info/SOURCES.txt
--rw-r--r--   0 aspin      (501) staff       (20)        1 2023-03-14 21:55:23.000000 bxsolana-trader-1.5.0/bxsolana_trader.egg-info/dependency_links.txt
--rw-r--r--   0 aspin      (501) staff       (20)      174 2023-03-14 21:55:23.000000 bxsolana-trader-1.5.0/bxsolana_trader.egg-info/requires.txt
--rw-r--r--   0 aspin      (501) staff       (20)       14 2023-03-14 21:55:23.000000 bxsolana-trader-1.5.0/bxsolana_trader.egg-info/top_level.txt
--rw-r--r--   0 aspin      (501) staff       (20)      217 2022-09-07 21:30:01.000000 bxsolana-trader-1.5.0/pyproject.toml
--rw-r--r--   0 aspin      (501) staff       (20)      707 2023-03-14 21:55:23.590719 bxsolana-trader-1.5.0/setup.cfg
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.585433 bxsolana-trader-1.5.0/test/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.587327 bxsolana-trader-1.5.0/test/integration/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/integration/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     4020 2023-02-20 23:04:33.000000 bxsolana-trader-1.5.0/test/integration/private.py
--rw-r--r--   0 aspin      (501) staff       (20)     2192 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/integration/public.py
--rw-r--r--   0 aspin      (501) staff       (20)      852 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/integration/stream.py
--rw-r--r--   0 aspin      (501) staff       (20)      701 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/integration/test_grpc.py
--rw-r--r--   0 aspin      (501) staff       (20)      544 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/integration/test_http.py
--rw-r--r--   0 aspin      (501) staff       (20)      664 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/integration/test_ws.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.587525 bxsolana-trader-1.5.0/test/unit/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/unit/__init__.py
-drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-03-14 21:55:23.588031 bxsolana-trader-1.5.0/test/unit/transaction/
--rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.5.0/test/unit/transaction/__init__.py
--rw-r--r--   0 aspin      (501) staff       (20)     1386 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/test/unit/transaction/test_memo.py
--rw-r--r--   0 aspin      (501) staff       (20)     4629 2023-03-14 21:50:18.000000 bxsolana-trader-1.5.0/test/unit/transaction/test_signing.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838762 bxsolana-trader-1.6.0/
+-rw-r--r--   0 aspin      (501) staff       (20)     1071 2022-09-13 19:43:40.000000 bxsolana-trader-1.6.0/LICENSE
+-rw-r--r--   0 aspin      (501) staff       (20)     4346 2023-04-27 20:19:29.838836 bxsolana-trader-1.6.0/PKG-INFO
+-rw-r--r--   0 aspin      (501) staff       (20)     2865 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/README.md
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.830409 bxsolana-trader-1.6.0/bxsolana/
+-rw-r--r--   0 aspin      (501) staff       (20)      280 2023-01-10 20:47:33.000000 bxsolana-trader-1.6.0/bxsolana/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.832968 bxsolana-trader-1.6.0/bxsolana/examples/
+-rw-r--r--   0 aspin      (501) staff       (20)      672 2023-01-10 20:47:33.000000 bxsolana-trader-1.6.0/bxsolana/examples/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)      617 2023-02-21 21:35:54.000000 bxsolana-trader-1.6.0/bxsolana/examples/constants.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2638 2022-12-21 21:25:04.000000 bxsolana-trader-1.6.0/bxsolana/examples/order_lifecycle.py
+-rw-r--r--   0 aspin      (501) staff       (20)     6862 2023-01-10 20:47:33.000000 bxsolana-trader-1.6.0/bxsolana/examples/order_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)    13092 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/bxsolana/examples/request_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)     3501 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/bxsolana/examples/stream_utils.py
+-rw-r--r--   0 aspin      (501) staff       (20)     5638 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/examples/transaction_request_utils.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.834972 bxsolana-trader-1.6.0/bxsolana/provider/
+-rw-r--r--   0 aspin      (501) staff       (20)      582 2022-10-10 22:32:15.000000 bxsolana-trader-1.6.0/bxsolana/provider/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)    10174 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/provider/base.py
+-rw-r--r--   0 aspin      (501) staff       (20)      970 2023-02-20 23:04:33.000000 bxsolana-trader-1.6.0/bxsolana/provider/constants.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2946 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/provider/grpc.py
+-rw-r--r--   0 aspin      (501) staff       (20)    28223 2023-04-24 22:32:24.000000 bxsolana-trader-1.6.0/bxsolana/provider/http.py
+-rw-r--r--   0 aspin      (501) staff       (20)      947 2023-03-06 23:02:29.000000 bxsolana-trader-1.6.0/bxsolana/provider/http_error.py
+-rw-r--r--   0 aspin      (501) staff       (20)     3888 2023-04-27 20:19:19.000000 bxsolana-trader-1.6.0/bxsolana/provider/ws.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.835884 bxsolana-trader-1.6.0/bxsolana/transaction/
+-rw-r--r--   0 aspin      (501) staff       (20)      593 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/bxsolana/transaction/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2361 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/transaction/memo.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2402 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/bxsolana/transaction/signing.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.836631 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/
+-rw-r--r--   0 aspin      (501) staff       (20)     4346 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/PKG-INFO
+-rw-r--r--   0 aspin      (501) staff       (20)     1138 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 aspin      (501) staff       (20)        1 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 aspin      (501) staff       (20)      174 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/requires.txt
+-rw-r--r--   0 aspin      (501) staff       (20)       14 2023-04-27 20:19:29.000000 bxsolana-trader-1.6.0/bxsolana_trader.egg-info/top_level.txt
+-rw-r--r--   0 aspin      (501) staff       (20)      217 2022-09-07 21:30:01.000000 bxsolana-trader-1.6.0/pyproject.toml
+-rw-r--r--   0 aspin      (501) staff       (20)      707 2023-04-27 20:19:29.839160 bxsolana-trader-1.6.0/setup.cfg
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.836753 bxsolana-trader-1.6.0/test/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838067 bxsolana-trader-1.6.0/test/integration/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4020 2023-02-20 23:04:33.000000 bxsolana-trader-1.6.0/test/integration/private.py
+-rw-r--r--   0 aspin      (501) staff       (20)     2192 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/public.py
+-rw-r--r--   0 aspin      (501) staff       (20)      852 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/stream.py
+-rw-r--r--   0 aspin      (501) staff       (20)      701 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/test_grpc.py
+-rw-r--r--   0 aspin      (501) staff       (20)      544 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/test_http.py
+-rw-r--r--   0 aspin      (501) staff       (20)      664 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/integration/test_ws.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838259 bxsolana-trader-1.6.0/test/unit/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/unit/__init__.py
+drwxr-xr-x   0 aspin      (501) staff       (20)        0 2023-04-27 20:19:29.838626 bxsolana-trader-1.6.0/test/unit/transaction/
+-rw-r--r--   0 aspin      (501) staff       (20)        0 2022-11-15 23:10:06.000000 bxsolana-trader-1.6.0/test/unit/transaction/__init__.py
+-rw-r--r--   0 aspin      (501) staff       (20)     1386 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/test/unit/transaction/test_memo.py
+-rw-r--r--   0 aspin      (501) staff       (20)     4629 2023-03-14 21:50:18.000000 bxsolana-trader-1.6.0/test/unit/transaction/test_signing.py
```

### Comparing `bxsolana-trader-1.5.0/LICENSE` & `bxsolana-trader-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/PKG-INFO` & `bxsolana-trader-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -113,21 +113,14 @@
 $ pip install -r requirements.txt
 ```
 
 Run tests:
 
 ```
 $ make test
-```
-
-Regenerate protobuf files:
-
-```
-$ make proto
-```
 
 Linting:
 ```
 $ make lint
 ```
 
 MIT License
```

### Comparing `bxsolana-trader-1.5.0/README.md` & `bxsolana-trader-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -101,19 +101,12 @@
 $ pip install -r requirements.txt
 ```
 
 Run tests:
 
 ```
 $ make test
-```
-
-Regenerate protobuf files:
-
-```
-$ make proto
-```
 
 Linting:
 ```
 $ make lint
 ```
```

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/__init__.py` & `bxsolana-trader-1.6.0/bxsolana/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/constants.py` & `bxsolana-trader-1.6.0/bxsolana/examples/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/order_lifecycle.py` & `bxsolana-trader-1.6.0/bxsolana/examples/order_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/order_utils.py` & `bxsolana-trader-1.6.0/bxsolana/examples/order_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/request_utils.py` & `bxsolana-trader-1.6.0/bxsolana/examples/request_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from bxsolana_trader_proto import api as proto
 from bxsolana_trader_proto.common import OrderType
+from bxsolana_trader_proto.common import PerpPositionSide
+from bxsolana_trader_proto.common import PerpOrderType
 from bxsolana_trader_proto.common import PerpContract
 from bxsolana_trader_proto.common import PerpCollateralType
 from bxsolana_trader_proto.common import PerpCollateralToken
 
 from .. import provider
 
 
@@ -241,42 +243,66 @@
                 owner_address=public_key,
                 steps=[step],
             )
         ).to_json()
     )
 
     # DRIFT
+    print("get user")
+    print(
+        (
+            await api.get_user(
+                project=proto.Project.P_DRIFT,
+                owner_address=public_key,
+            )
+        ).to_json()
+    )
 
-    # endpoint disabled in v1.6.5
-    # print("get Drift orderbook")
-    # print(
-    #     (
-    #         await api.get_perp_orderbook(
-    #             market="SOL-PERP", project=proto.Project.P_DRIFT
-    #         )
-    #     ).to_json()
-    # )
+    print("get Drift orderbook")
+    print(
+        (
+            await api.get_perp_orderbook(
+                contract=PerpContract.SOL_PERP, project=proto.Project.P_DRIFT
+            )
+        ).to_json()
+    )
+
+    print("post perp order")
+    print(
+        (
+            await api.post_perp_order(
+                project=proto.Project.P_DRIFT,
+                owner_address=public_key,
+                payer_address=public_key,
+                contract=PerpContract.SOL_PERP,
+                position_side=PerpPositionSide.PS_LONG,
+                slippage=0,
+                type=PerpOrderType.POT_LIMIT,
+                amount=0,
+                price=12000,
+                client_order_i_d=12,
+            )
+        ).to_json()
+    )
 
     print("get perp contracts")
     print(
         (
             await api.get_perp_contracts(
                 project=proto.Project.P_DRIFT,
-                contracts=[PerpContract.SOL_PERP, PerpContract.BTC_PERP],
             )
         ).to_json()
     )
 
     print("get perp assets")
     print(
         (
             await api.get_assets(
                 owner_address=public_key,
                 project=proto.Project.P_DRIFT,
-                contract=PerpContract.SOL_PERP,
             )
         ).to_json()
     )
 
     print("get open perp order")
     print(
         (
@@ -302,40 +328,46 @@
 
     print("post liquidate perp")
     print(
         (
             await api.post_liquidate_perp(
                 project=proto.Project.P_DRIFT,
                 owner_address=public_key,
-                settlee_account_address=public_key,
+                settlee_account_address=(
+                    "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                ),
                 contract=PerpContract.SOL_PERP,
                 amount=1,
             )
         ).to_json()
     )
 
     print("post settle pnl")
     print(
         (
             await api.post_settle_p_n_l(
                 project=proto.Project.P_DRIFT,
                 owner_address=public_key,
-                settlee_account_address=public_key,
+                settlee_account_address=(
+                    "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                ),
                 contract=PerpContract.SOL_PERP,
             )
         ).to_json()
     )
 
     print("post settle pnls")
     print(
         (
             await api.post_settle_p_n_ls(
                 project=proto.Project.P_DRIFT,
                 owner_address=public_key,
-                settlee_account_addresses=[public_key],
+                settlee_account_addresses=[
+                    "9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS"
+                ],
                 contract=PerpContract.SOL_PERP,
             )
         ).to_json()
     )
 
     print("post cancel perp order")
     print(
@@ -346,73 +378,88 @@
                 client_order_i_d=12,
                 order_i_d=0,
                 contract=PerpContract.SOL_PERP,
             )
         ).to_json()
     )
 
-    print("post cancel perp orders")
+    print("post close perp orders")
     print(
         (
-            await api.post_cancel_perp_orders(
+            await api.post_close_perp_positions(
                 project=proto.Project.P_DRIFT,
-                contract=PerpContract.SOL_PERP,
                 owner_address=public_key,
+                contracts=[PerpContract.SOL_PERP],
             )
         ).to_json()
     )
 
-    print("post create users")
+    print("post cancel perp orders")
     print(
         (
-            await api.post_create_user(
+            await api.post_cancel_perp_orders(
                 project=proto.Project.P_DRIFT,
-                owner_address="BgJ8uyf9yhLJaUVESRrqffzwVyQgRi9YvWmpEFaH14kx",
+                contract=PerpContract.SOL_PERP,
+                owner_address=public_key,
             )
         ).to_json()
     )
 
-    print("get user")
+    print("post create user")
     print(
         (
-            await api.get_user(
+            await api.post_create_user(
                 project=proto.Project.P_DRIFT,
-                owner_address=public_key,
+                owner_address="BgJ8uyf9yhLJaUVESRrqffzwVyQgRi9YvWmpEFaH14kx",
             )
         ).to_json()
     )
 
     print("post deposit collateral")
     print(
         (
             await api.post_manage_collateral(
                 project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                account_address="",
+                account_address="9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS",
                 amount=0.1,
                 token=PerpCollateralToken.PCTK_USDC,
                 type=PerpCollateralType.PCT_DEPOSIT,
             )
         ).to_json()
     )
 
     print("post withdraw collateral")
     print(
         (
             await api.post_manage_collateral(
                 project=proto.Project.P_DRIFT,
-                owner_address=public_key,
-                account_address="",
+                account_address="9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS",
                 amount=0.1,
                 token=PerpCollateralToken.PCTK_SOL,
                 type=PerpCollateralType.PCT_WITHDRAWAL,
             )
         ).to_json()
     )
 
+    print("post transfer collateral")
+    print(
+        (
+            await api.post_manage_collateral(
+                project=proto.Project.P_DRIFT,
+                account_address="9UnwdvTf5EfGeLyLrF4GZDUs7LKRUeJQzW7qsDVGQ8sS",
+                amount=0.1,
+                token=PerpCollateralToken.PCTK_SOL,
+                type=PerpCollateralType.PCT_TRANSFER,
+                to_account_address=(
+                    "AbnwAQGrYnvktT4ihhX5np8RbgtfXJfPwpgMJnCFa4MT"
+                ),
+            )
+        ).to_json()
+    )
+
     print("get perp positions")
     print(
         (
             await api.get_perp_positions(
                 project=proto.Project.P_DRIFT,
                 owner_address=public_key,
                 contracts=[PerpContract.SOL_PERP],
```

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/stream_utils.py` & `bxsolana-trader-1.6.0/bxsolana/examples/stream_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from bxsolana_trader_proto import api as proto
+from bxsolana_trader_proto.common import PerpContract
 
 from .. import provider
 
 
 async def do_stream(api: provider.Provider, run_slow: bool = False):
     item_count = 0
 
@@ -65,33 +66,45 @@
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 1:
                 item_count = 0
                 break
 
-    print("streaming price streams...")
-    async for response in api.get_prices_stream(
-        projects=[proto.Project.P_RAYDIUM],
-        tokens=[
-            "So11111111111111111111111111111111111111112",
-            "USDC",
-            "SOL",
-            "USDT",
-        ],
-    ):
-        print(response.to_json())
-        item_count += 1
-        if item_count == 1:
-            item_count = 0
-            break
+    if run_slow:
+        print("streaming price streams...")
+        async for response in api.get_prices_stream(
+            projects=[proto.Project.P_RAYDIUM],
+            tokens=[
+                "So11111111111111111111111111111111111111112",
+                "USDC",
+                "SOL",
+                "USDT",
+            ],
+        ):
+            print(response.to_json())
+            item_count += 1
+            if item_count == 1:
+                item_count = 0
+                break
 
     if run_slow:
         print("streaming Drift orderbook updates...")
         async for response in api.get_perp_orderbooks_stream(
-            markets=["SOL-PERP"], project=proto.Project.P_DRIFT
+            contracts=[PerpContract.ALL], project=proto.Project.P_DRIFT
         ):
             print(response.to_json())
             item_count += 1
             if item_count == 5:
                 item_count = 0
                 break
+
+    if run_slow:
+        print("streaming Drift trade updates...")
+        async for response in api.get_perp_trades_stream(
+            contracts=[PerpContract.ALL], project=proto.Project.P_DRIFT
+        ):
+            print(response.to_json())
+            item_count += 1
+            if item_count == 1:
+                item_count = 0
+                break
```

### Comparing `bxsolana-trader-1.5.0/bxsolana/examples/transaction_request_utils.py` & `bxsolana-trader-1.6.0/bxsolana/examples/transaction_request_utils.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/__init__.py` & `bxsolana-trader-1.6.0/bxsolana/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/base.py` & `bxsolana-trader-1.6.0/bxsolana/provider/base.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/constants.py` & `bxsolana-trader-1.6.0/bxsolana/provider/constants.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/grpc.py` & `bxsolana-trader-1.6.0/bxsolana/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/http.py` & `bxsolana-trader-1.6.0/bxsolana/provider/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 from bxsolana_trader_proto import api as proto
 from .. import transaction
 from . import constants
 from .base import Provider
 from .http_error import map_response
 from bxsolana_trader_proto.common import (
+    PerpPositionSide,
+    PostOnlyParams,
+    PerpOrderType,
     PerpContract,
     PerpCollateralType,
     PerpCollateralToken,
 )
 
 if TYPE_CHECKING:
     # noinspection PyUnresolvedReferences,PyProtectedMember
@@ -214,17 +217,15 @@
             f"{self._endpoint}/account/token-accounts?ownerAddress={owner_address}"
         ) as res:
             return await map_response(res, proto.GetTokenAccountsResponse())
 
     async def get_pools(
         self, projects: List["proto.Project"] = []
     ) -> proto.GetPoolsResponse:
-        params = (
-            "?" + serialize_projects(projects)
-        )
+        params = "?" + serialize_projects(projects)
 
         async with self._session.get(
             f"{self._endpoint}/market/pools{params}"
         ) as res:
             return await map_response(res, proto.GetPoolsResponse())
 
     async def get_price(self, tokens: List[str] = []) -> proto.GetPriceResponse:
@@ -239,20 +240,20 @@
             f"{self._endpoint}/system/blockhash"
         ) as res:
             return await map_response(res, proto.GetRecentBlockHashResponse())
 
     async def get_perp_orderbook(
         self,
         *,
-        market: str = "",
+        contract: PerpContract = PerpContract.ALL,
         limit: int = 0,
         project: proto.Project = proto.Project.P_UNKNOWN,
     ) -> proto.GetPerpOrderbookResponse:
         async with self._session.get(
-            f"{self._endpoint}/market/perp/orderbook/{market}?limit={limit}&project={project.name}"
+            f"{self._endpoint}/market/perp/orderbook/{contract}?limit={limit}&project={project.name}"
         ) as res:
             return await map_response(res, proto.GetPerpOrderbookResponse())
 
     async def post_settle_p_n_l(
         self,
         *,
         owner_address: str = "",
@@ -312,38 +313,67 @@
             return await map_response(res, proto.PostLiquidatePerpResponse())
 
     async def get_assets(
         self,
         *,
         owner_address: str = "",
         account_address: str = "",
-        contract: PerpContract = PerpContract.ALL,
         project: proto.Project = proto.Project.P_DRIFT,
     ) -> proto.GetAssetsResponse:
         async with self._session.get(
             f"{self._endpoint}/trade/perp/assets?ownerAddress={owner_address}&accountAddress={account_address}"
-            f"&project={project.name}&contract={contract.name}"
+            f"&project={project.name}"
         ) as res:
             return await map_response(res, proto.GetAssetsResponse())
 
     async def get_perp_contracts(
         self,
         *,
         project: proto.Project = proto.Project.P_DRIFT,
         contracts: List[PerpContract] = [],
     ) -> proto.GetPerpContractsResponse:
-        params = ""
-        for i in range(len(contracts)):
-            params += "&contracts=" + str(contracts[i].name)
-
         async with self._session.get(
-            f"{self._endpoint}/trade/perp/contracts?project={project.name}{params}"
+            f"{self._endpoint}/market/perp/contracts?project={project.name}"
         ) as res:
             return await map_response(res, proto.GetPerpContractsResponse())
 
+    async def post_perp_order(
+        self,
+        *,
+        project: proto.Project = proto.Project.P_DRIFT,
+        owner_address: str = "",
+        payer_address: str = "",
+        contract: PerpContract = PerpContract.SOL_PERP,
+        account_address: str = "",
+        position_side: PerpPositionSide = PerpPositionSide.PS_LONG,
+        slippage: float = 0,
+        type: PerpOrderType = PerpOrderType.POT_LIMIT,
+        amount: float = 0,
+        price: float = 0,
+        client_order_i_d: int = 0,
+        post_only: PostOnlyParams = PostOnlyParams.PO_NONE,
+    ) -> proto.PostPerpOrderResponse:
+        request = proto.PostPerpOrderRequest()
+        request.payer_address = payer_address
+        request.position_side = position_side
+        request.slippage = slippage
+        request.type = type
+        request.amount = amount
+        request.price = price
+        request.client_order_i_d = client_order_i_d
+        request.contract = contract
+        request.project = project
+        request.owner_address = owner_address
+        request.account_address = account_address
+
+        async with self._session.post(
+            f"{self._endpoint}/trade/perp/order", json=request.to_dict()
+        ) as res:
+            return await map_response(res, proto.PostPerpOrderResponse())
+
     async def get_open_perp_order(
         self,
         *,
         owner_address: str = "",
         account_address: str = "",
         project: proto.Project = proto.Project.P_DRIFT,
         contract: PerpContract = PerpContract.ALL,
@@ -416,21 +446,23 @@
         ) as res:
             return await map_response(res, proto.PostCancelPerpOrdersResponse())
 
     async def post_close_perp_positions(
         self,
         *,
         owner_address: str = "",
+        account_address: str = "",
         project: proto.Project = proto.Project.P_DRIFT,
         contracts: List[PerpContract] = [],
     ) -> proto.PostClosePerpPositionsResponse:
         request = proto.PostClosePerpPositionsRequest()
         request.contracts = contracts
         request.project = project
         request.owner_address = owner_address
+        request.account_address = account_address
 
         async with self._session.post(
             f"{self._endpoint}/trade/perp/close", json=request.to_dict()
         ) as res:
             return await map_response(
                 res, proto.PostClosePerpPositionsResponse()
             )
@@ -449,35 +481,36 @@
         ) as res:
             return await map_response(res, proto.PostCreateUserResponse())
 
     async def get_user(
         self,
         *,
         owner_address: str = "",
+        account_address: str = "",
         project: proto.Project = proto.Project.P_DRIFT,
     ) -> proto.GetUserResponse:
         async with self._session.get(
-            f"{self._endpoint}/trade/user?ownerAddress={owner_address}&&project={project.name}"
+            f"{self._endpoint}/trade/user?ownerAddress={owner_address}&project={project.name}&accountAddress={account_address}"
         ) as res:
-            return await map_response(res, proto.GetPerpOrderbookResponse())
+            return await map_response(res, proto.GetUserResponse())
 
     async def post_manage_collateral(
         self,
         *,
-        owner_address: str = "",
         account_address: str = "",
         amount: float = 0,
         project: proto.Project = proto.Project.P_DRIFT,
         type: PerpCollateralType = PerpCollateralType.PCT_DEPOSIT,
         token: PerpCollateralToken = PerpCollateralToken.PCTK_USDC,
+        to_account_address: str = "",
     ) -> proto.PostManageCollateralResponse:
         request = proto.PostManageCollateralRequest()
         request.project = project
-        request.owner_address = owner_address
         request.account_address = account_address
+        request.to_account_address = to_account_address
         request.amount = amount
         request.type = type
         request.token = token
         async with self._session.post(
             f"{self._endpoint}/trade/perp/managecollateral",
             json=request.to_dict(),
         ) as res:
@@ -749,19 +782,19 @@
             "streaming is not implemented in HTTP provider"
         )
 
         # useless line to turn function into a generator
         yield response_type()
 
 
-def serialize_list(key: str, l: List[Any]) -> str:
+def serialize_list(key: str, values: List[Any]) -> str:
     parts = []
-    for i, v in enumerate(l):
+    for i, v in enumerate(values):
         parts.append(f"{key}={v}")
-        if i != len(l) - 1:
+        if i != len(values) - 1:
             parts.append("&")
     return "".join(parts)
 
 
 def serialize_projects(projects: List[proto.Project]) -> str:
     return serialize_list("projects", [project.name for project in projects])
```

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/http_error.py` & `bxsolana-trader-1.6.0/bxsolana/provider/http_error.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/provider/ws.py` & `bxsolana-trader-1.6.0/bxsolana/provider/ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/transaction/__init__.py` & `bxsolana-trader-1.6.0/bxsolana/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/transaction/memo.py` & `bxsolana-trader-1.6.0/bxsolana/transaction/memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana/transaction/signing.py` & `bxsolana-trader-1.6.0/bxsolana/transaction/signing.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/bxsolana_trader.egg-info/PKG-INFO` & `bxsolana-trader-1.6.0/bxsolana_trader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxsolana-trader
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python SDK for bloXroute's Solana Trader API
 Home-page: https://github.com/bloXroute-Labs/solana-trader-client-python
 Author: bloXroute Labs
 Author-email: support@bloxroute.com
 Keywords: serum,solana,blockchain,trader,grpc,stream
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -113,21 +113,14 @@
 $ pip install -r requirements.txt
 ```
 
 Run tests:
 
 ```
 $ make test
-```
-
-Regenerate protobuf files:
-
-```
-$ make proto
-```
 
 Linting:
 ```
 $ make lint
 ```
 
 MIT License
```

### Comparing `bxsolana-trader-1.5.0/bxsolana_trader.egg-info/SOURCES.txt` & `bxsolana-trader-1.6.0/bxsolana_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/setup.cfg` & `bxsolana-trader-1.6.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bxsolana-trader
-version = 1.5.0
+version = 1.6.0
 description = Python SDK for bloXroute's Solana Trader API
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = bloXroute Labs
 author_email = support@bloxroute.com
 url = https://github.com/bloXroute-Labs/solana-trader-client-python
 keywords = serum, solana, blockchain, trader, grpc, stream
@@ -17,13 +17,13 @@
 	betterproto[compiler]==1.2.5
 	grpclib==0.4.3
 	aiounittest==1.4.1
 	base58==2.1.1
 	solana==0.29.1
 	solders==0.14.4
 	bx-jsonrpc-py==0.2.0
-	bxsolana-trader-proto==0.0.11
+	bxsolana-trader-proto==0.0.18
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `bxsolana-trader-1.5.0/test/integration/private.py` & `bxsolana-trader-1.6.0/test/integration/private.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/integration/public.py` & `bxsolana-trader-1.6.0/test/integration/public.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/integration/stream.py` & `bxsolana-trader-1.6.0/test/integration/stream.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/integration/test_grpc.py` & `bxsolana-trader-1.6.0/test/integration/test_grpc.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/integration/test_http.py` & `bxsolana-trader-1.6.0/test/integration/test_http.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/integration/test_ws.py` & `bxsolana-trader-1.6.0/test/integration/test_ws.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/unit/transaction/test_memo.py` & `bxsolana-trader-1.6.0/test/unit/transaction/test_memo.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-1.5.0/test/unit/transaction/test_signing.py` & `bxsolana-trader-1.6.0/test/unit/transaction/test_signing.py`

 * *Files identical despite different names*

