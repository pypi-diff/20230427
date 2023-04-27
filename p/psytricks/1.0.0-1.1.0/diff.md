# Comparing `tmp/psytricks-1.0.0.tar.gz` & `tmp/psytricks-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-1.0.0.tar", max compression
+gzip compressed data, was "psytricks-1.1.0.tar", max compression
```

## Comparing `psytricks-1.0.0.tar` & `psytricks-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-1.0.0/LICENSE
--rw-r--r--   0        0        0     3557 2023-04-25 12:23:05.630073 psytricks-1.0.0/README.md
--rw-r--r--   0        0        0      973 2023-04-25 12:40:48.831068 psytricks-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-25 12:40:48.831068 psytricks-1.0.0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     5145 2023-04-25 11:22:59.630911 psytricks-1.0.0/src/psytricks/cli.py
--rw-r--r--   0        0        0     2247 2023-04-13 12:44:28.211286 psytricks-1.0.0/src/psytricks/decoder.py
--rw-r--r--   0        0        0     1801 2023-04-13 12:44:28.207286 psytricks-1.0.0/src/psytricks/mappings.py
--rw-r--r--   0        0        0     3014 2023-04-13 12:38:57.964112 psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-04-25 07:07:36.345357 psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-04-25 07:59:35.398779 psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetSessions.json
--rw-r--r--   0        0        0    11759 2023-04-25 11:05:43.569742 psytricks-1.0.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1
--rw-r--r--   0        0        0    11067 2023-04-25 11:09:47.919739 psytricks-1.0.0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 psytricks-1.0.0/setup.py
--rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 psytricks-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3557 2023-04-25 12:23:05.630073 psytricks-1.1.0/README.md
+-rw-r--r--   0        0        0      973 2023-04-27 10:15:37.642659 psytricks-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-27 10:15:37.642659 psytricks-1.1.0/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-25 11:22:59.630911 psytricks-1.1.0/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-1.1.0/src/psytricks/decoder.py
+-rw-r--r--   0        0        0     2265 2023-04-27 09:43:59.712708 psytricks-1.1.0/src/psytricks/mappings.py
+-rw-r--r--   0        0        0     3014 2023-04-13 12:38:57.964112 psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-04-25 07:07:36.345357 psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-04-25 07:59:35.398779 psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetSessions.json
+-rw-r--r--   0        0        0    11759 2023-04-25 11:05:43.569742 psytricks-1.1.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0    11067 2023-04-25 11:09:47.919739 psytricks-1.1.0/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 psytricks-1.1.0/setup.py
+-rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 psytricks-1.1.0/PKG-INFO
```

### Comparing `psytricks-1.0.0/LICENSE` & `psytricks-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/README.md` & `psytricks-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/pyproject.toml` & `psytricks-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "1.0.0"
+version = "1.1.0"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-1.0.0/src/psytricks/cli.py` & `psytricks-1.1.0/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/src/psytricks/mappings.py` & `psytricks-1.1.0/src/psytricks/mappings.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,25 @@
     5: "suspended",
     6: "turningon",
     7: "turningoff",
     8: "suspending",
     9: "resuming",
 }
 
+# Citrix.Broker.Admin.Sdk.Hostingpoweraction (e.g. by `New-BrokerHostingPowerAction`)
+power_action = {
+    0: "turnon",
+    1: "turnoff",
+    2: "shutdown",
+    3: "reset",
+    4: "restart",
+    5: "suspend",
+    6: "resume",
+}
+
 
 # Citrix.Broker.Admin.SDK.RegistrationState (e.g. used by `Get-BrokerMachine`)
 registration_state = {
     0: "unregistered",
     1: "initializing",
     2: "registered",
     3: "agenterror",
@@ -52,7 +63,17 @@
 # it is below "L7" the mapping apparently different (but even Xen 8.0 VMs are
 # reporting "L7_9", so this is fairly reasonable)!
 session_state = {
     1: "connected",
     2: "active",
     3: "disconnected",
 }
+
+
+by_keyword = {
+    "SummaryState": summary_state,
+    "MachineSummaryState": summary_state,
+    "RegistrationState": registration_state,
+    "PowerState": power_state,
+    "SessionState": session_state,
+    "Action": power_action,
+}
```

### Comparing `psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json` & `psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json` & `psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/src/psytricks/ps1scripts/dummydata/GetSessions.json` & `psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1` & `psytricks-1.1.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/src/psytricks/wrapper.py` & `psytricks-1.1.0/src/psytricks/wrapper.py`

 * *Files identical despite different names*

### Comparing `psytricks-1.0.0/setup.py` & `psytricks-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['click>=8.1.3,<9.0.0', 'loguru>=0.6.0,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['psytricks = psytricks.cli:run_cli']}
 
 setup_kwargs = {
     'name': 'psytricks',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'PowerShell Python Citrix Tricks.',
     'long_description': '# PSytricks\n\n`P`ower`S`hell P`y`thon Ci`tri`x Tri`cks`.\n\nPun intended.\n\n![logo](https://raw.githubusercontent.com/imcf/psytricks/main/resources/images/logo.png)\n\nThis package provides an abstraction layer allowing Python code to interact with\na [Citrix Virtual Apps and Desktops (CVAD)][www_cvad] stack, i.e. to fetch\nstatus information and trigger actions on machines and sessions. It does this by\ncalling a wrapper script written in `Windows PowerShell` (note: **not**\n`PowerShell Core`, see below) that is using the *Citrix Broker PowerShell\nSnap-In* which is provided along with the `Delivery Controller` installation\nmedia.\n\n## 🤯 Are you serious?\n\nCalling PowerShell as a subprocess from within Python? 😳\n\nTo convert results to JSON and pass them back, just to parse it again in Python.\nReally? 🧐\n\n### ✅ Yes. We. Are\n\n*And the package name was chosen to reflect this.*\n\nTo be very clear: performance is abysmal, but this is *not at all* an issue for\nus. Abysmal, as in: for every wrapped call a full (new) PowerShell process needs\nto be instantiated, usually taking something like 1-2 seconds. ⏱\n\nHowever, the frequency of calls is also *very* low in our use case - not more\nthan a handful per minute, and that\'s already the peak. Therefore, having a\nrobust way of interacting with the Citrix platform outnumbers all other\narguments. 🍹\n\n## Installation\n\n### Prerequisites\n\nAs mentioned above, the *Citrix Broker PowerShell Snap-In* is required to be\ninstalled on the machine that will run the wrapper script, since its commands\nare being used to communicate with the CVAD stack. This is also the reason why\nthis package will work on ***Windows PowerShell only*** as snap-ins are not\nsupported on other PowerShell editions. Please note this also implies that the\nlatest usable PowerShell version is 5.1 as newer ones have dropped support for\nsnap-ins (but that\'s a different problem that Citrix will have to solve at some\npoint).\n\nTo install the snap-in, look for an MSI package like this in the `Delivery\nController` or `XenDesktop` installation media and install it as usual:\n\n* `Broker_PowerShellSnapIn_x64.msi`\n\n### Installing the package\n\nFor installing `psytricks` please create a `venv`, then run:\n\n```bash\npip install psytricks\n```\n\nThis will also register the CLI tool `psytricks.exe` although that one is mostly\nmeant for testing and demonstration purposes, otherwise the `*-Broker*` commands\nprovided by the PowerShell snap-in could be used directly.\n\n## What does it provide?\n\nTo interact with CVAD, a `psytricks.wrapper.PSyTricksWrapper` object needs to be\ninstantiated and passed the address of the *Delivery Controller* to connect to,\nfor example:\n\n```Python\nfrom psytricks.wrapper import PSyTricksWrapper\n\nwrapper = PSyTricksWrapper(deliverycontroller="cdc01.vdi.example.xy")\n```\n\n### Fetching status information\n\nThe wrapper object can then be used to e.g. retrieve information on the machines\ncontrolled ("brokered") by Citrix:\n\n```Python\nmachines = wrapper.get_machine_status()\n\nfor machine in machines:\n    print(f"[{machine["DNSName"]}] is in power state \'{machine["PowerState"]}\'")\nprint(f"Got status details on {len(machines)} machines.")\n```\n\n### Performing actions\n\nTo restart a machine, use something like this:\n\n```Python\nwrapper.perform_poweraction(machine="vm23.vdi.example.xy", action="restart")\n```\n\nFor placing a machine in *Maintenance Mode* use:\n\n```Python\nwrapper.set_maintenance(machine="vm42.vdi.example.xy", disable=False)\n```\n\n[www_cvad]: https://docs.citrix.com/en-us/citrix-virtual-apps-desktops\n',
     'author': 'Niko Ehrenfeuchter',
     'author_email': 'nikolaus.ehrenfeuchter@unibas.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psytricks-1.0.0/PKG-INFO` & `psytricks-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 1.0.0
+Version: 1.1.0
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

