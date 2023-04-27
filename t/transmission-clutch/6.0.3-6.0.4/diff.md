# Comparing `tmp/transmission-clutch-6.0.3.tar.gz` & `tmp/transmission_clutch-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission-clutch-6.0.3.tar", max compression
+gzip compressed data, was "transmission_clutch-6.0.4.tar", max compression
```

## Comparing `transmission-clutch-6.0.3.tar` & `transmission_clutch-6.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1070 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/LICENSE
--rw-r--r--   0        0        0     1900 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/README.rst
--rw-r--r--   0        0        0       27 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/clutch/__init__.py
--rw-r--r--   0        0        0     1650 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/client.py
--rw-r--r--   0        0        0      132 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/compat.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/method/__init__.py
--rw-r--r--   0        0        0      448 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/method/method.py
--rw-r--r--   0        0        0     1112 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/method/misc.py
--rw-r--r--   0        0        0      662 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/method/queue.py
--rw-r--r--   0        0        0     1819 2021-10-03 15:25:41.575131 transmission-clutch-6.0.3/clutch/method/session.py
--rw-r--r--   0        0        0      277 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/method/shared.py
--rw-r--r--   0        0        0     4319 2021-10-03 15:25:41.575131 transmission-clutch-6.0.3/clutch/method/torrent.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/__init__.py
--rw-r--r--   0        0        0     1062 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/connection.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/rpc/__init__.py
--rw-r--r--   0        0        0     2096 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/rpc/convert.py
--rw-r--r--   0        0        0      691 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/rpc/message.py
--rw-r--r--   0        0        0     2142 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/session.py
--rw-r--r--   0        0        0      682 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/network/utility.py
--rw-r--r--   0        0        0        0 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/clutch/py.typed
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/schema/__init__.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission-clutch-6.0.3/clutch/schema/request/__init__.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/request/session/__init__.py
--rw-r--r--   0        0        0     2119 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/clutch/schema/request/session/accessor.py
--rw-r--r--   0        0        0     3940 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/request/session/mutator.py
--rw-r--r--   0        0        0      741 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/request/session/shared.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/request/torrent/__init__.py
--rw-r--r--   0        0        0     2440 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/clutch/schema/request/torrent/accessor.py
--rw-r--r--   0        0        0     1508 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/request/torrent/add.py
--rw-r--r--   0        0        0     2161 2021-10-03 15:25:41.575131 transmission-clutch-6.0.3/clutch/schema/request/torrent/mutator.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/__init__.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/__init__.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/session/__init__.py
--rw-r--r--   0        0        0     1293 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/session/accessor.py
--rw-r--r--   0        0        0     1368 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/session/mutator.py
--rw-r--r--   0        0        0      556 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/session/shared.py
--rw-r--r--   0        0        0      179 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/clutch/schema/user/method/shared.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/__init__.py
--rw-r--r--   0        0        0     3275 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/accessor.py
--rw-r--r--   0        0        0      231 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/action.py
--rw-r--r--   0        0        0      744 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/add.py
--rw-r--r--   0        0        0      260 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/move.py
--rw-r--r--   0        0        0     1061 2020-10-14 14:06:14.792631 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/mutator.py
--rw-r--r--   0        0        0      261 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/remove.py
--rw-r--r--   0        0        0      178 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/method/torrent/rename.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/response/__init__.py
--rw-r--r--   0        0        0      224 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/response/misc.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/response/session/__init__.py
--rw-r--r--   0        0        0     2782 2021-10-03 15:25:41.575131 transmission-clutch-6.0.3/clutch/schema/user/response/session/accessor.py
--rw-r--r--   0        0        0      390 2020-10-14 13:41:21.070363 transmission-clutch-6.0.3/clutch/schema/user/response/session/stats.py
--rw-r--r--   0        0        0        0 2020-10-14 13:41:21.074363 transmission-clutch-6.0.3/clutch/schema/user/response/torrent/__init__.py
--rw-r--r--   0        0        0     4540 2021-10-03 15:13:54.032694 transmission-clutch-6.0.3/clutch/schema/user/response/torrent/accessor.py
--rw-r--r--   0        0        0      613 2020-10-14 13:41:21.074363 transmission-clutch-6.0.3/clutch/schema/user/response/torrent/add.py
--rw-r--r--   0        0        0      105 2020-10-14 13:41:21.074363 transmission-clutch-6.0.3/clutch/schema/user/response/torrent/rename.py
--rw-r--r--   0        0        0      682 2021-10-03 15:25:41.575131 transmission-clutch-6.0.3/pyproject.toml
--rw-r--r--   0        0        0     3207 2021-10-03 15:34:21.283064 transmission-clutch-6.0.3/setup.py
--rw-r--r--   0        0        0     2733 2021-10-03 15:34:21.283299 transmission-clutch-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/LICENSE
+-rw-r--r--   0        0        0     1900 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/README.rst
+-rw-r--r--   0        0        0       27 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/clutch/__init__.py
+-rw-r--r--   0        0        0     1649 2023-04-27 16:35:02.063017 transmission_clutch-6.0.4/clutch/client.py
+-rw-r--r--   0        0        0      132 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/compat.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/method/__init__.py
+-rw-r--r--   0        0        0      448 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/method/method.py
+-rw-r--r--   0        0        0     1112 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/method/misc.py
+-rw-r--r--   0        0        0      662 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/method/queue.py
+-rw-r--r--   0        0        0     1819 2021-10-03 15:25:41.575131 transmission_clutch-6.0.4/clutch/method/session.py
+-rw-r--r--   0        0        0      277 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/method/shared.py
+-rw-r--r--   0        0        0     4319 2021-10-03 15:25:41.575131 transmission_clutch-6.0.4/clutch/method/torrent.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/__init__.py
+-rw-r--r--   0        0        0     1062 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/connection.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/rpc/__init__.py
+-rw-r--r--   0        0        0     2096 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/rpc/convert.py
+-rw-r--r--   0        0        0      691 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/rpc/message.py
+-rw-r--r--   0        0        0     2142 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/session.py
+-rw-r--r--   0        0        0      682 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/network/utility.py
+-rw-r--r--   0        0        0        0 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/clutch/py.typed
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/schema/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.066363 transmission_clutch-6.0.4/clutch/schema/request/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/request/session/__init__.py
+-rw-r--r--   0        0        0     2119 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/clutch/schema/request/session/accessor.py
+-rw-r--r--   0        0        0     3940 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/request/session/mutator.py
+-rw-r--r--   0        0        0      741 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/request/session/shared.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/request/torrent/__init__.py
+-rw-r--r--   0        0        0     2440 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/clutch/schema/request/torrent/accessor.py
+-rw-r--r--   0        0        0     1508 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/request/torrent/add.py
+-rw-r--r--   0        0        0     2161 2023-04-27 14:00:00.620041 transmission_clutch-6.0.4/clutch/schema/request/torrent/mutator.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/session/__init__.py
+-rw-r--r--   0        0        0     1293 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/session/accessor.py
+-rw-r--r--   0        0        0     1368 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/session/mutator.py
+-rw-r--r--   0        0        0      556 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/session/shared.py
+-rw-r--r--   0        0        0      179 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/clutch/schema/user/method/shared.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/__init__.py
+-rw-r--r--   0        0        0     3275 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/accessor.py
+-rw-r--r--   0        0        0      231 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/action.py
+-rw-r--r--   0        0        0      744 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/add.py
+-rw-r--r--   0        0        0      260 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/move.py
+-rw-r--r--   0        0        0     1061 2023-04-27 14:00:00.620041 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/mutator.py
+-rw-r--r--   0        0        0      261 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/remove.py
+-rw-r--r--   0        0        0      178 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/method/torrent/rename.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/response/__init__.py
+-rw-r--r--   0        0        0      224 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/response/misc.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/response/session/__init__.py
+-rw-r--r--   0        0        0     2782 2021-10-03 15:25:41.575131 transmission_clutch-6.0.4/clutch/schema/user/response/session/accessor.py
+-rw-r--r--   0        0        0      390 2020-10-14 13:41:21.070363 transmission_clutch-6.0.4/clutch/schema/user/response/session/stats.py
+-rw-r--r--   0        0        0        0 2020-10-14 13:41:21.074363 transmission_clutch-6.0.4/clutch/schema/user/response/torrent/__init__.py
+-rw-r--r--   0        0        0     4540 2021-10-03 15:13:54.032694 transmission_clutch-6.0.4/clutch/schema/user/response/torrent/accessor.py
+-rw-r--r--   0        0        0      613 2020-10-14 13:41:21.074363 transmission_clutch-6.0.4/clutch/schema/user/response/torrent/add.py
+-rw-r--r--   0        0        0      105 2020-10-14 13:41:21.074363 transmission_clutch-6.0.4/clutch/schema/user/response/torrent/rename.py
+-rw-r--r--   0        0        0      756 2023-04-27 16:35:00.031031 transmission_clutch-6.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 transmission_clutch-6.0.4/setup.py
+-rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 transmission_clutch-6.0.4/PKG-INFO
```

### Comparing `transmission-clutch-6.0.3/LICENSE` & `transmission_clutch-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/README.rst` & `transmission_clutch-6.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/client.py` & `transmission_clutch-6.0.4/clutch/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from clutch.method.torrent import TorrentMethods
 from clutch.network.connection import Connection
 from clutch.network.session import TransmissionSession
 from clutch.network.utility import make_endpoint
 
 
 class Client:
-
     session: SessionMethods = SessionMethods()
     torrent: TorrentMethods = TorrentMethods()
     queue: QueueMethods = QueueMethods()
     misc: MiscellaneousMethods = MiscellaneousMethods()
 
     def __init__(
         self,
```

### Comparing `transmission-clutch-6.0.3/clutch/method/misc.py` & `transmission_clutch-6.0.4/clutch/method/misc.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/method/queue.py` & `transmission_clutch-6.0.4/clutch/method/queue.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/method/session.py` & `transmission_clutch-6.0.4/clutch/method/session.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/method/torrent.py` & `transmission_clutch-6.0.4/clutch/method/torrent.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/network/connection.py` & `transmission_clutch-6.0.4/clutch/network/connection.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/network/rpc/convert.py` & `transmission_clutch-6.0.4/clutch/network/rpc/convert.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/network/rpc/message.py` & `transmission_clutch-6.0.4/clutch/network/rpc/message.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/network/session.py` & `transmission_clutch-6.0.4/clutch/network/session.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/network/utility.py` & `transmission_clutch-6.0.4/clutch/network/utility.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/request/session/accessor.py` & `transmission_clutch-6.0.4/clutch/schema/request/session/accessor.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/request/session/mutator.py` & `transmission_clutch-6.0.4/clutch/schema/request/session/mutator.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/request/session/shared.py` & `transmission_clutch-6.0.4/clutch/schema/request/session/shared.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/request/torrent/accessor.py` & `transmission_clutch-6.0.4/clutch/schema/request/torrent/accessor.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/request/torrent/add.py` & `transmission_clutch-6.0.4/clutch/schema/request/torrent/add.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/request/torrent/mutator.py` & `transmission_clutch-6.0.4/clutch/schema/request/torrent/mutator.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 
 class TorrentMutatorArgumentsRequest(BaseModel):
     bandwidth_priority: Optional[int] = Field(None, alias="bandwidthPriority")
     download_limit: Optional[int] = Field(None, alias="downloadLimit")
     download_limited: Optional[bool] = Field(None, alias="downloadLimited")
     edit_date: Optional[int] = Field(None, alias="editDate")
-    files_wanted: Optional[Sequence[str]] = Field(None, alias="files-wanted")
-    files_unwanted: Optional[Sequence[str]] = Field(None, alias="file-unwanted")
+    files_wanted: Optional[Sequence[int]] = Field(None, alias="files-wanted")
+    files_unwanted: Optional[Sequence[int]] = Field(None, alias="file-unwanted")
     honors_session_limits: Optional[bool] = Field(None, alias="honorsSessionLimits")
     ids: Optional[IdsArg]
     labels: Optional[Sequence[str]]
     location: Optional[str]
     peer_limit: Optional[int] = Field(None, alias="peer-limit")
-    priority_high: Optional[Sequence[str]] = Field(None, alias="priority-high")
-    priority_low: Optional[Sequence[str]] = Field(None, alias="priority-low")
-    priority_normal: Optional[Sequence[str]] = Field(None, alias="priority-normal")
+    priority_high: Optional[Sequence[int]] = Field(None, alias="priority-high")
+    priority_low: Optional[Sequence[int]] = Field(None, alias="priority-low")
+    priority_normal: Optional[Sequence[int]] = Field(None, alias="priority-normal")
     queue_position: Optional[int] = Field(None, alias="queuePosition")
     seed_idle_limit: Optional[int] = Field(None, alias="seedIdleLimit")
     seed_idle_mode: Optional[int] = Field(None, alias="seedIdleMode")
     seed_ratio_limit: Optional[float] = Field(None, alias="seedRatioLimit")
     seed_ratio_mode: Optional[int] = Field(None, alias="seedRatioMode")
     tracker_add: Optional[Sequence[str]] = Field(None, alias="trackerAdd")
     tracker_remove: Optional[Sequence[int]] = Field(None, alias="trackerRemove")
```

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/method/session/accessor.py` & `transmission_clutch-6.0.4/clutch/schema/user/method/session/accessor.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/method/session/mutator.py` & `transmission_clutch-6.0.4/clutch/schema/user/method/session/mutator.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/method/session/shared.py` & `transmission_clutch-6.0.4/clutch/schema/user/method/session/shared.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/method/torrent/accessor.py` & `transmission_clutch-6.0.4/clutch/schema/user/method/torrent/accessor.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/method/torrent/add.py` & `transmission_clutch-6.0.4/clutch/schema/user/method/torrent/add.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/method/torrent/mutator.py` & `transmission_clutch-6.0.4/clutch/schema/user/method/torrent/mutator.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 
 class TorrentMutatorArguments(TypedDict, total=False):
     bandwidth_priority: int
     download_limit: int
     download_limited: bool
     edit_date: int
-    files_wanted: Sequence[str]  # empty is shorthand for all
-    files_unwanted: Sequence[str]  # empty is shorthand for all
+    files_wanted: Sequence[int]  # empty is shorthand for all
+    files_unwanted: Sequence[int]  # empty is shorthand for all
     honors_session_limits: bool
     ids: IdsArg
     labels: Sequence[str]
     location: str
     peer_limit: int
-    priority_high: Sequence[str]  # empty is shorthand for all
-    priority_low: Sequence[str]  # empty is shorthand for all
-    priority_normal: Sequence[str]  # empty is shorthand for all
+    priority_high: Sequence[int]  # empty is shorthand for all
+    priority_low: Sequence[int]  # empty is shorthand for all
+    priority_normal: Sequence[int]  # empty is shorthand for all
     queue_position: int
     seed_idle_limit: int
     seed_idle_mode: int
     seed_ratio_limit: float
     seed_ratio_mode: int
     tracker_add: Sequence[str]
     tracker_remove: Sequence[int]
```

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/response/session/accessor.py` & `transmission_clutch-6.0.4/clutch/schema/user/response/session/accessor.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/response/torrent/accessor.py` & `transmission_clutch-6.0.4/clutch/schema/user/response/torrent/accessor.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/clutch/schema/user/response/torrent/add.py` & `transmission_clutch-6.0.4/clutch/schema/user/response/torrent/add.py`

 * *Files identical despite different names*

### Comparing `transmission-clutch-6.0.3/pyproject.toml` & `transmission_clutch-6.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "transmission-clutch"
-version = "6.0.3"
+version = "6.0.4"
 description = "An RPC client library for the Transmission BitTorrent client"
 authors = ["mhadam <michael@hadam.us>"]
 repository = "https://github.com/mhadam/clutch"
 documentation = "https://clutch.readthedocs.io/en/latest/"
 readme = "README.rst"
 license = "MIT"
 packages = [{ include = "clutch" }]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = "^2.22.0"
 pydantic = "^1.4"
 typing-extensions = {version = "^3.7.4", python = "3.7"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^4.6"
 mypy = "^0.761"
 sphinx-autodoc-typehints = "^1.12.0"
 
+[tool.poetry.group.dev.dependencies]
+sphinx = "^6.2.1"
+black = "^23.3.0"
+
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `transmission-clutch-6.0.3/setup.py` & `transmission_clutch-6.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 ['pydantic>=1.4,<2.0', 'requests>=2.22.0,<3.0.0']
 
 extras_require = \
 {':python_version == "3.7"': ['typing-extensions>=3.7.4,<4.0.0']}
 
 setup_kwargs = {
     'name': 'transmission-clutch',
-    'version': '6.0.3',
+    'version': '6.0.4',
     'description': 'An RPC client library for the Transmission BitTorrent client',
     'long_description': 'Clutch\n------\n\n.. image:: https://readthedocs.org/projects/clutch/badge/?version=latest\n    :target: https://clutch.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation badge\n\n.. image:: https://img.shields.io/pypi/v/transmission-clutch.svg\n    :target: https://pypi.org/project/transmission-clutch\n    :alt: PyPI badge\n\n.. image:: https://img.shields.io/pypi/pyversions/transmission-clutch.svg\n    :target: https://pypi.org/project/transmission-clutch\n    :alt: PyPI versions badge\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/ambv/black\n    :alt: Black formatter badge\n\n.. image:: https://img.shields.io/pypi/l/transmission-clutch.svg\n    :target: https://en.wikipedia.org/wiki/MIT_License\n    :alt: License badge\n\n.. image:: https://img.shields.io/pypi/dm/transmission-clutch.svg\n    :target: https://pypistats.org/packages/transmission-clutch\n    :alt: PyPI downloads badge\n\nSupport\n=======\nbtc: bc1q9spjh7nuqatz4pa7dscd0357p3ql588tla6af7\n\nDocumentation\n=============\n\nFound here: `<https://clutch.readthedocs.io>`_\n\nQuick start\n===========\n\nInstall the package:\n\n.. code-block:: console\n\n    $ pip install transmission-clutch\n\nMake a client:\n\n.. code-block:: python\n\n    from clutch import Client\n    client = Client()\n\nIf you find the client isn\'t connecting (an error will be raised), make sure you\'re entering the address correctly. Reference `urllib.parse.urlparse`_ for parsing rules.\n\nYou can specify Transmission\'s address when making the client:\n\n.. code-block:: python\n\n    client = Client(address="http://localhost:9091/transmission/rpc")\n\n.. _urllib.parse.urlparse: https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse\n\nRPC methods are separated into groups: torrent, session, queue and misc.\n\nMethods are called by first specifying a group:\n\n.. code-block:: python\n\n    client.torrent.add(...)\n',
     'author': 'mhadam',
     'author_email': 'michael@hadam.us',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mhadam/clutch',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `transmission-clutch-6.0.3/PKG-INFO` & `transmission_clutch-6.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: transmission-clutch
-Version: 6.0.3
+Version: 6.0.4
 Summary: An RPC client library for the Transmission BitTorrent client
 Home-page: https://github.com/mhadam/clutch
 License: MIT
 Author: mhadam
 Author-email: michael@hadam.us
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.4,<2.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
-Requires-Dist: typing-extensions (>=3.7.4,<4.0.0); python_version == "3.7"
+Requires-Dist: typing-extensions (>=3.7.4,<4.0.0) ; python_version == "3.7"
 Project-URL: Documentation, https://clutch.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/mhadam/clutch
 Description-Content-Type: text/x-rst
 
 Clutch
 ------
```

