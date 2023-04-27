# Comparing `tmp/seedboxtools-1.6.2.tar.gz` & `tmp/seedboxtools-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedboxtools-1.6.2.tar", last modified: Wed Jul 27 15:11:19 2022, max compression
+gzip compressed data, was "seedboxtools-1.6.7.tar", last modified: Thu Apr 27 00:32:14 2023, max compression
```

## Comparing `seedboxtools-1.6.2.tar` & `seedboxtools-1.6.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.355627 seedboxtools-1.6.2/
--rw-rw-r--   0 user      (1000) user      (1000)      127 2022-07-27 12:19:35.000000 seedboxtools-1.6.2/BUGS
--rw-rw-r--   0 user      (1000) user      (1000)       86 2013-11-16 07:26:25.000000 seedboxtools-1.6.2/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     9622 2022-07-27 15:11:19.355627 seedboxtools-1.6.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     8674 2022-07-27 15:10:53.000000 seedboxtools-1.6.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.352627 seedboxtools-1.6.2/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)      156 2019-06-15 14:45:42.000000 seedboxtools-1.6.2/bin/configleecher
--rwxrwxr-x   0 user      (1000) user      (1000)      161 2019-06-15 14:45:42.000000 seedboxtools-1.6.2/bin/leechtorrents
--rwxrwxr-x   0 user      (1000) user      (1000)      144 2019-06-15 14:45:42.000000 seedboxtools-1.6.2/bin/uploadtorrents
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.353627 seedboxtools-1.6.2/default/
--rw-rw-r--   0 user      (1000) user      (1000)      307 2022-07-27 12:22:56.000000 seedboxtools-1.6.2/default/leechtorrents
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.353627 seedboxtools-1.6.2/desktop/
--rw-r--r--   0 user      (1000) user      (1000)      283 2013-11-16 07:24:51.000000 seedboxtools-1.6.2/desktop/uploadtorrents.desktop
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.353627 seedboxtools-1.6.2/doc/
--rw-rw-r--   0 user      (1000) user      (1000)     2556 2013-03-10 04:09:47.000000 seedboxtools-1.6.2/doc/bitcoin.png
--rw-rw-r--   0 user      (1000) user      (1000)       85 2022-07-27 12:07:41.000000 seedboxtools-1.6.2/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.353627 seedboxtools-1.6.2/service/
--rw-rw-r--   0 user      (1000) user      (1000)      511 2022-07-27 14:08:00.000000 seedboxtools-1.6.2/service/leechtorrents@.service
--rw-rw-r--   0 user      (1000) user      (1000)     1335 2022-07-27 15:11:19.356627 seedboxtools-1.6.2/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.351627 seedboxtools-1.6.2/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.354627 seedboxtools-1.6.2/src/seedboxtools/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2022-07-27 15:08:46.000000 seedboxtools-1.6.2/src/seedboxtools/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2016-10-09 10:36:10.000000 seedboxtools-1.6.2/src/seedboxtools/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)    18551 2022-07-27 11:50:51.000000 seedboxtools-1.6.2/src/seedboxtools/clients.py
--rw-rw-r--   0 user      (1000) user      (1000)     8104 2019-06-15 14:45:42.000000 seedboxtools-1.6.2/src/seedboxtools/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     9473 2022-07-27 12:56:21.000000 seedboxtools-1.6.2/src/seedboxtools/leecher.py
--rw-rw-r--   0 user      (1000) user      (1000)      174 2022-06-01 03:12:59.000000 seedboxtools-1.6.2/src/seedboxtools/test_util.py
--rw-rw-r--   0 user      (1000) user      (1000)     2021 2019-07-21 14:14:33.000000 seedboxtools-1.6.2/src/seedboxtools/uploader.py
--rw-rw-r--   0 user      (1000) user      (1000)     6793 2022-07-27 11:39:17.000000 seedboxtools-1.6.2/src/seedboxtools/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-07-27 15:11:19.355627 seedboxtools-1.6.2/src/seedboxtools.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     9622 2022-07-27 15:11:19.000000 seedboxtools-1.6.2/src/seedboxtools.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      625 2022-07-27 15:11:19.000000 seedboxtools-1.6.2/src/seedboxtools.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-07-27 15:11:19.000000 seedboxtools-1.6.2/src/seedboxtools.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       18 2022-07-27 15:11:19.000000 seedboxtools-1.6.2/src/seedboxtools.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       13 2022-07-27 15:11:19.000000 seedboxtools-1.6.2/src/seedboxtools.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.342000 seedboxtools-1.6.7/
+-rw-rw-r--   0 user      (1000) user      (1000)      127 2022-07-27 12:19:35.000000 seedboxtools-1.6.7/BUGS
+-rw-rw-r--   0 user      (1000) user      (1000)       86 2013-11-16 07:26:25.000000 seedboxtools-1.6.7/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     9622 2023-04-27 00:32:14.342000 seedboxtools-1.6.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     8674 2022-07-27 15:10:53.000000 seedboxtools-1.6.7/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.337000 seedboxtools-1.6.7/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)      156 2019-06-15 14:45:42.000000 seedboxtools-1.6.7/bin/configleecher
+-rwxrwxr-x   0 user      (1000) user      (1000)      161 2019-06-15 14:45:42.000000 seedboxtools-1.6.7/bin/leechtorrents
+-rwxrwxr-x   0 user      (1000) user      (1000)      144 2019-06-15 14:45:42.000000 seedboxtools-1.6.7/bin/uploadtorrents
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.337000 seedboxtools-1.6.7/default/
+-rw-rw-r--   0 user      (1000) user      (1000)      307 2022-07-27 12:22:56.000000 seedboxtools-1.6.7/default/leechtorrents
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.338000 seedboxtools-1.6.7/desktop/
+-rw-r--r--   0 user      (1000) user      (1000)      283 2013-11-16 07:24:51.000000 seedboxtools-1.6.7/desktop/uploadtorrents.desktop
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.338000 seedboxtools-1.6.7/doc/
+-rw-rw-r--   0 user      (1000) user      (1000)     2556 2013-03-10 04:09:47.000000 seedboxtools-1.6.7/doc/bitcoin.png
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2022-07-27 12:07:41.000000 seedboxtools-1.6.7/pyproject.toml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.338000 seedboxtools-1.6.7/service/
+-rw-rw-r--   0 user      (1000) user      (1000)      511 2022-07-27 14:08:00.000000 seedboxtools-1.6.7/service/leechtorrents@.service
+-rw-rw-r--   0 user      (1000) user      (1000)     1335 2023-04-27 00:32:14.342000 seedboxtools-1.6.7/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.335000 seedboxtools-1.6.7/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.341000 seedboxtools-1.6.7/src/seedboxtools/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-04-27 00:22:00.000000 seedboxtools-1.6.7/src/seedboxtools/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2016-10-09 10:36:10.000000 seedboxtools-1.6.7/src/seedboxtools/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-04-27 00:20:24.000000 seedboxtools-1.6.7/src/seedboxtools/clients.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8104 2019-06-15 14:45:42.000000 seedboxtools-1.6.7/src/seedboxtools/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9473 2022-07-27 12:56:21.000000 seedboxtools-1.6.7/src/seedboxtools/leecher.py
+-rw-rw-r--   0 user      (1000) user      (1000)      174 2022-06-01 03:12:59.000000 seedboxtools-1.6.7/src/seedboxtools/test_util.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2021 2019-07-21 14:14:33.000000 seedboxtools-1.6.7/src/seedboxtools/uploader.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6799 2022-07-29 21:46:16.000000 seedboxtools-1.6.7/src/seedboxtools/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-27 00:32:14.342000 seedboxtools-1.6.7/src/seedboxtools.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     9622 2023-04-27 00:32:14.000000 seedboxtools-1.6.7/src/seedboxtools.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      625 2023-04-27 00:32:14.000000 seedboxtools-1.6.7/src/seedboxtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-27 00:32:14.000000 seedboxtools-1.6.7/src/seedboxtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       18 2023-04-27 00:32:14.000000 seedboxtools-1.6.7/src/seedboxtools.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       13 2023-04-27 00:32:14.000000 seedboxtools-1.6.7/src/seedboxtools.egg-info/top_level.txt
```

### Comparing `seedboxtools-1.6.2/PKG-INFO` & `seedboxtools-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedboxtools
-Version: 1.6.2
+Version: 1.6.7
 Summary: A tool to automate downloading finished torrents from a seedbox
 Home-page: https://github.com/Rudd-O/seedboxtools
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 Keywords: seedbox,TorrentFlux,Transmission,PulsedMedia,torrents,download
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `seedboxtools-1.6.2/README.md` & `seedboxtools-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/doc/bitcoin.png` & `seedboxtools-1.6.7/doc/bitcoin.png`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/setup.cfg` & `seedboxtools-1.6.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/src/seedboxtools/cli.py` & `seedboxtools-1.6.7/src/seedboxtools/cli.py`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/src/seedboxtools/clients.py` & `seedboxtools-1.6.7/src/seedboxtools/clients.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Client classes for seedboxtools
 """
 
-from functools import partial
 import seedboxtools.util as util
 import re
 import os
 import requests
 import json
 import subprocess
+import xmlrpc.client
 
+from functools import partial
+from urllib.parse import quote
 
 # We must present some form of timeout or else the request can hang forever.
 # The documentation insists production code must specify it.
 def post(*args, **kwargs):
     if "timeout" not in kwargs:
         kwargs = dict(kwargs)
         kwargs["timeout"] = 15
@@ -299,14 +301,15 @@
         local_download_dir,
         hostname,
         login,
         password,
         ssh_hostname="",
         label="",
     ):
+        """Client for ruTorrent servers default in PulsedMedia seedboxes."""
         SeedboxClient.__init__(self, local_download_dir)
         self.hostname = hostname
         self.ssh_hostname = ssh_hostname or hostname
         self.login = login
         self.password = password
         self.label = label.strip()
 
@@ -331,15 +334,14 @@
 
     def get_finished_torrents(self):
         r = post(
             "https://%s/user-%s/rutorrent/plugins/httprpc/action.php"
             % (self.hostname, self.login),
             auth=(self.login, self.password),
             data="mode=list",
-            verify=False,
         )
         if r.status_code == 500:
             raise TemporaryMalfunction(
                 "Server returned a temporary 500 status code: %s" % r.content
             )
         if r.status_code == 404:
             raise Misconfiguration(
@@ -417,145 +419,62 @@
             return self._upload(files={"torrent_file": (n, tf)})
 
     def _upload(self, **params):
         r = post(
             "https://%s/user-%s/rutorrent/php/addtorrent.php"
             % (self.hostname, self.login),
             auth=(self.login, self.password),
-            verify=False,
             **params,
         )
         if r.status_code == 500:
             raise TemporaryMalfunction(
                 "Server returned a temporary 500 status code: %s" % r.text
             )
         if r.status_code == 404:
             raise Misconfiguration(
-                "Server address (%s) may be misconfigured: %s" % self.hostname
+                "Server address (%s) may be misconfigured: %s"
+                % (self.hostname, r.status_code)
             )
+
         if "addTorrentSuccess" in r.text:
             return
-        elif "addTorrentFailed" in r.text:
+
+        if "addTorrentFailed" in r.text:
             if "data" in params:
                 raise InvalidTorrent(params["data"]["url"])
-            else:
-                raise InvalidTorrent(params["files"]["torrent_file"][0])
-        else:
-            assert 0, (r.status_code, r.text)
+            raise InvalidTorrent(params["files"]["torrent_file"][0])
+
+        assert 0, (r.status_code, r.text)
 
     def remove_remote_download(self, filename):
         # in this implementation, get_finished_torrents MUST BE called first
         # or else this will bomb out with an attribute error
-        thehash = self.hash_for_filename_cache[filename]
-        payload_template = """<?xml version="1.0" encoding="UTF-8"?>
-<methodCall>
-  <methodName>system.multicall</methodName>
-  <params>
-    <param>
-      <value>
-        <array>
-          <data>
-            <value>
-              <struct>
-                <member>
-                  <name>methodName</name>
-                  <value>
-                    <string>d.set_custom5</string>
-                  </value>
-                </member>
-                <member>
-                  <name>params</name>
-                  <value>
-                    <array>
-                      <data>
-                        <value>
-                          <string>%s</string>
-                        </value>
-                        <value>
-                          <string>1</string>
-                        </value>
-                      </data>
-                    </array>
-                  </value>
-                </member>
-              </struct>
-            </value>
-            <value>
-              <struct>
-                <member>
-                  <name>methodName</name>
-                  <value>
-                    <string>d.delete_tied</string>
-                  </value>
-                </member>
-                <member>
-                  <name>params</name>
-                  <value>
-                    <array>
-                      <data>
-                        <value>
-                          <string>%s</string>
-                        </value>
-                      </data>
-                    </array>
-                  </value>
-                </member>
-              </struct>
-            </value>
-            <value>
-              <struct>
-                <member>
-                  <name>methodName</name>
-                  <value>
-                    <string>d.erase</string>
-                  </value>
-                </member>
-                <member>
-                  <name>params</name>
-                  <value>
-                    <array>
-                      <data>
-                        <value>
-                          <string>%s</string>
-                        </value>
-                      </data>
-                    </array>
-                  </value>
-                </member>
-              </struct>
-            </value>
-          </data>
-        </array>
-      </value>
-    </param>
-  </params>
-</methodCall>"""
-        payload = payload_template % (thehash, thehash, thehash)
-        headers = {"Content-Type": "text/xml; charset=UTF-8"}
-        r = post(
-            "https://%s/user-%s/rutorrent/plugins/httprpc/action.php"
-            % (self.hostname, self.login),
-            auth=(self.login, self.password),
-            data=payload,
-            verify=False,
-            headers=headers,
-        )
-        if r.status_code == 500:
-            raise TemporaryMalfunction(
-                "Server returned a temporary 500 status code: %s" % r.content
-            )
-        if r.status_code == 404:
+        login = quote(self.login, safe="")
+        passw = quote(self.password, safe="")
+        url = (
+            f"https://{login}:{passw}@{self.hostname}/user-{login}"
+            + "/rutorrent/plugins/httprpc/action.php"
+        )
+        client = xmlrpc.client.ServerProxy(url)
+        infohash = self.hash_for_filename_cache[filename]
+        mcall = xmlrpc.client.MultiCall(client)
+        mcall.d.custom5.set(infohash, "1")
+        mcall.d.delete_tied(infohash)
+        mcall.d.erase(infohash)
+        try:
+            _, delete_tied_result, erase_result = list(mcall())
+        except xmlrpc.client.ProtocolError as exc:
             raise Misconfiguration(
-                "Server address (%s) may be misconfigured: %s" % self.hostname
-            )
-        assert r.status_code == 200, (
-            "Non-OK status code while retrieving get_finished_torrents: %r"
-            % r.status_code
-        )
-        _ = r.text
+                f"Server address ({self.hostname}) may be misconfigured"
+            ) from exc
+        except xmlrpc.client.Fault as exc:
+            raise TemporaryMalfunction("Server returned a fault.") from exc
+
+        assert delete_tied_result == 0, f"Delete tied result {delete_tied_result}"
+        assert erase_result == 0, f"Erase result {erase_result}"
 
 
 clients = {
     "TransmissionClient": TransmissionClient,
     "TorrentFluxClient": TorrentFluxClient,
     "PulsedMedia": PulsedMediaClient,
 }
```

### Comparing `seedboxtools-1.6.2/src/seedboxtools/config.py` & `seedboxtools-1.6.7/src/seedboxtools/config.py`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/src/seedboxtools/leecher.py` & `seedboxtools-1.6.7/src/seedboxtools/leecher.py`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/src/seedboxtools/uploader.py` & `seedboxtools-1.6.7/src/seedboxtools/uploader.py`

 * *Files identical despite different names*

### Comparing `seedboxtools-1.6.2/src/seedboxtools/util.py` & `seedboxtools-1.6.7/src/seedboxtools/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 def passthru(cmdline: list[str]) -> int:
     return call(cmdline)  # return status code, pass the outputs thru
 
 
 def rsync(source: str, destination: str) -> int:
-    RSYNC_OPTS = ["-rtlDvzP", "--chmod=go+rX --chmod=u+rwX --executability"]
+    RSYNC_OPTS = ["-rtlDvzP", "--chmod=go+rX", "--chmod=u+rwX", "--executability"]
     cmdline = ["rsync"] + RSYNC_OPTS + ["--", source, destination]
     return passthru(cmdline)
 
 
 def quote_cmdline(cmdline):
     """Quote a command line in list form for SSH usage"""
     return " ".join(shell_quote(x) for x in cmdline)
```

### Comparing `seedboxtools-1.6.2/src/seedboxtools.egg-info/PKG-INFO` & `seedboxtools-1.6.7/src/seedboxtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedboxtools
-Version: 1.6.2
+Version: 1.6.7
 Summary: A tool to automate downloading finished torrents from a seedbox
 Home-page: https://github.com/Rudd-O/seedboxtools
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 Keywords: seedbox,TorrentFlux,Transmission,PulsedMedia,torrents,download
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `seedboxtools-1.6.2/src/seedboxtools.egg-info/SOURCES.txt` & `seedboxtools-1.6.7/src/seedboxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

