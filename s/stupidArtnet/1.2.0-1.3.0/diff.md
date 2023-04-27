# Comparing `tmp/stupidArtnet-1.2.0.tar.gz` & `tmp/stupidArtnet-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/stupidArtnet/stupidArtnet/dist/tmpyxgx8do4/stupidArtnet-1.2.0.tar", last modified: Sun Feb 27 20:28:48 2022, max compression
+gzip compressed data, was "/home/runner/work/stupidArtnet/stupidArtnet/dist/tmp7tkn_qyg/stupidArtnet-1.3.0.tar", last modified: Sun Feb 27 20:44:34 2022, max compression
```

## Comparing `stupidArtnet-1.2.0.tar` & `stupidArtnet-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/stupidArtnet/
--rw-r--r--   0 runner    (1001) docker     (121)     6539 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/stupidArtnet/StupidArtnetServer.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/stupidArtnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10624 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/stupidArtnet/StupidArtnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/stupidArtnet/ArtnetUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/stupidArtnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/stupidArtnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/stupidArtnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/stupidArtnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/stupidArtnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-02-27 20:28:48.000000 stupidArtnet-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5839 2022-02-27 20:28:32.000000 stupidArtnet-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/stupidArtnet/
+-rw-r--r--   0 runner    (1001) docker     (121)     6745 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/stupidArtnet/StupidArtnetServer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/stupidArtnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10966 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/stupidArtnet/StupidArtnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/stupidArtnet/ArtnetUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/stupidArtnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/stupidArtnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6497 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/stupidArtnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/stupidArtnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/stupidArtnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6497 2022-02-27 20:44:34.000000 stupidArtnet-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-02-27 20:44:19.000000 stupidArtnet-1.3.0/README.md
```

### Comparing `stupidArtnet-1.2.0/LICENSE` & `stupidArtnet-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stupidArtnet-1.2.0/stupidArtnet/StupidArtnetServer.py` & `stupidArtnet-1.3.0/stupidArtnet/StupidArtnetServer.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,36 +14,37 @@
 from stupidArtnet.ArtnetUtils import make_address_mask
 
 
 class StupidArtnetServer():
     """(Very) simple implementation of an Artnet Server."""
 
     UDP_PORT = 6454
-    s = None
+    socket_server = None
     ARTDMX_HEADER = b'Art-Net\x00\x00P\x00\x0e'
     listeners = []
 
     def __init__(self):
         """Initializes Art-Net server."""
         # server active flag
         self.listen = True
 
-        self.th = Thread(target=self.__init_socket, daemon=True)
-        self.th.start()
+        self.server_thread = Thread(target=self.__init_socket, daemon=True)
+        self.server_thread.start()
 
     def __init_socket(self):
         """Initializes server socket."""
         # Bind to UDP on the correct PORT
-        self.s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.s.bind(('', self.UDP_PORT))  # Listen on any valid IP
+        self.socket_server = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.socket_server.setsockopt(
+            socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.socket_server.bind(('', self.UDP_PORT))  # Listen on any valid IP
 
         while self.listen:
 
-            data, unused_address = self.s.recvfrom(1024)
+            data, unused_address = self.socket_server.recvfrom(1024)
 
             # only dealing with Art-Net DMX
             if self.validate_header(data):
 
                 # check if this address is in any registered listener
                 for listener in self.listeners:
 
@@ -58,17 +59,17 @@
     def __del__(self):
         """Graceful shutdown."""
         self.listeners.clear()
         self.close()
 
     def __str__(self):
         """Printable object state."""
-        s = "===================================\n"
-        s += "Stupid Artnet Listening\n"
-        return s
+        state = "===================================\n"
+        state += "Stupid Artnet Listening\n"
+        return state
 
     def register_listener(self, universe=0, sub=0, net=0,
                           is_simplified=True, callback_function=None):
         """Adds a listener to an Art-Net Universe.
 
         Args:
         universe - Universe to listen
@@ -114,26 +115,29 @@
         """
         self.listeners = []
 
     def see_buffer(self, listener_id):
         """Show buffer values."""
         for listener in self.listeners:
             if listener.get('id') == listener_id:
-                print(listener.get('buffer'))
+                return listener.get('buffer')
 
         return "Listener not found"
 
     def get_buffer(self, listener_id):
         """Return buffer values."""
         for listener in self.listeners:
             if listener.get('id') == listener_id:
                 return listener.get('buffer')
         print("Buffer object not found")
         return []
 
+        print("No Listener with given id found")
+        return []
+
     def clear_buffer(self, listener_id):
         """Clear buffer in listener."""
         for listener in self.listeners:
             if listener.get('id') == listener_id:
                 listener['buffer'] = []
 
     def set_callback(self, listener_id, callback_function):
@@ -155,15 +159,15 @@
                 listener['simplified'] = is_simplified
                 listener['address_mask'] = address_mask
                 listener['buffer'] = []
 
     def close(self):
         """Close UDP socket."""
         self.listen = False         # Set flag
-        self.th.join()              # Terminate thread once jobs are complete
+        self.server_thread.join()              # Terminate thread once jobs are complete
 
     @staticmethod
     def validate_header(header):
         """Validates packet header as Art-Net packet.
 
         - The packet header spells Art-Net
         - The definition is for DMX Artnet (OPCode 0x50)
@@ -190,24 +194,24 @@
 
     print("===================================")
     print("Namespace run")
 
     # Art-Net 4 definition specifies nets and subnets
     # Please see README and Art-Net user guide for details
     # Here we use the simplified default
-    universe = 1
+    UNIVERSE_TO_LISTEN = 1
 
     # Initilize server, this starts a server in the Art-Net port
     a = StupidArtnetServer()
 
     # For every universe we would like to receive,
     # add a new listener with a optional callback
     # the return is an id for the listener
     u1_listener = a.register_listener(
-        universe, callback_function=test_callback)
+        UNIVERSE_TO_LISTEN, callback_function=test_callback)
 
     # print object state
     print(a)
 
     # giving it some time for the demo
     time.sleep(3)
```

### Comparing `stupidArtnet-1.2.0/stupidArtnet/StupidArtnet.py` & `stupidArtnet-1.3.0/stupidArtnet/StupidArtnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 NOTES
 - For simplicity: NET and SUBNET not used by default but optional
 
 """
 
 import socket
 from threading import Timer
-from stupidArtnet.ArtnetUtils import shift_this, put_in_range
 from time import sleep
+from stupidArtnet.ArtnetUtils import shift_this, put_in_range
 
 
 class StupidArtnet():
     """(Very) simple implementation of Artnet."""
 
     UDP_PORT = 6454
 
-    def __init__(self, targetIP='127.0.0.1', universe=0, packet_size=512, fps=30,
+    def __init__(self, target_ip='127.0.0.1', universe=0, packet_size=512, fps=30,
                  even_packet_size=True, broadcast=False):
         """Initializes Art-Net Client.
 
         Args:
         targetIP - IP of receiving device
         universe - universe to listen
         packet_size - amount of channels to transmit
@@ -32,289 +32,290 @@
         broadcast - whether to broadcast in local sub
 
         Returns:
         None
 
         """
         # Instance variables
-        self.TARGET_IP = targetIP
-        self.SEQUENCE = 0
-        self.PHYSICAL = 0
-        self.UNIVERSE = universe
-        self.SUB = 0
-        self.NET = 0
-        self.PACKET_SIZE = put_in_range(packet_size, 2, 512, even_packet_size)
-        self.HEADER = bytearray()
-        self.BUFFER = bytearray(self.PACKET_SIZE)
+        self.target_ip = target_ip
+        self.sequence = 0
+        self.physical = 0
+        self.universe = universe
+        self.subnet = 0
+        self.net = 0
+        self.packet_size = put_in_range(packet_size, 2, 512, even_packet_size)
+        self.packet_header = bytearray()
+        self.buffer = bytearray(self.packet_size)
 
-        self.bMakeEven = even_packet_size
+        self.make_even = even_packet_size
 
-        self.bIsSimplified = True		# simplify use of universe, net and subnet
+        self.is_simplified = True		# simplify use of universe, net and subnet
 
         # UDP SOCKET
-        self.s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.socket_client = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
         if broadcast:
-            self.s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+            self.socket_client.setsockopt(
+                socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
 
         # Timer
         self.fps = fps
         self.__clock = None
 
         self.make_header()
 
     def __del__(self):
         """Graceful shutdown."""
         self.stop()
         self.close()
 
     def __str__(self):
         """Printable object state."""
-        s = "===================================\n"
-        s += "Stupid Artnet initialized\n"
-        s += "Target IP: %s:%i \n" % (self.TARGET_IP, self.UDP_PORT)
-        s += "Universe: %i \n" % self.UNIVERSE
-        if not self.bIsSimplified:
-            s += "Subnet: %i \n" % self.SUB
-            s += "Net: %i \n" % self.NET
-        s += "Packet Size: %i \n" % self.PACKET_SIZE
-        s += "==================================="
+        state = "===================================\n"
+        state += "Stupid Artnet initialized\n"
+        state += f"Target IP: {self.target_ip} : {self.UDP_PORT} \n"
+        state += f"Universe: {self.universe} \n"
+        if not self.is_simplified:
+            state += f"Subnet: {self.subnet} \n"
+            state += f"Net: {self.net} \n"
+        state += f"Packet Size: {self.packet_size} \n"
+        state += "==================================="
 
-        return s
+        return state
 
     def make_header(self):
         """Make packet header."""
         # 0 - id (7 x bytes + Null)
-        self.HEADER = bytearray()
-        self.HEADER.extend(bytearray('Art-Net', 'utf8'))
-        self.HEADER.append(0x0)
+        self.packet_header = bytearray()
+        self.packet_header.extend(bytearray('Art-Net', 'utf8'))
+        self.packet_header.append(0x0)
         # 8 - opcode (2 x 8 low byte first)
-        self.HEADER.append(0x00)
-        self.HEADER.append(0x50)  # ArtDmx data packet
+        self.packet_header.append(0x00)
+        self.packet_header.append(0x50)  # ArtDmx data packet
         # 10 - prototocol version (2 x 8 high byte first)
-        self.HEADER.append(0x0)
-        self.HEADER.append(14)
+        self.packet_header.append(0x0)
+        self.packet_header.append(14)
         # 12 - sequence (int 8), NULL for not implemented
-        self.HEADER.append(self.SEQUENCE)
+        self.packet_header.append(self.sequence)
         # 13 - physical port (int 8)
-        self.HEADER.append(0x00)
+        self.packet_header.append(0x00)
         # 14 - universe, (2 x 8 low byte first)
-        if self.bIsSimplified:
+        if self.is_simplified:
             # not quite correct but good enough for most cases:
             # the whole net subnet is simplified
             # by transforming a single uint16 into its 8 bit parts
             # you will most likely not see any differences in small networks
-            v = shift_this(self.UNIVERSE)			# convert to MSB / LSB
-            self.HEADER.append(v[1])
-            self.HEADER.append(v[0])
+            msb, lsb = shift_this(self.universe)   # convert to MSB / LSB
+            self.packet_header.append(lsb)
+            self.packet_header.append(msb)
         # 14 - universe, subnet (2 x 4 bits each)
         # 15 - net (7 bit value)
         else:
             # as specified in Artnet 4 (remember to set the value manually after):
             # Bit 3  - 0 = Universe (1-16)
             # Bit 7  - 4 = Subnet (1-16)
             # Bit 14 - 8 = Net (1-128)
             # Bit 15     = 0
             # this means 16 * 16 * 128 = 32768 universes per port
             # a subnet is a group of 16 Universes
             # 16 subnets will make a net, there are 128 of them
-            self.HEADER.append(self.SUB << 4 | self.UNIVERSE)
-            self.HEADER.append(self.NET & 0xFF)
+            self.packet_header.append(self.subnet << 4 | self.universe)
+            self.packet_header.append(self.net & 0xFF)
         # 16 - packet size (2 x 8 high byte first)
-        v = shift_this(self.PACKET_SIZE)		# convert to MSB / LSB
-        self.HEADER.append(v[0])
-        self.HEADER.append(v[1])
+        msb, lsb = shift_this(self.packet_size)		# convert to MSB / LSB
+        self.packet_header.append(msb)
+        self.packet_header.append(lsb)
 
     def show(self):
         """Finally send data."""
         packet = bytearray()
-        packet.extend(self.HEADER)
-        packet.extend(self.BUFFER)
+        packet.extend(self.packet_header)
+        packet.extend(self.buffer)
         try:
-            self.s.sendto(packet, (self.TARGET_IP, self.UDP_PORT))
-        except socket.error as e:
-            print("ERROR: Socket error with exception: %s" % e)
+            self.socket_client.sendto(packet, (self.target_ip, self.UDP_PORT))
+        except socket.error as error:
+            print(f"ERROR: Socket error with exception: {error}")
         finally:
-            self.SEQUENCE = (self.SEQUENCE + 1) % 256
+            self.sequence = (self.sequence + 1) % 256
 
     def close(self):
         """Close UDP socket."""
-        self.s.close()
+        self.socket_client.close()
 
     # THREADING #
 
     def start(self):
         """Starts thread clock."""
         self.show()
         self.__clock = Timer((1000.0 / self.fps) / 1000.0, self.start)
         self.__clock.daemon = True
         self.__clock.start()
 
     def stop(self):
         """Stops thread clock."""
-        self.__clock.cancel()
+        if self.__clock is not None:
+            self.__clock.cancel()
 
     # SETTERS - HEADER #
 
     def set_universe(self, universe):
         """Setter for universe (0 - 15 / 256).
 
         Mind if protocol has been simplified
         """
         # This is ugly, trying to keep interface easy
         # With simplified mode the universe will be split into two
         # values, (uni and sub) which is correct anyway. Net will always be 0
-        if self.bIsSimplified:
-            self.UNIVERSE = put_in_range(universe, 0, 255, False)
+        if self.is_simplified:
+            self.universe = put_in_range(universe, 0, 255, False)
         else:
-            self.UNIVERSE = put_in_range(universe, 0, 15, False)
+            self.universe = put_in_range(universe, 0, 15, False)
         self.make_header()
 
     def set_subnet(self, sub):
         """Setter for subnet address (0 - 15).
 
         Set simplify to false to use
         """
-        self.SUB = put_in_range(sub, 0, 15, False)
+        self.subnet = put_in_range(sub, 0, 15, False)
         self.make_header()
 
     def set_net(self, net):
         """Setter for net address (0 - 127).
 
         Set simplify to false to use
         """
-        self.NET = put_in_range(net, 0, 127, False)
+        self.net = put_in_range(net, 0, 127, False)
         self.make_header()
 
     def set_packet_size(self, packet_size):
         """Setter for packet size (2 - 512, even only)."""
-        self.PACKET_SIZE = put_in_range(packet_size, 2, 512, self.bMakeEven)
+        self.packet_size = put_in_range(packet_size, 2, 512, self.make_even)
         self.make_header()
 
     # SETTERS - DATA #
 
     def clear(self):
         """Clear DMX buffer."""
-        self.BUFFER = bytearray(self.PACKET_SIZE)
+        self.buffer = bytearray(self.packet_size)
 
-    def set(self, p):
+    def set(self, value):
         """Set buffer."""
-        if len(self.BUFFER) != self.PACKET_SIZE:
+        if len(value) != self.packet_size:
             print("ERROR: packet does not match declared packet size")
             return
-        self.BUFFER = p
+        self.buffer = value
 
     def set_16bit(self, address, value, high_first=False):
         """Set single 16bit value in DMX buffer."""
-        if address > self.PACKET_SIZE:
+        if address > self.packet_size:
             print("ERROR: Address given greater than defined packet size")
             return
         if address < 1 or address > 512 - 1:
             print("ERROR: Address out of range")
             return
         value = put_in_range(value, 0, 65535, False)
 
         # Check for endianess
         if high_first:
-            self.BUFFER[address - 1] = (value >> 8) & 0xFF  # high
-            self.BUFFER[address] = (value) & 0xFF 			# low
+            self.buffer[address - 1] = (value >> 8) & 0xFF  # high
+            self.buffer[address] = (value) & 0xFF 			# low
         else:
-            self.BUFFER[address - 1] = (value) & 0xFF				# low
-            self.BUFFER[address] = (value >> 8) & 0xFF  # high
+            self.buffer[address - 1] = (value) & 0xFF				# low
+            self.buffer[address] = (value >> 8) & 0xFF  # high
 
     def set_single_value(self, address, value):
         """Set single value in DMX buffer."""
-        if address > self.PACKET_SIZE:
+        if address > self.packet_size:
             print("ERROR: Address given greater than defined packet size")
             return
         if address < 1 or address > 512:
             print("ERROR: Address out of range")
             return
-        self.BUFFER[address - 1] = put_in_range(value, 0, 255, False)
+        self.buffer[address - 1] = put_in_range(value, 0, 255, False)
 
     def set_single_rem(self, address, value):
         """Set single value while blacking out others."""
-        if address > self.PACKET_SIZE:
+        if address > self.packet_size:
             print("ERROR: Address given greater than defined packet size")
             return
         if address < 1 or address > 512:
             print("ERROR: Address out of range")
             return
         self.clear()
-        self.BUFFER[address - 1] = put_in_range(value, 0, 255, False)
+        self.buffer[address - 1] = put_in_range(value, 0, 255, False)
 
-    def set_rgb(self, address, r, g, b):
+    def set_rgb(self, address, red, green, blue):
         """Set RGB from start address."""
-        if address > self.PACKET_SIZE:
+        if address > self.packet_size:
             print("ERROR: Address given greater than defined packet size")
             return
         if address < 1 or address > 510:
             print("ERROR: Address out of range")
             return
 
-        self.BUFFER[address - 1] = put_in_range(r, 0, 255, False)
-        self.BUFFER[address] = put_in_range(g, 0, 255, False)
-        self.BUFFER[address + 1] = put_in_range(b, 0, 255, False)
+        self.buffer[address - 1] = put_in_range(red, 0, 255, False)
+        self.buffer[address] = put_in_range(green, 0, 255, False)
+        self.buffer[address + 1] = put_in_range(blue, 0, 255, False)
 
     # AUX Function #
 
-    def send(self, p):
+    def send(self, packet):
         """Set buffer and send straightaway.
 
         Args:
         array - integer array to send
         """
-        self.set(p)
+        self.set(packet)
         self.show()
 
-    def set_simplified(self, bDoSimplify):
+    def set_simplified(self, simplify):
         """Builds Header accordingly.
 
         True - Header sends 16 bit universe value (OK but incorrect)
         False - Headers sends Universe - Net and Subnet values as protocol
         It is recommended that you set these values with .set_net() and set_physical
         """
-        if bDoSimplify == self.bIsSimplified:
+        # avoid remaking header if there are no changes
+        if simplify == self.is_simplified:
             return
-        self.bIsSimplified = bDoSimplify
+        self.is_simplified = simplify
         self.make_header()
 
     def see_header(self):
         """Show header values."""
-        print(self.HEADER)
+        print(self.packet_header)
 
     def see_buffer(self):
         """Show buffer values."""
-        print(self.BUFFER)
+        print(self.buffer)
 
     def blackout(self):
         """Sends 0's all across."""
         self.clear()
         self.show()
 
     def flash_all(self, delay=None):
         """Sends 255's all across."""
-        packet = [255] * self.PACKET_SIZE
-        self.set(packet)
+        self.set([255] * self.packet_size)
         self.show()
         # Blackout after delay
         if delay:
             sleep(delay)
             self.blackout()
 
 
 if __name__ == '__main__':
     print("===================================")
     print("Namespace run")
-    target_ip = '127.0.0.1'			# typically in 2.x or 10.x range
-    universe = 15 					# see docs
-    packet_size = 20				# it is not necessary to send whole universe
-    packet = bytearray(packet_size)
+    TARGET_IP = '127.0.0.1'         # typically in 2.x or 10.x range
+    UNIVERSE_TO_SEND = 15           # see docs
+    PACKET_SIZE = 20                # it is not necessary to send whole universe
 
-    a = StupidArtnet(target_ip, universe, packet_size)
+    a = StupidArtnet(TARGET_IP, UNIVERSE_TO_SEND, PACKET_SIZE)
     a.set_simplified(False)
     a.set_net(129)
     a.set_subnet(16)
 
     # Look at the object state
     print(a)
```

### Comparing `stupidArtnet-1.2.0/stupidArtnet/ArtnetUtils.py` & `stupidArtnet-1.3.0/stupidArtnet/ArtnetUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Provides common functions byte objects."""
+
+
 def shift_this(number, high_first=True):
     """Utility method: extracts MSB and LSB from number.
 
     Args:
     number - number to shift
     high_first - MSB or LSB first (true / false)
```

### Comparing `stupidArtnet-1.2.0/setup.py` & `stupidArtnet-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(name='stupidArtnet',
       author='cpvalente',
-      version='1.2.0',
+      version='1.3.0',
       license='MIT',
       description='(Very) Simple implementation of the Art-Net protocol',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/cpvalente/stupidArtnet',
       project_urls={
           'Bug Tracker': 'https://github.com/cpvalente/stupidArtnet/issues',
```

### Comparing `stupidArtnet-1.2.0/stupidArtnet.egg-info/PKG-INFO` & `stupidArtnet-1.3.0/stupidArtnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stupidArtnet
-Version: 1.2.0
+Version: 1.3.0
 Summary: (Very) Simple implementation of the Art-Net protocol
 Home-page: https://github.com/cpvalente/stupidArtnet
 Author: cpvalente
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cpvalente/stupidArtnet/issues
 Keywords: LIGHTING,DMX,LIGHTING CONTROL
 Platform: UNKNOWN
@@ -137,18 +137,19 @@
 This will look correct and behave fine for smaller networks, wanting to be able to specify Universes, Subnets and Nets you can disable simplification and give values as needed. <br />
 The spec for Artnet 4 applies here: 128 Nets contain 16 Subnets which contain 16 Universes. 128 * 16 * 16 = 32 768 Universes
 
 ```python
 # Create a StupidArtnet instance with the relevant values
 
 # By default universe is simplified to a value between 0 - 255
+# this should suffice for anything not using subnets
 # on sending universe will be masked to two values
 # making the use of subnets invisible
 
-universe = 17
+universe = 17	# equivalent to universe 1 subnet 1
 a = StupidArtnet(target_ip, universe, packet_size)
 
 
 #############################################
 
 # You can also disable simplification
 a.set_simplified(False)
```

### Comparing `stupidArtnet-1.2.0/PKG-INFO` & `stupidArtnet-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stupidArtnet
-Version: 1.2.0
+Version: 1.3.0
 Summary: (Very) Simple implementation of the Art-Net protocol
 Home-page: https://github.com/cpvalente/stupidArtnet
 Author: cpvalente
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cpvalente/stupidArtnet/issues
 Keywords: LIGHTING,DMX,LIGHTING CONTROL
 Platform: UNKNOWN
@@ -137,18 +137,19 @@
 This will look correct and behave fine for smaller networks, wanting to be able to specify Universes, Subnets and Nets you can disable simplification and give values as needed. <br />
 The spec for Artnet 4 applies here: 128 Nets contain 16 Subnets which contain 16 Universes. 128 * 16 * 16 = 32 768 Universes
 
 ```python
 # Create a StupidArtnet instance with the relevant values
 
 # By default universe is simplified to a value between 0 - 255
+# this should suffice for anything not using subnets
 # on sending universe will be masked to two values
 # making the use of subnets invisible
 
-universe = 17
+universe = 17	# equivalent to universe 1 subnet 1
 a = StupidArtnet(target_ip, universe, packet_size)
 
 
 #############################################
 
 # You can also disable simplification
 a.set_simplified(False)
```

### Comparing `stupidArtnet-1.2.0/README.md` & `stupidArtnet-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -120,18 +120,19 @@
 This will look correct and behave fine for smaller networks, wanting to be able to specify Universes, Subnets and Nets you can disable simplification and give values as needed. <br />
 The spec for Artnet 4 applies here: 128 Nets contain 16 Subnets which contain 16 Universes. 128 * 16 * 16 = 32 768 Universes
 
 ```python
 # Create a StupidArtnet instance with the relevant values
 
 # By default universe is simplified to a value between 0 - 255
+# this should suffice for anything not using subnets
 # on sending universe will be masked to two values
 # making the use of subnets invisible
 
-universe = 17
+universe = 17	# equivalent to universe 1 subnet 1
 a = StupidArtnet(target_ip, universe, packet_size)
 
 
 #############################################
 
 # You can also disable simplification
 a.set_simplified(False)
```

