# Comparing `tmp/opb-32.tar.gz` & `tmp/opb-33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opb-32.tar", last modified: Thu Apr 13 12:46:06 2023, max compression
+gzip compressed data, was "opb-33.tar", last modified: Thu Apr 27 14:41:09 2023, max compression
```

## Comparing `opb-32.tar` & `opb-33.tar`

### file list

```diff
@@ -1,57 +1,44 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.374288 opb-32/
--rw-r--r--   0 bart      (1000) bart      (1001)       52 2023-04-13 12:34:46.000000 opb-32/MANIFEST.in
--rw-r--r--   0 bart      (1000) bart      (1001)     7042 2023-04-13 12:46:06.370288 opb-32/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4672 2023-04-13 12:45:02.000000 opb-32/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2395 2023-04-13 12:34:46.000000 opb-32/bin/opb
--rwxr-xr-x   0 bart      (1000) bart      (1001)      936 2023-04-13 12:39:42.000000 opb-32/bin/opbc
--rwxr-xr-x   0 bart      (1000) bart      (1001)      209 2023-04-13 12:34:46.000000 opb-32/bin/opbctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1147 2023-04-13 12:34:46.000000 opb-32/bin/opbd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      301 2023-04-13 12:34:46.000000 opb-32/files/opb.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/mod/
--rw-r--r--   0 bart      (1000) bart      (1001)      184 2023-04-13 12:34:46.000000 opb-32/mod/dbg.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2931 2023-04-13 12:34:46.000000 opb-32/mod/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17762 2023-04-13 12:34:46.000000 opb-32/mod/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2353 2023-04-13 12:34:46.000000 opb-32/mod/req.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2339 2023-04-13 12:34:46.000000 opb-32/mod/shl.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2461 2023-04-13 12:34:46.000000 opb-32/mod/udp.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5693 2023-04-13 12:34:46.000000 opb-32/mod/wsd.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 12:34:46.000000 opb-32/modules/__init__.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/opb/
--rw-r--r--   0 bart      (1000) bart      (1001)       97 2023-04-13 12:34:46.000000 opb-32/opb/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-13 12:34:46.000000 opb-32/opb/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5943 2023-04-13 12:34:46.000000 opb-32/opb/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/opb/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 12:34:46.000000 opb-32/opb/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-13 12:34:46.000000 opb-32/opb/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      410 2023-04-13 12:34:46.000000 opb-32/opb/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-13 12:34:46.000000 opb-32/opb/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1136 2023-04-13 12:34:46.000000 opb-32/opb/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    16371 2023-04-13 12:34:46.000000 opb-32/opb/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      900 2023-04-13 12:34:46.000000 opb-32/opb/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7736 2023-04-13 12:34:46.000000 opb-32/opb/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      344 2023-04-13 12:34:46.000000 opb-32/opb/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1003 2023-04-13 12:34:46.000000 opb-32/opb/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      996 2023-04-13 12:34:46.000000 opb-32/opb/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-13 12:34:46.000000 opb-32/opb/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2638 2023-04-13 12:34:46.000000 opb-32/opb/modules/usr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4838 2023-04-13 12:34:46.000000 opb-32/opb/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-13 12:34:46.000000 opb-32/opb/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-13 12:34:46.000000 opb-32/opb/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-13 12:34:46.000000 opb-32/opb/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-13 12:34:46.000000 opb-32/opb/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/opb.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7042 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      770 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-13 12:46:06.374288 opb-32/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1556 2023-04-13 12:34:46.000000 opb-32/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-13 12:34:46.000000 opb-32/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-13 12:34:46.000000 opb-32/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-13 12:34:46.000000 opb-32/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-13 12:34:46.000000 opb-32/test/test_objects.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-27 14:41:09.089810 opb-33/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7144 2023-04-27 14:41:09.089810 opb-33/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4768 2023-04-27 14:05:11.000000 opb-33/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-27 14:41:09.085810 opb-33/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2653 2023-04-27 14:10:30.000000 opb-33/bin/opb
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      861 2023-04-26 14:31:53.000000 opb-33/bin/opbc
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1089 2023-04-26 14:32:18.000000 opb-33/bin/opbd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-27 14:41:09.085810 opb-33/opb/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-25 10:38:03.000000 opb-33/opb/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-25 10:38:03.000000 opb-33/opb/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-04-25 10:38:03.000000 opb-33/opb/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-27 14:41:09.085810 opb-33/opb/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-25 10:38:10.000000 opb-33/opb/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-25 10:38:10.000000 opb-33/opb/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-25 10:38:10.000000 opb-33/opb/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1130 2023-04-25 10:37:50.000000 opb-33/opb/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17599 2023-04-25 10:38:10.000000 opb-33/opb/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      918 2023-04-25 10:38:10.000000 opb-33/opb/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7792 2023-04-25 10:38:10.000000 opb-33/opb/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-25 10:38:10.000000 opb-33/opb/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1022 2023-04-25 10:38:10.000000 opb-33/opb/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-25 10:38:10.000000 opb-33/opb/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-25 10:38:10.000000 opb-33/opb/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2657 2023-04-25 10:38:10.000000 opb-33/opb/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-25 10:38:03.000000 opb-33/opb/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4769 2023-04-27 13:57:10.000000 opb-33/opb/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      380 2023-04-26 10:56:40.000000 opb-33/opb/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-25 10:38:03.000000 opb-33/opb/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-25 10:38:03.000000 opb-33/opb/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-25 10:38:03.000000 opb-33/opb/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-27 14:41:09.085810 opb-33/opb.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7144 2023-04-27 14:41:09.000000 opb-33/opb.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      658 2023-04-27 14:41:09.000000 opb-33/opb.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-27 14:41:09.000000 opb-33/opb.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       16 2023-04-27 14:41:09.000000 opb-33/opb.egg-info/namespace_packages.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-27 14:41:09.000000 opb-33/opb.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-27 14:41:09.000000 opb-33/opb.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-27 14:41:09.089810 opb-33/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1631 2023-04-27 14:13:48.000000 opb-33/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-27 14:41:09.085810 opb-33/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-25 10:37:50.000000 opb-33/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-25 10:37:50.000000 opb-33/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-25 10:37:50.000000 opb-33/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-25 10:37:50.000000 opb-33/test/test_objects.py
```

### Comparing `opb-32/PKG-INFO` & `opb-33/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 32
-Summary: object programming bot
+Version: 33
+Summary: operator bot
 Home-page: http://github.com/operbot/opb
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
         
@@ -48,15 +48,17 @@
         
         
         **INSTALL**
         
         
         ::
         
-         $ sudo pip3 install opb
+         $ sudo pip3 install opb --upgrade --force-reinstall
+        
+         (*) use remove and reinstall if ``opb`` doesn't work properly
         
         
         **CONFIGURATION**
         
         
         configuration is done by calling the ``cfg`` command:
         
@@ -173,15 +175,15 @@
         
         ::
         
          sudo cp /usr/local/opb/opb.service
                  /etc/systemd/system``
          sudo systemctl enable opb --now
         
-         default is #opb on localhost
+         (*) default is #opb on localhost
         
         use ``opbctl <cmd>`` as you would have use ``opb <cmd>``.
         
         
         **PROGRAMMING**
```

### Comparing `opb-32/README.rst` & `opb-33/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 
 
 **INSTALL**
 
 
 ::
 
- $ sudo pip3 install opb
+ $ sudo pip3 install opb --upgrade --force-reinstall
+
+ (*) use remove and reinstall if ``opb`` doesn't work properly
 
 
 **CONFIGURATION**
 
 
 configuration is done by calling the ``cfg`` command:
 
@@ -165,15 +167,15 @@
 
 ::
 
  sudo cp /usr/local/opb/opb.service
          /etc/systemd/system``
  sudo systemctl enable opb --now
 
- default is #opb on localhost
+ (*) default is #opb on localhost
 
 use ``opbctl <cmd>`` as you would have use ``opb <cmd>``.
 
 
 **PROGRAMMING**
```

### Comparing `opb-32/bin/opb` & `opb-33/bin/opb`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,C0413,W0212,E0611,E0401,I1101
-
-
-'object programming bot'
+# pylint: disable=C0114,C0115,C0116,C0413,W0212,E0611,E0401,I1101
 
 
 import os
+import readline
 import sys
 import termios
 import time
 import traceback
 
 
 sys.path.insert(0, os.getcwd())
 
 
+readline.redisplay()
+
+
 import opb.modules
 
 
 from opb.handler import Client, Error, command, parse
+from opb.loggers import Logging
+from opb.objects import update
+from opb.persist import Persist
+from opb.runtime import Cfg, date
 from opb.scanner import importer, scandir, scanpkg, starter
 from opb.threads import launch
 
 
-MOD = "cmd,err,irc,rss,sts,thr"
+def cprint(txt):
+    if "v" in Cfg.opts:
+        print(txt)
+        sys.stdout.flush()
+
+
+Logging.raw = cprint
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
@@ -86,32 +97,34 @@
             termios.tcsetattr(fds, termios.TCSADRAIN, old)
         waiter()
 
 
 def main():
     dowait = False
     cfg = parse(' '.join(sys.argv[1:]))
+    update(Cfg, cfg)
+    mod = Cfg.sets.mod
     if os.path.exists("modules"):
-        scandir("modules", importer, cfg.mod or MOD)
-    scanpkg(opb.modules, importer, cfg.mod or MOD)
+        scandir("modules", importer, mod + Cfg.mod)
+    scanpkg(opb.modules, importer, mod + Cfg.mod)
     if cfg.txt:
         cli = CLI()
         command(cli, cfg.otxt)
     elif 'd' in cfg.opts:
         daemon()
         dowait = True
     elif 'c' in cfg.opts:
-        date = time.ctime(time.time()).replace('  ', ' ')
-        print(f'OPB started {date}')
-        csl = Console()
-        launch(csl.loop)
+        print(f'{Cfg.name.upper()} started {date}')
         dowait = True
     if dowait:
-        scanpkg(opb.modules, starter, cfg.mod or MOD)
-        scandir("modules", starter, cfg.mod or MOD)
+        scanpkg(opb.modules, starter, mod + Cfg.mod)
+        scandir("modules", starter, mod + Cfg.mod)
+        if "c" in cfg.opts:
+            csl = Console()
+            launch(csl.loop)
         while 1:
             time.sleep(1.0)
             waiter()
 
 
 wrap(main)
 waiter()
```

### Comparing `opb-32/opb/clocked.py` & `opb-33/opb/clocked.py`

 * *Files identical despite different names*

### Comparing `opb-32/opb/handler.py` & `opb-33/opb/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,21 @@
     def byorig(orig):
         for obj in Listens.objs:
             if repr(obj) == orig:
                 return obj
         return None
 
     @staticmethod
+    def remove(bot):
+        try:
+            Listens.objs.remove(bot)
+        except ValueError:
+            pass
+
+    @staticmethod
     def say(orig, txt, channel=None):
         bot = Listens.byorig(orig)
         if bot:
             if channel:
                 bot.say(channel, txt)
             else:
                 bot.raw(txt)
```

### Comparing `opb-32/opb/modules/fnd.py` & `opb-33/opb/modules/fnd.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 'locate objects'
 
 
 import time
 
 
-from opb.clocked import elapsed
-from opb.objects import keys, prt
-from opb.persist import files, find, fntime
+from ..clocked import elapsed
+from ..objects import keys, prt
+from ..persist import files, find, fntime
 
 
 def __dir__():
     return (
             'fnd',
            )
```

### Comparing `opb-32/opb/modules/irc.py` & `opb-33/opb/modules/irc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915,E0402
+# pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915
+# pylint: disable=E0402,E0401
 
 
 'internet relay chat'
 
 
 import base64
 import os
@@ -13,59 +14,65 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from opb.handler import Client, Command, Error, Event
-from opb.objects import Default, Object, keys, prt, update
-from opb.persist import last, write
-from opb.threads import launch
+from ..handler import Client, Command, Error, Event, Listens
+from ..loggers import Logging
+from ..objects import Default, Object, edit, keys, prt
+from ..persist import Class, last, write
+from ..runtime import Cfg
+from ..threads import launch
 
 
-from opb.modules.usr import Users
+from .usr import Users
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
             'cfg',
             'mre',
             'pwd',
             'start'
            )
 
 
-NAME = "opb"
-
-
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
+    if "v" in Cfg.opts:
+        Logging.debug(prt(
+                          irc.cfg,
+                          ",".join(keys(irc.cfg)),
+                          skip='control,password,realname,sleep,username')
+                         )
+        irc.joined.wait()
     return irc
 
 
 class Config(Default):
 
-    channel = '#%s' % NAME
+    channel = '#%s' % Cfg.name
     control = '!'
-    nick = NAME
+    nick = Cfg.name
     password = ''
     port = 6667
-    realname = NAME
+    realname = Cfg.name
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = NAME
+    username = Cfg.name
     users = False
 
     def __init__(self):
         Default.__init__(self)
         self.control = Config.control
         self.channel = Config.channel
         self.nick = Config.nick
@@ -76,14 +83,17 @@
         self.server = Config.server
         self.servermodes = Config.servermodes
         self.sleep = Config.sleep
         self.username = Config.username
         self.users = Config.users
 
 
+Class.add(Config)
+
+
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = True
         self.fix_sentence_endings = True
@@ -96,14 +106,16 @@
 
     cache = Object()
 
     def __init__(self):
         Object.__init__(self)
         self.oqueue = queue.Queue()
         self.dostop = threading.Event()
+        self.state = Default()
+        self.state.starttime = time.time()
 
     def dosay(self, channel, txt):
         raise NotImplementedError
 
     def extend(self, channel, txtlist):
         if channel not in self.cache:
             setattr(self.cache, channel, [])
@@ -163,14 +175,15 @@
 class IRC(Client, Output):
 
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
+        self.authed = threading.Event()
         self.connected = threading.Event()
         self.channels = []
         self.joined = threading.Event()
         self.keeprunning = False
         self.outqueue = queue.Queue()
         self.sock = None
         self.speed = 'slow'
@@ -179,14 +192,15 @@
         self.state.errors = []
         self.state.last = 0
         self.state.lastline = ''
         self.state.nrconnect = 0
         self.state.nrerror = 0
         self.state.nrsend = 0
         self.state.pongcheck = False
+        self.state.starttime = time.time()
         self.threaded = False
         self.zelf = ''
         self.register('903', self.h903)
         self.register('904', self.h903)
         self.register('AUTHENTICATE', self.auth)
         self.register('CAP', self.cap)
         self.register('ERROR', self.error)
@@ -198,19 +212,18 @@
         self.target = 'type'
 
     def announce(self, txt):
         for channel in self.channels:
             self.say(channel, txt)
 
     def auth(self, event):
-        time.sleep(1.0)
+        assert self.cfg.password
         self.direct('AUTHENTICATE %s' % self.cfg.password)
 
     def cap(self, event):
-        time.sleep(1.0)
         if self.cfg.password and 'ACK' in event.arguments:
             self.direct('AUTHENTICATE PLAIN')
         else:
             self.direct('CAP REQ :sasl')
 
     def command(self, cmd, *args):
         with saylock:
@@ -243,38 +256,52 @@
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
             self.sock.connect((server, port))
             self.command('CAP LS 302')
         else:
             addr = socket.getaddrinfo(server, port, socket.AF_INET)[-1][-1]
             self.sock = socket.create_connection(addr)
+            self.authed.set()
         if self.sock:
             os.set_inheritable(self.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.connected.set()
             return True
         return False
 
+
     def direct(self, txt):
-        self.sock.send(bytes(txt+'\n', 'utf-8'))
+        Logging.debug(txt)
+        self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
-        self.sock.shutdown(2)
+        try:
+            self.sock.shutdown(2)
+        except (
+                ssl.SSLError,
+                OSError,
+                BrokenPipeError
+               ) as ex:
+            Error.errors.append(ex)
 
     def docommand(self, evt):
         evt.orig = repr(self)
         Command.handle(evt)
 
     def doconnect(self, server, nck, port=6667):
         while 1:
             try:
                 if self.connect(server, port):
                     break
-            except (ssl.SSLError, OSError, ConnectionResetError) as ex:
+            except (
+                    ssl.SSLError,
+                    OSError,
+                    ConnectionResetError
+                   ) as ex:
                 self.state.errors = str(ex)
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def dosay(self, channel, txt):
         self.joined.wait()
         txt = str(txt).replace('\n', '')
@@ -311,20 +338,20 @@
             self.command('NICK', nck)
         return evt
 
     def fileno(self):
         return self.sock.fileno()
 
     def h903(self, event):
-        time.sleep(1.0)
         self.command('CAP END')
+        self.authed.set()
 
     def h904(self, event):
-        time.sleep(1.0)
         self.command('CAP END')
+        self.authed.set()
 
     def joinall(self):
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
         while 1:
@@ -332,24 +359,28 @@
             self.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 self.state.pongcheck = False
                 self.keeprunning = False
-                self.reconnect()
-
+                self.connected.clear()
+                self.stop()
+                start()
+                break
 
     def logon(self, server, nck):
+        self.connected.wait()
+        self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username or "opb",
+                 'USER %s %s %s :%s' % (self.cfg.username or Cfg.name,
                  server,
                  server,
-                 self.cfg.realname or "opb")
+                 self.cfg.realname or Cfg.name)
                 )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
@@ -414,28 +445,35 @@
             obj.txt = arguments[1]
         spl = obj.txt.split()
         if len(spl) > 1:
             obj.args = spl[1:]
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
+        Logging.debug(rawstr)
         return obj
 
     def poll(self):
         self.connected.wait()
         if not self.buffer:
             try:
                 self.some()
-            except (ssl.SSLError, socket.timeout, ConnectionResetError) as ex:
-                self.joined.clear()
-                time.sleep(5.0)
-                evt = Event()
-                evt.txt = str(ex)
-                evt.orig = repr(self)
-                return evt
+            except BlockingIOError as ex:
+                time.sleep(1.0)
+                return self.event(str(ex))
+            except (
+                    socket.timeout,
+                    ssl.SSLError,
+                    ssl.SSLZeroReturnError,
+                    ConnectionResetError,
+                    BrokenPipeError
+                   ) as ex:
+                Error.errors.append(ex)
+                self.stop()
+                return self.event(str(ex))
         return self.event(self.buffer.pop(0))
 
     def privmsg(self, event):
         if event.txt:
             if event.txt[0] in [self.cfg.control, '!']:
                 event.txt = event.txt[1:]
             elif event.txt.startswith('%s:' % self.cfg.nick):
@@ -451,28 +489,29 @@
 
     def quit(self, event):
         if event.orig and event.orig in self.zelf:
             self.stop()
 
     def raw(self, txt):
         txt = txt.rstrip()
+        Logging.debug(txt)
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
                     ssl.SSLError,
+                    ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                time.sleep(5.0)
                 Error.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
@@ -508,40 +547,39 @@
         self.connected.clear()
         self.joined.clear()
         launch(Client.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
-               self.cfg.nick or "opb",
+               self.cfg.nick or Cfg.name,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        try:
-            self.sock.shutdown(2)
-        except(ssl.SSLError,  OSError):
-            pass
+        Logging.debug("stopping")
+        Listens.remove(self)
         Client.stop(self)
         Output.stop(self)
+        self.disconnect()
 
 
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(prt(
                         config,
                         keys(config),
                         skip='control,password,realname,sleep,username')
                        )
     else:
-        update(config, event.sets)
+        edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
```

### Comparing `opb-32/opb/modules/log.py` & `opb-33/opb/modules/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 'log'
 
 
 import time
 
 
-from opb.clocked import elapsed
-from opb.persist import find, fntime, write
-from opb.objects import Object
+from ..clocked import elapsed
+from ..persist import Class, find, fntime, write
+from ..objects import Object
 
 
 def __dir__():
     return (
             'Log',
             'log',
            )
@@ -23,14 +23,17 @@
 class Log(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
+Class.add(Log)
+
+
 def log(event):
     if not event.rest:
         nmr = 0
         for obj in find('log'):
             event.reply('%s %s %s' % (
                                       nmr,
                                       obj.txt,
```

### Comparing `opb-32/opb/modules/rss.py` & `opb-33/opb/modules/rss.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from opb.clocked import Repeater, elapsed
-from opb.handler import Listens, spl
-from opb.objects import Object, prt, update
-from opb.persist import find, fntime, last, write
-from opb.threads import launch, threaded
+from ..clocked import Repeater, elapsed
+from ..handler import Listens, spl
+from ..objects import Object, prt, update
+from ..persist import Class, find, fntime, last, write
+from ..runtime import Cfg
+from ..threads import launch, threaded
 
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
@@ -62,21 +63,27 @@
     def __init__(self):
         super().__init__()
         self.display_list = 'title,link,author'
         self.name = ''
         self.rss = ''
 
 
+Class.add(Rss)
+
+
 class Seen(Object):
 
     def __init__(self):
         super().__init__()
         self.urls = []
 
 
+Class.add(Seen)
+
+
 class Fetcher(Object):
 
     dosave = False
     seen = Seen()
 
     def __init__(self):
         super().__init__()
@@ -182,15 +189,15 @@
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
 def getfeed(url, item):
-    if DEBUG:
+    if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
     if not result:
         return [Object(), Object()]
@@ -213,15 +220,15 @@
             return i.groups()
     return []
 
 
 def geturl(url):
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
-    req.add_header('User-agent', useragent('OPB - object programming bot'))
+    req.add_header('User-agent', useragent('OPERBOT - operator bot'))
     response = urllib.request.urlopen(req)
     response.data = response.read()
     return response
 
 
 def striphtml(text):
     clean = re.compile('<.*?>')
```

### Comparing `opb-32/opb/modules/tdo.py` & `opb-33/opb/modules/tdo.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 'todo'
 
 
 import time
 
 
-from opb.clocked import elapsed
-from opb.objects import Object
-from opb.persist import find, fntime, write
+from ..clocked import elapsed
+from ..objects import Object
+from ..persist import Class, find, fntime, write
 
 
 class Todo(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
+Class.add(Todo)
+
+
 def dne(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
     for obj in find('todo', selector):
         obj.__deleted__ = True
         write(obj)
```

### Comparing `opb-32/opb/modules/thr.py` & `opb-33/opb/modules/thr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0114,C0115,C0116,E1101,E0402
 
 
-"list running commands."
+"list running threads."
 
 
 import threading
 import time
 
 
-from opb.clocked import elapsed
-from opb.objects import Object, update
+from ..clocked import elapsed
+from ..objects import Object, update
 
 
 def __dir__():
     return (
             'thr',
            )
 
@@ -30,14 +30,16 @@
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
             uptime = obj.sleep - int(time.time() - obj.state.latest)
+        elif getattr(obj, 'starttime', None):
+            uptime = int(time.time() - obj.starttime)
         else:
             uptime = int(time.time() - starttime)
         result.append((uptime, thread.name))
     res = []
     for uptime, txt in sorted(result, key=lambda x: x[0]):
         res.append('%s/%s' % (txt, elapsed(uptime)))
     if res:
```

### Comparing `opb-32/opb/modules/usr.py` & `opb-33/opb/modules/usr.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 'users'
 
 
 import time
 
 
-from opb.clocked import elapsed
-from opb.objects import Object, update
-from opb.persist import find, fntime, write
+from ..clocked import elapsed
+from ..objects import Object, update
+from ..persist import Class, find, fntime, write
 
 
 def __dir__():
     return (
             'NoUser',
             'Users',
             'User',
@@ -81,14 +81,17 @@
         Object.__init__(self)
         self.user = ''
         self.perms = []
         if val:
             update(self, val)
 
 
+Class.add(User)
+
+
 def dlt(event):
     if not event.args:
         event.reply('dlt <username>')
         return
     selector = {'user': event.args[0]}
     for obj in find('user', selector):
         obj.__deleted__ = True
```

### Comparing `opb-32/opb/objects.py` & `opb-33/opb/objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 def __dir__():
     return (
             'Default',
             'Object',
             'dumps',
+            'edit',
             'items',
             'keys',
             'kind',
             'loads',
             'prt',
             'search',
             'update',
@@ -62,14 +63,45 @@
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
+def edit(obj, setter, skip=False):
+    try:
+        setter = vars(setter)
+    except (TypeError, ValueError):
+        pass
+    if not setter:
+        setter = {}
+    count = 0
+    for key, val in setter.items():
+        if skip and val == "":
+            continue
+        count += 1
+        try:
+            setattr(obj, key, int(val))
+            continue
+        except ValueError:
+            pass
+        try:
+            setattr(obj, key, float(val))
+            continue
+        except ValueError:
+            pass
+        if val in ["True", "true"]:
+            setattr(obj, key, True)
+        elif val in ["False", "false"]:
+            setattr(obj, key, False)
+        else:
+            setattr(obj, key, val)
+    return count
+
+
 def ident(obj):
     return os.path.join(
                         kind(obj),
                         str(uuid.uuid4().hex),
                         os.sep.join(str(datetime.datetime.now()).split()),
                        )
```

### Comparing `opb-32/opb/scanner.py` & `opb-33/opb/scanner.py`

 * *Files identical despite different names*

### Comparing `opb-32/opb/threads.py` & `opb-33/opb/threads.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pylint: disable=C0115,C0116,W0613,E0402
 
 
 'threads'
 
 
 import queue
+import time
 import types
 
 
 from functools import wraps
 from threading import Thread as BasicThread
 
 
@@ -29,14 +30,15 @@
     def __init__(self, func, thrname, *args, daemon=True):
         super().__init__(None, self.run, thrname, (), {}, daemon=daemon)
         self._result = None
         self.name = thrname or name(func)
         self.queue = queue.Queue()
         self.queue.put_nowait((func, args))
         self.sleep = None
+        self.starttime = time.time()
 
     def __iter__(self):
         return self
 
     def __next__(self):
         for k in dir(self):
             yield k
```

### Comparing `opb-32/opb/utility.py` & `opb-33/opb/utility.py`

 * *Files identical despite different names*

### Comparing `opb-32/opb.egg-info/PKG-INFO` & `opb-33/opb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 32
-Summary: object programming bot
+Version: 33
+Summary: operator bot
 Home-page: http://github.com/operbot/opb
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
         
@@ -48,15 +48,17 @@
         
         
         **INSTALL**
         
         
         ::
         
-         $ sudo pip3 install opb
+         $ sudo pip3 install opb --upgrade --force-reinstall
+        
+         (*) use remove and reinstall if ``opb`` doesn't work properly
         
         
         **CONFIGURATION**
         
         
         configuration is done by calling the ``cfg`` command:
         
@@ -173,15 +175,15 @@
         
         ::
         
          sudo cp /usr/local/opb/opb.service
                  /etc/systemd/system``
          sudo systemctl enable opb --now
         
-         default is #opb on localhost
+         (*) default is #opb on localhost
         
         use ``opbctl <cmd>`` as you would have use ``opb <cmd>``.
         
         
         **PROGRAMMING**
```

### Comparing `opb-32/opb.egg-info/SOURCES.txt` & `opb-33/opb.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-MANIFEST.in
 README.rst
 setup.py
 bin/opb
 bin/opbc
-bin/opbctl
 bin/opbd
-files/opb.service
-mod/dbg.py
-mod/mbx.py
-mod/mdl.py
-mod/req.py
-mod/shl.py
-mod/udp.py
-mod/wsd.py
-modules/__init__.py
-opb/__init__.py
 opb/clocked.py
 opb/handler.py
+opb/loggers.py
 opb/objects.py
 opb/persist.py
+opb/runtime.py
 opb/scanner.py
 opb/threads.py
 opb/utility.py
 opb.egg-info/PKG-INFO
 opb.egg-info/SOURCES.txt
 opb.egg-info/dependency_links.txt
+opb.egg-info/namespace_packages.txt
 opb.egg-info/top_level.txt
 opb.egg-info/zip-safe
-opb/modules/__init__.py
 opb/modules/cmd.py
 opb/modules/err.py
 opb/modules/flt.py
 opb/modules/fnd.py
 opb/modules/irc.py
 opb/modules/log.py
 opb/modules/rss.py
```

### Comparing `opb-32/setup.py` & `opb-33/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,32 +27,36 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="opb",
-    version="32",
+    version="33",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/opb",
-    description="object programming bot",
+    description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
     packages=[
               "opb",
               "opb.modules"
              ],
+    namespace_packages=[
+                        "opb",
+                        "opb.modules"
+                       ],
     zip_safe=True,
     include_package_data=True,
     data_files=[
-                ("opb", ["README.rst", "files/opb.service",]),
+                ("opb", ["README.rst",]),
                ],
-    scripts=["bin/opb", "bin/opbc", "bin/opbctl", "bin/opbd"],
+    scripts=["bin/opb", "bin/opbc", "bin/opbd"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: Public Domain",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
         "Intended Audience :: System Administrators",
         "Topic :: Communications :: Chat :: Internet Relay Chat",
```

### Comparing `opb-32/test/test_decoder.py` & `opb-33/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `opb-32/test/test_inherit.py` & `opb-33/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `opb-32/test/test_objects.py` & `opb-33/test/test_objects.py`

 * *Files identical despite different names*

