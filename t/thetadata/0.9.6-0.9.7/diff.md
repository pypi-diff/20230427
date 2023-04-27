# Comparing `tmp/thetadata-0.9.6.tar.gz` & `tmp/thetadata-0.9.7.tar.gz`

## Comparing `thetadata-0.9.6.tar` & `thetadata-0.9.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.6/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.6/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.6/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/reference.md
--rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/quote_1min.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/quote_streaming.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/trade_streaming.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.6/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.6/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.6/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/__init__.py
--rw-r--r--   0        0        0    58526 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/client.py
--rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/exceptions.py
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/py.typed
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/terminal.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.6/LICENSE
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 thetadata-0.9.6/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 thetadata-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.7/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.7/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/reference.md
+-rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/quote_1min.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/quote_streaming.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.7/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.7/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.7/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.7/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/__init__.py
+-rw-r--r--   0        0        0    58685 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/client.py
+-rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/py.typed
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.7/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.7/LICENSE
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 thetadata-0.9.7/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 thetadata-0.9.7/PKG-INFO
```

### Comparing `thetadata-0.9.6/mkdocs.yml` & `thetadata-0.9.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/.github/workflows/main.yml` & `thetadata-0.9.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/.github/workflows/python-publish.yml` & `thetadata-0.9.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/connection_msgs.py` & `thetadata-0.9.7/docs/connection_msgs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/explanation.md` & `thetadata-0.9.7/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/how-to-guides.md` & `thetadata-0.9.7/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/index.md` & `thetadata-0.9.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/logo.png` & `thetadata-0.9.7/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/manipulate_series.py` & `thetadata-0.9.7/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/tutorials.md` & `thetadata-0.9.7/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/cancel_streams.py` & `thetadata-0.9.7/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/eod.py` & `thetadata-0.9.7/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/get_last.py` & `thetadata-0.9.7/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/open_interest_streaming.py` & `thetadata-0.9.7/docs/options/open_interest_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/quote_1min.py` & `thetadata-0.9.7/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/quote_streaming.py` & `thetadata-0.9.7/docs/options/quote_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/quote_tick.py` & `thetadata-0.9.7/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/trade_streaming.py` & `thetadata-0.9.7/docs/options/trade_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/options/trade_streaming_full.py` & `thetadata-0.9.7/docs/options/trade_streaming_full.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/stocks/eod.py` & `thetadata-0.9.7/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/stocks/get_last.py` & `thetadata-0.9.7/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/stocks/quote_1min.py` & `thetadata-0.9.7/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/docs/stocks/quote_tick.py` & `thetadata-0.9.7/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/tests/test_client.py` & `thetadata-0.9.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/tests/test_docs.py` & `thetadata-0.9.7/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/thetadata/client.py` & `thetadata-0.9.7/thetadata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TickBody,
     ListBody,
     parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
-_VERSION = '0.9.6'
+_VERSION = '0.9.7'
 URL_BASE = "http://127.0.0.1:25510/"
 
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
 
@@ -277,14 +277,15 @@
         self.trade = Trade()
         self.ohlcvc = OHLCVC()
         self.quote = Quote()
         self.open_interest = OpenInterest()
         self.contract = Contract()
         self.date = None
 
+
 class ThetaClient:
     """A high-level, blocking client used to fetch market data. Instantiating this class
     runs a java background process, which is responsible for the heavy lifting of market
     data communication. Java 11 or higher is required to use this class."""
 
     def __init__(self, port: int = 11000, timeout: Optional[float] = 60, launch: bool = True, jvm_mem: int = 0,
                  username: str = "default", passwd: str = "default", auto_update: bool = True, use_bundle: bool = True,
@@ -313,14 +314,15 @@
         self._server: Optional[socket.socket] = None  # None while disconnected
         self._stream_server: Optional[socket.socket] = None  # None while disconnected
         self.launch = launch
         self._stream_impl = None
         self._stream_responses = {}
         self._counter_lock = threading.Lock()
         self._stream_req_id = 0
+        self._stream_connected = False
 
         print('If you require API support, feel free to join our discord server! http://discord.thetadata.us')
         if launch:
             terminal.kill_existing_terminal()
             if username == "default" or passwd == "default":
                 print('------------------------------------------------------------------------------------------------')
                 print("You are using the free version of Theta Data. You are currently limited to "
@@ -378,14 +380,15 @@
             except ConnectionError:
                 if i == 14:
                     raise ConnectionError('Unable to connect to the local Theta Terminal Stream process. '
                                           'Try restarting your system.')
                 sleep(1)
         self._stream_server.settimeout(10)
         self._stream_impl = callback
+        self._stream_connected = True
         out = Thread(target=self._recv_stream)
         out.start()
         return out
 
     def close_stream(self):
         self._stream_server.close()
 
@@ -529,15 +532,15 @@
     def _recv_stream(self):
         """from_bytes
           """
         msg = StreamMsg()
         msg.client = self
         parse_int = lambda d: int.from_bytes(d, "big")
         self._stream_server.settimeout(10)
-        while True:
+        while self._stream_connected:
             try:
                 msg.type = StreamMsgType.from_code(parse_int(self._read_stream(1)[:1]))
                 msg.contract.from_bytes(self._read_stream(parse_int(self._read_stream(1)[:1])))
                 if msg.type == StreamMsgType.QUOTE:
                     msg.quote.from_bytes(self._read_stream(44))
                 elif msg.type == StreamMsgType.TRADE:
                     data = self._read_stream(n_bytes=32)
@@ -556,17 +559,18 @@
                     self._stream_responses[msg.req_response_id] = msg.req_response
                 elif msg.type == StreamMsgType.STOP or msg.type == StreamMsgType.START:
                     msg.date = datetime.strptime(str(parse_int(self._read_stream(4))), "%Y%m%d").date()
                 elif msg.type == StreamMsgType.DISCONNECTED or msg.type == StreamMsgType.RECONNECTED:
                     self._read_stream(4)  # Future use.
                 else:
                     raise ValueError('undefined msg type: ' + str(msg.type))
-            except ConnectionResetError:
+            except (ConnectionResetError, OSError) as e:
                 msg.type = StreamMsgType.STREAM_DEAD
                 self._stream_impl(msg)
+                self._stream_connected = False
                 return
             except Exception as e:
                 msg.type = StreamMsgType.ERROR
                 print('Stream error for contract: ' + msg.contract.to_string())
                 traceback.print_exc()
             self._stream_impl(msg)
```

### Comparing `thetadata-0.9.6/thetadata/enums.py` & `thetadata-0.9.7/thetadata/enums.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/thetadata/exceptions.py` & `thetadata-0.9.7/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/thetadata/parsing.py` & `thetadata-0.9.7/thetadata/parsing.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/thetadata/terminal.py` & `thetadata-0.9.7/thetadata/terminal.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/LICENSE` & `thetadata-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/README.md` & `thetadata-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.6/pyproject.toml` & `thetadata-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.6"
+version = "0.9.7"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `thetadata-0.9.6/PKG-INFO` & `thetadata-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
```

