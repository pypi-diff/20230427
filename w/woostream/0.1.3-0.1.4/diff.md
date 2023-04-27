# Comparing `tmp/woostream-0.1.3.tar.gz` & `tmp/woostream-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woostream-0.1.3.tar", max compression
+gzip compressed data, was "woostream-0.1.4.tar", max compression
```

## Comparing `woostream-0.1.3.tar` & `woostream-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2044 2023-04-27 13:45:40.249556 woostream-0.1.3/README.md
--rw-r--r--   0        0        0      422 2023-04-27 14:38:18.354806 woostream-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6661 2023-04-27 14:36:06.382984 woostream-0.1.3/woostream/__main__.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 woostream-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2044 2023-04-27 13:45:40.249556 woostream-0.1.4/README.md
+-rw-r--r--   0        0        0      422 2023-04-27 14:41:54.991971 woostream-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6659 2023-04-27 14:40:47.658990 woostream-0.1.4/woostream/__main__.py
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 woostream-0.1.4/PKG-INFO
```

### Comparing `woostream-0.1.3/README.md` & `woostream-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `woostream-0.1.3/woostream/__main__.py` & `woostream-0.1.4/woostream/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 endpoint='/v1/client/holding'
             ),
         ])
 
         asyncio.ensure_future(broadcast("\n".join([
             f"Positions:",
             *[
-                f"- {position['symbol']}: {position['holding']} @ ${position['average_open_price']}"
+                f"- {position['symbol']}: {position['holding']} @ {position['average_open_price']}"
                 for position in positions.get('positions', [])
             ],
             f"Balances:",
             *[
                 f"- {asset}: {holding}"
                 for asset, holding in balances.get('holding', {}).items()
             ],
@@ -216,12 +216,12 @@
         async for topic, message in streamer:
             match topic:
                 case 'position':
                     pass
                 case 'executionreport':
                     if message['data']['status'] == 'FILLED':
                         asyncio.ensure_future(broadcast("\n".join([
-                            f"{'Bought' if message['data']['side'] == 'BUY' else 'Sold'} {message['data']['totalExecutedQuantity']} {message['data']['symbol']} @ ${message['data']['avgPrice']}"
+                            f"{'Bought' if message['data']['side'] == 'BUY' else 'Sold'} {message['data']['totalExecutedQuantity']} {message['data']['symbol']} @ {message['data']['avgPrice']}"
                         ])))
 
 if __name__ == '__main__':
     asyncio.run(main())
```

### Comparing `woostream-0.1.3/PKG-INFO` & `woostream-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woostream
-Version: 0.1.3
+Version: 0.1.4
 Summary: Listen to fills & position updates on Woo X
 License: MIT
 Author: waterquarks
 Author-email: waterquarks@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

