# Comparing `tmp/pyserve3-0.0.3.tar.gz` & `tmp/pyserve3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserve3-0.0.3.tar", last modified: Wed Mar 29 05:15:12 2023, max compression
+gzip compressed data, was "pyserve3-0.0.4.tar", last modified: Wed Apr 26 23:00:53 2023, max compression
```

## Comparing `pyserve3-0.0.3.tar` & `pyserve3-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-29 05:15:12.015532 pyserve3-0.0.3/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-03-26 23:32:22.000000 pyserve3-0.0.3/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-03-29 05:15:12.015532 pyserve3-0.0.3/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      944 2023-03-19 20:01:09.000000 pyserve3-0.0.3/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-29 05:15:12.015532 pyserve3-0.0.3/pyserve/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5755 2023-03-26 23:29:59.000000 pyserve3-0.0.3/pyserve/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1608 2023-03-19 08:30:13.000000 pyserve3-0.0.3/pyserve/abc.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6477 2023-03-29 03:56:56.000000 pyserve3-0.0.3/pyserve/threading.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3398 2023-03-19 18:24:12.000000 pyserve3-0.0.3/pyserve/transport.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-29 05:15:12.015532 pyserve3-0.0.3/pyserve3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-03-29 05:15:11.000000 pyserve3-0.0.3/pyserve3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      231 2023-03-29 05:15:12.000000 pyserve3-0.0.3/pyserve3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-03-29 05:15:11.000000 pyserve3-0.0.3/pyserve3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-03-29 05:15:11.000000 pyserve3-0.0.3/pyserve3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-03-29 05:15:12.015532 pyserve3-0.0.3/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)      674 2023-03-29 05:14:51.000000 pyserve3-0.0.3/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 23:00:53.510634 pyserve3-0.0.4/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-03-26 23:32:22.000000 pyserve3-0.0.4/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-04-26 23:00:53.510634 pyserve3-0.0.4/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      944 2023-03-19 20:01:09.000000 pyserve3-0.0.4/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 23:00:53.510634 pyserve3-0.0.4/pyserve/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5912 2023-04-26 22:52:30.000000 pyserve3-0.0.4/pyserve/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1608 2023-04-26 22:44:45.000000 pyserve3-0.0.4/pyserve/abc.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6621 2023-04-26 22:58:51.000000 pyserve3-0.0.4/pyserve/threading.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3029 2023-04-26 22:37:10.000000 pyserve3-0.0.4/pyserve/transport.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 23:00:53.510634 pyserve3-0.0.4/pyserve3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-04-26 23:00:53.000000 pyserve3-0.0.4/pyserve3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      231 2023-04-26 23:00:53.000000 pyserve3-0.0.4/pyserve3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-26 23:00:53.000000 pyserve3-0.0.4/pyserve3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-04-26 23:00:53.000000 pyserve3-0.0.4/pyserve3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-26 23:00:53.510634 pyserve3-0.0.4/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      674 2023-04-26 23:00:04.000000 pyserve3-0.0.4/setup.py
```

### Comparing `pyserve3-0.0.3/LICENSE` & `pyserve3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.3/PKG-INFO` & `pyserve3-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserve3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unify SocketServer Implementations based on a Session Model
 Home-page: https://github.com/imgurbot12/pyserve
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyserve3-0.0.3/README.md` & `pyserve3-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.3/pyserve/__init__.py` & `pyserve3-0.0.4/pyserve/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Unify SocketServer Implementations based on Session Model
 """
 import asyncio
 from ssl import SSLContext
 from typing import Type, Optional
 
-from .abc import RawAddr, Address, Writer, Session
+from .abc import RawAddr, Address, Writer, Session, modify_socket
 from .transport import UdpProtocol, TcpProtocol
 from .threading import UdpThreadServer, TcpThreadServer
 
 #** Variables **#
 __all__ = [
     'listen_udp_async',
     'listen_tcp_async',
@@ -23,37 +23,39 @@
 
 #** Functions **#
 
 async def listen_udp_async(
     address:         RawAddr, 
     factory:         Type[Session],
     *args,
-    timeout:         Optional[int]   = None,
     interface:       Optional[bytes] = None,
     reuse_port:      bool            = False,
     allow_broadcast: bool            = False,
     **kwargs,
 ):
     """
     :param address:         host/port of server
     :param factory:         type factory for server request handler
     :param args:            positional args to pass to the session factory
-    :param timeout:         max socket lifetime duration timeout if configured
     :param interface:       interface to bind server socket to
     :param reuse_port:      allow reuse of same port when enabled
     :param allow_broadcast: allow for udp broadcast messages when enabled
     :param kwargs:          keyword arguments to pass to session factory
     """
     # spawn protocol factory and test session generation
     loop = asyncio.get_running_loop()
-    func = lambda: UdpProtocol(factory, args, kwargs, timeout, interface)
+    func = lambda: UdpProtocol(factory, args, kwargs)
     func().test_factory()
     # spawn server instance
-    tport, _ = await loop.create_datagram_endpoint(func, address, 
+    tport, protocol = await loop.create_datagram_endpoint(func, address, 
         reuse_port=reuse_port, allow_broadcast=allow_broadcast)
+    # modify transport interface when enabled
+    if interface:
+        sock = protocol.transport.get_extra_info('socket')
+        modify_socket(sock, None, interface)
     # run server forever
     try:
         while True:
             await asyncio.sleep(3600)
     finally:
         tport.close()
 
@@ -77,29 +79,32 @@
     :param reuse_port:      allow reuse of same port when enabled
     :param backlog:         number of allowed and backloged async requests
     :param ssl:             TLS context to encrypt socket communications
     :param kwargs:          keyword arguments to pass to session factory
     """
     # spawn protocol factory and test session generation
     loop = asyncio.get_running_loop()
-    func = lambda: TcpProtocol(factory, args, kwargs, timeout, interface)
+    func = lambda: TcpProtocol(factory, args, kwargs, timeout)
     func().test_factory()
     # spawn server instance
     host, port = address
     server = await loop.create_server(func, host, port, 
         reuse_port=reuse_port, backlog=backlog, ssl=ssl)
+    # modify interface settings for sockets (when enabled)
+    if interface:
+        for sock in server.sockets:
+            modify_socket(sock, None, interface)
     # run server forever
     async with server:
         await server.serve_forever()
 
 def listen_udp_threaded(
     address:         RawAddr, 
     factory:         Type[Session],
     *args,
-    timeout:         Optional[int]   = None,
     interface:       Optional[bytes] = None,
     reuse_port:      bool            = False,
     allow_broadcast: bool            = False,
     **kwargs,
 ):
     """
     :param address:         host/port of server
@@ -107,20 +112,20 @@
     :param args:            positional args to pass to the session factory
     :param timeout:         max socket lifetime duration timeout if configured
     :param interface:       interface to bind server socket to
     :param reuse_port:      allow reuse of same port when enabled
     :param allow_broadcast: allow for udp broadcast messages when enabled
     :param kwargs:          keyword arguments to pass to session factory
     """
+    factory(*args, **kwargs)
     server = UdpThreadServer(
         address=address, 
         factory=factory, 
         args=args, 
         kwargs=kwargs, 
-        timeout=timeout, 
         interface=interface, 
         reuse_port=reuse_port, 
         allow_broadcast=allow_broadcast,
     )
     with server:
         server.serve_forever()
 
@@ -142,15 +147,15 @@
     :param timeout:         max socket lifetime duration timeout if configured
     :param interface:       interface to bind server socket to
     :param reuse_port:      allow reuse of same port when enabled
     :param backlog:         number of allowed and backloged async requests
     :param ssl:             TLS context to encrypt socket communications
     :param kwargs:          keyword arguments to pass to session factory
     """
-    factory.test_factory()
+    factory(*args, **kwargs)
     server = TcpThreadServer(
         address=address, 
         factory=factory, 
         args=args, 
         kwargs=kwargs, 
         timeout=timeout, 
         interface=interface,
```

### Comparing `pyserve3-0.0.3/pyserve/abc.py` & `pyserve3-0.0.4/pyserve/abc.py`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.3/pyserve/threading.py` & `pyserve3-0.0.4/pyserve/threading.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,31 +15,27 @@
 #** Functions **#
 
 def new_handler(
     base:      Type['BaseRequestHandler'],
     factory:   Type[Session],
     args:      tuple           = (),
     kwargs:    Dict[str, Any]  = {},
-    timeout:   Optional[int]   = None,
-    interface: Optional[bytes] = None,
     blocksize: int             = 8192
 ) -> Type['BaseRequestHandler']:
     """
     spawn new request-handler class w/ configured settings
     """
     # test factory generation
     factory(*args, **kwargs)
     # generate new request handler
     name = f'{base.__name__}Instance'
     return type(name, (base, ), dict(
         factory=factory,
         args=args,
         kwargs=kwargs,
-        timeout=timeout,
-        interface=interface,
         blocksize=blocksize,
     ))
 
 #** Classes **#
 
 @dataclass
 class UdpWriter(Writer):
@@ -72,25 +68,21 @@
     def is_closing(self) -> bool:
         return self.closing
 
 class BaseRequestHandler(socketserver.BaseRequestHandler):
     factory:   Type[Session]
     args:      tuple           
     kwargs:    Dict[str, Any]
-    timeout:   Optional[int]
-    interface: Optional[bytes]
     blocksize: int
 
     def setup(self):
         """configure and generate session w/ information collected"""
         self.addr:   Address = Address(*self.client_address)
-        self.sock:   socket.socket
         self.writer: Writer
         self.error:  Optional[Exception] = None
-        modify_socket(self.sock, self.timeout, self.interface)
         # spawn session object
         self.session = self.factory(*self.args, **self.kwargs)
         self.session.connection_made(self.addr, self.writer)
     
     def finish(self):
         """notify that connection disconnected"""
         self.session.connection_lost(self.error)
@@ -134,84 +126,101 @@
                 self.error = e
                 if not self.writer.closing:
                     self.writer.close()
                 break
 
 @dataclass
 class BaseThreadServer(socketserver.ThreadingMixIn):
-    server:    ClassVar[Type[socketserver.BaseServer]]
-    handler:   ClassVar[Type[BaseRequestHandler]]
+    handler: ClassVar[Type[BaseRequestHandler]]
 
     address:    RawAddr
     factory:    Type[Session]
     args:       tuple           = field(default_factory=tuple)
     kwargs:     Dict[str, Any]  = field(default_factory=dict)
-    timeout:    Optional[int]   = None
     interface:  Optional[bytes] = None
     reuse_port: bool            = False
-    
+    blocksize: int              = 8192
+ 
     def __post_init__(self):
+        self.max_packet_size  = self.blocksize
         self.allow_reuse_port = self.reuse_port
-        # build handler for base init
-        self.server.__init__(self, self.address, new_handler( #type: ignore
+
+    def new_handler(self) -> Type[BaseRequestHandler]:
+        return new_handler(
             base=self.handler, 
             factory=self.factory, 
             args=self.args, 
             kwargs=self.kwargs,
-            timeout=self.timeout,
-            interface=self.interface,
-            blocksize=getattr(self, 'blocksize', 8192),
-        ))
+            blocksize=self.blocksize,
+        )
 
-    def __exit__(self, *_):
-        """ensure server is shutdown properly"""
-        self.shutdown() #type: ignore
-    
-    def get_request(self):
-        """respawn socket after socket error to prevent infinite hanging loop"""
-        try:
-            return self.server.get_request(self) #type: ignore
-        except socket.error as e:
-            self.socket.close()
-            self.socket = socket.socket(self.address_family, self.socket_type) #type: ignore
-            self.server.server_bind(self) #type: ignore
-            raise e
+    def rebuild_socket(self, s: socketserver.BaseServer):
+        """rebuild socket to recover from socket failure"""
+        s.socket.close()
+        s.socket = socket.socket(s.address_family, s.socket_type)
+        s.server_bind()
 
 @dataclass
 class UdpThreadServer(BaseThreadServer, socketserver.UDPServer):
-    server  = socketserver.UDPServer
     handler = UdpHandler
 
     allow_broadcast: bool = False
 
-    def __post_init__(self):
-        super().__post_init__()
+    def __exit__(self, *_):
+        self.shutdown()
+
+    def server_bind(self):
+        """additional socket modification controls on server-bind"""
+        super().server_bind()
+        modify_socket(self.socket, None, self.interface)
         if self.allow_broadcast:
             self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
 
+    def get_request(self):
+        """respawn socket after socket error to prevent infinite hanging loop"""
+        try:
+            return super().get_request()
+        except socket.error as e:
+            self.rebuild_socket(self)
+            raise e
+
     def shutdown(self):
         """override shutdown behavior"""
-        self.server.shutdown(self)
+        super().shutdown()
         self.socket.close()
         self.server_close()
 
 @dataclass
 class TcpThreadServer(BaseThreadServer, socketserver.TCPServer):
-    server  = socketserver.TCPServer
     handler = TcpHandler
 
-    ssl:       Optional[SSLContext] = None
-    blocksize: int                  = 8192
-    
-    def __post_init__(self):
-        super().__post_init__()
+    ssl:     Optional[SSLContext] = None
+    timeout: Optional[int]        = None
+ 
+    def __exit__(self, *_):
+        self.shutdown()
+ 
+    def server_bind(self):
+        """additional socket modification controls on server-bind"""
+        super().server_bind()
+        modify_socket(self.socket, None, self.interface)
         if self.ssl:
             self.socket = wrap_socket(self.socket, server_side=True)
 
+    def get_request(self):
+        """respawn socket after socket error to prevent infinite hanging loop"""
+        try:
+            sock, addr = super().get_request()
+            modify_socket(sock, self.timeout, None)
+            return (sock, addr)
+        except socket.timeout as e:
+            raise e
+        except socket.error as e:
+            self.rebuild_socket(self)
+            raise e
+
     def shutdown(self):
         """override shutdown behavior"""
-        self.socket: socket.socket
-        self.server.shutdown(self)
+        super().shutdown()
         self.socket.shutdown(socket.SHUT_RDWR)
         self.socket.close()
         self.server_close()
-
```

### Comparing `pyserve3-0.0.3/pyserve/transport.py` & `pyserve3-0.0.4/pyserve/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 AsyncIO Implementations of session-based servers
 """
 import asyncio
 from dataclasses import dataclass, field
 from typing import Type, Optional, Dict, Any
 
-from .abc import RawAddr, Address, Writer, Session, modify_socket
+from .abc import RawAddr, Address, Writer, Session
 
 #** Variables **#
 __all__ = ['UdpProtocol', 'TcpProtocol']
 
 #** Classes **#
 
 @dataclass
@@ -27,16 +27,14 @@
         return self.transport.is_closing()
 
 @dataclass
 class BaseProtocol:
     factory:   Type[Session]
     args:      tuple           = field(default_factory=tuple)
     kwargs:    Dict[str, Any]  = field(default_factory=dict)
-    timeout:   Optional[int]   = None
-    interface: Optional[bytes] = None
 
     def test_factory(self):
         """validate session can be generated w/ args and kwargs"""
         self.factory(*self.args, **self.kwargs)
 
     def set_timeout(self, timeout: int, tport: asyncio.Transport):
         """implement timeout handling for async servers"""
@@ -49,43 +47,39 @@
         loop = asyncio.get_event_loop()
         loop.create_task(expire())
 
 class UdpProtocol(BaseProtocol, asyncio.DatagramTransport):
  
     def connection_made(self, transport: asyncio.DatagramTransport):
         """"""
-        self.transport = transport
         # handle modifying socket and making changes for handling
-        socket = transport.get_extra_info('socket')
-        modify_socket(socket, None, self.interface)
-        if self.timeout is not None:
-            self.set_timeout(self.timeout, transport) #pyright: ignore
-       
+        self.transport = transport
+ 
     def datagram_received(self, data: bytes, addr: RawAddr):
         """"""
         # generate session w/ attributes and notify on connection-made
         address      = Address(*addr)
         writer       = UdpWriter(address, self.transport)
         self.session = self.factory(*self.args, **self.kwargs)
         self.session.connection_made(address, writer)
         self.session.data_recieved(data)
 
     def connection_lost(self, err: Optional[Exception]):
         """"""
         self.session.connection_lost(err)
 
+@dataclass
 class TcpProtocol(BaseProtocol, asyncio.Protocol):
+    timeout: Optional[int] = None
    
     def connection_made(self, transport: asyncio.Transport):
         """"""
         # collect attributes and prepare socket for session
         address = Address(*transport.get_extra_info('peername'))
-        socket  = transport.get_extra_info('socket')
         # handle modifying socket and making changes for handling
-        modify_socket(socket, None, self.interface)
         if self.timeout is not None:
             self.set_timeout(self.timeout, transport)
         # generate session w/ attributes and notify on connection-made
         self.session = self.factory(*self.args, **self.kwargs)
         self.session.connection_made(address, transport)
 
     def data_received(self, data: bytes):
```

### Comparing `pyserve3-0.0.3/pyserve3.egg-info/PKG-INFO` & `pyserve3-0.0.4/pyserve3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserve3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unify SocketServer Implementations based on a Session Model
 Home-page: https://github.com/imgurbot12/pyserve
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyserve3-0.0.3/setup.py` & `pyserve3-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='pyserve3',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/pyserve',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description='Unify SocketServer Implementations based on a Session Model',
     python_requires='>=3.7',
```

