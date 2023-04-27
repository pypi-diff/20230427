# Comparing `tmp/octodns-gcore-0.0.3.tar.gz` & `tmp/octodns-gcore-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-gcore-0.0.3.tar", last modified: Mon Nov 21 15:46:29 2022, max compression
+gzip compressed data, was "octodns-gcore-0.0.4.tar", last modified: Thu Apr 27 09:25:08 2023, max compression
```

## Comparing `octodns-gcore-0.0.3.tar` & `octodns-gcore-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-21 15:46:29.850880 octodns-gcore-0.0.3/
--rw-r--r--   0 ross       (501) staff       (20)     2513 2022-11-21 15:46:29.850580 octodns-gcore-0.0.3/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     2160 2022-11-20 16:25:51.000000 octodns-gcore-0.0.3/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-21 15:46:29.848299 octodns-gcore-0.0.3/octodns_gcore/
--rw-r--r--   0 ross       (501) staff       (20)    19828 2022-11-21 15:46:18.000000 octodns-gcore-0.0.3/octodns_gcore/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-21 15:46:29.850268 octodns-gcore-0.0.3/octodns_gcore.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     2513 2022-11-21 15:46:29.000000 octodns-gcore-0.0.3/octodns_gcore.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      228 2022-11-21 15:46:29.000000 octodns-gcore-0.0.3/octodns_gcore.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2022-11-21 15:46:29.000000 octodns-gcore-0.0.3/octodns_gcore.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      224 2022-11-21 15:46:29.000000 octodns-gcore-0.0.3/octodns_gcore.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       14 2022-11-21 15:46:29.000000 octodns-gcore-0.0.3/octodns_gcore.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)       38 2022-11-21 15:46:29.850958 octodns-gcore-0.0.3/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     1718 2022-10-26 15:20:24.000000 octodns-gcore-0.0.3/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-27 09:25:08.264088 octodns-gcore-0.0.4/
+-rw-r--r--   0 ross       (501) staff       (20)     2041 2023-04-27 09:25:08.263777 octodns-gcore-0.0.4/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     1711 2023-01-22 16:05:30.000000 octodns-gcore-0.0.4/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-27 09:25:08.261335 octodns-gcore-0.0.4/octodns_gcore/
+-rw-r--r--   0 ross       (501) staff       (20)    23192 2023-04-27 09:24:56.000000 octodns-gcore-0.0.4/octodns_gcore/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-27 09:25:08.262894 octodns-gcore-0.0.4/octodns_gcore.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     2041 2023-04-27 09:25:08.000000 octodns-gcore-0.0.4/octodns_gcore.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      280 2023-04-27 09:25:08.000000 octodns-gcore-0.0.4/octodns_gcore.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-04-27 09:25:08.000000 octodns-gcore-0.0.4/octodns_gcore.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      238 2023-04-27 09:25:08.000000 octodns-gcore-0.0.4/octodns_gcore.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       14 2023-04-27 09:25:08.000000 octodns-gcore-0.0.4/octodns_gcore.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      306 2023-02-04 19:18:58.000000 octodns-gcore-0.0.4/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-04-27 09:25:08.264181 octodns-gcore-0.0.4/setup.cfg
+-rw-r--r--   0 ross       (501) staff       (20)     1812 2023-02-04 19:18:58.000000 octodns-gcore-0.0.4/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-27 09:25:08.263298 octodns-gcore-0.0.4/tests/
+-rw-r--r--   0 ross       (501) staff       (20)    31050 2023-04-06 18:40:52.000000 octodns-gcore-0.0.4/tests/test_octodns_provider_gcore.py
```

### Comparing `octodns-gcore-0.0.3/PKG-INFO` & `octodns-gcore-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: octodns-gcore
-Version: 0.0.3
-Summary:  EdgeCenter DNS & G-Core Labs DNS v2 API provider for octoDNS
+Version: 0.0.4
+Summary:  Gcore DNS v2 API provider for octoDNS
 Home-page: https://github.com/octodns/octodns-gcore
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
-## EdgeCenter DNS & G-Core Labs DNS v2 API provider for octoDNS
+## Gcore DNS v2 API provider for octoDNS
 
-An [octoDNS](https://github.com/octodns/octodns/) provider that targets [EdgeCenter DNS](https://edgecenter.ru/dns/) and [G-Core Labs DNS](https://gcorelabs.com/dns/).
+An [octoDNS](https://github.com/octodns/octodns/) provider that targets [Gcore DNS](https://gcore.com/dns/).
 
 ### Installation
 
 #### Command line
 
 ```
 pip install octodns-gcore
@@ -41,46 +41,28 @@
 # Start with the latest/specific versions and don't just copy what's here
 -e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
 -e git+https://git@github.com/octodns/octodns-gcore.git@ec9661f8b335241ae4746eea467a8509205e6a30#egg=octodns_gcore
 ```
 
 ### Configuration
 
-
-#### EdgeCenterProvider
-
-```
-providers:
-  ec:
-    class: octodns_gcore.EdgeCenterProvider
-    # Your API key
-    token: env/EC_TOKEN
-    token_type: APIKey
-    # or login + password
-    #login: env/EC_LOGIN
-    #password: env/EC_PASSWORD
-    #auth_url: https://api.edgecenter.ru/id
-    #url: https://api.edgecenter.ru/dns/v2
-    #records_per_response: 1
-```
-
 #### GCoreProvider
 
 ```yaml
 providers:
   gcore:
     class: octodns_gcore.GCoreProvider
     # Your API key
     token: env/GCORE_TOKEN
     token_type: APIKey
     # or login + password
     #login: env/GCORE_LOGIN
     #password: env/GCORE_PASSWORD
-    #auth_url: https://api.gcorelabs.com/id
-    #url: https://api.gcorelabs.com/dns/v2
+    #auth_url: https://api.gcore.com/iam
+    #url: https://api.gcore.com/dns/v2
     #records_per_response: 1
 ```
 
 ### Support Information
 
 #### Records
```

### Comparing `octodns-gcore-0.0.3/README.md` & `octodns-gcore-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-## EdgeCenter DNS & G-Core Labs DNS v2 API provider for octoDNS
+## Gcore DNS v2 API provider for octoDNS
 
-An [octoDNS](https://github.com/octodns/octodns/) provider that targets [EdgeCenter DNS](https://edgecenter.ru/dns/) and [G-Core Labs DNS](https://gcorelabs.com/dns/).
+An [octoDNS](https://github.com/octodns/octodns/) provider that targets [Gcore DNS](https://gcore.com/dns/).
 
 ### Installation
 
 #### Command line
 
 ```
 pip install octodns-gcore
@@ -28,46 +28,28 @@
 # Start with the latest/specific versions and don't just copy what's here
 -e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
 -e git+https://git@github.com/octodns/octodns-gcore.git@ec9661f8b335241ae4746eea467a8509205e6a30#egg=octodns_gcore
 ```
 
 ### Configuration
 
-
-#### EdgeCenterProvider
-
-```
-providers:
-  ec:
-    class: octodns_gcore.EdgeCenterProvider
-    # Your API key
-    token: env/EC_TOKEN
-    token_type: APIKey
-    # or login + password
-    #login: env/EC_LOGIN
-    #password: env/EC_PASSWORD
-    #auth_url: https://api.edgecenter.ru/id
-    #url: https://api.edgecenter.ru/dns/v2
-    #records_per_response: 1
-```
-
 #### GCoreProvider
 
 ```yaml
 providers:
   gcore:
     class: octodns_gcore.GCoreProvider
     # Your API key
     token: env/GCORE_TOKEN
     token_type: APIKey
     # or login + password
     #login: env/GCORE_LOGIN
     #password: env/GCORE_PASSWORD
-    #auth_url: https://api.gcorelabs.com/id
-    #url: https://api.gcorelabs.com/dns/v2
+    #auth_url: https://api.gcore.com/iam
+    #url: https://api.gcore.com/dns/v2
     #records_per_response: 1
 ```
 
 ### Support Information
 
 #### Records
```

### Comparing `octodns-gcore-0.0.3/octodns_gcore/__init__.py` & `octodns-gcore-0.0.4/octodns_gcore/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #
 #
 #
 
-from collections import defaultdict
-from requests import Session
 import http
 import logging
 import urllib.parse
+from collections import defaultdict
 
-from octodns.record import GeoCodes, Record
+from requests import Session
+
+from octodns import __VERSION__ as octodns_version
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
+from octodns.record import GeoCodes, Record
 
-__VERSION__ = '0.0.3'
+__VERSION__ = '0.0.4'
 
 
 class GCoreClientException(ProviderException):
     def __init__(self, r):
         super().__init__(r.text)
 
 
@@ -27,29 +29,33 @@
 
 class GCoreClientNotFound(GCoreClientException):
     def __init__(self, r):
         super().__init__(r)
 
 
 class GCoreClient(object):
-
     ROOT_ZONES = "zones"
 
     def __init__(
         self,
         log,
         api_url,
         auth_url,
         token=None,
         token_type=None,
         login=None,
         password=None,
     ):
         self.log = log
         self._session = Session()
+        self._session.headers.update(
+            {
+                'User-Agent': f'octodns/{octodns_version} octodns-gcore/{__VERSION__}'
+            }
+        )
         self._api_url = api_url
         if token is not None and token_type is not None:
             self._session.headers.update(
                 {"Authorization": f"{token_type} {token}"}
             )
         elif login is not None and password is not None:
             token = self._auth(auth_url, login, password)
@@ -103,24 +109,33 @@
             self._api_url, self.ROOT_ZONES, zone_name, "rrsets"
         )
         rrsets = self._request("GET", url, params={"all": "true"}).json()
         records = rrsets["rrsets"]
         return records
 
     def record_create(self, zone_name, rrset_name, type_, data):
+        # change ALIAS records to CNAME
+        if type_ == 'ALIAS':
+            type_ = 'CNAME'
         self._request(
             "POST", self._rrset_url(zone_name, rrset_name, type_), data=data
         )
 
     def record_update(self, zone_name, rrset_name, type_, data):
+        # change ALIAS records to CNAME
+        if type_ == 'ALIAS':
+            type_ = 'CNAME'
         self._request(
             "PUT", self._rrset_url(zone_name, rrset_name, type_), data=data
         )
 
     def record_delete(self, zone_name, rrset_name, type_):
+        # change ALIAS records to CNAME
+        if type_ == 'ALIAS':
+            type_ = 'CNAME'
         self._request("DELETE", self._rrset_url(zone_name, rrset_name, type_))
 
     def _rrset_url(self, zone_name, rrset_name, type_):
         return self._build_url(
             self._api_url, self.ROOT_ZONES, zone_name, rrset_name, type_
         )
 
@@ -131,15 +146,17 @@
             base = urllib.parse.urljoin(base, i)
         return base
 
 
 class _BaseProvider(BaseProvider):
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = True
-    SUPPORTS = set(("A", "AAAA", "NS", "MX", "TXT", "SRV", "CNAME", "PTR"))
+    SUPPORTS = set(
+        ("A", "AAAA", 'ALIAS', "NS", "MX", "TXT", "SRV", "CNAME", "PTR")
+    )
 
     def __init__(self, id, api_url, auth_url, *args, **kwargs):
         token = kwargs.pop("token", None)
         token_type = kwargs.pop("token_type", "APIKey")
         login = kwargs.pop("login", None)
         password = kwargs.pop("password", None)
         self.records_per_response = kwargs.pop("records_per_response", 1)
@@ -242,14 +259,15 @@
             "type": _type,
             "value": self._add_dot_if_need(
                 record["resource_records"][0]["content"][0]
             ),
         }
 
     _data_for_PTR = _data_for_single
+    _data_for_ALIAS = _data_for_single
 
     def _data_for_CNAME(self, _type, record):
         if record.get("filters") is None:
             return self._data_for_single(_type, record)
 
         pools, rules, defaults = self._data_for_dynamic(
             record, self._add_dot_if_need
@@ -349,20 +367,22 @@
             target,
             lenient,
         )
 
         values = defaultdict(defaultdict)
         records, exists = self.zone_records(zone)
         for record in records:
+            rr_name = zone.hostname_from_fqdn(record["name"])
             _type = record["type"].upper()
+            if _type == 'CNAME' and rr_name == '':
+                _type = 'ALIAS'
             if _type not in self.SUPPORTS:
                 continue
             if self._should_ignore(record):
                 continue
-            rr_name = zone.hostname_from_fqdn(record["name"])
             values[rr_name][_type] = record
 
         before = len(zone.records)
         for name, types in values.items():
             for _type, record in types.items():
                 data_for = getattr(self, f"_data_for_{_type}")
                 record = Record.new(
@@ -458,14 +478,15 @@
     def _params_for_single(self, record):
         return {
             "ttl": record.ttl,
             "resource_records": [{"content": [record.value]}],
         }
 
     _params_for_PTR = _params_for_single
+    _params_for_ALIAS = _params_for_single
 
     def _params_for_CNAME(self, record):
         if not record.dynamic:
             return self._params_for_single(record)
 
         return {
             "ttl": record.ttl,
@@ -576,22 +597,79 @@
             self._client.zone_create(zone)
             self.log.info("_apply: zone has been successfully created")
 
         for change in changes:
             class_name = change.__class__.__name__
             getattr(self, f"_apply_{class_name.lower()}")(change)
 
-
-class EdgeCenterProvider(_BaseProvider):
-    def __init__(self, id, *args, **kwargs):
-        self.log = logging.getLogger(f"EdgeCenterProvider[{id}]")
-        api_url = kwargs.pop("url", "https://api.edgecenter.ru/dns/v2")
-        auth_url = kwargs.pop("auth_url", "https://api.edgecenter.ru/id")
-        super().__init__(id, api_url, auth_url, *args, **kwargs)
+    def _process_desired_zone(self, desired):
+        for record in desired.records:
+            if getattr(record, "dynamic", False):
+                dynamic = record.dynamic
+                rules = []
+                for index, rule in enumerate(dynamic.rules):
+                    geos = rule.data.get("geos", [])
+                    if not geos:
+                        rules.append(rule)
+                        continue
+                    filtered_geos = [
+                        g
+                        for g in geos
+                        if not g.startswith('NA-US-')
+                        and not g.startswith("NA-CA-")
+                    ]
+                    if not filtered_geos:
+                        msg = f'NA-US- and NA-CA-* not supported for {record.fqdn}'
+                        fallback = f'skipping rule {index}'
+                        self.supports_warn_or_except(msg, fallback)
+                        continue
+                    elif geos != filtered_geos:
+                        msg = f'NA-US- and NA-CA-* not supported for {record.fqdn}'
+                        before = ', '.join(geos)
+                        after = ', '.join(filtered_geos)
+                        fallback = (
+                            f'filtering rule {index} from ({before}) to '
+                            f'({after})'
+                        )
+                        self.supports_warn_or_except(msg, fallback)
+                        rule.data['geos'] = filtered_geos
+                    rules.append(rule)
+
+                if rules != dynamic.rules:
+                    record = record.copy()
+                    record.dynamic.rules = rules
+                    desired.add_record(record, replace=True)
+            elif getattr(record, "geo", False):
+                geos = set(record.geo.keys())
+                filtered_geos = {
+                    g
+                    for g in geos
+                    if not g.startswith('NA-US-') and not g.startswith("NA-CA-")
+                }
+                if not filtered_geos:
+                    msg = f'NA-US- and NA-CA-* not supported for {record.fqdn}'
+                    fallback = 'skipping rule 0'
+                    self.supports_warn_or_except(msg, fallback)
+                elif geos != filtered_geos:
+                    msg = f'NA-US- and NA-CA-* not supported for {record.fqdn}'
+                    before = ', '.join(geos)
+                    after = ', '.join(filtered_geos)
+                    fallback = f'filtering rule 0 from ({before}) to ({after})'
+                    self.supports_warn_or_except(msg, fallback)
+                if geos != filtered_geos:
+                    record = record.copy()
+                    new_geo = {
+                        geo: value
+                        for geo, value in record.geo.items()
+                        if geo in filtered_geos
+                    }
+                    record.geo = new_geo
+                    desired.add_record(record, replace=True)
+        return super()._process_desired_zone(desired)
 
 
 class GCoreProvider(_BaseProvider):
     def __init__(self, id, *args, **kwargs):
         self.log = logging.getLogger(f"GCoreProvider[{id}]")
-        api_url = kwargs.pop("url", "https://api.gcorelabs.com/dns/v2")
-        auth_url = kwargs.pop("auth_url", "https://api.gcorelabs.com/id")
+        api_url = kwargs.pop("url", "https://api.gcore.com/dns/v2")
+        auth_url = kwargs.pop("auth_url", "https://api.gcore.com/id")
         super().__init__(id, api_url, auth_url, *args, **kwargs)
```

### Comparing `octodns-gcore-0.0.3/octodns_gcore.egg-info/PKG-INFO` & `octodns-gcore-0.0.4/octodns_gcore.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: octodns-gcore
-Version: 0.0.3
-Summary:  EdgeCenter DNS & G-Core Labs DNS v2 API provider for octoDNS
+Version: 0.0.4
+Summary:  Gcore DNS v2 API provider for octoDNS
 Home-page: https://github.com/octodns/octodns-gcore
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
-## EdgeCenter DNS & G-Core Labs DNS v2 API provider for octoDNS
+## Gcore DNS v2 API provider for octoDNS
 
-An [octoDNS](https://github.com/octodns/octodns/) provider that targets [EdgeCenter DNS](https://edgecenter.ru/dns/) and [G-Core Labs DNS](https://gcorelabs.com/dns/).
+An [octoDNS](https://github.com/octodns/octodns/) provider that targets [Gcore DNS](https://gcore.com/dns/).
 
 ### Installation
 
 #### Command line
 
 ```
 pip install octodns-gcore
@@ -41,46 +41,28 @@
 # Start with the latest/specific versions and don't just copy what's here
 -e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
 -e git+https://git@github.com/octodns/octodns-gcore.git@ec9661f8b335241ae4746eea467a8509205e6a30#egg=octodns_gcore
 ```
 
 ### Configuration
 
-
-#### EdgeCenterProvider
-
-```
-providers:
-  ec:
-    class: octodns_gcore.EdgeCenterProvider
-    # Your API key
-    token: env/EC_TOKEN
-    token_type: APIKey
-    # or login + password
-    #login: env/EC_LOGIN
-    #password: env/EC_PASSWORD
-    #auth_url: https://api.edgecenter.ru/id
-    #url: https://api.edgecenter.ru/dns/v2
-    #records_per_response: 1
-```
-
 #### GCoreProvider
 
 ```yaml
 providers:
   gcore:
     class: octodns_gcore.GCoreProvider
     # Your API key
     token: env/GCORE_TOKEN
     token_type: APIKey
     # or login + password
     #login: env/GCORE_LOGIN
     #password: env/GCORE_PASSWORD
-    #auth_url: https://api.gcorelabs.com/id
-    #url: https://api.gcorelabs.com/dns/v2
+    #auth_url: https://api.gcore.com/iam
+    #url: https://api.gcore.com/dns/v2
     #records_per_response: 1
 ```
 
 ### Support Information
 
 #### Records
```

### Comparing `octodns-gcore-0.0.3/setup.py` & `octodns-gcore-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from os import environ
-from setuptools import find_packages, setup
 from subprocess import CalledProcessError, check_output
 
+from setuptools import find_packages, setup
+
 
 def descriptions():
     with open('README.md') as fh:
         ret = fh.read()
         first = ret.split('\n', 1)[0].replace('#', '')
         return first, ret
 
@@ -39,14 +40,16 @@
     author_email='rwmcfa1@gmail.com',
     description=description,
     extras_require={
         'dev': tests_require
         + (
             'black>=22.3.0',
             'build>=0.7.0',
+            # >=5.12.0 does not support python 3.7, we still do
+            'isort==5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
     },
     install_requires=('octodns>=0.9.14', 'requests>=2.27.0'),
```

