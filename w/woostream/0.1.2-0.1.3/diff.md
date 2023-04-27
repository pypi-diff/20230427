# Comparing `tmp/woostream-0.1.2.tar.gz` & `tmp/woostream-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woostream-0.1.2.tar", max compression
+gzip compressed data, was "woostream-0.1.3.tar", max compression
```

## Comparing `woostream-0.1.2.tar` & `woostream-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-04-27 11:05:40.612337 woostream-0.1.2/README.md
--rw-r--r--   0        0        0      422 2023-04-27 12:58:19.984352 woostream-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5249 2023-04-27 12:58:01.819694 woostream-0.1.2/woostream/__main__.py
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 woostream-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2044 2023-04-27 13:45:40.249556 woostream-0.1.3/README.md
+-rw-r--r--   0        0        0      422 2023-04-27 14:38:18.354806 woostream-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6661 2023-04-27 14:36:06.382984 woostream-0.1.3/woostream/__main__.py
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 woostream-0.1.3/PKG-INFO
```

### Comparing `woostream-0.1.2/woostream/__main__.py` & `woostream-0.1.3/woostream/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import time
 import typing
 
 import aiohttp
 import aiostream
 import telegram
 import websockets
+import secrets
 
 ENDPOINTS = {
     'mainnet': {
         'HTTP': 'https://api.woo.org',
         'WS_PUBLIC': 'wss://wss.woo.org/ws/stream/{application_id}',
         'WS_PRIVATE': 'wss://wss.woo.org/v2/ws/private/stream/{application_id}',
     },
@@ -46,20 +47,20 @@
     return (
         hmac.new(key, msg=msg, digestmod=hashlib.sha256)
             .hexdigest()
             .upper()
     )
 
 
-async def position(network: typing.Literal['mainnet', 'testnet'], api_public_key: str, api_secret_key: str):
+async def private_request(network: typing.Literal['mainnet', 'testnet'], api_public_key: str, api_secret_key: str, endpoint: str):
     timestamp = str(int(time.time() * 1000))
 
     async with aiohttp.ClientSession() as session:
         response = await session.get(
-            f"{ENDPOINTS[network]['HTTP']}/v1/positions",
+            f"{ENDPOINTS[network]['HTTP']}{endpoint}",
             headers={
                 'x-api-key': api_public_key,
                 'x-api-signature': signature(timestamp, api_secret_key),
                 'x-api-timestamp': timestamp
             }
         )
 
@@ -74,26 +75,28 @@
 
 
 async def private_stream(network: typing.Literal['mainnet', 'testnet'], application_id: str, api_public_key: str, api_secret_key: str, topic: str):
     async for connection in websockets.connect(ENDPOINTS[network]['WS_PRIVATE'].format(application_id=application_id)):
         try:
             timestamp = str(int(time.time() * 1000))
 
+            tag = secrets.token_urlsafe(8)
+
             await connection.send(json.dumps({
-                'id': 'test',
+                'id': tag,
                 'event': 'auth',
                 'params': {
                     'apikey': api_public_key,
                     'sign': signature(timestamp, api_secret_key),
                     'timestamp': timestamp
                 }
             }))
 
             await connection.send(json.dumps({
-                "id": "test",
+                "id": tag,
                 "topic": topic,
                 "event": "subscribe"
             }))
 
             async def ping():
                 await connection.send(json.dumps({'event': 'ping'}))
 
@@ -101,26 +104,30 @@
                 message = json.loads(raw_message)
 
                 if message.get('event') == 'ping': asyncio.ensure_future(ping())
 
                 if 'data' not in message:
                     continue
 
-                yield message
+                yield topic, message
         except Exception as exception:
             logging.error(exception)
 
 
 async def main():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog='woostream',
+        description='Stream fills & position updates from Woo X'
+    )
 
     parser.add_argument(
         '--network',
         choices=['mainnet', 'testnet'],
-        default='mainnet'
+        default='mainnet',
+        help='mainnet uses x.staging.woo.org, whilst testnet x.woo.org'
     )
 
     parser.add_argument(
         '--application-id',
         type=str,
         required=True
     )
@@ -146,48 +153,75 @@
     parser.add_argument(
         '--telegram-chat-id',
         type=str,
         required='--telegram-token' in sys.argv
     )
 
     parser.add_argument(
-        '--debug-level',
+        '--log-level',
         type=str,
         choices=list(logging._nameToLevel.keys()),
         default=logging._levelToName[logging.INFO]
     )
 
     args = parser.parse_args()
 
     logging.basicConfig(
-        level=logging._nameToLevel[args.debug_level]
+        level=logging._nameToLevel[args.log_level]
     )
 
     async with (
         aiostream.stream.merge(
             private_stream(args.network, args.application_id, args.api_public_key, args.api_secret_key, 'position'),
             private_stream(args.network, args.application_id, args.api_public_key, args.api_secret_key, 'executionreport')
         ).stream() as streamer,
         telegram.Bot(args.telegram_token) if args.telegram_token else contextlib.nullcontext() as bot
     ):
         async def broadcast(message: str):
-            logging.info(message)
+            print(message)
 
             if bot:
                 await bot.send_message(
                     text=message,
                     chat_id=args.telegram_chat_id
                 )
 
-        asyncio.ensure_future(broadcast(
-            await position(
+        positions, balances = await asyncio.gather(*[
+            private_request(
                 network=args.network,
                 api_public_key=args.api_public_key,
-                api_secret_key=args.api_secret_key
-            )
-        ))
-
-        async for message in streamer:
-            asyncio.ensure_future(broadcast(message))
+                api_secret_key=args.api_secret_key,
+                endpoint='/v1/positions'
+            ),
+            private_request(
+                network=args.network,
+                api_public_key=args.api_public_key,
+                api_secret_key=args.api_secret_key,
+                endpoint='/v1/client/holding'
+            ),
+        ])
+
+        asyncio.ensure_future(broadcast("\n".join([
+            f"Positions:",
+            *[
+                f"- {position['symbol']}: {position['holding']} @ ${position['average_open_price']}"
+                for position in positions.get('positions', [])
+            ],
+            f"Balances:",
+            *[
+                f"- {asset}: {holding}"
+                for asset, holding in balances.get('holding', {}).items()
+            ],
+        ])))
+
+        async for topic, message in streamer:
+            match topic:
+                case 'position':
+                    pass
+                case 'executionreport':
+                    if message['data']['status'] == 'FILLED':
+                        asyncio.ensure_future(broadcast("\n".join([
+                            f"{'Bought' if message['data']['side'] == 'BUY' else 'Sold'} {message['data']['totalExecutedQuantity']} {message['data']['symbol']} @ ${message['data']['avgPrice']}"
+                        ])))
 
 if __name__ == '__main__':
     asyncio.run(main())
```

