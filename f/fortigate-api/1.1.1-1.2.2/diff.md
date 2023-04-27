# Comparing `tmp/fortigate_api-1.1.1.tar.gz` & `tmp/fortigate_api-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate_api-1.1.1.tar", last modified: Thu Mar 16 07:54:23 2023, max compression
+gzip compressed data, was "fortigate_api-1.2.2.tar", last modified: Thu Apr 27 05:53:27 2023, max compression
```

## Comparing `fortigate_api-1.1.1.tar` & `fortigate_api-1.2.2.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 07:54:23.490637 fortigate_api-1.1.1/
--rw-rw-rw-   0        0        0     1091 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    43014 2023-03-16 07:54:23.489637 fortigate_api-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    41750 2023-03-16 07:47:09.000000 fortigate_api-1.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-16 07:54:23.476638 fortigate_api-1.1.1/fortigate_api/
--rw-rw-rw-   0        0        0      181 2022-10-29 16:40:28.000000 fortigate_api-1.1.1/fortigate_api/__init__.py
--rw-rw-rw-   0        0        0      221 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/address.py
--rw-rw-rw-   0        0        0      236 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/address_group.py
--rw-rw-rw-   0        0        0      228 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/antivirus.py
--rw-rw-rw-   0        0        0      233 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/application.py
--rw-rw-rw-   0        0        0     7139 2022-10-29 08:32:02.000000 fortigate_api-1.1.1/fortigate_api/base.py
--rw-rw-rw-   0        0        0     9769 2023-03-05 18:01:17.000000 fortigate_api-1.1.1/fortigate_api/ccp.py
--rw-rw-rw-   0        0        0     1472 2022-08-31 22:28:52.000000 fortigate_api-1.1.1/fortigate_api/dhcp_server.py
--rw-rw-rw-   0        0        0     4029 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/dict_.py
--rw-rw-rw-   0        0        0     7481 2022-10-29 12:09:25.000000 fortigate_api-1.1.1/fortigate_api/extended_filters.py
--rw-rw-rw-   0        0        0    13063 2023-02-08 08:21:50.000000 fortigate_api-1.1.1/fortigate_api/fortigate.py
--rw-rw-rw-   0        0        0     3798 2023-03-16 07:50:24.000000 fortigate_api-1.1.1/fortigate_api/fortigate_api.py
--rw-rw-rw-   0        0        0      609 2022-10-29 14:30:46.000000 fortigate_api-1.1.1/fortigate_api/helpers.py
--rw-rw-rw-   0        0        0     1155 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/interface.py
--rw-rw-rw-   0        0        0      254 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/internet_service.py
--rw-rw-rw-   0        0        0      217 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/ip_pool.py
--rw-rw-rw-   0        0        0     2617 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/policy.py
--rw-rw-rw-   0        0        0        0 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/py.typed
--rw-rw-rw-   0        0        0      233 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/schedule.py
--rw-rw-rw-   0        0        0      228 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/service.py
--rw-rw-rw-   0        0        0      254 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/service_category.py
--rw-rw-rw-   0        0        0      242 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/service_group.py
--rw-rw-rw-   0        0        0     1021 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/snmp_community.py
--rw-rw-rw-   0        0        0     3050 2022-10-29 14:30:46.000000 fortigate_api-1.1.1/fortigate_api/ssh.py
--rw-rw-rw-   0        0        0     1934 2022-10-29 18:43:34.000000 fortigate_api-1.1.1/fortigate_api/str_.py
--rw-rw-rw-   0        0        0      580 2022-10-29 09:24:35.000000 fortigate_api-1.1.1/fortigate_api/types_.py
--rw-rw-rw-   0        0        0      223 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/virtual_ip.py
--rw-rw-rw-   0        0        0      207 2022-07-14 18:32:10.000000 fortigate_api-1.1.1/fortigate_api/zone.py
-drwxrwxrwx   0        0        0        0 2023-03-16 07:54:23.486641 fortigate_api-1.1.1/fortigate_api.egg-info/
--rw-rw-rw-   0        0        0    43014 2023-03-16 07:54:23.000000 fortigate_api-1.1.1/fortigate_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      978 2023-03-16 07:54:23.000000 fortigate_api-1.1.1/fortigate_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 07:54:23.000000 fortigate_api-1.1.1/fortigate_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-03-16 07:54:23.000000 fortigate_api-1.1.1/fortigate_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-16 07:54:23.000000 fortigate_api-1.1.1/fortigate_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1670 2023-03-16 07:47:09.000000 fortigate_api-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-16 07:54:23.491637 fortigate_api-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      112 2022-10-29 16:50:15.000000 fortigate_api-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:53:27.846122 fortigate_api-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2022-07-14 18:32:10.000000 fortigate_api-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    44303 2023-04-27 05:53:27.845122 fortigate_api-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    43039 2023-04-27 05:36:12.000000 fortigate_api-1.2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 05:53:27.837119 fortigate_api-1.2.2/fortigate_api/
+-rw-rw-rw-   0        0        0      182 2023-04-22 19:54:39.000000 fortigate_api-1.2.2/fortigate_api/__init__.py
+-rw-rw-rw-   0        0        0      371 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/address.py
+-rw-rw-rw-   0        0        0      394 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/address_group.py
+-rw-rw-rw-   0        0        0      380 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/antivirus.py
+-rw-rw-rw-   0        0        0      387 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/application.py
+-rw-rw-rw-   0        0        0     8427 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/base.py
+-rw-rw-rw-   0        0        0     9884 2023-04-22 19:54:39.000000 fortigate_api-1.2.2/fortigate_api/ccp.py
+-rw-rw-rw-   0        0        0     1851 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/dhcp_server.py
+-rw-rw-rw-   0        0        0     7997 2023-04-27 05:52:33.000000 fortigate_api-1.2.2/fortigate_api/extended_filters.py
+-rw-rw-rw-   0        0        0      418 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/external_resource.py
+-rw-rw-rw-   0        0        0    15110 2023-04-25 09:56:56.000000 fortigate_api-1.2.2/fortigate_api/fortigate.py
+-rw-rw-rw-   0        0        0     4494 2023-04-24 14:18:26.000000 fortigate_api-1.2.2/fortigate_api/fortigate_api.py
+-rw-rw-rw-   0        0        0     9009 2023-04-22 19:54:39.000000 fortigate_api-1.2.2/fortigate_api/helpers.py
+-rw-rw-rw-   0        0        0     1456 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/interface.py
+-rw-rw-rw-   0        0        0      415 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/internet_service.py
+-rw-rw-rw-   0        0        0      369 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/ip_pool.py
+-rw-rw-rw-   0        0        0     3266 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/policy.py
+-rw-rw-rw-   0        0        0        0 2022-07-14 18:32:10.000000 fortigate_api-1.2.2/fortigate_api/py.typed
+-rw-rw-rw-   0        0        0      384 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/schedule.py
+-rw-rw-rw-   0        0        0      378 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/service.py
+-rw-rw-rw-   0        0        0      415 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/service_category.py
+-rw-rw-rw-   0        0        0      400 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/service_group.py
+-rw-rw-rw-   0        0        0     1315 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/snmp_community.py
+-rw-rw-rw-   0        0        0     3347 2023-04-22 19:54:39.000000 fortigate_api-1.2.2/fortigate_api/ssh.py
+-rw-rw-rw-   0        0        0      731 2023-04-22 19:54:39.000000 fortigate_api-1.2.2/fortigate_api/types_.py
+-rw-rw-rw-   0        0        0      378 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/virtual_ip.py
+-rw-rw-rw-   0        0        0      354 2023-04-24 14:23:05.000000 fortigate_api-1.2.2/fortigate_api/zone.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:53:27.843119 fortigate_api-1.2.2/fortigate_api.egg-info/
+-rw-rw-rw-   0        0        0    44303 2023-04-27 05:53:27.000000 fortigate_api-1.2.2/fortigate_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      968 2023-04-27 05:53:27.000000 fortigate_api-1.2.2/fortigate_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:53:27.000000 fortigate_api-1.2.2/fortigate_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-04-27 05:53:27.000000 fortigate_api-1.2.2/fortigate_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-27 05:53:27.000000 fortigate_api-1.2.2/fortigate_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1771 2023-04-27 05:48:44.000000 fortigate_api-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:53:27.847118 fortigate_api-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      113 2023-04-22 19:54:40.000000 fortigate_api-1.2.2/setup.py
```

### Comparing `fortigate_api-1.1.1/LICENSE.txt` & `fortigate_api-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.1.1/PKG-INFO` & `fortigate_api-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fortigate_api
-Version: 1.1.1
+Version: 1.2.2
 Summary: Python package to configure Fortigate (Fortios) devices using REST API and SSH
 Author-email: Vladimir Prusakov <vladimir.prusakovs@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Repository, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/fortigate-api/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.1.1.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 Keywords: fortigate,api,fortios,firewall,networking,telecommunication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: License :: OSI Approved :: MIT License
@@ -28,28 +28,29 @@
 .. image:: https://img.shields.io/pypi/v/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/pypi/pyversions/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/github/last-commit/vladimirs-git/fortigate-api
    :target: https://pypi.python.org/pypi/fortigate-api
 
+
 fortigate-api
 =============
 
 Python package to configure Fortigate (Fortios) devices using REST API and SSH.
 With this package, you can change objects in the Fortigate. The most commonly used `Objects`_
 are implemented in the `FortigateAPI`_ methods, but you can manipulate any other objects
 that can be accessed through the REST API using the `Fortigate`_ methods.
 You can also get and change the Fortigate configuration through SSH.
 
 Main features:
 
-- REST API to create, delete, get, update objects. Move policy before, after other policy.
-- SSH Netmiko connector to work with CLI commands.
-- CiscoConfParse to search and modify commands in config.
+- REST API to create, delete, get, update objects. Move policy before, after other policy
+- Session-based (user, password) and Token-based authentication
+- SSH Netmiko connector to work with CLI commands
 - Usage examples in `./examples`_
 
 ----------------------------------------------------------------------------------------------------
 
 .. contents:: **Contents**
     :local:
 
@@ -70,15 +71,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.1.1.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
 
@@ -89,138 +90,168 @@
 -------
 The objects implemented in `FortigateAPI`_.
 To get an idea of the objects, you can change the *hostname* in the following URLs and
 look it in the Fortigate web management interface. The first URL is for the Web GUI, the second
 one is for the REST API. Not all object implemented in `FortigateAPI`_ (only the most used by me),
 access to any other objects is available via `Fortigate`_.
 
-=================== ================================================================================
-Object              GUI and REST API URL to the object, FortiOS v6.4
-=================== ================================================================================
-`Address`_          https://hostname/ng/firewall/address
+===================== ==============================================================================
+Object                GUI and REST API URL to the object (FortiOS v6.4)
+===================== ==============================================================================
+`Address`_            https://hostname/ng/firewall/address
+
+                      https://hostname/api/v2/cmdb/firewall/address/
 
-                    https://hostname/api/v2/cmdb/firewall/address/
+`AddressGroup`_       https://hostname/ng/firewall/address
 
-`AddressGroup`_     https://hostname/ng/firewall/address
+                      https://hostname/api/v2/cmdb/firewall/addrgrp/
 
-                    https://hostname/api/v2/cmdb/firewall/addrgrp/
+`Antivirus`_          https://hostname/ng/utm/antivirus/profile
 
-`Antivirus`_        https://hostname/ng/utm/antivirus/profile
+                      https://hostname/api/v2/cmdb/antivirus/profile/
 
-                    https://hostname/api/v2/cmdb/antivirus/profile/
+`Application`_        https://hostname/ng/utm/appctrl/sensor
 
-`Application`_      https://hostname/ng/utm/appctrl/sensor
+                      https://hostname/api/v2/cmdb/application/list/
 
-                    https://hostname/api/v2/cmdb/application/list/
+`DhcpServer`_         https://hostname/ng/interface/edit/{name}
 
-`DhcpServer`_       https://hostname/ng/interface/edit/{name}
+                      https://hostname/api/v2/cmdb/system.dhcp/server/
 
-                    https://hostname/api/v2/cmdb/system.dhcp/server/
+`ExternalResource`_   https://hostname/ng/external-connector
 
-`Interface`_        https://hostname/ng/interface
+                      https://hostname/api/v2/cmdb/system/external-resource/
 
-                    https://hostname/api/v2/cmdb/system/interface/
+`Interface`_          https://hostname/ng/interface
 
-`InternetService`_  https://hostname/ng/firewall/internet_service
+                      https://hostname/api/v2/cmdb/system/interface/
 
-                    https://hostname/api/v2/cmdb/firewall/internet-service/
+`InternetService`_    https://hostname/ng/firewall/internet_service
 
-`IpPool`_           https://hostname/ng/firewall/ip-pool
+                      https://hostname/api/v2/cmdb/firewall/internet-service/
 
-                    https://hostname/api/v2/cmdb/firewall/ippool/
+`IpPool`_             https://hostname/ng/firewall/ip-pool
 
-`Policy`_           https://hostname/ng/firewall/policy/policy/standard
+                      https://hostname/api/v2/cmdb/firewall/ippool/
 
-                    https://hostname/api/v2/cmdb/firewall/policy/
+`Policy`_             https://hostname/ng/firewall/policy/policy/standard
 
-`Schedule`_         https://hostname/ng/firewall/schedule
+                      https://hostname/api/v2/cmdb/firewall/policy/
 
-                    https://hostname/api/v2/cmdb/firewall.schedule/onetime/
+`Schedule`_           https://hostname/ng/firewall/schedule
 
-`Service`_          https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.schedule/onetime/
 
-                    https://hostname/api/v2/cmdb/firewall.service/custom/
+`Service`_            https://hostname/ng/firewall/service
 
-`ServiceCategory`_  https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.service/custom/
 
-                    https://hostname/api/v2/cmdb/firewall.service/category/
+`ServiceCategory`_    https://hostname/ng/firewall/service
 
-`ServiceGroup`_     https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.service/category/
 
-                    https://hostname/api/v2/cmdb/firewall.service/group/
+`ServiceGroup`_       https://hostname/ng/firewall/service
 
-`SnmpCommunity`_    https://hostname/ng/system/snmp
+                      https://hostname/api/v2/cmdb/firewall.service/group/
 
-                    https://hostname/api/v2/cmdb/system.snmp/community/
+`SnmpCommunity`_      https://hostname/ng/system/snmp
 
-`VirtualIp`_        https://hostname/ng/firewall/virtual-ip
+                      https://hostname/api/v2/cmdb/system.snmp/community/
 
-                    https://hostname/api/v2/cmdb/firewall/vip/
+`VirtualIp`_          https://hostname/ng/firewall/virtual-ip
 
-`Zone`_             https://hostname/ng/interface
+                      https://hostname/api/v2/cmdb/firewall/vip/
 
-                    https://hostname/api/v2/cmdb/system/zone/
-=================== ================================================================================
+`Zone`_               https://hostname/ng/interface
+
+                      https://hostname/api/v2/cmdb/system/zone/
+===================== ==============================================================================
 
 
 ----------------------------------------------------------------------------------------------------
 
 FortigateAPI
 ------------
 **FortigateAPI(host, username, password, scheme, port, timeout, vdom)**
 Set of methods for working with the most commonly used `Objects`_.
-Code usage examples in *./examples/examples.py*
 
 =============== ======= ============================================================================
 Parameter        Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
-username        *str*   Administrator name
-password        *str*   Administrator password
+username        *str*   Administrator name. Mutually exclusive with token
+password        *str*   Administrator password. Mutually exclusive with token
+token           *str*   Administrator token. Mutually exclusive with username and password
 scheme          *str*   (optional) "https" (default) or "http"
 port            *int*   (optional) TCP port, by default 443 for "https", 80 for "http"
 timeout         *int*   (optional) Session timeout minutes (default 15)
 verify          *str*   (optional) Enable SSL certificate verification for HTTPS requests. True -  enable, False - disable (default)
 vdom            *str*   Name of virtual domain (default "root")
 =============== ======= ============================================================================
 
 
 ----------------------------------------------------------------------------------------------------
 
 Address
 -------
+Python examples `./examples/address.py`_
+
+Python examples `./examples/address_token.py`_
+
 FortiOS v6.4 data example `./examples/yml/address.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create address
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.252",
+            "type": "ipmask"}
+    response = fgt.address.create(data)
+
+    # Get all addresses
+    addresses_all = fgt.address.get()
+
+    # Get address by name
+    addresses_by_name = fgt.address.get(uid="ADDRESS")
+
+    # Get address by operator contains \"=@\"
+    addresses_contains = fgt.address.get(filter="subnet=@127.0")
+
 
 create()
 ........
 **FortigateAPI.address.create(data)**
-Creates address-object in the Fortigate.
+Create address-object in the Fortigate.
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the address-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
 **FortigateAPI.address.delete(uid, filter)**
-Deletes address-object from the Fortigate.
+Delete address-object from the Fortigate.
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*               Unique identifier. Name of the address-object. Used to delete a single object
-filter          *str*, *List[str]*  Filters address-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters address-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -266,68 +297,70 @@
 uid             *str*   Name of the address-object, taken from the `uid` parameter or from data["name"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
+----------------------------------------------------------------------------------------------------
 
-Address examples:
+AddressGroup
+------------
+Python examples `./examples/address_group.py`_
 
-- Creates address in the Fortigate
-- Gets all addresses from the Fortigate
-- Gets filtered address by name (unique identifier)
-- Filters address by operator *equals* "=="
-- Filters address by operator *contains* "=@"
-- Filters address by operator *not equals* "!="
-- Updates address data in the Fortigate
-- Checks for presence of address in the Fortigate
-- Deletes address from the Fortigate by name
-- Deletes addresses from the Fortigate by filter
-- Checks for absence of address in the Fortigate
-- FortigateAPI *with* statement
+FortiOS v6.4 data example `./examples/yml/address_group.yml`_
 
-`./examples/address.py`_
+.. code:: python
 
+    from fortigate_api import FortigateAPI
 
-----------------------------------------------------------------------------------------------------
+    fgt = FortigateAPI(host="host", username="username", password="password")
 
-AddressGroup
-------------
-FortiOS v6.4 data example `./examples/yml/address_group.yml`_
+    # Create address and address-group in the Fortigate
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.255",
+            "type": "ipmask"}
+    fgt.address.create(data)
+    data = {"name": "ADDR_GROUP", "member": [{"name": "ADDRESS"}]}
+    fgt.address_group.create(data)
+
+    # Get all address-groups from the Fortigate
+    address_groups_all = fgt.address_group.get()
+
+    # Get filtered address_group by name (unique identifier)
+    address_groups_name = fgt.address_group.get(uid="ADDR_GROUP")
 
 
 create()
 ........
 **FortigateAPI.address_group.create(data)**
-Creates address-group-object in the Fortigate
+Create address-group-object in the Fortigate
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the address-group-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
 **FortigateAPI.address_group.delete(uid, filter)**
-Deletes address-group-object from the Fortigate
+Delete address-group-object from the Fortigate
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*               Name of the address-group-object (unique identifier). Used to delete a single object
-filter          *str*, *List[str]*  Filters address-group-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters address-group-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -373,33 +406,14 @@
 uid             *str*   Name of the address-group-object, taken from the `uid` parameter or from data["name"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-AddressGroup examples:
-
-- Creates address-group in the Fortigate
-- Gets all address-groups from the Fortigate
-- Gets filtered address-group by name (unique identifier)
-- Filters address-group by operator *equals* "=="
-- Filters address-group by operator *contains* "=@"
-- Filters address-group by operator *not equals* "!="
-- Updates address-group data in the Fortigate
-- Checks for presence of address-group in the Fortigate
-- Deletes address-group from the Fortigate by name
-- Deletes address-groups from the Fortigate by filter
-- Checks for absence of address-group in the Fortigate
-
-`./examples/address_group.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Antivirus
 ---------
 **Antivirus** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/antivirus.yml`_
@@ -436,37 +450,95 @@
 
 ----------------------------------------------------------------------------------------------------
 
 DhcpServer
 ----------
 **DhcpServer** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/dhcp_server.py`_
+
 FortiOS v6.4 data example `./examples/yml/dhcp_server.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create dhcp server
+    data = {
+        "default-gateway": "192.168.255.1",
+        "netmask": "255.255.255.0",
+        "interface": "vlan.123",
+        "ip-range": [{"start-ip": "192.168.255.2", "end-ip": "192.168.255.254", }],
+    }
+    fgt.dhcp_server.create(data)
+
+    # Get all dhcp servers
+    dhcp_servers = fgt.dhcp_server.get()
+
+
 **FortigateAPI.dhcp_server.create(data)** Note, in Fortigate is possible to create multiple DHCP servers with the same settings, you need control duplicates
 
 **FortigateAPI.dhcp_server.delete(uid, filter)**
 
 **FortigateAPI.dhcp_server.get(uid, filter)**
 
 **FortigateAPI.dhcp_server.is_exist(uid)**
 
 **FortigateAPI.dhcp_server.update(data, uid)**
 
-DhcpServer examples `./examples/dhcp_server.py`_
+
+----------------------------------------------------------------------------------------------------
+
+ExternalResource
+----------------
+**ExternalResource** object has the same parameters and methods as `Address`_
+
+Python examples `./examples/external_resource.py`_
+
+FortiOS v6.4 data example `./examples/yml/external_resource.yml`_
+
+**FortigateAPI.external_resource.create(data)**
+
+**FortigateAPI.external_resource.delete(uid, filter)**
+
+**FortigateAPI.external_resource.get(uid, filter)**
+
+**FortigateAPI.external_resource.is_exist(uid)**
+
+**FortigateAPI.external_resource.update(data, uid)**
+
 
 
 ----------------------------------------------------------------------------------------------------
 
 Interface
 ---------
 **Interface** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/interface.py`_
+
 FortiOS v6.4 data example `./examples/yml/interface.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+
+    # Get all interfaces in vdom \"root\" from the Fortigate
+    interfaces = fgt.interface.get()
+    print(f"interfaces count={len(interfaces)}")  # interfaces count=21
+
+    # Gets filtered interface by name (unique identifier)
+    interfaces = fgt.interface.get(uid="dmz")
+
+
 **FortigateAPI.interface.create(data)**
 
 **FortigateAPI.interface.delete(uid, filter)**
 
 
 get()
 .....
@@ -485,31 +557,14 @@
     *List[dict]* List of interface-objects
 
 **FortigateAPI.interface.is_exist(uid)**
 
 **FortigateAPI.interface.update(data, uid)**
 
 
-Examples
-........
-Interface examples:
-
-- Gets all interfaces in vdom "root" from the Fortigate
-- Gets filtered interface by name (unique identifier)
-- Filters interface by operator *equals* "=="
-- Filters interface by operator contains "=@"
-- Filters interface by operator *not equals* "!="
-- Filters interface by multiple conditions
-- Updates interface data in the Fortigate
-- Checks for presence of interface in the Fortigate
-- Gets all interfaces in vdom "VDOM"
-
-`./examples/interface.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 InternetService
 ---------------
 **InternetService** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/internet_service.yml`_
@@ -527,66 +582,91 @@
 
 ----------------------------------------------------------------------------------------------------
 
 IpPool
 ------
 **IpPool** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/ip_pool.py`_
+
 FortiOS v6.4 data example `./examples/yml/ip_pool.yml`_
 
 **FortigateAPI.ip_pool.create(data)**
 
 **FortigateAPI.ip_pool.delete(uid, filter)**
 
 **FortigateAPI.ip_pool.get(uid, filter)**
 
 **FortigateAPI.ip_pool.is_exist(uid)**
 
 **FortigateAPI.ip_pool.update(data, uid)**
 
 
-Examples
-........
-IpPool examples:
-
-`./examples/ip_pool.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Policy
 ------
+Python examples `./examples/policy.py`_
+
+Python examples `./examples/policy_extended_filter.py`_
+
 FortiOS v6.4 data example `./examples/yml/policy.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create policy in the Fortigate
+    data = dict(
+        name="POLICY",
+        status="enable",
+        action="accept",
+        srcintf=[{"name": "any"}],
+        dstintf=[{"name": "any"}],
+        srcaddr=[{"name": "all"}],
+        dstaddr=[{"name": "all"}],
+        service=[{"name": "ALL"}],
+        schedule="always",
+    )
+    fgt.policy.create(data)
+
+    # Get all policies from the Fortigate
+    policies_all = fgt.policy.get()
+
+    # Filters policies by name, by operator equals
+    policies_name = fgt.policy.get(filter="name==POLICY")
+
 
 create()
 ........
 **FortigateAPI.policy.create(data)**
-Creates policy-object in the Fortigate
+Create policy-object in the Fortigate
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the policy-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
-Deletes policy-object from the Fortigate
+Delete policy-object from the Fortigate
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*, *int*        Identifier of the policy-object. Used to delete a single object
-filter          *str*, *List[str]*  Filters policy-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters policy-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -649,46 +729,14 @@
 uid             *int*   Policyid of the policy-object, taken from the `uid` parameter or from data["policyid"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-Policy examples:
-
-- Creates policy in the Fortigate
-- Gets all policies from the Fortigate
-- Gets filtered policy by policyid (unique identifier)
-- Filters policies by name, by operator *equals* "=="
-- Filters policies by operator *contains* "=@"
-- Filters policies by operator *not equals* "!="
-- Updates policy data in the Fortigate
-- Checks for presence of policy in the Fortigate
-- Gets all policies with destination address == "192.168.1.2/32"
-- Deletes policy from the Fortigate by policyid (unique identifier)
-- Deletes policies from the Fortigate by filter (by name)
-- Checks for absence of policy in the Fortigate
-
-`./examples/policy.py`_
-
-
-Policy Extended Filter examples:
-
-- Gets the rules where source prefix is equals 127.0.1.0/30
-- Gets the rules where source prefix is not equals 127.0.1.0/30
-- Gets the rules where source addresses are in subnets of 127.0.1.0/24
-- Gets the rules where source prefixes are supernets of address 127.0.1.1/32
-- Gets the rules where source prefix are equals 127.0.1.0/30 and destination prefix are equals 127.0.2.0/30
-- Delete policy, address-group, addresses from the Fortigate (order is important)
-
-`./examples/policy_extended_filter.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Schedule
 --------
 **Schedule** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/schedule.yml`_
@@ -763,14 +811,16 @@
 
 ----------------------------------------------------------------------------------------------------
 
 SnmpCommunity
 -------------
 **SnmpCommunity**
 
+Python examples `./examples/snmp_community.py`_
+
 FortiOS v6.4 data example `./examples/yml/snmp_community.yml`_
 
 **FortigateAPI.snmp_community.create(data)**
 
 **FortigateAPI.snmp_community.delete(uid, filter)**
 
 **FortigateAPI.snmp_community.get(uid, filter)**
@@ -787,19 +837,14 @@
 uid             *str*   Name of the snmp-community-object, taken from the `uid` parameter or from data["id"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-SnmpCommunity examples `./examples/snmp_community.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 VirtualIP
 ---------
 **VirtualIP** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/virtual_ip.yml`_
@@ -839,20 +884,42 @@
 Fortigate
 ---------
 **Fortigate(host, username, password, scheme, port, timeout, vdom)**
 REST API connector to the Fortigate. Contains generic methods (get, put, delete, etc.)
 to work with any objects available through the REST API. `Fortigate`_ is useful for working with
 objects that are not implemented in `FortigateAPI`_
 
+Python examples `./examples/fortigate.py`_
+
+Python examples `./examples/fortigate_token.py`_
+
+.. code:: python
+
+    from fortigate_api import Fortigate
+
+    fgt = Fortigate(host="host", username="username", password="password")
+
+    # Create address in the Fortigate
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.252",
+            "type": "ipmask"}
+    fgt.post(url="api/v2/cmdb/firewall/address/", data=data)
+
+    # Get address data from the Fortigate
+    addresses_all = fgt.get(url="api/v2/cmdb/firewall/address/")
+
+
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
-username        *str*   Administrator name
-password        *str*   Administrator password
+username        *str*   Administrator name. Mutually exclusive with token
+password        *str*   Administrator password. Mutually exclusive with token
+token           *str*   Administrator token. Mutually exclusive with username and password
 scheme          *str*   (optional) "https" (default) or "http"
 port            *int*   (optional) TCP port, by default 443 for "https", 80 for "http"
 timeout         *int*   (optional) Session timeout minutes (default 15)
 verify          *str*   (optional) Enable SSL certificate verification for HTTPS requests. True -  enable, False - disable (default)
 vdom            *str*   Name of virtual domain (default "root")
 =============== ======= ============================================================================
 
@@ -935,38 +1002,45 @@
 data            *dict*  Data of the object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-Fortigate examples:
-
-- Creates address in the Fortigate
-- Gets address data from the Fortigate
-- Updates address data in the Fortigate
-- Checks for presence of address in the Fortigate
-- Deletes address from the Fortigate
-- Checks for absence of address in the Fortigate
-- Fortigate *with* statement
-
-`./examples/fortigate.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 SSH
 ---
 **SSH(host, username, password, ssh)**
 SSH connector to the Fortigate. Contains methods to get and put configuration commands using ssh.
 Note, FortigateAPI parameter "vdom" used in REST API only and not used in SSH.
 In order to send cli commands to a specific vdom, you need "config vdom" before.
 
+Python examples `./examples/ssh.py`_
+
+Python examples `./examples/ssh_vdom.py`_
+
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt_api = FortigateAPI(host="host", username="username", password="password")
+    fgt_api.ssh.login()
+
+    # Show interface config
+    config = fgt_api.ssh.send_command("show system interface dmz")
+
+    # Change interface description from "dmz" to "DMZ"
+    cmds = ["config system interface",
+            "edit dmz",
+            "set description DMZ",
+            "end"]
+    output = fgt_api.ssh.send_config_set(cmds)
+
+
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
 username        *str*   Administrator name
 password        *str*   Administrator password
 ssh             *dict*  Netmiko *ConnectHandler* parameters
@@ -1008,79 +1082,44 @@
 cmds            *List[str]*   Configuration commands to be executed on the Fortigate
 kwargs          *dict*        (optional) Netmiko parameters
 =============== ============= ======================================================================
 
 Return
     Output of the commands
 
-
-Examples
-........
-SSH examples:
-
-- Show interface config
-- Change interface description from "dmz" to "DMZ"
-- Check interface description is changed
-- Change read-timeout timer for long awaited commands
-
-`./examples/ssh.py`_
-
-SSH examples for working with vdom:
-
-- get system arp from interfaces associated with vdom="VDOM"
-- get system arp from interfaces associated with vdom="root"
-
-`./examples/ssh_vdom.py`_
-
 ----------------------------------------------------------------------------------------------------
 
-CiscoConfParse
---------------
-Helper that parses the Fortigate configuration to find and modify command lines.
-CiscoConfParse doesn't natively support Fortigate configuration,
-but after some tweaking in this package it has become a good tool to play with Fortigate config lines.
-For more information, see the documentation for the JunosCfgLine object at https://github.com/mpenning/ciscoconfparse
-
-
-Examples
-........
-CiscoConfParse examples:
-
-- get config from the Fortigate by SSH
-- create CiscoConfParse object
-- filter all JunosCfgLine objects of wan interfaces
-- print some data in CiscoConfParse objects
-- filter all wan interfaces blocks
-
-`./examples/ccp.py`_
-
 
 .. _`./examples`: ./examples
+.. _`./examples/yml`: ./examples/yml
 .. _`./examples/yml/address.yml`: ./examples/yml/address.yml
 .. _`./examples/yml/address_group.yml`: ./examples/yml/address_group.yml
 .. _`./examples/yml/antivirus.yml`: ./examples/yml/antivirus.yml
 .. _`./examples/yml/application.yml`: ./examples/yml/application.yml
 .. _`./examples/yml/dhcp_server.yml`: ./examples/yml/dhcp_server.yml
+.. _`./examples/yml/external_resource.yml`: ./examples/yml/external_resource.yml
 .. _`./examples/yml/interface.yml`: ./examples/yml/interface.yml
 .. _`./examples/yml/internet_service.yml`: ./examples/yml/internet_service.yml
 .. _`./examples/yml/ip_pool.yml`: ./examples/yml/ip_pool.yml
 .. _`./examples/yml/policy.yml`: ./examples/yml/policy.yml
 .. _`./examples/yml/schedule.yml`: ./examples/yml/schedule.yml
 .. _`./examples/yml/service.yml`: ./examples/yml/service.yml
 .. _`./examples/yml/service_category.yml`: ./examples/yml/service_category.yml
 .. _`./examples/yml/service_group.yml`: ./examples/yml/service_group.yml
 .. _`./examples/yml/snmp_community.yml`: ./examples/yml/snmp_community.yml
 .. _`./examples/yml/virtual_ip.yml`: ./examples/yml/virtual_ip.yml
 .. _`./examples/yml/zone.yml`: ./examples/yml/zone.yml
 
 .. _`./examples/address.py`: ./examples/address.py
+.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/address_group.py`: ./examples/address_group.py
-.. _`./examples/ccp.py`: ./examples/ccp.py
 .. _`./examples/dhcp_server.py`: ./examples/dhcp_server.py
+.. _`./examples/external_resource.py`: ./examples/external_resource.py
 .. _`./examples/fortigate.py`: ./examples/fortigate.py
+.. _`./examples/fortigate_token.py`: ./examples/fortigate_token.py
 .. _`./examples/interface.py`: ./examples/interface.py
 .. _`./examples/ip_pool.py`: ./examples/ip_pool.py
 .. _`./examples/policy.py`: ./examples/policy.py
 .. _`./examples/policy_extended_filter.py`: ./examples/policy_extended_filter.py
 .. _`./examples/snmp_community.py`: ./examples/snmp_community.py
 .. _`./examples/ssh.py`: ./examples/ssh.py
 .. _`./examples/ssh_vdom.py`: ./examples/ssh_vdom.py
```

### Comparing `fortigate_api-1.1.1/README.rst` & `fortigate_api-1.2.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 .. image:: https://img.shields.io/pypi/v/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/pypi/pyversions/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/github/last-commit/vladimirs-git/fortigate-api
    :target: https://pypi.python.org/pypi/fortigate-api
 
+
 fortigate-api
 =============
 
 Python package to configure Fortigate (Fortios) devices using REST API and SSH.
 With this package, you can change objects in the Fortigate. The most commonly used `Objects`_
 are implemented in the `FortigateAPI`_ methods, but you can manipulate any other objects
 that can be accessed through the REST API using the `Fortigate`_ methods.
 You can also get and change the Fortigate configuration through SSH.
 
 Main features:
 
-- REST API to create, delete, get, update objects. Move policy before, after other policy.
-- SSH Netmiko connector to work with CLI commands.
-- CiscoConfParse to search and modify commands in config.
+- REST API to create, delete, get, update objects. Move policy before, after other policy
+- Session-based (user, password) and Token-based authentication
+- SSH Netmiko connector to work with CLI commands
 - Usage examples in `./examples`_
 
 ----------------------------------------------------------------------------------------------------
 
 .. contents:: **Contents**
     :local:
 
@@ -44,15 +45,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.1.1.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
 
@@ -63,138 +64,168 @@
 -------
 The objects implemented in `FortigateAPI`_.
 To get an idea of the objects, you can change the *hostname* in the following URLs and
 look it in the Fortigate web management interface. The first URL is for the Web GUI, the second
 one is for the REST API. Not all object implemented in `FortigateAPI`_ (only the most used by me),
 access to any other objects is available via `Fortigate`_.
 
-=================== ================================================================================
-Object              GUI and REST API URL to the object, FortiOS v6.4
-=================== ================================================================================
-`Address`_          https://hostname/ng/firewall/address
+===================== ==============================================================================
+Object                GUI and REST API URL to the object (FortiOS v6.4)
+===================== ==============================================================================
+`Address`_            https://hostname/ng/firewall/address
+
+                      https://hostname/api/v2/cmdb/firewall/address/
 
-                    https://hostname/api/v2/cmdb/firewall/address/
+`AddressGroup`_       https://hostname/ng/firewall/address
 
-`AddressGroup`_     https://hostname/ng/firewall/address
+                      https://hostname/api/v2/cmdb/firewall/addrgrp/
 
-                    https://hostname/api/v2/cmdb/firewall/addrgrp/
+`Antivirus`_          https://hostname/ng/utm/antivirus/profile
 
-`Antivirus`_        https://hostname/ng/utm/antivirus/profile
+                      https://hostname/api/v2/cmdb/antivirus/profile/
 
-                    https://hostname/api/v2/cmdb/antivirus/profile/
+`Application`_        https://hostname/ng/utm/appctrl/sensor
 
-`Application`_      https://hostname/ng/utm/appctrl/sensor
+                      https://hostname/api/v2/cmdb/application/list/
 
-                    https://hostname/api/v2/cmdb/application/list/
+`DhcpServer`_         https://hostname/ng/interface/edit/{name}
 
-`DhcpServer`_       https://hostname/ng/interface/edit/{name}
+                      https://hostname/api/v2/cmdb/system.dhcp/server/
 
-                    https://hostname/api/v2/cmdb/system.dhcp/server/
+`ExternalResource`_   https://hostname/ng/external-connector
 
-`Interface`_        https://hostname/ng/interface
+                      https://hostname/api/v2/cmdb/system/external-resource/
 
-                    https://hostname/api/v2/cmdb/system/interface/
+`Interface`_          https://hostname/ng/interface
 
-`InternetService`_  https://hostname/ng/firewall/internet_service
+                      https://hostname/api/v2/cmdb/system/interface/
 
-                    https://hostname/api/v2/cmdb/firewall/internet-service/
+`InternetService`_    https://hostname/ng/firewall/internet_service
 
-`IpPool`_           https://hostname/ng/firewall/ip-pool
+                      https://hostname/api/v2/cmdb/firewall/internet-service/
 
-                    https://hostname/api/v2/cmdb/firewall/ippool/
+`IpPool`_             https://hostname/ng/firewall/ip-pool
 
-`Policy`_           https://hostname/ng/firewall/policy/policy/standard
+                      https://hostname/api/v2/cmdb/firewall/ippool/
 
-                    https://hostname/api/v2/cmdb/firewall/policy/
+`Policy`_             https://hostname/ng/firewall/policy/policy/standard
 
-`Schedule`_         https://hostname/ng/firewall/schedule
+                      https://hostname/api/v2/cmdb/firewall/policy/
 
-                    https://hostname/api/v2/cmdb/firewall.schedule/onetime/
+`Schedule`_           https://hostname/ng/firewall/schedule
 
-`Service`_          https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.schedule/onetime/
 
-                    https://hostname/api/v2/cmdb/firewall.service/custom/
+`Service`_            https://hostname/ng/firewall/service
 
-`ServiceCategory`_  https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.service/custom/
 
-                    https://hostname/api/v2/cmdb/firewall.service/category/
+`ServiceCategory`_    https://hostname/ng/firewall/service
 
-`ServiceGroup`_     https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.service/category/
 
-                    https://hostname/api/v2/cmdb/firewall.service/group/
+`ServiceGroup`_       https://hostname/ng/firewall/service
 
-`SnmpCommunity`_    https://hostname/ng/system/snmp
+                      https://hostname/api/v2/cmdb/firewall.service/group/
 
-                    https://hostname/api/v2/cmdb/system.snmp/community/
+`SnmpCommunity`_      https://hostname/ng/system/snmp
 
-`VirtualIp`_        https://hostname/ng/firewall/virtual-ip
+                      https://hostname/api/v2/cmdb/system.snmp/community/
 
-                    https://hostname/api/v2/cmdb/firewall/vip/
+`VirtualIp`_          https://hostname/ng/firewall/virtual-ip
 
-`Zone`_             https://hostname/ng/interface
+                      https://hostname/api/v2/cmdb/firewall/vip/
 
-                    https://hostname/api/v2/cmdb/system/zone/
-=================== ================================================================================
+`Zone`_               https://hostname/ng/interface
+
+                      https://hostname/api/v2/cmdb/system/zone/
+===================== ==============================================================================
 
 
 ----------------------------------------------------------------------------------------------------
 
 FortigateAPI
 ------------
 **FortigateAPI(host, username, password, scheme, port, timeout, vdom)**
 Set of methods for working with the most commonly used `Objects`_.
-Code usage examples in *./examples/examples.py*
 
 =============== ======= ============================================================================
 Parameter        Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
-username        *str*   Administrator name
-password        *str*   Administrator password
+username        *str*   Administrator name. Mutually exclusive with token
+password        *str*   Administrator password. Mutually exclusive with token
+token           *str*   Administrator token. Mutually exclusive with username and password
 scheme          *str*   (optional) "https" (default) or "http"
 port            *int*   (optional) TCP port, by default 443 for "https", 80 for "http"
 timeout         *int*   (optional) Session timeout minutes (default 15)
 verify          *str*   (optional) Enable SSL certificate verification for HTTPS requests. True -  enable, False - disable (default)
 vdom            *str*   Name of virtual domain (default "root")
 =============== ======= ============================================================================
 
 
 ----------------------------------------------------------------------------------------------------
 
 Address
 -------
+Python examples `./examples/address.py`_
+
+Python examples `./examples/address_token.py`_
+
 FortiOS v6.4 data example `./examples/yml/address.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create address
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.252",
+            "type": "ipmask"}
+    response = fgt.address.create(data)
+
+    # Get all addresses
+    addresses_all = fgt.address.get()
+
+    # Get address by name
+    addresses_by_name = fgt.address.get(uid="ADDRESS")
+
+    # Get address by operator contains \"=@\"
+    addresses_contains = fgt.address.get(filter="subnet=@127.0")
+
 
 create()
 ........
 **FortigateAPI.address.create(data)**
-Creates address-object in the Fortigate.
+Create address-object in the Fortigate.
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the address-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
 **FortigateAPI.address.delete(uid, filter)**
-Deletes address-object from the Fortigate.
+Delete address-object from the Fortigate.
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*               Unique identifier. Name of the address-object. Used to delete a single object
-filter          *str*, *List[str]*  Filters address-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters address-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -240,68 +271,70 @@
 uid             *str*   Name of the address-object, taken from the `uid` parameter or from data["name"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
+----------------------------------------------------------------------------------------------------
 
-Address examples:
+AddressGroup
+------------
+Python examples `./examples/address_group.py`_
 
-- Creates address in the Fortigate
-- Gets all addresses from the Fortigate
-- Gets filtered address by name (unique identifier)
-- Filters address by operator *equals* "=="
-- Filters address by operator *contains* "=@"
-- Filters address by operator *not equals* "!="
-- Updates address data in the Fortigate
-- Checks for presence of address in the Fortigate
-- Deletes address from the Fortigate by name
-- Deletes addresses from the Fortigate by filter
-- Checks for absence of address in the Fortigate
-- FortigateAPI *with* statement
+FortiOS v6.4 data example `./examples/yml/address_group.yml`_
 
-`./examples/address.py`_
+.. code:: python
 
+    from fortigate_api import FortigateAPI
 
-----------------------------------------------------------------------------------------------------
+    fgt = FortigateAPI(host="host", username="username", password="password")
 
-AddressGroup
-------------
-FortiOS v6.4 data example `./examples/yml/address_group.yml`_
+    # Create address and address-group in the Fortigate
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.255",
+            "type": "ipmask"}
+    fgt.address.create(data)
+    data = {"name": "ADDR_GROUP", "member": [{"name": "ADDRESS"}]}
+    fgt.address_group.create(data)
+
+    # Get all address-groups from the Fortigate
+    address_groups_all = fgt.address_group.get()
+
+    # Get filtered address_group by name (unique identifier)
+    address_groups_name = fgt.address_group.get(uid="ADDR_GROUP")
 
 
 create()
 ........
 **FortigateAPI.address_group.create(data)**
-Creates address-group-object in the Fortigate
+Create address-group-object in the Fortigate
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the address-group-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
 **FortigateAPI.address_group.delete(uid, filter)**
-Deletes address-group-object from the Fortigate
+Delete address-group-object from the Fortigate
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*               Name of the address-group-object (unique identifier). Used to delete a single object
-filter          *str*, *List[str]*  Filters address-group-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters address-group-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -347,33 +380,14 @@
 uid             *str*   Name of the address-group-object, taken from the `uid` parameter or from data["name"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-AddressGroup examples:
-
-- Creates address-group in the Fortigate
-- Gets all address-groups from the Fortigate
-- Gets filtered address-group by name (unique identifier)
-- Filters address-group by operator *equals* "=="
-- Filters address-group by operator *contains* "=@"
-- Filters address-group by operator *not equals* "!="
-- Updates address-group data in the Fortigate
-- Checks for presence of address-group in the Fortigate
-- Deletes address-group from the Fortigate by name
-- Deletes address-groups from the Fortigate by filter
-- Checks for absence of address-group in the Fortigate
-
-`./examples/address_group.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Antivirus
 ---------
 **Antivirus** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/antivirus.yml`_
@@ -410,37 +424,95 @@
 
 ----------------------------------------------------------------------------------------------------
 
 DhcpServer
 ----------
 **DhcpServer** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/dhcp_server.py`_
+
 FortiOS v6.4 data example `./examples/yml/dhcp_server.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create dhcp server
+    data = {
+        "default-gateway": "192.168.255.1",
+        "netmask": "255.255.255.0",
+        "interface": "vlan.123",
+        "ip-range": [{"start-ip": "192.168.255.2", "end-ip": "192.168.255.254", }],
+    }
+    fgt.dhcp_server.create(data)
+
+    # Get all dhcp servers
+    dhcp_servers = fgt.dhcp_server.get()
+
+
 **FortigateAPI.dhcp_server.create(data)** Note, in Fortigate is possible to create multiple DHCP servers with the same settings, you need control duplicates
 
 **FortigateAPI.dhcp_server.delete(uid, filter)**
 
 **FortigateAPI.dhcp_server.get(uid, filter)**
 
 **FortigateAPI.dhcp_server.is_exist(uid)**
 
 **FortigateAPI.dhcp_server.update(data, uid)**
 
-DhcpServer examples `./examples/dhcp_server.py`_
+
+----------------------------------------------------------------------------------------------------
+
+ExternalResource
+----------------
+**ExternalResource** object has the same parameters and methods as `Address`_
+
+Python examples `./examples/external_resource.py`_
+
+FortiOS v6.4 data example `./examples/yml/external_resource.yml`_
+
+**FortigateAPI.external_resource.create(data)**
+
+**FortigateAPI.external_resource.delete(uid, filter)**
+
+**FortigateAPI.external_resource.get(uid, filter)**
+
+**FortigateAPI.external_resource.is_exist(uid)**
+
+**FortigateAPI.external_resource.update(data, uid)**
+
 
 
 ----------------------------------------------------------------------------------------------------
 
 Interface
 ---------
 **Interface** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/interface.py`_
+
 FortiOS v6.4 data example `./examples/yml/interface.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+
+    # Get all interfaces in vdom \"root\" from the Fortigate
+    interfaces = fgt.interface.get()
+    print(f"interfaces count={len(interfaces)}")  # interfaces count=21
+
+    # Gets filtered interface by name (unique identifier)
+    interfaces = fgt.interface.get(uid="dmz")
+
+
 **FortigateAPI.interface.create(data)**
 
 **FortigateAPI.interface.delete(uid, filter)**
 
 
 get()
 .....
@@ -459,31 +531,14 @@
     *List[dict]* List of interface-objects
 
 **FortigateAPI.interface.is_exist(uid)**
 
 **FortigateAPI.interface.update(data, uid)**
 
 
-Examples
-........
-Interface examples:
-
-- Gets all interfaces in vdom "root" from the Fortigate
-- Gets filtered interface by name (unique identifier)
-- Filters interface by operator *equals* "=="
-- Filters interface by operator contains "=@"
-- Filters interface by operator *not equals* "!="
-- Filters interface by multiple conditions
-- Updates interface data in the Fortigate
-- Checks for presence of interface in the Fortigate
-- Gets all interfaces in vdom "VDOM"
-
-`./examples/interface.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 InternetService
 ---------------
 **InternetService** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/internet_service.yml`_
@@ -501,66 +556,91 @@
 
 ----------------------------------------------------------------------------------------------------
 
 IpPool
 ------
 **IpPool** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/ip_pool.py`_
+
 FortiOS v6.4 data example `./examples/yml/ip_pool.yml`_
 
 **FortigateAPI.ip_pool.create(data)**
 
 **FortigateAPI.ip_pool.delete(uid, filter)**
 
 **FortigateAPI.ip_pool.get(uid, filter)**
 
 **FortigateAPI.ip_pool.is_exist(uid)**
 
 **FortigateAPI.ip_pool.update(data, uid)**
 
 
-Examples
-........
-IpPool examples:
-
-`./examples/ip_pool.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Policy
 ------
+Python examples `./examples/policy.py`_
+
+Python examples `./examples/policy_extended_filter.py`_
+
 FortiOS v6.4 data example `./examples/yml/policy.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create policy in the Fortigate
+    data = dict(
+        name="POLICY",
+        status="enable",
+        action="accept",
+        srcintf=[{"name": "any"}],
+        dstintf=[{"name": "any"}],
+        srcaddr=[{"name": "all"}],
+        dstaddr=[{"name": "all"}],
+        service=[{"name": "ALL"}],
+        schedule="always",
+    )
+    fgt.policy.create(data)
+
+    # Get all policies from the Fortigate
+    policies_all = fgt.policy.get()
+
+    # Filters policies by name, by operator equals
+    policies_name = fgt.policy.get(filter="name==POLICY")
+
 
 create()
 ........
 **FortigateAPI.policy.create(data)**
-Creates policy-object in the Fortigate
+Create policy-object in the Fortigate
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the policy-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
-Deletes policy-object from the Fortigate
+Delete policy-object from the Fortigate
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*, *int*        Identifier of the policy-object. Used to delete a single object
-filter          *str*, *List[str]*  Filters policy-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters policy-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -623,46 +703,14 @@
 uid             *int*   Policyid of the policy-object, taken from the `uid` parameter or from data["policyid"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-Policy examples:
-
-- Creates policy in the Fortigate
-- Gets all policies from the Fortigate
-- Gets filtered policy by policyid (unique identifier)
-- Filters policies by name, by operator *equals* "=="
-- Filters policies by operator *contains* "=@"
-- Filters policies by operator *not equals* "!="
-- Updates policy data in the Fortigate
-- Checks for presence of policy in the Fortigate
-- Gets all policies with destination address == "192.168.1.2/32"
-- Deletes policy from the Fortigate by policyid (unique identifier)
-- Deletes policies from the Fortigate by filter (by name)
-- Checks for absence of policy in the Fortigate
-
-`./examples/policy.py`_
-
-
-Policy Extended Filter examples:
-
-- Gets the rules where source prefix is equals 127.0.1.0/30
-- Gets the rules where source prefix is not equals 127.0.1.0/30
-- Gets the rules where source addresses are in subnets of 127.0.1.0/24
-- Gets the rules where source prefixes are supernets of address 127.0.1.1/32
-- Gets the rules where source prefix are equals 127.0.1.0/30 and destination prefix are equals 127.0.2.0/30
-- Delete policy, address-group, addresses from the Fortigate (order is important)
-
-`./examples/policy_extended_filter.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Schedule
 --------
 **Schedule** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/schedule.yml`_
@@ -737,14 +785,16 @@
 
 ----------------------------------------------------------------------------------------------------
 
 SnmpCommunity
 -------------
 **SnmpCommunity**
 
+Python examples `./examples/snmp_community.py`_
+
 FortiOS v6.4 data example `./examples/yml/snmp_community.yml`_
 
 **FortigateAPI.snmp_community.create(data)**
 
 **FortigateAPI.snmp_community.delete(uid, filter)**
 
 **FortigateAPI.snmp_community.get(uid, filter)**
@@ -761,19 +811,14 @@
 uid             *str*   Name of the snmp-community-object, taken from the `uid` parameter or from data["id"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-SnmpCommunity examples `./examples/snmp_community.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 VirtualIP
 ---------
 **VirtualIP** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/virtual_ip.yml`_
@@ -813,20 +858,42 @@
 Fortigate
 ---------
 **Fortigate(host, username, password, scheme, port, timeout, vdom)**
 REST API connector to the Fortigate. Contains generic methods (get, put, delete, etc.)
 to work with any objects available through the REST API. `Fortigate`_ is useful for working with
 objects that are not implemented in `FortigateAPI`_
 
+Python examples `./examples/fortigate.py`_
+
+Python examples `./examples/fortigate_token.py`_
+
+.. code:: python
+
+    from fortigate_api import Fortigate
+
+    fgt = Fortigate(host="host", username="username", password="password")
+
+    # Create address in the Fortigate
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.252",
+            "type": "ipmask"}
+    fgt.post(url="api/v2/cmdb/firewall/address/", data=data)
+
+    # Get address data from the Fortigate
+    addresses_all = fgt.get(url="api/v2/cmdb/firewall/address/")
+
+
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
-username        *str*   Administrator name
-password        *str*   Administrator password
+username        *str*   Administrator name. Mutually exclusive with token
+password        *str*   Administrator password. Mutually exclusive with token
+token           *str*   Administrator token. Mutually exclusive with username and password
 scheme          *str*   (optional) "https" (default) or "http"
 port            *int*   (optional) TCP port, by default 443 for "https", 80 for "http"
 timeout         *int*   (optional) Session timeout minutes (default 15)
 verify          *str*   (optional) Enable SSL certificate verification for HTTPS requests. True -  enable, False - disable (default)
 vdom            *str*   Name of virtual domain (default "root")
 =============== ======= ============================================================================
 
@@ -909,38 +976,45 @@
 data            *dict*  Data of the object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-Fortigate examples:
-
-- Creates address in the Fortigate
-- Gets address data from the Fortigate
-- Updates address data in the Fortigate
-- Checks for presence of address in the Fortigate
-- Deletes address from the Fortigate
-- Checks for absence of address in the Fortigate
-- Fortigate *with* statement
-
-`./examples/fortigate.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 SSH
 ---
 **SSH(host, username, password, ssh)**
 SSH connector to the Fortigate. Contains methods to get and put configuration commands using ssh.
 Note, FortigateAPI parameter "vdom" used in REST API only and not used in SSH.
 In order to send cli commands to a specific vdom, you need "config vdom" before.
 
+Python examples `./examples/ssh.py`_
+
+Python examples `./examples/ssh_vdom.py`_
+
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt_api = FortigateAPI(host="host", username="username", password="password")
+    fgt_api.ssh.login()
+
+    # Show interface config
+    config = fgt_api.ssh.send_command("show system interface dmz")
+
+    # Change interface description from "dmz" to "DMZ"
+    cmds = ["config system interface",
+            "edit dmz",
+            "set description DMZ",
+            "end"]
+    output = fgt_api.ssh.send_config_set(cmds)
+
+
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
 username        *str*   Administrator name
 password        *str*   Administrator password
 ssh             *dict*  Netmiko *ConnectHandler* parameters
@@ -982,79 +1056,44 @@
 cmds            *List[str]*   Configuration commands to be executed on the Fortigate
 kwargs          *dict*        (optional) Netmiko parameters
 =============== ============= ======================================================================
 
 Return
     Output of the commands
 
-
-Examples
-........
-SSH examples:
-
-- Show interface config
-- Change interface description from "dmz" to "DMZ"
-- Check interface description is changed
-- Change read-timeout timer for long awaited commands
-
-`./examples/ssh.py`_
-
-SSH examples for working with vdom:
-
-- get system arp from interfaces associated with vdom="VDOM"
-- get system arp from interfaces associated with vdom="root"
-
-`./examples/ssh_vdom.py`_
-
 ----------------------------------------------------------------------------------------------------
 
-CiscoConfParse
---------------
-Helper that parses the Fortigate configuration to find and modify command lines.
-CiscoConfParse doesn't natively support Fortigate configuration,
-but after some tweaking in this package it has become a good tool to play with Fortigate config lines.
-For more information, see the documentation for the JunosCfgLine object at https://github.com/mpenning/ciscoconfparse
-
-
-Examples
-........
-CiscoConfParse examples:
-
-- get config from the Fortigate by SSH
-- create CiscoConfParse object
-- filter all JunosCfgLine objects of wan interfaces
-- print some data in CiscoConfParse objects
-- filter all wan interfaces blocks
-
-`./examples/ccp.py`_
-
 
 .. _`./examples`: ./examples
+.. _`./examples/yml`: ./examples/yml
 .. _`./examples/yml/address.yml`: ./examples/yml/address.yml
 .. _`./examples/yml/address_group.yml`: ./examples/yml/address_group.yml
 .. _`./examples/yml/antivirus.yml`: ./examples/yml/antivirus.yml
 .. _`./examples/yml/application.yml`: ./examples/yml/application.yml
 .. _`./examples/yml/dhcp_server.yml`: ./examples/yml/dhcp_server.yml
+.. _`./examples/yml/external_resource.yml`: ./examples/yml/external_resource.yml
 .. _`./examples/yml/interface.yml`: ./examples/yml/interface.yml
 .. _`./examples/yml/internet_service.yml`: ./examples/yml/internet_service.yml
 .. _`./examples/yml/ip_pool.yml`: ./examples/yml/ip_pool.yml
 .. _`./examples/yml/policy.yml`: ./examples/yml/policy.yml
 .. _`./examples/yml/schedule.yml`: ./examples/yml/schedule.yml
 .. _`./examples/yml/service.yml`: ./examples/yml/service.yml
 .. _`./examples/yml/service_category.yml`: ./examples/yml/service_category.yml
 .. _`./examples/yml/service_group.yml`: ./examples/yml/service_group.yml
 .. _`./examples/yml/snmp_community.yml`: ./examples/yml/snmp_community.yml
 .. _`./examples/yml/virtual_ip.yml`: ./examples/yml/virtual_ip.yml
 .. _`./examples/yml/zone.yml`: ./examples/yml/zone.yml
 
 .. _`./examples/address.py`: ./examples/address.py
+.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/address_group.py`: ./examples/address_group.py
-.. _`./examples/ccp.py`: ./examples/ccp.py
 .. _`./examples/dhcp_server.py`: ./examples/dhcp_server.py
+.. _`./examples/external_resource.py`: ./examples/external_resource.py
 .. _`./examples/fortigate.py`: ./examples/fortigate.py
+.. _`./examples/fortigate_token.py`: ./examples/fortigate_token.py
 .. _`./examples/interface.py`: ./examples/interface.py
 .. _`./examples/ip_pool.py`: ./examples/ip_pool.py
 .. _`./examples/policy.py`: ./examples/policy.py
 .. _`./examples/policy_extended_filter.py`: ./examples/policy_extended_filter.py
 .. _`./examples/snmp_community.py`: ./examples/snmp_community.py
 .. _`./examples/ssh.py`: ./examples/ssh.py
 .. _`./examples/ssh_vdom.py`: ./examples/ssh_vdom.py
```

### Comparing `fortigate_api-1.1.1/fortigate_api/ccp.py` & `fortigate_api-1.2.2/fortigate_api/ccp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-"""CiscoConfParse
+"""CiscoConfParse.
+
 Helper that parses the Fortigate config to find and change config commands.
 For more details see https://github.com/mpenning/ciscoconfparse
 """
 import re
 from typing import List
 
 from ciscoconfparse import CiscoConfParse, JunosCfgLine  # type: ignore
 
-from fortigate_api import str_
+from fortigate_api import helpers as h
 from fortigate_api.types_ import LStr, T2Str, T3Str, UStr
 
 LJunosCfgLine = List[JunosCfgLine]
 
 
 class FgtConfParse(CiscoConfParse):
-    """CiscoConfParse adapted for Fortigate"""
+    """CiscoConfParse adapted for Fortigate."""
 
     def __init__(self, config: UStr, comment="#", encoding="UTF-8", **kwargs):
-        """FgtConfParse
+        """FgtConfParse.
+
         ::
             :param config: Fortigate config
             :type config: str, List[str]
             :param comment: Comment delimiter (default "#")
             :type comment: str
             :param kwargs: Other CiscoConfParse parameters
             :return: CiscoConfParse object with JunosCfgLine lines
@@ -30,48 +32,50 @@
         config_ = convert_fgt_to_junos(config_)
         lines = config_.splitlines()
         kwargs.update(config=lines, comment=comment, encoding=encoding, syntax="junos")
         super().__init__(**kwargs)
 
     @staticmethod
     def _init_config(config: UStr) -> str:
-        """Init Fortigate config"""
+        """Init Fortigate config."""
         if isinstance(config, str):
             return config
         if not isinstance(config, (list, tuple)):
             raise TypeError(f"{config=} {str} expected")
         for line in config:
             if not isinstance(line, str):
                 raise TypeError(f"{line=} {str} expected")
         return "\n".join(config)
 
 
 # ============================= function =============================
 
 def convert_fgt_to_junos(config: str) -> str:
-    """Convert Fortigate commands to Junos syntax, to parse by ciscoconfparse
-    :param config: Fortigate syntax config
-    :return config: CiscoConfParse junos syntax config
-    :example:
-        config = "
-            config system interface
-              edit "mgmt"
-                set ip 10.0.0.1 255.255.255.0
-              next
-            end
-           "
-        convert_fgt_to_junos(config) -> "
-            config system interface {
-              edit "mgmt" {
-                set ip 10.0.0.1 255.255.255.0
-              }
-              next
-            }
-            end
-           "
+    """Convert Fortigate commands to Junos syntax, to parse by ciscoconfparse.
+
+    ::
+        :param config: Fortigate syntax config
+        :return config: CiscoConfParse junos syntax config
+        :example:
+            config = "
+                config system interface
+                  edit "mgmt"
+                    set ip 10.0.0.1 255.255.255.0
+                  next
+                end
+               "
+            convert_fgt_to_junos(config) -> "
+                config system interface {
+                  edit "mgmt" {
+                    set ip 10.0.0.1 255.255.255.0
+                  }
+                  next
+                }
+                end
+               "
     """
     spaces = r"^(\s+)?"
     re_config = f"({spaces}config .+)"
     re_end = f"{spaces}(end)"
     re_edit = f"({spaces}edit .+)"
     re_next = f"{spaces}(next)"
     re_comment = f"$|{spaces}#"
@@ -99,74 +103,79 @@
             line = indent + "}\n" + indent + "next"
         junos_lines.append(line)
 
     return "\n".join(junos_lines)
 
 
 def findall(regex: str, obj: JunosCfgLine, flags=0) -> LStr:
-    """Parses substrings from *JunosCfgLine* objects by regex
+    """Parse substrings from *JunosCfgLine* objects by regex.
+
     ::
         :param regex: Regex pattern with 1 group
         :param obj: JunosCfgLine object
         :param flags: re.findall flags
         :return: List of interested substrings
     """
     string = "\n".join(obj.ioscfg)
     values = re.findall(pattern=regex, string=string, flags=flags)
     return values
 
 
 def findall1(regex: str, obj: JunosCfgLine, flags=0) -> str:
-    """Parses substring from *JunosCfgLine* objects by regex
+    """Parse substring from *JunosCfgLine* objects by regex.
+
     ::
         :param regex: Regex pattern with 1 group
         :param obj: JunosCfgLine object
         :param flags: re.findall flags
         :return: Interested substring
     """
     value = ""
     for item in obj.ioscfg:
-        if value := str_.findall1(pattern=regex, string=item, flags=flags):
+        if value := h.findall1(pattern=regex, string=item, flags=flags):
             break
     return value
 
 
 def findall2(regex: str, obj: JunosCfgLine, flags=0) -> T2Str:
-    """Parses 2 substrings from *JunosCfgLine* objects by regex
+    """Parse 2 substrings from *JunosCfgLine* objects by regex.
+
     ::
         :param regex: Regex pattern with 2 groups
         :param obj: JunosCfgLine object
         :param flags: re.findall flags
         :return: Interested substrings
     """
     value1, value2 = "", ""
     for item in obj.ioscfg:
-        value1, value2 = str_.findall2(pattern=regex, string=item, flags=flags)
+        value1, value2 = h.findall2(pattern=regex, string=item, flags=flags)
         if value1:
             break
     return value1, value2
 
 
 def findall3(regex: str, obj: JunosCfgLine) -> T3Str:
-    """Parses 3 substrings from *JunosCfgLine* objects by regex
+    """Parse 3 substrings from *JunosCfgLine* objects by regex.
+
     ::
         :param regex: Regex pattern with 3 groups
         :param obj: JunosCfgLine object
         :return: Interested substrings
     """
     value1, value2, value3 = "", "", ""
     for item in obj.ioscfg:
-        value1, value2, value3 = str_.findall3(pattern=regex, string=item)
+        value1, value2, value3 = h.findall3(pattern=regex, string=item)
         if value1:
             break
     return value1, value2, value3
 
 
 def find_by_keys(ccp: CiscoConfParse, keys: LStr) -> LJunosCfgLine:
-    """Finds object by keys in geneology
+    r"""Find object by keys in geneology.
+
     ::
         :param ccp: CiscoConfParse object
         :param keys: Geneology keys to find object
         :return: List of JunosCfgLine objects
         :rtype: List[JunosCfgLine]
         :example:
             keys = ["config system global", "edit \"wan1\""]
@@ -188,15 +197,16 @@
         all_parents: LStr = [o.text.strip() for o in obj.all_parents]
         if keys_parent == all_parents:
             results.append(obj)
     return results
 
 
 def find_by_re_keys(ccp: CiscoConfParse, keys: LStr) -> LJunosCfgLine:
-    """Finds object by keys regex in geneology
+    """Find object by keys regex in geneology.
+
     ::
         :param ccp: CiscoConfParse object
         :param keys: Geneology regex keys to find object
         :return: List of JunosCfgLine objects
         :rtype: List[JunosCfgLine]
         :example:
             keys = ["config system global", r"edit .wan[12]."]
@@ -231,15 +241,16 @@
                 if re.search(re_parent, parent):
                     results.append(obj)
                     break
     return results
 
 
 def find_children(ccp: CiscoConfParse, keys: LStr) -> LJunosCfgLine:
-    """Finds children object by geneology keys
+    r"""Find children object by geneology keys.
+
     ::
         :param ccp: CiscoConfParse object
         :param keys: Geneology keys to find object
         :return: List of children JunosCfgLine objects
         :rtype: List[JunosCfgLine]
         :example:
             keys = ["config system global", "edit \"wan1\""]
@@ -247,26 +258,28 @@
                                          "set ip 10.0.1.1 255.255.255.0",
                                          ...]
     """
     return [o for oo in find_by_keys(ccp, keys) for o in oo.children]
 
 
 def join_children(obj: JunosCfgLine) -> str:
-    """Join all children of JunosCfgLine object
+    """Join all children of JunosCfgLine object.
+
     ::
         :param obj: JunosCfgLine object
         :return: joined text lines of all children
         :rtype: str
     """
     lines = [o.text for o in obj.all_children]
     return "\n".join(lines)
 
 
 def find_re_blocks(ccp: CiscoConfParse, regex: str) -> LStr:
-    """Works similar to CiscoConfParse.find_block(), but returns list of config sections"
+    r"""Work similar to CiscoConfParse.find_block(), but return list of config sections".
+
     ::
         :param ccp: CiscoConfParse object
         :param regex: Regex pattern to find
         :return: Lines of all_children in found block
         :example:
             regex = "edit \"wan1\""
             find_children(ccp, keys) -> ["set vdom \"root\"",
```

### Comparing `fortigate_api-1.1.1/fortigate_api/dhcp_server.py` & `fortigate_api-1.2.2/fortigate_api/dhcp_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,56 @@
-"""DHCP Server Object"""
+"""DHCP Server Object."""
 
 from requests import Response
 
 from fortigate_api.base import Base
 from fortigate_api.types_ import DAny, StrInt
 
 
 class DhcpServer(Base):
-    """DHCP Server Object"""
+    """DHCP Server Object."""
 
-    def __init__(self, fgt):
-        super().__init__(fgt=fgt, url_obj="api/v2/cmdb/system.dhcp/server/", uid_key="id")
+    def __init__(self, rest):
+        """DHCP Server Object.
+
+        ::
+            :param rest: Fortigate REST API connector
+            :type rest: Fortigate
+        """
+        super().__init__(rest=rest, url_obj="api/v2/cmdb/system.dhcp/server/", uid_key="id")
 
     def create(self, data: DAny) -> Response:
-        """Creates dhcp-server-object in the Fortigate.
+        """Create dhcp-server-object in the Fortigate.
+
         Note, in Fortigate is possible to create multiple DHCP servers with the same settings,
         you need control duplicates
-        :param data: Data of the fortigate-object
-        :return: Session response
-            *<Response [200]>* Object successfully created or already exists
+        ::
+            :param data: Data of the fortigate-object
+            :type data: dict
+
+            :return: Session response
+                *<Response [200]>* Object successfully created or already exists
+            :rtype: Response
         """
-        return self.fgt.post(url=self.url_, data=data)
+        return self.rest.post(url=self.url_, data=data)
 
     def update(self, data: DAny, uid: StrInt = "") -> Response:
-        """Updates dhcp-server-object, where `uid` is data["id"]
-        :param data: Data of the dhcp-server-object
-        :param uid: ID of the dhcp-server-object,
-            taken from the `uid` parameter or from data["id"]
-        :return: Session response
-            *<Response [200]>* Object successfully updated
-            *<Response [404]>* Object has not been updated
+        """Update dhcp-server-object, where `uid` is data["id"].
+
+        ::
+            :param data: Data of the dhcp-server-object
+            :type data: dict
+
+            :param uid: ID of the dhcp-server-object,
+                taken from the `uid` parameter or from data["id"]
+            :type uid: str or int
+
+            :return: Session response
+                *<Response [200]>* Object successfully updated
+                *<Response [404]>* Object has not been updated
+            :rtype: Response
         """
         if not uid:
             uid = data.get("id") or ""
             if not uid:
                 raise ValueError(f"absent {uid=} and data[\"id\"]")
         return self._update(uid=uid, data=data)
```

### Comparing `fortigate_api-1.1.1/fortigate_api/extended_filters.py` & `fortigate_api-1.2.2/fortigate_api/extended_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,114 @@
-"""Extended Filters"""
+"""Extended Filters."""
 import logging
 from collections import Counter
 from functools import wraps
 from ipaddress import ip_network, IPv4Network
 from typing import Tuple
 
-from fortigate_api import dict_, str_
+from fortigate_api import helpers as h
 from fortigate_api.address import Address
 from fortigate_api.address_group import AddressGroup
 from fortigate_api.types_ import LDAny, LStr, DLStr, DLInet
 
 EFILTER_KEYS = ["dstaddr", "srcaddr"]
 EFILTER_OPERATORS = [
     "==",  # equal
     "!=",  # not equal
     ">=",  # supernets of interested prefix
     "<=",  # subnets of interested prefix
 ]
 
 
 def wrapp_efilters(func):
-    """Wrapper. Extended Filters"""
-
+    """Wrapp Extended Filters."""
     # noinspection PyIncorrectDocstring
     @wraps(func)
     def wrapper(fgt_api, **kwargs):
-        """Wrapper. Extended Filters
-        :param FortigateAPI fgt_api: Wrapped object
-        :param str efilter: Extended filter: "srcaddr", "dstaddr" by condition: equals "==",
-            not equals "!=",  supernets ">=", subnets "<="
-        :param kwargs: Parameters for wrapped object
-        :return: *List[dict_]* List of the fortigate-objects
+        """Wrapp Extended Filters.
+
+        ::
+            :param fgt_api: Wrapped object
+            :type fgt_api: FortigateAPI
+
+            :param efilter: Extended filter: "srcaddr", "dstaddr" by condition: equals "==",
+                not equals "!=",  supernets ">=", subnets "<="
+            :type efilter: str or List[str]
+
+            :param kwargs: Parameters for wrapped object
+
+            :return: List of the fortigate-objects
+            :rtype: List[dict]
         """
-        if efilters := dict_.pop_lstr(key="efilter", data=kwargs):
+        if efilters := h.pop_lstr(key="efilter", data=kwargs):
             _valid_efilters(efilters)
 
         datas = func(fgt_api, **kwargs)
 
         for efilter in efilters:
-            efilter_by_sdst(policies=datas, efilter=efilter, fgt=fgt_api.fgt)
+            efilter_by_sdst(policies=datas, efilter=efilter, rest=fgt_api.rest)
         return datas
 
     return wrapper
 
 
-def efilter_by_sdst(policies: LDAny, efilter: str, fgt) -> None:
-    """Filter policies by efilter "srcaddr", "dstaddr"
-    :param policies: Policies
-    :param efilter: Extended filter
-    :param Fortigate fgt: Fortigate connector
-    :return: Side effect `policies`. Pass policies matched by efilter
+def efilter_by_sdst(policies: LDAny, efilter: str, rest) -> None:
+    """Filter policies by efilter "srcaddr", "dstaddr".
+
+    ::
+        :param policies: Policies (side effect)
+        :type policies: List[dict]
+
+        :param efilter: Extended filter
+        :type efilter: str
+
+        :param rest: Fortigate REST API connector
+        :type rest: Fortigate
+
+        :return: None. Updates policies (side effect). Pass policies matched by efilter
     """
     if not _split_efilter(efilter)[0]:
         return
     # get addresses and address-groups from the Fortigate
-    addresses: LDAny = Address(fgt).get()
-    addr_groups: LDAny = AddressGroup(fgt).get()
+    addresses: LDAny = Address(rest).get()
+    addr_groups: LDAny = AddressGroup(rest).get()
     names_subnets_d: DLStr = _get_names_subnets(addresses, addr_groups)
     names_ipnets_d: DLInet = _convert_subnets_to_ipnets(names_subnets_d)
 
     # filter policies
     policies_ = _filter_policy_by_ipnets(efilter, policies, names_ipnets_d)
     policies.clear()
     policies.extend(policies_)
 
 
 def _split_efilter(efilter: str) -> Tuple[str, str, IPv4Network]:
-    """Parse `key`, `operator`, `value` from `efilter` for "srcaddr", "dstaddr"
-    :param efilter: Extended filter
+    """Parse `key`, `operator`, `value` from `efilter` for "srcaddr", "dstaddr".
+
+    ::
+        :param efilter: Extended filter
+        :type efilter: str
+
+        :return: efilter key, efilter operator, efilter value IPv4Network
     """
-    key, operator, value = str_.findall3(pattern=r"(\w+)(..)(.+)", string=efilter)
+    key, operator, value = h.findall3(pattern=r"(\w+)(..)(.+)", string=efilter)
     if key not in ["srcaddr", "dstaddr"]:
         return "", "", IPv4Network("0.0.0.0")
     ipnet = ip_network(value)
     if not isinstance(ipnet, IPv4Network):
         raise ValueError(f"{efilter=} {IPv4Network} expected")
     return key, operator, ipnet
 
 
 def _get_names_subnets(addresses: LDAny, addr_groups: LDAny) -> DLStr:
-    """Get all IPv4Networks from the Fortigate address-objects and address-group-objects.
-    Skip IPv6Networks
-    :param addresses: Fortigate address-objects
-    :param addr_groups: Fortigate address-group-objects
-    :return: Data indexed by address and address-group names (policy members)
+    """Get all IPv4Networks from the Fortigate address-objects, address-group-objects.
+
+    ::
+        :param addresses: Fortigate address-objects
+        :param addr_groups: Fortigate address-group-objects
+        :return: Data indexed by address and address-group names (policy members)
     """
     members_d: DLStr = {d["name"]: [d["subnet"]] for d in addresses if d["type"] == "ipmask"}
     for addgr_d in addr_groups:
         addgr_name = addgr_d["name"]
         members_d[addgr_name] = []
     for addgr_d in addr_groups:
         addgr_name = addgr_d["name"]
@@ -95,20 +116,22 @@
         for member_name in members_:
             subnets = members_d[member_name]
             members_d[addgr_name].extend(subnets)
     return members_d
 
 
 def _convert_subnets_to_ipnets(members_d: DLStr) -> DLInet:
-    """Converts subnets to IPv4Networks
-    :param members_d: Members names and subnets (in policies)
-    :return: Members names and IPv4Networks
-    :example:
-        members: {"ADDRESS": ["1.1.1.1 255.255.255.255"], "ADDR_GR": ["2.2.2.0 255.255.255.0"]}
-        return: {"ADDRESS": [IPv4Network("1.1.1.1/32")], "ADDR_GR": [IPv4Network("2.2.2.0/24")]}
+    """Convert subnets to IPv4Networks.
+
+    ::
+        :param members_d: Members names and subnets (in policies)
+        :return: Members names and IPv4Networks
+        :example:
+            members: {"ADDRESS": ["1.1.1.1 255.255.255.255"], "ADDR_GR": ["2.2.2.0 255.255.255.0"]}
+            return: {"ADDRESS": [IPv4Network("1.1.1.1/32")], "ADDR_GR": [IPv4Network("2.2.2.0/24")]}
     """
     ipnets_d: DLInet = {}
     for name, subnets in members_d.items():
         ipnets_d[name] = []
     for name, subnets in members_d.items():
         for subnet in subnets:
             subnet = "/".join(subnet.strip().split(" "))
@@ -121,42 +144,47 @@
                 logging.error(msg)
 
     ipnets_d["all"] = [IPv4Network("0.0.0.0/0")]
     return ipnets_d
 
 
 def _valid_efilters(efilters: LStr) -> None:
-    """Validate efilters key, operator, value
-    :param efilters: Extended filters keys
-    :raises ValueError: If efilter has invalid format
+    """Validate efilters key, operator, value.
+
+    ::
+        :param efilters: Extended filters keys
+        :return: None. efilters has valid format
+        :raises ValueError: If efilter has invalid format
     """
     re_operators = "|".join(EFILTER_OPERATORS)
     regex = r"(\w+?)({})(.+)".format(re_operators)
     keys: LStr = []
     for efilter in efilters:
-        key, operator, value = str_.findall3(pattern=regex, string=efilter)
+        key, operator, value = h.findall3(pattern=regex, string=efilter)
         keys.append(key)
         expected = EFILTER_KEYS
         if key not in expected:
             raise ValueError(f"invalid {efilter=}, {expected=}")
         expected = EFILTER_OPERATORS
         if operator not in expected:
             raise ValueError(f"invalid {operator=}, {expected=}")
 
     counts = Counter(keys)
     if invalid := [k for k, v in counts.items() if v > 1]:
         raise ValueError(f"{invalid=} in {efilters=}, expected only one key")
 
 
 def _filter_policy_by_ipnets(efilter: str, policies: LDAny, names_ipnets_d: DLInet) -> LDAny:
-    """Filter `policies` by `efilter` "srcaddr", "dstaddr"
-    :param efilter: Extended filter
-    :param policies: Policies
-    :param names_ipnets_d: Members names and IPv4Networks
-    :return: Filtered policies
+    """Filter `policies` by `efilter` "srcaddr", "dstaddr".
+
+    ::
+        :param efilter: Extended filter
+        :param policies: Policies
+        :param names_ipnets_d: Members names and IPv4Networks
+        :return: Filtered policies
     """
     key, operator, ipnet_filter = _split_efilter(efilter)
 
     policies_: LDAny = []  # result
     for policy in policies:
         members = [d["name"] for d in policy[key]]
         for member in members:
```

### Comparing `fortigate_api-1.1.1/fortigate_api/fortigate.py` & `fortigate_api-1.2.2/fortigate_api/fortigate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,205 @@
-"""**Fortigate(host, username, password, scheme, port, timeout, vdom)**
+"""**Fortigate(host, username, password, scheme, port, timeout, vdom)**.
+
 REST API connector to the Fortigate. Contains generic methods (get, put, delete, etc.)
 to work with any objects available through the REST API. `Fortigate`_ is useful for working with
 objects that are not implemented in `FortigateAPI`_
 """
 from __future__ import annotations
 
 import json
 import logging
 import re
-from typing import Iterable, Optional
+from typing import Callable, Iterable, Optional
 from urllib.parse import urlencode
 
 import requests
 from requests import Session, Response
 from requests.exceptions import SSLError
 from requests.packages import urllib3  # type: ignore
 
-from fortigate_api import str_
-from fortigate_api.types_ import DAny, LDAny
+from fortigate_api import helpers as h
+from fortigate_api.types_ import DAny, LDAny, DStr, Method
 
 # noinspection PyUnresolvedReferences
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 HTTPS = "https"
 PORT_443 = 443
 PORT_80 = 80
 TIMEOUT = 15
 VDOM = "root"
 
 
 class Fortigate:
-    """**Fortigate(host, username, password, scheme, port, timeout, vdom)**
+    """**Fortigate(host, username, password, scheme, port, timeout, vdom)**.
+
     REST API connector to the Fortigate. Contains generic methods (get, put, delete, etc.)
     to work with any objects available through the REST API. `Fortigate`_ is useful for working with
     objects that are not implemented in `FortigateAPI`_
     """
 
-    def __init__(self, host: str, username: str, password: str, **kwargs):
-        """**Fortigate** - Firewall Connector
-        :param host: Firewall ip address or hostname
-        :type host: str
+    def __init__(self, host: str, **kwargs):
+        """**Fortigate** - Firewall Connector.
+
+        ::
+            :param host: Firewall ip address or hostname
+            :type host: str
 
-        :param username: Administrator name
-        :type username: str
+            :param username: Administrator name. Mutually exclusive with token
+            :type username: str
 
-        :param password: Administrator password
-        :type password: str
+            :param password: Administrator password. Mutually exclusive with token
+            :type password: str
 
-        :param scheme: (optional) "https" (default) or "http"
-        :type scheme: str
+            :param token: Administrator token. Mutually exclusive with username and password
+            :type token: str
 
-        :param port: (optional) TCP port, by default 443 for "https", 80 for "http"
-        :type port: str
+            :param scheme: (optional) "https" (default) or "http"
+            :type scheme: str
 
-        :param timeout: (optional) Session timeout minutes (default 15)
-        :type timeout: int
+            :param port: (optional) TCP port, by default 443 for "https", 80 for "http"
+            :type port: str
 
-        :param verify: (optional) Enable SSL certificate verification for HTTPS requests.
-            True -  enable
-            False - disable (default)
-        :type verify: bool
+            :param timeout: (optional) Session timeout minutes (default 15)
+            :type timeout: int
 
-        :param vdom: Name of virtual domain (default "root")
-        :type vdom: str
+            :param verify: (optional) Enable SSL certificate verification for HTTPS requests.
+                True -  enable
+                False - disable (default)
+            :type verify: bool
+
+            :param vdom: Name of virtual domain (default "root")
+            :type vdom: str
         """
         self.host = host
-        self.username = username
-        self.password = password
+        self.username = str(kwargs.get("username") or "")
+        self.password = str(kwargs.get("password") or "")
+        self.token = self._init_token(**kwargs)
         self.scheme: str = self._init_scheme(**kwargs)
         self.port: int = self._init_port(**kwargs)
         self.timeout: int = int(kwargs.get("timeout") or TIMEOUT)
         self.vdom: str = str(kwargs.get("vdom") or VDOM)
         self.verify: bool = bool(kwargs.get("verify") or False)
         self._session: Optional[Session] = None
 
     def __repr__(self):
+        """Return a string representation related to this object."""
         host = self.host
         username = self.username
-        password = "*" * len(self.password)
         scheme = self.scheme
         port = self.port if not (scheme == HTTPS and self.port == PORT_443) else ""
         timeout = self.timeout
         verify = self.verify
         vdom = self.vdom
         params = [
             f"{host=!r}",
             f"{username=!r}",
-            f"{password=!r}",
         ]
         params_optional = [
             f"{scheme=!r}" if scheme != HTTPS else "",
             f"{port=!r}" if port else "",
             f"{timeout=!r}" if timeout != TIMEOUT else "",
             f"{verify=!r}" if verify is True else "",
             f"{vdom=!r}" if vdom != VDOM else "",
         ]
         params.extend([s for s in params_optional if s])
         params_ = ", ".join([s for s in params if s])
         return f"{self.__class__.__name__}({params_})"
 
     def __enter__(self):
+        """Enter the runtime context related to this object."""
         self.login()
         return self
 
     def __exit__(self, *args):
+        """Exit the runtime context related to this object."""
         self.logout()
 
     # ============================= init =============================
 
+    def _init_port(self, **kwargs) -> int:
+        """Init port, 443 for "https", 80 for "http"."""
+        if port := int(kwargs.get("port") or 0):
+            return port
+        if self.scheme == "http":
+            return PORT_80
+        return PORT_443
+
     @staticmethod
     def _init_scheme(**kwargs) -> str:
-        """Init scheme "https" or "http" """
+        """Init scheme "https" or "http"."""
         scheme = str(kwargs.get("scheme") or HTTPS)
         expected = ["https", "http"]
         if scheme not in expected:
             raise ValueError(f"{scheme=}, {expected=}")
         return scheme
 
-    def _init_port(self, **kwargs) -> int:
-        """Init port, 443 for "https", 80 for "http" """
-        if port := int(kwargs.get("port") or 0):
-            return port
-        if self.scheme == "http":
-            return PORT_80
-        return PORT_443
+    def _init_token(self, **kwargs) -> str:
+        """Init token."""
+        token = str(kwargs.get("token") or "")
+        if not token:
+            return ""
+        if self.username:
+            raise ValueError("mutually excluded: username, token")
+        if self.password:
+            raise ValueError("mutually excluded: password, token")
+        return token
 
     # =========================== property ===========================
 
     @property
     def is_connected(self) -> bool:
-        """Check connection to the Fortigate
-        :return: True if session is connected to the Fortigate"""
+        """Check connection to the Fortigate.
+
+        ::
+            :return: True if session is connected to the Fortigate
+            :rtype: bool
+        """
         return isinstance(self._session, Session)
 
     @property
-    def url(self):
-        """Returns URL to the Fortigate"""
+    def url(self) -> str:
+        """Return URL to the Fortigate."""
         if self.port == 443:
             return f"{self.scheme}://{self.host}"
         return f"{self.scheme}://{self.host}:{self.port}"
 
     # ============================ login =============================
 
     def login(self) -> None:
-        """Login to the Fortigate using REST API
-        :return: self *Fortigate* object
+        """Login to the Fortigate using REST API, creates Session object.
+
+        ::
+            :return: None. Creates Session object
         """
         session: Session = requests.session()
+
+        # token
+        if self.token:
+            try:
+                response: Response = session.get(
+                    url=f"{self.url}/api/v2/cmdb/system/status",
+                    headers=self._bearer_token(),
+                    verify=self.verify,
+                )
+            except Exception as ex:
+                raise self._hide_secret_ex(ex)
+            response.raise_for_status()
+            self._session = session
+            return
+
+        # username
         try:
-            session.post(url=f"{self.url}/logincheck",
-                         data=urlencode([("username", self.username),
-                                         ("secretkey", self.password)]),
-                         timeout=self.timeout,
-                         verify=self.verify)
+            session.post(
+                url=f"{self.url}/logincheck",
+                data=urlencode([("username", self.username), ("secretkey", self.password)]),
+                timeout=self.timeout,
+                verify=self.verify,
+            )
         except Exception as ex:
             raise self._hide_secret_ex(ex)
 
         cookie_name = "ccsrftoken"
         cookies = [o for o in session.cookies if o and o.name == cookie_name]
         if not cookies:
             regex = cookie_name + r"_\d+$"
@@ -164,172 +207,224 @@
         cookies = [o for o in cookies if isinstance(o.value, str)]
         if not cookies:
             raise ValueError("invalid login credentials, absent cookie ccsrftoken")
         cookie = cookies[0]
         token = str(cookie.value).strip("\"")
         session.headers.update({"X-CSRFTOKEN": token})
 
-        response: Response = session.get(url=f"{self.url}/api/v2/cmdb/system/vdom")
+        response = session.get(url=f"{self.url}/api/v2/cmdb/system/vdom")
         response.raise_for_status()
         self._session = session
 
     def logout(self) -> None:
-        """Logout from the Fortigate using REST API"""
+        """Logout from the Fortigate using REST API, deletes Session object.
+
+        ::
+            :return: None. Deletes Session object
+        """
         if isinstance(self._session, Session):
-            try:
-                self._session.get(url=f"{self.url}/logout",
-                                  timeout=self.timeout,
-                                  verify=self.verify)
-            except SSLError:
-                pass
+            if not self.token:
+                try:
+                    self._session.get(url=f"{self.url}/logout",
+                                      timeout=self.timeout,
+                                      verify=self.verify)
+                except SSLError:
+                    pass
+            del self._session
         self._session = None
 
     # =========================== methods ============================
 
     def delete(self, url: str) -> Response:
-        """DELETE object from the Fortigate
-        :param url: REST API URL to the object
-        :return: Session response
-            *<Response [200]>* Object successfully deleted
-            *<Response [404]>* Object absent in the Fortigate
+        """DELETE object from the Fortigate.
+
+        ::
+            :param url: REST API URL to the object
+            :type url: str
+
+            :return: Session response
+                *<Response [200]>* Object successfully deleted
+                *<Response [404]>* Object absent in the Fortigate
+            :rtype: Response
         """
-        url = self._valid_url(url)
-        session: Session = self._get_session()
-        try:
-            response: Response = session.delete(url=url,
-                                                params=urlencode([("vdom", self.vdom)]),
-                                                timeout=self.timeout,
-                                                verify=self.verify)
-        except Exception as ex:
-            raise self._hide_secret_ex(ex)
+        response: Response = self._response("delete", url)
         if not response.ok:
             self._logging(response)
         return response
 
+    def directory(self, url: str) -> LDAny:
+        """Get directory schema of available REST API data source.
+
+        ::
+            :param url: REST API URL to the directory
+            :type url: str
+
+            :return: List of the Fortigate objects
+            :rtype: List[dict]
+        """
+        response: Response = self._response("get", url)
+        if not response.ok:
+            logging.info("code=%s, reason=%s, url=%s", response.status_code, response.reason, url)
+            return []
+        response_json = response.json()
+        results: LDAny = response_json.get("directory") or []
+        return results
+
     def exist(self, url: str) -> Response:
-        """Checks does an object exists in the Fortigate
-        :param url: REST API URL to the object
-        :return: Session response
-            *<Response [200]>* Object exist
-            *<Response [404]>* Object does not exist
+        """Check does an object exists in the Fortigate.
+
+        ::
+            :param url: REST API URL to the object
+            :type url: str
+
+            :return: Session response
+                *<Response [200]>* Object exist
+                *<Response [404]>* Object does not exist
+            :rtype: Response
         """
-        url = self._valid_url(url)
-        session: Session = self._get_session()
-        response: Response = session.get(url=url,
-                                         params=urlencode([("vdom", self.vdom)]),
-                                         timeout=self.timeout,
-                                         verify=self.verify)
-        return response
+        return self._response("get", url)
 
     def get(self, url: str) -> LDAny:
-        """GET object configured in the Fortigate
-        :param url: REST API URL to the object
-        :return: *List[dict_]* of the objects data
+        """GET object configured in the Fortigate.
+
+        ::
+            :param url: REST API URL to the object
+            :type url: str
+
+            :return: List of the Fortigate objects
+            :rtype: List[dict]
         """
-        url = self._valid_url(url)
-        session: Session = self._get_session()
-        try:
-            response: Response = session.get(url=url,
-                                             params=urlencode([("vdom", self.vdom)]),
-                                             timeout=self.timeout,
-                                             verify=self.verify)
-        except Exception as ex:
-            raise self._hide_secret_ex(ex)
+        response: Response = self._response("get", url)
         if not response.ok:
-            logging.info("code=%s, reason=%s, str_=%s", response.status_code, response.reason, url)
+            logging.info("code=%s, reason=%s, url=%s", response.status_code, response.reason, url)
             return []
-        result: LDAny = response.json()["results"]
-        return result
+        response_json = response.json()
+        results: LDAny = response_json.get("results") or []
+        return results
 
     def post(self, url: str, data: DAny) -> Response:
-        """POST (create) object in the Fortigate based on the data
-        :param url: REST API URL to the object
-        :param data: Data of the object
-        :return: Session response
-            *<Response [200]>* Object successfully created or already exists
-            *<Response [500]>* Object already exist in the Fortigate
+        """POST (create) object in the Fortigate based on the data.
+
+        ::
+            :param url: REST API URL to the object
+            :type url: str
+
+            :param data: Data of the object
+            :type data: dict
+
+            :return: Session response
+                *<Response [200]>* Object successfully created or already exists
+                *<Response [500]>* Object already exist in the Fortigate
+            :rtype: Response
         """
-        url = self._valid_url(url)
-        session: Session = self._get_session()
-        try:
-            response: Response = session.post(url=url,
-                                              params=urlencode([("vdom", self.vdom)]),
-                                              data=json.dumps(data),
-                                              timeout=self.timeout,
-                                              verify=self.verify)
-        except Exception as ex:
-            raise self._hide_secret_ex(ex)
+        response: Response = self._response("post", url, data)
         if not response.ok:
             self._logging(response)
         return response
 
     def put(self, url: str, data: DAny) -> Response:
-        """PUT (update) existing object in the Fortigate
-        :param url: REST API URL to the object
-        :param data: Data of the object
-        :return: Session response
-            *<Response [200]>* Object successfully updated
-            *<Response [404]>* Object has not been updated
+        """PUT (update) existing object in the Fortigate.
+
+        ::
+            :param url: REST API URL to the object
+            :type url: str
+
+            :param data: Data of the object
+            :type data: dict
+
+            :return: Session response
+                *<Response [200]>* Object successfully updated
+                *<Response [404]>* Object has not been updated
+            :rtype: Response
         """
-        url = self._valid_url(url)
-        session: Session = self._get_session()
-        try:
-            response: Response = session.put(url=url,
-                                             params=urlencode([("vdom", self.vdom)]),
-                                             data=json.dumps(data),
-                                             timeout=self.timeout,
-                                             verify=self.verify)
-        except Exception as ex:
-            raise self._hide_secret_ex(ex)
+        response: Response = self._response("put", url, data)
         if not response.ok:
             self._logging(response)
         return response
 
     # =========================== helpers ============================
 
+    def _bearer_token(self) -> DStr:
+        """Return bearer token."""
+        return {"Authorization": f"Bearer {self.token}"}
+
     def _get_session(self) -> Session:
-        """Returns an existing session or create a new one"""
+        """Return an existing session or create a new one."""
         if not self.is_connected:
             self.login()
         session = self._session
         if not isinstance(session, Session):
             raise TypeError(f"{session=} {Session} expected")
         return session
 
     def _logging(self, resp: Response) -> None:
-        """Logging response"""
+        """Log response."""
         code = resp.status_code
         reason = resp.reason
         url = self._hide_secret(string=resp.url)
         msg = f"{code=} {reason=} {url=}"
         logging.info(msg)
         if logging.getLogger().level <= logging.DEBUG:
             logging.debug("text=%s", resp.text)
 
     def _hide_secret(self, string: str) -> str:
-        """Hides password, secretkey in text (for safe logging)"""
+        """Hide password, secretkey in text (for safe logging)."""
         if not self.password:
             return string
         result = string.replace(self.password, "<hidden>")
-        quoted_password = str_.quote(self.password)
+        quoted_password = h.quote(self.password)
         result = result.replace(quoted_password, "<hidden>")
         return result
 
     def _hide_secret_ex(self, ex):
-        """Hides secretkey in exception (for safe logging)"""
+        """Hide secretkey in exception (for safe logging)."""
         if hasattr(ex, "args"):
             if (args := getattr(ex, "args")) and isinstance(args, Iterable):
                 msgs = []  # result
                 for arg in args:
                     if isinstance(arg, str):
                         msgs.append(self._hide_secret(string=arg))
                     else:
                         msgs.append(arg)
                 return type(ex)(tuple(msgs))
         return ex
 
+    def _response(self, method: Method, url: str, data: DAny = None) -> Response:
+        """Call Session method and return Response.
+
+        ::
+            :param method: Session method: "delete", "get", "post", "put"
+            :type method: str
+
+            :param url: REST API URL to the object
+            :type url: str
+
+            :param data: Data of the object
+
+            :return: Session response
+            :rtype: Response
+        """
+        params: DAny = dict(
+            url=self._valid_url(url),
+            params=urlencode([("vdom", self.vdom)]),
+            timeout=self.timeout,
+            verify=self.verify,
+        )
+        if isinstance(data, dict):
+            params["data"] = json.dumps(data)
+        if self.token:
+            params["headers"] = self._bearer_token()
+
+        session: Session = self._get_session()
+        method_: Callable = getattr(session, method)
+        try:
+            response: Response = method_(**params)
+        except Exception as ex:
+            raise self._hide_secret_ex(ex)
+        return response
+
     def _valid_url(self, url: str) -> str:
-        """Adds "https://" to `url`"""
+        """Add "https://" to `url` if absent."""
         if re.match("http(s)?://", url):
             return url
         url = url.strip("/")
         return f"{self.url}/{url}/"
```

### Comparing `fortigate_api-1.1.1/fortigate_api/fortigate_api.py` & `fortigate_api-1.2.2/fortigate_api/fortigate_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""fortigate-api"""
+"""**FortigateAPI** - a set of methods for working with the most commonly used objects."""
 
 from __future__ import annotations
 
 from fortigate_api.address import Address
 from fortigate_api.address_group import AddressGroup
 from fortigate_api.antivirus import Antivirus
 from fortigate_api.application import Application
 from fortigate_api.dhcp_server import DhcpServer
+from fortigate_api.external_resource import ExternalResource
 from fortigate_api.fortigate import Fortigate, VDOM
 from fortigate_api.interface import Interface
 from fortigate_api.internet_service import InternetService
 from fortigate_api.ip_pool import IpPool
 from fortigate_api.policy import Policy
 from fortigate_api.schedule import Schedule
 from fortigate_api.service import Service
@@ -19,93 +20,102 @@
 from fortigate_api.snmp_community import SnmpCommunity
 from fortigate_api.ssh import SSH
 from fortigate_api.virtual_ip import VirtualIP
 from fortigate_api.zone import Zone
 
 
 class FortigateAPI:
-    """**FortigateAPI** - a set of methods for working with the most commonly used objects"""
+    """**FortigateAPI** - a set of methods for working with the most commonly used objects."""
 
     def __init__(self, **kwargs):
-        """**FortigateAPI** - a set of methods for working with the most commonly used objects
-        :param host: Firewall ip address or hostname
-        :type host: str
+        """**FortigateAPI** - a set of methods for working with the most commonly used objects.
 
-        :param username: Administrator name
-        :type username: str
+        ::
+            :param host: Firewall ip address or hostname
+            :type host: str
 
-        :param password: Administrator password
-        :type password: str
+            :param username: Administrator name. Mutually exclusive with token
+            :type username: str
 
-        :param scheme: (optional) "https" (default) or "http"
-        :type scheme: str
+            :param password: Administrator password. Mutually exclusive with token
+            :type password: str
 
-        :param port: (optional) TCP port, by default 443 for "https", 80 for "http"
-        :type port: str
+            :param token: Administrator token. Mutually exclusive with username and password
+            :type token: str
 
-        :param timeout: (optional) Session timeout minutes (default 15)
-        :type timeout: int
+            :param scheme: (optional) "https" (default) or "http"
+            :type scheme: str
 
-        :param verify: (optional) Enable SSL certificate verification for HTTPS requests.
-            True -  enable
-            False - disable (default)
-        :type verify: bool
+            :param port: (optional) TCP port, by default 443 for "https", 80 for "http"
+            :type port: str
 
-        :param vdom: Name of virtual domain (default "root").
-            Used in REST API (Not used in SSH)
-        :type vdom: str
+            :param timeout: (optional) Session timeout minutes (default 15)
+            :type timeout: int
 
-        :param ssh: Netmiko ConnectHandler parameters
-        :type ssh: Dict[str, Any]
+            :param verify: (optional) Enable SSL certificate verification for HTTPS requests.
+                True -  enable
+                False - disable (default)
+            :type verify: bool
+
+            :param vdom: Name of virtual domain (default "root").
+                Used in REST API (Not used in SSH)
+            :type vdom: str
+
+            :param ssh: Netmiko ConnectHandler parameters
+            :type ssh: dict
         """
-        self.fgt = Fortigate(**kwargs)
+        self.rest = Fortigate(**kwargs)
         self.ssh = SSH(**kwargs)
 
-        self.address = Address(self.fgt)
-        self.address_group = AddressGroup(self.fgt)
-        self.antivirus = Antivirus(self.fgt)
-        self.application = Application(self.fgt)
-        self.dhcp_server = DhcpServer(self.fgt)
-        self.interface = Interface(self.fgt)
-        self.internet_service = InternetService(self.fgt)
-        self.ip_pool = IpPool(self.fgt)
-        self.policy = Policy(self.fgt)
-        self.schedule = Schedule(self.fgt)
-        self.service = Service(self.fgt)
-        self.service_category = ServiceCategory(self.fgt)
-        self.service_group = ServiceGroup(self.fgt)
-        self.snmp_community = SnmpCommunity(self.fgt)
-        self.virtual_ip = VirtualIP(self.fgt)
-        self.zone = Zone(self.fgt)
+        self.address = Address(self.rest)
+        self.address_group = AddressGroup(self.rest)
+        self.antivirus = Antivirus(self.rest)
+        self.application = Application(self.rest)
+        self.dhcp_server = DhcpServer(self.rest)
+        self.external_resource = ExternalResource(self.rest)
+        self.interface = Interface(self.rest)
+        self.internet_service = InternetService(self.rest)
+        self.ip_pool = IpPool(self.rest)
+        self.policy = Policy(self.rest)
+        self.schedule = Schedule(self.rest)
+        self.service = Service(self.rest)
+        self.service_category = ServiceCategory(self.rest)
+        self.service_group = ServiceGroup(self.rest)
+        self.snmp_community = SnmpCommunity(self.rest)
+        self.virtual_ip = VirtualIP(self.rest)
+        self.zone = Zone(self.rest)
 
     def __repr__(self):
-        return self.fgt.__repr__()
+        """Return a string representation related to this object."""
+        return self.rest.__repr__()
 
     def __enter__(self):
+        """Enter the runtime context related to this object."""
         return self
 
     def __exit__(self, *args):
-        self.fgt.__exit__()
+        """Exit the runtime context related to this object."""
+        self.rest.__exit__()
         self.ssh.__exit__()
 
     # =========================== methods ============================
 
     def login(self) -> FortigateAPI:
-        """Login to the Fortigate using REST API """
-        self.fgt.login()
+        """Login to the Fortigate using REST API."""
+        self.rest.login()
         return self
 
     def logout(self) -> None:
-        """Logout from the Fortigate using REST API"""
-        self.fgt.logout()
+        """Logout from the Fortigate using REST API."""
+        self.rest.logout()
 
     @property
     def vdom(self) -> str:
         """ACE TCP/UDP ports."""
-        return self.fgt.vdom
+        return self.rest.vdom
 
     @vdom.setter
     def vdom(self, vdom: str) -> None:
         vdom = str(vdom)
         if not vdom:
             vdom = VDOM
-        self.fgt.vdom = vdom
+        self.rest.vdom = vdom
```

### Comparing `fortigate_api-1.1.1/fortigate_api/interface.py` & `fortigate_api-1.2.2/fortigate_api/interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,43 @@
-"""Interface Object"""
+"""Interface Object."""
 
-from fortigate_api import dict_
+from fortigate_api import helpers as h
 from fortigate_api.base import Base
 from fortigate_api.types_ import LDAny
 
 
 class Interface(Base):
-    """Interface Object"""
+    """Interface Object."""
 
-    def __init__(self, fgt):
-        super().__init__(fgt=fgt, url_obj="api/v2/cmdb/system/interface/")
+    def __init__(self, rest):
+        """Interface Object.
+
+        ::
+            :param rest: Fortigate REST API connector
+            :type rest: Fortigate
+        """
+        super().__init__(rest=rest, url_obj="api/v2/cmdb/system/interface/")
 
     # noinspection PyIncorrectDocstring
     def get(self, **kwargs) -> LDAny:
-        """Gets interface-objects in specified vdom, all or filtered by some of params
-        :param str uid: Filters interface-object by unique identifier. Used to get a single object
-        :param list filter: Filters interface-objects by one or multiple conditions: equals "==",
-            not equals "!=", contains "=@". Used to get multiple objects
-        :param bool all: Gets all interface-objects from all vdom
-        :return: *List[dict_]* List of interface-objects
+        """Get interface-objects in specified vdom, all or filtered by some of params.
+
+        ::
+            :param uid: Filters interface-object by unique identifier. Used to get a single object
+            :type uid: str
+
+            :param filter: Filters interface-objects by one or multiple conditions: equals "==",
+                not equals "!=", contains "=@". Used to get multiple objects
+            :type filter: str or List[str]
+
+            :param all: Gets all interface-objects from all vdom
+            :type all: bool
+
+            :return: List of interface-objects
+            :rtype: List[dict]
         """
         if kwargs.get("all"):
-            dict_.pop_quoted(key="all", data=kwargs)
+            h.pop_quoted(key="all", data=kwargs)
             return super().get(**kwargs)
         interfaces = super().get(**kwargs)
-        interfaces = [d for d in interfaces if d["vdom"] == self.fgt.vdom]
+        interfaces = [d for d in interfaces if d["vdom"] == self.rest.vdom]
         return interfaces
```

### Comparing `fortigate_api-1.1.1/fortigate_api/policy.py` & `fortigate_api-1.2.2/fortigate_api/policy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,91 @@
-"""Policy Object"""
+"""Policy Object."""
 
 from requests import Response
 
-from fortigate_api import str_
+from fortigate_api import helpers as h
 from fortigate_api.base import Base
 from fortigate_api.extended_filters import wrapp_efilters
 from fortigate_api.types_ import DAny
 from fortigate_api.types_ import LDAny, StrInt
 
 
 class Policy(Base):
-    """Policy Object"""
+    """Policy Object."""
 
-    def __init__(self, fgt):
-        super().__init__(fgt=fgt, url_obj="api/v2/cmdb/firewall/policy/", uid_key="policyid")
+    def __init__(self, rest):
+        """Policy Object.
+
+        ::
+            :param rest: Fortigate REST API connector
+            :type rest: Fortigate
+        """
+        super().__init__(rest=rest, url_obj="api/v2/cmdb/firewall/policy/", uid_key="policyid")
 
     # noinspection PyIncorrectDocstring
     @wrapp_efilters
     def get(self, **kwargs) -> LDAny:
-        """Gets fortigate-objects, all or filtered by some of params.
+        """Get fortigate-objects, all or filtered by some of params.
+
         Need to use only one of params
-        :param int uid: Filters fortigate-object by identifier. Used to get a single object
-        :param list filter: Filters fortigate-objects by one or multiple conditions: equals "==",
-            not equals "!=", contains "=@". Used to get multiple objects
-        :param str efilter: Extended filter: "srcaddr", "dstaddr" by condition: equals "==",
-            not equals "!=",  supernets ">=", subnets "<="
-        :return: *List[dict_]* List of the fortigate-objects
+        ::
+            :param uid: Filters fortigate-object by identifier. Used to get a single object
+            :type uid: str or int
+
+            :param filter: Filters fortigate-objects by one or multiple conditions: equals "==",
+                not equals "!=", contains "=@". Used to get multiple objects
+            :type filter: str or List[str]
+
+            :param efilter: Extended filter: "srcaddr", "dstaddr" by condition: equals "==",
+                not equals "!=",  supernets ">=", subnets "<="
+            :type efilter: str or List[str]
+
+            :return: List of the fortigate-objects
+            :rtype: List[dict]
         """
         return super().get(**kwargs)
 
     def move(self, uid: StrInt, position: str, neighbor: StrInt) -> Response:
-        """Move policy to before/after other neighbor-policy
-        :param uid: Identifier of policy being moved
-        :param position: "before" or "after" neighbor
-        :param neighbor: Policy will be moved near to this neighbor-policy
-        :return: Session response
-            *<Response [200]>* Policy successfully moved
-            *<Response [500]>* Policy has not been moved
+        """Move policy to before/after other neighbor-policy.
+
+        ::
+            :param uid: Identifier of policy being moved
+            :type uid: str or int
+
+            :param position: "before" or "after" neighbor
+            :type position: str
+
+            :param neighbor: Policy will be moved near to this neighbor-policy
+            :type neighbor: str or int
+
+            :return: Session response
+                *<Response [200]>* Policy successfully moved
+                *<Response [500]>* Policy has not been moved
+            :rtype: Response
         """
-        kwargs = dict(action="move", username=self.fgt.username, secretkey=self.fgt.password)
+        kwargs = dict(action="move", username=self.rest.username, secretkey=self.rest.password)
         kwargs[position] = neighbor
         url = f"{self.url_}{uid}"
-        url = str_.make_url(url, **kwargs)
-        return self.fgt.put(url=url, data={})
+        url = h.make_url(url, **kwargs)
+        return self.rest.put(url=url, data={})
 
     def update(self, data: DAny, uid: StrInt = "") -> Response:
-        """Updates policy-object in the Fortigate
-        :param data: Data of the policy-object
-        :param uid:  Policyid of the policy-object,
-            taken from the `uid` parameter or from data["policyid"]
-        :return: Session response
-            *<Response [200]>* Object successfully updated
-            *<Response [404]>* Object has not been updated
+        """Update policy-object in the Fortigate.
+
+        ::
+            :param data: Data of the policy-object
+            :type data: dict
+
+            :param uid:  Policyid of the policy-object,
+                taken from the `uid` parameter or from data["policyid"]
+            :type uid: str or int
+
+            :return: Session response
+                *<Response [200]>* Object successfully updated
+                *<Response [404]>* Object has not been updated
+            :rtype: Response
         """
         if not uid:
             uid = data.get("policyid") or ""
             if not uid:
                 raise ValueError(f"absent {uid=} and data[\"policyid\"]")
         return self._update(uid=uid, data=data)
```

### Comparing `fortigate_api-1.1.1/fortigate_api/snmp_community.py` & `fortigate_api-1.2.2/fortigate_api/snmp_community.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,41 @@
-"""SNMP Community Object"""
+"""SNMP Community Object."""
 
 from requests import Response
 
 from fortigate_api.base import Base
 from fortigate_api.types_ import DAny, StrInt
 
 
 class SnmpCommunity(Base):
-    """SNMP Community Object"""
+    """SNMP Community Object."""
 
-    def __init__(self, fgt):
-        super().__init__(fgt=fgt, url_obj="api/v2/cmdb/system.snmp/community/", uid_key="id")
+    def __init__(self, rest):
+        """SNMP Community Object.
+
+        ::
+            :param rest: Fortigate REST API connector
+            :type rest: Fortigate
+        """
+        super().__init__(rest=rest, url_obj="api/v2/cmdb/system.snmp/community/", uid_key="id")
 
     def update(self, data: DAny, uid: StrInt = "") -> Response:
-        """Updates snmp-community-object, where `uid` is data["id"]
-        :param data: Data of the snmp-community-object
-        :param uid: ID of the snmp-community-object,
-            taken from the `uid` parameter or from data["id"]
-        :return: Session response
-            *<Response [200]>* Object successfully updated
-            *<Response [404]>* Object has not been updated
+        """Update snmp-community-object, where `uid` is data["id"].
+
+        ::
+            :param data: Data of the snmp-community-object
+            :type data: dict
+
+            :param uid: ID of the snmp-community-object,
+                taken from the `uid` parameter or from data["id"]
+            :type uid: str or int
+
+            :return: Session response
+                *<Response [200]>* Object successfully updated
+                *<Response [404]>* Object has not been updated
+            :rtype: Response
         """
         if not uid:
             uid = data.get("id") or ""
             if not uid:
                 raise ValueError(f"absent {uid=} and data[\"id\"]")
         return self._update(uid=uid, data=data)
```

### Comparing `fortigate_api-1.1.1/fortigate_api/ssh.py` & `fortigate_api-1.2.2/fortigate_api/ssh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,106 @@
 """SSH connector to the Fortigate.
-Contains methods to get and put configuration commands using ssh
+
+Contains methods to get and put configuration commands using ssh.
 """
 
 from netmiko import ConnectHandler  # type: ignore
 
 from fortigate_api.types_ import DAny, UStr
 
 
 class SSH:
     """SSH connector to the Fortigate.
-    Contains methods to get and put configuration commands using ssh
+
+    Contains methods to get and put configuration commands using ssh.
     """
 
-    def __init__(self, host: str, username: str, password: str, **kwargs):
-        """SSH
-        :param host: Firewall ip address or hostname
-        :type host: str
+    def __init__(self, host: str, username: str = "", password: str = "", **kwargs):
+        """SSH connector to the Fortigate.
+
+        ::
+            :param host: Firewall ip address or hostname
+            :type host: str
 
-        :param username: Administrator name
-        :type username: str
+            :param username: Administrator name
+            :type username: str
 
-        :param password: Administrator password
-        :type password: str
+            :param password: Administrator password
+            :type password: str
 
-        :param ssh: Netmiko *ConnectHandler* parameters
-        :type ssh: Dict[str, Any]
+            :param ssh: Netmiko *ConnectHandler* parameters
+            :type ssh: Dict[str, Any]
         """
         ssh_kwargs: DAny = dict(kwargs.get("ssh") or {})
         ssh_kwargs.update(dict(
             device_type="fortinet",
             auto_connect=False,
         ))
         self.session = ConnectHandler(host=host,
                                       username=username,
                                       password=password,
                                       **ssh_kwargs)
 
     def __enter__(self):
+        """Enter the runtime context related to this object."""
         self.login()
         return self
 
     def __exit__(self, *args):
+        """Exit the runtime context related to this object."""
         self.logout()
 
     # ============================ login =============================
 
     def login(self) -> None:
-        """Login to Fortigate using SSH"""
+        """Login to Fortigate using SSH."""
         if self.session.remote_conn:
             return
         # noinspection PyProtectedMember
         self.session._open()
         if not self.session.remote_conn:
             raise ConnectionError("Cannot open remote connection")
 
     def logout(self) -> None:
-        """Logout from the Fortigate using SSH"""
+        """Logout from the Fortigate using SSH."""
         if self.session.remote_conn:
             self.session.cleanup()
             self.session.remote_conn = None
 
     # =========================== methods ============================
 
     def send_command(self, cmd: str, **kwargs) -> str:
-        """Sends the command to the Fortigate
-        :param cmd: The command to be executed on the Fortigate
-        :type cmd: str
+        """Send the command to the Fortigate.
 
-        :param kwargs: (optional) Netmiko parameters
-        :type kwargs: Dict[str, Any]
+        ::
+            :param cmd: The command to be executed on the Fortigate
+            :type cmd: str
 
-        :return: Output of the command
-        :rtype: str
+            :param kwargs: (optional) Netmiko parameters
+            :type kwargs: Dict[str, Any]
+
+            :return: Output of the command
+            :rtype: str
         """
         self.login()
         output = self.session.send_command(cmd, **kwargs)
         return str(output)
 
     def send_config_set(self, cmds: UStr, **kwargs) -> str:
-        """Sends configuration commands to the Fortigate
-        :param cmds: Configuration commands to be executed on the Fortigate
-        :type cmds: List[str], str
+        """Send configuration commands to the Fortigate.
+
+        ::
+            :param cmds: Configuration commands to be executed on the Fortigate
+            :type cmds: List[str], str
 
-        :param kwargs: (optional) Netmiko parameters
-        :type kwargs: Dict[str, Any]
+            :param kwargs: (optional) Netmiko parameters
+            :type kwargs: Dict[str, Any]
 
-        :return: Output of the commands
-        :rtype: str
+            :return: Output of the commands
+            :rtype: str
         """
         self.login()
         if isinstance(cmds, str):
             cmds = [cmds]
         cmds_ = list(cmds)
 
         output = self.session.send_config_set(cmds_, **kwargs)
```

### Comparing `fortigate_api-1.1.1/fortigate_api/types_.py` & `fortigate_api-1.2.2/fortigate_api/types_.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-"""Typing"""
+"""Types."""
 
+from datetime import date
 from ipaddress import IPv4Network
-from typing import Any, Dict, Iterable, List, Set, Tuple, Union
+from pathlib import Path
+from typing import Any, Dict, Iterable, List, Literal, Set, Tuple, Union
 
 from requests import Response
 
 DAny = Dict[str, Any]
 DStr = Dict[str, str]
 IStr = Iterable[str]
+LPath = List[Path]
 LResponse = List[Response]
 LStr = List[str]
+Method = Literal["delete", "get", "post", "put"]
+SDate = Set[date]
 SStr = Set[str]
 StrInt = Union[str, int]
 T2Str = Tuple[str, str]
 T3Str = Tuple[str, str, str]
 
 DDAny = Dict[str, DAny]
 DLInet = Dict[str, List[IPv4Network]]
```

### Comparing `fortigate_api-1.1.1/fortigate_api.egg-info/PKG-INFO` & `fortigate_api-1.2.2/fortigate_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fortigate-api
-Version: 1.1.1
+Version: 1.2.2
 Summary: Python package to configure Fortigate (Fortios) devices using REST API and SSH
 Author-email: Vladimir Prusakov <vladimir.prusakovs@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Repository, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/fortigate-api/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.1.1.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 Keywords: fortigate,api,fortios,firewall,networking,telecommunication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: License :: OSI Approved :: MIT License
@@ -28,28 +28,29 @@
 .. image:: https://img.shields.io/pypi/v/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/pypi/pyversions/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/github/last-commit/vladimirs-git/fortigate-api
    :target: https://pypi.python.org/pypi/fortigate-api
 
+
 fortigate-api
 =============
 
 Python package to configure Fortigate (Fortios) devices using REST API and SSH.
 With this package, you can change objects in the Fortigate. The most commonly used `Objects`_
 are implemented in the `FortigateAPI`_ methods, but you can manipulate any other objects
 that can be accessed through the REST API using the `Fortigate`_ methods.
 You can also get and change the Fortigate configuration through SSH.
 
 Main features:
 
-- REST API to create, delete, get, update objects. Move policy before, after other policy.
-- SSH Netmiko connector to work with CLI commands.
-- CiscoConfParse to search and modify commands in config.
+- REST API to create, delete, get, update objects. Move policy before, after other policy
+- Session-based (user, password) and Token-based authentication
+- SSH Netmiko connector to work with CLI commands
 - Usage examples in `./examples`_
 
 ----------------------------------------------------------------------------------------------------
 
 .. contents:: **Contents**
     :local:
 
@@ -70,15 +71,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.1.1.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
 
@@ -89,138 +90,168 @@
 -------
 The objects implemented in `FortigateAPI`_.
 To get an idea of the objects, you can change the *hostname* in the following URLs and
 look it in the Fortigate web management interface. The first URL is for the Web GUI, the second
 one is for the REST API. Not all object implemented in `FortigateAPI`_ (only the most used by me),
 access to any other objects is available via `Fortigate`_.
 
-=================== ================================================================================
-Object              GUI and REST API URL to the object, FortiOS v6.4
-=================== ================================================================================
-`Address`_          https://hostname/ng/firewall/address
+===================== ==============================================================================
+Object                GUI and REST API URL to the object (FortiOS v6.4)
+===================== ==============================================================================
+`Address`_            https://hostname/ng/firewall/address
+
+                      https://hostname/api/v2/cmdb/firewall/address/
 
-                    https://hostname/api/v2/cmdb/firewall/address/
+`AddressGroup`_       https://hostname/ng/firewall/address
 
-`AddressGroup`_     https://hostname/ng/firewall/address
+                      https://hostname/api/v2/cmdb/firewall/addrgrp/
 
-                    https://hostname/api/v2/cmdb/firewall/addrgrp/
+`Antivirus`_          https://hostname/ng/utm/antivirus/profile
 
-`Antivirus`_        https://hostname/ng/utm/antivirus/profile
+                      https://hostname/api/v2/cmdb/antivirus/profile/
 
-                    https://hostname/api/v2/cmdb/antivirus/profile/
+`Application`_        https://hostname/ng/utm/appctrl/sensor
 
-`Application`_      https://hostname/ng/utm/appctrl/sensor
+                      https://hostname/api/v2/cmdb/application/list/
 
-                    https://hostname/api/v2/cmdb/application/list/
+`DhcpServer`_         https://hostname/ng/interface/edit/{name}
 
-`DhcpServer`_       https://hostname/ng/interface/edit/{name}
+                      https://hostname/api/v2/cmdb/system.dhcp/server/
 
-                    https://hostname/api/v2/cmdb/system.dhcp/server/
+`ExternalResource`_   https://hostname/ng/external-connector
 
-`Interface`_        https://hostname/ng/interface
+                      https://hostname/api/v2/cmdb/system/external-resource/
 
-                    https://hostname/api/v2/cmdb/system/interface/
+`Interface`_          https://hostname/ng/interface
 
-`InternetService`_  https://hostname/ng/firewall/internet_service
+                      https://hostname/api/v2/cmdb/system/interface/
 
-                    https://hostname/api/v2/cmdb/firewall/internet-service/
+`InternetService`_    https://hostname/ng/firewall/internet_service
 
-`IpPool`_           https://hostname/ng/firewall/ip-pool
+                      https://hostname/api/v2/cmdb/firewall/internet-service/
 
-                    https://hostname/api/v2/cmdb/firewall/ippool/
+`IpPool`_             https://hostname/ng/firewall/ip-pool
 
-`Policy`_           https://hostname/ng/firewall/policy/policy/standard
+                      https://hostname/api/v2/cmdb/firewall/ippool/
 
-                    https://hostname/api/v2/cmdb/firewall/policy/
+`Policy`_             https://hostname/ng/firewall/policy/policy/standard
 
-`Schedule`_         https://hostname/ng/firewall/schedule
+                      https://hostname/api/v2/cmdb/firewall/policy/
 
-                    https://hostname/api/v2/cmdb/firewall.schedule/onetime/
+`Schedule`_           https://hostname/ng/firewall/schedule
 
-`Service`_          https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.schedule/onetime/
 
-                    https://hostname/api/v2/cmdb/firewall.service/custom/
+`Service`_            https://hostname/ng/firewall/service
 
-`ServiceCategory`_  https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.service/custom/
 
-                    https://hostname/api/v2/cmdb/firewall.service/category/
+`ServiceCategory`_    https://hostname/ng/firewall/service
 
-`ServiceGroup`_     https://hostname/ng/firewall/service
+                      https://hostname/api/v2/cmdb/firewall.service/category/
 
-                    https://hostname/api/v2/cmdb/firewall.service/group/
+`ServiceGroup`_       https://hostname/ng/firewall/service
 
-`SnmpCommunity`_    https://hostname/ng/system/snmp
+                      https://hostname/api/v2/cmdb/firewall.service/group/
 
-                    https://hostname/api/v2/cmdb/system.snmp/community/
+`SnmpCommunity`_      https://hostname/ng/system/snmp
 
-`VirtualIp`_        https://hostname/ng/firewall/virtual-ip
+                      https://hostname/api/v2/cmdb/system.snmp/community/
 
-                    https://hostname/api/v2/cmdb/firewall/vip/
+`VirtualIp`_          https://hostname/ng/firewall/virtual-ip
 
-`Zone`_             https://hostname/ng/interface
+                      https://hostname/api/v2/cmdb/firewall/vip/
 
-                    https://hostname/api/v2/cmdb/system/zone/
-=================== ================================================================================
+`Zone`_               https://hostname/ng/interface
+
+                      https://hostname/api/v2/cmdb/system/zone/
+===================== ==============================================================================
 
 
 ----------------------------------------------------------------------------------------------------
 
 FortigateAPI
 ------------
 **FortigateAPI(host, username, password, scheme, port, timeout, vdom)**
 Set of methods for working with the most commonly used `Objects`_.
-Code usage examples in *./examples/examples.py*
 
 =============== ======= ============================================================================
 Parameter        Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
-username        *str*   Administrator name
-password        *str*   Administrator password
+username        *str*   Administrator name. Mutually exclusive with token
+password        *str*   Administrator password. Mutually exclusive with token
+token           *str*   Administrator token. Mutually exclusive with username and password
 scheme          *str*   (optional) "https" (default) or "http"
 port            *int*   (optional) TCP port, by default 443 for "https", 80 for "http"
 timeout         *int*   (optional) Session timeout minutes (default 15)
 verify          *str*   (optional) Enable SSL certificate verification for HTTPS requests. True -  enable, False - disable (default)
 vdom            *str*   Name of virtual domain (default "root")
 =============== ======= ============================================================================
 
 
 ----------------------------------------------------------------------------------------------------
 
 Address
 -------
+Python examples `./examples/address.py`_
+
+Python examples `./examples/address_token.py`_
+
 FortiOS v6.4 data example `./examples/yml/address.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create address
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.252",
+            "type": "ipmask"}
+    response = fgt.address.create(data)
+
+    # Get all addresses
+    addresses_all = fgt.address.get()
+
+    # Get address by name
+    addresses_by_name = fgt.address.get(uid="ADDRESS")
+
+    # Get address by operator contains \"=@\"
+    addresses_contains = fgt.address.get(filter="subnet=@127.0")
+
 
 create()
 ........
 **FortigateAPI.address.create(data)**
-Creates address-object in the Fortigate.
+Create address-object in the Fortigate.
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the address-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
 **FortigateAPI.address.delete(uid, filter)**
-Deletes address-object from the Fortigate.
+Delete address-object from the Fortigate.
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*               Unique identifier. Name of the address-object. Used to delete a single object
-filter          *str*, *List[str]*  Filters address-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters address-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -266,68 +297,70 @@
 uid             *str*   Name of the address-object, taken from the `uid` parameter or from data["name"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
+----------------------------------------------------------------------------------------------------
 
-Address examples:
+AddressGroup
+------------
+Python examples `./examples/address_group.py`_
 
-- Creates address in the Fortigate
-- Gets all addresses from the Fortigate
-- Gets filtered address by name (unique identifier)
-- Filters address by operator *equals* "=="
-- Filters address by operator *contains* "=@"
-- Filters address by operator *not equals* "!="
-- Updates address data in the Fortigate
-- Checks for presence of address in the Fortigate
-- Deletes address from the Fortigate by name
-- Deletes addresses from the Fortigate by filter
-- Checks for absence of address in the Fortigate
-- FortigateAPI *with* statement
+FortiOS v6.4 data example `./examples/yml/address_group.yml`_
 
-`./examples/address.py`_
+.. code:: python
 
+    from fortigate_api import FortigateAPI
 
-----------------------------------------------------------------------------------------------------
+    fgt = FortigateAPI(host="host", username="username", password="password")
 
-AddressGroup
-------------
-FortiOS v6.4 data example `./examples/yml/address_group.yml`_
+    # Create address and address-group in the Fortigate
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.255",
+            "type": "ipmask"}
+    fgt.address.create(data)
+    data = {"name": "ADDR_GROUP", "member": [{"name": "ADDRESS"}]}
+    fgt.address_group.create(data)
+
+    # Get all address-groups from the Fortigate
+    address_groups_all = fgt.address_group.get()
+
+    # Get filtered address_group by name (unique identifier)
+    address_groups_name = fgt.address_group.get(uid="ADDR_GROUP")
 
 
 create()
 ........
 **FortigateAPI.address_group.create(data)**
-Creates address-group-object in the Fortigate
+Create address-group-object in the Fortigate
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the address-group-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
 **FortigateAPI.address_group.delete(uid, filter)**
-Deletes address-group-object from the Fortigate
+Delete address-group-object from the Fortigate
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*               Name of the address-group-object (unique identifier). Used to delete a single object
-filter          *str*, *List[str]*  Filters address-group-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters address-group-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -373,33 +406,14 @@
 uid             *str*   Name of the address-group-object, taken from the `uid` parameter or from data["name"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-AddressGroup examples:
-
-- Creates address-group in the Fortigate
-- Gets all address-groups from the Fortigate
-- Gets filtered address-group by name (unique identifier)
-- Filters address-group by operator *equals* "=="
-- Filters address-group by operator *contains* "=@"
-- Filters address-group by operator *not equals* "!="
-- Updates address-group data in the Fortigate
-- Checks for presence of address-group in the Fortigate
-- Deletes address-group from the Fortigate by name
-- Deletes address-groups from the Fortigate by filter
-- Checks for absence of address-group in the Fortigate
-
-`./examples/address_group.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Antivirus
 ---------
 **Antivirus** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/antivirus.yml`_
@@ -436,37 +450,95 @@
 
 ----------------------------------------------------------------------------------------------------
 
 DhcpServer
 ----------
 **DhcpServer** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/dhcp_server.py`_
+
 FortiOS v6.4 data example `./examples/yml/dhcp_server.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create dhcp server
+    data = {
+        "default-gateway": "192.168.255.1",
+        "netmask": "255.255.255.0",
+        "interface": "vlan.123",
+        "ip-range": [{"start-ip": "192.168.255.2", "end-ip": "192.168.255.254", }],
+    }
+    fgt.dhcp_server.create(data)
+
+    # Get all dhcp servers
+    dhcp_servers = fgt.dhcp_server.get()
+
+
 **FortigateAPI.dhcp_server.create(data)** Note, in Fortigate is possible to create multiple DHCP servers with the same settings, you need control duplicates
 
 **FortigateAPI.dhcp_server.delete(uid, filter)**
 
 **FortigateAPI.dhcp_server.get(uid, filter)**
 
 **FortigateAPI.dhcp_server.is_exist(uid)**
 
 **FortigateAPI.dhcp_server.update(data, uid)**
 
-DhcpServer examples `./examples/dhcp_server.py`_
+
+----------------------------------------------------------------------------------------------------
+
+ExternalResource
+----------------
+**ExternalResource** object has the same parameters and methods as `Address`_
+
+Python examples `./examples/external_resource.py`_
+
+FortiOS v6.4 data example `./examples/yml/external_resource.yml`_
+
+**FortigateAPI.external_resource.create(data)**
+
+**FortigateAPI.external_resource.delete(uid, filter)**
+
+**FortigateAPI.external_resource.get(uid, filter)**
+
+**FortigateAPI.external_resource.is_exist(uid)**
+
+**FortigateAPI.external_resource.update(data, uid)**
+
 
 
 ----------------------------------------------------------------------------------------------------
 
 Interface
 ---------
 **Interface** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/interface.py`_
+
 FortiOS v6.4 data example `./examples/yml/interface.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+
+    # Get all interfaces in vdom \"root\" from the Fortigate
+    interfaces = fgt.interface.get()
+    print(f"interfaces count={len(interfaces)}")  # interfaces count=21
+
+    # Gets filtered interface by name (unique identifier)
+    interfaces = fgt.interface.get(uid="dmz")
+
+
 **FortigateAPI.interface.create(data)**
 
 **FortigateAPI.interface.delete(uid, filter)**
 
 
 get()
 .....
@@ -485,31 +557,14 @@
     *List[dict]* List of interface-objects
 
 **FortigateAPI.interface.is_exist(uid)**
 
 **FortigateAPI.interface.update(data, uid)**
 
 
-Examples
-........
-Interface examples:
-
-- Gets all interfaces in vdom "root" from the Fortigate
-- Gets filtered interface by name (unique identifier)
-- Filters interface by operator *equals* "=="
-- Filters interface by operator contains "=@"
-- Filters interface by operator *not equals* "!="
-- Filters interface by multiple conditions
-- Updates interface data in the Fortigate
-- Checks for presence of interface in the Fortigate
-- Gets all interfaces in vdom "VDOM"
-
-`./examples/interface.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 InternetService
 ---------------
 **InternetService** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/internet_service.yml`_
@@ -527,66 +582,91 @@
 
 ----------------------------------------------------------------------------------------------------
 
 IpPool
 ------
 **IpPool** object has the same parameters and methods as `Address`_
 
+Python examples `./examples/ip_pool.py`_
+
 FortiOS v6.4 data example `./examples/yml/ip_pool.yml`_
 
 **FortigateAPI.ip_pool.create(data)**
 
 **FortigateAPI.ip_pool.delete(uid, filter)**
 
 **FortigateAPI.ip_pool.get(uid, filter)**
 
 **FortigateAPI.ip_pool.is_exist(uid)**
 
 **FortigateAPI.ip_pool.update(data, uid)**
 
 
-Examples
-........
-IpPool examples:
-
-`./examples/ip_pool.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Policy
 ------
+Python examples `./examples/policy.py`_
+
+Python examples `./examples/policy_extended_filter.py`_
+
 FortiOS v6.4 data example `./examples/yml/policy.yml`_
 
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt = FortigateAPI(host="host", username="username", password="password")
+
+    # Create policy in the Fortigate
+    data = dict(
+        name="POLICY",
+        status="enable",
+        action="accept",
+        srcintf=[{"name": "any"}],
+        dstintf=[{"name": "any"}],
+        srcaddr=[{"name": "all"}],
+        dstaddr=[{"name": "all"}],
+        service=[{"name": "ALL"}],
+        schedule="always",
+    )
+    fgt.policy.create(data)
+
+    # Get all policies from the Fortigate
+    policies_all = fgt.policy.get()
+
+    # Filters policies by name, by operator equals
+    policies_name = fgt.policy.get(filter="name==POLICY")
+
 
 create()
 ........
 **FortigateAPI.policy.create(data)**
-Creates policy-object in the Fortigate
+Create policy-object in the Fortigate
 
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 data            *dict*  Data of the policy-object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully created or already exists, *<Response [500]>* Object has not been created in the Fortigate
 
 
 delete()
 ........
-Deletes policy-object from the Fortigate
+Delete policy-object from the Fortigate
 Only one of the parameters *uid* or *filter* can be used in the same time.
 
 =============== =================== ================================================================
 Parameter       Type                Description
 =============== =================== ================================================================
 uid             *str*, *int*        Identifier of the policy-object. Used to delete a single object
-filter          *str*, *List[str]*  Filters policy-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than returns *<Response [200]>*
+filter          *str*, *List[str]*  Filters policy-objects by one or multiple conditions: equals "==", not equals "!=", contains "=@". Used to delete multiple objects. *Response* with the highest *status_code* (most important error) will be returned. If no address-objects was found and deleted than return *<Response [200]>*
 =============== =================== ================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully deleted, *<Response [404]>* Object absent in the Fortigate
 
 
 get()
@@ -649,46 +729,14 @@
 uid             *int*   Policyid of the policy-object, taken from the `uid` parameter or from data["policyid"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-Policy examples:
-
-- Creates policy in the Fortigate
-- Gets all policies from the Fortigate
-- Gets filtered policy by policyid (unique identifier)
-- Filters policies by name, by operator *equals* "=="
-- Filters policies by operator *contains* "=@"
-- Filters policies by operator *not equals* "!="
-- Updates policy data in the Fortigate
-- Checks for presence of policy in the Fortigate
-- Gets all policies with destination address == "192.168.1.2/32"
-- Deletes policy from the Fortigate by policyid (unique identifier)
-- Deletes policies from the Fortigate by filter (by name)
-- Checks for absence of policy in the Fortigate
-
-`./examples/policy.py`_
-
-
-Policy Extended Filter examples:
-
-- Gets the rules where source prefix is equals 127.0.1.0/30
-- Gets the rules where source prefix is not equals 127.0.1.0/30
-- Gets the rules where source addresses are in subnets of 127.0.1.0/24
-- Gets the rules where source prefixes are supernets of address 127.0.1.1/32
-- Gets the rules where source prefix are equals 127.0.1.0/30 and destination prefix are equals 127.0.2.0/30
-- Delete policy, address-group, addresses from the Fortigate (order is important)
-
-`./examples/policy_extended_filter.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 Schedule
 --------
 **Schedule** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/schedule.yml`_
@@ -763,14 +811,16 @@
 
 ----------------------------------------------------------------------------------------------------
 
 SnmpCommunity
 -------------
 **SnmpCommunity**
 
+Python examples `./examples/snmp_community.py`_
+
 FortiOS v6.4 data example `./examples/yml/snmp_community.yml`_
 
 **FortigateAPI.snmp_community.create(data)**
 
 **FortigateAPI.snmp_community.delete(uid, filter)**
 
 **FortigateAPI.snmp_community.get(uid, filter)**
@@ -787,19 +837,14 @@
 uid             *str*   Name of the snmp-community-object, taken from the `uid` parameter or from data["id"]
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-SnmpCommunity examples `./examples/snmp_community.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 VirtualIP
 ---------
 **VirtualIP** object has the same parameters and methods as `Address`_
 
 FortiOS v6.4 data example `./examples/yml/virtual_ip.yml`_
@@ -839,20 +884,42 @@
 Fortigate
 ---------
 **Fortigate(host, username, password, scheme, port, timeout, vdom)**
 REST API connector to the Fortigate. Contains generic methods (get, put, delete, etc.)
 to work with any objects available through the REST API. `Fortigate`_ is useful for working with
 objects that are not implemented in `FortigateAPI`_
 
+Python examples `./examples/fortigate.py`_
+
+Python examples `./examples/fortigate_token.py`_
+
+.. code:: python
+
+    from fortigate_api import Fortigate
+
+    fgt = Fortigate(host="host", username="username", password="password")
+
+    # Create address in the Fortigate
+    data = {"name": "ADDRESS",
+            "obj-type": "ip",
+            "subnet": "127.0.0.100 255.255.255.252",
+            "type": "ipmask"}
+    fgt.post(url="api/v2/cmdb/firewall/address/", data=data)
+
+    # Get address data from the Fortigate
+    addresses_all = fgt.get(url="api/v2/cmdb/firewall/address/")
+
+
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
-username        *str*   Administrator name
-password        *str*   Administrator password
+username        *str*   Administrator name. Mutually exclusive with token
+password        *str*   Administrator password. Mutually exclusive with token
+token           *str*   Administrator token. Mutually exclusive with username and password
 scheme          *str*   (optional) "https" (default) or "http"
 port            *int*   (optional) TCP port, by default 443 for "https", 80 for "http"
 timeout         *int*   (optional) Session timeout minutes (default 15)
 verify          *str*   (optional) Enable SSL certificate verification for HTTPS requests. True -  enable, False - disable (default)
 vdom            *str*   Name of virtual domain (default "root")
 =============== ======= ============================================================================
 
@@ -935,38 +1002,45 @@
 data            *dict*  Data of the object
 =============== ======= ============================================================================
 
 Return
     Session response. *<Response [200]>* Object successfully updated, *<Response [404]>* Object has not been updated
 
 
-Examples
-........
-Fortigate examples:
-
-- Creates address in the Fortigate
-- Gets address data from the Fortigate
-- Updates address data in the Fortigate
-- Checks for presence of address in the Fortigate
-- Deletes address from the Fortigate
-- Checks for absence of address in the Fortigate
-- Fortigate *with* statement
-
-`./examples/fortigate.py`_
-
-
 ----------------------------------------------------------------------------------------------------
 
 SSH
 ---
 **SSH(host, username, password, ssh)**
 SSH connector to the Fortigate. Contains methods to get and put configuration commands using ssh.
 Note, FortigateAPI parameter "vdom" used in REST API only and not used in SSH.
 In order to send cli commands to a specific vdom, you need "config vdom" before.
 
+Python examples `./examples/ssh.py`_
+
+Python examples `./examples/ssh_vdom.py`_
+
+.. code:: python
+
+    from fortigate_api import FortigateAPI
+
+    fgt_api = FortigateAPI(host="host", username="username", password="password")
+    fgt_api.ssh.login()
+
+    # Show interface config
+    config = fgt_api.ssh.send_command("show system interface dmz")
+
+    # Change interface description from "dmz" to "DMZ"
+    cmds = ["config system interface",
+            "edit dmz",
+            "set description DMZ",
+            "end"]
+    output = fgt_api.ssh.send_config_set(cmds)
+
+
 =============== ======= ============================================================================
 Parameter       Type    Description
 =============== ======= ============================================================================
 host            *str*   Firewall ip address or hostname
 username        *str*   Administrator name
 password        *str*   Administrator password
 ssh             *dict*  Netmiko *ConnectHandler* parameters
@@ -1008,79 +1082,44 @@
 cmds            *List[str]*   Configuration commands to be executed on the Fortigate
 kwargs          *dict*        (optional) Netmiko parameters
 =============== ============= ======================================================================
 
 Return
     Output of the commands
 
-
-Examples
-........
-SSH examples:
-
-- Show interface config
-- Change interface description from "dmz" to "DMZ"
-- Check interface description is changed
-- Change read-timeout timer for long awaited commands
-
-`./examples/ssh.py`_
-
-SSH examples for working with vdom:
-
-- get system arp from interfaces associated with vdom="VDOM"
-- get system arp from interfaces associated with vdom="root"
-
-`./examples/ssh_vdom.py`_
-
 ----------------------------------------------------------------------------------------------------
 
-CiscoConfParse
---------------
-Helper that parses the Fortigate configuration to find and modify command lines.
-CiscoConfParse doesn't natively support Fortigate configuration,
-but after some tweaking in this package it has become a good tool to play with Fortigate config lines.
-For more information, see the documentation for the JunosCfgLine object at https://github.com/mpenning/ciscoconfparse
-
-
-Examples
-........
-CiscoConfParse examples:
-
-- get config from the Fortigate by SSH
-- create CiscoConfParse object
-- filter all JunosCfgLine objects of wan interfaces
-- print some data in CiscoConfParse objects
-- filter all wan interfaces blocks
-
-`./examples/ccp.py`_
-
 
 .. _`./examples`: ./examples
+.. _`./examples/yml`: ./examples/yml
 .. _`./examples/yml/address.yml`: ./examples/yml/address.yml
 .. _`./examples/yml/address_group.yml`: ./examples/yml/address_group.yml
 .. _`./examples/yml/antivirus.yml`: ./examples/yml/antivirus.yml
 .. _`./examples/yml/application.yml`: ./examples/yml/application.yml
 .. _`./examples/yml/dhcp_server.yml`: ./examples/yml/dhcp_server.yml
+.. _`./examples/yml/external_resource.yml`: ./examples/yml/external_resource.yml
 .. _`./examples/yml/interface.yml`: ./examples/yml/interface.yml
 .. _`./examples/yml/internet_service.yml`: ./examples/yml/internet_service.yml
 .. _`./examples/yml/ip_pool.yml`: ./examples/yml/ip_pool.yml
 .. _`./examples/yml/policy.yml`: ./examples/yml/policy.yml
 .. _`./examples/yml/schedule.yml`: ./examples/yml/schedule.yml
 .. _`./examples/yml/service.yml`: ./examples/yml/service.yml
 .. _`./examples/yml/service_category.yml`: ./examples/yml/service_category.yml
 .. _`./examples/yml/service_group.yml`: ./examples/yml/service_group.yml
 .. _`./examples/yml/snmp_community.yml`: ./examples/yml/snmp_community.yml
 .. _`./examples/yml/virtual_ip.yml`: ./examples/yml/virtual_ip.yml
 .. _`./examples/yml/zone.yml`: ./examples/yml/zone.yml
 
 .. _`./examples/address.py`: ./examples/address.py
+.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/address_group.py`: ./examples/address_group.py
-.. _`./examples/ccp.py`: ./examples/ccp.py
 .. _`./examples/dhcp_server.py`: ./examples/dhcp_server.py
+.. _`./examples/external_resource.py`: ./examples/external_resource.py
 .. _`./examples/fortigate.py`: ./examples/fortigate.py
+.. _`./examples/fortigate_token.py`: ./examples/fortigate_token.py
 .. _`./examples/interface.py`: ./examples/interface.py
 .. _`./examples/ip_pool.py`: ./examples/ip_pool.py
 .. _`./examples/policy.py`: ./examples/policy.py
 .. _`./examples/policy_extended_filter.py`: ./examples/policy_extended_filter.py
 .. _`./examples/snmp_community.py`: ./examples/snmp_community.py
 .. _`./examples/ssh.py`: ./examples/ssh.py
 .. _`./examples/ssh_vdom.py`: ./examples/ssh_vdom.py
```

### Comparing `fortigate_api-1.1.1/fortigate_api.egg-info/SOURCES.txt` & `fortigate_api-1.2.2/fortigate_api.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 fortigate_api/address.py
 fortigate_api/address_group.py
 fortigate_api/antivirus.py
 fortigate_api/application.py
 fortigate_api/base.py
 fortigate_api/ccp.py
 fortigate_api/dhcp_server.py
-fortigate_api/dict_.py
 fortigate_api/extended_filters.py
+fortigate_api/external_resource.py
 fortigate_api/fortigate.py
 fortigate_api/fortigate_api.py
 fortigate_api/helpers.py
 fortigate_api/interface.py
 fortigate_api/internet_service.py
 fortigate_api/ip_pool.py
 fortigate_api/policy.py
 fortigate_api/py.typed
 fortigate_api/schedule.py
 fortigate_api/service.py
 fortigate_api/service_category.py
 fortigate_api/service_group.py
 fortigate_api/snmp_community.py
 fortigate_api/ssh.py
-fortigate_api/str_.py
 fortigate_api/types_.py
 fortigate_api/virtual_ip.py
 fortigate_api/zone.py
 fortigate_api.egg-info/PKG-INFO
 fortigate_api.egg-info/SOURCES.txt
 fortigate_api.egg-info/dependency_links.txt
 fortigate_api.egg-info/requires.txt
```

### Comparing `fortigate_api-1.1.1/pyproject.toml` & `fortigate_api-1.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "fortigate_api"
-version = "1.1.1"
+version = "1.2.2"
 authors = [
   { name="Vladimir Prusakov", email="vladimir.prusakovs@gmail.com" },
 ]
 description = "Python package to configure Fortigate (Fortios) devices using REST API and SSH"
 readme = "README.rst"
 license = { text="MIT" }
 requires-python = ">=3.8"
 dependencies = [
-    "requests ~= 2.28",
-    "netmiko ~= 4.1",
-    "ciscoconfparse ~= 1.7",
+    "requests >= 2.28",
+    "netmiko >= 4.1",
+    "ciscoconfparse >= 1.7",
 ]
 keywords = ["fortigate", "api", "fortios", "firewall", "networking", "telecommunication"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Telecommunications Industry",
@@ -27,21 +27,24 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
 ]
 [project.urls]
 "Homepage" = "https://github.com/vladimirs-git/fortigate-api"
 "Repository" = "https://github.com/vladimirs-git/fortigate-api"
 "Bug Tracker" = "https://github.com/vladimirs-git/fortigate-api/issues"
-"Download URL" = "https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.1.1.tar.gz"
+"Download URL" = "https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz"
 [tool.setuptools.packages.find]
 include = ["fortigate_api"]
 [tool.setuptools.package-data]
 fortigate_api = ["py.typed"]
 [project.optional-dependencies]
 dev = [
-    "mypy < 1",
+    "dictdiffer == 0.9.0",
+    "mypy == 0.982",
+    "pydocstyle == 6.3.0",
     "pylint == 2.13.9",
-    "pytest ~= 7.2",
-    "restructuredtext-lint ~= 1.4",
-    "twine ~= 4.0",
-    "types-requests ~= 2.28"
+    "pytest == 7.2.0",
+    "pytest-cov == 4.0.0",
+    "restructuredtext-lint == 1.4.0",
+    "twine == 4.0.1",
+    "types-requests == 2.28.11.2",
 ]
```

