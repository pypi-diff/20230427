# Comparing `tmp/fortigate-exporter-discovery-0.3.3.tar.gz` & `tmp/fortigate-exporter-discovery-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate-exporter-discovery-0.3.3.tar", last modified: Sun Apr 23 11:45:32 2023, max compression
+gzip compressed data, was "fortigate-exporter-discovery-0.4.0.tar", last modified: Wed Apr 26 14:36:30 2023, max compression
```

## Comparing `fortigate-exporter-discovery-0.3.3.tar` & `fortigate-exporter-discovery-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/fmg_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/fmg_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/fw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/fmg_discovery/http_service_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 11:45:32.000000 fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:45:32.426667 fortigate-exporter-discovery-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 11:45:04.000000 fortigate-exporter-discovery-0.3.3/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/fmg_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/http_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/tests/test_dummy.py
```

### Comparing `fortigate-exporter-discovery-0.3.3/LICENSE` & `fortigate-exporter-discovery-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/PKG-INFO` & `fortigate-exporter-discovery-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,21 @@
-Metadata-Version: 2.1
-Name: fortigate-exporter-discovery
-Version: 0.3.3
-Summary: A Prometheus file discovery for Fortigate's based on FortiManager
-Home-page: https://github.com/thenodon/fortigate-exporter-discovery
-Author: thenodon
-Author-email: aha@ingby.com
-License: GPLv3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 [![Python application](https://github.com/thenodon/fortigate-exporter-discovery//actions/workflows/python-app.yml/badge.svg)](https://github.com/thenodon/fortigate-exporter-discovery//actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/fortigate-exporter-discovery.svg)](https://badge.fury.io/py/fortigate-exporter-discovery)
 
 fortigate-exporter-discovery
 ------------------------
 # Overview
 
 The fortigate-exporter-discovery is a Prometheus discovery tool that use a Fortimanager instance
-to get fortigate's based on an adom. 
+to get fortigate's based on adoms. 
 It works both for file and http service discovery.
 
+The tool can also work as an exporter for metrics related to the relation between a Fortimanager and its Fortigate's.
+This is only supported when run in `server` mode.
+
 The tool work with the [fortigate-exporter](https://github.com/bluecmd/fortigate_exporter).
 > It requires that the following pull request is accepted https://github.com/bluecmd/fortigate_exporter/pull/206 or 
 > you can use https://github.com/thenodon/fortigate_exporter. 
 
 # Configuration
 
 The configuration file include the credentials for the Fortimanager and the configuration for each adom.
@@ -87,19 +77,36 @@
 FMG_DISCOVERY_CONFIG=config.yml
 FMG_DISCOVERY_BASIC_AUTH_ENABLED=true
 FMG_DISCOVERY_BASIC_AUTH_USERNAME=foo
 FMG_DISCOVERY_BASIC_AUTH_PASSWORD=bar
 FMG_DISCOVERY_LOG_LEVEL=INFO
 python -m fmg_discovery --server
 ```
-Test by curl
+Test discovery by curl
 
 ```shell
 curl -ufoo:bar localhost:9693/prometheus-sd-targets
 ```
+
+Test exporter by curl
+
+```shell
+curl -ufoo:bar localhost:9693/metrics
+# HELP fmg_conf_status Configuration status 1==insync 0==all other states
+# TYPE fmg_conf_status gauge
+....
+# HELP fmg_conn_status Connection status 1==up 0==all other states
+# TYPE fmg_conn_status gauge
+....
+# HELP fmg_conn_mode Connection mode 1==active 0==all other states
+# TYPE fmg_conn_mode gauge
+....
+
+```
+
 # Prometheus job configuration
 
 Example:
 
 ```yaml
   - job_name: 'fortigate_exporter'
     metrics_path: /probe
```

### Comparing `fortigate-exporter-discovery-0.3.3/fmg_discovery/__init__.py` & `fortigate-exporter-discovery-0.4.0/fmg_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/fmg_discovery/__main__.py` & `fortigate-exporter-discovery-0.4.0/fmg_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/fmg_discovery/environments.py` & `fortigate-exporter-discovery-0.4.0/fmg_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/fmg_discovery/file_service_discovery.py` & `fortigate-exporter-discovery-0.4.0/fmg_discovery/file_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/fmg_discovery/fmg_api.py` & `fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import json
 
 from typing import List, Dict, Any
 
 import requests
 import urllib3
 
-from fmg_discovery.fw import Fortigate
+from fmg_discovery.fw import Fortigate, fw_factory
 from fmg_discovery.fmglogging import Log
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 log = Log(__name__)
 
 
@@ -81,29 +81,15 @@
             return {}
         # Loop for each adom
         all_adom_devices = {}
         for adom in self.fmg_configuration['fmg']['adoms']:
             all_devices = []
             devices = self._get_fw_devices(adom['name'])
             for device in devices:
-                fw = Fortigate(name=device['name'], ip=device['ip'])
-                fw.labels['adom'] = adom['name'].strip()
-                fw.labels['latitude'] = device['latitude'].strip()
-                fw.labels['longitude'] = device['longitude'].strip()
-                fw.labels['platform'] = device['platform_str'].strip()
-                #fw.labels['name'] = device['name']
-
-                if 'labels' in adom:
-                    fw.labels.update(adom['labels'])
-                if 'token' in adom['fortigate']:
-                    fw.token = adom['fortigate']['token']
-                if 'port' in adom['fortigate']:
-                    fw.port = adom['fortigate']['port']
-                if 'profile' in adom['fortigate']:
-                    fw.profile = adom['fortigate']['profile']
+                fw = fw_factory(adom, device)
                 valid, cause = fw.valid()
                 if not valid:
                     log.warn_fmt({'operation': 'fw_validate', 'adom': adom['name'], 'fw': fw.name, "status": 'false',
                                   "cause": cause})
                     continue
                 all_devices.append(fw)
             all_adom_devices[adom['name']] = all_devices
```

### Comparing `fortigate-exporter-discovery-0.3.3/fmg_discovery/fmglogging.py` & `fortigate-exporter-discovery-0.4.0/fmg_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/PKG-INFO` & `fortigate-exporter-discovery-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.3.3
+Version: 0.4.0
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,17 +15,20 @@
 [![PyPI version](https://badge.fury.io/py/fortigate-exporter-discovery.svg)](https://badge.fury.io/py/fortigate-exporter-discovery)
 
 fortigate-exporter-discovery
 ------------------------
 # Overview
 
 The fortigate-exporter-discovery is a Prometheus discovery tool that use a Fortimanager instance
-to get fortigate's based on an adom. 
+to get fortigate's based on adoms. 
 It works both for file and http service discovery.
 
+The tool can also work as an exporter for metrics related to the relation between a Fortimanager and its Fortigate's.
+This is only supported when run in `server` mode.
+
 The tool work with the [fortigate-exporter](https://github.com/bluecmd/fortigate_exporter).
 > It requires that the following pull request is accepted https://github.com/bluecmd/fortigate_exporter/pull/206 or 
 > you can use https://github.com/thenodon/fortigate_exporter. 
 
 # Configuration
 
 The configuration file include the credentials for the Fortimanager and the configuration for each adom.
@@ -87,19 +90,36 @@
 FMG_DISCOVERY_CONFIG=config.yml
 FMG_DISCOVERY_BASIC_AUTH_ENABLED=true
 FMG_DISCOVERY_BASIC_AUTH_USERNAME=foo
 FMG_DISCOVERY_BASIC_AUTH_PASSWORD=bar
 FMG_DISCOVERY_LOG_LEVEL=INFO
 python -m fmg_discovery --server
 ```
-Test by curl
+Test discovery by curl
 
 ```shell
 curl -ufoo:bar localhost:9693/prometheus-sd-targets
 ```
+
+Test exporter by curl
+
+```shell
+curl -ufoo:bar localhost:9693/metrics
+# HELP fmg_conf_status Configuration status 1==insync 0==all other states
+# TYPE fmg_conf_status gauge
+....
+# HELP fmg_conn_status Connection status 1==up 0==all other states
+# TYPE fmg_conn_status gauge
+....
+# HELP fmg_conn_mode Connection mode 1==active 0==all other states
+# TYPE fmg_conn_mode gauge
+....
+
+```
+
 # Prometheus job configuration
 
 Example:
 
 ```yaml
   - job_name: 'fortigate_exporter'
     metrics_path: /probe
```

### Comparing `fortigate-exporter-discovery-0.3.3/fortigate_exporter_discovery.egg-info/SOURCES.txt` & `fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE
 NOTICE
 README.md
 setup.py
 fmg_discovery/__init__.py
 fmg_discovery/__main__.py
 fmg_discovery/environments.py
+fmg_discovery/exceptions.py
 fmg_discovery/file_service_discovery.py
 fmg_discovery/fmg_api.py
+fmg_discovery/fmg_collector.py
+fmg_discovery/fmg_metrics.py
 fmg_discovery/fmglogging.py
 fmg_discovery/fw.py
 fmg_discovery/http_service_discovery.py
+fmg_discovery/transform.py
 fortigate_exporter_discovery.egg-info/PKG-INFO
 fortigate_exporter_discovery.egg-info/SOURCES.txt
 fortigate_exporter_discovery.egg-info/dependency_links.txt
 fortigate_exporter_discovery.egg-info/not-zip-safe
 fortigate_exporter_discovery.egg-info/requires.txt
 fortigate_exporter_discovery.egg-info/top_level.txt
 tests/test_dummy.py
```

### Comparing `fortigate-exporter-discovery-0.3.3/setup.py` & `fortigate-exporter-discovery-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.3.3/tests/test_dummy.py` & `fortigate-exporter-discovery-0.4.0/tests/test_dummy.py`

 * *Files identical despite different names*

