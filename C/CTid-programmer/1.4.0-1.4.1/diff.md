# Comparing `tmp/CTid-programmer-1.4.0.tar.gz` & `tmp/CTid-programmer-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTid-programmer-1.4.0.tar", last modified: Fri May 13 23:39:27 2022, max compression
+gzip compressed data, was "CTid-programmer-1.4.1.tar", last modified: Thu Apr 27 20:37:16 2023, max compression
```

## Comparing `CTid-programmer-1.4.0.tar` & `CTid-programmer-1.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.442600 CTid-programmer-1.4.0/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.314602 CTid-programmer-1.4.0/CTid_programmer.egg-info/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1586 2022-05-13 23:39:27.000000 CTid-programmer-1.4.0/CTid_programmer.egg-info/PKG-INFO
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1063 2022-05-13 23:39:27.000000 CTid-programmer-1.4.0/CTid_programmer.egg-info/SOURCES.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2022-05-13 23:39:27.000000 CTid-programmer-1.4.0/CTid_programmer.egg-info/dependency_links.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       69 2022-05-13 23:39:27.000000 CTid-programmer-1.4.0/CTid_programmer.egg-info/entry_points.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       54 2022-05-13 23:39:27.000000 CTid-programmer-1.4.0/CTid_programmer.egg-info/requires.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       16 2022-05-13 23:39:27.000000 CTid-programmer-1.4.0/CTid_programmer.egg-info/top_level.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-07 04:32:39.000000 CTid-programmer-1.4.0/LICENSE
--rw-r--r--   0 davidm    (1000) davidm    (1000)      101 2020-03-07 04:32:39.000000 CTid-programmer-1.4.0/MANIFEST.in
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1586 2022-05-13 23:39:27.442600 CTid-programmer-1.4.0/PKG-INFO
--rw-rw-r--   0 davidm    (1000) davidm    (1000)      677 2020-10-07 01:16:20.000000 CTid-programmer-1.4.0/README.rst
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.358601 CTid-programmer-1.4.0/ctid_programmer/
--rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-07 04:32:39.000000 CTid-programmer-1.4.0/ctid_programmer/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.414600 CTid-programmer-1.4.0/ctid_programmer/gui/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:39:49.000000 CTid-programmer-1.4.0/ctid_programmer/gui/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.418600 CTid-programmer-1.4.0/ctid_programmer/gui/images/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     5957 2020-03-07 04:32:39.000000 CTid-programmer-1.4.0/ctid_programmer/gui/images/ctid-logo.svg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14163 2022-05-05 19:33:57.000000 CTid-programmer-1.4.0/ctid_programmer/gui/main_window.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     5128 2020-10-07 04:04:20.000000 CTid-programmer-1.4.0/ctid_programmer/gui/main_window_rc.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14134 2022-05-13 18:49:59.000000 CTid-programmer-1.4.0/ctid_programmer/gui/param_ct.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4416 2021-04-26 21:41:35.000000 CTid-programmer-1.4.0/ctid_programmer/gui/param_linear.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     6693 2020-10-07 04:04:19.000000 CTid-programmer-1.4.0/ctid_programmer/gui/param_ntc.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4749 2020-10-07 04:04:20.000000 CTid-programmer-1.4.0/ctid_programmer/gui/param_pulse.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3141 2020-10-07 04:04:20.000000 CTid-programmer-1.4.0/ctid_programmer/gui/param_temp.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4153 2020-10-07 04:04:19.000000 CTid-programmer-1.4.0/ctid_programmer/gui/param_volt.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3619 2020-10-07 04:04:20.000000 CTid-programmer-1.4.0/ctid_programmer/gui/preferences_dialog.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3796 2020-10-07 04:04:20.000000 CTid-programmer-1.4.0/ctid_programmer/gui/template_dialog.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2139 2020-03-07 04:32:39.000000 CTid-programmer-1.4.0/ctid_programmer/preferences.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)    36185 2022-05-05 14:42:37.000000 CTid-programmer-1.4.0/ctid_programmer/programmer.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.426600 CTid-programmer-1.4.0/ctid_programmer/qt4/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:37:26.000000 CTid-programmer-1.4.0/ctid_programmer/qt4/__init__.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.258603 CTid-programmer-1.4.0/ctid_programmer/resources/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2022-05-13 23:39:27.434600 CTid-programmer-1.4.0/ctid_programmer/resources/code/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1249 2020-03-07 04:32:39.000000 CTid-programmer-1.4.0/ctid_programmer/resources/code/ac.hex
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1482 2022-05-05 14:42:37.000000 CTid-programmer-1.4.0/ctid_programmer/resources/code/powered.hex
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14730 2021-04-26 21:39:08.000000 CTid-programmer-1.4.0/ctid_programmer/sensor_params.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4966 2021-07-18 19:04:23.000000 CTid-programmer-1.4.0/ctid_programmer/sn.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     7652 2022-05-05 19:51:03.000000 CTid-programmer-1.4.0/ctid_programmer/sn_egauge.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4154 2021-07-18 19:04:23.000000 CTid-programmer-1.4.0/ctid_programmer/sn_local.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2409 2020-03-07 05:02:08.000000 CTid-programmer-1.4.0/ctid_programmer/template.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 04:55:43.000000 CTid-programmer-1.4.0/pyproject.toml
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2022-05-13 23:39:27.446600 CTid-programmer-1.4.0/setup.cfg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1407 2022-05-13 23:38:53.000000 CTid-programmer-1.4.0/setup.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.335142 CTid-programmer-1.4.1/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.255143 CTid-programmer-1.4.1/CTid_programmer.egg-info/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1413 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/PKG-INFO
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1063 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/SOURCES.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/dependency_links.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       69 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/entry_points.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       54 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/requires.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       16 2023-04-27 20:37:16.000000 CTid-programmer-1.4.1/CTid_programmer.egg-info/top_level.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1122 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/LICENSE
+-rw-r--r--   0 davidm    (1000) davidm    (1000)      101 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/MANIFEST.in
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1413 2023-04-27 20:37:16.335142 CTid-programmer-1.4.1/PKG-INFO
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)      677 2020-10-07 01:16:20.000000 CTid-programmer-1.4.1/README.rst
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.283143 CTid-programmer-1.4.1/ctid_programmer/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/ctid_programmer/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.319142 CTid-programmer-1.4.1/ctid_programmer/gui/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:39:49.000000 CTid-programmer-1.4.1/ctid_programmer/gui/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.323142 CTid-programmer-1.4.1/ctid_programmer/gui/images/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     5957 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/ctid_programmer/gui/images/ctid-logo.svg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14163 2022-05-05 19:33:57.000000 CTid-programmer-1.4.1/ctid_programmer/gui/main_window.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     5128 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/main_window_rc.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14134 2022-05-13 18:49:59.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_ct.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4416 2021-04-26 21:41:35.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_linear.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     6693 2020-10-07 04:04:19.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_ntc.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4749 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_pulse.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3141 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_temp.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4153 2020-10-07 04:04:19.000000 CTid-programmer-1.4.1/ctid_programmer/gui/param_volt.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3619 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/preferences_dialog.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3796 2020-10-07 04:04:20.000000 CTid-programmer-1.4.1/ctid_programmer/gui/template_dialog.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2140 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/preferences.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)    36022 2023-04-27 20:36:40.000000 CTid-programmer-1.4.1/ctid_programmer/programmer.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.323142 CTid-programmer-1.4.1/ctid_programmer/qt4/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)        0 2020-10-03 17:37:26.000000 CTid-programmer-1.4.1/ctid_programmer/qt4/__init__.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.227144 CTid-programmer-1.4.1/ctid_programmer/resources/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-27 20:37:16.331142 CTid-programmer-1.4.1/ctid_programmer/resources/code/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1249 2020-03-07 04:32:39.000000 CTid-programmer-1.4.1/ctid_programmer/resources/code/ac.hex
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1482 2022-05-05 14:42:37.000000 CTid-programmer-1.4.1/ctid_programmer/resources/code/powered.hex
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    15071 2023-04-27 17:10:08.000000 CTid-programmer-1.4.1/ctid_programmer/sensor_params.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4969 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/sn.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     7654 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/sn_egauge.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4075 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/sn_local.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2410 2023-04-27 17:10:07.000000 CTid-programmer-1.4.1/ctid_programmer/template.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2023-04-27 17:09:38.000000 CTid-programmer-1.4.1/pyproject.toml
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-04-27 20:37:16.335142 CTid-programmer-1.4.1/setup.cfg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1407 2023-04-27 20:35:22.000000 CTid-programmer-1.4.1/setup.py
```

### Comparing `CTid-programmer-1.4.0/CTid_programmer.egg-info/SOURCES.txt` & `CTid-programmer-1.4.1/CTid_programmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/LICENSE` & `CTid-programmer-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/README.rst` & `CTid-programmer-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/images/ctid-logo.svg` & `CTid-programmer-1.4.1/ctid_programmer/gui/images/ctid-logo.svg`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/main_window.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/main_window_rc.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/main_window_rc.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/param_ct.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/param_ct.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/param_linear.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/param_linear.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/param_ntc.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/param_ntc.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/param_pulse.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/param_pulse.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/param_temp.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/param_temp.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/param_volt.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/param_volt.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/preferences_dialog.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/gui/template_dialog.py` & `CTid-programmer-1.4.1/ctid_programmer/gui/template_dialog.py`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/preferences.py` & `CTid-programmer-1.4.1/ctid_programmer/preferences.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,33 +26,33 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 import json
 import os
 
-class Manager:
 
+class Manager:
     def __init__(self, state_directory_path):
-        self.path = os.path.join(state_directory_path, 'preferences.json')
+        self.path = os.path.join(state_directory_path, "preferences.json")
         self.load()
 
     def load(self):
         try:
-            with open(self.path, 'r') as f:
+            with open(self.path, "r") as f:
                 prefs = json.load(f)
-                self.sn_service = prefs.get('sn_service', None)
-                self.sn_increment = prefs['sn_increment']
-                self.station_id = prefs['station_id']
+                self.sn_service = prefs.get("sn_service", None)
+                self.sn_increment = prefs["sn_increment"]
+                self.station_id = prefs["station_id"]
         except IOError:
             self.sn_service = None
             self.sn_increment = 1
             self.station_id = 0
 
     def save(self):
         prefs = {
-            'sn_service': self.sn_service,
-            'sn_increment': self.sn_increment,
-            'station_id': self.station_id
+            "sn_service": self.sn_service,
+            "sn_increment": self.sn_increment,
+            "station_id": self.station_id,
         }
-        with open(self.path, 'w') as f:
+        with open(self.path, "w") as f:
             json.dump(prefs, f, sort_keys=True, indent=2)
```

### Comparing `CTid-programmer-1.4.0/ctid_programmer/programmer.py` & `CTid-programmer-1.4.1/ctid_programmer/programmer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# Copyright (c) 2016-2017, 2019-2021 eGauge Systems LLC
+# Copyright (c) 2016-2017, 2019-2023 eGauge Systems LLC
 # 	1644 Conestoga St, Suite 2
 # 	Boulder, CO 80301
 # 	voice: 720-545-9767
 # 	email: davidm@egauge.net
 #
 #  All rights reserved.
 #
@@ -39,16 +39,23 @@
 import importlib_resources
 import pexpect
 import pkg_resources
 
 from pexpect import fdpexpect
 
 from PySide2.QtCore import Qt
-from PySide2.QtWidgets import QAction, QApplication, \
-    QDialog, QDialogButtonBox, QMainWindow, QMessageBox, QListWidgetItem
+from PySide2.QtWidgets import (
+    QAction,
+    QApplication,
+    QDialog,
+    QDialogButtonBox,
+    QMainWindow,
+    QMessageBox,
+    QListWidgetItem,
+)
 
 import egauge.ctid as ctid
 
 from egauge.pyside2 import terminal
 
 from ctid_programmer import preferences
 from ctid_programmer import sensor_params
@@ -63,77 +70,81 @@
 from ctid_programmer.gui.param_ct import Ui_Param_CT
 from ctid_programmer.gui.param_linear import Ui_Param_Linear
 from ctid_programmer.gui.param_temp import Ui_Param_Temp
 from ctid_programmer.gui.param_ntc import Ui_Param_NTC
 from ctid_programmer.gui.param_pulse import Ui_Param_Pulse
 
 
-PACKAGE_NAME = 'CTid-programmer'
-PACKAGE_VERSION = pkg_resources.get_distribution('CTid-programmer').version
-VERSION_INFO = f'''{PACKAGE_NAME} {PACKAGE_VERSION}
-Copyright (c) 2018-2022 eGauge Systems LLC
+PACKAGE_NAME = "CTid-programmer"
+PACKAGE_VERSION = pkg_resources.get_distribution("CTid-programmer").version
+VERSION_INFO = f"""{PACKAGE_NAME} {PACKAGE_VERSION}
+Copyright (c) 2018-2023 eGauge Systems LLC
 License MIT: <https://opensource.org/licenses/MIT>.
 This is free software: you are free to change and redistribute it.
 
-Written by Alexandra Kaufhold and David Mosberger.'''
+Written by Alexandra Kaufhold and David Mosberger."""
 
-PATH_AVRDUDE = 'avrdude'
-PATH_CTID_ENCODER = 'ctid-encoder'
+PATH_AVRDUDE = "avrdude"
+PATH_CTID_ENCODER = "ctid-encoder"
 
-PATH_STATE_DIR = os.path.join(os.getenv('HOME'), '.CTid')
+PATH_STATE_DIR = os.path.join(os.getenv("HOME"), ".CTid")
+
+CMD_AVRDUDE = [PATH_AVRDUDE, "-b", "300000", "-ctc2030"]
 
 SENSOR_LONG_NAME = {
-    'AC': 'AC Current Sensor',
-    'DC': 'DC Current Sensor',
-    'RC': 'Rogowski Coil Sensor',
-    'linear': 'Linear Sensor',
-    'temp': 'Linear Temperature Sensor',
-    'NTC': 'NTC Thermistor Sensor',
-    'pulse': 'Pulse Sensor'
+    "AC": "AC Current Sensor",
+    "DC": "DC Current Sensor",
+    "RC": "Rogowski Coil Sensor",
+    "linear": "Linear Sensor",
+    "temp": "Linear Temperature Sensor",
+    "NTC": "NTC Thermistor Sensor",
+    "pulse": "Pulse Sensor",
 }
 
 # Filename of template to use for each sensor-type:
-CODE_TEMPLATE = {
-    'AC': 'ac.hex',
-    'RC': 'ac.hex'
-}
+CODE_TEMPLATE = {"AC": "ac.hex", "RC": "ac.hex"}
+
+CHIP_ID_TO_NAME = {0x1E9008: ("t9", "ATtiny9"), 0x1E9003: ("t10", "ATtiny10")}
 
-CHIP_ID_TO_NAME = {
-    0x1e9008: ('t9', 'ATtiny9'),
-    0x1e9003: ('t10', 'ATtiny10')
-}
 
 class Command_Processor:
-    def __init__(self, argv, pattern_list=None, logfile=None,
-                 stdout=None):
+    def __init__(self, argv, pattern_list=None, logfile=None, stdout=None):
         self.pattern_list = pattern_list + [pexpect.EOF, pexpect.TIMEOUT]
         self.error = None
         self.exit_status = None
         self.pipe = None
         self.prog = None
 
         if stdout is not None:
-            self.pipe = subprocess.Popen(argv, stdout=stdout,
-                                         stdin=subprocess.DEVNULL,
-                                         stderr=subprocess.PIPE)
+            self.pipe = subprocess.Popen(
+                argv,
+                stdout=stdout,
+                stdin=subprocess.DEVNULL,
+                stderr=subprocess.PIPE,
+            )
 
         try:
 
             if self.pipe is None:
-                self.prog = pexpect.spawn(argv[0], argv[1:],
-                                          encoding='utf-8',
-                                          codec_errors='replace',
-                                          logfile=logfile)
+                self.prog = pexpect.spawn(
+                    argv[0],
+                    argv[1:],
+                    encoding="utf-8",
+                    codec_errors="replace",
+                    logfile=logfile,
+                )
             else:
-                self.prog = fdpexpect.fdspawn(self.pipe.stderr,
-                                              encoding='utf-8',
-                                              codec_errors='replace',
-                                              logfile=logfile)
+                self.prog = fdpexpect.fdspawn(
+                    self.pipe.stderr,
+                    encoding="utf-8",
+                    codec_errors="replace",
+                    logfile=logfile,
+                )
         except pexpect.ExceptionPexpect:
-            self.error = 'Failed to start command: %s' % sys.exc_info()[1]
+            self.error = "Failed to start command: %s" % sys.exc_info()[1]
             return
 
     def __iter__(self):
         return self
 
     def __next__(self):
         while self.prog is not None:
@@ -143,40 +154,41 @@
             if got == len(self.pattern_list) - 2:
                 if self.pipe is None:
                     self.prog.close()
                     self.exit_status = self.prog.exitstatus
                 else:
                     self.pipe.wait()
                     self.exit_status = self.pipe.returncode
-                break   # EOF: done
+                break  # EOF: done
             if got == len(self.pattern_list) - 1:
-                pass    # timeout; process events and then try again...
+                pass  # timeout; process events and then try again...
             QApplication.processEvents()
         raise StopIteration
 
     def stop(self):
         if self.error is None:
-            self.error = 'program interrupted by user'
+            self.error = "program interrupted by user"
         self.prog.close()
         self.prog = None
 
+
 class Template_List_Dialog(QDialog, Ui_Template_Dialog):
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
         self.setupUi(self)
         self.listWidget.itemChanged.connect(self.item_changed)
         self.listWidget.itemDoubleClicked.connect(self.item_double_clicked)
         self.operation = None
 
-        action = QAction('Rename', self)
+        action = QAction("Rename", self)
         action.triggered.connect(self.rename_selected_template)
         self.listWidget.addAction(action)
 
-        action = QAction('Delete', self)
+        action = QAction("Delete", self)
         action.triggered.connect(self.delete_selected_template)
         self.listWidget.addAction(action)
 
         template_names = []
         for name, _ in self.parent.template_manager.items():
             template_names.append(name)
         template_names.sort()
@@ -186,27 +198,27 @@
     def add_template(self, name):
         item = QListWidgetItem(name, self.listWidget)
         item.setFlags(item.flags() | Qt.ItemIsEditable)
         # save a copy of the original name as user data for renames:
         item.setData(Qt.UserRole, name)
 
     def rename_selected_template(self, is_checked):
-        #pylint: disable=unused-argument
+        # pylint: disable=unused-argument
         self.listWidget.editItem(self.listWidget.currentItem())
 
     def delete_selected_template(self, is_checked):
-        #pylint: disable=unused-argument
+        # pylint: disable=unused-argument
         item = self.listWidget.currentItem()
         self.parent.template_manager.remove(item.text())
 
         idx = self.listWidget.row(item)
         self.listWidget.takeItem(idx)
 
     def item_double_clicked(self):
-        if self.operation == 'save':
+        if self.operation == "save":
             self.lineEdit.setText(self.listWidget.currentItem().text())
         self.accept()
 
     def item_changed(self):
         item = self.listWidget.currentItem()
         if item is None:
             return
@@ -214,56 +226,63 @@
         old_name = item.data(Qt.UserRole)
         if new_name != old_name:
             template = self.parent.template_manager.load(old_name)
             self.parent.template_manager.save(template, new_name)
             self.parent.template_manager.remove(old_name)
 
     def accept(self):
-        if self.operation == 'save':
+        if self.operation == "save":
             new_name = self.lineEdit.text().strip().lstrip()
             if not new_name:
-                QMessageBox.warning(self, 'Template Name Missing',
-                                    'Please enter a template name.',
-                                    QMessageBox.Ok)
+                QMessageBox.warning(
+                    self,
+                    "Template Name Missing",
+                    "Please enter a template name.",
+                    QMessageBox.Ok,
+                )
                 self.lineEdit.setFocus()
                 self.lineEdit.selectAll()
                 return
             if new_name in dict(self.parent.template_manager.items()):
-                choice = QMessageBox.question(self,
-                                              'Template Name Exists',
-                                              'A template named `%s\' '
-                                              'exists already.  '
-                                              'Would you like to replace '
-                                              'that template?' % new_name,
-                                              QMessageBox.Yes,
-                                              QMessageBox.Cancel)
+                choice = QMessageBox.question(
+                    self,
+                    "Template Name Exists",
+                    "A template named `%s' "
+                    "exists already.  "
+                    "Would you like to replace "
+                    "that template?" % new_name,
+                    QMessageBox.Yes,
+                    QMessageBox.Cancel,
+                )
                 if choice == QMessageBox.Cancel:
-                    return	# let user correct name
+                    return  # let user correct name
             else:
                 self.add_template(new_name)
             template = self.parent.get_template()
             self.parent.template_manager.save(template, new_name)
         else:
             item = self.listWidget.currentItem()
             name = item.text()
             template = self.parent.template_manager.load(name)
             self.parent.template_activate(template)
-            self.parent.log('Template `%s\' loaded.' % name)
+            self.parent.log("Template `%s' loaded." % name)
 
         super().accept()
 
+
 class Preferences_Editor(QDialog, Ui_Preferences_Dialog):
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
         self.setupUi(self)
 
     def exec_(self):
         self.sn_service_combo.currentIndexChanged.connect(
-            self.sn_service_changed)
+            self.sn_service_changed
+        )
         self.sn_service_combo.setCurrentIndex(0)
         selected_service = self.parent.preferences.sn_service
         if selected_service is not None:
             for idx in range(1, self.sn_service_combo.count()):
                 service_name = self.sn_service_combo.itemText(idx)
                 if service_name == selected_service:
                     self.sn_service_combo.setCurrentIndex(idx)
@@ -273,95 +292,106 @@
         return super().exec_()
 
     def accept(self):
         increment = self.increment_spinbox.value()
         station_id = self.station_id_spinbox.value()
 
         if station_id >= increment:
-            QMessageBox.critical(self, 'Invalid Station Number',
-                                 'Station id (%d) must be smaller than '
-                                 'the serial-number increment (%d).'
-                                 % (station_id, increment), QMessageBox.Ok)
+            QMessageBox.critical(
+                self,
+                "Invalid Station Number",
+                "Station id (%d) must be smaller than "
+                "the serial-number increment (%d)." % (station_id, increment),
+                QMessageBox.Ok,
+            )
             return
         super().accept()
         prefs = self.parent.preferences
         if self.sn_service_combo.currentIndex() == 0:
             prefs.sn_service = None
         else:
             prefs.sn_service = self.sn_service_combo.currentText()
         prefs.sn_increment = increment
         prefs.station_id = station_id
         prefs.save()
         self.parent.prefs_changed()
 
     def sn_service_changed(self):
-        enable = (self.sn_service_combo.currentIndex() == 0)
+        enable = self.sn_service_combo.currentIndex() == 0
         self.increment_spinbox.setEnabled(enable)
         self.station_id_spinbox.setEnabled(enable)
 
+
 class UI(QMainWindow, Ui_MainWindow):
     def __init__(self):
         QMainWindow.__init__(self)
         self.setupUi(window)
 
         self.params = {}
 
-        ct_params = sensor_params.CT(Ui_Param_CT(), self.param_group,
-                                     'CT Parameters')
-        self.params['AC'] = self.params['DC'] = self.params['RC'] = ct_params
-        self.params['linear'] = sensor_params.Linear(Ui_Param_Linear(),
-                                                     self.param_group,
-                                                     'Linear Parameters')
-        self.params['temp'] = sensor_params.Temp(Ui_Param_Temp(),
-                                                 self.param_group,
-                                                 'Temperature Parameters')
-        self.params['NTC'] = sensor_params.NTC(Ui_Param_NTC(), self.param_group,
-                                               'NTC Thermistor Parameters')
-        self.params['pulse'] = sensor_params.Pulse(Ui_Param_Pulse(),
-                                                   self.param_group,
-                                                   'Pulse Parameters')
+        ct_params = sensor_params.CT(
+            Ui_Param_CT(), self.param_group, "CT Parameters"
+        )
+        self.params["AC"] = self.params["DC"] = self.params["RC"] = ct_params
+        self.params["linear"] = sensor_params.Linear(
+            Ui_Param_Linear(), self.param_group, "Linear Parameters"
+        )
+        self.params["temp"] = sensor_params.Temp(
+            Ui_Param_Temp(), self.param_group, "Temperature Parameters"
+        )
+        self.params["NTC"] = sensor_params.NTC(
+            Ui_Param_NTC(), self.param_group, "NTC Thermistor Parameters"
+        )
+        self.params["pulse"] = sensor_params.Pulse(
+            Ui_Param_Pulse(), self.param_group, "Pulse Parameters"
+        )
 
-        self.current_params = self.params['AC']
+        self.current_params = self.params["AC"]
         self.current_params.activate()
 
         self.auto_serial_checkbox.setChecked(True)
         self.serial_spinbox.setEnabled(False)
         self.console = terminal.Terminal(self.plainTextEdit)
         self.add_mfgs()
         self.busy = False
         self.cmd = None
         self.sn_service = None
         self.mfg_id = None
         self.model = None
 
-        self.console.write('Welcome to the CTid® Programmer!\n\n'
-                           'You can use this tool to program '
-                           'the microcontroller of a CTid board (PCB).\n\n'
-                           'Please start by filling out the form on the left. '
-                           'Then attach the programming cable to the '
-                           'CTid board, and click "Program" to write the '
-                           'information to the microcontroller.\n')
-        self.welcome_msg = True	# we're displaying welcome message
+        self.console.write(
+            VERSION_INFO + "\n\n"
+            "You can use this tool to program "
+            "the microcontroller of a CTid board (PCB).\n\n"
+            "Please start by filling out the form on the left. "
+            "Then attach the programming cable to the "
+            'CTid board, and click "Program" to write the '
+            "information to the microcontroller.\n"
+        )
+        self.welcome_msg = True  # we're displaying welcome message
 
         if not os.path.isdir(PATH_STATE_DIR):
             os.mkdir(PATH_STATE_DIR)
         self.preferences = preferences.Manager(PATH_STATE_DIR)
         self.sn = None
         self.template_manager = template.Manager(PATH_STATE_DIR)
 
         for st in ctid.SENSOR_TYPE_NAME:
             name = SENSOR_LONG_NAME[st] if st in SENSOR_LONG_NAME else st
             self.sensor_type_combo.addItem(name)
 
         self.action_About.triggered.connect(self.about)
         self.sensor_type_combo.currentIndexChanged.connect(
-            self.sensor_type_changed)
+            self.sensor_type_changed
+        )
         self.mfg_combo.currentIndexChanged.connect(self.product_changed)
         self.model_lineEdit.editingFinished.connect(self.product_changed)
-        self.auto_serial_checkbox.stateChanged.connect(self.auto_serial_changed)
+        self.auto_serial_checkbox.stateChanged.connect(
+            self.auto_serial_changed
+        )
         self.program_btn.clicked.connect(self.program_or_cancel)
         self.read_btn.clicked.connect(self.read)
         self.reprogram_after_cal_btn.clicked.connect(self.reprogram_after_cal)
         self.load_template_btn.clicked.connect(self.template_load)
         self.save_template_btn.clicked.connect(self.template_save)
         self.save_template_btn.setVisible(self.template_manager.may_save())
 
@@ -369,70 +399,75 @@
 
         self.preferences_editor = Preferences_Editor(self)
         self.actionPreferences.triggered.connect(self.preferences_editor.exec)
 
         self.prefs_changed()
 
     def about(self):
-        QMessageBox.about(self, 'About', VERSION_INFO)
+        QMessageBox.about(self, "About", VERSION_INFO)
 
     def log(self, msg):
         if self.welcome_msg:
             self.plainTextEdit.clear()
             self.welcome_msg = False
-        self.console.write(msg + '\n')
+        self.console.write(msg + "\n")
 
     def template_activate(self, template):
-        '''Load values from template, except never load the serial-number.'''
+        """Load values from template, except never load the serial-number."""
         try:
-            if 'model' in template:
-                self.model_lineEdit.setText(template['model'])
+            if "model" in template:
+                self.model_lineEdit.setText(template["model"])
 
-            if 'mfg' in template:
+            if "mfg" in template:
                 for idx in range(self.mfg_combo.count()):
-                    if self.mfg_combo.itemData(idx) == template['mfg']:
+                    if self.mfg_combo.itemData(idx) == template["mfg"]:
                         # this may trigger call to product_changed() so
                         # model_lineEdit() must have been updated already...
                         self.mfg_combo.setCurrentIndex(idx)
 
             self.product_changed()
 
             # 'voltage' sensor type is now called 'linear':
-            if template['sensor_type'] == 'voltage':
-                template['sensor_type'] = 'linear'
-                template['unit'] = 0
+            if template["sensor_type"] == "voltage":
+                template["sensor_type"] = "linear"
+                template["unit"] = 0
 
             self.sensor_type_combo.setCurrentIndex(0)
             for idx, code in enumerate(ctid.SENSOR_TYPE_NAME):
-                if code == template['sensor_type']:
+                if code == template["sensor_type"]:
                     self.sensor_type_combo.setCurrentIndex(idx)
                     break
 
-            self.r_source_spinbox.setValue(template['r_source'])
-            self.r_load_spinbox.setValue(template['r_load'])
+            self.r_source_spinbox.setValue(template["r_source"])
+            self.r_load_spinbox.setValue(template["r_load"])
 
             if self.current_params is not None:
                 self.current_params.load(template)
         except KeyError as key:
-            QMessageBox.warning(self, 'Warning',
-                                'Template is missing parameter %s.'
-                                % (key), QMessageBox.Ok)
+            QMessageBox.warning(
+                self,
+                "Warning",
+                "Template is missing parameter %s." % (key),
+                QMessageBox.Ok,
+            )
 
     def template_load(self):
-        self.template_list_dialog.operation = 'load'
+        self.template_list_dialog.operation = "load"
         self.template_list_dialog.template_name_frame.hide()
         self.template_list_dialog.buttonBox.setStandardButtons(
-            QDialogButtonBox.Open|QDialogButtonBox.Cancel)
+            QDialogButtonBox.Open | QDialogButtonBox.Cancel
+        )
         self.template_list_dialog.exec()
 
     def template_save(self):
-        self.template_list_dialog.operation = 'save'
+        self.template_list_dialog.operation = "save"
         self.template_list_dialog.template_name_frame.show()
         self.template_list_dialog.buttonBox.setStandardButtons(
-            QDialogButtonBox.Save|QDialogButtonBox.Cancel)
+            QDialogButtonBox.Save | QDialogButtonBox.Cancel
+        )
         self.template_list_dialog.exec()
 
     def get_mfg_id(self):
         mfg_idx = self.mfg_combo.currentIndex()
         if mfg_idx == 0:
             return None
         return self.mfg_combo.itemData(mfg_idx)
@@ -450,60 +485,66 @@
         if self.get_mfg_id() is None or self.get_model() is None:
             return
 
         next_sn = None
         try:
             next_sn = self.sn.get()
             if next_sn is None:
-                QMessageBox.warning(self, 'Serial Number Unavailable',
-                                    'Serial number service failed to return '
-                                    'a serial number.  Reverting to '
-                                    'manual serial numbers.',
-                                    QMessageBox.Ok)
+                QMessageBox.warning(
+                    self,
+                    "Serial Number Unavailable",
+                    "Serial number service failed to return "
+                    "a serial number.  Reverting to "
+                    "manual serial numbers.",
+                    QMessageBox.Ok,
+                )
         except sn.SpaceExhausted:
-            QMessageBox.warning(self, 'Serial Number Space Exhausted',
-                                'All available serial-numbers have been used '
-                                'for \"%s %s\".  Please use a different '
-                                'manufacturer and/or model name.' \
-                                % (ctid.mfg_short_name(self.mfg_id),
-                                   self.model), QMessageBox.Ok)
+            QMessageBox.warning(
+                self,
+                "Serial Number Space Exhausted",
+                "All available serial-numbers have been used "
+                'for "%s %s".  Please use a different '
+                "manufacturer and/or model name."
+                % (ctid.mfg_short_name(self.mfg_id), self.model),
+                QMessageBox.Ok,
+            )
 
         if next_sn is None:
             self.auto_serial_checkbox.setChecked(False)
             self.serial_spinbox.setEnabled(True)
             self.serial_spinbox.setValue(0)
             return
 
         self.serial_spinbox.setValue(next_sn)
 
     def sensor_type_changed(self):
         st = ctid.SENSOR_TYPE_NAME[self.sensor_type_combo.currentIndex()]
         new_params = self.params[st] if st in self.params else None
 
         if new_params == self.current_params:
-            return	# no change
+            return  # no change
 
         if self.current_params is not None:
             self.current_params.deactivate()
         self.current_params = new_params
 
         if self.current_params is not None:
             self.current_params.activate()
 
     def product_changed(self):
         mfg_id = self.get_mfg_id()
         model = self.get_model()
 
-        log.debug('product_changed: mfg_id=%s model=%s', mfg_id, model)
+        log.debug("product_changed: mfg_id=%s model=%s", mfg_id, model)
 
         if mfg_id is None or model is None:
             return
 
         if self.mfg_id == mfg_id and self.model == model:
-            return	# no change
+            return  # no change
         self.mfg_id = mfg_id
         self.model = model
 
         if self.sn.set_product(mfg_id, model):
             self.update_sn()
         else:
             self.auto_serial_checkbox.setChecked(False)
@@ -516,18 +557,18 @@
             self.sn.activate(latest_sn)
             self.update_sn()
         else:
             self.sn.deactivate()
         self.serial_spinbox.setEnabled(not auto_serial)
 
     def add_mfgs(self):
-        '''Add companies per their table/manufacturer number as stated by CTid
+        """Add companies per their table/manufacturer number as stated by CTid
         Spec Sheet.
 
-        '''
+        """
         for mfg_id, name in ctid.MFG_ID.items():
             self.mfg_combo.addItem(name, mfg_id)
 
     def set_input_enabled(self, enabled):
         self.chip_combo.setEnabled(enabled)
         self.mfg_combo.setEnabled(enabled)
         self.sensor_type_combo.setEnabled(enabled)
@@ -544,308 +585,371 @@
 
         self.load_template_btn.setEnabled(enabled)
         self.save_template_btn.setEnabled(enabled)
         self.read_btn.setEnabled(enabled)
         self.reprogram_after_cal_btn.setEnabled(enabled)
 
     def cmd_start(self, argv, pattern_list, logfile=None, stdout=None):
-        self.cmd = Command_Processor(argv, pattern_list, logfile=logfile,
-                                     stdout=stdout)
+        self.cmd = Command_Processor(
+            argv, pattern_list, logfile=logfile, stdout=stdout
+        )
 
     def cmd_done(self):
         if self.cmd.error is not None:
-            self.log('Command failed: %s' % self.cmd.error)
+            self.log("Command failed: %s" % self.cmd.error)
 
     def get_template(self):
-        '''Get form-data as a dictionary.  No validation is performed beyond
+        """Get form-data as a dictionary.  No validation is performed beyond
         the constraints imposed by the user-interface controls.
 
-        '''
+        """
         template = {}
 
         mfg_id = self.get_mfg_id()
         if mfg_id is not None:
-            template['mfg'] = mfg_id
+            template["mfg"] = mfg_id
 
         model = self.get_model()
         if model is not None:
-            template['model'] = model
+            template["model"] = model
 
-        template['sn'] = self.serial_spinbox.value()
+        template["sn"] = self.serial_spinbox.value()
         st_idx = self.sensor_type_combo.currentIndex()
-        template['sensor_type'] = ctid.SENSOR_TYPE_NAME[st_idx]
-        template['r_source'] = self.r_source_spinbox.value()
-        template['r_load'] = self.r_load_spinbox.value()
+        template["sensor_type"] = ctid.SENSOR_TYPE_NAME[st_idx]
+        template["r_source"] = self.r_source_spinbox.value()
+        template["r_load"] = self.r_load_spinbox.value()
 
         if self.current_params is not None:
             self.current_params.save(template)
         return template
 
     def validate_form(self):
-        '''Validate form data and return cleaned data as a dictionary.'''
+        """Validate form data and return cleaned data as a dictionary."""
         cleaned_data = self.get_template()
 
-        if 'mfg' not in cleaned_data:
-            QMessageBox.warning(self, 'Manufacturer Missing',
-                                'Please select manufacturer.', QMessageBox.Ok)
+        if "mfg" not in cleaned_data:
+            QMessageBox.warning(
+                self,
+                "Manufacturer Missing",
+                "Please select manufacturer.",
+                QMessageBox.Ok,
+            )
             self.mfg_combo.setFocus()
             return None
 
-        if 'model' not in cleaned_data:
-            QMessageBox.warning(self, 'Model Name Missing',
-                                'Please enter model name.', QMessageBox.Ok)
+        if "model" not in cleaned_data:
+            QMessageBox.warning(
+                self,
+                "Model Name Missing",
+                "Please enter model name.",
+                QMessageBox.Ok,
+            )
             self.model_lineEdit.setFocus()
             return None
 
-        utf8_model = cleaned_data['model'].encode('utf-8')
+        utf8_model = cleaned_data["model"].encode("utf-8")
         if len(utf8_model) > 8:
-            QMessageBox.warning(self, 'Model Name Too Long',
-                                'Model name is %d bytes long in '
-                                'UTF-8 encoding.  '
-                                'Please limit name to 8 bytes in length.'
-                                % len(utf8_model), QMessageBox.Ok)
+            QMessageBox.warning(
+                self,
+                "Model Name Too Long",
+                "Model name is %d bytes long in "
+                "UTF-8 encoding.  "
+                "Please limit name to 8 bytes in length." % len(utf8_model),
+                QMessageBox.Ok,
+            )
             self.model_lineEdit.setFocus()
             return None
         return cleaned_data
 
     def show_cmd_error(self, cmd, title, msg):
         if cmd.exit_status is not None:
-            msg += '  Exit status %d.' % cmd.exit_status
+            msg += "  Exit status %d." % cmd.exit_status
         QMessageBox.warning(self, title, msg, QMessageBox.Ok)
 
     def create_hexfile(self, cleaned_data, params):
-        st = cleaned_data['sensor_type']
-        argv = [PATH_CTID_ENCODER,
-                '-M', '%d' % cleaned_data['mfg'],
-                '-S', st,
-                '-m', cleaned_data['model'],
-                '-n', '%d' % cleaned_data['sn'],
-                '-l', '%d' % cleaned_data['r_load'],
-                '-r', '%d' % cleaned_data['r_source']]
+        st = cleaned_data["sensor_type"]
+        argv = [
+            PATH_CTID_ENCODER,
+            "-M",
+            "%d" % cleaned_data["mfg"],
+            "-S",
+            st,
+            "-m",
+            cleaned_data["model"],
+            "-n",
+            "%d" % cleaned_data["sn"],
+            "-l",
+            "%d" % cleaned_data["r_load"],
+            "-r",
+            "%d" % cleaned_data["r_source"],
+        ]
 
         if params is not None:
             argv += params.encoder_argv(cleaned_data)
 
-        output = tempfile.mkstemp(suffix='.hex', prefix='CTid-')
-
-        template_filename = CODE_TEMPLATE[st] if st in CODE_TEMPLATE \
-                            else 'powered.hex'
+        output = tempfile.mkstemp(suffix=".hex", prefix="CTid-")
 
-        ref = (importlib_resources.files('ctid_programmer')
-               / 'resources' / 'code' / template_filename)
+        template_filename = (
+            CODE_TEMPLATE[st] if st in CODE_TEMPLATE else "powered.hex"
+        )
+
+        ref = (
+            importlib_resources.files("ctid_programmer")
+            / "resources"
+            / "code"
+            / template_filename
+        )
         with importlib_resources.as_file(ref) as code_template_path:
             argv.append(str(code_template_path))
 
-            log.debug('create_hexfile: argv=%s', argv)
+            log.debug("create_hexfile: argv=%s", argv)
 
-            self.cmd_start(argv, [], logfile=self.console,
-                           stdout=output[0])
+            self.cmd_start(argv, [], logfile=self.console, stdout=output[0])
             # consume command's output by iterating over it:
             for _ in self.cmd:
                 pass
             self.cmd_done()
 
         if self.cmd.exit_status != 0:
-            self.show_cmd_error(self.cmd, 'Command Failed',
-                                'Failed to create hex file.')
+            self.show_cmd_error(
+                self.cmd, "Command Failed", "Failed to create hex file."
+            )
             os.close(output[0])
             os.remove(output[1])
             return None
 
         # now that we have created the actual hexfile, it's safe to close
         # the original (empty) file created by mkstemp():
         os.close(output[0])
         return output[1]
 
     def detect_chip_type(self):
-        self.cmd_start([PATH_AVRDUDE, '-ctc2030', '-pt9', '-nq'],
-                       [r'Device signature = 0x([0-9a-f]+)'])
+        print('detecting')
+        self.cmd_start(
+            CMD_AVRDUDE + ["-pt9", "-nq"],
+            [r"[dD]evice signature = 0x([0-9a-f]+)"],
+        )
         chip_id = None
         for _, match in self.cmd:
             chip_id = int(match.group(1), base=16)
         self.cmd_done()
         if chip_id is None:
-            QMessageBox.warning(self, 'No Microcontroller Detected',
-                                'No microcontroller detected.  '
-                                'Please confirm programming cable is '
-                                'properly attached.',
-                                QMessageBox.Ok)
+            QMessageBox.warning(
+                self,
+                "No Microcontroller Detected",
+                "No microcontroller detected.  "
+                "Please confirm programming cable is "
+                "properly attached.",
+                QMessageBox.Ok,
+            )
             return None
         if chip_id not in CHIP_ID_TO_NAME:
-            QMessageBox.warning(self, 'Unknown Microcontroller',
-                                'Unknown microcontroller chip type 0x%x.'
-                                % chip_id, QMessageBox.Ok)
+            QMessageBox.warning(
+                self,
+                "Unknown Microcontroller",
+                "Unknown microcontroller chip type 0x%x." % chip_id,
+                QMessageBox.Ok,
+            )
             return None
         chip = CHIP_ID_TO_NAME[chip_id]
-        self.log('Detected %s chip.' % chip[1])
+        self.log("Detected %s chip." % chip[1])
         return chip[0]
 
-    def write_flash(self, chip_type, hexfile, cleaned_data, auto_serial_number):
-        '''Write HEXFILE to the flash to a chip of type CHIP_TYPE.  The
+    def write_flash(
+        self, chip_type, hexfile, cleaned_data, auto_serial_number
+    ):
+        """Write HEXFILE to the flash to a chip of type CHIP_TYPE.  The
         HEXFILE contains the data passed in CLEANED_DATA.
         AUTO_SERILA_NUMBER must be True if the serial numbers are
         being assigned automatically, False otherwise.
 
         Returns True on success, False on any failure.
-        '''
-        self.cmd_start([PATH_AVRDUDE, '-ctc2030', '-p%s' % chip_type,
-                        '-Uflash:w:%s' % hexfile], [], logfile=self.console)
+        """
+        self.cmd_start(
+            CMD_AVRDUDE + ["-p%s" % chip_type, "-Uflash:w:%s" % hexfile],
+            [],
+            logfile=self.console,
+        )
         for _ in self.cmd:
-            pass	# consume output until program is done...
+            pass  # consume output until program is done...
         self.cmd_done()
         if self.cmd.exit_status != 0:
-            self.show_cmd_error(self.cmd, 'Programming Failed',
-                                'Failed to write the microcontroller flash.')
+            self.show_cmd_error(
+                self.cmd,
+                "Programming Failed",
+                "Failed to write the microcontroller flash.",
+            )
             return False
 
-        self.log('Success: CTid board has been programmed with '
-                 'serial number %d.' % cleaned_data['sn'])
-        self.sn.commit(cleaned_data['sn'], cleaned_data, auto_serial_number)
+        self.log(
+            "Success: CTid board has been programmed with "
+            "serial number %d." % cleaned_data["sn"]
+        )
+        self.sn.commit(cleaned_data["sn"], cleaned_data, auto_serial_number)
         return True
 
     def read_template_from_flash(self, chip_type):
-        temp = tempfile.TemporaryFile(suffix='.bin', prefix='CTid-')
-        self.cmd_start([PATH_AVRDUDE, '-ctc2030', '-p%s' % chip_type,
-                        '-Uflash:r:-:r'], [], logfile=self.console,
-                       stdout=temp)
+        temp = tempfile.TemporaryFile(suffix=".bin", prefix="CTid-")
+        self.cmd_start(
+            CMD_AVRDUDE + ["-p%s" % chip_type, "-Uflash:r:-:r"],
+            [],
+            logfile=self.console,
+            stdout=temp,
+        )
         for _ in self.cmd:
-            pass	# consume output until program is done...
+            pass  # consume output until program is done...
         self.cmd_done()
 
         if self.cmd.exit_status != 0:
             temp.close()
-            self.show_cmd_error(self.cmd, 'Read Failed',
-                                'Failed to read the microcontroller flash.')
+            self.show_cmd_error(
+                self.cmd,
+                "Read Failed",
+                "Failed to read the microcontroller flash.",
+            )
             return None
 
         temp.seek(0)
         flash = temp.read()
         temp.close()
 
-        if len(flash) < 0x3e1:
+        if len(flash) < 0x3E1:
             if not flash:
-                QMessageBox.critical(self, 'Read Failed',
-                                     'Microcontroller flash is empty.',
-                                     QMessageBox.Ok)
+                QMessageBox.critical(
+                    self,
+                    "Read Failed",
+                    "Microcontroller flash is empty.",
+                    QMessageBox.Ok,
+                )
             else:
-                QMessageBox.critical(self, 'Read Failed',
-                                     'Read only %u bytes from '
-                                     'microcontroller flash.'
-                                     % len(flash), QMessageBox.Ok)
+                QMessageBox.critical(
+                    self,
+                    "Read Failed",
+                    "Read only %u bytes from "
+                    "microcontroller flash." % len(flash),
+                    QMessageBox.Ok,
+                )
             return None
-        self.log('Success: CTid board has been read.')
+        self.log("Success: CTid board has been read.")
 
-        CTid_table_addr = 0x3c0		# table goes in last 64 bytes
+        CTid_table_addr = 0x3C0  # table goes in last 64 bytes
         length = flash[CTid_table_addr]
-        table = flash[CTid_table_addr + 1:CTid_table_addr + 1 + length]
+        table = flash[CTid_table_addr + 1 : CTid_table_addr + 1 + length]
         table = ctid.Table(ctid.unstuff(table))
         template = self.ctid_table_to_template(table)
 
         if template is not None:
-            m = re.match(r'(.*)-[^-]+$', template['model'])
+            m = re.match(r"(.*)-[^-]+$", template["model"])
             if m is not None:
                 # strip suffix off model-name:
-                template['model'] = m.group(1)
+                template["model"] = m.group(1)
         return template
 
     def reprogram_with_cal_params(self, chip_type):
         template = self.read_template_from_flash(chip_type)
         if template is None:
             return
 
-        sn = template['sn']
-        mfg = template['mfg']
-        model = template['model']
+        sn = template["sn"]
+        mfg = template["mfg"]
+        model = template["model"]
 
         saved_product = self.sn.product
         self.sn.set_product(mfg, model)
         cal_params = self.sn.get_cal_data(sn)
         if cal_params is None:
             self.sn.restore_product(saved_product)
-            QMessageBox.critical(self, 'No Calibration Data Found',
-                                 'No calibration data was found for '
-                                 'product %s with serial number %s.' \
-                                 % (self.sn.product, sn), QMessageBox.Ok)
+            QMessageBox.critical(
+                self,
+                "No Calibration Data Found",
+                "No calibration data was found for "
+                "product %s with serial number %s." % (self.sn.product, sn),
+                QMessageBox.Ok,
+            )
             return
 
-        msg = ''
+        msg = ""
         for key, value in cal_params.items():
-            msg += '\t%16s: %s\n' % (key, value)
+            msg += "\t%16s: %s\n" % (key, value)
 
         # merge the calibrated parameters with existing template:
         for name, value in cal_params.items():
             template[name] = value
-        model = template['model']
+        model = template["model"]
 
-        self.console.write('\n\nFound calibration data for %s %s #%d:\n%s\n' %
-                           (ctid.mfg_short_name(mfg), model, sn, msg))
-
-        hexfile = self.create_hexfile(template,
-                                      self.params[template['sensor_type']])
+        self.console.write(
+            "\n\nFound calibration data for %s %s #%d:\n%s\n"
+            % (ctid.mfg_short_name(mfg), model, sn, msg)
+        )
+
+        hexfile = self.create_hexfile(
+            template, self.params[template["sensor_type"]]
+        )
         if hexfile is None:
             self.sn.restore_product(saved_product)
             self.mark_idle()
             return
-        self.write_flash(chip_type, hexfile, template,
-                         auto_serial_number=False)
+        self.write_flash(
+            chip_type, hexfile, template, auto_serial_number=False
+        )
         os.remove(hexfile)
         self.mark_idle()
 
         self.sn.restore_product(saved_product)
 
     def read_flash(self, chip_type):
         template = self.read_template_from_flash(chip_type)
         if template is None:
             return
         self.template_activate(template)
         self.auto_serial_checkbox.setChecked(False)
-        self.serial_spinbox.setValue(template['sn'])
+        self.serial_spinbox.setValue(template["sn"])
 
     def ctid_table_to_template(self, table):
         sensor_type = ctid.SENSOR_TYPE_NAME[table.sensor_type]
         template = {}
-        template['mfg'] = table.mfg_id
-        template['model'] = table.model
-        template['sn'] = table.serial_number
-        template['sensor_type'] = sensor_type
-        template['r_source'] = table.r_source
-        template['r_load'] = table.r_load
+        template["mfg"] = table.mfg_id
+        template["model"] = table.model
+        template["sn"] = table.serial_number
+        template["sensor_type"] = sensor_type
+        template["r_source"] = table.r_source
+        template["r_load"] = table.r_load
         self.params[sensor_type].table_to_template(table, template)
         return template
 
     def mark_busy(self):
         self.plainTextEdit.clear()
         self.busy = True
         self.set_input_enabled(False)
-        self.program_btn.setText('Cancel')
+        self.program_btn.setText("Cancel")
 
     def mark_idle(self):
         self.busy = False
-        self.program_btn.setText('Program')
+        self.program_btn.setText("Program")
         self.set_input_enabled(True)
 
     def chip_type(self):
         if self.chip_combo.currentIndex() == 0:
             # auto-detect chip
             chip_type = self.detect_chip_type()
         elif self.chip_combo.currentIndex() == 1:
-            chip_type = 't9'
+            chip_type = "t9"
         else:
-            chip_type = 't10'
+            chip_type = "t10"
         return chip_type
 
     def program_or_cancel(self):
-        '''Program the microcontroller with the info specified in the form.
+        """Program the microcontroller with the info specified in the form.
         This consists of two steps: (1) creating a hex file with the
         info encoded and (2) writing the file to the microcontroller.
 
-        '''
+        """
         if self.busy:
             if self.cmd is not None:
-                self.cmd.stop()	# cancel the running command
+                self.cmd.stop()  # cancel the running command
                 self.cmd_done()
             self.mark_idle()
             return
 
         cleaned_data = self.validate_form()
         if cleaned_data is None:
             return
@@ -856,85 +960,104 @@
         if hexfile is None:
             self.mark_idle()
             return
 
         chip_type = self.chip_type()
         if chip_type is not None:
             auto_serial_number = self.auto_serial_checkbox.isChecked()
-            if self.write_flash(chip_type, hexfile, cleaned_data,
-                                auto_serial_number):
+            if self.write_flash(
+                chip_type, hexfile, cleaned_data, auto_serial_number
+            ):
                 self.update_sn()
 
         os.remove(hexfile)
         self.mark_idle()
 
     def read(self):
-        '''Reads CTid parameters from the flash.'''
+        """Reads CTid parameters from the flash."""
         self.mark_busy()
 
         chip_type = self.chip_type()
         if chip_type is not None:
             self.read_flash(chip_type)
 
         self.mark_idle()
 
     def reprogram_after_cal(self):
-        '''Reads CTid parameters from the flash, lookup calibration parameters
+        """Reads CTid parameters from the flash, lookup calibration parameters
         for the read serial-number and, if that exists, reprogram with
         those parameters.
 
-        '''
+        """
         self.mark_busy()
 
         chip_type = self.chip_type()
         if chip_type is not None:
             self.reprogram_with_cal_params(chip_type)
 
         self.mark_idle()
 
     def prefs_changed(self):
         prefs = self.preferences
 
         if self.sn is None or self.sn_service != prefs.sn_service:
             self.sn_service = prefs.sn_service
-            if prefs.sn_service == 'eGauge':
+            if prefs.sn_service == "eGauge":
                 self.sn = sn_egauge.Manager(self, PATH_STATE_DIR)
             else:
                 if prefs.sn_service is not None:
-                    QMessageBox.critical(self, 'Unknown Serial Number Service',
-                                         'Serial number service %s is '
-                                         'unknown.  Reverting to locally '
-                                         'managed serial numbers.' \
-                                         % prefs.sn_service)
+                    QMessageBox.critical(
+                        self,
+                        "Unknown Serial Number Service",
+                        "Serial number service %s is "
+                        "unknown.  Reverting to locally "
+                        "managed serial numbers." % prefs.sn_service,
+                    )
                     self.sn_service = None
                 self.sn = sn_local.Manager(self, PATH_STATE_DIR)
             if self.mfg_id is not None and self.model is not None:
                 self.sn.set_product(self.mfg_id, self.model)
             self.reprogram_after_cal_btn.setVisible(
-                self.sn.has_calibration_data())
+                self.sn.has_calibration_data()
+            )
         self.sn.set_preferences(prefs)
         self.update_sn()
 
-parser = argparse.ArgumentParser(description='CTid GUI programmer.')
-parser.add_argument('-F', '--full-screen', action='store_true',
-                    help='Start application in full-screen mode.')
-parser.add_argument('-d', '--debug', action='store_const', const=logging.DEBUG,
-                    dest='log_level', help='Show debug output.')
-parser.add_argument('-v', '--version', action='store_true',
-                    help='Output version information and exit.')
+
+parser = argparse.ArgumentParser(description="CTid GUI programmer.")
+parser.add_argument(
+    "-F",
+    "--full-screen",
+    action="store_true",
+    help="Start application in full-screen mode.",
+)
+parser.add_argument(
+    "-d",
+    "--debug",
+    action="store_const",
+    const=logging.DEBUG,
+    dest="log_level",
+    help="Show debug output.",
+)
+parser.add_argument(
+    "-v",
+    "--version",
+    action="store_true",
+    help="Output version information and exit.",
+)
 args = parser.parse_args()
 
 if args.version:
     print(VERSION_INFO)
     sys.exit(0)
 
 log_level = logging.ERROR if args.log_level is None else args.log_level
 logging.basicConfig()
-log = logging.getLogger()	# get the root logger
-log.setLevel(log_level)		# sets default logging for all child loggers
+log = logging.getLogger()  # get the root logger
+log.setLevel(log_level)  # sets default logging for all child loggers
 
 app = QApplication(sys.argv)
 window = QMainWindow()
 ui = UI()
 
 if args.full_screen:
     window.showMaximized()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `CTid-programmer-1.4.0/ctid_programmer/resources/code/ac.hex` & `CTid-programmer-1.4.1/ctid_programmer/resources/code/ac.hex`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/resources/code/powered.hex` & `CTid-programmer-1.4.1/ctid_programmer/resources/code/powered.hex`

 * *Files identical despite different names*

### Comparing `CTid-programmer-1.4.0/ctid_programmer/sensor_params.py` & `CTid-programmer-1.4.1/ctid_programmer/sensor_params.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,337 +27,380 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 from PySide2.QtWidgets import QMessageBox, QWidget
 
 import egauge.ctid as ctid
 
+
 def invalid_double(string):
     try:
         float(string)
     except ValueError:
         return True
     return False
 
+
 class Sensor_Params:
-    def __init__(self, ui, parent, title='Sensor Parameters'):
+    def __init__(self, ui, parent, title="Sensor Parameters"):
         self.parent = parent
         self.ui = ui
         self.widget = QWidget(parent)
         self.widget.setVisible(False)
         self.ui.setupUi(self.widget)
         self.title = title
 
     def activate(self):
-        '''Display our set of sensor parameters.'''
+        """Display our set of sensor parameters."""
         self.widget.setVisible(True)
         self.parent.setTitle(self.title)
 
     def deactivate(self):
-        '''Hide our set of sensor parameters.'''
+        """Hide our set of sensor parameters."""
         self.widget.setVisible(False)
-        self.parent.setTitle('Sensor Parameters')
+        self.parent.setTitle("Sensor Parameters")
 
     def set_input_enabled(self, enabled):
-        '''Enable or disable inputs.'''
+        """Enable or disable inputs."""
 
     def load(self, template):
-        '''Load sensor parameters from a template.'''
+        """Load sensor parameters from a template."""
 
     def save(self, template):
-        '''Save sensor parameters in the template dictionary, without
+        """Save sensor parameters in the template dictionary, without
         validation.
 
-        '''
+        """
 
     def validate(self, template):
-        '''Validate the parameter values in the template.  If there are any
+        """Validate the parameter values in the template.  If there are any
         errors, focus on the input element with the erroneous value
         and return False, otherwise return True.
 
-        '''
+        """
         return True
 
     def encoder_argv(self, template):
-        '''Convert the parameter values to the argument list required for the
-        CTid-encoder program.'''
+        """Convert the parameter values to the argument list required for the
+        CTid-encoder program."""
         return []
 
     def table_to_template(self, table, template):
-        '''Extract sensor parameters from table and add them to the template.'''
+        """Extract sensor parameters from table and add them to the template."""
+
 
 class CT(Sensor_Params):
     def set_input_enabled(self, enabled):
         self.ui.current_spinbox.setEnabled(enabled)
         self.ui.size_spinbox.setEnabled(enabled)
         self.ui.output_voltage_spinbox.setEnabled(enabled)
         self.ui.bias_voltage_spinbox.setEnabled(enabled)
         self.ui.phase_spinbox.setEnabled(enabled)
         self.ui.voltage_temp_coeff_spinbox.setEnabled(enabled)
         self.ui.phase_temp_coeff_spinbox.setEnabled(enabled)
         for row in range(4):
-            v_cal = self.ui.__dict__['calv%d' % (row + 1)]
-            p_cal = self.ui.__dict__['calp%d' % (row + 1)]
+            v_cal = self.ui.__dict__["calv%d" % (row + 1)]
+            p_cal = self.ui.__dict__["calp%d" % (row + 1)]
             v_cal.setEnabled(enabled)
             p_cal.setEnabled(enabled)
 
     def load(self, template):
-        self.ui.current_spinbox.setValue(template['current'])
-        self.ui.size_spinbox.setValue(template['size'])
-        self.ui.output_voltage_spinbox.setValue(template['v_output'])
-        self.ui.bias_voltage_spinbox.setValue(template['v_bias'])
-        self.ui.phase_spinbox.setValue(template['phi'])
-        self.ui.voltage_temp_coeff_spinbox.setValue(template['v_temp_coeff'])
-        self.ui.phase_temp_coeff_spinbox.setValue(template['phi_temp_coeff'])
+        self.ui.current_spinbox.setValue(template["current"])
+        self.ui.size_spinbox.setValue(template["size"])
+        self.ui.output_voltage_spinbox.setValue(template["v_output"])
+        self.ui.bias_voltage_spinbox.setValue(template["v_bias"])
+        self.ui.phase_spinbox.setValue(template["phi"])
+        self.ui.voltage_temp_coeff_spinbox.setValue(template["v_temp_coeff"])
+        self.ui.phase_temp_coeff_spinbox.setValue(template["phi_temp_coeff"])
 
-        cal_table = template['cal_table']
+        cal_table = template["cal_table"]
         for row in range(4):
-            levels = ['1.5', '5', '15', '50']
-            v_cal = self.ui.__dict__['calv%d' % (row + 1)]
-            p_cal = self.ui.__dict__['calp%d' % (row + 1)]
+            levels = ["1.5", "5", "15", "50"]
+            v_cal = self.ui.__dict__["calv%d" % (row + 1)]
+            p_cal = self.ui.__dict__["calp%d" % (row + 1)]
             if levels[row] not in cal_table:
                 v_cal.setValue(0.0)
                 p_cal.setValue(0.0)
                 continue
             adj = cal_table[levels[row]]
             v_cal.setValue(adj[0])
             p_cal.setValue(adj[1])
 
     def save(self, template):
-        template['current'] = self.ui.current_spinbox.value()
-        template['size'] = self.ui.size_spinbox.value()
-        template['v_output'] = self.ui.output_voltage_spinbox.value()
-        template['v_bias'] = self.ui.bias_voltage_spinbox.value()
-        template['phi'] = self.ui.phase_spinbox.value()
-        template['v_temp_coeff'] = self.ui.voltage_temp_coeff_spinbox.value()
-        template['phi_temp_coeff'] = self.ui.phase_temp_coeff_spinbox.value()
+        template["current"] = self.ui.current_spinbox.value()
+        template["size"] = self.ui.size_spinbox.value()
+        template["v_output"] = self.ui.output_voltage_spinbox.value()
+        template["v_bias"] = self.ui.bias_voltage_spinbox.value()
+        template["phi"] = self.ui.phase_spinbox.value()
+        template["v_temp_coeff"] = self.ui.voltage_temp_coeff_spinbox.value()
+        template["phi_temp_coeff"] = self.ui.phase_temp_coeff_spinbox.value()
         cal_table = {}
         for row in range(4):
-            levels = ['1.5', '5', '15', '50']
-            v_cal = self.ui.__dict__['calv%d' % (row + 1)].value()
-            p_cal = self.ui.__dict__['calp%d' % (row + 1)].value()
+            levels = ["1.5", "5", "15", "50"]
+            v_cal = self.ui.__dict__["calv%d" % (row + 1)].value()
+            p_cal = self.ui.__dict__["calp%d" % (row + 1)].value()
             if v_cal == 0.0 and p_cal == 0.0:
                 continue
             cal_table[levels[row]] = (v_cal, p_cal)
-        template['cal_table'] = cal_table
+        template["cal_table"] = cal_table
 
     def encoder_argv(self, template):
-        argv = ['-s', '%.1f' % template['size'],
-                '-c', '%.1f' % template['current'],
-                '-v', '%.5f' % template['v_output'],
-                '-b', '%.6f' % (1e-3 * template['v_bias']),
-                '-p', '%.2f' % template['phi'],
-                '-t', '%d' % template['v_temp_coeff'],
-                '-T', '%.1f' % template['phi_temp_coeff']]
-        for lvl, adj in template['cal_table'].items():
-            argv += ['-a', '%s:%.3f/%.3f' % (lvl, adj[0], adj[1])]
+        argv = [
+            "-s",
+            "%.1f" % template["size"],
+            "-c",
+            "%.1f" % template["current"],
+            "-v",
+            "%.5f" % template["v_output"],
+            "-b",
+            "%.6f" % (1e-3 * template["v_bias"]),
+            "-p",
+            "%.2f" % template["phi"],
+            "-t",
+            "%d" % template["v_temp_coeff"],
+            "-T",
+            "%.1f" % template["phi_temp_coeff"],
+        ]
+        for lvl, adj in template["cal_table"].items():
+            argv += ["-a", "%s:%.3f/%.3f" % (lvl, adj[0], adj[1])]
         return argv
 
     def table_to_template(self, table, template):
-        template['current'] = table.rated_current
-        template['size'] = table.size
-        template['v_output'] = table.voltage_at_rated_current
-        template['v_bias'] = 1e3 * table.bias_voltage
-        template['phi'] = table.phase_at_rated_current
-        template['v_temp_coeff'] = table.voltage_temp_coeff
-        template['phi_temp_coeff'] = table.phase_temp_coeff
+        template["current"] = table.rated_current
+        template["size"] = table.size
+        template["v_output"] = table.voltage_at_rated_current
+        template["v_bias"] = 1e3 * table.bias_voltage
+        template["phi"] = table.phase_at_rated_current
+        template["v_temp_coeff"] = table.voltage_temp_coeff
+        template["phi_temp_coeff"] = table.phase_temp_coeff
         cal_table = {}
         for row in range(4):
             levels = [1.5, 5, 15, 50]
             v_cal = table.cal_table[levels[row]][0]
             p_cal = table.cal_table[levels[row]][1]
             if v_cal == 0.0 and p_cal == 0.0:
                 continue
             cal_table[str(levels[row])] = (v_cal, p_cal)
-        template['cal_table'] = cal_table
+        template["cal_table"] = cal_table
+
 
 class Linear(Sensor_Params):
     def __init__(self, ui, parent, title):
         super().__init__(ui, parent, title)
         max_float = 3.4028235e38
         self.ui.scale_spinbox.setRange(-max_float, max_float)
         self.ui.offset_spinbox.setRange(-max_float, max_float)
         for _, unit_desc in ctid.SENSOR_UNITS:
             self.ui.unit_comboBox.addItem(unit_desc)
         self.ui.unit_comboBox.currentIndexChanged.connect(self._unit_changed)
 
     def _unit_changed(self):
         unit_code = self.ui.unit_comboBox.currentIndex()
         unit = ctid.get_sensor_unit(unit_code)
-        if unit == '':
-            scale_unit = ' 1/V'
-            offset_unit = ''
+        if unit == "":
+            scale_unit = " 1/V"
+            offset_unit = ""
         else:
-            scale_unit = ' %s/V' % unit
-            offset_unit = ' %s' % unit
+            scale_unit = " %s/V" % unit
+            offset_unit = " %s" % unit
         self.ui.scale_spinbox.setSuffix(scale_unit)
         self.ui.offset_spinbox.setSuffix(offset_unit)
 
     def set_input_enabled(self, enabled):
         self.ui.unit_comboBox.setEnabled(enabled)
         self.ui.scale_spinbox.setEnabled(enabled)
         self.ui.offset_spinbox.setEnabled(enabled)
         self.ui.delay_spinbox.setEnabled(enabled)
 
     def load(self, template):
-        self.ui.unit_comboBox.setCurrentIndex(template['unit'])
-        self.ui.scale_spinbox.setValue(template['scale'])
-        self.ui.offset_spinbox.setValue(template['offset'])
-        self.ui.delay_spinbox.setValue(template['delay'])
+        self.ui.unit_comboBox.setCurrentIndex(template["unit"])
+        self.ui.scale_spinbox.setValue(template["scale"])
+        self.ui.offset_spinbox.setValue(template["offset"])
+        self.ui.delay_spinbox.setValue(template["delay"])
 
     def save(self, template):
-        template['unit'] = self.ui.unit_comboBox.currentIndex()
-        template['scale'] = self.ui.scale_spinbox.value()
-        template['offset'] = self.ui.offset_spinbox.value()
-        template['delay'] = self.ui.delay_spinbox.value()
+        template["unit"] = self.ui.unit_comboBox.currentIndex()
+        template["scale"] = self.ui.scale_spinbox.value()
+        template["offset"] = self.ui.offset_spinbox.value()
+        template["delay"] = self.ui.delay_spinbox.value()
 
     def encoder_argv(self, template):
-        return ['--unit', str(template['unit']),
-                '--scale', str(template['scale']),
-                '--offset', str(template['offset']),
-                '--delay', str(template['delay'])]
+        return [
+            "--unit",
+            str(template["unit"]),
+            "--scale",
+            str(template["scale"]),
+            "--offset",
+            str(template["offset"]),
+            "--delay",
+            str(template["delay"]),
+        ]
 
     def table_to_template(self, table, template):
-        template['unit'] = table.sensor_unit
-        template['scale'] = table.scale
-        template['offset'] = table.offset
-        template['delay'] = table.delay
+        template["unit"] = table.sensor_unit
+        template["scale"] = table.scale
+        template["offset"] = table.offset
+        template["delay"] = table.delay
+
 
 class Temp(Sensor_Params):
     def set_input_enabled(self, enabled):
         self.ui.scale_spinbox.setEnabled(enabled)
         self.ui.offset_spinbox.setEnabled(enabled)
 
     def load(self, template):
-        self.ui.scale_spinbox.setValue(template['scale'])
-        self.ui.offset_spinbox.setValue(template['offset'])
+        self.ui.scale_spinbox.setValue(template["scale"])
+        self.ui.offset_spinbox.setValue(template["offset"])
 
     def save(self, template):
-        template['scale'] = self.ui.scale_spinbox.value()
-        template['offset'] = self.ui.offset_spinbox.value()
+        template["scale"] = self.ui.scale_spinbox.value()
+        template["offset"] = self.ui.offset_spinbox.value()
 
     def encoder_argv(self, template):
         # convert from °C/V to °C/V:
-        return ['--scale', str(template['scale']),
-                '--offset', str(template['offset'])]
+        return [
+            "--scale",
+            str(template["scale"]),
+            "--offset",
+            str(template["offset"]),
+        ]
 
     def table_to_template(self, table, template):
-        template['scale'] = table.scale
-        template['offset'] = table.offset
+        template["scale"] = table.scale
+        template["offset"] = table.offset
+
 
 class NTC(Sensor_Params):
-    '''Note that the NTC parameters are line editors rather than spinboxes
+    """Note that the NTC parameters are line editors rather than spinboxes
     because their value can be any double value, including some really
     tiny values that are best entered via exponent notation.  The QT4
     double spinbox is not well setup for such values.
 
-    '''
+    """
 
     def set_input_enabled(self, enabled):
         self.ui.ntc_a_lineEdit.setEnabled(enabled)
         self.ui.ntc_b_lineEdit.setEnabled(enabled)
         self.ui.ntc_c_lineEdit.setEnabled(enabled)
         self.ui.ntc_m_lineEdit.setEnabled(enabled)
         self.ui.ntc_n_lineEdit.setEnabled(enabled)
         self.ui.ntc_k_lineEdit.setEnabled(enabled)
 
     def load(self, template):
-        self.ui.ntc_a_lineEdit.setText(template['ntc_a'])
-        self.ui.ntc_b_lineEdit.setText(template['ntc_b'])
-        self.ui.ntc_c_lineEdit.setText(template['ntc_c'])
-        self.ui.ntc_m_lineEdit.setText(template['ntc_m'])
-        self.ui.ntc_n_lineEdit.setText(template['ntc_n'])
-        self.ui.ntc_k_lineEdit.setText(template['ntc_k'])
+        self.ui.ntc_a_lineEdit.setText(template["ntc_a"])
+        self.ui.ntc_b_lineEdit.setText(template["ntc_b"])
+        self.ui.ntc_c_lineEdit.setText(template["ntc_c"])
+        self.ui.ntc_m_lineEdit.setText(template["ntc_m"])
+        self.ui.ntc_n_lineEdit.setText(template["ntc_n"])
+        self.ui.ntc_k_lineEdit.setText(template["ntc_k"])
 
     def save(self, template):
-        template['ntc_a'] = self.ui.ntc_a_lineEdit.text()
-        template['ntc_b'] = self.ui.ntc_b_lineEdit.text()
-        template['ntc_c'] = self.ui.ntc_c_lineEdit.text()
-        template['ntc_m'] = self.ui.ntc_m_lineEdit.text()
-        template['ntc_n'] = self.ui.ntc_n_lineEdit.text()
-        template['ntc_k'] = self.ui.ntc_k_lineEdit.text()
+        template["ntc_a"] = self.ui.ntc_a_lineEdit.text()
+        template["ntc_b"] = self.ui.ntc_b_lineEdit.text()
+        template["ntc_c"] = self.ui.ntc_c_lineEdit.text()
+        template["ntc_m"] = self.ui.ntc_m_lineEdit.text()
+        template["ntc_n"] = self.ui.ntc_n_lineEdit.text()
+        template["ntc_k"] = self.ui.ntc_k_lineEdit.text()
 
     def validate(self, template):
         bad_field = None
-        if invalid_double(template['ntc_a']):
+        if invalid_double(template["ntc_a"]):
             bad_field = self.ui.ntc_a_lineEdit
-        elif invalid_double(template['ntc_b']):
+        elif invalid_double(template["ntc_b"]):
             bad_field = self.ui.ntc_b_lineEdit
-        elif invalid_double(template['ntc_c']):
+        elif invalid_double(template["ntc_c"]):
             bad_field = self.ui.ntc_d_lineEdit
-        elif invalid_double(template['ntc_m']):
+        elif invalid_double(template["ntc_m"]):
             bad_field = self.ui.ntc_m_lineEdit
-        elif invalid_double(template['ntc_n']):
+        elif invalid_double(template["ntc_n"]):
             bad_field = self.ui.ntc_r1_lineEdit
-        elif invalid_double(template['ntc_k']):
+        elif invalid_double(template["ntc_k"]):
             bad_field = self.ui.ntc_r1_lineEdit
 
         if bad_field is not None:
-            QMessageBox.warning(self, 'Invalid number',
-                                'Please enter a value number.',
-                                QMessageBox.Ok)
+            QMessageBox.warning(
+                self,
+                "Invalid number",
+                "Please enter a value number.",
+                QMessageBox.Ok,
+            )
             bad_field.setFocus()
             return False
 
         return True
 
     def encoder_argv(self, template):
-        return ['--ntc-a', str(template['ntc_a']),
-                '--ntc-b', str(template['ntc_b']),
-                '--ntc-c', str(template['ntc_c']),
-                '--ntc-m', str(template['ntc_m']),
-                '--ntc-n', str(template['ntc_n']),
-                '--ntc-k', str(template['ntc_k'])]
+        return [
+            "--ntc-a",
+            str(template["ntc_a"]),
+            "--ntc-b",
+            str(template["ntc_b"]),
+            "--ntc-c",
+            str(template["ntc_c"]),
+            "--ntc-m",
+            str(template["ntc_m"]),
+            "--ntc-n",
+            str(template["ntc_n"]),
+            "--ntc-k",
+            str(template["ntc_k"]),
+        ]
 
     def table_to_template(self, table, template):
-        template['ntc_a'] = str(table.ntc_a)
-        template['ntc_b'] = str(table.ntc_b)
-        template['ntc_c'] = str(table.ntc_c)
-        template['ntc_m'] = str(table.ntc_m)
-        template['ntc_n'] = str(table.ntc_n)
-        template['ntc_k'] = str(table.ntc_k)
+        template["ntc_a"] = str(table.ntc_a)
+        template["ntc_b"] = str(table.ntc_b)
+        template["ntc_c"] = str(table.ntc_c)
+        template["ntc_m"] = str(table.ntc_m)
+        template["ntc_n"] = str(table.ntc_n)
+        template["ntc_k"] = str(table.ntc_k)
+
 
 class Pulse(Sensor_Params):
-    '''Note that the NTC parameters are line editors rather than spinboxes
+    """Note that the NTC parameters are line editors rather than spinboxes
     because their value can be any double value, including some really
     tiny values that are best entered via exponent notation.  The QT4
     double spinbox is not well setup for such values.
 
-    '''
+    """
 
     def set_input_enabled(self, enabled):
         self.ui.threshold_spinbox.setEnabled(enabled)
         self.ui.hysteresis_spinbox.setEnabled(enabled)
         self.ui.debounce_spinbox.setEnabled(enabled)
         self.ui.edge_comboBox.setEnabled(enabled)
 
     def load(self, template):
-        self.ui.threshold_spinbox.setValue(template['threshold'])
-        self.ui.hysteresis_spinbox.setValue(template['hysteresis'])
-        self.ui.debounce_spinbox.setValue(template['debounce_time'])
-        idx = 0		# default to 'rising edge'
-        edge = template['edge_mask']
-        if edge == 'falling':
+        self.ui.threshold_spinbox.setValue(template["threshold"])
+        self.ui.hysteresis_spinbox.setValue(template["hysteresis"])
+        self.ui.debounce_spinbox.setValue(template["debounce_time"])
+        idx = 0  # default to 'rising edge'
+        edge = template["edge_mask"]
+        if edge == "falling":
             idx = 1
-        elif edge == 'both':
+        elif edge == "both":
             idx = 2
         self.ui.edge_comboBox.setCurrentIndex(idx)
 
     def save(self, template):
-        mask = ['rising', 'falling', 'both']
-        template['threshold'] = self.ui.threshold_spinbox.value()
-        template['hysteresis'] = self.ui.hysteresis_spinbox.value()
-        template['debounce_time'] = self.ui.debounce_spinbox.value()
-        template['edge_mask'] = mask[self.ui.edge_comboBox.currentIndex()]
+        mask = ["rising", "falling", "both"]
+        template["threshold"] = self.ui.threshold_spinbox.value()
+        template["hysteresis"] = self.ui.hysteresis_spinbox.value()
+        template["debounce_time"] = self.ui.debounce_spinbox.value()
+        template["edge_mask"] = mask[self.ui.edge_comboBox.currentIndex()]
 
     def encoder_argv(self, template):
-        return ['--threshold', str(1e-3 * template['threshold']),
-                '--hysteresis', str(1e-3 * template['hysteresis']),
-                '--debounce-time', str(template['debounce_time']),
-                '--edge-mask', template['edge_mask']]
+        return [
+            "--threshold",
+            str(1e-3 * template["threshold"]),
+            "--hysteresis",
+            str(1e-3 * template["hysteresis"]),
+            "--debounce-time",
+            str(template["debounce_time"]),
+            "--edge-mask",
+            template["edge_mask"],
+        ]
 
     def table_to_template(self, table, template):
-        mask = ['none', 'rising', 'falling', 'both']
-        template['threshold'] = 1e3 * table.threshold
-        template['hysteresis'] = 1e3 * table.hysteresis
-        template['debounce_time'] = table.debounce_time
-        template['edge_mask'] = mask[table.edge_mask]
+        mask = ["none", "rising", "falling", "both"]
+        template["threshold"] = 1e3 * table.threshold
+        template["hysteresis"] = 1e3 * table.hysteresis
+        template["debounce_time"] = table.debounce_time
+        template["edge_mask"] = mask[table.edge_mask]
```

### Comparing `CTid-programmer-1.4.0/ctid_programmer/sn.py` & `CTid-programmer-1.4.1/ctid_programmer/sn.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,124 +25,126 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 import pickle
 
-from abc import ABC, abstractmethod	# ABC = abstract base class
+from abc import ABC, abstractmethod  # ABC = abstract base class
+
 
 class Error(Exception):
     pass
 
+
 class SpaceExhausted(Error):
     pass
 
-class Manager(ABC):
 
+class Manager(ABC):
     def __init__(self, ui, state_path):
-        '''Create a SN manager object.  UI is the QT user-interface object
+        """Create a SN manager object.  UI is the QT user-interface object
         that can be used to interact with the user, e.g., to ask
         confirmation questions or to ask for authentication
         credentials, for example.  STATE_PATH is the path of a
         file that the manager can use to store state in.
 
-        '''
+        """
         self.ui = ui
         self.path = state_path
         self.product = None
         self.serial = {}
         self._load_state()
 
     def has_calibration_data(self):
-        '''Should return True if this serial-number manager can retrieve
+        """Should return True if this serial-number manager can retrieve
         calibration data with get_calibration_data(), False otherwise.
 
-        '''
+        """
         return False
 
     @abstractmethod
     def set_preferences(self, prefs):
-        '''This method must be called whenever the SN manager's preferences
+        """This method must be called whenever the SN manager's preferences
         may have changed.
 
-        '''
+        """
 
     def set_product(self, manufacturer, model):
-        '''Set the product for which to manage serial numbers.  Each product
+        """Set the product for which to manage serial numbers.  Each product
         has its own serial-number space, so this function must be
         called at least once before any serial-numbers can be
         allocated.
 
-        '''
+        """
         if manufacturer is None or model is None:
             self.product = None
             return True
 
-        self.product = '%s-%s' % (manufacturer, model)
+        self.product = "%s-%s" % (manufacturer, model)
         return True
 
     def restore_product(self, product):
-        '''Restore the product to PRODUCT.'''
+        """Restore the product to PRODUCT."""
         self.product = product
 
     def activate(self, sn):
-        '''Activate automatic serial number generation using this SN manager.
+        """Activate automatic serial number generation using this SN manager.
         SN is the serial number that was most recently used in manual
         mode.  It may be None if the most recently used serial number
         is unavailable.  Some SN managers may choose to offer the next
         automatic serial number based on this number.
 
-        '''
+        """
 
     def deactivate(self):
-        '''Called when this SN manager is no longer used.  That is, when this
+        """Called when this SN manager is no longer used.  That is, when this
         method gets called when the user switches to manually entered
         serial-numbers.
 
-        '''
+        """
 
     def get(self):
-        '''Get the serial-number to be used next.'''
+        """Get the serial-number to be used next."""
         if self.product is None:
             return None
         return self.serial.get(self.product)
 
     def set(self, sn):
         if self.product is None:
             return
 
         self.serial[self.product] = sn
         self._save_state()
 
     @abstractmethod
     def commit(self, sn, info, auto_serial_number):
-        '''This is called after serial-number SN has been committed
+        """This is called after serial-number SN has been committed
         (programmed) into a device.  INFO must be a dictionary of
         information to be associated with this device.  Not all SN
         managers can preserve INFO.
 
         Note that this gets called even if the SN was manually
         selected (indicated by AUTH_SERIAL_NUMBER==False).  This is
         done such that if a device needs to be re-programmed (e.g.,
         with a different calibration), we get notified here with the
         latest INFO that is used for this SN.
 
-        '''
+        """
 
     def get_cal_data(self, sn):
-        '''Return the calibration data for the current product with serial
+        """Return the calibration data for the current product with serial
         number SN or None if no such data is available.
 
-        '''
+        """
         return None
 
     def _load_state(self):
         try:
-            with open(self.path, 'rb') as f:
+            with open(self.path, "rb") as f:
                 self.serial = pickle.load(f)
         except IOError:
             self.serial = {}
 
     def _save_state(self):
-        with open(self.path, 'wb') as f:
+        with open(self.path, "wb") as f:
             pickle.dump(self.serial, f)
```

### Comparing `CTid-programmer-1.4.0/ctid_programmer/sn_egauge.py` & `CTid-programmer-1.4.1/ctid_programmer/sn_egauge.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 # pylint: disable=no-name-in-module
 #
-'''Serial number allocation via the eGauge serial-number API.'''
+"""Serial number allocation via the eGauge serial-number API."""
 
 import logging
 import os
 
 from PySide2.QtWidgets import QMessageBox
 
 from egauge import ctid
@@ -41,170 +41,197 @@
 
 from egauge.webapi.cloud.credentials import CredentialsManager, LoginCanceled
 
 from ctid_programmer import sn
 
 log = logging.getLogger(__name__)
 
+
 class Manager(sn.Manager):
     def auth_wrapper(self, method, *args, **kwargs):
         while True:
             try:
                 ret = method(*args, *kwargs)
                 self.credentials_manager.previous_login_failed = False
                 return ret
             except webapi.json_api.UnauthenticatedError:
                 pass
             except LoginCanceled:
                 return None
 
     def __init__(self, ui, state_directory_path):
-        SerialNumberWithAuth \
-            = webapi.decorate_public(webapi.cloud.SerialNumber,
-                                     self.auth_wrapper)
+        SerialNumberWithAuth = webapi.decorate_public(
+            webapi.cloud.SerialNumber, self.auth_wrapper
+        )
         self.credentials_manager = CredentialsManager(ui)
         self.sn_api = SerialNumberWithAuth(
-            auth=webapi.auth.TokenAuth(ask=self.credentials_manager.ask))
-        super().__init__(ui, os.path.join(state_directory_path,
-                                          'egauge_sn_api.bin'))
+            auth=webapi.auth.TokenAuth(ask=self.credentials_manager.ask)
+        )
+        super().__init__(
+            ui, os.path.join(state_directory_path, "egauge_sn_api.bin")
+        )
 
     def has_calibration_data(self):
-        '''Should return True if this serial-number manager can retrieve
+        """Should return True if this serial-number manager can retrieve
         calibration data with get_calibration_data(), False otherwise.
 
-        '''
+        """
         return True
 
     def set_product(self, manufacturer, model):
-        log.debug('set_product: manufacturer=%s, model=%s',
-                  manufacturer, model)
+        log.debug(
+            "set_product: manufacturer=%s, model=%s", manufacturer, model
+        )
 
         mfg = ctid.mfg_short_name(manufacturer)
         if not super().set_product(mfg, model):
             return False
 
         model_list = None
         try:
             model_list = self.sn_api.get_models()
         except webapi.Error:
             pass
 
         if model_list is None:
-            QMessageBox.critical(self.ui, 'Serial-number service failed',
-                                 'Serial-number service failed to return '
-                                 'model-name list.  '
-                                 'Reverting to manual '
-                                 'serial numbers.', QMessageBox.Ok)
+            QMessageBox.critical(
+                self.ui,
+                "Serial-number service failed",
+                "Serial-number service failed to return "
+                "model-name list.  "
+                "Reverting to manual "
+                "serial numbers.",
+                QMessageBox.Ok,
+            )
             return False
 
         found = False
         for r in model_list:
-            if r['name'] == self.product:
+            if r["name"] == self.product:
                 found = True
                 break
         if found:
             return True
 
-        choice = QMessageBox \
-                 .question(self.ui,
-                           'Create Serial-Number Record?',
-                           ('The eGauge Serial-Number service has no record '
-                            'of product \"%s %s\".  Would you like to '
-                            'create one?'
-                            % (mfg, model)), QMessageBox.Yes | QMessageBox.No)
+        choice = QMessageBox.question(
+            self.ui,
+            "Create Serial-Number Record?",
+            (
+                "The eGauge Serial-Number service has no record "
+                'of product "%s %s".  Would you like to '
+                "create one?" % (mfg, model)
+            ),
+            QMessageBox.Yes | QMessageBox.No,
+        )
         if choice == QMessageBox.No:
             return False
 
         result = None
         try:
-            result = self.sn_api.create_model(self.product, 0xffffff)
+            result = self.sn_api.create_model(self.product, 0xFFFFFF)
         except webapi.Error:
-            log.exception('sn_api.create_model() for model "%s" failed',
-                          self.product)
+            log.exception(
+                'sn_api.create_model() for model "%s" failed', self.product
+            )
         return result
 
     def set_preferences(self, prefs):
         pass
 
     def get(self):
         # see if we already have a serial-number for this product:
         sn = super().get()
         if sn is not None:
-            log.debug('get: product=%s; using existing SN %s',
-                      self.product, sn)
+            log.debug(
+                "get: product=%s; using existing SN %s", self.product, sn
+            )
             return sn
 
-        log.debug('get: product=%s; allocating new SN ', self.product)
+        log.debug("get: product=%s; allocating new SN ", self.product)
         return self._allocate_sn()
 
     def commit(self, sn, info, auto_serial_number):
         meta = {}
         try:
             ret = self.sn_api.get_metadata(self.product, sn)
             if ret is not None:
                 meta = ret
         except webapi.Error:
-            log.exception('commit: no metadata found for %s SN %s.',
-                          self.product, sn)
-        meta['ctid'] = info
+            log.exception(
+                "commit: no metadata found for %s SN %s.", self.product, sn
+            )
+        meta["ctid"] = info
         try:
             self.sn_api.set_metadata(self.product, sn, meta)
         except webapi.Error as e:
-            QMessageBox.warning(self.ui, 'Failed to save CTid info',
-                                'Failed to save meta data for product %s '
-                                'serial-number %s: %s.' \
-                                % (self.product, sn, e), QMessageBox.Ok)
+            QMessageBox.warning(
+                self.ui,
+                "Failed to save CTid info",
+                "Failed to save meta data for product %s "
+                "serial-number %s: %s." % (self.product, sn, e),
+                QMessageBox.Ok,
+            )
 
         if auto_serial_number:
-            self._allocate_sn()		# allocate serial number to use next
+            self._allocate_sn()  # allocate serial number to use next
         else:
             super().set(None)
 
     def get_cal_data(self, sn):
         try:
             meta = self.sn_api.get_metadata(self.product, sn)
         except webapi.Error:
-            log.exception('Failed to get cal data for %s SN %s.',
-                          self.product, sn)
+            log.exception(
+                "Failed to get cal data for %s SN %s.", self.product, sn
+            )
             return None
 
         if meta is None:
             return None
-        if 'cal' in meta:
-            cal = meta['cal']
-        elif 'ntc' in meta:
+        if "cal" in meta:
+            cal = meta["cal"]
+        elif "ntc" in meta:
             # for backwards compatibility:
             cal = {}
-            for key, value in meta['ntc'].items():
-                cal['ntc_%s' % key] = str(value)
+            for key, value in meta["ntc"].items():
+                cal["ntc_%s" % key] = str(value)
         else:
             return None
         return cal
 
     def _allocate_sn(self):
         # allocate a new serial number:
         super().set(None)
         try:
             sn = self.sn_api.allocate(self.product)
             if sn is None:
                 return None
         except webapi.Error as e:
-            log.exception('Failed to allocate SN for product %s.',
-                          self.product)
-            if len(e.args) > 2 and isinstance(e.args[2], list) \
-               and len(e.args[2]) >= 1:
+            log.exception(
+                "Failed to allocate SN for product %s.", self.product
+            )
+            if (
+                len(e.args) > 2
+                and isinstance(e.args[2], list)
+                and len(e.args[2]) >= 1
+            ):
                 errors = e.args[2]
                 # If this product is out of serial-numbers, let the user know:
-                if errors[0] == 'Maximum serial number reached':
+                if errors[0] == "Maximum serial number reached":
                     raise sn.SpaceExhausted
-                QMessageBox.critical(self.ui, 'Serial-number Failure',
-                                     'Failed to allocate serial-number: %s'
-                                     % '\n'.join(errors),
-                                     QMessageBox.Ok)
+                QMessageBox.critical(
+                    self.ui,
+                    "Serial-number Failure",
+                    "Failed to allocate serial-number: %s" % "\n".join(errors),
+                    QMessageBox.Ok,
+                )
             else:
-                QMessageBox.critical(self.ui, 'Serial-number Failure',
-                                     'Failed to allocate serial-number: %s'
-                                     % e, QMessageBox.Ok)
+                QMessageBox.critical(
+                    self.ui,
+                    "Serial-number Failure",
+                    "Failed to allocate serial-number: %s" % e,
+                    QMessageBox.Ok,
+                )
             return None
 
         super().set(sn)
         return sn
```

### Comparing `CTid-programmer-1.4.0/ctid_programmer/sn_local.py` & `CTid-programmer-1.4.1/ctid_programmer/sn_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,57 +23,61 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
-'''Local serial number manager.
+"""Local serial number manager.
 
 This manager works locally (no network connectivity required) and
 assumes that there may be up to N different programming stations.  It
 returns a sequence of serial numbers that are guaranteed to be unique,
 provided the station id of each station is unique and the step value
 is >= N.
 
-'''
+"""
 
 import os
 
 from PySide2.QtWidgets import QMessageBox
 
 from ctid_programmer import sn
 
-class Manager(sn.Manager):
 
+class Manager(sn.Manager):
     def __init__(self, ui, state_directory_path):
-        super().__init__(ui, os.path.join(state_directory_path,
-                                          'serial_numbers.bin'))
+        super().__init__(
+            ui, os.path.join(state_directory_path, "serial_numbers.bin")
+        )
         self.increment = 1
         self.first = 0
 
     def set_preferences(self, prefs):
         self._set_stepping(prefs.sn_increment, prefs.station_id)
 
     def activate(self, sn):
         old_sn = self.get()
         if old_sn is None:
             self._reset_serial_number(sn)
         elif sn != old_sn:
-            choice = QMessageBox \
-                     .question(self.ui,
-                               'Serial Number Selection',
-                               ('Would you like to switch to %d '
-                                'as the next automatic serial number '
-                                'for this product?  If you press "No", '
-                                'the program will revert back to '
-                                'the old sequence and use %d '
-                                'as the next automatic serial number.'
-                                % (sn, old_sn)),
-                               QMessageBox.Yes, QMessageBox.No)
+            choice = QMessageBox.question(
+                self.ui,
+                "Serial Number Selection",
+                (
+                    "Would you like to switch to %d "
+                    "as the next automatic serial number "
+                    'for this product?  If you press "No", '
+                    "the program will revert back to "
+                    "the old sequence and use %d "
+                    "as the next automatic serial number." % (sn, old_sn)
+                ),
+                QMessageBox.Yes,
+                QMessageBox.No,
+            )
             if choice == QMessageBox.Yes:
                 self._reset_serial_number(sn)
 
     def deactivate(self):
         pass
 
     def get(self):
@@ -87,18 +91,20 @@
         if auto_serial_number:
             self._increment_serial_number()
         else:
             super().set(None)
 
     def _set_stepping(self, increment, first):
         if increment < 1:
-            raise ValueError('Increment must be greater than 0.')
+            raise ValueError("Increment must be greater than 0.")
         if first >= increment:
-            raise ValueError('First valid serial-number must be in range '
-                             '0..%d.' % (self.increment - 1))
+            raise ValueError(
+                "First valid serial-number must be in range "
+                "0..%d." % (self.increment - 1)
+            )
         self.increment = increment
         self.first = first
 
     def _next_valid_serial_number(self, sn):
         mod = sn % self.increment
         if mod != self.first:
             # round up to first valid serial number
```

### Comparing `CTid-programmer-1.4.0/ctid_programmer/template.py` & `CTid-programmer-1.4.1/ctid_programmer/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,37 +26,38 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 import json
 import os
 
+
 class Manager:
     def __init__(self, state_directory_path):
-        self.path = os.path.join(state_directory_path, 'templates.json')
+        self.path = os.path.join(state_directory_path, "templates.json")
         self.templates = {}
         try:
-            with open(self.path, 'r') as f:
+            with open(self.path, "r") as f:
                 self.templates = json.load(f)
         except FileNotFoundError:
             try:
                 # try to create a new, empty file:
-                with open(self.path, 'w') as f:
+                with open(self.path, "w") as f:
                     json.dump({}, f)
             except IOError:
                 pass
         except IOError:
             pass
 
     def _save_state(self):
-        with open(self.path, 'w') as f:
+        with open(self.path, "w") as f:
             json.dump(self.templates, f, sort_keys=True, indent=2)
 
     def items(self):
-        '''Return a iterator of {name: template} items.'''
+        """Return a iterator of {name: template} items."""
         return self.templates.items()
 
     def load(self, name):
         return self.templates[name]
 
     def save(self, template, name):
         self.templates[name] = template
```

### Comparing `CTid-programmer-1.4.0/setup.py` & `CTid-programmer-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name='CTid-programmer',
-    version='1.4.0',
+    version='1.4.1',
     packages=setuptools.find_packages(),
     package_data={
         '': ['resources/code/*.hex']
     },
-    install_requires=['egauge-python>=0.6.0,!=0.21',
+    install_requires=['egauge-python>=0.7.2,!=0.21',
                       'importlib_resources', 'wheel'],
     entry_points={
         'console_scripts': [
             'CTid-programmer = ctid_programmer.programmer:main'
         ]
     },
     license='MIT License',  # example license
```

