# Comparing `tmp/xoa-utils-1.1.1.tar.gz` & `tmp/xoa-utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-utils-1.1.1.tar", last modified: Sat Mar  4 03:10:02 2023, max compression
+gzip compressed data, was "xoa-utils-1.2.0.tar", last modified: Thu Apr 27 12:45:03 2023, max compression
```

## Comparing `xoa-utils-1.1.1.tar` & `xoa-utils-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.081513 xoa-utils-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-03-04 03:09:52.000000 xoa-utils-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-03-04 03:10:02.081513 xoa-utils-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-03-04 03:09:52.000000 xoa-utils-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-04 03:10:02.081513 xoa-utils-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/clicks/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/an.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/anlt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/lt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_commands/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clicks/click_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/clis/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/clis/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/cmds/cmd_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/cmds/cmd_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.081513 xoa-utils-1.1.1/xoa_utils/ssh_server/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/ssh_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-04 03:09:53.000000 xoa-utils-1.1.1/xoa_utils/ssh_server/xena_ssh_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:10:02.077513 xoa-utils-1.1.1/xoa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-03-04 03:10:02.000000 xoa-utils-1.1.1/xoa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-04 03:10:02.000000 xoa-utils-1.1.1/xoa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 03:10:02.000000 xoa-utils-1.1.1/xoa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-04 03:10:02.000000 xoa-utils-1.1.1/xoa_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-04 03:10:02.000000 xoa-utils-1.1.1/xoa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-04 03:10:02.000000 xoa-utils-1.1.1/xoa_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.930048 xoa-utils-1.2.0/xoa_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.930048 xoa-utils-1.2.0/xoa_utils/clicks/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/an.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/anlt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/lt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_commands/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clicks/click_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/xoa_utils/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/clis/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/xoa_utils/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/cmds/cmd_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/cmds/cmd_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/xoa_utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/xoa_utils/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.934048 xoa-utils-1.2.0/xoa_utils/ssh_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/ssh_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-27 12:44:50.000000 xoa-utils-1.2.0/xoa_utils/ssh_server/xena_ssh_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:45:03.930048 xoa-utils-1.2.0/xoa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 12:45:03.000000 xoa-utils-1.2.0/xoa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 12:45:03.000000 xoa-utils-1.2.0/xoa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:45:03.000000 xoa-utils-1.2.0/xoa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 12:45:03.000000 xoa-utils-1.2.0/xoa_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-27 12:45:03.000000 xoa-utils-1.2.0/xoa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 12:45:03.000000 xoa-utils-1.2.0/xoa_utils.egg-info/top_level.txt
```

### Comparing `xoa-utils-1.1.1/LICENSE` & `xoa-utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/setup.py` & `xoa-utils-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,31 +22,29 @@
         author_email="rdi@xenanetworks.com, hyu@xenanetworks.com",
         maintainer="Xena Networks",
         maintainer_email="support@xenanetworks.com",
         url="https://github.com/xenanetworks/open-automation-utilities",
         packages=setuptools.find_packages(),
         license="Apache 2.0",
         install_requires=[
-            "xoa-driver>=1.2",
             "typing_extensions>=4.4.0",
             "cffi>=1.15.1",
             "cryptography>=39.0.0",
             "pycparser>=2.21",
             "colorama>=0.4.6",
             "idna>=3.4",
             "asyncssh>=2.13.0",
             "asyncclick>=8.1.3.4",
             "anyio>=3.6.2",
             "loguru>=0.6.0",
             "pdoc>=12.3.1",
             "pytest>=7.2.1",
             "asyncclick>=8.1.3.4",
-            "asyncssh>=2.13.0",
-            "anyio>=3.6.2",
             "psutil>=5.9.4",
+            "xoa-driver>=1.3",
         ],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "Topic :: Software Development :: Libraries :: Python Modules",
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python :: 3.8",
```

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_backend.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_backend.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_commands/__init__.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_commands/an.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_commands/an.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import asyncclick as ac
-from xoa_utils.clicks import click_backend as cb
 from xoa_driver.hlfuncs import anlt as anlt_utils
+from xoa_utils.clicks import click_backend as cb
 from xoa_utils.clis import format_an_status, format_an_config
 from xoa_utils.clicks.click_commands.group import xoa_util
 from xoa_utils.clicks import click_help as h
 from xoa_utils.cmds import CmdContext
 
 
 # --------------------------
```

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_commands/anlt.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_commands/anlt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from __future__ import annotations
 import asyncclick as ac
 import json
 import typing as t
 from xoa_driver.hlfuncs import anlt as anlt_utils
 from xoa_utils.clicks import click_backend as cb
-from xoa_utils.clis import format_recovery, format_port_status
+from xoa_utils.clis import (
+    format_recovery,
+    format_port_status,
+    format_strict,
+    format_log_control
+    )
+from xoa_driver.enums import AnLtLogControl
 from xoa_utils.clicks.click_commands.group import xoa_util
 from xoa_utils.clicks import click_help as h
 from xoa_utils.cmds import CmdContext
 from enum import Enum
 
 
 class ASCIIStyle(Enum):
@@ -79,15 +85,15 @@
     """
     Show AN/LT status of the working port.
     """
     storage: CmdContext = context.obj
     port_obj = storage.retrieve_port()
     status_dic = await anlt_utils.anlt_status(port_obj)
     port_id = storage.retrieve_port_str()
-    return format_port_status(port_id, status_dic, storage)
+    return format_port_status(status_dic, storage)
 
 
 # --------------------------
 # command: do
 # --------------------------
 @anlt.command(cls=cb.XenaCommand)
 @ac.pass_context
@@ -113,17 +119,17 @@
         lt_initial_modulations,
         lt_interactive,
         lt_algorithm,
     )
     return ""
 
 
-# **************************
+# --------------------------
 # command: log
-# **************************
+# --------------------------
 @anlt.command(cls=cb.XenaCommand, name="log")
 @ac.option(
     "-f", "--filename", type=ac.STRING, help=h.HELP_ANLT_LOG_FILENAME, default=""
 )
 @ac.option(
     "-k",
     "--keep",
@@ -233,14 +239,15 @@
             )
             log_ufmt_fec = _dict_get(
                 i, "entry", "pkt", "fields", "un-formatted message", "fec"
             )
             log_ufmt_ab = _dict_get(
                 i, "entry", "pkt", "fields", "un-formatted message", "ability"
             )
+            log_errors = _dict_get(i, "entry", "pkt", "errors")
 
             if log_pkt_locked == "true":
                 log_pkt_locked = _ascii_styler(log_pkt_locked, [ASCIIStyle.GREEN_BG])
             else:
                 log_pkt_locked = _ascii_styler(log_pkt_locked, [ASCIIStyle.RED_BG])
 
             log_pkt_done = _dict_get(i, "entry", "pkt", "fields", "done")
@@ -248,15 +255,15 @@
                 log_pkt_done = _ascii_styler(log_pkt_done, [ASCIIStyle.GREEN_BG])
             else:
                 log_pkt_done = _ascii_styler(log_pkt_done, [ASCIIStyle.RED_BG])
 
             log_pkt_value = _dict_get(i, "entry", "pkt", "value")
 
             serdes_str = f"(S{log_serdes})," if "LT" in log_m else ","
-            common = f"{log_time/1000000}, {log_m}{serdes_str}"
+            common = f"{log_time/1000000:.6f}, {log_m}{serdes_str}"
 
             if log_type == "debug":
                 b_str = f"{common:<32}{'DBG:':<5}{log_log}"
             elif log_type == "fsm":
                 b_str = (
                     f"{common:<32}{'FSM:':<5}({log_event}) {log_current} -> {log_new}"
                 )
@@ -267,17 +274,25 @@
                     if log_ptype == "base page":
                         b_str = f"{common:<32}{(log_direction + ':'):<14}{log_value}, {log_ptype}, NP:{int(log_np, 0)}, ACK:{int(log_ack, 0)}, RF:{int(log_rf, 0)}, TN:{int(log_tn, 0)}, EN:{int(log_en ,0)}, C:{int(log_c, 0)}\n{'':<37}FEC:{log_fec}, ABILITY:{log_ab}"
                     else:
                         if log_fmt_v:
                             b_str = f"{common:<32}{(log_direction + ':'):<14}{log_value}, {log_ptype}, NP:{int(log_np, 0)}, ACK:{int(log_ack, 0)}, MP:{int(log_mp, 0)}, ACK2:{int(log_ack2, 0)}, T:{int(log_t ,0)}\n{'':<37}Formatted message:\n{'':<37}Value:{log_fmt_v}, Msg:{log_fmt_msg}"
                         else:
                             b_str = f"{common:<32}{(log_direction + ':'):<14}{log_value}, {log_ptype}, NP:{int(log_np, 0)}, ACK:{int(log_ack, 0)}, MP:{int(log_mp, 0)}, ACK2:{int(log_ack2, 0)}, T:{int(log_t ,0)}\n{'':<37}Un-formatted message:\n{'':<37}Value:{log_ufmt_v}, Msg:{log_ufmt_msg}\n{'':<37}FEC:{log_ufmt_fec}, ABILITY:{log_ufmt_ab}"
+                    if log_errors:
+                        b_str += "\n" + f"{'':<37}" + _ascii_styler("ERRORS:", [ASCIIStyle.RED_BG]) + f"{log_errors}"
+
             elif log_type == "trace" and "direction" in log_entry and "LT" in log_m:
                 if log_pstate == "new" or log_pstate == "":
-                    b_str = f"{common:<32}{(log_direction + ':'):<14}{log_pkt_value}, LOCKED={log_pkt_locked}, DONE={log_pkt_done}\n{'':<37}{_flatten(log_pkt_ctrl)}\n{'':<37}{_flatten(log_pkt_status)}"
+                    b_str = f"{common:<32}{(log_direction + ':'):<14}{log_pkt_value}, LOCKED={log_pkt_locked}, TRAINED={log_pkt_done}\n{'':<37}{_flatten(log_pkt_ctrl)}\n{'':<37}{_flatten(log_pkt_status)}"
+                    if log_errors:
+                        b_str += "\n" + f"{'':<37}" + _ascii_styler("ERRORS:", [ASCIIStyle.RED_BG]) + f"{log_errors}"
+            elif log_type == "xla":
+                log_xla = _ascii_styler("XLA", [ASCIIStyle.RED_BG])
+                b_str = f"{common:<32}{(log_xla + ': '):<5}{log_log}"
 
             if b_str:
                 real.append(b_str)
         return "\n".join(real)
 
     async def log(
         storage: CmdContext, filename: str, keep: str, serdes: list[int]
@@ -292,7 +307,105 @@
         return string
 
     real_serdes_list = [int(i.strip()) for i in serdes.split(",")] if serdes else []
     kw = {"filename": filename, "keep": keep, "serdes": real_serdes_list}
     storage: CmdContext = ctx.obj
     storage.set_loop_coro(log, kw)
     return ""
+
+
+# --------------------------
+# command: strict
+# --------------------------
+@anlt.command(cls=cb.XenaCommand)
+@ac.option("--on/--off", type=ac.BOOL, help=h.HELP_STRICT_ON, default=True)
+@ac.pass_context
+async def strict(context: ac.Context, on: bool) -> str:
+    """
+    ANLT strict mode ignores errored frames.
+    """
+    storage: CmdContext = context.obj
+
+    port_obj = storage.retrieve_port()
+    await anlt_utils.anlt_strict(port_obj, on)
+    return format_strict(storage, on)
+
+# --------------------------
+# command: log-ctrl
+# --------------------------
+@anlt.command(cls=cb.XenaCommand)
+@ac.option("-D/-d", "--debug/--no-debug", type=ac.BOOL, help=h.HELP_LOG_CONTROL_DEBUG_ON, default=True)
+@ac.option("-A/-a", "--an-trace/--no-an-trace", type=ac.BOOL, help=h.HELP_LOG_CONTROL_AN_TRACE_ON, default=True)
+@ac.option("-L/-l", "--lt-trace/--no-lt-trace", type=ac.BOOL, help=h.HELP_LOG_CONTROL_LT_TRACE_ON, default=True)
+@ac.option("-G/-g", "--alg-trace/--no-alg-trace", type=ac.BOOL, help=h.HELP_LOG_CONTROL_ALG_TRACE_ON, default=True)
+@ac.option("-P/-p", "--fsm-port/--no-fsm-port", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_PORT_ON, default=False)
+@ac.option("-N/-n", "--fsm-an/--no-fsm-an", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_AN_ON, default=True)
+@ac.option("-M/-m", "--fsm-an-stimuli/--no-fsm-an-stimuli", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_AN_STIMULI_ON, default=False)
+@ac.option("-T/-t", "--fsm-lt/--no-fsm-lt", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_LT_ON, default=True)
+@ac.option("-C/-c", "--fsm-lt-coeff/--no-fsm-lt-coeff", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_LT_COEFF_ON, default=False)
+@ac.option("-S/-s", "--fsm-lt-stimuli/--no-fsm-lt-stimuli", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_LT_STIMULI_ON, default=False)
+@ac.option("-Z/-z", "--fsm-lt-alg0/--no-fsm-lt-alg0", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_LT_ALG0_ON, default=True)
+@ac.option("-O/-o", "--fsm-lt-algn1/--no-fsm-lt-algn1", type=ac.BOOL, help=h.HELP_LOG_CONTROL_FSM_LT_ALGN1_ON, default=True)
+@ac.pass_context
+async def log_ctrl(
+    context: ac.Context, 
+    debug: bool, 
+    an_trace: bool, 
+    lt_trace: bool, 
+    alg_trace: bool,
+    fsm_port: bool,
+    fsm_an: bool,
+    fsm_an_stimuli: bool,
+    fsm_lt: bool,
+    fsm_lt_coeff: bool,
+    fsm_lt_stimuli: bool,
+    fsm_lt_alg0: bool,
+    fsm_lt_algn1: bool,
+    ) -> str:
+    """
+    Control what should be logged in ANLT by xenaserver
+    """
+    storage: CmdContext = context.obj
+    port_obj = storage.retrieve_port()
+    types = []
+    if debug:
+        types.append(AnLtLogControl.LOG_TYPE_DEBUG)
+    if an_trace:
+        types.append(AnLtLogControl.LOG_TYPE_AN_TRACE)
+    if lt_trace:
+        types.append(AnLtLogControl.LOG_TYPE_LT_TRACE)
+    if alg_trace:
+        types.append(AnLtLogControl.LOG_TYPE_ALG_TRACE)
+    if fsm_port:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_PORT)
+    if fsm_an:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_ANEG)
+    if fsm_an_stimuli:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_ANEG_STIMULI)
+    if fsm_lt:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_LT)
+    if fsm_lt_coeff:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_LT_COEFF)
+    if fsm_lt_stimuli:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_LT_STIMULI)
+    if fsm_lt_alg0:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_LT_ALG0)
+    if fsm_lt_algn1:
+        types.append(AnLtLogControl.LOG_TYPE_FSM_LT_ALG1)
+
+
+    await anlt_utils.anlt_log_control(port_obj, types)
+    return format_log_control(
+        storage, 
+        debug, 
+        an_trace, 
+        lt_trace, 
+        alg_trace,
+        fsm_port,
+        fsm_an,
+        fsm_an_stimuli,
+        fsm_lt,
+        fsm_lt_coeff,
+        fsm_lt_stimuli,
+        fsm_lt_alg0,
+        fsm_lt_algn1
+        )
```

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_commands/lt.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_commands/lt.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,19 @@
     Set initial modulation for the specified serdes.
 
         <SERDES>: Specifies the transceiver serdes index.
 
         <ENCODING>: Specifies the initial modulation. Allowed values: nrz | pam4 | pam4pre
     """
     storage: CmdContext = context.obj
-    storage.retrieve_port()
+    port_obj = storage.retrieve_port()
     storage.validate_current_serdes(serdes)
     storage.store_lt_initial_mod(serdes, encoding)
-    return format_lt_im(storage, serdes)
+    status_dic = await anlt_utils.lt_im_status(port_obj)
+    return format_lt_im(status_dic, storage, serdes)
 
 
 # **************************
 # sub-command: lt alg
 # **************************
 @lt.command(cls=cb.XenaCommand, name="alg")
 @ac.argument("serdes", type=ac.INT)
@@ -97,18 +98,19 @@
     Set the link training algorithm for the specified serdes.
 
         <SERDES>: Specifies the transceiver serdes index.
 
         <ALGORITHM>: Specifies the algorithm. Allowed values: alg0 | algn1
     """
     storage: CmdContext = context.obj
-    storage.retrieve_port()
+    port_obj = storage.retrieve_port()
     storage.validate_current_serdes(serdes)
     storage.store_lt_algorithm(serdes, algorithm)
-    return format_lt_algorithm(storage, serdes)
+    status_dic = await anlt_utils.lt_algorithm_status(port_obj)
+    return format_lt_algorithm(status_dic, storage, serdes)
 
 
 # **************************
 # Type: Control
 # **************************
 # **************************
 # sub-command: lt inc
@@ -222,15 +224,15 @@
     port_obj = storage.retrieve_port()
     storage.validate_current_serdes(serdes)
     resp = await anlt_utils.lt_trained(port_obj, serdes)
     return format_lt_trained(storage, serdes, resp.name)
 
 
 # **************************
-# sub-command: txtapget
+# sub-command: lt txtapget
 # **************************
 @lt.command(cls=cb.XenaCommand, name="txtapget")
 @ac.argument("serdes", type=ac.INT)
 @ac.pass_context
 async def lt_txtapget(context: ac.Context, serdes: int) -> str:
     """
     Read the tap values of the specified serdes of the working port.
@@ -241,25 +243,25 @@
     port_obj = storage.retrieve_port()
     storage.validate_current_serdes(serdes)
     dic = await anlt_utils.txtap_get(port_obj, serdes)
     return format_txtap_get(serdes, dic)
 
 
 # **************************
-# sub-command: txtapset
+# sub-command: lt txtapset
 # **************************
 @lt.command(cls=cb.XenaCommand, name="txtapset")
 @ac.argument("serdes", type=ac.INT)
 @ac.argument("pre3", type=ac.INT)
 @ac.argument("pre2", type=ac.INT)
 @ac.argument("pre", type=ac.INT)
 @ac.argument("main", type=ac.INT)
 @ac.argument("post", type=ac.INT)
 @ac.pass_context
-async def txtapset(
+async def lt_txtapset(
     context: ac.Context,
     serdes: int,
     pre3: int,
     pre2: int,
     pre: int,
     main: int,
     post: int,
@@ -299,7 +301,31 @@
         <SERDES>: The serdes index.
     """
     storage: CmdContext = context.obj
     port_obj = storage.retrieve_port()
     storage.validate_current_serdes(serdes)
     dic = await anlt_utils.lt_status(port_obj, serdes)
     return format_lt_status(dic)
+
+
+# ******************************
+# sub-command: lt txtap-autotune
+# ******************************
+@lt.command(cls=cb.XenaCommand, name="txtap-autotune")
+@ac.argument("serdes", type=ac.INT)
+@ac.pass_context
+async def lt_txtap_autotune(
+    context: ac.Context,
+    serdes: int,
+) -> str:
+    """
+    Auto tune the tx tap values of the specified serdes of the working port.
+
+        <SERDES>: The serdes index.
+
+    """
+    storage: CmdContext = context.obj
+    port_obj = storage.retrieve_port()
+    storage.validate_current_serdes(serdes)
+    await anlt_utils.txtap_autotune(port_obj, serdes)
+    dic = await anlt_utils.txtap_get(port_obj, serdes)
+    return format_txtap_get(serdes, dic)
```

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_commands/management.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_commands/management.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 import asyncclick as ac
 import asyncio
 from xoa_utils.clicks import click_backend as cb
 from xoa_driver.hlfuncs import anlt as anlt_utils
 from xoa_driver.hlfuncs import mgmt as mgmt_utils
 from xoa_driver.testers import L23Tester
+from xoa_driver.enums import MediaConfigurationType
 from xoa_utils.clis import format_tester_status, format_ports_status, format_port_status
 from xoa_utils.clicks.click_commands.group import xoa_util
 from xoa_utils.clicks import click_help as h
 from xoa_utils.cmds import CmdContext
 from xoa_utils import exceptions as ex
 
 # --------------------------
@@ -44,30 +45,33 @@
     real_port_list = [i.strip() for i in ports.split(",")] if ports else []
     tester = await L23Tester(device, username, password, tcp, debug=False)
     con_info = f"{device}:{tcp}"
     storage.store_current_tester(username, con_info, tester)
     count = 0
     first_id = ""
     for id_str in real_port_list:
+        this_module_dic = storage.obtain_physical_modules(id_str)
+        for module_id, module_obj in this_module_dic.items():
+            storage.store_module(module_id, module_obj)
         this_port_dic = storage.obtain_physical_ports(id_str)
         for port_id, port_obj in this_port_dic.items():
             if force:
                 await mgmt_utils.reserve_port(port_obj, force)
             if reset:
                 await mgmt_utils.reset_port(port_obj)
             port_serdes_num = (await anlt_utils.anlt_status(port_obj))["serdes_count"]
             storage.store_port(port_id, port_obj, port_serdes_num)
             if count == 0:
                 first_id = port_id
             count += 1
-
     if real_port_list:
+        storage.store_current_module_str(first_id.split("/")[0])
         storage.store_current_port_str(first_id)
     if force or reset:
-        await asyncio.sleep(3)
+        await asyncio.sleep(2)
         # status will change when you reserve_port or reset_port, need to wait
     return format_tester_status(storage)
 
 
 # --------------------------
 # command: exit
 # --------------------------
@@ -78,20 +82,25 @@
 )
 @ac.pass_context
 async def exit(context: ac.Context, reset: bool, release: bool) -> str:
     """
     Exit the session. Exit by terminating port reservations, disconnecting from the chassis, releasing system resources, and removing the specified port configurations.
     """
     storage: CmdContext = context.obj
+    for module_id, module_obj in storage.retrieve_modules().copy().items():
+        if release:
+            await mgmt_utils.free_module(module_obj)
+        storage.remove_module(module_id)
     for port_id, port_obj in storage.retrieve_ports().copy().items():
         if reset:
             await mgmt_utils.reset_port(port_obj)
         if release:
             await mgmt_utils.free_port(port_obj)
         storage.remove_port(port_id)
+
     return ""
 
 
 # --------------------------
 # command: port
 # --------------------------
 @xoa_util.command(cls=cb.XenaCommand)
@@ -102,47 +111,132 @@
 async def port(context: ac.Context, port: str, reset: bool, force: bool) -> str:
     """
     Switch the working port. If the port is not yet reserved, reserve the port. Update the working port in the cache.
 
         <PORT>: The port on the specified device host. Specify a port using the format slot/port, e.g. 0/0
     """
     storage: CmdContext = context.obj
+    module_id = port.split("/")[0]
+    try:
+        storage.store_current_module_str(module_id)
+        p_obj = storage.retrieve_module(module_id)
+    except ex.NotInStoreError:
+        module_dic = storage.obtain_physical_modules(module_id)
+        for m_id, m_obj in module_dic.items():
+            storage.store_module(m_id, m_obj)
+            storage.store_current_module_str(m_id)
     try:
         storage.store_current_port_str(port)
         p_obj = storage.retrieve_port()
         port_serdes_num = (await anlt_utils.anlt_status(p_obj))["serdes_count"]
         storage.store_port(port, p_obj, port_serdes_num)
     except ex.NotInStoreError:
         port_dic = storage.obtain_physical_ports(port)
         for p_id, p_obj in port_dic.items():
             port_serdes_num = (await anlt_utils.anlt_status(p_obj))["serdes_count"]
             storage.store_port(p_id, p_obj, port_serdes_num)
             storage.store_current_port_str(p_id)
     port_obj = storage.retrieve_port()
     port_id = storage.retrieve_port_str()
     tester_obj = storage.retrieve_tester()
-    module_id = int(port.split("/")[0])
+
     if force:
-        module_obj = mgmt_utils.get_module(tester_obj, module_id)
+        module_obj = mgmt_utils.get_module(tester_obj, int(module_id))
         await mgmt_utils.free_module(module_obj)
         await mgmt_utils.reserve_port(port_obj, force)
     if reset:
         await mgmt_utils.reset_port(port_obj)
     if force or reset:
         await asyncio.sleep(2)
         # status will change when you reserve_port or reset_port, need to wait
     status_dic = await anlt_utils.anlt_status(port_obj)
-    return f"{format_ports_status(storage, False)}{format_port_status(port_id, status_dic, storage)}"
+    return f"{format_ports_status(storage, False)}{format_port_status(status_dic, storage)}"
 
 
 # --------------------------
 # command: ports
 # --------------------------
 @xoa_util.command(cls=cb.XenaCommand)
 @ac.option("--all/--no-all", type=ac.BOOL, help=h.HELP_PORTS_ALL, default=False)
 @ac.pass_context
 async def ports(context: ac.Context, all: bool) -> str:
     """
     List all the ports reserved by the current session.
     """
     storage: CmdContext = context.obj
     return format_ports_status(storage, all)
+
+
+# --------------------------
+# command: module-config
+# --------------------------
+@xoa_util.command(cls=cb.XenaCommand)
+@ac.argument("module", type=ac.INT)
+@ac.argument(
+    "media",
+    type=ac.Choice(
+        [
+            "cfp4",
+            "cxp",
+            "sfp28",
+            "qsfp28_nrz",
+            "qsfp28_pam4",
+            "qsfp56_pam4",
+            "qsfpdd_pam4",
+            "sfp56",
+            "sfpdd",
+            "sfp112",
+            "qsfpdd_nrz",
+            "cfp",
+            "base_t1",
+            "base_t1s",
+            "qsfpdd800",
+            "qsfp112",
+            "osfp800",
+        ]
+    ),
+)
+@ac.argument("port_count", type=ac.INT)
+@ac.argument(
+    "port_speed",
+    type=ac.Choice(
+        [
+            "800g",
+            "400g",
+            "200g",
+            "100g",
+        ]
+    ),
+)
+@ac.option("--force/--no-force", type=ac.BOOL, help=h.HELP_CONNECT_FORCE, default=True)
+@ac.pass_context
+async def module_config(
+    context: ac.Context,
+    module: int,
+    media: str,
+    port_count: int,
+    port_speed: str,
+    force: bool,
+) -> str:
+    """
+    Change module media configuration
+
+        <MODULE>: Specifies the module on the specified device host. Specify a module using the format slot, e.g. 0
+
+        <MEDIA>: Specifies the media configuration type of the module. Allowed values: qsfpddpam4 | sfpdd | sfp112 | qsfpddnrz | qsfpdd800 | qsfp112 | osfp800
+
+        <PORT_COUNT>: Specifies the port count of the module.
+
+        <PORT_SPEED>: Specifies the port speed in Gbps of the module. Allowed values: 800g | 400g | 200g | 100g
+
+    """
+    storage: CmdContext = context.obj
+    module_obj = storage.retrieve_module(str(module))
+    await mgmt_utils.set_module_media_config(
+        module_obj, MediaConfigurationType[media.upper()], force
+    )
+    await mgmt_utils.set_module_port_config(
+        module_obj, port_count, int(port_speed.replace("g", "000000000")), force
+    )
+    await module_obj._setup()
+    storage.remove_ports()
+    return ""
```

### Comparing `xoa-utils-1.1.1/xoa_utils/clicks/click_help.py` & `xoa-utils-1.2.0/xoa_utils/clicks/click_help.py`

 * *Files 25% similar despite different names*

```diff
@@ -54,8 +54,34 @@
 HELP_ANLT_LOG_KEEP = "Specifies what types of log entries to keep, default to keep all.\
 Allow values: all | an | lt \
 all: keep both AN and LT\
 an:  keep AN only\
 lt:  keep lt only"
 
 HELP_ANLT_LOG_SERDES = "Specifies which serdes of LT logs to keep. If you don't know how many\
-serdes the port has, use 'anlt log', default to all serdes."
+serdes the port has, use 'anlt log', default to all serdes."
+
+HELP_STRICT_ON = "Should enable ANLT strict mode, default to --on."
+
+HELP_LOG_CONTROL_DEBUG_ON = "Debug log out, default to --debug, -D"
+
+HELP_LOG_CONTROL_AN_TRACE_ON = "Auto-negotiation trace output, default to --an-trace, -A"
+
+HELP_LOG_CONTROL_LT_TRACE_ON = "Link training algorithm trace, default to --lt-trace, -L"
+
+HELP_LOG_CONTROL_ALG_TRACE_ON = "Link training algorithm trace output, default to --alg-trace, -G"
+
+HELP_LOG_CONTROL_FSM_PORT_ON = "Port state machine transitions output, default to --no-fsm-port, -p"
+
+HELP_LOG_CONTROL_FSM_AN_ON = "Auto-negotiation state machine transitions, default to --fsm-an, -N"
+
+HELP_LOG_CONTROL_FSM_AN_STIMULI_ON = "Auto-negotiation stimuli state machine transitions, default to --no-fsm-an-stimuli, -m"
+
+HELP_LOG_CONTROL_FSM_LT_ON = "Link training state machine transitions, default to --fsm-lt, -T"
+
+HELP_LOG_CONTROL_FSM_LT_COEFF_ON = "Link training coefficient state machine transitions, default to --no-fsm-lt-coeff, -c"
+
+HELP_LOG_CONTROL_FSM_LT_STIMULI_ON = "Link training stimuli state machine transitions, default to --no-fsm-lt-stimuli, -s"
+
+HELP_LOG_CONTROL_FSM_LT_ALG0_ON = "Link training algorithm 0 state machine transitions, default to --fsm-lt-alg0, -Z"
+
+HELP_LOG_CONTROL_FSM_LT_ALGN1_ON = "Link training algorithm -1 state machine transitions, default to --fsm-lt-algn1, -O"
```

### Comparing `xoa-utils-1.1.1/xoa_utils/clis/cli_utils.py` & `xoa-utils-1.2.0/xoa_utils/clis/cli_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,126 +113,107 @@
         port_dic = storage.get_all_ports()
     else:
         port_dic = storage.retrieve_ports()
     result_str = _port_dic_status(storage.retrieve_port_str(), port_dic)
     return result_str
 
 
-def format_port_status(port_id: str, status: dict, storage: "CmdContext") -> str:
-    ims = {}
-    # algs = {}
-
-    for key, val in storage.retrieve_lt_initial_mod().items():
-        ims[key] = enums.LinkTrainEncoding(val).name
-    # for key, val in storage.retrieve_lt_algorithm().items():
-    #     algs[key] = enums.LinkTrainAlgorithm(val).name
-
+def format_port_status(status: dict, storage: "CmdContext") -> str:
     return f"""
-[ ACTUAL CONFIG ]
+[ACTUAL CONFIG]
     Link recovery         : {status['link_recovery']}
     Serdes count          : {status['serdes_count']}
 
-    Auto-negotiation      : {status['autoneg_enabled']} (allow loopback: {'yes' if status['autoneg_allow_loopback'] else 'no'})
+    Auto-negotiation      : {status['autoneg_enabled']} ({'allow' if status['autoneg_allow_loopback'] else 'not allow'} loopback)
     Link training         : {'on' if status['link_training_mode'] != "disabled" else 'off'} ({'interactive' if status['link_training_mode'] == "interactive" else 'auto'}) (preset0: {'standard tap' if status['link_training_preset0'] == 'nrz_no_preset' else 'existing tap'} values) (timeout: {status['link_training_timeout']})
-        Initial Mod.      : {status['initial_mods']}
     
 
-[ SHADOW CONFIG ]
-    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} (allow loopback: {'yes' if storage.retrieve_an_loopback() else 'no'})
+[SHADOW CONFIG]
+    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} ({'allow' if storage.retrieve_an_loopback() else 'not allow'} loopback)
     Link training         : {'on' if storage.retrieve_lt_enable() else 'off'} ({'interactive' if storage.retrieve_lt_interactive() else 'auto'}) (preset0: {'standard tap' if storage.retrieve_lt_preset0() == enums.NRZPreset.NRZ_NO_PRESET else 'existing tap'} values)
-        Initial Mod.      : {ims}
 """
 
 
 def format_an_status(dic: dict) -> str:
     return f"""
-[ AN STATUS ]
+[AN STATUS]
+    Mode                  : {'enabled' if dic['is_enabled'] else 'disabled'}
     Loopback              : {dic['loopback']}
-    Duration              : {dic['duration']:,} µs
+
+    Duration              : {dic['duration']:,} µs {'(N/A)' if dic['duration'] == 0 else ''}
+
     Successful runs       : {dic['successes']}
     Timeouts              : {dic['timeouts']}
     Loss of sync          : {dic['loss_of_sync']}
     FEC negotiation fails : {dic['fec_negotiation_fails']}
     HCD negotiation fails : {dic['hcd_negotiation_fails']}
                                 RX    TX
     Link codewords        : {dic['link_codewords']['rx']:6}{dic['link_codewords']['tx']:6}
     Next-page messages    : {dic['next_page_messages']['rx']:6}{dic['next_page_messages']['tx']:6}
     Unformatted pages     : {dic['unformatted_pages']['rx']:6}{dic['unformatted_pages']['tx']:6}
     """
 
 
 def format_lt_config(storage: CmdContext) -> str:
-    ims = {}
-    # algs = {}
-
-    for key, val in storage.retrieve_lt_initial_mod().items():
-        ims[key] = enums.LinkTrainEncoding(val).name
-    # for key, val in storage.retrieve_lt_algorithm().items():
-    #     algs[key] = enums.LinkTrainAlgorithm(val).name
-
     return f"""
 LT configuration to be on port {storage.retrieve_port_str()}
-[ SHADOW CONFIG ]
-    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} (allow loopback: {'yes' if storage.retrieve_an_loopback() else 'no'})
+[SHADOW CONFIG]
     Link training         : {'on' if storage.retrieve_lt_enable() else 'off'} ({'interactive' if storage.retrieve_lt_interactive() else 'auto'}) (preset0: {'standard tap' if storage.retrieve_lt_preset0() == enums.NRZPreset.NRZ_NO_PRESET else 'existing tap'} values)
-        Initial Mod.      : {ims}
 """
 
 
-def format_lt_im(storage: CmdContext, serdes: int) -> str:
+def format_lt_im(status: dict, storage: CmdContext, serdes: int) -> str:
     ims = {}
-    # algs = {}
+    algs = {}
 
     for key, val in storage.retrieve_lt_initial_mod().items():
         ims[key] = enums.LinkTrainEncoding(val).name
-    # for key, val in storage.retrieve_lt_algorithm().items():
-    #     algs[key] = enums.LinkTrainAlgorithm(val).name
+    for key, val in storage.retrieve_lt_algorithm().items():
+        algs[key] = enums.LinkTrainAlgorithm(val).name
 
     return f"""
+[ACTUAL CONFIG]
+    Link training         :
+        Initial Mod.      : {status['initial_mods']}
+
 Initial modulation to be {storage.retrieve_lt_initial_mod_serdes(serdes).name} on Serdes {serdes}
-[ SHADOW CONFIG ]
-    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} (allow loopback: {'yes' if storage.retrieve_an_loopback() else 'no'})
+[SHADOW CONFIG]
     Link training         : {'on' if storage.retrieve_lt_enable() else 'off'} ({'interactive' if storage.retrieve_lt_interactive() else 'auto'}) (preset0: {'standard tap' if storage.retrieve_lt_preset0() == enums.NRZPreset.NRZ_NO_PRESET else 'existing tap'} values)
         Initial Mod.      : {ims}
     """
 
 
-def format_lt_algorithm(storage: CmdContext, serdes: int) -> str:
+def format_lt_algorithm(status: dict, storage: CmdContext, serdes: int) -> str:
     ims = {}
-    # algs = {}
+    algs = {}
 
     for key, val in storage.retrieve_lt_initial_mod().items():
         ims[key] = enums.LinkTrainEncoding(val).name
-    # for key, val in storage.retrieve_lt_algorithm().items():
-    #     algs[key] = enums.LinkTrainAlgorithm(val).name
+    for key, val in storage.retrieve_lt_algorithm().items():
+        algs[key] = enums.LinkTrainAlgorithm(val).name
 
     return f"""
+[ACTUAL CONFIG]
+    Link training         :
+        Algorithm         : {status['algorithms']}
+
 LT algorithm to be {storage.retrieve_lt_algorithm_serdes(serdes).name} on Serdes {serdes}
-[ SHADOW CONFIG ]
-    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} (allow loopback: {'yes' if storage.retrieve_an_loopback() else 'no'})
+[SHADOW CONFIG]
     Link training         : {'on' if storage.retrieve_lt_enable() else 'off'} ({'interactive' if storage.retrieve_lt_interactive() else 'auto'}) (preset0: {'standard tap' if storage.retrieve_lt_preset0() == enums.NRZPreset.NRZ_NO_PRESET else 'existing tap'} values)
-        Initial Mod.      : {ims}
+        Algorithm         : {algs}
     """
 
 
 def format_an_config(storage: CmdContext) -> str:
-    ims = {}
-    # algs = {}
-
-    for key, val in storage.retrieve_lt_initial_mod().items():
-        ims[key] = enums.LinkTrainEncoding(val).name
-    # for key, val in storage.retrieve_lt_algorithm().items():
-    #     algs[key] = enums.LinkTrainAlgorithm(val).name
 
     return f"""
 AN configuration to be on port {storage.retrieve_port_str()}
-[ SHADOW CONFIG ]
-    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} (allow loopback: {'yes' if storage.retrieve_an_loopback() else 'no'})
+[SHADOW CONFIG]
+    Auto-negotiation      : {'on' if storage.retrieve_an_enable() else 'off'} ({'allow' if storage.retrieve_an_loopback() else 'not allow'} loopback)
     Link training         : {'on' if storage.retrieve_lt_enable() else 'off'} ({'interactive' if storage.retrieve_lt_interactive() else 'auto'}) (preset0: {'standard tap' if storage.retrieve_lt_preset0() == enums.NRZPreset.NRZ_NO_PRESET else 'existing tap'} values)
-        Initial Mod.      : {ims}
 """
 
 
 def format_recovery(storage: CmdContext, on: bool) -> str:
     enable = "on" if on else "off"
     return f"Port {storage.retrieve_port_str()} link recovery: {enable}\n"
 
@@ -283,26 +264,27 @@
     return format_txtap_get(
         serdes, {"c(-3)": pre3, "c(-2)": pre2, "c(-1)": pre, "c(0)": main, "c(1)": post}
     )
 
 
 def format_lt_status(dic: dict) -> str:
     return f"""
-[ LT STATUS ]
-    Is enabled        : {str(dic['is_enabled']).lower()}
-    Is trained        : {str(dic['is_trained']).lower()}
+[LT STATUS]
+    Mode              : {'enabled' if dic['is_enabled'] else 'disabled'}
+    Status            : {'trained' if dic['is_trained'] else 'not trained'}
     Failure           : {dic['failure']}
 
     Initial mod.      : {dic['init_modulation']}
-    Preset0           : {"standard tap" if dic['preset0'] else "existing tap"} values
+    Preset0 (oos)     : {"standard tap" if dic['preset0'] else "existing tap"} values
+
     Total bits        : {dic['total_bits']:,}
     Total err. bits   : {dic['total_errored_bits']:,}
     BER               : {dic['ber']}
 
-    Duration          : {dic['duration']:,} µs
+    Duration          : {dic['duration']:,} µs {'(N/A)' if dic['duration'] == 0 else ''}
 
     Lock lost         : {dic['lock_lost']}
     Frame lock        : {dic['frame_lock']}
     Remote frame lock : {dic['remote_frame_lock']}
 
     Frame errors      : {dic['frame_errors']:,}
     Overrun errors    : {dic['overrun_errors']:,}
@@ -316,7 +298,51 @@
         + req                   :{dic['c(-3)']['+req']['rx']:11}{dic['c(-3)']['+req']['tx']:4}{dic['c(-2)']['+req']['rx']:8}{dic['c(-2)']['+req']['tx']:4}{dic['c(-1)']['+req']['rx']:8}{dic['c(-1)']['+req']['tx']:4}{dic['c(0)']['+req']['rx']:8}{dic['c(0)']['+req']['tx']:4}{dic['c(1)']['+req']['rx']:8}{dic['c(1)']['+req']['tx']:4}
         - req                   :{dic['c(-3)']['-req']['rx']:11}{dic['c(-3)']['-req']['tx']:4}{dic['c(-2)']['-req']['rx']:8}{dic['c(-2)']['-req']['tx']:4}{dic['c(-1)']['-req']['rx']:8}{dic['c(-1)']['-req']['tx']:4}{dic['c(0)']['-req']['rx']:8}{dic['c(0)']['-req']['tx']:4}{dic['c(1)']['-req']['rx']:8}{dic['c(1)']['-req']['tx']:4}
         coeff/eq limit reached  :{dic['c(-3)']['coeff_and_eq_limit_reached']['rx']:11}{dic['c(-3)']['coeff_and_eq_limit_reached']['tx']:4}{dic['c(-2)']['coeff_and_eq_limit_reached']['rx']:8}{dic['c(-2)']['coeff_and_eq_limit_reached']['tx']:4}{dic['c(-1)']['coeff_and_eq_limit_reached']['rx']:8}{dic['c(-1)']['coeff_and_eq_limit_reached']['tx']:4}{dic['c(0)']['coeff_and_eq_limit_reached']['rx']:8}{dic['c(0)']['coeff_and_eq_limit_reached']['tx']:4}{dic['c(1)']['coeff_and_eq_limit_reached']['rx']:8}{dic['c(1)']['coeff_and_eq_limit_reached']['tx']:4}
         eq limit reached        :{dic['c(-3)']['eq_limit_reached']['rx']:11}{dic['c(-3)']['eq_limit_reached']['tx']:4}{dic['c(-2)']['eq_limit_reached']['rx']:8}{dic['c(-2)']['eq_limit_reached']['tx']:4}{dic['c(-1)']['eq_limit_reached']['rx']:8}{dic['c(-1)']['eq_limit_reached']['tx']:4}{dic['c(0)']['eq_limit_reached']['rx']:8}{dic['c(0)']['eq_limit_reached']['tx']:4}{dic['c(1)']['eq_limit_reached']['rx']:8}{dic['c(1)']['eq_limit_reached']['tx']:4}
         coeff not supported     :{dic['c(-3)']['coeff_not_supported']['rx']:11}{dic['c(-3)']['coeff_not_supported']['tx']:4}{dic['c(-2)']['coeff_not_supported']['rx']:8}{dic['c(-2)']['coeff_not_supported']['tx']:4}{dic['c(-1)']['coeff_not_supported']['rx']:8}{dic['c(-1)']['coeff_not_supported']['tx']:4}{dic['c(0)']['coeff_not_supported']['rx']:8}{dic['c(0)']['coeff_not_supported']['tx']:4}{dic['c(1)']['coeff_not_supported']['rx']:8}{dic['c(1)']['coeff_not_supported']['tx']:4}
         coeff at limit          :{dic['c(-3)']['coeff_at_limit']['rx']:11}{dic['c(-3)']['coeff_at_limit']['tx']:4}{dic['c(-2)']['coeff_at_limit']['rx']:8}{dic['c(-2)']['coeff_at_limit']['tx']:4}{dic['c(-1)']['coeff_at_limit']['rx']:8}{dic['c(-1)']['coeff_at_limit']['tx']:4}{dic['c(0)']['coeff_at_limit']['rx']:8}{dic['c(0)']['coeff_at_limit']['tx']:4}{dic['c(1)']['coeff_at_limit']['rx']:8}{dic['c(1)']['coeff_at_limit']['tx']:4}
 """
+
+def format_debug_init(dic: dict) -> str:
+    return f"""
+    base:        0x{dic["base"]:0>8X}
+    rx_gtm_base: 0x{dic["rx_gtm_base"]:0>8X}
+    rx_serdes:   {dic["rx_serdes"]}
+    tx_gtm_base: 0x{dic["tx_gtm_base"]:0>8X}
+    tx_serdes:   {dic["tx_serdes"]}
+"""
+
+def format_strict(storage: CmdContext, on: bool) -> str:
+    enable = "on" if on else "off"
+    return f"Port {storage.retrieve_port_str()} ANLT strict mode: {enable}\n"
+
+def format_log_control(
+        storage: CmdContext, 
+        debug: bool, 
+        an_trace: bool, 
+        lt_trace: bool, 
+        alg_trace: bool,
+        fsm_port: bool,
+        fsm_an: bool,
+        fsm_an_stimuli: bool,
+        fsm_lt: bool,
+        fsm_lt_coeff: bool,
+        fsm_lt_stimuli: bool,
+        fsm_lt_alg0: bool,
+        fsm_lt_algn1: bool
+        ) -> str:
+    return f"""
+Port {storage.retrieve_port_str()} log control:
+    Type debug:             {'on' if debug else 'off'}
+    Type AN trace:          {'on' if an_trace else 'off'}
+    Type LT trace:          {'on' if lt_trace else 'off'}
+    Type ALG trace:         {'on' if alg_trace else 'off'}
+    Type FSM port:          {'on' if fsm_port else 'off'}
+    Type FSM AN:            {'on' if fsm_an else 'off'}
+    Type FSM AN Stimuli:    {'on' if fsm_an_stimuli else 'off'}
+    Type FSM LT:            {'on' if fsm_lt else 'off'}
+    Type FSM LT Coeff:      {'on' if fsm_lt_coeff else 'off'}
+    Type FSM LT Stimuli:    {'on' if fsm_lt_stimuli else 'off'}
+    Type FSM LT ALG  0:     {'on' if fsm_lt_alg0 else 'off'}
+    Type FSM LT ALG -1:     {'on' if fsm_lt_algn1 else 'off'}
+"""
```

### Comparing `xoa-utils-1.1.1/xoa_utils/cmds/cmd_context.py` & `xoa-utils-1.2.0/xoa_utils/cmds/cmd_context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import typing as t
 from xoa_driver.testers import L23Tester
+from xoa_driver.modules import GenericL23Module
 from xoa_driver.ports import GenericL23Port
 from xoa_utils.exceptions import (
     NotInStoreError,
     NotConnectedError,
     NoSuchIDError,
     NoWorkingPort,
     NotCorrectSerdesError,
@@ -29,14 +30,20 @@
     def __init__(self) -> None:
         self.serial: str = ""
         self.con_info: str = ""
         self.username: str = ""
         self.obj: t.Optional[L23Tester] = None
 
 
+class ModuleState:
+    def __init__(self) -> None:
+        self.modules: dict[str, GenericL23Module] = {}
+        self.module_str: str = ""
+
+
 class PortState:
     def __init__(self) -> None:
         self.ports: dict[str, GenericL23Port] = {}
         self.port_str: str = ""
         self.port_serdes_num: dict[str, int] = {}
 
 
@@ -70,14 +77,15 @@
 
 class CmdContext:
     def __init__(self) -> None:
         self.clear_all()
 
     def clear_all(self) -> None:
         self._tr_state: TesterState = TesterState()
+        self._md_state: ModuleState = ModuleState()
         self._pt_state: PortState = PortState()
         self._error: ErrorString = ErrorString()
         self._an_state: ANState = ANState()
         self._lt_state: LTState = LTState()
         self._fn_state: LoopFuncState = LoopFuncState()
         self._anlt_low_state: AnltLowState = AnltLowState()
 
@@ -131,14 +139,19 @@
 
     def store_lt_preset0(self, preset0: str) -> None:
         if preset0 == "standard":
             self._lt_state.preset0 = NRZPreset.NRZ_NO_PRESET
         else:
             self._lt_state.preset0 = NRZPreset.NRZ_WITH_PRESET
 
+    def store_current_module_str(self, current_module_str: str) -> None:
+        if current_module_str not in self._md_state.modules:
+            raise NotInStoreError(current_module_str)
+        self._md_state.module_str = current_module_str
+
     def store_current_port_str(self, current_port_str: str) -> None:
         if current_port_str not in self._pt_state.ports:
             raise NotInStoreError(current_port_str)
         self._pt_state.port_str = current_port_str
         self._anlt_low_state = AnltLowState()
 
     def store_current_tester(
@@ -189,14 +202,17 @@
 
     def retrieve_lt_preset0(self) -> NRZPreset:
         return self._lt_state.preset0
 
     def retrieve_ports(self) -> dict[str, GenericL23Port]:
         return self._pt_state.ports
 
+    def retrieve_modules(self) -> dict[str, GenericL23Module]:
+        return self._md_state.modules
+
     def retrieve_tester_username(self) -> str:
         return self._tr_state.username
 
     def retrieve_tester_con_info(self) -> str:
         return self._tr_state.con_info
 
     def retrieve_tester_serial(self) -> str:
@@ -204,20 +220,34 @@
 
     def retrieve_tester(self) -> t.Optional[L23Tester]:
         return self._tr_state.obj
 
     def retrieve_port_str(self) -> str:
         return self._pt_state.port_str
 
+    def store_module(self, exact_module_id: str, module_obj: GenericL23Module) -> None:
+        self._md_state.modules[exact_module_id] = module_obj
+
     def store_port(
         self, exact_port_id: str, port_obj: GenericL23Port, port_serdes_num: int
     ) -> None:
         self._pt_state.ports[exact_port_id] = port_obj
         self._pt_state.port_serdes_num[exact_port_id] = port_serdes_num
 
+    def retrieve_module(self, exact_module_id: str = "current") -> GenericL23Module:
+        if self.retrieve_tester() is None:
+            raise NotConnectedError()
+        if exact_module_id == "current":
+            if not self._md_state.module_str:
+                raise NoWorkingPort()
+            exact_module_id = self._md_state.module_str
+        if exact_module_id in self._md_state.modules:
+            return self._md_state.modules[exact_module_id]
+        raise NotInStoreError(exact_module_id)
+
     def retrieve_port(self, exact_port_id: str = "current") -> GenericL23Port:
         if self.retrieve_tester() is None:
             raise NotConnectedError()
         if exact_port_id == "current":
             if not self._pt_state.port_str:
                 raise NoWorkingPort()
             exact_port_id = self._pt_state.port_str
@@ -225,36 +255,62 @@
             return self._pt_state.ports[exact_port_id]
         raise NotInStoreError(exact_port_id)
 
     def validate_current_serdes(self, serdes: int) -> None:
         current_port_id = self._pt_state.port_str
         if current_port_id not in self._pt_state.port_serdes_num:
             raise NotInStoreError(current_port_id)
-        if not serdes in range(self._pt_state.port_serdes_num[self._pt_state.port_str]):
+        if serdes not in range(self._pt_state.port_serdes_num[self._pt_state.port_str]):
             raise NotCorrectSerdesError(current_port_id, serdes)
 
+    def remove_module(self, exact_module_id: str) -> None:
+        if exact_module_id in self._md_state.modules:
+            del self._md_state.modules[exact_module_id]
+
     def remove_port(self, exact_port_id: str) -> None:
         if exact_port_id in self._pt_state.ports:
             del self._pt_state.ports[exact_port_id]
 
+    def remove_ports(self) -> None:
+        self._pt_state = PortState()
+
     def set_error(self, error_str: str) -> None:
         self._error.set_val(error_str)
 
     clear_error = partialmethod(set_error, "")
 
     def get_error(self) -> str:
         return self._error.err_str
 
+    def obtain_physical_modules(
+        self, id_str: str = "*", update=True
+    ) -> dict[str, GenericL23Module]:
+        tester = self.retrieve_tester()
+        if tester is None:
+            raise NotConnectedError()
+        m_dics = {}
+        if id_str == "*":
+            for m in mgmt_utils.get_modules(tester):
+                m_dics[str(m.module_id)] = m
+        else:
+            module_id = id_str.split("/")[0]
+            m = mgmt_utils.get_module(tester, int(module_id))
+            m_dics[str(m.module_id)] = m
+
+        if update:
+            self._md_state.modules.update(m_dics)
+        return m_dics
+
     def obtain_physical_ports(
         self, id_str: str = "*", update: bool = True
     ) -> dict[str, GenericL23Port]:
-        if self.retrieve_tester() is None:
+        tester = self.retrieve_tester()
+        if tester is None:
             raise NotConnectedError()
 
-        tester = self.retrieve_tester()
         p_dics = {}
         if id_str == "*":
             m_id = p_id = -1
             for i in mgmt_utils.get_all_ports(tester):
                 p_dics[f"{i.kind.module_id}/{i.kind.port_id}"] = i
         else:
             splitted = id_str.split("/")
```

### Comparing `xoa-utils-1.1.1/xoa_utils/cmds/cmd_worker.py` & `xoa-utils-1.2.0/xoa_utils/cmds/cmd_worker.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/xoa_utils/exceptions/exceptions.py` & `xoa-utils-1.2.0/xoa_utils/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/xoa_utils/hub/hub.py` & `xoa-utils-1.2.0/xoa_utils/hub/hub.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/xoa_utils/ssh_server/xena_ssh_server.py` & `xoa-utils-1.2.0/xoa_utils/ssh_server/xena_ssh_server.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-1.1.1/xoa_utils.egg-info/SOURCES.txt` & `xoa-utils-1.2.0/xoa_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

