# Comparing `tmp/mcclient-lib-0.8.8.tar.gz` & `tmp/mcclient-lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcclient-lib-0.8.8.tar", last modified: Fri Jan 13 15:43:07 2023, max compression
+gzip compressed data, was "mcclient-lib-1.0.0.tar", last modified: Thu Apr 27 15:53:53 2023, max compression
```

## Comparing `mcclient-lib-0.8.8.tar` & `mcclient-lib-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.974768 mcclient-lib-0.8.8/
--rw-rw-rw-   0        0        0     1075 2022-12-26 17:27:07.000000 mcclient-lib-0.8.8/LICENSE
--rw-rw-rw-   0        0        0     2008 2023-01-13 15:43:07.974768 mcclient-lib-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2023-01-13 15:30:49.000000 mcclient-lib-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.952734 mcclient-lib-0.8.8/mcclient/
--rw-rw-rw-   0        0        0      225 2023-01-08 15:57:16.000000 mcclient-lib-0.8.8/mcclient/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-01-08 16:00:02.000000 mcclient-lib-0.8.8/mcclient/address.py
--rw-rw-rw-   0        0        0     2307 2023-01-08 16:03:54.000000 mcclient-lib-0.8.8/mcclient/base_client.py
--rw-rw-rw-   0        0        0     1363 2023-01-08 00:44:37.000000 mcclient-lib-0.8.8/mcclient/bedrock_slp.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.955736 mcclient-lib-0.8.8/mcclient/encoding/
--rw-rw-rw-   0        0        0        0 2022-12-15 16:55:04.000000 mcclient-lib-0.8.8/mcclient/encoding/__init__.py
--rw-rw-rw-   0        0        0      912 2022-12-15 16:56:27.000000 mcclient-lib-0.8.8/mcclient/encoding/packet.py
--rw-rw-rw-   0        0        0      655 2022-12-15 16:49:17.000000 mcclient-lib-0.8.8/mcclient/encoding/varint.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.959242 mcclient-lib-0.8.8/mcclient/query/
--rw-rw-rw-   0        0        0        0 2022-12-15 17:01:43.000000 mcclient-lib-0.8.8/mcclient/query/__init__.py
--rw-rw-rw-   0        0        0      413 2022-12-16 22:27:05.000000 mcclient-lib-0.8.8/mcclient/query/packet.py
--rw-rw-rw-   0        0        0     3047 2022-12-29 15:58:34.000000 mcclient-lib-0.8.8/mcclient/query/query_client.py
--rw-rw-rw-   0        0        0     5753 2023-01-01 16:31:18.000000 mcclient-lib-0.8.8/mcclient/response.py
--rw-rw-rw-   0        0        0     1883 2023-01-08 16:03:09.000000 mcclient-lib-0.8.8/mcclient/slp.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.972765 mcclient-lib-0.8.8/mcclient_lib.egg-info/
--rw-rw-rw-   0        0        0     2008 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-01-13 15:42:54.000000 mcclient-lib-0.8.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-13 15:43:07.974768 mcclient-lib-0.8.8/setup.cfg
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.681413 mcclient-lib-1.0.0/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1090 2023-02-17 12:34:30.000000 mcclient-lib-1.0.0/LICENSE
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3698 2023-04-27 15:53:53.678483 mcclient-lib-1.0.0/PKG-INFO
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3266 2023-04-25 18:09:46.000000 mcclient-lib-1.0.0/README.md
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.227221 mcclient-lib-1.0.0/mcclient/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      196 2023-04-26 19:07:22.000000 mcclient-lib-1.0.0/mcclient/__init__.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1590 2023-04-27 14:48:51.000000 mcclient-lib-1.0.0/mcclient/address.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2835 2023-04-27 14:52:51.000000 mcclient-lib-1.0.0/mcclient/base_client.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1763 2023-04-27 14:54:50.000000 mcclient-lib-1.0.0/mcclient/bedrock_slp.py
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.324435 mcclient-lib-1.0.0/mcclient/encoding/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-01-27 20:41:53.000000 mcclient-lib-1.0.0/mcclient/encoding/__init__.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1246 2023-04-26 20:35:05.000000 mcclient-lib-1.0.0/mcclient/encoding/packet.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      751 2023-04-26 20:24:04.000000 mcclient-lib-1.0.0/mcclient/encoding/varint.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3486 2023-04-27 14:56:04.000000 mcclient-lib-1.0.0/mcclient/query_client.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     7222 2023-04-27 15:19:29.000000 mcclient-lib-1.0.0/mcclient/response.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2062 2023-04-27 14:59:01.000000 mcclient-lib-1.0.0/mcclient/slp.py
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.464600 mcclient-lib-1.0.0/mcclient_lib.egg-info/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     3698 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      611 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        1 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)       24 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/requires.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        9 2023-04-27 15:53:52.000000 mcclient-lib-1.0.0/mcclient_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      861 2023-04-27 15:19:55.000000 mcclient-lib-1.0.0/pyproject.toml
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)       38 2023-04-27 15:53:53.682388 mcclient-lib-1.0.0/setup.cfg
+drwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)        0 2023-04-27 15:53:53.650164 mcclient-lib-1.0.0/tests/
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      421 2023-04-26 20:25:33.000000 mcclient-lib-1.0.0/tests/test_address.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1497 2023-04-26 18:55:31.000000 mcclient-lib-1.0.0/tests/test_bedrock.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)      753 2023-04-26 20:33:35.000000 mcclient-lib-1.0.0/tests/test_encoding.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1038 2023-04-26 18:53:32.000000 mcclient-lib-1.0.0/tests/test_formatting_removal.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     1343 2023-04-26 18:52:08.000000 mcclient-lib-1.0.0/tests/test_legacy_slp.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     4257 2023-04-26 18:56:39.000000 mcclient-lib-1.0.0/tests/test_query.py
+-rwxrwxrwx   0 sch8ill   (1000) sch8ill   (1000)     2019 2023-04-26 20:35:54.000000 mcclient-lib-1.0.0/tests/test_slp.py
```

### Comparing `mcclient-lib-0.8.8/LICENSE` & `mcclient-lib-1.0.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022
+Copyright (c) 2022-2023 Sch8ill
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `mcclient-lib-0.8.8/mcclient/address.py` & `mcclient-lib-1.0.0/mcclient/base_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,98 @@
+import socket
+import struct
 
-import dns.resolver
-
-
-
-class Address:
-    def __init__(self, addr, proto="tcp"):
-        self.addr = addr
-        self.proto = proto
-        self.is_ip = self._ip_check(self.addr)
-
-
-    def get_host(self, srv=True):
-        if self.is_ip:
-            return self.addr, None
+from mcclient.address import Address
+from mcclient.encoding.packet import Packet
+from mcclient.encoding.varint import VarInt
+
+DEFAULT_HOST = "localhost"
+DEFAULT_PORT = 25565
+DEFAULT_TIMEOUT = 5
+DEFAULT_PROTO = 47
+
+
+class BaseClient:
+    host: str
+    hostname: str
+    port: int
+    sock: socket.socket
+    varint: VarInt
+    connected: bool | None
+    protocol_version: int
+
+    def __init__(self, host: str = DEFAULT_HOST, port: int = DEFAULT_PORT, timeout: int = DEFAULT_TIMEOUT, proto: int = DEFAULT_PROTO, srv: bool = True):
+        self.sock = socket.socket(
+            socket.AF_INET, socket.SOCK_STREAM)
+        self.port = port
+        self.varint = VarInt()
+        self.connected = False
+        self.protocol_version = proto
+
+        self.sock.settimeout(timeout)
+        self.get_host(host, port, srv=srv)
+
+    def get_host(self, hostname: str, port: int, srv: bool) -> None:
+        addr = Address(hostname)
+        self.host, srv_port = addr.get_host(srv)
+        self.hostname = hostname
+        if srv_port == -1:
+            self.port = port
 
         else:
-            return self._resolve_hostname(self.addr, srv)
-
+            self.port = srv_port
 
-    def _resolve_hostname(self, hostname, srv):
-        host = self._resolve_a_record(hostname)
-        srv_record = None
-        if srv:
-            try:
-                srv_record = self._mc_srv_lookup(hostname, self.proto)
-                srv = True
-                
-            except Exception:
-                pass
-
-        if srv_record != None:
-            return host, srv_record[1]
+    def _connect(self) -> None:
+        if self.connected == False:
+            self.sock.connect((self.host, self.port))
+            self.connected = True
+
+        elif self.connected == None:
+            self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.connected = False
+            self._connect()
+
+    def _send(self, packet: Packet):
+        return self.sock.send(packet.pack())
+
+    def _recv(self) -> tuple[bool, int, bytes]:
+        length = self.varint.unpack(self.sock)
+        packet_id = self.varint.unpack(self.sock)
+        data = self.sock.recv(length)
+        if len(data) < length - 4:
+            loss = True
 
         else:
-            return host, None
-
-
-    @staticmethod
-    def _mc_srv_lookup(hostname, proto):
-        srv_prefix = f"_minecraft._{proto}."
-        srv_record = dns.resolver.resolve(srv_prefix + hostname, "SRV")[0]# only use the first srv record returned
-        host = str(srv_record.target).rstrip(".")
-        port = int(srv_record.port)
-        return host, port
-
-
-    @staticmethod
-    def _resolve_a_record(hostname):
-        record = dns.resolver.resolve(hostname, "A")[0]
-        return str(record).rstrip(".")
-
-
-    @staticmethod
-    def _ip_check(addr):
-        is_ip = True
-        if addr.count(".") == 3:
-            for octet in addr.split("."):
-                try:
-                    octet = int(octet)
-                    if not octet <= 255 and octet >= 0:
-                        is_ip = False
-                        break
+            loss = False
+        return loss, packet_id, data
 
-                except ValueError:
-                    is_ip = False
-
-        else:
-            is_ip = False
-        return is_ip
+    def _close(self, flush: bool = True):
+        if flush:
+            self._flush()
+        self.sock.close()
+        self.connected = None
+
+    def _reset(self) -> None:
+        self._close()
+        self._connect()
+        self._handshake()
+
+    def _flush(self, chunk_size: int = 8192) -> None:
+        try:
+            self.sock.recv(chunk_size)
+
+        except Exception:
+            return
+
+    def implant_socket(self, sock: socket.socket) -> None:
+        self.sock = sock
+        self.connected = True
+
+    def _handshake(self, next_state: int = 1) -> None:
+        packet = Packet(
+            b"\x00",  # packet id
+            self.varint.pack(self.protocol_version),
+            self.hostname,
+            struct.pack(">H", self.port),
+            self.varint.pack(next_state)  # next state 1 for status request
+        )
+        self._send(packet)
```

### Comparing `mcclient-lib-0.8.8/mcclient/bedrock_slp.py` & `mcclient-lib-1.0.0/mcclient/bedrock_slp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-
 import socket
 import struct
+
 from mcclient.address import Address
 from mcclient.response import BedrockResponse
+from mcclient.base_client import DEFAULT_TIMEOUT
 
-
-class BedrockSLPClient:
-    def __init__(self, host, port=19132, timeout=4):
-        self.get_host(host, port)
-        self.timeout = timeout
+DEFAULT_BEDROCK_PORT = 19132
 
 
-    def get_host(self, hostname, port):
-        addr = Address(hostname, proto="udp")
-        addr = addr.get_host()
+class BedrockSLPClient:
+    host: str
+    port: int
+    hostname: str
+    sock: socket.socket
+
+    def __init__(self, host: str, port: int = DEFAULT_BEDROCK_PORT, timeout: int = DEFAULT_TIMEOUT, srv: bool = True):
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.sock.settimeout(timeout)
+        self.get_host(host, port, srv)
+
+    def get_host(self, hostname: str, port: int, srv: bool) -> None:
+        addr = Address(hostname)
+        self.host, srv_port = addr.get_host(srv)
         self.hostname = hostname
-        self.host = addr[0]
-        if addr[1] == None:
+        if srv_port == -1:
             self.port = port
 
         else:
-            self.port = addr[1]
-
+            self.port = srv_port
 
-    def get_status(self):
-        res = self._request_status()
-        res = self._parse_res(res)
+    def get_status(self) -> BedrockResponse:
+        raw_res = self._request_status()
+        res = self._parse_res(raw_res)
         return BedrockResponse(self.hostname, self.port, res)
 
-    
-    def _request_status(self):
-        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        sock.settimeout(self.timeout)
-
+    def _request_status(self) -> bytes:
+        """
+        needs to be updated (https://wiki.vg/Raknet_Protocol#Unconnected_Ping)
+        """
         status_request = b"\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\xff\xff\x00\xfe\xfe\xfe\xfe\xfd\xfd\xfd\xfd\x124Vx"
-        sock.sendto(status_request, (self.host, self.port))
-        data, _ = sock.recvfrom(4096)
-        return data
-
+        self.sock.sendto(status_request, (self.host, self.port))
+        return self.sock.recv(4096)
 
     @staticmethod
-    def _parse_res(res):
-        res = res[1:]
-        extra_len = struct.unpack(">H", res[32:34])[0]
-        res = res[34 : 34 + extra_len]
-        res = res.decode()
-        res = res.split(";")
-        return res
+    def _parse_res(raw_bytes: bytes) -> list[str]:
+        res_bytes = raw_bytes[1:]
+        extra_len = struct.unpack(">H", res_bytes[32:34])[0]
+        res_bytes = res_bytes[34: 34 + extra_len]
+        res_str = res_bytes.decode()
+        res_split = res_str.split(";")
+        return res_split
```

### Comparing `mcclient-lib-0.8.8/mcclient/encoding/packet.py` & `mcclient-lib-1.0.0/mcclient/encoding/packet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-
 import struct
+
 from mcclient.encoding.varint import VarInt
 
 
 class Packet:
-    def __init__(self, fields=[]):
+    fields: tuple
+    varint: VarInt
+
+    def __init__(self, *fields):
         self.fields = fields
         self.varint = VarInt()
 
-
-    def pack(self):
+    def pack(self) -> bytes:
         packet = b""
         for field in self.fields:
             field = self._encode(field)
             packet += field
 
-        packet = self.varint.pack(len(packet)) + packet # add packetlength
+        packet = self.varint.pack(len(packet)) + \
+            packet  # add the packet length
         return packet
 
-
-    def _encode(self, data):
-        if type(data) == int:
-            data = struct.pack(">H", data)
-
-        elif type(data) == str:
+    def _encode(self, data) -> bytes:
+        if type(data) == str:
             data = data.encode("utf-8")
             data = self.varint.pack(len(data)) + data
 
         elif type(data) == bool:
             data = b"\x01" if data else b"\x00"
+        return data
 
-        elif type(data) == float:
-            print(data)
-            data = struct.pack(">Q", int(data))
-            print(data)
-        return data
+
+class QueryPacket:
+    type: int
+    session_id: int
+    payload: bytes
+
+    def __init__(self, type, session_id, payload):
+        self.type = type
+        self.session_id = session_id
+        self.payload = payload
+
+    def pack(self) -> bytes:
+        packet = b"\xFE\xFD"  # query packet padding
+        packet += struct.pack("!B", self.type)
+        packet += struct.pack('>l', self.session_id)
+        packet += self.payload
+        return packet
```

### Comparing `mcclient-lib-0.8.8/mcclient/query/query_client.py` & `mcclient-lib-1.0.0/mcclient/slp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,62 @@
+import json
 
-import socket
-import struct
-import random
-from mcclient.response import QueryResponse
-from mcclient.query.packet import QueryPacket
-
-class QueryClient:
-    def __init__(self, host="localhost", port=25565, timeout=0.5):
-        self.host = host
-        self.port = port
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.sock.settimeout(timeout)
-
-
-    def _handshake(self):
-        self.session_id = random.randint(0, 2147483648) & 0x0F0F0F0F # generate session id from int between 0 and 2147483648
-        packet = QueryPacket(
-            9, # type 9 for handshaking
-            self.session_id,
-            b"" # empty payload
-        )
-        packet = packet.pack()
-        self._send(packet)
-        res = self._recv()
-        self.token = struct.pack('>l', int(res[2][:-1])) # extract token from response
-        
-
-    def _send(self, packet):
-        return self.sock.sendto(packet, (self.host, self.port))
+from mcclient.response import SLPResponse, LegacySLPResponse
+from mcclient.base_client import BaseClient
+from mcclient.encoding.packet import Packet
+from mcclient.base_client import DEFAULT_PORT, DEFAULT_TIMEOUT, DEFAULT_PROTO
 
 
-    def _recv(self):
-        res = self.sock.recv(4096)
-        type = res[0]
-        session_id = res[1:5]
-        payload = res[5:]
-        return type, session_id, payload
+class SLPClient(BaseClient):
+    retries: int
 
+    def __init__(self, host: str, port: int = DEFAULT_PORT, timeout: int = DEFAULT_TIMEOUT, proto: int = DEFAULT_PROTO, srv: bool = True):
+        super().__init__(host=host, port=port, timeout=timeout, proto=proto, srv=srv)
+        self.retries = 0
 
-    def _query_request(self):
-        self._handshake()
-        payload = self.token + b"\x00\x00\x00\x00" # challenge token and some padding for full status request
-        packet = QueryPacket(
-            0, # packettype 0 for status request
-            self.session_id,
-            payload
-        )
-        packet = packet.pack()
+    def _status_request(self) -> dict:
+        packet = Packet(b"\x00")  # send status request
         self._send(packet)
         res = self._recv()
-        res = self._read_query(res)
-        return res
 
-
-    def get_status(self):
-        res = self._query_request()
-        return QueryResponse(self.host, self.port, res)
-
-
-    @staticmethod
-    def _read_query(res):
-        res = res[2][11:] # remove unnecessary padding
-        stats, players = res.split(b"\x00\x00\x01player_\x00\x00") # split stats from players
-        data = {}
-
-        stats = stats.split(b"\x00")
-        stats = [stat.decode("utf-8") for stat in stats] # decode keys and values
-        stats[0] = "motd" # replace "hostname" with "motd"
-        key = True
-        for y, x in enumerate(stats):
-            if key:
-                data[x] = stats[y + 1]
-                key = False
+        if res[0]:
+            # if packetloss occured
+            if self.retries < 3:
+                self.retries += 1
+                self._reset()
+                return self._status_request()
 
             else:
-                key = True
+                raise Exception("Max retries exceeded.")
+
+        self._close(flush=False)
 
-        for key in ["numplayers", "maxplayers", "hostport"]: # convert strings to ints
-            data[key] = int(data[key])
+        res_data = res[2][2:]
+        res_str = res_data.decode("utf-8")
+        res_dict = json.loads(res_str)
+        return res_dict
 
-        data["software"] = "Vanilla"
-        software_parts = data["plugins"].split(":", 1)
-        data["software"] = software_parts[0].strip()
-        if len(software_parts) == 2:
-            data["plugins"] = [plugin.strip() for plugin in software_parts[1].split(";")]
-
-        else:
-            data["plugins"] = []
-
-        players = players[:-2] # remove endpadding
-        players = players.split(b"\x00") # split players
-        data["players"] = [player.decode("utf-8") for player in players if player != b""] # decode players
-        return data
+    def get_status(self) -> SLPResponse:
+        self._connect()
+        self._handshake()
+        res = self._status_request()
+        self.retries = 0
+        return SLPResponse(self.hostname, self.port, res)
+
+
+class LegacySLPClient(BaseClient):
+    def __init__(self, host: str, port: int = 25565, timeout: int = 5):
+        super().__init__(host=host, port=port, timeout=timeout)
+
+    def get_status(self) -> LegacySLPResponse:
+        self._connect()
+        # legacy status request
+        self.sock.send(b"\xFE\x01")
+        raw_res = self.sock.recv(1024)
+        self._close()
+
+        # remove padding and other headers
+        res_bytes = raw_res[3:]
+        res_str = res_bytes.decode("UTF-16-be", errors="ignore")
+        res_split_str = res_str.split("\x00")
+        res = LegacySLPResponse(self.hostname, self.port, res_split_str)
+        return res
```

