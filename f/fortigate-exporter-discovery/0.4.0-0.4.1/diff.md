# Comparing `tmp/fortigate-exporter-discovery-0.4.0.tar.gz` & `tmp/fortigate-exporter-discovery-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate-exporter-discovery-0.4.0.tar", last modified: Wed Apr 26 14:36:30 2023, max compression
+gzip compressed data, was "fortigate-exporter-discovery-0.4.1.tar", last modified: Thu Apr 27 12:57:36 2023, max compression
```

## Comparing `fortigate-exporter-discovery-0.4.0.tar` & `fortigate-exporter-discovery-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/fmg_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/fw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/http_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/fmg_discovery/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 14:36:30.000000 fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:36:30.896958 fortigate-exporter-discovery-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 14:36:07.000000 fortigate-exporter-discovery-0.4.0/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:57:36.789427 fortigate-exporter-discovery-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-27 12:57:36.789427 fortigate-exporter-discovery-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:57:36.785427 fortigate-exporter-discovery-0.4.1/fmg_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/fmg_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/fmg_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/fmg_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/fw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/http_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/fmg_discovery/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:57:36.789427 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-27 12:57:36.000000 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-27 12:57:36.000000 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:57:36.000000 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:57:36.000000 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-27 12:57:36.000000 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 12:57:36.000000 fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:57:36.789427 fortigate-exporter-discovery-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:57:36.789427 fortigate-exporter-discovery-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-27 12:57:13.000000 fortigate-exporter-discovery-0.4.1/tests/test_dummy.py
```

### Comparing `fortigate-exporter-discovery-0.4.0/LICENSE` & `fortigate-exporter-discovery-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/PKG-INFO` & `fortigate-exporter-discovery-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.4.0/README.md` & `fortigate-exporter-discovery-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/__init__.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/__main__.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/environments.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/exceptions.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/exceptions.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/file_service_discovery.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/file_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_api.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/fmg_api.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_collector.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/fmg_collector.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/fmg_metrics.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/fmg_metrics.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/fmglogging.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/fw.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/fw.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.ha_slave: List[Dict[str, Any]] = []
 
     def _as_labels(self) -> Dict[str, str]:
 
         labels = self.labels.copy()
         labels['adom'] = self.adom
         labels['latitude'] = self.latitude
-        labels['latitude'] = self.latitude
+        labels['longitude'] = self.longitude
         labels['platform'] = self.platform
 
         if self.token:
             labels['token'] = self.token
         if self.profile:
             labels['profile'] = self.profile
 
@@ -68,32 +68,34 @@
             valid = False
         if not self.ip:
             cause = f"Missing ip {cause}"
             valid = False
         if self.ip and not ipaddress.ip_address(self.ip):
             cause = f"Not a ip4/ip6 address {cause}"
             valid = False
+        if self.ip and self.ip == '0.0.0.0':
+            cause = f"IP is 0.0.0.0 {cause}"
+            valid = False
         if not self.token:
             cause = f"Missing token {cause}"
             valid = False
 
         return valid, cause
 
     def as_prometheus_file_sd_entry(self) -> Dict[str, Any]:
         return {'targets': [f"https://{self.ip}:{self.port}"], 'labels': self._as_labels()}
 
 
 def fw_factory(adom, device) -> Fortigate:
     fw = Fortigate(name=device['name'], ip=device['ip'])
     # Discovery
-    fw.adom = adom['name'].strip()
     fw.latitude = device['latitude'].strip()
     fw.longitude = device['longitude'].strip()
     fw.platform = device['platform_str'].strip()
-    # fw.labels['name'] = device['name']
+
     if 'labels' in adom:
         fw.labels.update(adom['labels'])
     if 'token' in adom['fortigate']:
         fw.token = adom['fortigate']['token']
     if 'port' in adom['fortigate']:
         fw.port = adom['fortigate']['port']
     if 'profile' in adom['fortigate']:
```

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/http_service_discovery.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/http_service_discovery.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fmg_discovery/transform.py` & `fortigate-exporter-discovery-0.4.1/fmg_discovery/transform.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/PKG-INFO` & `fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-exporter-discovery
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Prometheus file discovery for Fortigate's based on FortiManager
 Home-page: https://github.com/thenodon/fortigate-exporter-discovery
 Author: thenodon
 Author-email: aha@ingby.com
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fortigate-exporter-discovery-0.4.0/fortigate_exporter_discovery.egg-info/SOURCES.txt` & `fortigate-exporter-discovery-0.4.1/fortigate_exporter_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/setup.py` & `fortigate-exporter-discovery-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `fortigate-exporter-discovery-0.4.0/tests/test_dummy.py` & `fortigate-exporter-discovery-0.4.1/tests/test_dummy.py`

 * *Files identical despite different names*

