# Comparing `tmp/woostream-0.1.6.tar.gz` & `tmp/woostream-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woostream-0.1.6.tar", max compression
+gzip compressed data, was "woostream-0.1.7.tar", max compression
```

## Comparing `woostream-0.1.6.tar` & `woostream-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2044 2023-04-27 13:45:40.249556 woostream-0.1.6/README.md
--rw-r--r--   0        0        0      422 2023-04-27 15:26:13.707547 woostream-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7655 2023-04-27 15:25:36.429349 woostream-0.1.6/woostream/__main__.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 woostream-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2044 2023-04-27 13:45:40.249556 woostream-0.1.7/README.md
+-rw-r--r--   0        0        0      422 2023-04-27 15:30:44.791373 woostream-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7803 2023-04-27 15:30:20.029960 woostream-0.1.7/woostream/__main__.py
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 woostream-0.1.7/PKG-INFO
```

### Comparing `woostream-0.1.6/README.md` & `woostream-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `woostream-0.1.6/woostream/__main__.py` & `woostream-0.1.7/woostream/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,31 +213,35 @@
                 api_secret_key=args.api_secret_key,
                 endpoint='/v1/client/holding'
             ),
         ])
 
         asyncio.ensure_future(broadcast("\n".join([
             f"Positions:",
-            *[
-                f"- {position['symbol']}: {position['holding']} @ {position['average_open_price']}"
-                for position in positions.get('positions', [])
-                if position['holding'] != 0
-            ],
+            *(
+                [
+                    f"- {position['symbol']}: {position['holding']} @ {position['average_open_price']}"
+                    for position in positions.get('positions', [])
+                    if position['holding'] != 0
+                ] or ["(None)"]
+            ),
             f"Balances:",
-            *[
-                f"- {asset}: {round(holding, str(meta['base_tick']).count('0')) if meta['base_tick'] < 1 else holding}"
-                for asset, holding, meta in [
-                    [asset, holding, [
-                        entry for entry in tokens['rows']
-                        if entry['symbol'] == f"SPOT_{asset}_USDT" or (asset == 'USDT' and entry['symbol'] == 'SPOT_USDC_USDT')
-                    ][0]]
-                    for asset, holding in balances.get('holding', {}).items()
-                ]
-                if holding > meta['base_tick']
-            ],
+            *(
+                [
+                    f"- {asset}: {round(holding, str(meta['base_tick']).count('0')) if meta['base_tick'] < 1 else holding}"
+                    for asset, holding, meta in [
+                        [asset, holding, [
+                            entry for entry in tokens['rows']
+                            if entry['symbol'] == f"SPOT_{asset}_USDT" or (asset == 'USDT' and entry['symbol'] == 'SPOT_USDC_USDT')
+                        ][0]]
+                        for asset, holding in balances.get('holding', {}).items()
+                    ]
+                    if holding > meta['base_tick']
+                ] or ["(None)"]
+            ),
         ])))
 
         async for topic, message in streamer:
             match topic:
                 case 'position':
                     pass
                 case 'executionreport':
```

### Comparing `woostream-0.1.6/PKG-INFO` & `woostream-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woostream
-Version: 0.1.6
+Version: 0.1.7
 Summary: Listen to fills & position updates on Woo X
 License: MIT
 Author: waterquarks
 Author-email: waterquarks@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

