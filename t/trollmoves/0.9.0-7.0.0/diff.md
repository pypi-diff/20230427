# Comparing `tmp/trollmoves-0.9.0.tar.gz` & `tmp/trollmoves-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trollmoves-0.9.0.tar", last modified: Fri Dec  3 12:53:59 2021, max compression
+gzip compressed data, was "trollmoves-7.0.0.tar", last modified: Wed Aug 25 09:19:48 2021, max compression
```

## Comparing `trollmoves-0.9.0.tar` & `trollmoves-7.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 12:53:59.126397 trollmoves-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-03 12:53:58.000000 trollmoves-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-12-03 12:53:59.126397 trollmoves-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-03 12:53:58.000000 trollmoves-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 12:53:59.126397 trollmoves-0.9.0/bin/
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2021-12-03 12:53:58.000000 trollmoves-0.9.0/bin/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    21448 2021-12-03 12:53:58.000000 trollmoves-0.9.0/bin/move_it.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2021-12-03 12:53:58.000000 trollmoves-0.9.0/bin/move_it_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2021-12-03 12:53:58.000000 trollmoves-0.9.0/bin/move_it_mirror.py
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2021-12-03 12:53:58.000000 trollmoves-0.9.0/bin/move_it_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     8947 2021-12-03 12:53:58.000000 trollmoves-0.9.0/bin/remove_it.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2021-12-03 12:53:59.126397 trollmoves-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2021-12-03 12:53:58.000000 trollmoves-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 12:53:59.126397 trollmoves-0.9.0/trollmoves/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34709 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    20417 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/heartbeat_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6547 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/mirror.py
--rw-r--r--   0 runner    (1001) docker     (121)     7443 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/move_it_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    15479 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/movers.py
--rw-r--r--   0 runner    (1001) docker     (121)    29800 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2021-12-03 12:53:58.000000 trollmoves-0.9.0/trollmoves/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-12-03 12:53:59.126397 trollmoves-0.9.0/trollmoves/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 12:53:59.126397 trollmoves-0.9.0/trollmoves.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-12-03 12:53:59.000000 trollmoves-0.9.0/trollmoves.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-12-03 12:53:59.000000 trollmoves-0.9.0/trollmoves.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-03 12:53:59.000000 trollmoves-0.9.0/trollmoves.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-03 12:53:59.000000 trollmoves-0.9.0/trollmoves.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-12-03 12:53:59.000000 trollmoves-0.9.0/trollmoves.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-03 12:53:59.000000 trollmoves-0.9.0/trollmoves.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-12-03 12:53:58.000000 trollmoves-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 09:19:48.184271 trollmoves-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-08-25 09:19:47.000000 trollmoves-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-08-25 09:19:48.184271 trollmoves-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-08-25 09:19:47.000000 trollmoves-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 09:19:48.184271 trollmoves-7.0.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2021-08-25 09:19:47.000000 trollmoves-7.0.0/bin/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21499 2021-08-25 09:19:47.000000 trollmoves-7.0.0/bin/move_it.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-08-25 09:19:47.000000 trollmoves-7.0.0/bin/move_it_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5713 2021-08-25 09:19:47.000000 trollmoves-7.0.0/bin/move_it_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-08-25 09:19:47.000000 trollmoves-7.0.0/bin/move_it_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8947 2021-08-25 09:19:47.000000 trollmoves-7.0.0/bin/remove_it.py
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2021-08-25 09:19:48.188271 trollmoves-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2021-08-25 09:19:47.000000 trollmoves-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 09:19:48.188271 trollmoves-7.0.0/trollmoves/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33245 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19610 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3702 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/heartbeat_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2327 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5098 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/move_it_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15539 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/movers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30215 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-08-25 09:19:47.000000 trollmoves-7.0.0/trollmoves/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-08-25 09:19:48.188271 trollmoves-7.0.0/trollmoves/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 09:19:48.184271 trollmoves-7.0.0/trollmoves.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-08-25 09:19:48.000000 trollmoves-7.0.0/trollmoves.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2021-08-25 09:19:48.000000 trollmoves-7.0.0/trollmoves.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 09:19:48.000000 trollmoves-7.0.0/trollmoves.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 09:19:48.000000 trollmoves-7.0.0/trollmoves.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-08-25 09:19:48.000000 trollmoves-7.0.0/trollmoves.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-25 09:19:48.000000 trollmoves-7.0.0/trollmoves.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-08-25 09:19:47.000000 trollmoves-7.0.0/versioneer.py
```

### Comparing `trollmoves-0.9.0/PKG-INFO` & `trollmoves-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: trollmoves
-Version: 0.9.0
+Version: 7.0.0
 Summary: Pytroll file utilities
 Home-page: https://github.com/pytroll/trollmoves
 Author: Martin Raspaud
 Author-email: martin.raspaud@smhi.se
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `trollmoves-0.9.0/bin/dispatcher.py` & `trollmoves-7.0.0/bin/dispatcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 
     formatter = logging.Formatter(LOG_FORMAT)
     fh_.setFormatter(formatter)
 
     root.addHandler(fh_)
 
 
-def parse_args():
-    """Parse commandline arguments."""
+def main():
+    """Start and run the dispatcher."""
     parser = argparse.ArgumentParser()
     parser.add_argument("config_file",
                         help="The configuration file to run on.")
     parser.add_argument("-l", "--log",
                         help="The file to log to. stdout otherwise.")
     parser.add_argument("-c", "--log-config",
                         help="Log config file to use instead of the standard logging.")
@@ -89,20 +89,15 @@
         "-p", "--publish-port", type=int, dest="pub_port", nargs='?',
         const=0, default=None,
         help="Publish messages for dispatched files on this port. "
         "Default: no publishing.")
     parser.add_argument("-n", "--publish-nameserver", nargs='*',
                         dest="pub_nameservers",
                         help="Nameserver for publisher to connect to")
-    return parser.parse_args()
-
-
-def main():
-    """Start and run the dispatcher."""
-    cmd_args = parse_args()
+    cmd_args = parser.parse_args()
     setup_logging(cmd_args)
     logger.info("Starting up.")
 
     try:
         dispatcher = Dispatcher(cmd_args.config_file,
                                 publish_port=cmd_args.pub_port,
                                 publish_nameservers=cmd_args.pub_nameservers)
```

### Comparing `trollmoves-0.9.0/bin/move_it.py` & `trollmoves-7.0.0/bin/move_it.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,43 +120,45 @@
 
 When the script is launched, or when a section is added or updated, existing
 files matching the pattern defined in `origin` are touched in order to create a
 triggering of the chain on them. To avoid any race conditions, chain is
 executed tree seconds after the list of file is gathered.
 """
 
+import bz2
 import fnmatch
 import glob
 import logging
 import logging.handlers
 import os
 import shutil
 import subprocess
 import sys
 import time
-from configparser import RawConfigParser
-from urllib.parse import urlparse, urlunparse
+from six.moves.configparser import RawConfigParser
+from ftplib import FTP, all_errors
+from six.moves.urllib.parse import urlparse, urlunparse
 import argparse
 import signal
 
-import bz2
-from ftplib import FTP, all_errors
 import pyinotify
+
 from trollsift import globify, parse
+
+LOGGER = logging.getLogger("move_it")
+LOG_FORMAT = "[%(asctime)s %(levelname)-8s] %(message)s"
+
 # messaging is optional
 try:
     from posttroll.publisher import NoisyPublisher
     from posttroll.message import Message
 except ImportError:
     print("\nNOTICE! Import of posttroll failed, "
           "messaging will not be used.\n")
 
-LOGGER = logging.getLogger("move_it")
-LOG_FORMAT = "[%(asctime)s %(levelname)-8s] %(message)s"
-
 
 chains = {}
 
 # Config management
 
 
 def read_config(filename):
@@ -342,15 +344,16 @@
 def xrit(pathname, destination=None, cmd="./xRITDecompress"):
     """Unpacks xrit data.
     """
     opath, ofile = os.path.split(pathname)
     destination = destination or "/tmp/"
     dest_url = urlparse(destination)
     if dest_url.scheme in ("", "file"):
-        _ = check_output([cmd, pathname], cwd=(destination or opath))
+        res = check_output([cmd, pathname], cwd=(destination or opath))
+        del res
     else:
         LOGGER.exception("Can not extract file %s to %s, destination has to be local.",
                          pathname, destination)
     LOGGER.info("Successfully extracted %s to %s", pathname,
                 destination)
     return os.path.join((destination or opath), ofile[:-2] + "__")
 
@@ -388,23 +391,23 @@
     """
     err = None
     for dest in destinations:
         LOGGER.debug("Copying to: %s", dest)
         dest_url = urlparse(dest)
         try:
             mover = MOVERS[dest_url.scheme]
-        except KeyError:
+        except KeyError as err:
             LOGGER.error("Unsupported protocol '%s'. Could not copy %s to %s",
                          str(dest_url.scheme), pathname, str(dest))
             continue
         try:
             mover(pathname, dest_url).copy()
             if hook:
                 hook(pathname, dest_url)
-        except Exception:
+        except Exception as err:
             LOGGER.exception("Something went wrong during copy of %s to %s",
                              pathname, str(dest))
             continue
         else:
             LOGGER.info("Successfully copied %s to %s", pathname,
                         str(dest))
 
@@ -554,24 +557,24 @@
                     if "prog" in attrs:
                         new_path = unpack_fun(pathname,
                                               attrs["working_directory"],
                                               attrs["prog"])
                     else:
                         new_path = unpack_fun(pathname,
                                               attrs["working_directory"])
-                except Exception:
+                except:
                     LOGGER.exception("Could not decompress %s", pathname)
                     return
 
             else:
                 new_path = pathname
             try:
                 move_it(new_path, attrs["destinations"],
                         attrs.get("copy_hook", None))
-            except Exception:
+            except Exception as err:
                 LOGGER.error("Something went wrong during copy of %s",
                              pathname)
             else:
                 if attrs["delete"]:
                     try:
                         os.remove(pathname)
                         if attrs["delete_hook"]:
```

### Comparing `trollmoves-0.9.0/bin/move_it_client.py` & `trollmoves-7.0.0/bin/move_it_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,65 +78,74 @@
 # TODO: implement ping and server selection
 import logging
 import logging.handlers
 import argparse
 import signal
 import time
 
+from posttroll.publisher import NoisyPublisher
 from trollmoves.move_it_base import MoveItBase
+from trollmoves.client import StatCollector
 
 LOGGER = logging.getLogger("move_it_client")
 LOG_FORMAT = "[%(asctime)s %(levelname)-8s %(name)s] %(message)s"
 
 
 class MoveItClient(MoveItBase):
     """Trollmoves client class."""
 
     def __init__(self, cmd_args):
         """Initialize client."""
         super(MoveItClient, self).__init__(cmd_args, "client")
+        self._np = NoisyPublisher("move_it_client")
+        self.sync_publisher = self._np.start()
+        self.setup_watchers(cmd_args)
 
     def run(self):
         """Start the transfer chains."""
         signal.signal(signal.SIGTERM, self.chains_stop)
         signal.signal(signal.SIGHUP, self.signal_reload_cfg_file)
         self.notifier.start()
         self.running = True
         while self.running:
             time.sleep(1)
+            self.sync_publisher.heartbeat(30)
             for chain_name in self.chains:
                 if not self.chains[chain_name].is_alive():
                     self.chains[chain_name] = self.chains[chain_name].restart()
-                self.chains[chain_name].publisher.heartbeat(30)
 
 
 def parse_args():
     """Parse commandline arguments."""
     parser = argparse.ArgumentParser()
     parser.add_argument("config_file",
                         help="The configuration file to run on.")
     parser.add_argument("-l", "--log",
                         help="The file to log to. stdout otherwise.")
+    parser.add_argument("-s", "--stats",
+                        help="Save stats to this file")
     parser.add_argument("-v", "--verbose", default=False, action="store_true",
                         help="Toggle verbose logging")
     return parser.parse_args()
 
 
 def main():
     """Run the Trollmoves Client."""
     cmd_args = parse_args()
     client = MoveItClient(cmd_args)
 
     try:
-        client.reload_cfg_file(cmd_args.config_file)
+        if cmd_args.stats:
+            stat = StatCollector(cmd_args.stats)
+            client.reload_cfg_file(cmd_args.config_file, callback=stat.collect)
+        else:
+            client.reload_cfg_file(cmd_args.config_file)
         client.run()
     except KeyboardInterrupt:
         LOGGER.debug("Interrupting")
-    except Exception as err:
-        LOGGER.exception(err)
     finally:
         if client.running:
             client.chains_stop()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `trollmoves-0.9.0/bin/move_it_server.py` & `trollmoves-7.0.0/bin/move_it_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,20 +91,41 @@
 
   move_it_server --log /path/to/mylogfile.log myconfig.ini
 """
 
 import logging
 import logging.handlers
 import argparse
-from trollmoves.server import MoveItServer
+import signal
+import time
+from trollmoves.move_it_base import MoveItBase, create_publisher
 
 LOGGER = logging.getLogger("move_it_server")
 LOG_FORMAT = "[%(asctime)s %(levelname)-8s %(name)s] %(message)s"
 
 
+class MoveItServer(MoveItBase):
+    """Wrapper class for Trollmoves Server."""
+
+    def __init__(self, cmd_args):
+        """Initialize server."""
+        publisher = create_publisher(cmd_args.port, "move_it_server")
+        super(MoveItServer, self).__init__(cmd_args, "server", publisher=publisher)
+
+    def run(self):
+        """Start the transfer chains."""
+        signal.signal(signal.SIGTERM, self.chains_stop)
+        signal.signal(signal.SIGHUP, self.signal_reload_cfg_file)
+        self.notifier.start()
+        self.running = True
+        while self.running:
+            time.sleep(1)
+            self.sync_publisher.heartbeat(30)
+
+
 def parse_args():
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser()
     parser.add_argument("config_file",
                         help="The configuration file to run on.")
     parser.add_argument("-l", "--log",
                         help="The file to log to. stdout otherwise.")
```

### Comparing `trollmoves-0.9.0/bin/remove_it.py` & `trollmoves-7.0.0/bin/remove_it.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Remove files, and send messages about it."""
 
-from configparser import RawConfigParser, NoOptionError
+from six.moves.configparser import RawConfigParser, NoOptionError
 from datetime import datetime, timedelta
 from glob import glob
 import os
 import time
 import argparse
 import logging
 import logging.handlers
@@ -78,15 +78,15 @@
                 msg = "From: %s\r\nTo: %s\r\nSubject: %s\r\n\r\n" % (
                     self.fromaddr, ",".join(self.toaddrs), self.subject)
                 for record in self.buffer:
                     s = self.format(record)
                     msg = msg + s + "\r\n"
                 smtp.sendmail(self.fromaddr, self.toaddrs, msg)
                 smtp.quit()
-            except Exception:
+            except:
                 self.handleError(None)  # no particular record
             self.buffer = []
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("configuration_file",
```

### Comparing `trollmoves-0.9.0/setup.py` & `trollmoves-7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `trollmoves-0.9.0/trollmoves/client.py` & `trollmoves-7.0.0/trollmoves/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 """Trollmoves client."""
 
 import logging
 import os
 import socket
 import sys
 import time
+import tarfile
 from collections import deque
-from configparser import RawConfigParser
+from six.moves.configparser import RawConfigParser
 from threading import Lock, Thread, Event
 import hashlib
-from urllib.parse import urlparse, urlunparse
+import six
+from six.moves.urllib.parse import urlparse, urlunparse
 import subprocess
 from contextlib import suppress
-
-import tarfile
+import pyinotify
 from zmq import LINGER, POLLIN, REQ, Poller
 import bz2
+
 from posttroll import get_context
 from posttroll.message import Message, MessageError
 from posttroll.publisher import NoisyPublisher
 from posttroll.subscriber import Subscriber
 from trollsift.parser import compose
 
 from trollmoves import heartbeat_monitor
@@ -57,130 +59,108 @@
 ongoing_transfers = dict()
 ongoing_transfers_lock = Lock()
 hot_spare_timer_lock = Lock()
 ongoing_hot_spare_timers = dict()
 
 DEFAULT_REQ_TIMEOUT = 1
 SERVER_HEARTBEAT_TOPIC = "/heartbeat/move_it_server"
-CLIENT_HEARTBEAT_TOPIC_BASE = "/heartbeat/move_it"
 
 COMPRESSED_ENDINGS = {'xrit': ['C_'],
                       'tar': ['.tar', '.tar.gz', '.tgz', '.tar.bz2'],
                       'bzip': ['.bz2'],
                       }
 BUNZIP_BLOCK_SIZE = 1024
 LISTENER_CHECK_INTERVAL = 1
 
 
+# Config management
 def read_config(filename):
     """Read the config file called *filename*."""
     cp_ = RawConfigParser()
     cp_.read(filename)
 
     res = {}
 
     for section in cp_.sections():
         res[section] = dict(cp_.items(section))
-        _set_config_defaults(res[section])
-        _parse_boolean_config_items(res[section])
-        if not _check_provider_config(res, section):
+        res[section].setdefault("delete", False)
+        if res[section]["delete"] in ["", "False", "false", "0", "off"]:
+            res[section]["delete"] = False
+        if res[section]["delete"] in ["True", "true", "on", "1"]:
+            res[section]["delete"] = True
+        res[section].setdefault("working_directory", None)
+        res[section].setdefault("compression", False)
+        res[section].setdefault("xritdecompressor", None)
+        res[section].setdefault("heartbeat", True)
+        res[section].setdefault("req_timeout", DEFAULT_REQ_TIMEOUT)
+        res[section].setdefault("transfer_req_timeout", 10 * DEFAULT_REQ_TIMEOUT)
+        res[section].setdefault("nameservers", None)
+        if res[section]["heartbeat"] in ["", "False", "false", "0", "off"]:
+            res[section]["heartbeat"] = False
+
+        if "providers" not in res[section]:
+            LOGGER.warning("Incomplete section %s: add an 'providers' item.",
+                           section)
+            LOGGER.info("Ignoring section %s: incomplete.",
+                        section)
+            del res[section]
             continue
-        if not _check_destination(res, section):
+        else:
+            res[section]["providers"] = [
+                "tcp://" + item.split('/', 1)[0] for item in res[section]["providers"].split()
+            ]
+
+        if "destination" not in res[section]:
+            LOGGER.warning("Incomplete section %s: add an 'destination' item.",
+                           section)
+            LOGGER.info("Ignoring section %s: incomplete.", section)
+            del res[section]
             continue
-        if not _check_subscribing(res, section):
+
+        if "topic" in res[section]:
+            try:
+                res[section]["publish_port"] = int(res[section][
+                    "publish_port"])
+            except (KeyError, ValueError):
+                res[section]["publish_port"] = 0
+        elif not res[section]["heartbeat"]:
+            # We have no topics and therefor no subscriber (if you want to
+            # subscribe everything, then explicit specify an empty topic).
+            LOGGER.warning("Incomplete section %s: add an 'topic' "
+                           "item or enable heartbeat.", section)
+            LOGGER.info("Ignoring section %s: incomplete.", section)
+            del res[section]
             continue
 
     return res
 
 
-def _set_config_defaults(conf):
-    conf.setdefault("delete", False)
-    conf.setdefault("working_directory", None)
-    conf.setdefault("compression", False)
-    conf.setdefault("xritdecompressor", None)
-    conf.setdefault("heartbeat", True)
-    conf.setdefault("req_timeout", DEFAULT_REQ_TIMEOUT)
-    conf.setdefault("transfer_req_timeout", 10 * DEFAULT_REQ_TIMEOUT)
-    conf.setdefault("nameservers", None)
-
-
-def _parse_boolean_config_items(conf):
-    if conf["delete"] in ["", "False", "false", "0", "off"]:
-        conf["delete"] = False
-    if conf["delete"] in ["True", "true", "on", "1"]:
-        conf["delete"] = True
-    if conf["heartbeat"] in ["", "False", "false", "0", "off"]:
-        conf["heartbeat"] = False
-
-
-def _check_provider_config(conf, section):
-    if "providers" not in conf[section]:
-        LOGGER.warning("Incomplete section %s: add an 'providers' item.",
-                       section)
-        LOGGER.info("Ignoring section %s: incomplete.",
-                    section)
-        del conf[section]
-        return False
-
-    conf[section]["providers"] = [
-        "tcp://" + item.split('/', 1)[0] for item in conf[section]["providers"].split()
-    ]
-    return True
-
-
-def _check_subscribing(res, section):
-    if "topic" in res[section]:
-        try:
-            res[section]["publish_port"] = int(res[section][
-                "publish_port"])
-        except (KeyError, ValueError):
-            res[section]["publish_port"] = 0
-    elif not res[section]["heartbeat"]:
-        # We have no topics and therefor no subscriber (if you want to
-        # subscribe everything, then explicit specify an empty topic).
-        LOGGER.warning("Incomplete section %s: add an 'topic' "
-                       "item or enable heartbeat.", section)
-        LOGGER.info("Ignoring section %s: incomplete.", section)
-        del res[section]
-        return False
-    return True
-
-
-def _check_destination(res, section):
-    if "destination" not in res[section]:
-        LOGGER.warning("Incomplete section %s: add an 'destination' item.",
-                       section)
-        LOGGER.info("Ignoring section %s: incomplete.", section)
-        del res[section]
-        return False
-    return True
-
-
 class Listener(Thread):
     """PyTroll listener class for reading messages for Trollduction."""
 
-    def __init__(self, address, topics, *args, die_event=None, **kwargs):
+    def __init__(self, address, topics, callback, *args, die_event=None, **kwargs):
         """Init Listener object."""
         super(Listener, self).__init__()
 
         self.topics = topics
+        self.callback = callback
         self.subscriber = None
         self.address = address
         self.running = False
         self.die_event = die_event
         self.cargs = args
         self.ckwargs = kwargs
         self.restart_event = Event()
         self.cause_of_death = None
         self.death_count = 0
 
     def restart(self):
         """Restart the listener, returns a new running instance."""
         self.stop()
-        new_listener = self.__class__(self.address, self.topics, *self.cargs,
+        new_listener = self.__class__(self.address, self.topics, self.callback, *self.cargs,
                                       die_event=self.die_event, **self.ckwargs)
         new_listener.death_count = self.death_count + 1
         new_listener.start()
         return new_listener
 
     def create_subscriber(self):
         """Create a subscriber using specified addresses and message types."""
@@ -191,114 +171,85 @@
                 self.subscriber = Subscriber(self.address, self.topics)
                 LOGGER.debug("Subscriber %s", str(self.subscriber))
 
     def run(self):
         """Run listener."""
         try:
             with heartbeat_monitor.Monitor(self.restart_event, **self.ckwargs) as beat_monitor:
+
                 self.running = True
+
                 while self.running:
+                    # Loop for restart.
+
                     LOGGER.debug("Starting listener %s", str(self.address))
                     self.create_subscriber()
-                    self._get_messages(beat_monitor)
-        except Exception as err:
-            LOGGER.exception("Listener died.")
-            self.cause_of_death = err
-            with suppress(AttributeError):
-                self.die_event.set()
-
-    def _get_messages(self, beat_monitor):
-        for msg in self.subscriber(timeout=1):
-            if not self.running:
-                break
-            if not self._check_heartbeat():
-                break
-            if msg is None:
-                continue
 
-            LOGGER.debug("Receiving (SUB) %s", str(msg))
-
-            beat_monitor(msg)
+                    for msg in self.subscriber(timeout=1):
+                        if not self.running:
+                            break
 
-            if self._is_message_already_handled(msg):
-                continue
+                        # If the heartbeat didn't arrive, restart the subscriber
+                        if self.restart_event.is_set():
+                            LOGGER.warning("Missing a heartbeat, restarting the subscriber to %s.",
+                                           str(self.subscriber.addresses))
+                            self.restart_event.clear()
+                            self.stop()
+                            self.running = True
+                            break
 
-            self._process_message(msg)
+                        if msg is None:
+                            continue
 
-        LOGGER.debug("Exiting listener %s", str(self.address))
+                        LOGGER.debug("Receiving (SUB) %s", str(msg))
 
-    def _check_heartbeat(self):
-        if self.restart_event.is_set():
-            LOGGER.warning("Missing a heartbeat, restarting the subscriber to %s.",
-                           str(self.subscriber.addresses))
-            self.restart_event.clear()
-            self.stop()
-            self.running = True
-            return False
-        return True
+                        beat_monitor(msg)
+                        if msg.type == "beat":
+                            self.death_count = 0
+                            continue
+                        # Handle public "push" messages as a hot spare client
+                        if msg.type == "push":
+                            # TODO: these need to be checked and acted if
+                            # the transfers are not finished on primary
+                            # client and are not cleared
+                            LOGGER.debug("Primary client published 'push'")
+                            add_to_ongoing(msg)
+
+                        # Handle public "ack" messages as a hot spare client
+                        if msg.type == "ack":
+                            LOGGER.debug("Primary client finished transfer")
+                            _ = add_to_file_cache(msg)
+                            _ = clean_ongoing_transfer(get_msg_uid(msg))
+
+                        # If this is a hot spare client, wait for a while
+                        # for a public "push" message which will update
+                        # the ongoing transfers before starting processing here
+                        delay = self.ckwargs.get("processing_delay", False)
+                        if delay:
+                            add_timer(float(delay), self.callback, msg, *self.cargs,
+                                      **self.ckwargs)
+                        else:
+                            self.callback(msg, *self.cargs, **self.ckwargs)
 
-    def _is_message_already_handled(self, msg):
-        return (self._handle_beat_message(msg) or _handle_push_message(msg) or
-                _handle_ack_message(msg) or _handle_message_from_another_client(msg))
-
-    def _handle_beat_message(self, msg):
-        if msg.type == "beat":
-            self.death_count = 0
-            return True
-        return False
-
-    def _process_message(self, msg):
-        delay = self.ckwargs.get("processing_delay", False)
-        if delay:
-            # If this is a hot spare client, wait for a while
-            # for a public "push" message which will update
-            # the ongoing transfers before starting processing here
-            add_request_push_timer(float(delay), msg, *self.cargs, **self.ckwargs)
-        else:
-            request_push(msg, *self.cargs, **self.ckwargs)
+                    LOGGER.debug("Exiting listener %s", str(self.address))
+        except Exception as err:
+            LOGGER.exception("Listener died.")
+            self.cause_of_death = err
+            with suppress(AttributeError):
+                self.die_event.set()
 
     def stop(self):
         """Stop subscriber and delete the instance."""
         self.running = False
         time.sleep(1)
         if self.subscriber is not None:
             self.subscriber.close()
             self.subscriber = None
 
 
-def _handle_push_message(msg):
-    if msg.type == "push":
-        # TODO: these need to be checked and acted if
-        # the transfers are not finished on primary
-        # client and are not cleared
-        LOGGER.debug("Primary client published 'push'")
-        add_to_ongoing(msg)
-        return True
-    return False
-
-
-def _handle_ack_message(msg):
-    if msg.type == "ack":
-        LOGGER.debug("Primary client finished transfer")
-        _ = add_to_file_cache(msg)
-        _ = clean_ongoing_transfer(get_msg_uid(msg))
-        return True
-    return False
-
-
-def _handle_message_from_another_client(msg):
-    if msg.type == "file" and "request_address" not in msg.data:
-        LOGGER.debug("Ignoring 'file' message from primary client.")
-        add_to_ongoing(msg)
-        _ = add_to_file_cache(msg)
-        _ = clean_ongoing_transfer(get_msg_uid(msg))
-        return True
-    return False
-
-
 def clean_ongoing_transfer(uid):
     """Clear transfer for the given UID from the cache."""
     with ongoing_transfers_lock:
         msgs = ongoing_transfers.pop(uid, [])
         LOGGER.debug("Remove uid %s: %s", uid, str(msgs))
     return msgs
 
@@ -484,23 +435,20 @@
         var['uri'] = urlunparse((scheme_, host_, path, "", "", ""))
         return var
     msg.data = translate_dict(msg.data, ('uri', 'uid'), uri_callback)
     return msg
 
 
 def replace_mda(msg, kwargs):
-    """Replace messate metadata with items in kwargs dict."""
+    """Replace messate metadata with itmes in kwargs dict."""
     for key in msg.data:
         if key in kwargs:
-            try:
-                replacement = dict(item.split(':') for item in kwargs[key].split('|'))
-                replacement = replacement[msg.data[key]]
-            except ValueError:
-                replacement = kwargs[key]
-            msg.data[key] = replacement
+            replacement = dict(item.split(':')
+                               for item in kwargs[key].split('|'))
+            msg.data[key] = replacement[msg.data[key]]
     return msg
 
 
 def send_request(msg, req, timeout):
     """Send a request for push."""
     LOGGER.debug("Send and recv timeout is %.2f seconds", timeout)
 
@@ -551,20 +499,20 @@
 
 def get_next_msg(uid):
     """Get the next message with this *uid* from the available sources."""
     with ongoing_transfers_lock:
         return ongoing_transfers[uid].pop(0)
 
 
-def add_request_push_timer(timeout, msg, *args, **kwargs):
+def add_timer(timeout, callback, msg, *args, **kwargs):
     """Add a timer for hot spare."""
     huid = get_msg_uid(msg)
     cargs = [msg] + list(args)
     with hot_spare_timer_lock:
-        timer = CTimer(timeout, request_push, args=cargs, kwargs=kwargs)
+        timer = CTimer(timeout, callback, args=cargs, kwargs=kwargs)
         ongoing_hot_spare_timers[huid] = timer
         ongoing_hot_spare_timers[huid].start()
     LOGGER.debug("Added timer for UID %s.", huid)
 
 
 def add_to_ongoing(msg):
     """Add message to ongoing transfers.
@@ -590,146 +538,121 @@
     with cache_lock:
         for uid in gen_dict_extract(msg.data, 'uid'):
             if uid not in file_cache:
                 LOGGER.debug("Add %s to file cache", str(uid))
                 file_cache.append(uid)
 
 
-def request_push(msg_in, destination, login=None, publisher=None, **kwargs):
+def request_push(msg_in, destination, login=None, sync_publisher=None, publisher=None, **kwargs):
     """Request a push for data."""
     huid = add_to_ongoing(msg_in)
     if huid is None:
         return
 
     if already_received(msg_in):
         timeout = float(kwargs["req_timeout"])
         send_ack(msg_in, timeout)
         _ = clean_ongoing_transfer(huid)
         return
 
-    _request_files(huid, destination, login, publisher, **kwargs)
-
-
-def _request_files(huid, destination, login, publisher, **kwargs):
     for msg in iterate_messages(huid):
-        _destination = _compose_destination(destination, msg)
-
+        try:
+            _destination = compose(destination, msg.data)
+        except KeyError as ke:
+            LOGGER.error("Format identifier is missing from the msg.data: %s", str(ke))
+            raise
+        except ValueError as ve:
+            LOGGER.error("Type of format identifier doesn't match the type in m msg.data: %s", str(ve))
+            raise
+        except AttributeError as ae:
+            LOGGER.error("msg or msg.data is None: %s", str(ae))
+            raise
         req, fake_req = create_push_req_message(msg, _destination, login)
         LOGGER.info("Requesting: %s", str(fake_req))
+        timeout = float(kwargs["transfer_req_timeout"])
         local_dir = create_local_dir(_destination, kwargs.get('ftp_root', '/'))
 
-        publisher.send(str(fake_req))
-
-        response, hostname = send_request(msg, req, float(kwargs["transfer_req_timeout"]))
+        if sync_publisher:
+            sync_publisher.send(str(fake_req))
+        response, hostname = send_request(msg, req, timeout)
 
         if response and response.type in ['file', 'collection', 'dataset']:
             LOGGER.debug("Server done sending file")
             add_to_file_cache(msg)
-            _send_ack_message(msg, publisher)
-
+            if sync_publisher:
+                # Send an 'ack' message so that possible hot spares know
+                # the primary has completed the request
+                msg = Message(msg.subject, 'ack', msg.data)
+                LOGGER.debug("Sending a public 'ack' of completed transfer: %s",
+                             str(msg))
+                sync_publisher.send(str(msg))
             try:
-                lmsg = unpack_and_create_local_message(response, local_dir, **kwargs)
-                lmsg = _update_local_message(lmsg, _destination, login, response, **kwargs)
+                lmsg = unpack_and_create_local_message(response, local_dir,
+                                                       **kwargs)
             except IOError:
                 LOGGER.exception("Couldn't unpack %s", str(response))
                 continue
+            if publisher:
+                lmsg = make_uris(lmsg, _destination, login)
+                lmsg.data['origin'] = response.data['request_address']
+                lmsg.data.pop('request_address', None)
+                lmsg = replace_mda(lmsg, kwargs)
+                lmsg.data.pop('destination', None)
 
-            LOGGER.debug("publishing %s", str(lmsg))
-            publisher.send(str(lmsg))
+                LOGGER.debug("publishing %s", str(lmsg))
+                publisher.send(str(lmsg))
             terminate_transfers(huid, float(kwargs["req_timeout"]))
             break
         else:
             LOGGER.error("Failed to get valid response from server %s: %s",
                          str(hostname), str(response))
     else:
         LOGGER.warning('Could not get a working source for requesting %s',
                        str(msg))
         terminate_transfers(huid, float(kwargs["req_timeout"]))
 
 
-def _compose_destination(destination, msg):
-    try:
-        _destination = compose(destination, msg.data)
-    except KeyError as ke:
-        LOGGER.error("Format identifier is missing from the msg.data: %s", str(ke))
-        raise
-    except ValueError as ve:
-        LOGGER.error("Type of format identifier doesn't match the type in m msg.data: %s", str(ve))
-        raise
-    except AttributeError as ae:
-        LOGGER.error("msg or msg.data is None: %s", str(ae))
-        raise
-    return _destination
-
-
-def _send_ack_message(msg, publisher):
-    """Send an 'ack' message.
-
-    This is for the possible hot spare clients so they know the primary has completed the request.
-    """
-    msg = Message(msg.subject, 'ack', msg.data)
-    LOGGER.debug("Sending a public 'ack' of completed transfer: %s", str(msg))
-    publisher.send(str(msg))
-
-
-def _update_local_message(lmsg, _destination, login, response, **kwargs):
-    lmsg = make_uris(lmsg, _destination, login)
-    lmsg.data['origin'] = response.data['request_address']
-    lmsg.data.pop('request_address', None)
-    lmsg = replace_mda(lmsg, kwargs)
-    lmsg.data.pop('destination', None)
-
-    return lmsg
-
-
 class Chain(Thread):
     """The Chain class."""
 
     def __init__(self, name, config):
         """Init a chain object."""
         super(Chain, self).__init__()
         self._config = config
         self._name = name
-        self._np = None
         self.publisher = None
         self.listeners = {}
         self.listener_died_event = Event()
         self.running = True
-        self.setup_publisher()
+        self.sync_publisher = None
 
-    def setup_publisher(self):
-        """Initialize publisher."""
-        if self._np is None:
-            try:
-                nameservers = self._config["nameservers"]
-                if nameservers:
-                    nameservers = nameservers.split()
-                self._np = NoisyPublisher(
-                    "move_it_" + self._name,
-                    port=self._config["publish_port"],
-                    nameservers=nameservers)
-                self.publisher = self._np.start()
-            except (KeyError, NameError):
-                pass
+        # Setup publisher
+        try:
+            nameservers = self._config["nameservers"]
+            if nameservers:
+                nameservers = nameservers.split()
+            self.publisher = NoisyPublisher(
+                "move_it_" + self._name,
+                port=self._config["publish_port"],
+                nameservers=nameservers)
+            self.publisher.start()
+        except (KeyError, NameError):
+            pass
 
-    def setup_listeners(self, keep_providers=None):
+    def setup_listeners(self, callback, sync_publisher):
         """Set up the listeners."""
-        keep_providers = keep_providers or []
+        self.callback = callback
+        self.sync_publisher = sync_publisher
         try:
             topics = []
             if "topic" in self._config:
                 topics.append(self._config["topic"])
             if self._config.get("heartbeat", False):
                 topics.append(SERVER_HEARTBEAT_TOPIC)
-                # Subscribe also to heartbeat messages of other clients
-                topics.append(CLIENT_HEARTBEAT_TOPIC_BASE + '_' + self._name)
             for provider in self._config["providers"]:
-                if provider in keep_providers and provider in self.listeners:
-                    LOGGER.debug("Not restarting Listener to %s, config not changed.", provider)
-                    continue
                 if '/' in provider.split(':')[-1]:
                     parts = urlparse(provider)
                     if parts.scheme != '':
                         provider = urlunparse((parts.scheme, parts.netloc,
                                                '', '', '', ''))
                     else:
                         # If there's no scheme, urlparse thinks the
@@ -738,14 +661,16 @@
                                                '', '', '', ''))
                     topics.append(parts.path)
                 LOGGER.debug("Add listener for %s with topic %s",
                              provider, str(topics))
                 listener = Listener(
                     provider,
                     topics,
+                    callback,
+                    sync_publisher=sync_publisher,
                     publisher=self.publisher,
                     die_event=self.listener_died_event,
                     **self._config)
                 listener.start()
                 self.listeners[provider] = listener
         except Exception as err:
             LOGGER.exception(str(err))
@@ -789,97 +714,58 @@
         for key, val in other_config.items():
             if ((key not in ["listeners", "publisher"]) and
                 ((key not in self._config) or
                     (self._config[key] != val))):
                 return False
         return True
 
-    def get_unchanged_providers(self, other_config):
-        """Get a list of providers that have not changed between this and other config."""
-        if self._config["topic"] != other_config["topic"]:
-            return []
-        return list(set(self._config["providers"]).intersection(set(other_config["providers"])))
-
-    def publisher_needs_restarting(self, other_config):
-        """Check that current config is the same as `other_config`."""
-        for key in ["nameservers", "publish_port"]:
-            if self._config[key] != other_config[key]:
-                return True
-        return False
-
-    def refresh(self, new_config):
-        """Refresh the chain with new config."""
-        publisher_needs_restarting = self.publisher_needs_restarting(new_config)
-        unchanged_providers = self.get_unchanged_providers(new_config)
-        self._config = new_config
-        if publisher_needs_restarting:
-            self._refresh_publisher()
-        self._refresh_listeners(unchanged_providers)
-        if not self.running:
-            self.start()
-
-    def _refresh_publisher(self):
-        self._stop_publisher()
-        self.setup_publisher()
-
-    def _refresh_listeners(self, unchanged_providers):
-        self.reset_listeners(keep_providers=unchanged_providers)
-        self.setup_listeners(keep_providers=unchanged_providers)
-
-    def reset_listeners(self, keep_providers=None):
+    def reset_listeners(self):
         """Reset the listeners."""
-        keep_providers = keep_providers or []
-        kept_listeners = {}
-        for key, listener in self.listeners.items():
-            if key in keep_providers:
-                kept_listeners[key] = listener
-                continue
+        for listener in self.listeners.values():
             listener.stop()
-        self.listeners = kept_listeners
+        self.listeners = {}
 
     def stop(self):
         """Stop the chain."""
-        self._stop_publisher()
         self.running = False
+        if self.publisher:
+            self.publisher.stop()
         self.reset_listeners()
 
-    def _stop_publisher(self):
-        if self._np:
-            self._np.stop()
-            self._np = None
-
     def restart(self):
         """Restart the chain, return a new running instance."""
         self.stop()
         new_chain = self.__class__(self._name, self._config)
-        new_chain.setup_listeners()
+        new_chain.setup_listeners(self.callback, self.sync_publisher)
         new_chain.start()
         return new_chain
 
 
-def reload_config(filename, chains):
+def reload_config(filename, chains, callback=request_push, sync_publisher=None):
     """Rebuild chains if needed (if the configuration changed) from *filename*."""
     LOGGER.debug("New config file detected: %s", filename)
 
     new_configs = read_config(filename)
 
     # setup new chains
+
     for key, new_config in new_configs.items():
         if key in chains:
             if chains[key].config_equals(new_config):
                 continue
+
+            chains[key].stop()
             verb = "Updated"
             LOGGER.debug("Updating %s", key)
         else:
             verb = "Added"
             LOGGER.debug("Adding %s", key)
-            chains[key] = Chain(key, new_config)
-            chains[key].start()
-
-        chains[key].refresh(new_config)
+        chains[key] = Chain(key, new_config)
+        chains[key].setup_listeners(callback, sync_publisher)
+        chains[key].start()
 
         LOGGER.debug("%s %s", verb, key)
 
     # disable old chains
 
     for key in (set(chains.keys()) - set(new_configs.keys())):
         chains[key].stop()
@@ -978,17 +864,57 @@
                 LOGGER.info("Reconnecting and resending %s", str(msg))
                 # Create new connection
                 self.connect()
                 self._socket.send_string(request)
 
         return rep
 
+# Generic event handler
+
+
+class EventHandler(pyinotify.ProcessEvent):
+    """Handle events with a generic *fun* function."""
+
+    def __init__(self, fun, *args, **kwargs):
+        """Initialize handler."""
+        pyinotify.ProcessEvent.__init__(self, *args, **kwargs)
+        self._fun = fun
+
+    def process_IN_CLOSE_WRITE(self, event):
+        """Process on closing after writing."""
+        self._fun(event.pathname)
+
+    def process_IN_CREATE(self, event):
+        """Process on closing after linking."""
+        try:
+            if os.stat(event.pathname).st_nlink > 1:
+                self._fun(event.pathname)
+        except OSError:
+            return
+
+    def process_IN_MOVED_TO(self, event):
+        """Process on closing after moving."""
+        self._fun(event.pathname)
+
+
+class StatCollector(object):
+    """StatCollector class."""
+
+    def __init__(self, statfile):
+        """Initialize collector."""
+        self.statfile = statfile
+
+    def collect(self, msg, *args, **kwargs):
+        """Collect."""
+        with open(self.statfile, 'a') as fd:
+            fd.write(time.asctime() + " - " + str(msg) + "\n")
+
 
 def terminate(chains):
     """Terminate client chains."""
-    for chain in chains.values():
+    for chain in six.itervalues(chains):
         chain.stop()
     LOGGER.info("Shutting down.")
     print("Thank you for using pytroll/move_it_client."
           " See you soon on pytroll.org!")
     time.sleep(1)
     sys.exit(0)
```

### Comparing `trollmoves-0.9.0/trollmoves/dispatcher.py` & `trollmoves-7.0.0/trollmoves/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,49 +151,49 @@
 """
 
 import logging
 import os
 import signal
 from queue import Empty
 from threading import Thread
-from urllib.parse import urlsplit, urlunsplit, urlparse
-import socket
 
 import yaml
+
 import inotify.adapters
 from inotify.constants import IN_MODIFY, IN_CLOSE_WRITE, IN_CREATE, IN_MOVED_TO
+from six.moves.urllib.parse import urlsplit, urlunsplit, urlparse
+import socket
 from posttroll.listener import ListenerContainer
 from posttroll.publisher import NoisyPublisher
 from posttroll.message import Message
-from trollsift import compose
-
 from trollmoves.movers import move_it
 from trollmoves.utils import (clean_url, is_file_local)
+from trollsift import compose
 
 logger = logging.getLogger(__name__)
 
 INOTIFY_MASK = IN_MODIFY | IN_CLOSE_WRITE | IN_CREATE | IN_MOVED_TO
 
 
 class Notifier(Thread):
     """Class to handle file notifications."""
 
     def __init__(self, filename, event_types, callback):
         """Initialize the notifier."""
         self.filename = filename
         self.loop = True
-        self.inotify = inotify.adapters.Inotify()
-        self.inotify.add_watch(filename, mask=INOTIFY_MASK)
+        self.i = inotify.adapters.Inotify()
+        self.i.add_watch(filename, mask=INOTIFY_MASK)
         self.event_types = set(event_types)
         self.callback = callback
         super().__init__()
 
     def run(self):
         """Run the notifier."""
-        for event in self.inotify.event_gen():
+        for event in self.i.event_gen():
             if event is None:
                 if not self.loop:
                     logger.info('Terminating watch on %s', self.filename)
                     return
                 else:
                     continue
             (_, type_names, path, filename) = event
@@ -263,148 +263,150 @@
     def __init__(self, config_file, publish_port=None,
                  publish_nameservers=None):
         """Initialize dispatcher class."""
         super().__init__()
         self.config = None
         self.topics = None
         self.listener = None
-        self._publish_port = publish_port
-        self._publish_nameservers = publish_nameservers
         self.publisher = None
         self.host = socket.gethostname()
-        self._create_publisher()
+
+        if publish_port is not None:
+            self.publisher = NoisyPublisher(
+                "dispatcher", port=publish_port,
+                nameservers=publish_nameservers)
+            self.publisher.start()
         self.loop = True
         self.config_handler = DispatchConfig(config_file, self.update_config)
         signal.signal(signal.SIGTERM, self.signal_shutdown)
 
-    def _create_publisher(self):
-        if self._publish_port is not None:
-            self.publisher = NoisyPublisher("dispatcher", port=self._publish_port,
-                                            nameservers=self._publish_nameservers)
-            self.publisher.start()
-
     def signal_shutdown(self, *args, **kwargs):
         """Shutdown dispatcher."""
         self.close()
 
     def update_config(self, new_config):
         """Update configuration and reload listeners."""
         old_config = self.config
         topics = set()
         try:
             for _client, client_config in new_config.items():
                 topics |= set(sum([item['topics'] for item in client_config['dispatch_configs']], []))
             if self.topics != topics:
+                if self.listener is not None:
+                    # FIXME: make sure to get the last messages though
+                    self.listener.stop()
                 self.config = new_config
-                self._create_listener(client_config, topics)
+                addresses = client_config.get('subscribe_addresses', None)
+                nameserver = client_config.get('nameserver', 'localhost')
+                services = client_config.get('subscribe_services', '')
+                self.listener = ListenerContainer(topics=topics,
+                                                  addresses=addresses,
+                                                  nameserver=nameserver,
+                                                  services=services)
+                self.topics = topics
+
         except KeyError as err:
             logger.warning('Invalid config for %s, keeping the old one running: %s', _client, str(err))
             self.config = old_config
 
-    def _create_listener(self, client_config, topics):
-        if self.listener is not None:
-            # FIXME: make sure to get the last messages though
-            self.listener.stop()
-        addresses = client_config.get('subscribe_addresses', None)
-        nameserver = client_config.get('nameserver', 'localhost')
-        services = client_config.get('subscribe_services', '')
-        self.listener = ListenerContainer(topics=topics,
-                                          addresses=addresses,
-                                          nameserver=nameserver,
-                                          services=services)
-        self.topics = topics
-
     def run(self):
         """Run dispatcher."""
         while self.loop:
             try:
                 msg = self.listener.output_queue.get(timeout=1)
             except Empty:
                 continue
-            if msg.type != 'file':
-                continue
-            self._dispatch_from_message(msg)
-
-    def _dispatch_from_message(self, msg):
-        destinations = self.get_destinations(msg)
-        if destinations:
-            # Check if the url are on another host:
-            url = urlparse(msg.data['uri'])
-            _check_file_locality(url, self.host)
-            success = dispatch(url.path, destinations)
-            if self.publisher:
-                self._publish(msg, destinations, success)
+            else:
+                if msg.type != 'file':
+                    continue
+                destinations = self.get_destinations(msg)
+                if destinations:
+                    # Check if the url are on another host:
+                    url = urlparse(msg.data['uri'])
+                    if not is_file_local(url):
+                        # This warning may appear even if the file path
+                        # does exist on both servers (a central file server
+                        # reachable from both). But in those cases one
+                        # should probably not use an url scheme but just a
+                        # file path:
+                        raise NotImplementedError(("uri is pointing to a file path on another server! "
+                                                   "Host=<%s> uri netloc=<%s>", self.host, url.netloc))
+                    success = dispatch(url.path, destinations)
+                    if self.publisher:
+                        self._publish(msg, destinations, success)
 
     def _publish(self, msg, destinations, success):
         """Publish a message.
 
         The URI is replaced with the URI on the target server.
 
         """
-        for url, _, client in destinations:
+        for url, params, client in destinations:
             if not success[client]:
                 continue
-            msg = self._get_new_message(msg, url, client)
-            if msg is None:
+            del params
+            info = msg.data.copy()
+            info["uri"] = urlsplit(url).path
+            topic = self.config[client].get("publish_topic")
+            if topic is None:
+                logger.error("Publish topic not configured for '%s'",
+                             client)
                 continue
+            topic = compose(topic, info)
+            msg = Message(topic, 'file', info)
             logger.debug('Publishing %s', str(msg))
             self.publisher.send(str(msg))
 
-    def _get_new_message(self, msg, url, client):
-        info = self._get_message_info(msg, url)
-        topic = self._get_topic(client, info)
-        if topic is None:
-            return None
-        return Message(topic, 'file', info)
-
-    def _get_message_info(self, msg, url):
-        info = msg.data.copy()
-        info["uri"] = urlsplit(url).path
-        return info
-
-    def _get_topic(self, client, info):
-        topic = self.config[client].get("publish_topic")
-        if topic is None:
-            logger.error("Publish topic not configured for '%s'", client)
-            return None
-        return compose(topic, info)
-
     def get_destinations(self, msg):
         """Get the destinations for this message."""
         destinations = []
         for client, config in self.config.items():
-            for dispatch_config in config['dispatch_configs']:
-                destination = self._get_destination(dispatch_config, msg, client)
-                if destination is None:
+            for disp_config in config['dispatch_configs']:
+                for topic in disp_config['topics']:
+                    if msg.subject.startswith(topic):
+                        break
+                else:
                     continue
-                destinations.append(destination)
+                if check_conditions(msg, disp_config):
+                    destinations.append(
+                        self.create_dest_url(msg, client, disp_config))
         return destinations
 
-    def _get_destination(self, dispatch_config, msg, client):
-        destination = None
-        if _has_correct_topic(dispatch_config, msg):
-            if check_conditions(msg, dispatch_config):
-                destination = self.create_dest_url(msg, client, dispatch_config)
-        return destination
-
-    def create_dest_url(self, msg, client, conf):
+    def create_dest_url(self, msg, client, disp_config):
         """Create the destination URL and the connection parameters."""
         defaults = self.config[client].copy()
-        _verify_filepattern(defaults, msg)
-        connection_parameters = conf.get('connection_parameters', defaults.get('connection_parameters'))
-        host = conf.get('host', defaults['host'])
-
-        metadata = _get_metadata_with_aliases(msg, defaults)
-
-        path = compose(
-            os.path.join(conf.get('directory', defaults['directory']),
-                         conf.get('filepattern', defaults['filepattern'])),
-            metadata)
+        if 'filepattern' not in defaults:
+            source_filename = os.path.basename(urlsplit(msg.data['uri']).path)
+            defaults['filepattern'] = source_filename
+        info_dict = dict()
+        for key in ['host', 'directory', 'filepattern']:
+            try:
+                info_dict[key] = disp_config[key]
+            except KeyError:
+                info_dict[key] = defaults[key]
+        connection_parameters = disp_config.get(
+            'connection_parameters',
+            defaults.get('connection_parameters'))
+        host = info_dict['host']
+        path = os.path.join(info_dict['directory'], info_dict['filepattern'])
+        mda = msg.data.copy()
+
+        for key, aliases in defaults.get('aliases', {}).items():
+            if isinstance(aliases, dict):
+                aliases = [aliases]
+
+            for alias in aliases:
+                new_key = alias.pop("_alias_name", key)
+                if key in msg.data:
+                    mda[new_key] = alias.get(msg.data[key], msg.data[key])
+
+        path = compose(path, mda)
         parts = urlsplit(host)
-        host_path = urlunsplit((parts.scheme, parts.netloc, path, parts.query, parts.fragment))
+        host_path = urlunsplit((parts.scheme, parts.netloc, path,
+                                parts.query, parts.fragment))
         return host_path, connection_parameters, client
 
     def close(self):
         """Shutdown the dispatcher."""
         logger.info('Terminating dispatcher.')
         self.loop = False
         try:
@@ -418,49 +420,14 @@
                 logger.exception("Couldn't stop publisher.")
         try:
             self.config_handler.close()
         except Exception:
             logger.exception("Couldn't stop config handler.")
 
 
-def _check_file_locality(url, host):
-    if not is_file_local(url):
-        # This warning may appear even if the file path does exist on both servers (a central file server
-        # reachable from both). But in those cases one should probably not use an url scheme but just a
-        # file path:
-        raise NotImplementedError(("uri is pointing to a file path on another server! "
-                                   "Host=<%s> uri netloc=<%s>", host, url.netloc))
-
-
-def _has_correct_topic(dispatch_config, msg):
-    for topic in dispatch_config['topics']:
-        if msg.subject.startswith(topic):
-            return True
-    return False
-
-
-def _verify_filepattern(defaults, msg):
-    if 'filepattern' not in defaults:
-        source_filename = os.path.basename(urlsplit(msg.data['uri']).path)
-        defaults['filepattern'] = source_filename
-
-
-def _get_metadata_with_aliases(msg, defaults):
-    metadata = msg.data.copy()
-    for key, aliases in defaults.get('aliases', {}).items():
-        if isinstance(aliases, dict):
-            aliases = [aliases]
-
-        for alias in aliases:
-            new_key = alias.pop("_alias_name", key)
-            if key in msg.data:
-                metadata[new_key] = alias.get(msg.data[key], msg.data[key])
-    return metadata
-
-
 def check_conditions(msg, item):
     """Check if a message matches the config item's conditions.
 
     The conditions sets are OR'ed, so this returns True if one condition set
     matches. Within a condition set, all the conditions are AND'ed.
     Example::
```

### Comparing `trollmoves-0.9.0/trollmoves/heartbeat_monitor.py` & `trollmoves-7.0.0/trollmoves/heartbeat_monitor.py`

 * *Files identical despite different names*

### Comparing `trollmoves-0.9.0/trollmoves/hooks.py` & `trollmoves-7.0.0/trollmoves/hooks.py`

 * *Files identical despite different names*

### Comparing `trollmoves-0.9.0/trollmoves/mirror.py` & `trollmoves-7.0.0/bin/move_it_mirror.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,176 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021 Trollmoves developers
+# Copyright (c) 2016
 #
 # Author(s):
 #
 #   Martin Raspaud <martin.raspaud@smhi.se>
+#   Panu Lahtinen <panu.lahtinen@fmi.fi>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""Move it Mirror."""
 
-"""All you need for mirroring."""
-
-import os
-import logging
-import signal
-import time
-
-from urllib.parse import urlparse, urlunparse
+import logging.handlers
 from threading import Lock, Timer
+from urllib.parse import urlunparse
+import argparse
 
 from posttroll.message import Message
-from posttroll.publisher import get_own_ip
+from posttroll.publisher import Publisher, get_own_ip
 
-from trollmoves.client import Listener
-from trollmoves.client import request_push
-from trollmoves.server import RequestManager, Deleter
 from trollmoves.move_it_base import MoveItBase, create_publisher
+from trollmoves.client import Listener
 from trollmoves.server import reload_config
+from trollmoves.mirror import MirrorRequestManager, file_registry
 
-
-LOGGER = logging.getLogger(__name__)
-file_registry = {}
-cache_lock = Lock()
-
-
-class MirrorListener(Listener):
-    """Listener for Trollmoves Mirror.
-
-    Subclass the Client Listener to replace how the messages are processed.
-    """
-
-    def _process_message(self, msg):
-        if _file_already_published(msg):
-            return
-        file_registry[msg.data['uid']] = [msg]
-        request_address = self.ckwargs.get("request_address", get_own_ip()) + ":" + self.ckwargs["request_port"]
-        delay = float(self.ckwargs.get("delay", 0))
-        publisher = self.ckwargs["publisher"]
-        mirror_message = _get_mirror_message(msg, request_address)
-        if delay:
-            Timer(delay, publisher.send, [mirror_message]).start()
-        else:
-            publish_mirror_message(mirror_message, publisher.send)
-
-
-def _file_already_published(msg):
-    with cache_lock:
-        if msg.data['uid'] in file_registry:
-            file_registry[msg.data['uid']].append(msg)
-            return True
-    return False
-
-
-def _get_mirror_message(msg, request_address):
-    mirror_message = Message(msg.subject, msg.type, msg.data.copy())
-    mirror_message.data['request_address'] = request_address
-    return mirror_message
-
-
-def publish_mirror_message(mirror_message, publisher_send):
-    """Forward an updated message."""
-    LOGGER.debug('Sending %s', str(mirror_message))
-    publisher_send(str(mirror_message))
+LOGGER = logging.getLogger("move_it_mirror")
+LOG_FORMAT = "[%(asctime)s %(levelname)-8s %(name)s] %(message)s"
 
 
 class MoveItMirror(MoveItBase):
     """Mirror for move_it."""
 
     def __init__(self, cmd_args):
         """Set up the mirror."""
         publisher = create_publisher(cmd_args.port, "move_it_mirror")
         super(MoveItMirror, self).__init__(cmd_args, "mirror", publisher=publisher)
+        self.cache_lock = Lock()
 
     def reload_cfg_file(self, filename):
         """Reload the config file."""
         reload_config(filename, self.chains, self.create_listener_notifier,
-                      MirrorRequestManager, publisher=self.publisher, disable_backlog=True)
+                      MirrorRequestManager, publisher=self.sync_publisher)
 
     def signal_reload_cfg_file(self, *args):
         """Reload the config file when we get a signal."""
         del args
         self.reload_cfg_file(self.cmd_args.config_file)
 
     def create_listener_notifier(self, attrs, publisher):
         """Create a listener notifier."""
-        if "publisher" not in attrs:
-            attrs["publisher"] = publisher
-        listeners = Listeners(attrs.pop("client_topic"), attrs.pop("providers"), **attrs)
-
-        return listeners, noop
-
-    def run(self):
-        """Start the transfer chains."""
-        signal.signal(signal.SIGTERM, self.chains_stop)
-        signal.signal(signal.SIGHUP, self.signal_reload_cfg_file)
-        self.notifier.start()
-        self.running = True
-        while self.running:
-            time.sleep(1)
-            self.publisher.heartbeat(30)
+        request_address = attrs.get("request_address",
+                                    get_own_ip()) + ":" + attrs["request_port"]
+
+        delay = float(attrs.get('delay', 0))
+        if delay > 0:
+            def send(msg):
+                """Delay the sending."""
+                Timer(delay, publisher.send, [msg]).start()
+        else:
+            def send(msg):
+                """Use the regular publisher to send."""
+                publisher.send(msg)
+
+        def publish_callback(msg, *args, **kwargs):
+            """Forward an updated message."""
+            del args
+            del kwargs
+            # save to file_cache
+            with self.cache_lock:
+                if msg.data['uid'] in file_registry:
+                    file_registry[msg.data['uid']].append(msg)
+                    return
+
+            file_registry[msg.data['uid']] = [msg]
+            # transform message
+            new_msg = Message(msg.subject, msg.type, msg.data.copy())
+            new_msg.data['request_address'] = request_address
+
+            # send onwards
+            LOGGER.debug('Sending %s', str(new_msg))
+            send(str(new_msg))
+
+        if "client_topic" not in attrs:
+            attrs["client_topic"] = None
+        listeners = Listeners(publish_callback, **attrs)
+
+        return listeners, foo
 
 
-def noop(*args, **kwargs):
+def foo(*args, **kwargs):
     """Do not do anything."""
     pass
 
 
 class Listeners(object):
     """Class for multiple listeners."""
 
-    def __init__(self, client_topic, providers, **attrs):
+    def __init__(self, callback, client_topic, providers, **attrs):
         """Set up the listeners."""
         self.listeners = []
         if client_topic is None:
             client_topic = []
         else:
             client_topic = [client_topic]
 
         for provider in providers.split():
-            topic = _get_topic(client_topic, provider)
-            self.listeners.append(MirrorListener(
+            topic = client_topic
+            if '/' in provider:
+                parts = provider.split('/', 1)
+                provider = parts[0]
+                topic = ['/' + parts[1]]
+                LOGGER.info("Using provider-specific topic %s for %s",
+                            topic, provider)
+            self.listeners.append(Listener(
                 urlunparse(('tcp', provider, '', '', '', '')),
                 topic,
-                **attrs))
+                callback, **attrs))
 
     def start(self):
         """Start the listeners."""
         for listener in self.listeners:
             listener.start()
 
     def stop(self):
         """Stop the listeners."""
         for listener in self.listeners:
             listener.stop()
 
 
-def _get_topic(client_topic, provider):
-    topic = client_topic
-    if '/' in provider:
-        parts = provider.split('/', 1)
-        provider = parts[0]
-        topic = ['/' + parts[1]]
-        LOGGER.info("Using provider-specific topic %s for %s",
-                    topic, provider)
-    return topic
-
-
-class MirrorRequestManager(RequestManager):
-    """Handle requests as a mirror."""
-
-    def __init__(self, port, attrs):
-        """Set up this mirror request manager."""
-        RequestManager.__init__(self, port, attrs)
-        self._deleter = MirrorDeleter(attrs)
-
-    def push(self, message):
-        """Push the file."""
-        new_uri = None
-        for source_message in file_registry.get(message.data['uid'], []):
-            request_push(source_message, **self._attrs)
-            destination = urlparse(self._attrs['destination']).path
-            new_uri = os.path.join(destination, message.data['uid'])
-            if os.path.exists(new_uri):
-                break
-        if new_uri is None:
-            raise KeyError('No source message found for %s',
-                           str(message.data['uid']))
-        message.data['uri'] = new_uri
-        return RequestManager.push(self, message)
-
-
-class MirrorDeleter(Deleter):
-    """Deleter for mirroring."""
-
-    def __init__(self, attrs=None):
-        """Set up the deleter."""
-        super().__init__(attrs)
-
-    @staticmethod
-    def delete(filename):
-        """Delete the file."""
-        Deleter.delete(filename)
-        # Pop is atomic, so we don't need a lock.
-        file_registry.pop(os.path.basename(filename), None)
+def parse_args():
+    """Parse the command line arguments."""
+    parser = argparse.ArgumentParser()
+    parser.add_argument("config_file",
+                        help="The configuration file to run on.")
+    parser.add_argument("-l",
+                        "--log",
+                        help="The file to log to. stdout otherwise.")
+    parser.add_argument("-p",
+                        "--port",
+                        help="The port to publish on. 9010 is the default",
+                        default=9010)
+    parser.add_argument("-v", "--verbose", default=False, action="store_true",
+                        help="Toggle verbose logging")
+
+    return parser.parse_args()
+
+
+def main():
+    """Start the mirroring."""
+    cmd_args = parse_args()
+    mirror = MoveItMirror(cmd_args)
+
+    try:
+        mirror.reload_cfg_file(cmd_args.config_file)
+        mirror.run()
+    except KeyboardInterrupt:
+        LOGGER.debug("Interrupting")
+    finally:
+        if mirror.running:
+            mirror.chains_stop()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `trollmoves-0.9.0/trollmoves/move_it_base.py` & `trollmoves-7.0.0/trollmoves/move_it_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,58 +26,61 @@
 import logging
 import logging.handlers
 import os
 
 import pyinotify
 from posttroll.publisher import Publisher
 
+from trollmoves.server import EventHandler
+
 LOGGER = logging.getLogger("move_it_base")
 LOG_FORMAT = "[%(asctime)s %(levelname)-8s %(name)s] %(message)s"
 
 
 class MoveItBase(object):
     """Base class for Trollmoves."""
 
     def __init__(self, cmd_args, chain_type, publisher=None):
         """Initialize the class."""
         self.cmd_args = cmd_args
         self.chain_type = chain_type
         self.running = False
         self.notifier = None
         self.watchman = None
-        self.publisher = publisher
+        self.sync_publisher = publisher
         self._np = None
         self.chains = {}
         setup_logging(cmd_args, chain_type)
         LOGGER.info("Starting up.")
         self.setup_watchers(cmd_args)
 
     def reload_cfg_file(self, filename, *args, **kwargs):
         """Reload configuration file."""
         if self.chain_type == "client":
             from trollmoves.client import reload_config
-            reload_config(filename, self.chains, *args, **kwargs)
+            reload_config(filename, self.chains, *args, sync_publisher=self.sync_publisher,
+                          **kwargs)
         else:
             # Also Mirror uses the reload_config from the Server
             from trollmoves.server import reload_config
-            reload_config(filename, self.chains, *args, publisher=self.publisher,
+            reload_config(filename, self.chains, *args, publisher=self.sync_publisher,
                           use_watchdog=self.cmd_args.watchdog,
                           disable_backlog=self.cmd_args.disable_backlog)
 
     def signal_reload_cfg_file(self, *args):
         """Handle reload signal."""
         del args
         if self.chain_type == "client":
             from trollmoves.client import reload_config
             reload_config(self.cmd_args.config_file, self.chains,
-                          publisher=self.publisher)
+                          sync_publisher=self.sync_publisher)
         else:
             from trollmoves.server import reload_config
             reload_config(self.cmd_args.config_file, self.chains,
-                          publisher=self.publisher,
+                          publisher=self.sync_publisher,
                           use_watchdog=self.cmd_args.watchdog,
                           disable_backlog=self.cmd_args.disable_backlog)
 
     def chains_stop(self, *args):
         """Stop all transfer chains."""
         del args
         if self.chain_type == "client":
@@ -135,72 +138,7 @@
     pyinotify.log.handlers = [fh_]
 
 
 def create_publisher(port, publisher_name):
     """Create a publisher using port *port*."""
     LOGGER.info("Starting publisher on port %s.", str(port))
     return Publisher("tcp://*:" + str(port), publisher_name)
-
-
-# Generic event handler
-# fixme: on deletion, the file should be removed from the filecache
-class EventHandler(pyinotify.ProcessEvent):
-    """Handle events with a generic *fun* function."""
-
-    def __init__(self, fun, *args, **kwargs):
-        """Initialize event handler."""
-        pyinotify.ProcessEvent.__init__(self, *args, **kwargs)
-        self._cmd_filename = kwargs.get('cmd_filename')
-        if self._cmd_filename:
-            self._cmd_filename = os.path.abspath(self._cmd_filename)
-        self._fun = fun
-        self._watched_dirs = dict()
-        self._watchManager = kwargs.get('watchManager', None)
-        self._tmask = kwargs.get('tmask', None)
-
-    def process_IN_CLOSE_WRITE(self, event):
-        """On closing after writing."""
-        if self._cmd_filename and os.path.abspath(
-                event.pathname) != self._cmd_filename:
-            return
-        self._fun(event.pathname)
-
-    def process_IN_CREATE(self, event):
-        """On closing after linking."""
-        if (event.mask & pyinotify.IN_ISDIR):
-            self._watched_dirs.update(self._watchManager.add_watch(event.pathname, self._tmask))
-
-        if self._cmd_filename and os.path.abspath(
-                event.pathname) != self._cmd_filename:
-            return
-        try:
-            if os.stat(event.pathname).st_nlink > 1:
-                self._fun(event.pathname)
-        except OSError:
-            return
-
-    def process_IN_MOVED_TO(self, event):
-        """On closing after moving."""
-        if self._cmd_filename and os.path.abspath(
-                event.pathname) != self._cmd_filename:
-            return
-        self._fun(event.pathname)
-
-    def process_IN_DELETE(self, event):
-        """On delete."""
-        if (event.mask & pyinotify.IN_ISDIR):
-            try:
-                try:
-                    self._watchManager.rm_watch(self._watched_dirs[event.pathname], quiet=False)
-                except pyinotify.WatchManagerError:
-                    # As the directory is deleted prior removing the
-                    # watch will cause a error message from
-                    # pyinotify. This is ok, so just pass the
-                    # exception.
-                    pass
-                finally:
-                    del self._watched_dirs[event.pathname]
-            except KeyError:
-                LOGGER.warning(
-                    "Dir %s not watched by inotify. Can not delete watch.",
-                    event.pathname)
-        return
```

### Comparing `trollmoves-0.9.0/trollmoves/movers.py` & `trollmoves-7.0.0/trollmoves/movers.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 
 import logging
 import os
 import shutil
 import sys
 import time
 import traceback
+from ftplib import FTP, all_errors, error_perm
 from threading import Event, Lock, Thread, current_thread
-from urllib.parse import urlparse
 import netrc
 
-from ftplib import FTP, all_errors, error_perm
-from paramiko import SSHClient, SSHException, AutoAddPolicy
-from scp import SCPClient
+from six import string_types
+from six.moves.urllib.parse import urlparse
+
 
 from trollmoves.utils import clean_url
+from paramiko import SSHClient, SSHException, AutoAddPolicy
+from scp import SCPClient
 
 LOGGER = logging.getLogger(__name__)
 
 
 def move_it(pathname, destination, attrs=None, hook=None, rel_path=None):
     """Check if the file pointed by *pathname* is in the filelist, and move it
     if it is.
@@ -60,16 +62,16 @@
 
     LOGGER.debug("new_dest = %s", new_dest)
     LOGGER.debug("Copying to: %s", fake_dest)
     try:
         LOGGER.debug("Scheme = %s", str(dest_url.scheme))
         mover = MOVERS[dest_url.scheme]
     except KeyError:
-        LOGGER.error("Unsupported protocol '" + str(dest_url.scheme) +
-                     "'. Could not copy " + pathname + " to " + str(destination))
+        LOGGER.error("Unsupported protocol '" + str(dest_url.scheme)
+                     + "'. Could not copy " + pathname + " to " + str(destination))
         raise
 
     try:
         mover(pathname, new_dest, attrs=attrs).copy()
         if hook:
             hook(pathname, new_dest)
     except Exception as err:
@@ -83,35 +85,35 @@
                     pathname, str(fake_dest))
 
 
 class Mover(object):
     """Base mover object. Doesn't do anything as it has to be subclassed."""
 
     def __init__(self, origin, destination, attrs=None):
-        try:
+        if isinstance(destination, string_types):
             self.destination = urlparse(destination)
-        except AttributeError:
+        else:
             self.destination = destination
 
         self._dest_username = self.destination.username
         self._dest_password = self.destination.password
 
         LOGGER.debug("Destination: %s", str(destination))
         self.origin = origin
         self.attrs = attrs or {}
 
     def copy(self):
         """Copy it !"""
-        raise NotImplementedError("Copy for scheme " + self.destination.scheme +
-                                  " not implemented (yet).")
+        raise NotImplementedError("Copy for scheme " + self.destination.scheme
+                                  + " not implemented (yet).")
 
     def move(self):
         """Move it !"""
-        raise NotImplementedError("Move for scheme " + self.destination.scheme +
-                                  " not implemented (yet).")
+        raise NotImplementedError("Move for scheme " + self.destination.scheme
+                                  + " not implemented (yet).")
 
     def get_connection(self, hostname, port, username=None):
         """Get the connection."""
         with self.active_connection_lock:
             LOGGER.debug("Destination username and passwd: %s %s",
                          self._dest_username, self._dest_password)
             LOGGER.debug('Getting connection to %s@%s:%s',
```

### Comparing `trollmoves-0.9.0/trollmoves/server.py` & `trollmoves-7.0.0/trollmoves/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,76 +19,55 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Classes and functions for Trollmoves server."""
 
+import bz2
 import datetime
 import errno
 import fnmatch
 import glob
 import logging
 import logging.handlers
 import os
 import subprocess
 import sys
 import tempfile
 import time
 from collections import deque
 from threading import Lock, Thread
-from configparser import RawConfigParser
-from queue import Empty, Queue
-from urllib.parse import urlparse
-import signal
 
-import bz2
 import pyinotify
 from zmq import NOBLOCK, POLLIN, PULL, PUSH, ROUTER, Poller, ZMQError
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers.polling import PollingObserver
+
 from posttroll import get_context
 from posttroll.message import Message
 from posttroll.publisher import get_own_ip
 from posttroll.subscriber import Subscribe
-from trollsift import globify, parse
-
+from configparser import RawConfigParser
+from queue import Empty, Queue
+from six.moves.urllib.parse import urlparse
 from trollmoves.client import DEFAULT_REQ_TIMEOUT
 from trollmoves.movers import move_it
 from trollmoves.utils import (clean_url, gen_dict_contains, gen_dict_extract,
                               is_file_local)
-from trollmoves.move_it_base import MoveItBase, create_publisher, EventHandler
+from trollsift import globify, parse
 
 LOGGER = logging.getLogger(__name__)
 
 
 file_cache = deque(maxlen=61000)
 file_cache_lock = Lock()
 START_TIME = datetime.datetime.utcnow()
 
 
-class MoveItServer(MoveItBase):
-    """Wrapper class for Trollmoves Server."""
-
-    def __init__(self, cmd_args):
-        """Initialize server."""
-        publisher = create_publisher(cmd_args.port, "move_it_server")
-        super(MoveItServer, self).__init__(cmd_args, "server", publisher=publisher)
-
-    def run(self):
-        """Start the transfer chains."""
-        signal.signal(signal.SIGTERM, self.chains_stop)
-        signal.signal(signal.SIGHUP, self.signal_reload_cfg_file)
-        self.notifier.start()
-        self.running = True
-        while self.running:
-            time.sleep(1)
-            self.publisher.heartbeat(30)
-
-
 class ConfigError(Exception):
     """Configuration error."""
 
     pass
 
 
 class Deleter(Thread):
@@ -150,164 +129,155 @@
 class RequestManager(Thread):
     """Manage requests."""
 
     def __init__(self, port, attrs=None):
         """Initialize request manager."""
         Thread.__init__(self)
 
-        self.port = port
-        self._attrs = attrs
         self._loop = True
-        self.out_socket = None
-        self.in_socket = None
-        self._poller = None
-        self._station = None
-
-        self._validate_file_pattern()
-        self._set_out_socket()
-        self._set_in_socket()
-        self._set_station()
-        self._create_poller()
-        self._deleter = Deleter(attrs)
-
-    def _set_out_socket(self):
         self.out_socket = get_context().socket(ROUTER)
-        self.out_socket.bind("tcp://*:" + str(self.port))
-
-    def _set_in_socket(self):
+        self.out_socket.bind("tcp://*:" + str(port))
+        self.port = port
         self.in_socket = get_context().socket(PULL)
-        self.in_socket.bind("inproc://replies" + str(self.port))
+        self.in_socket.bind("inproc://replies" + str(port))
 
-    def _set_station(self):
-        try:
-            self._station = self._attrs["station"]
-        except (KeyError, TypeError):
-            LOGGER.warning("Station is not defined in config file")
-            self._station = "unknown"
-        LOGGER.debug("Station is '%s'", self._station)
-
-    def _create_poller(self):
         self._poller = Poller()
         self._poller.register(self.out_socket, POLLIN)
         self._poller.register(self.in_socket, POLLIN)
-
-    def _validate_file_pattern(self):
+        self._attrs = attrs
         try:
-            _ = globify(self._attrs["origin"])
+            # Checking the validity of the file pattern
+            globify(attrs["origin"])
         except ValueError as err:
             raise ConfigError('Invalid file pattern: ' + str(err))
         except KeyError:
-            if 'listen' not in self._attrs:
+            if 'listen' not in attrs:
                 raise
+        self._deleter = Deleter(attrs)
+
+        try:
+            self._station = self._attrs["station"]
+        except (KeyError, TypeError):
+            LOGGER.warning("Station is not defined in config file")
+            self._station = "unknown"
+        LOGGER.debug("Station is '%s'", self._station)
 
     def start(self):
         """Start the request manager."""
         self._deleter.start()
         Thread.start(self)
 
     def pong(self, message):
         """Reply to ping."""
         return Message(message.subject, "pong", {"station": self._station})
 
     def push(self, message):
         """Reply to push request."""
-        new_msg = self._move_files(message)
-        if new_msg is None:
-            new_msg = Message(message.subject,
-                              _get_push_message_type(message),
-                              data=message.data.copy())
-            new_msg.data['destination'] = clean_url(new_msg.data['destination'])
+        for the_dict in gen_dict_contains(message.data, 'uri'):
+            uri = urlparse(the_dict['uri'])
+            rel_path = the_dict.get('path', None)
+            pathname = uri.path
+            # FIXME: check against file_cache
+            if 'origin' in self._attrs and not fnmatch.fnmatch(
+                    os.path.basename(pathname),
+                    os.path.basename(globify(self._attrs["origin"]))):
+                LOGGER.warning('Client trying to get invalid file: %s', pathname)
+                return Message(message.subject,
+                               "err",
+                               data="{0:s} not reachable".format(pathname))
+            try:
+                move_it(pathname, message.data['destination'], self._attrs, rel_path=rel_path)
+            except Exception as err:
+                return Message(message.subject, "err", data=str(err))
+            else:
+                if (self._attrs.get('compression') or self._attrs.get(
+                        'delete', 'False').lower() in ["1", "yes", "true", "on"]):
+                    self._deleter.add(pathname)
+
+            if 'dataset' in message.data:
+                mtype = 'dataset'
+            elif 'collection' in message.data:
+                mtype = 'collection'
+            elif 'uid' in message.data:
+                mtype = 'file'
+            else:
+                raise KeyError('No known metadata in message.')
 
+        new_msg = Message(message.subject,
+                          mtype,
+                          data=message.data.copy())
+        new_msg.data['destination'] = clean_url(new_msg.data[
+            'destination'])
         return new_msg
 
-    def _move_files(self, message):
-        error_message = None
-        for data in gen_dict_contains(message.data, 'uri'):
-            pathname = urlparse(data['uri']).path
-            rel_path = data.get('path', None)
-            error_message = self._validate_requested_file(pathname, message)
-            if error_message is not None:
-                break
-            error_message = self._move_file(pathname, message, rel_path)
-            if error_message is not None:
-                break
-
-        return error_message
-
-    def _validate_requested_file(self, pathname, message):
-        # FIXME: check against file_cache
-        if 'origin' in self._attrs and not fnmatch.fnmatch(
-                os.path.basename(pathname),
-                os.path.basename(globify(self._attrs["origin"]))):
-            LOGGER.warning('Client trying to get invalid file: %s', pathname)
-            return Message(message.subject, "err", data="{0:s} not reachable".format(pathname))
-        return None
-
-    def _move_file(self, pathname, message, rel_path):
-        error_message = None
-        try:
-            move_it(pathname, message.data['destination'], self._attrs, rel_path=rel_path)
-        except Exception as err:
-            error_message = Message(message.subject, "err", data=str(err))
-        else:
-            self._add_to_deleter(pathname)
-        return error_message
-
-    def _add_to_deleter(self, pathname):
-        if self._attrs.get('compression') or self._is_delete_set():
-            self._deleter.add(pathname)
-
-    def _is_delete_set(self):
-        return self._attrs.get('delete', 'False').lower() in ["1", "yes", "true", "on"]
-
     def ack(self, message):
         """Reply with ack to a publication."""
-        new_msg = None
         for url in gen_dict_extract(message.data, 'uri'):
-            pathname = urlparse(url).path
-            new_msg = self._validate_requested_file(pathname, message)
-            if new_msg is not None:
-                break
-            self._add_to_deleter(pathname)
-
-        if new_msg is None:
-            new_msg = _get_cleaned_ack_message(message)
+            uri = urlparse(url)
+            pathname = uri.path
 
+            if 'origin' in self._attrs and not fnmatch.fnmatch(
+                    os.path.basename(pathname),
+                    os.path.basename(globify(self._attrs["origin"]))):
+                LOGGER.warning('Client trying to get invalid file: %s', pathname)
+                return Message(message.subject,
+                               "err",
+                               data="{0:s} not reacheable".format(pathname))
+
+            if (self._attrs.get('compression') or self._attrs.get(
+                    'delete', 'False').lower() in ["1", "yes", "true", "on"]):
+                self._deleter.add(pathname)
+        new_msg = Message(message.subject, "ack", data=message.data.copy())
+        try:
+            new_msg.data['destination'] = clean_url(new_msg.data[
+                'destination'])
+        except KeyError:
+            pass
         return new_msg
 
     def info(self, message):
         """Collect information from file cache to message."""
+        topic = message.subject
+        max_count = 2256  # Let's set a (close to arbitrary) limit on messages size.
+        try:
+            max_count = min(message.data.get("max_count", max_count), max_count)
+        except AttributeError:
+            pass
         uptime = datetime.datetime.utcnow() - START_TIME
-        files, max_count = _collect_cached_files(message)
-
+        files = []
+        with file_cache_lock:
+            for i in file_cache:
+                if i.startswith(topic):
+                    files.append(i)
+                    if len(files) == max_count:
+                        break
         return Message(message.subject, "info", data={"files": files, "max_count": max_count, "uptime": str(uptime)})
 
     def unknown(self, message):
         """Reply to any unknown request."""
         return Message(message.subject, "unknown")
 
     def reply_and_send(self, fun, address, message):
         """Reply to request."""
+        in_socket = get_context().socket(PUSH)
+        in_socket.connect("inproc://replies" + str(self.port))
+
         reply = Message(message.subject, "error")
         try:
             reply = fun(message)
         except Exception:
             LOGGER.exception("Something went wrong"
                              " when processing the request: %s", str(message))
         finally:
-            self._send_multipart_reply(reply, address)
-
-    def _send_multipart_reply(self, reply, address):
-        LOGGER.debug("Response: %s", str(reply))
-        in_socket = get_context().socket(PUSH)
-        in_socket.connect("inproc://replies" + str(self.port))
-        try:
-            in_socket.send_multipart([address, b'', str(reply)])
-        except TypeError:
-            in_socket.send_multipart([address, b'', bytes(str(reply), 'utf-8')])
+            LOGGER.debug("Response: %s", str(reply))
+            try:
+                in_socket.send_multipart([address, b'', str(reply)])
+            except TypeError:
+                in_socket.send_multipart([address, b'', bytes(str(reply),
+                                                              'utf-8')])
 
     def run(self):
         """Run request manager."""
         try:
             self._run()
         except Exception:
             LOGGER.exception("Request Manager died.")
@@ -317,401 +287,167 @@
         while self._loop:
             try:
                 socks = dict(self._poller.poll(timeout=2000))
             except ZMQError:
                 LOGGER.info("Poller interrupted.")
                 continue
             if socks.get(self.out_socket) == POLLIN:
-                address, payload = self._get_address_and_payload()
-                if payload is None:
+                LOGGER.debug("Received a request")
+                multiparts = self.out_socket.recv_multipart(NOBLOCK)
+                try:
+                    address, _, payload = multiparts
+                except ValueError:
+                    LOGGER.warning("Invalid request.")
+                    try:
+                        address = multiparts[0]
+                    except (TypeError, IndexError):
+                        LOGGER.warning("Address unknown, not sending an error message back.")
+                    else:
+                        message = Message('error', 'error', "Invalid message received")
+                        Thread(target=self.reply_and_send,
+                               args=(self.unknown, address, message)).start()
+                        LOGGER.warning("Sent error message back.")
                     continue
-                self._process_request(Message(rawstr=payload), address)
+
+                message = Message(rawstr=payload)
+                fake_msg = Message(rawstr=str(message))
+                try:
+                    urlparse(message.data['destination'])
+                except (KeyError, TypeError):
+                    pass
+                else:
+                    fake_msg.data['destination'] = clean_url(message.data[
+                        'destination'])
+
+                LOGGER.debug("processing request: %s", str(fake_msg))
+                if message.type == "ping":
+                    Thread(target=self.reply_and_send,
+                           args=(self.pong, address, message)).start()
+                elif message.type == "push":
+                    Thread(target=self.reply_and_send,
+                           args=(self.push, address, message)).start()
+                elif message.type == "ack":
+                    Thread(target=self.reply_and_send,
+                           args=(self.ack, address, message)).start()
+                elif message.type == "info":
+                    Thread(target=self.reply_and_send,
+                           args=(self.info, address, message)).start()
+                else:  # unknown request
+                    Thread(target=self.reply_and_send,
+                           args=(self.unknown, address, message)).start()
             elif socks.get(self.in_socket) == POLLIN:
-                self.out_socket.send_multipart(self.in_socket.recv_multipart(NOBLOCK))
+                self.out_socket.send_multipart(
+                    self.in_socket.recv_multipart(NOBLOCK))
 
-    def _get_address_and_payload(self):
-        address, payload = None, None
-        LOGGER.debug("Received a request")
-        multiparts = self.out_socket.recv_multipart(NOBLOCK)
-        try:
-            address, _, payload = multiparts
-        except ValueError:
-            LOGGER.warning("Invalid request.")
-            try:
-                address = multiparts[0]
-            except (TypeError, IndexError):
-                LOGGER.warning("Address unknown, not sending an error message back.")
-            else:
-                message = Message('error', 'error', "Invalid message received")
-                Thread(target=self.reply_and_send, args=(self.unknown, address, message)).start()
-                LOGGER.warning("Sent error message back.")
-        return address, payload
-
-    def _process_request(self, message, address):
-        LOGGER.debug("processing request: %s", str(_sanitize_message_destination(message)))
-        if message.type == "ping":
-            Thread(target=self.reply_and_send, args=(self.pong, address, message)).start()
-        elif message.type == "push":
-            Thread(target=self.reply_and_send, args=(self.push, address, message)).start()
-        elif message.type == "ack":
-            Thread(target=self.reply_and_send, args=(self.ack, address, message)).start()
-        elif message.type == "info":
-            Thread(target=self.reply_and_send, args=(self.info, address, message)).start()
-        else:  # unknown request
-            Thread(target=self.reply_and_send, args=(self.unknown, address, message)).start()
+            else:  # timeout
+                pass
 
     def stop(self):
         """Stop the request manager."""
         self._loop = False
         self._deleter.stop()
         self.out_socket.close(1)
         self.in_socket.close(1)
 
 
-def _get_push_message_type(message):
-    message_type = message.type
-    if 'uri' in message.data:
-        message_type = 'file'
-    elif 'dataset' in message.data:
-        message_type = 'dataset'
-    elif 'collection' in message.data:
-        message_type = 'collection'
-    return message_type
-
-
-def _get_cleaned_ack_message(message):
-    new_msg = Message(message.subject, "ack", data=message.data.copy())
-    try:
-        new_msg.data['destination'] = clean_url(new_msg.data[
-            'destination'])
-    except KeyError:
-        pass
-
-    return new_msg
-
-
-def _collect_cached_files(message):
-    max_count = 2256  # Let's set a (close to arbitrary) limit on messages size.
-    try:
-        max_count = min(message.data.get("max_count", max_count), max_count)
-    except AttributeError:
-        pass
-    files = []
-    with file_cache_lock:
-        for i in file_cache:
-            if i.startswith(message.subject):
-                files.append(i)
-                if len(files) == max_count:
-                    break
-    return files, max_count
-
-
-def _sanitize_message_destination(message):
-    sanitized_message = Message(rawstr=str(message))
-    try:
-        _ = urlparse(message.data['destination'])
-    except (KeyError, TypeError):
-        pass
-    else:
-        sanitized_message.data['destination'] = clean_url(message.data['destination'])
-    return sanitized_message
-
-
 class Listener(Thread):
     """A message listener for the server."""
 
     def __init__(self, attrs, publisher):
         """Initialize the listener."""
         super(Listener, self).__init__()
         self.attrs = attrs
         self.publisher = publisher
         self.loop = True
 
     def run(self):
         """Start listening to messages."""
         with Subscribe('', topics=self.attrs['listen'], addr_listener=True) as sub:
-            self._run(sub)
-
-    def _run(self, sub):
-        for msg in sub.recv(1):
-            if not self.loop:
-                break
-            if msg is None:
-                continue
-            if not _files_in_message_are_local(msg):
-                break
-            self._send_message(msg)
-
-    def _send_message(self, msg):
-        LOGGER.debug('We have a match: %s', str(msg))
-        info = self._collect_message_info(msg)
-        msg = Message(self.attrs["topic"], msg.type, info)
-        self.publisher.send(str(msg))
-        self._add_files_to_cache(msg)
-        LOGGER.debug("Message sent: %s", str(msg))
-
-    def _collect_message_info(self, msg):
-        info = _collect_attribute_info(self.attrs)
-        info.update(msg.data)
-        info['request_address'] = self.attrs.get(
-            "request_address", get_own_ip()) + ":" + self.attrs["request_port"]
-        return info
+            for msg in sub.recv(1):
+                if msg is None:
+                    if not self.loop:
+                        break
+                    else:
+                        continue
 
-    def _add_files_to_cache(self, msg):
-        with file_cache_lock:
-            for filename in gen_dict_extract(msg.data, 'uid'):
-                file_cache.appendleft(self.attrs["topic"] + '/' + filename)
+                # check that files are local
+                for uri in gen_dict_extract(msg.data, 'uri'):
+                    urlobj = urlparse(uri)
+                    if not is_file_local(urlobj):
+                        break
+                else:
+                    LOGGER.debug('We have a match: %s', str(msg))
+
+                    # pathname = unpack(orig_pathname, **attrs)
+
+                    info = self.attrs.get("info", {})
+                    if info:
+                        info = dict((elt.strip().split('=') for elt in info.split(";")))
+                        for infokey, infoval in info.items():
+                            if "," in infoval:
+                                info[infokey] = infoval.split(",")
+
+                    # info.update(parse(attrs["origin"], orig_pathname))
+                    # info['uri'] = pathname
+                    # info['uid'] = os.path.basename(pathname)
+                    info.update(msg.data)
+                    info['request_address'] = self.attrs.get(
+                        "request_address", get_own_ip()) + ":" + self.attrs["request_port"]
+                    old_data = msg.data
+                    msg = Message(self.attrs["topic"], msg.type, info)
+                    self.publisher.send(str(msg))
+                    with file_cache_lock:
+                        for filename in gen_dict_extract(old_data, 'uid'):
+                            file_cache.appendleft(self.attrs["topic"] + '/' + filename)
+                    LOGGER.debug("Message sent: %s", str(msg))
+                    if not self.loop:
+                        break
 
     def stop(self):
         """Stop the listener."""
         self.loop = False
 
 
-def _files_in_message_are_local(msg):
-    for uri in gen_dict_extract(msg.data, 'uri'):
-        urlobj = urlparse(uri)
-        if not is_file_local(urlobj):
-            return False
-    return True
-
-
-def _collect_attribute_info(attrs):
-    info = attrs.get("info", {})
-    if info:
-        info = dict((elt.strip().split('=') for elt in info.split(";")))
-        for infokey, infoval in info.items():
-            if "," in infoval:
-                info[infokey] = infoval.split(",")
-    return info
-
-
-class WatchdogHandler(FileSystemEventHandler):
-    """Trigger processing on filesystem events."""
-
-    def __init__(self, fun, publisher, pattern, attrs):
-        """Initialize the processor."""
-        FileSystemEventHandler.__init__(self)
-        self.fun = fun
-        self.publisher = publisher
-        self.pattern = pattern
-        self.attrs = attrs
-
-    def on_created(self, event):
-        """Process file creation."""
-        self.fun(event.src_path, self.publisher, self.pattern, self.attrs)
-
-    def on_moved(self, event):
-        """Process a file being moved to the destination directory."""
-        self.fun(event.dest_path, self.publisher, self.pattern, self.attrs)
-
-
-def read_config(filename):
-    """Read the config file called *filename*."""
-    cp_ = RawConfigParser()
-    cp_.read(filename)
-
-    res = {}
-
-    for section in cp_.sections():
-        res[section] = dict(cp_.items(section))
-        _set_config_defaults(res[section])
-        if not _check_origin_and_listen(res, section):
-            continue
-        if not _check_topic(res, section):
-            continue
-        _verify_publish_port(res[section])
-    return res
-
-
-def _set_config_defaults(conf):
-    conf.setdefault("working_directory", None)
-    conf.setdefault("compression", False)
-    conf.setdefault("req_timeout", DEFAULT_REQ_TIMEOUT)
-    conf.setdefault("transfer_req_timeout", 10 * DEFAULT_REQ_TIMEOUT)
-    conf.setdefault("ssh_key_filename", None)
-
-
-def _check_origin_and_listen(res, section):
-    if ("origin" not in res[section]) and ('listen' not in res[section]):
-        LOGGER.warning("Incomplete section %s: add an 'origin' or 'listen' item.", section)
-        LOGGER.info("Ignoring section %s: incomplete.", section)
-        del res[section]
-        return False
-    return True
-
-
-def _check_topic(res, section):
-    if "topic" not in res[section]:
-        LOGGER.warning("Incomplete section %s: add an 'topic' item.", section)
-        LOGGER.info("Ignoring section %s: incomplete.", section)
-        return False
-    return True
-
-
-def _verify_publish_port(conf):
-    try:
-        conf["publish_port"] = int(conf["publish_port"])
-    except (KeyError, ValueError):
-        conf["publish_port"] = 0
-
-
-def reload_config(filename,
-                  chains,
-                  notifier_builder=None,
-                  manager=RequestManager,
-                  publisher=None,
-                  disable_backlog=False,
-                  use_watchdog=False):
-    """Rebuild chains if needed (if the configuration changed) from *filename*."""
-    LOGGER.debug("New config file detected: %s", filename)
-
-    new_chains = read_config(filename)
-
-    old_glob = _update_chains(chains, new_chains, manager, use_watchdog, publisher, notifier_builder)
-    _disable_removed_chains(chains, new_chains)
-    LOGGER.debug("Reloaded config from %s", filename)
-    _process_old_files(old_glob, disable_backlog, publisher)
-    LOGGER.debug("done reloading config")
-
-
-def _update_chains(chains, new_chains, manager, use_watchdog, publisher, notifier_builder):
-    old_glob = []
-    for chain_name, chain in new_chains.items():
-        chain_updated = False
-        if chain_name in chains:
-            if _chains_are_identical(chains, new_chains, chain_name):
-                continue
-            chain_updated = True
-            _stop_chain(chains[chain_name])
-
-        if not _add_chain(chains, chain_name, chain, manager):
-            continue
-
-        fun = _create_notifier_and_get_function(notifier_builder, chains[chain_name], use_watchdog, chain, publisher)
-
-        if 'origin' in chain:
-            old_glob.append((globify(chain["origin"]), fun, chain))
-
-        if chain_updated:
-            LOGGER.debug("Updated %s", chain_name)
-        else:
-            LOGGER.debug("Added %s", chain_name)
-
-    return old_glob
-
-
-def _chains_are_identical(chains, new_chains, chain_name):
-    identical = True
-    for config_key, config_value in new_chains[chain_name].items():
-        if ((config_key not in ["notifier", "publisher"]) and
-            ((config_key not in chains[chain_name]) or
-                (chains[chain_name][config_key] != config_value))):
-            identical = False
-            break
-    return identical
-
-
-def _stop_chain(chain):
-    chain["notifier"].stop()
-    try:
-        chain["notifier"].join()
-    except AttributeError:
-        pass
-    if "request_manager" in chain:
-        chain["request_manager"].stop()
-        LOGGER.debug('Stopped reqman')
-
-
-def _add_chain(chains, chain_name, chain, manager):
-    chains[chain_name] = chain.copy()
-    manager_added = _create_manager(chains, chain_name, chain, manager)
-    if not manager_added:
-        del chains[chain]
-    return manager_added
-
-
-def _create_manager(chains, chain_name, chain, manager):
-    try:
-        chains[chain_name]["request_manager"] = manager(int(chain["request_port"]), chain)
-        LOGGER.debug("Created request manager on port %s", chain["request_port"])
-    except (KeyError, NameError):
-        LOGGER.exception('In reading config')
-    except ConfigError as err:
-        LOGGER.error('Invalid config parameters in %s: %s', chain_name, str(err))
-        LOGGER.warning('Remove and skip %s', chain_name)
-        return False
-    chains[chain_name]["request_manager"].start()
-    return True
-
-
-def _create_notifier_and_get_function(notifier_builder, conf, use_watchdog, chain, publisher):
-    if notifier_builder is None:
-        notifier_builder = _get_notifier_builder(use_watchdog, chain)
-    conf["notifier"], fun = notifier_builder(chain, publisher)
-    conf["notifier"].start()
-
-    return fun
-
-
-def _get_notifier_builder(use_watchdog, val):
-    if 'origin' in val:
-        if use_watchdog:
-            LOGGER.info("Using Watchdog notifier")
-            notifier_builder = create_watchdog_notifier
-        else:
-            LOGGER.info("Using inotify notifier")
-            notifier_builder = create_inotify_notifier
-    elif 'listen' in val:
-        notifier_builder = create_posttroll_notifier
-
-    return notifier_builder
-
-
-def create_watchdog_notifier(attrs, publisher):
-    """Create a notifier from the specified configuration attributes *attrs*."""
-    pattern = globify(attrs["origin"])
-    opath = os.path.dirname(pattern)
-
-    timeout = float(attrs.get("watchdog_timeout", 1.))
-    LOGGER.debug("Watchdog timeout: %.1f", timeout)
-    observer = PollingObserver(timeout=timeout)
-    handler = WatchdogHandler(process_notify, publisher, pattern, attrs)
-
-    observer.schedule(handler, opath)
+def create_posttroll_notifier(attrs, publisher):
+    """Create a notifier listening to posttroll messages from *attrs*."""
+    listener = Listener(attrs, publisher)
 
-    return observer, process_notify
+    return listener, None
 
 
 def process_notify(orig_pathname, publisher, pattern, attrs):
     """Publish what we have."""
     if not fnmatch.fnmatch(orig_pathname, pattern):
         return
-    elif os.stat(orig_pathname).st_size == 0:
+    elif (os.stat(orig_pathname).st_size == 0):
+        # Want to avoid files with size 0.
         LOGGER.debug("Ignoring empty file: %s", orig_pathname)
         return
     else:
         LOGGER.debug('We have a match: %s', orig_pathname)
 
     pathname = unpack(orig_pathname, **attrs)
-    info = _get_notify_message_info(attrs, orig_pathname, pathname)
-    msg = Message(attrs["topic"], 'file', info)
-    publisher.send(str(msg))
-    with file_cache_lock:
-        file_cache.appendleft(attrs["topic"] + '/' + info["uid"])
-    LOGGER.debug("Message sent: %s", str(msg))
 
+    info = attrs.get("info", {})
+    if info:
+        info = dict((elt.strip().split('=') for elt in info.split(";")))
+        for infokey, infoval in info.items():
+            if "," in infoval:
+                info[infokey] = infoval.split(",")
 
-def _get_notify_message_info(attrs, orig_pathname, pathname):
-    info = _collect_attribute_info(attrs)
     info.update(parse(attrs["origin"], orig_pathname))
     info['uri'] = pathname
     info['uid'] = os.path.basename(pathname)
     info['request_address'] = attrs.get(
         "request_address", get_own_ip()) + ":" + attrs["request_port"]
-    return info
+    msg = Message(attrs["topic"], 'file', info)
+    publisher.send(str(msg))
+    with file_cache_lock:
+        file_cache.appendleft(attrs["topic"] + '/' + info["uid"])
+    LOGGER.debug("Message sent: %s", str(msg))
 
 
 def create_inotify_notifier(attrs, publisher):
     """Create a notifier from the specified configuration attributes *attrs*."""
     tmask = (pyinotify.IN_CLOSE_WRITE |
              pyinotify.IN_MOVED_TO |
              pyinotify.IN_CREATE |
@@ -746,64 +482,186 @@
         wm_, EventHandler(process_notify_publish, watchManager=wm_, tmask=tmask))
 
     wm_.add_watch(opath, tmask)
 
     return tnotifier, process_notify
 
 
-def create_posttroll_notifier(attrs, publisher):
-    """Create a notifier listening to posttroll messages from *attrs*."""
-    listener = Listener(attrs, publisher)
+class WatchdogHandler(FileSystemEventHandler):
+    """Trigger processing on filesystem events."""
 
-    return listener, None
+    def __init__(self, fun, publisher, pattern, attrs):
+        """Initialize the processor."""
+        FileSystemEventHandler.__init__(self)
+        self.fun = fun
+        self.publisher = publisher
+        self.pattern = pattern
+        self.attrs = attrs
+
+    def on_created(self, event):
+        """Process file creation."""
+        self.fun(event.src_path, self.publisher, self.pattern, self.attrs)
+
+    def on_moved(self, event):
+        """Process a file being moved to the destination directory."""
+        self.fun(event.dest_path, self.publisher, self.pattern, self.attrs)
+
+
+def create_watchdog_notifier(attrs, publisher):
+    """Create a notifier from the specified configuration attributes *attrs*."""
+    pattern = globify(attrs["origin"])
+    opath = os.path.dirname(pattern)
+
+    timeout = float(attrs.get("watchdog_timeout", 1.))
+    LOGGER.debug("Watchdog timeout: %.1f", timeout)
+    observer = PollingObserver(timeout=timeout)
+    handler = WatchdogHandler(process_notify, publisher, pattern, attrs)
+
+    observer.schedule(handler, opath)
+
+    return observer, process_notify
+
+
+def read_config(filename):
+    """Read the config file called *filename*."""
+    cp_ = RawConfigParser()
+    cp_.read(filename)
+
+    res = {}
+
+    for section in cp_.sections():
+        res[section] = dict(cp_.items(section))
+        res[section].setdefault("working_directory", None)
+        res[section].setdefault("compression", False)
+        res[section].setdefault("req_timeout", DEFAULT_REQ_TIMEOUT)
+        res[section].setdefault("transfer_req_timeout", 10 * DEFAULT_REQ_TIMEOUT)
+        res[section].setdefault("ssh_key_filename", None)
+        if ("origin" not in res[section]) and ('listen' not in res[section]):
+            LOGGER.warning("Incomplete section %s: add an 'origin' or "
+                           "'listen' item.", section)
+            LOGGER.info("Ignoring section %s: incomplete.", section)
+            del res[section]
+            continue
+
+        # if "publisher_port" not in res[section]:
+        #    LOGGER.warning("Incomplete section " + section
+        #                   + ": add an 'publisher_port' item.")
+        #    LOGGER.info("Ignoring section " + section
+        #                + ": incomplete.")
+        #    del res[section]
+        #    continue
+
+        if "topic" not in res[section]:
+            LOGGER.warning("Incomplete section %s: add an 'topic' item.",
+                           section)
+            LOGGER.info("Ignoring section %s: incomplete.",
+                        section)
+            continue
+        else:
+            try:
+                res[section]["publish_port"] = int(res[section][
+                    "publish_port"])
+            except (KeyError, ValueError):
+                res[section]["publish_port"] = 0
+    return res
 
 
-def _disable_removed_chains(chains, new_chains):
+def reload_config(filename,
+                  chains,
+                  notifier_builder=None,
+                  manager=RequestManager,
+                  publisher=None,
+                  disable_backlog=False,
+                  use_watchdog=False):
+    """Rebuild chains if needed (if the configuration changed) from *filename*."""
+    LOGGER.debug("New config file detected: %s", filename)
+
+    new_chains = read_config(filename)
+
+    old_glob = []
+
+    for key, val in new_chains.items():
+        identical = True
+        if key in chains:
+            for key2, val2 in new_chains[key].items():
+                if ((key2 not in ["notifier", "publisher"]) and
+                    ((key2 not in chains[key]) or
+                     (chains[key][key2] != val2))):
+                    identical = False
+                    break
+            if identical:
+                continue
+
+            chains[key]["notifier"].stop()
+            try:
+                # Join the Watchdog thread
+                chains[key]["notifier"].join()
+            except AttributeError:
+                pass
+            if "request_manager" in chains[key]:
+                chains[key]["request_manager"].stop()
+                LOGGER.debug('Stopped reqman')
+
+        chains[key] = val.copy()
+        try:
+            chains[key]["request_manager"] = manager(
+                int(val["request_port"]), val)
+            LOGGER.debug("Created request manager on port %s",
+                         val["request_port"])
+        except (KeyError, NameError):
+            LOGGER.exception('In reading config')
+        except ConfigError as err:
+            LOGGER.error('Invalid config parameters in %s: %s', key, str(err))
+            LOGGER.warning('Remove and skip %s', key)
+            del chains[key]
+            continue
+
+        if notifier_builder is None:
+            if 'origin' in val:
+                if use_watchdog:
+                    LOGGER.info("Using Watchdog notifier")
+                    notifier_builder = create_watchdog_notifier
+                else:
+                    LOGGER.info("Using inotify notifier")
+                    notifier_builder = create_inotify_notifier
+            elif 'listen' in val:
+                notifier_builder = create_posttroll_notifier
+
+        chains[key]["notifier"], fun = notifier_builder(val, publisher)
+        chains[key]["request_manager"].start()
+        chains[key]["notifier"].start()
+        if 'origin' in val:
+            old_glob.append((globify(val["origin"]), fun, val))
+
+        if not identical:
+            LOGGER.debug("Updated %s", key)
+        else:
+            LOGGER.debug("Added %s", key)
+
     for key in (set(chains.keys()) - set(new_chains.keys())):
         chains[key]["notifier"].stop()
         try:
             # Join the Watchdog thread
             chains[key]["notifier"].join()
         except AttributeError:
             pass
         del chains[key]
         LOGGER.debug("Removed %s", key)
 
-
-def _process_old_files(old_glob, disable_backlog, publisher):
+    LOGGER.debug("Reloaded config from %s", filename)
     if old_glob and not disable_backlog:
         time.sleep(3)
         for pattern, fun, attrs in old_glob:
             process_old_files(pattern, fun, publisher, attrs)
 
+    LOGGER.debug("done reloading config")
 
-def process_old_files(pattern, fun, publisher, kwargs):
-    """Process files from *pattern* with function *fun*."""
-    fnames = glob.glob(pattern)
-    if fnames:
-        # time.sleep(3)
-        LOGGER.debug("Touching old files")
-        for fname in fnames:
-            if os.path.exists(fname):
-                fun(fname, publisher, pattern, kwargs)
-
+# Unpackers
 
-def xrit(pathname, destination=None, cmd="./xRITDecompress"):
-    """Unpacks xrit data."""
-    opath, ofile = os.path.split(pathname)
-    destination = destination or tempfile.gettempdir()
-    dest_url = urlparse(destination)
-    expected = os.path.join((destination or opath), ofile[:-2] + "__")
-    if dest_url.scheme in ("", "file"):
-        check_output([cmd, pathname], cwd=(destination or opath))
-    else:
-        LOGGER.exception("Can not extract file %s to %s, destination "
-                         "has to be local.", pathname, destination)
-    LOGGER.info("Successfully extracted %s to %s", pathname, destination)
-    return expected
+# xrit
 
 
 def check_output(*popenargs, **kwargs):
     """Copy from python 2.7, `subprocess.check_output`."""
     if 'stdout' in kwargs:
         raise ValueError('stdout argument not allowed, it will be overridden.')
     LOGGER.debug("Calling %s", str(popenargs))
@@ -815,14 +673,31 @@
         cmd = kwargs.get("args")
         if cmd is None:
             cmd = popenargs[0]
         raise RuntimeError(output)
     return output
 
 
+def xrit(pathname, destination=None, cmd="./xRITDecompress"):
+    """Unpacks xrit data."""
+    opath, ofile = os.path.split(pathname)
+    destination = destination or tempfile.gettempdir()
+    dest_url = urlparse(destination)
+    expected = os.path.join((destination or opath), ofile[:-2] + "__")
+    if dest_url.scheme in ("", "file"):
+        check_output([cmd, pathname], cwd=(destination or opath))
+    else:
+        LOGGER.exception("Can not extract file %s to %s, destination "
+                         "has to be local.", pathname, destination)
+    LOGGER.info("Successfully extracted %s to %s", pathname, destination)
+    return expected
+
+
+# bzip
+
 BLOCK_SIZE = 1024
 
 
 def bzip(origin, destination=None):
     """Unzip files."""
     ofile = os.path.split(origin)[1]
     destfile = os.path.join(destination or tempfile.gettempdir(), ofile[:-4])
@@ -863,14 +738,90 @@
         else:
             if delete.lower() in ["1", "yes", "true", "on"]:
                 os.remove(pathname)
             return new_path
     return pathname
 
 
+# Generic event handler
+# fixme: on deletion, the file should be removed from the filecache
+class EventHandler(pyinotify.ProcessEvent):
+    """Handle events with a generic *fun* function."""
+
+    def __init__(self, fun, *args, **kwargs):
+        """Initialize event handler."""
+        pyinotify.ProcessEvent.__init__(self, *args, **kwargs)
+        self._cmd_filename = kwargs.get('cmd_filename')
+        if self._cmd_filename:
+            self._cmd_filename = os.path.abspath(self._cmd_filename)
+        self._fun = fun
+        self._watched_dirs = dict()
+        self._watchManager = kwargs.get('watchManager', None)
+        self._tmask = kwargs.get('tmask', None)
+
+    def process_IN_CLOSE_WRITE(self, event):
+        """On closing after writing."""
+        if self._cmd_filename and os.path.abspath(
+                event.pathname) != self._cmd_filename:
+            return
+        self._fun(event.pathname)
+
+    def process_IN_CREATE(self, event):
+        """On closing after linking."""
+        if (event.mask & pyinotify.IN_ISDIR):
+            self._watched_dirs.update(self._watchManager.add_watch(event.pathname, self._tmask))
+
+        if self._cmd_filename and os.path.abspath(
+                event.pathname) != self._cmd_filename:
+            return
+        try:
+            if os.stat(event.pathname).st_nlink > 1:
+                self._fun(event.pathname)
+        except OSError:
+            return
+
+    def process_IN_MOVED_TO(self, event):
+        """On closing after moving."""
+        if self._cmd_filename and os.path.abspath(
+                event.pathname) != self._cmd_filename:
+            return
+        self._fun(event.pathname)
+
+    def process_IN_DELETE(self, event):
+        """On delete."""
+        if (event.mask & pyinotify.IN_ISDIR):
+            try:
+                try:
+                    self._watchManager.rm_watch(self._watched_dirs[event.pathname], quiet=False)
+                except pyinotify.WatchManagerError:
+                    # As the directory is deleted prior removing the
+                    # watch will cause a error message from
+                    # pyinotify. This is ok, so just pass the
+                    # exception.
+                    pass
+                finally:
+                    del self._watched_dirs[event.pathname]
+            except KeyError:
+                LOGGER.warning(
+                    "Dir %s not watched by inotify. Can not delete watch.",
+                    event.pathname)
+        return
+
+
+def process_old_files(pattern, fun, publisher, kwargs):
+    """Process files from *pattern* with function *fun*."""
+    fnames = glob.glob(pattern)
+    if fnames:
+        # time.sleep(3)
+        LOGGER.debug("Touching old files")
+        for fname in fnames:
+            if os.path.exists(fname):
+                fun(fname, publisher, pattern, kwargs)
+
+
 def terminate(chains, publisher=None):
     """Terminate the given *chains* and stop the *publisher*."""
     for chain in chains.values():
         chain["notifier"].stop()
         try:
             # Join the Watchdog thread
             chain["notifier"].join()
```

### Comparing `trollmoves-0.9.0/trollmoves/utils.py` & `trollmoves-7.0.0/trollmoves/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#
+
 # Copyright (c) 2018, 2020
-#
+
 # Author(s):
-#
+
 #   Martin Raspaud <martin.raspaud@smhi.se>
-#
+
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
-#
+
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-#
+
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+import netifaces
+from six import string_types
 import socket
-from urllib.parse import urlparse, urlunparse
 
-import netifaces
+from six.moves.urllib.parse import urlparse, urlunparse
 
 
 def clean_url(url):
     """Remove login info from *url*."""
-    if isinstance(url, str):
+    if isinstance(url, string_types):
         urlobj = urlparse(url)
     else:
         urlobj = url
     return urlunparse((urlobj.scheme, urlobj.hostname,
                        urlobj.path, "", "", ""))
 
 
@@ -123,11 +124,12 @@
         return newvar
     else:
         return var
 
 
 def is_file_local(urlobj):
     """Check that a url path is for a local file."""
-    if(urlobj.scheme not in ['', 'file'] and not socket.gethostbyname(urlobj.netloc) in get_local_ips()):
+    if(urlobj.scheme not in ['', 'file']
+       and not socket.gethostbyname(urlobj.netloc) in get_local_ips()):
         return False
 
     return True
```

### Comparing `trollmoves-0.9.0/trollmoves.egg-info/PKG-INFO` & `trollmoves-7.0.0/trollmoves.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: trollmoves
-Version: 0.9.0
+Version: 7.0.0
 Summary: Pytroll file utilities
 Home-page: https://github.com/pytroll/trollmoves
 Author: Martin Raspaud
 Author-email: martin.raspaud@smhi.se
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `trollmoves-0.9.0/trollmoves.egg-info/SOURCES.txt` & `trollmoves-7.0.0/trollmoves.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trollmoves-0.9.0/versioneer.py` & `trollmoves-7.0.0/versioneer.py`

 * *Files identical despite different names*

