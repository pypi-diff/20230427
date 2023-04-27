# Comparing `tmp/edl-mod-0.0.29.tar.gz` & `tmp/edl-mod-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmp0l7stv45/edl-mod-0.0.29.tar", last modified: Wed Sep 28 15:09:49 2022, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmppxdb_fo9/edl-mod-0.0.30.tar", last modified: Thu Apr 27 20:39:48 2023, max compression
```

## Comparing `edl-mod-0.0.29.tar` & `edl-mod-0.0.30.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2022-09-28 15:09:49.000000 edl-mod-0.0.29/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.29/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    45867 2022-09-28 15:09:25.000000 edl-mod-0.0.29/edl.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2022-09-28 15:09:49.000000 edl-mod-0.0.29/edl_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2022-09-28 15:09:49.000000 edl-mod-0.0.29/edl_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2022-09-28 15:09:49.000000 edl-mod-0.0.29/edl_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2022-09-28 15:09:49.000000 edl-mod-0.0.29/edl_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2022-09-28 15:09:49.000000 edl-mod-0.0.29/edl_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2022-09-28 15:09:49.000000 edl-mod-0.0.29/edl_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.29/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.29/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.29/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2022-09-28 15:09:49.000000 edl-mod-0.0.29/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2022-09-28 15:09:49.000000 edl-mod-0.0.29/setup.cfg
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-27 20:39:48.000000 edl-mod-0.0.30/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.30/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46525 2023-04-27 20:36:39.000000 edl-mod-0.0.30/edl.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-27 20:39:48.000000 edl-mod-0.0.30/edl_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-04-27 20:39:48.000000 edl-mod-0.0.30/edl_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-04-27 20:39:48.000000 edl-mod-0.0.30/edl_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-04-27 20:39:48.000000 edl-mod-0.0.30/edl_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-04-27 20:39:48.000000 edl-mod-0.0.30/edl_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-04-27 20:39:48.000000 edl-mod-0.0.30/edl_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.30/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.30/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.30/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-04-27 20:39:48.000000 edl-mod-0.0.30/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-04-27 20:39:48.000000 edl-mod-0.0.30/setup.cfg
```

### Comparing `edl-mod-0.0.29/edl.py` & `edl-mod-0.0.30/edl.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Many firewalls or other security services can import EDL's, or, lists of hosts to block.
 This project can be used as command line tool and as a module. It has the capability to
 to search, add, delete and view the designated list.
 
 This module produces 2 EDL's, a master list and the actual EDL. The actual EDL is one IP
 address per line.
 
-By default, the list only takes IP addresses and will reject anything that else that is NOT
+By default, this script only takes IP addresses and will reject anything that is NOT
 resolvable into an IP address.
 
 The master list contains the IP, user who submitted the IP, the timestamp, whois owner and
 abuse contact and finally a comment about the block. This information is for accounting purposes
 only (although you might find the abuse contact useful), but the actual EDL is derived from it.
 The actual EDL is just a list of IP's with no commentary or other designators. You must save the
 master EDL and consumable EDL's, although in some places you can set the module to save the
@@ -45,14 +45,15 @@
 import copy
 import csv
 import getpass
 import subprocess
 import shutil
 import socket
 import cmd
+import configparser
 
 # Ma Stoof
 
 import py_helper as ph
 from py_helper import Msg,DbgMsg,ErrMsg,DebugMode,CmdLineMode,ModuleMode
 from py_helper import Taggable, AuditTrail, ValidIP, IsIPv4, IsIPv6, IsNetwork
 from py_helper import Clear, NewLine, Pause, Menu
@@ -713,20 +714,23 @@
 # Explicit No Prompt
 NoPrompt=False
 
 # Autosave EDLFIle
 AutoSave=False
 
 # Version
-VERSION=(0,0,29)
+VERSION=(0,0,30)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Parser
 __Parser__ = None
 
+# Config File
+__Config__ = "/etc/edl/config"
+
 # Response list
 Responses = list()
 
 # Test File
 DMEDLFile="/tmp/edl.test.txt"
 # EDL Master File
 EDLMaster = "/tmp/edlmaster.csv"
@@ -1050,15 +1054,15 @@
 	else:
 		success = False
 
 	return (success,excluded,existing)
 
 # Add IP (or list of IPs, or DNS Names) To EDL Master
 def Add(host,user=None,timestamp=None,owner=None,abuse=None,comment=None,protect=False,nosleep=False,masterfile=None,edlfile=None):
-	"""Add Host/List of Hosts/DNS names  to EDL Master"""
+	"""Add Host/List of Hosts/Subnets/List of subnets/DNS names to EDL Master"""
 
 	global LastAdd, Responses, EDLRowTemplate
 
 	if user == None:
 		user = getpass.getuser()
 
 	if timestamp == None:
@@ -1080,20 +1084,21 @@
 	else:
 		hosts = [ host ]
 
 	sanity_check = list()
 
 	# Check for DNS names
 	for host in hosts:
-		if not ValidIP(host):
+		if IsNetwork(host) or ValidIP(host):
+			sanity_check.append(host)
+		else:
+			# Not subnet or IP
 			ips = HostIPCheck(host)
 
 			sanity_check.extend(ips)
-		else:
-			sanity_check.append(host)
 
 	hosts = sanity_check
 
 	# Builds a list of 5-tuples (invalid-flag,exists-flag,entry,excluded-flag,edl_entry)
 	for host in hosts:
 		# Determine if Excluded
 		# Determine if already in EDL
@@ -1872,23 +1877,36 @@
 # Initialization
 #
 
 # Initialize Module
 def Initialize():
 	"""Initialize Module"""
 
-	global __EnvEDLMaster__,__EnvEDLFile__,__EnvEDLExcludes__,__EnvComment__
+	global __EnvEDLMaster__,__EnvEDLFile__,__EnvEDLExcludes__,__EnvComment__,__Config__
 	global EDLFile, EDLMaster, Excludes
 
 	random.seed()
 
+	comment = "No comment at this time"
+
+	if os.path.exists(__Config__):
+		cfg = configparser.ConfigParser()
+
+		cfg.read(__Config__)
+
+		EDLMaster = cfg.get("appsettings","EDLMaster",fallback="/tmp/edlmaster.csv")
+		EDLFile = cfg.get("appsettings","EDLFile",fallback="/tmp/edlfile.csv")
+		Excludes = cfg.get("appsettings","Excludes",fallback="/tmp/excludes.txt")
+
+		comment = cfg.get("appsettings","Comment",fallback=comment)
+
 	# Check Environment
-	EDLMaster = os.environ.get(__EnvEDLMaster__,EDLMaster)
-	EDLFile = os.environ.get(__EnvEDLFile__,EDLFile)
-	Excludes = os.environ.get(__EnvEDLExcludes__,Excludes)
+	if __EnvEDLMaster__ in os.environ: EDLMaster = os.environ.get(__EnvEDLMaster__,EDLMaster)
+	if __EnvEDLFile__ in os.environ: EDLFile = os.environ.get(__EnvEDLFile__,EDLFile)
+	if __EnvEDLExcludes__ in os.environ: Excludes = os.environ.get(__EnvEDLExcludes__,Excludes)
 
 	# Check for preset comment in ENV, preset if there
 	comment = os.environ.get(__EnvComment__,None)
 
 	if comment:
 		AddResponse(comment)
```

### Comparing `edl-mod-0.0.29/edl_mod.egg-info/PKG-INFO` & `edl-mod-0.0.30/edl_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.29
+Version: 0.0.30
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.29/LICENSE` & `edl-mod-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `edl-mod-0.0.29/PKG-INFO` & `edl-mod-0.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.29
+Version: 0.0.30
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.29/setup.cfg` & `edl-mod-0.0.30/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = edl-mod
-version = 0.0.29
+version = 0.0.30
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Module for editting and searching external dynamic lists (EDLs)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/edl
 project_urls =
```

