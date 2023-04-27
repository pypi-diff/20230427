# Comparing `tmp/fortigate_api-1.2.1.tar.gz` & `tmp/fortigate_api-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate_api-1.2.1.tar", last modified: Wed Apr 26 12:09:22 2023, max compression
+gzip compressed data, was "fortigate_api-1.2.2.tar", last modified: Thu Apr 27 05:53:27 2023, max compression
```

## Comparing `fortigate_api-1.2.1.tar` & `fortigate_api-1.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 12:09:22.441627 fortigate_api-1.2.1/
--rw-rw-rw-   0        0        0     1091 2022-07-14 18:32:10.000000 fortigate_api-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0    44303 2023-04-26 12:09:22.440626 fortigate_api-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    43039 2023-04-26 12:08:03.000000 fortigate_api-1.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-26 12:09:22.432627 fortigate_api-1.2.1/fortigate_api/
--rw-rw-rw-   0        0        0      182 2023-04-22 19:54:39.000000 fortigate_api-1.2.1/fortigate_api/__init__.py
--rw-rw-rw-   0        0        0      371 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/address.py
--rw-rw-rw-   0        0        0      394 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/address_group.py
--rw-rw-rw-   0        0        0      380 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/antivirus.py
--rw-rw-rw-   0        0        0      387 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/application.py
--rw-rw-rw-   0        0        0     8427 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/base.py
--rw-rw-rw-   0        0        0     9884 2023-04-22 19:54:39.000000 fortigate_api-1.2.1/fortigate_api/ccp.py
--rw-rw-rw-   0        0        0     1851 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/dhcp_server.py
--rw-rw-rw-   0        0        0     7997 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/extended_filters.py
--rw-rw-rw-   0        0        0      418 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/external_resource.py
--rw-rw-rw-   0        0        0    15110 2023-04-25 09:56:56.000000 fortigate_api-1.2.1/fortigate_api/fortigate.py
--rw-rw-rw-   0        0        0     4494 2023-04-24 14:18:26.000000 fortigate_api-1.2.1/fortigate_api/fortigate_api.py
--rw-rw-rw-   0        0        0     9009 2023-04-22 19:54:39.000000 fortigate_api-1.2.1/fortigate_api/helpers.py
--rw-rw-rw-   0        0        0     1456 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/interface.py
--rw-rw-rw-   0        0        0      415 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/internet_service.py
--rw-rw-rw-   0        0        0      369 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/ip_pool.py
--rw-rw-rw-   0        0        0     3266 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/policy.py
--rw-rw-rw-   0        0        0        0 2022-07-14 18:32:10.000000 fortigate_api-1.2.1/fortigate_api/py.typed
--rw-rw-rw-   0        0        0      384 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/schedule.py
--rw-rw-rw-   0        0        0      378 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/service.py
--rw-rw-rw-   0        0        0      415 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/service_category.py
--rw-rw-rw-   0        0        0      400 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/service_group.py
--rw-rw-rw-   0        0        0     1315 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/snmp_community.py
--rw-rw-rw-   0        0        0     3347 2023-04-22 19:54:39.000000 fortigate_api-1.2.1/fortigate_api/ssh.py
--rw-rw-rw-   0        0        0      731 2023-04-22 19:54:39.000000 fortigate_api-1.2.1/fortigate_api/types_.py
--rw-rw-rw-   0        0        0      378 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/virtual_ip.py
--rw-rw-rw-   0        0        0      354 2023-04-24 14:23:05.000000 fortigate_api-1.2.1/fortigate_api/zone.py
-drwxrwxrwx   0        0        0        0 2023-04-26 12:09:22.439627 fortigate_api-1.2.1/fortigate_api.egg-info/
--rw-rw-rw-   0        0        0    44303 2023-04-26 12:09:22.000000 fortigate_api-1.2.1/fortigate_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      968 2023-04-26 12:09:22.000000 fortigate_api-1.2.1/fortigate_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 12:09:22.000000 fortigate_api-1.2.1/fortigate_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2023-04-26 12:09:22.000000 fortigate_api-1.2.1/fortigate_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 12:09:22.000000 fortigate_api-1.2.1/fortigate_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1749 2023-04-26 12:08:03.000000 fortigate_api-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 12:09:22.441627 fortigate_api-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      113 2023-04-22 19:54:40.000000 fortigate_api-1.2.1/setup.py
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

### Comparing `fortigate_api-1.2.1/LICENSE.txt` & `fortigate_api-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/PKG-INFO` & `fortigate_api-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fortigate_api
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package to configure Fortigate (Fortios) devices using REST API and SSH
 Author-email: Vladimir Prusakov <vladimir.prusakovs@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Repository, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/fortigate-api/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.1.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 Keywords: fortigate,api,fortios,firewall,networking,telecommunication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: License :: OSI Approved :: MIT License
@@ -71,15 +71,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.1.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
```

### Comparing `fortigate_api-1.2.1/README.rst` & `fortigate_api-1.2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.1.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
```

### Comparing `fortigate_api-1.2.1/fortigate_api/base.py` & `fortigate_api-1.2.2/fortigate_api/base.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/ccp.py` & `fortigate_api-1.2.2/fortigate_api/ccp.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/dhcp_server.py` & `fortigate_api-1.2.2/fortigate_api/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/extended_filters.py` & `fortigate_api-1.2.2/fortigate_api/extended_filters.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/fortigate.py` & `fortigate_api-1.2.2/fortigate_api/fortigate.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/fortigate_api.py` & `fortigate_api-1.2.2/fortigate_api/fortigate_api.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/helpers.py` & `fortigate_api-1.2.2/fortigate_api/helpers.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/interface.py` & `fortigate_api-1.2.2/fortigate_api/interface.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/policy.py` & `fortigate_api-1.2.2/fortigate_api/policy.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/snmp_community.py` & `fortigate_api-1.2.2/fortigate_api/snmp_community.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/ssh.py` & `fortigate_api-1.2.2/fortigate_api/ssh.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api/types_.py` & `fortigate_api-1.2.2/fortigate_api/types_.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/fortigate_api.egg-info/PKG-INFO` & `fortigate_api-1.2.2/fortigate_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fortigate-api
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package to configure Fortigate (Fortios) devices using REST API and SSH
 Author-email: Vladimir Prusakov <vladimir.prusakovs@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Repository, https://github.com/vladimirs-git/fortigate-api
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/fortigate-api/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.1.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 Keywords: fortigate,api,fortios,firewall,networking,telecommunication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: License :: OSI Approved :: MIT License
@@ -71,15 +71,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.1.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
```

### Comparing `fortigate_api-1.2.1/fortigate_api.egg-info/SOURCES.txt` & `fortigate_api-1.2.2/fortigate_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.1/pyproject.toml` & `fortigate_api-1.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "fortigate_api"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Vladimir Prusakov", email="vladimir.prusakovs@gmail.com" },
 ]
 description = "Python package to configure Fortigate (Fortios) devices using REST API and SSH"
 readme = "README.rst"
 license = { text="MIT" }
 requires-python = ">=3.8"
 dependencies = [
-    "requests == 2.28.*",
-    "netmiko == 4.1.*",
-    "ciscoconfparse == 1.7.*",
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
@@ -27,23 +27,24 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
 ]
 [project.urls]
 "Homepage" = "https://github.com/vladimirs-git/fortigate-api"
 "Repository" = "https://github.com/vladimirs-git/fortigate-api"
 "Bug Tracker" = "https://github.com/vladimirs-git/fortigate-api/issues"
-"Download URL" = "https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.1.tar.gz"
+"Download URL" = "https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.2.tar.gz"
 [tool.setuptools.packages.find]
 include = ["fortigate_api"]
 [tool.setuptools.package-data]
 fortigate_api = ["py.typed"]
 [project.optional-dependencies]
 dev = [
     "dictdiffer == 0.9.0",
     "mypy == 0.982",
     "pydocstyle == 6.3.0",
     "pylint == 2.13.9",
     "pytest == 7.2.0",
+    "pytest-cov == 4.0.0",
     "restructuredtext-lint == 1.4.0",
     "twine == 4.0.1",
     "types-requests == 2.28.11.2",
 ]
```

