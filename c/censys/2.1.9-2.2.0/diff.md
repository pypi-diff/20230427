# Comparing `tmp/censys-2.1.9.tar.gz` & `tmp/censys-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys-2.1.9.tar", max compression
+gzip compressed data, was "censys-2.2.0.tar", max compression
```

## Comparing `censys-2.1.9.tar` & `censys-2.2.0.tar`

### file list

```diff
@@ -1,52 +1,50 @@
--rw-r--r--   0        0        0    10174 2022-10-21 19:04:42.251354 censys-2.1.9/LICENSE
--rw-r--r--   0        0        0     3889 2022-10-21 19:04:42.251354 censys-2.1.9/README.md
--rw-r--r--   0        0        0       91 2022-10-21 19:04:42.251354 censys-2.1.9/censys/__main__.py
--rw-r--r--   0        0        0      566 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/__init__.py
--rw-r--r--   0        0        0     3474 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/api.py
--rw-r--r--   0        0        0      341 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/assets/__init__.py
--rw-r--r--   0        0        0     5900 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/assets/assets.py
--rw-r--r--   0        0        0      424 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/assets/certificates.py
--rw-r--r--   0        0        0     1118 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/assets/domains.py
--rw-r--r--   0        0        0      389 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/assets/hosts.py
--rw-r--r--   0        0        0     2075 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/assets/subdomains.py
--rw-r--r--   0        0        0     1493 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/client.py
--rw-r--r--   0        0        0     2380 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/clouds.py
--rw-r--r--   0        0        0     2519 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/events.py
--rw-r--r--   0        0        0     2482 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/inventory.py
--rw-r--r--   0        0        0      150 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/risks/__init__.py
--rw-r--r--   0        0        0     1827 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/risks/v1.py
--rw-r--r--   0        0        0     3990 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/risks/v2.py
--rw-r--r--   0        0        0     2784 2022-10-21 19:04:42.251354 censys-2.1.9/censys/asm/seeds.py
--rw-r--r--   0        0        0      569 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/__init__.py
--rw-r--r--   0        0        0     1901 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/args.py
--rw-r--r--   0        0        0      174 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/__init__.py
--rw-r--r--   0        0        0     2045 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/account.py
--rw-r--r--   0        0        0     6795 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/asm.py
--rw-r--r--   0        0        0     3171 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/config.py
--rw-r--r--   0        0        0     5526 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/hnri.py
--rw-r--r--   0        0        0     7492 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/search.py
--rw-r--r--   0        0        0     3319 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/subdomains.py
--rw-r--r--   0        0        0     2570 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/commands/view.py
--rw-r--r--   0        0        0     4402 2022-10-21 19:04:42.251354 censys-2.1.9/censys/cli/utils.py
--rw-r--r--   0        0        0      105 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/__init__.py
--rw-r--r--   0        0        0     7435 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/base.py
--rw-r--r--   0        0        0     1690 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/config.py
--rw-r--r--   0        0        0     1106 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/deprecation.py
--rw-r--r--   0        0        0    12264 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/exceptions.py
--rw-r--r--   0        0        0      144 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/types.py
--rw-r--r--   0        0        0      453 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/utils.py
--rw-r--r--   0        0        0      242 2022-10-21 19:04:42.251354 censys-2.1.9/censys/common/version.py
--rw-r--r--   0        0        0        0 2022-10-21 19:04:42.251354 censys-2.1.9/censys/py.typed
--rw-r--r--   0        0        0      375 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/__init__.py
--rw-r--r--   0        0        0     2090 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/client.py
--rw-r--r--   0        0        0      169 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v1/__init__.py
--rw-r--r--   0        0        0     5805 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v1/api.py
--rw-r--r--   0        0        0     1655 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v1/certificates.py
--rw-r--r--   0        0        0     1224 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v1/data.py
--rw-r--r--   0        0        0      151 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v2/__init__.py
--rw-r--r--   0        0        0    17311 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v2/api.py
--rw-r--r--   0        0        0     4325 2022-10-21 19:04:42.251354 censys-2.1.9/censys/search/v2/certs.py
--rw-r--r--   0        0        0     8013 2022-10-21 19:04:42.255354 censys-2.1.9/censys/search/v2/hosts.py
--rw-r--r--   0        0        0     3272 2022-10-21 19:04:42.255354 censys-2.1.9/pyproject.toml
--rw-r--r--   0        0        0     5070 1970-01-01 00:00:00.000000 censys-2.1.9/setup.py
--rw-r--r--   0        0        0     6453 1970-01-01 00:00:00.000000 censys-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-04-27 15:38:12.948205 censys-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3893 2023-04-27 15:38:12.948205 censys-2.2.0/README.md
+-rw-r--r--   0        0        0       91 2023-04-27 15:38:12.948205 censys-2.2.0/censys/__main__.py
+-rw-r--r--   0        0        0      633 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/__init__.py
+-rw-r--r--   0        0        0     3474 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/api.py
+-rw-r--r--   0        0        0      410 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/__init__.py
+-rw-r--r--   0        0        0     5900 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/assets.py
+-rw-r--r--   0        0        0      424 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/certificates.py
+-rw-r--r--   0        0        0     1118 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/domains.py
+-rw-r--r--   0        0        0      389 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/hosts.py
+-rw-r--r--   0        0        0     2075 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/subdomains.py
+-rw-r--r--   0        0        0     1775 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/assets/web_entities.py
+-rw-r--r--   0        0        0     1598 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/client.py
+-rw-r--r--   0        0        0     2380 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/clouds.py
+-rw-r--r--   0        0        0     2519 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/events.py
+-rw-r--r--   0        0        0     2482 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/inventory.py
+-rw-r--r--   0        0        0     3981 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/risks.py
+-rw-r--r--   0        0        0     2784 2023-04-27 15:38:12.948205 censys-2.2.0/censys/asm/seeds.py
+-rw-r--r--   0        0        0      569 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/args.py
+-rw-r--r--   0        0        0      174 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2045 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/account.py
+-rw-r--r--   0        0        0     6793 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/asm.py
+-rw-r--r--   0        0        0     3171 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/config.py
+-rw-r--r--   0        0        0     5526 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/hnri.py
+-rw-r--r--   0        0        0     5356 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/search.py
+-rw-r--r--   0        0        0     3439 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/subdomains.py
+-rw-r--r--   0        0        0     3760 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/commands/view.py
+-rw-r--r--   0        0        0     3279 2023-04-27 15:38:12.948205 censys-2.2.0/censys/cli/utils.py
+-rw-r--r--   0        0        0      105 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/__init__.py
+-rw-r--r--   0        0        0     7435 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/base.py
+-rw-r--r--   0        0        0     1690 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/config.py
+-rw-r--r--   0        0        0     1106 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/deprecation.py
+-rw-r--r--   0        0        0    12264 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/exceptions.py
+-rw-r--r--   0        0        0      144 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/types.py
+-rw-r--r--   0        0        0      453 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/utils.py
+-rw-r--r--   0        0        0      242 2023-04-27 15:38:12.948205 censys-2.2.0/censys/common/version.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:38:12.948205 censys-2.2.0/censys/py.typed
+-rw-r--r--   0        0        0      375 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/__init__.py
+-rw-r--r--   0        0        0     2133 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/client.py
+-rw-r--r--   0        0        0      169 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/__init__.py
+-rw-r--r--   0        0        0     5805 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/api.py
+-rw-r--r--   0        0        0     1830 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/certificates.py
+-rw-r--r--   0        0        0     1224 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v1/data.py
+-rw-r--r--   0        0        0      151 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/__init__.py
+-rw-r--r--   0        0        0    17201 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/api.py
+-rw-r--r--   0        0        0    12750 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/certs.py
+-rw-r--r--   0        0        0    10570 2023-04-27 15:38:12.948205 censys-2.2.0/censys/search/v2/hosts.py
+-rw-r--r--   0        0        0     3298 2023-04-27 15:38:12.952205 censys-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 censys-2.2.0/PKG-INFO
```

### Comparing `censys-2.1.9/LICENSE` & `censys-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/README.md` & `censys-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Censys Python Library
 
 [![PyPI](https://img.shields.io/pypi/v/censys?color=orange&logo=pypi&logoColor=orange)](https://pypi.org/project/censys/)
-[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue?logo=python)](https://www.python.org/downloads/)
+[![Python Version](https://img.shields.io/badge/python-3.7.2%2B-blue?logo=python)](https://www.python.org/downloads/)
 [![Read the Docs (version)](https://img.shields.io/readthedocs/censys-python/latest?logo=read%20the%20docs)](https://censys-python.readthedocs.io/en/stable/?badge=stable)
 [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-brightgreen?logo=github)](https://github.com/censys/censys-python/discussions)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-organge.svg?logo=git&logoColor=organge)](http://makeapullrequest.com)
 [![License](https://img.shields.io/github/license/censys/censys-python?logo=apache)](https://github.com/censys/censys-python/blob/main/LICENSE)
 
-An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7+ is currently supported.
+An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7.2+ is currently supported.
 
 > **Notice:** The Censys Search v1 endpoints are deprecated as of Nov. 30, 2021. Please begin using v2 endpoints to query hosts and certificates and check out our [support center](https://support.censys.io/hc/en-us/sections/360013076551-Censys-Search-2-0) for resources.
 
 ## Features
 
 - [Search Censys data](https://censys-python.readthedocs.io/en/stable/usage-v2.html)
 - [Bulk Certificate lookups](https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk)
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # Censys Python Library [![PyPI](https://img.shields.io/pypi/v/
 censys?color=orange&logo=pypi&logoColor=orange)](https://pypi.org/project/
-censys/) [![Python Version](https://img.shields.io/badge/python-3.7%2B-
+censys/) [![Python Version](https://img.shields.io/badge/python-3.7.2%2B-
 blue?logo=python)](https://www.python.org/downloads/) [![Read the Docs
 (version)](https://img.shields.io/readthedocs/censys-python/
 latest?logo=read%20the%20docs)](https://censys-python.readthedocs.io/en/stable/
 ?badge=stable) [![GitHub Discussions](https://img.shields.io/badge/GitHub-
 Discussions-brightgreen?logo=github)](https://github.com/censys/censys-python/
 discussions) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-
 organge.svg?logo=git&logoColor=organge)](http://makeapullrequest.com) [!
 [License](https://img.shields.io/github/license/censys/censys-
 python?logo=apache)](https://github.com/censys/censys-python/blob/main/LICENSE)
 An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https:/
-/censys.io/)). Python 3.7+ is currently supported. > **Notice:** The Censys
+/censys.io/)). Python 3.7.2+ is currently supported. > **Notice:** The Censys
 Search v1 endpoints are deprecated as of Nov. 30, 2021. Please begin using v2
 endpoints to query hosts and certificates and check out our [support center]
 (https://support.censys.io/hc/en-us/sections/360013076551-Censys-Search-2-0)
 for resources. ## Features - [Search Censys data](https://censys-
 python.readthedocs.io/en/stable/usage-v2.html) - [Bulk Certificate lookups]
 (https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk) - [Download
 Bulk Data](https://censys-python.readthedocs.io/en/stable/usage-v1.html#data) -
```

### Comparing `censys-2.1.9/censys/asm/api.py` & `censys-2.2.0/censys/asm/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/assets/assets.py` & `censys-2.2.0/censys/asm/assets/assets.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/assets/domains.py` & `censys-2.2.0/censys/asm/assets/domains.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/assets/subdomains.py` & `censys-2.2.0/censys/asm/assets/subdomains.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/client.py` & `censys-2.2.0/censys/asm/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """Interact with the Censys Seeds, Assets, and Logbook APIs."""
 from typing import Optional
 
-from .assets import CertificatesAssets, DomainsAssets, HostsAssets, SubdomainsAssets
+from .assets import (
+    CertificatesAssets,
+    DomainsAssets,
+    HostsAssets,
+    SubdomainsAssets,
+    WebEntitiesAssets,
+)
 from .clouds import Clouds
 from .events import Events
 from .inventory import InventorySearch
-from .risks import Risksv2
+from .risks import Risks
 from .seeds import Seeds
 
 
 class AsmClient:
     """Client ASM API class."""
 
     def __init__(self, api_key: Optional[str] = None, **kwargs):
@@ -21,16 +27,17 @@
         """
         self.seeds = Seeds(api_key, **kwargs)
         self.hosts = HostsAssets(api_key, **kwargs)
         self.certificates = CertificatesAssets(api_key, **kwargs)
         self.domains = DomainsAssets(api_key, **kwargs)
         self.events = Events(api_key, **kwargs)
         self.clouds = Clouds(api_key, **kwargs)
-        self.risks = Risksv2(api_key, **kwargs)
+        self.risks = Risks(api_key, **kwargs)
         self.inventory = InventorySearch(api_key, **kwargs)
+        self.web_entities = WebEntitiesAssets(api_key, **kwargs)
 
         # Save the arguments for parameterized client usage
         self.__api_kwargs = kwargs
 
     def get_subdomains(self, domain: str):
         """Get an API instance for subdomains of the parent domain.
```

### Comparing `censys-2.1.9/censys/asm/clouds.py` & `censys-2.2.0/censys/asm/clouds.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/events.py` & `censys-2.2.0/censys/asm/events.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/inventory.py` & `censys-2.2.0/censys/asm/inventory.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/asm/risks/v2.py` & `censys-2.2.0/censys/asm/risks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Interact with the Censys Risks v2 API."""
+"""Interact with the Censys Risks API."""
 from typing import List, Optional
 
-from ..api import CensysAsmAPI
+from .api import CensysAsmAPI
 
 
-class Risksv2(CensysAsmAPI):
-    """Risks v2 API class."""
+class Risks(CensysAsmAPI):
+    """Risks API class."""
 
     base_path = "/v2/risk"
     risk_instances_path = f"{base_path}-instances"
     risk_types_path = f"{base_path}-types"
 
     def get_risk_instances(
         self, include_events: Optional[bool] = None, accept: Optional[str] = None
```

### Comparing `censys-2.1.9/censys/asm/seeds.py` & `censys-2.2.0/censys/asm/seeds.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/cli/__init__.py` & `censys-2.2.0/censys/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/cli/args.py` & `censys-2.2.0/censys/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/cli/commands/account.py` & `censys-2.2.0/censys/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/cli/commands/asm.py` & `censys-2.2.0/censys/cli/commands/asm.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     if added_count < to_add_count:
         console.print(f"Seeds not added: {to_add_count - added_count}")
         if args.verbose:  # pragma: no cover
             console.print(
                 "The following seed(s) were not able to be added as they already exist or are reserved."
             )
             for seed in seeds_to_add:
-                if not any([s for s in added_seeds if seed["value"] == s["value"]]):
+                if not any(s for s in added_seeds if seed["value"] == s["value"]):
                     console.print_json(seed)
 
 
 def include(parent_parser: argparse._SubParsersAction, parents: dict):
     """Include this subcommand into the parent parser.
 
     Args:
```

### Comparing `censys-2.1.9/censys/cli/commands/config.py` & `censys-2.2.0/censys/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/cli/commands/hnri.py` & `censys-2.2.0/censys/cli/commands/hnri.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/cli/commands/subdomains.py` & `censys-2.2.0/censys/cli/commands/subdomains.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from censys.cli.utils import console, err_console
 from censys.common.exceptions import (
     CensysException,
     CensysRateLimitExceededException,
     CensysUnauthorizedException,
 )
-from censys.search import CensysCertificates
+from censys.search import CensysCerts
 
 
 def print_subdomains(subdomains: Set[str], as_json: bool = False):
     """Print subdomains.
 
     Args:
         subdomains (Set[str]): Subdomains.
@@ -31,32 +31,31 @@
     """Subdomain subcommand.
 
     Args:
         args: Argparse Namespace.
     """
     subdomains = set()
     try:
-        client = CensysCertificates(api_id=args.api_id, api_secret=args.api_secret)
-        certificate_query = f"parsed.names: {args.domain}"
+        client = CensysCerts(api_id=args.api_id, api_secret=args.api_secret)
+        certificate_query = f"names: {args.domain}"
 
         with err_console.status(f"Querying {args.domain} subdomains"):
-            certificates_search_results = client.search(
-                certificate_query, fields=["parsed.names"], max_records=args.max_records
-            )
+            query = client.search(certificate_query, fields=["names"], pages=args.pages)
 
             # Flatten the result, and remove duplicates
-            for search_result in certificates_search_results:
-                new_subdomains: List[str] = search_result.get("parsed.names", [])
-                subdomains.update(
-                    [
-                        subdomain
-                        for subdomain in new_subdomains
-                        if subdomain.endswith(args.domain)
-                    ]
-                )
+            for hits in query:
+                for cert in hits:
+                    new_subdomains: List[str] = cert.get("names", [])
+                    subdomains.update(
+                        [
+                            subdomain
+                            for subdomain in new_subdomains
+                            if subdomain.endswith(args.domain)
+                        ]
+                    )
 
         # Don't make console prints if we're in json mode
         if not args.json:
             if len(subdomains) == 0:
                 err_console.print(f"No subdomains found for {args.domain}")
                 return
             console.print(
@@ -67,14 +66,19 @@
         err_console.print("Censys API rate limit exceeded")
         print_subdomains(subdomains, args.json)
     except CensysUnauthorizedException:
         err_console.print("Invalid Censys API ID or secret")
         sys.exit(1)
     except CensysException as e:
         err_console.print(str(e))
+        print_subdomains(subdomains, args.json)
+        sys.exit(1)
+    except KeyboardInterrupt:
+        err_console.print("Caught Ctrl-C, exiting...")
+        print_subdomains(subdomains, args.json)
         sys.exit(1)
 
 
 def include(parent_parser: argparse._SubParsersAction, parents: dict):
     """Include this subcommand into the parent parser.
 
     Args:
@@ -85,13 +89,13 @@
         "subdomains",
         description="Enumerates subdomains using the Censys Search Certificates index",
         help="enumerate subdomains",
         parents=[parents["auth"]],
     )
     subdomains_parser.add_argument("domain", help="The base domain to search for")
     subdomains_parser.add_argument(
-        "--max-records", type=int, default=100, help="Max records to query"
+        "--pages", type=int, default=1, help="Max records to query"
     )
     subdomains_parser.add_argument(
         "-j", "--json", action="store_true", help="Output in JSON format"
     )
     subdomains_parser.set_defaults(func=cli_subdomains)
```

### Comparing `censys-2.1.9/censys/cli/commands/view.py` & `censys-2.2.0/censys/cli/commands/view.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 """Censys view CLI."""
 import argparse
+import ipaddress
 import sys
 import webbrowser
 
-from censys.cli.utils import V2_INDEXES, console, valid_datetime_type, write_file
+from censys.cli.utils import (
+    V2_INDEXES,
+    console,
+    err_console,
+    valid_datetime_type,
+    write_file,
+)
+from censys.common.exceptions import CensysCLIException
 from censys.search import SearchClient
 from censys.search.v2.api import CensysSearchAPIv2
 
 
 def cli_view(args: argparse.Namespace):
     """Search subcommand.
 
     Args:
         args (Namespace): Argparse Namespace.
+
+    Raises:
+        CensysCLIException: If invalid options are provided.
     """
     if args.open:
         webbrowser.open(
             f"https://search.censys.io/{args.index_type}/{args.document_id}"
         )
         sys.exit(0)
 
@@ -26,24 +37,48 @@
         censys_args["api_id"] = args.api_id
 
     if args.api_secret:
         censys_args["api_secret"] = args.api_secret
 
     c = SearchClient(**censys_args)
 
-    index: CensysSearchAPIv2 = getattr(c.v2, args.index_type)
+    index_type = args.index_type
+
+    if index_type == "hosts":
+        try:
+            ip_address = args.document_id
+            if "+" in ip_address:
+                ip_address, _ = args.document_id.split("+")
+            ipaddress.ip_address(ip_address)
+        except ValueError:
+            if len(args.document_id) == 64:
+                err_console.print(
+                    "This is a SHA-256 certificate fingerprint. Switching to certificates index."
+                )
+                index_type = "certificates"
+            else:
+                raise CensysCLIException(
+                    f"Invalid IP address: {args.document_id}. Please provide a valid IPv4 or IPv6 address."
+                )
+
+    index: CensysSearchAPIv2 = getattr(c.v2, index_type)
 
     view_args = {}
     write_args = {
         "file_format": "json" if args.output else "screen",
         "file_path": args.output,
     }
 
     if args.at_time:
-        view_args["at_time"] = args.at_time
+        if index_type == "hosts":
+            view_args["at_time"] = args.at_time
+        else:
+            err_console.print(
+                "The --at-time option is only supported for the hosts index. Ignoring."
+            )
 
     document = index.view(args.document_id, **view_args)
 
     try:
         write_file(document, **write_args)
     except ValueError as error:  # pragma: no cover
         console.print(f"Error writing log file. Error: {error}")
@@ -62,36 +97,39 @@
             id and the resource index",
         help="view document",
         parents=[parents["auth"]],
     )
     view_parser.add_argument(
         "document_id",
         type=str,
-        help="a document id (IP address) to view",
+        help="a document id (IP address or SHA-256 certificate fingerprint) to view",
     )
     view_parser.add_argument(
         "--index-type",
         type=str,
         default="hosts",
         choices=V2_INDEXES,
         metavar="|".join(V2_INDEXES),
         help="which resource index to query",
     )
     view_parser.add_argument(
-        "--at-time",
-        type=valid_datetime_type,
-        metavar="YYYY-MM-DD (HH:mm)",
-        help="Fetches a document at a given point in time",
-    )
-    view_parser.add_argument(
         "-o",
         "--output",
         type=str,
         help="json output file path",
     )
     view_parser.add_argument(
         "-O",
         "--open",
         action="store_true",
         help="open document in browser",
     )
+
+    hosts_group = view_parser.add_argument_group("hosts specific arguments")
+    hosts_group.add_argument(
+        "--at-time",
+        type=valid_datetime_type,
+        metavar="YYYY-MM-DD (HH:mm)",
+        help="Fetches a document at a given point in time",
+    )
+
     view_parser.set_defaults(func=cli_view)
```

### Comparing `censys-2.1.9/censys/cli/utils.py` & `censys-2.2.0/censys/cli/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Censys CLI utilities."""
 import argparse
-import csv
 import datetime
 import json
 import os.path
 import sys
 from typing import Any, Dict, List, Optional, Union
 
 from rich.console import Console
 
 from censys.common.config import DEFAULT, get_config
-from censys.common.deprecation import DeprecationDecorator
 
 Results = Union[List[dict], Dict[str, Any]]
 
 V1_INDEXES = ["certs"]
-V2_INDEXES = ["hosts"]
+V2_INDEXES = ["hosts", "certificates"]
 INDEXES = V1_INDEXES + V2_INDEXES
 
 config = get_config()
 color = config.get(DEFAULT, "color")
 color_system = "auto" if color else None
 console = Console(color_system=color_system)  # type: ignore
 err_console = Console(color_system=color_system, file=sys.stderr)  # type: ignore
@@ -31,36 +29,14 @@
     Args:
         file_path (str): Name of the file to write to on the disk.
     """
     abs_file_path = os.path.abspath(file_path)
     console.print(f"Wrote results to file {abs_file_path}", soft_wrap=True)
 
 
-@DeprecationDecorator("CSV output is deprecated and will be removed in the future.")
-def _write_csv(file_path: str, search_results: Results, fields: List[str]):
-    """Write search results to a new file in CSV format.
-
-    Args:
-        file_path (str): Name of the file to write to on the disk.
-        search_results (Results): A list of results from the query.
-        fields (List[str]): A list of fields to write as headers.
-    """
-    with open(file_path, "w") as output_file:
-        if search_results and isinstance(search_results, list):
-            # Get the header row from the first result
-            writer = csv.DictWriter(output_file, fieldnames=fields)
-            writer.writeheader()
-
-            for result in search_results:
-                # Use the Dict writer to process and write results to CSV
-                writer.writerow(result)
-
-    print_wrote_file(file_path)
-
-
 def _write_json(file_path: str, search_results: Results):
     """Write search results to a new file in JSON format.
 
     Args:
         file_path (str): Name of the file to write to on the disk.
         search_results (Results): A list of results from the query.
     """
@@ -102,18 +78,14 @@
         file_format = file_format.lower()
 
     if not file_path:
         file_path = "temp-out.json"
 
     if file_format == "json":
         _write_json(file_path, results_list)
-    elif file_format == "csv":
-        if csv_fields is None:  # pragma: no cover
-            csv_fields = []
-        _write_csv(file_path, results_list, fields=csv_fields)
     else:
         _write_screen(results_list)
 
 
 def valid_datetime_type(datetime_str: str) -> datetime.datetime:
     """Custom argparse type for user datetime values from arg.
```

### Comparing `censys-2.1.9/censys/common/base.py` & `censys-2.2.0/censys/common/base.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/common/config.py` & `censys-2.2.0/censys/common/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/common/deprecation.py` & `censys-2.2.0/censys/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/common/exceptions.py` & `censys-2.2.0/censys/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/search/client.py` & `censys-2.2.0/censys/search/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
             Args:
                 *args: Variable length argument list.
                 **kwargs: Arbitrary keyword arguments.
             """
             self.hosts = CensysHosts(*args, **kwargs)
             self.certs = CensysCerts(*args, **kwargs)
+            self.certificates = self.certs
 
     def __init__(self, *args, **kwargs):
         """Inits SearchClient.
 
         Args:
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
```

### Comparing `censys-2.1.9/censys/search/v1/api.py` & `censys-2.2.0/censys/search/v1/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/search/v1/data.py` & `censys-2.2.0/censys/search/v1/data.py`

 * *Files identical despite different names*

### Comparing `censys-2.1.9/censys/search/v2/api.py` & `censys-2.2.0/censys/search/v2/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 from censys.common.base import CensysAPIBase
 from censys.common.config import DEFAULT, get_config
 from censys.common.exceptions import (
     CensysException,
     CensysExceptionMapper,
     CensysSearchException,
 )
-from censys.common.types import Datetime
-from censys.common.utils import format_rfc3339
 
-INDEX_TO_KEY = {"hosts": "ip"}
+INDEX_TO_KEY = {"hosts": "ip", "certificates": "fingerprint_sha256"}
 
 
 class CensysSearchAPIv2(CensysAPIBase):
     """This class is the base class for the Hosts index.
 
     Examples:
         >>> c = CensysSearchAPIv2()
@@ -64,15 +62,14 @@
 
         self._session.auth = (self._api_id, self._api_secret)
 
         # Generate concrete paths to be called
         self.view_path = f"/v2/{self.INDEX_NAME}/"
         self.search_path = f"/v2/{self.INDEX_NAME}/search"
         self.aggregate_path = f"/v2/{self.INDEX_NAME}/aggregate"
-        self.metadata_path = f"/v2/metadata/{self.INDEX_NAME}"
         self.tags_path = "/v2/tags"
         self.account_path = "/v1/account"
 
     def _get_exception_class(  # type: ignore
         self, res: Response
     ) -> Type[CensysSearchException]:
         return CensysExceptionMapper.SEARCH_EXCEPTIONS.get(
@@ -152,15 +149,15 @@
                 query=self.query,
                 per_page=per_page or self.per_page or 100,
                 cursor=self.nextCursor or self.cursor,
                 **self.extra_args,
             )
             self.page += 1
             result = payload["result"]
-            self.nextCursor = result["links"]["next"]
+            self.nextCursor = result["links"].get("next")
             if result["total"] == 0 or not self.nextCursor:
                 self.pages = 0
             return result["hits"]
 
         def __next__(self) -> List[dict]:
             """Gets next page of search results.
 
@@ -190,33 +187,34 @@
             """
             results = {}
 
             document_key = INDEX_TO_KEY.get(self.api.INDEX_NAME, "ip")
 
             with ThreadPoolExecutor(max_workers) as executor:
                 threads = {}
-                for hit in self.__call__():
-                    hit_key = hit[document_key]
-                    if "name" in hit:
-                        hit_key += "+" + hit["name"]
-                    threads[executor.submit(self.api.view, hit_key)] = hit_key
+                while self.page <= self.pages:
+                    for hit in self.__call__():
+                        hit_key = hit[document_key]
+                        if "name" in hit and self.api.INDEX_NAME == "hosts":
+                            hit_key += "+" + hit["name"]
+                        threads[executor.submit(self.api.view, hit_key)] = hit_key
 
                 for task in as_completed(threads):
                     document_id = threads[task]
                     try:
                         results[document_id] = task.result()
                     except Exception as e:
                         results[document_id] = {"error": str(e)}
 
             return results
 
     def search(
         self,
         query: str,
-        per_page: Optional[int] = None,
+        per_page: int = 100,
         cursor: Optional[str] = None,
         pages: int = 1,
         **kwargs: Any,
     ) -> Query:
         """Search current index.
 
         Searches the given index for all records that match the given query.
@@ -233,15 +231,15 @@
             Query: Query object that can be a callable or an iterable.
         """
         return self.Query(self, query, per_page, cursor, pages, **kwargs)
 
     def raw_search(
         self,
         query: str,
-        per_page: Optional[int] = None,
+        per_page: int = 100,
         cursor: Optional[str] = None,
         **kwargs: Any,
     ) -> dict:
         """Search current index.
 
         Searches the given index for all records that match the given query.
         This method does no automatic pagination or post processing.
@@ -253,85 +251,72 @@
             **kwargs (Any): Optional; Additional arguments to be passed to the query.
 
         Returns:
             dict: The raw result set.
         """
         args = {
             "q": query,
-            "per_page": per_page or 100,
+            "per_page": per_page,
             "cursor": cursor,
             **kwargs,
         }
         return self._get(self.search_path, args)
 
-    def view(
-        self,
-        document_id: str,
-        at_time: Optional[Datetime] = None,
-    ) -> dict:
+    def view(self, document_id: str, **kwargs: Any) -> dict:
         """View document from current index.
 
         View the current structured data we have on a specific document.
         For more details, see our documentation: https://search.censys.io/api
 
         Args:
             document_id (str): The ID of the document you are requesting.
-            at_time ([str, datetime.date, datetime.datetime]):
-                Optional; Fetches a document at a given point in time.
+            **kwargs (Any): Optional; Additional arguments to be passed to the query.
 
         Returns:
             dict: The result set returned.
         """
-        args = {}
-        if at_time:
-            args["at_time"] = format_rfc3339(at_time)
-
-        return self._get(self.view_path + document_id, args)["result"]
+        return self._get(self.view_path + document_id, args=kwargs)["result"]
 
     def bulk_view(
         self,
         document_ids: List[str],
-        at_time: Optional[Datetime] = None,
         max_workers: int = 20,
+        **kwargs: Any,
     ) -> Dict[str, dict]:
         """Bulk view documents from current index.
 
         View the current structured data we have on a list of documents.
         For more details, see our documentation: https://search.censys.io/api
 
         Args:
             document_ids (List[str]): The IDs of the documents you are requesting.
-            at_time ([str, datetime.date, datetime.datetime]):
-                Optional; Fetches a document at a given point in time.
             max_workers (int): The number of workers to use. Defaults to 20.
+            **kwargs (Any): Optional; Additional arguments to be passed to the query.
 
         Returns:
             Dict[str, dict]: Dictionary mapping document IDs to that document's result set.
         """
-        if at_time:
-            at_time = format_rfc3339(at_time)
-
         documents = {}
         with ThreadPoolExecutor(max_workers) as executor:
             threads = {
-                executor.submit(self.view, document_id, at_time): document_id
+                executor.submit(self.view, document_id, **kwargs): document_id
                 for document_id in document_ids
             }
 
             for task in as_completed(threads):
                 document_id = threads[task]
                 try:
                     documents[document_id] = task.result()
                 except Exception as e:
                     documents[document_id] = {"error": str(e)}
 
         return documents
 
     def aggregate(
-        self, query: str, field: str, num_buckets: Optional[int] = None, **kwargs: Any
+        self, query: str, field: str, num_buckets: int = 50, **kwargs: Any
     ) -> dict:
         """Aggregate current index.
 
         Creates a report on the breakdown of the values of a field in a result set.
         For more details, see our documentation: https://search.censys.io/api
 
         Args:
@@ -342,22 +327,14 @@
 
         Returns:
             dict: The result set returned.
         """
         args = {"q": query, "field": field, "num_buckets": num_buckets, **kwargs}
         return self._get(self.aggregate_path, args)["result"]
 
-    def metadata(self) -> dict:
-        """Get current index metadata.
-
-        Returns:
-            dict: The result set returned.
-        """
-        return self._get(self.metadata_path)["result"]
-
     # Comments
 
     def get_comments(self, document_id: str) -> List[dict]:
         """Get comments for a document.
 
         Args:
             document_id (str): The ID of the document you are requesting.
@@ -365,14 +342,28 @@
         Returns:
             List[dict]: The list of comments.
         """
         return self._get(self.view_path + document_id + "/comments")["result"][
             "comments"
         ]
 
+    def get_comment(self, document_id: str, comment_id: str) -> dict:
+        """Get comment for a document.
+
+        Args:
+            document_id (str): The ID of the document you are requesting.
+            comment_id (str): The ID of the comment you are requesting.
+
+        Returns:
+            dict: The result set returned.
+        """
+        return self._get(self.view_path + document_id + "/comments/" + comment_id)[
+            "result"
+        ]
+
     def add_comment(self, document_id: str, contents: str) -> dict:
         """Add comment to a document.
 
         Args:
             document_id (str): The ID of the document you are requesting.
             contents (str): The contents of the comment.
```

### Comparing `censys-2.1.9/censys/search/v2/hosts.py` & `censys-2.2.0/censys/search/v2/hosts.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,18 +68,84 @@
         >>> h.view_host_events("1.1.1.1")
         [{'timestamp': '2019-01-01T00:00:00.000Z'}]
     """
 
     INDEX_NAME = "hosts"
     """Name of Censys Index."""
 
+    def __init__(
+        self, api_id: Optional[str] = None, api_secret: Optional[str] = None, **kwargs
+    ):
+        """Inits CensysHosts.
+
+        See CensysSearchAPIv2 for additional arguments.
+
+        Args:
+            api_id (Optional[str], optional): API ID. Defaults to None.
+            api_secret (Optional[str], optional): API Secret. Defaults to None.
+            **kwargs: Arbitrary keyword arguments.
+        """
+        super().__init__(api_id=api_id, api_secret=api_secret, **kwargs)
+        self.metadata_path = f"/v2/metadata/{self.INDEX_NAME}"
+
+    def view(
+        self,
+        document_id: str,
+        at_time: Optional[Datetime] = None,
+        **kwargs: Any,
+    ) -> dict:
+        """View document from current index.
+
+        View the current structured data we have on a specific document.
+        For more details, see our documentation: https://search.censys.io/api
+
+        Args:
+            document_id (str): The ID of the document you are requesting.
+            at_time ([str, datetime.date, datetime.datetime]):
+                Optional; Fetches a document at a given point in time.
+            **kwargs (Any): Optional; Additional arguments to be passed to the query.
+
+        Returns:
+            dict: The result set returned.
+        """
+        args = {}
+        if at_time:
+            args["at_time"] = format_rfc3339(at_time)
+
+        return super().view(document_id, **args)
+
+    def bulk_view(
+        self,
+        document_ids: List[str],
+        max_workers: int = 20,
+        at_time: Optional[Datetime] = None,
+        **kwargs: Any,
+    ) -> Dict[str, dict]:
+        """Bulk view documents from current index.
+
+        View the current structured data we have on a list of documents.
+
+        Args:
+            document_ids (List[str]): The IDs of the documents you are requesting.
+            max_workers (int): Optional; The number of workers to use. Defaults to 20.
+            at_time ([str, datetime.date, datetime.datetime]):
+                Optional; Fetches a document at a given point in time.
+            **kwargs (Any): Optional; Additional arguments to be passed to the query.
+
+        Returns:
+            Dict[str, dict]: The result set returned.
+        """
+        if at_time:
+            kwargs["at_time"] = format_rfc3339(at_time)
+        return super().bulk_view(document_ids, max_workers, **kwargs)
+
     def search(
         self,
         query: str,
-        per_page: Optional[int] = None,
+        per_page: int = 100,
         cursor: Optional[str] = None,
         pages: int = 1,
         virtual_hosts: Optional[str] = None,
         **kwargs: Any,
     ) -> CensysSearchAPIv2.Query:
         """Search host index.
 
@@ -101,15 +167,15 @@
             kwargs["virtual_hosts"] = virtual_hosts
         return super().search(query, per_page, cursor, pages, **kwargs)
 
     def aggregate(
         self,
         query: str,
         field: str,
-        num_buckets: Optional[int] = None,
+        num_buckets: int = 50,
         virtual_hosts: Optional[str] = None,
         **kwargs: Any,
     ) -> dict:
         """Aggregate host index.
 
         Creates a report on the breakdown of the values of a field in a result set.
         For more details, see our documentation: https://search.censys.io/api
@@ -124,14 +190,22 @@
         Returns:
             dict: The result set returned.
         """
         if virtual_hosts:
             kwargs["virtual_hosts"] = virtual_hosts
         return super().aggregate(query, field, num_buckets, **kwargs)
 
+    def metadata(self) -> dict:
+        """Get metadata for the host index.
+
+        Returns:
+            dict: The result set returned.
+        """
+        return self._get(self.metadata_path)["result"]
+
     def view_host_names(
         self, ip: str, per_page: Optional[int] = None, cursor: Optional[str] = None
     ) -> List[str]:
         """Fetches a list of host names for the specified IP address.
 
         Args:
             ip (str): The IP address of the requested host.
```

### Comparing `censys-2.1.9/pyproject.toml` & `censys-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censys"
-version = "2.1.9"
+version = "2.2.0"
 description = "An easy-to-use and lightweight API wrapper for Censys APIs (censys.io)."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = ["censys/py.typed"]
 keywords = ["censys", "api", "search", "attack surface management"]
 classifiers = [
@@ -46,44 +46,44 @@
 "Tracker" = "https://github.com/censys/censys-python/issues"
 "Source" = "https://github.com/censys/censys-python"
 
 [tool.poetry.scripts]
 censys = "censys.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-requests = ">=2.26.0"
+python = ">=3.7.2,<4.0.0"
+requests = ">=2.29.0"
 backoff = "^2.0.1"
 rich = ">=10.16.2"
 importlib-metadata = { version = "*", python = "<3.8" }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 # Lint
 flake8 = "^5.0.4"
-flake8-docstrings = "^1.6.0"
-flake8-pytest-style = "^1.6.0"
-flake8-simplify = "^0.19.3"
-flake8-comprehensions = "^3.10.0"
-flake8-isort = "^5.0.0"
-isort = "^5.10.1"
-pep8-naming = "^0.13.2"
-flake8-black = "^0.3.3"
-black = "^22.10.0"
-blacken-docs = "^1.12.1"
+flake8-docstrings = "^1.7.0"
+flake8-pytest-style = "^1.7.2"
+flake8-simplify = "^0.20.0"
+flake8-comprehensions = "^3.12.0"
+flake8-isort = "^6.0.0"
+isort = "^5.11.5"
+pep8-naming = "^0.13.3"
+flake8-black = "^0.3.6"
+black = "^23.3.0"
+blacken-docs = "^1.13.0"
 darglint = "^1.8.1"
-pyupgrade = "^3.1.0"
+pyupgrade = "^3.3.1"
 # Tests
-pytest = "^7.1.3"
+pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
-responses = "^0.22.0"
-parameterized = "^0.8.1"
+responses = "^0.23.1"
+parameterized = "^0.9.0"
 # Types
-mypy = "^0.982"
-types-requests = ">=2.26.0"
+mypy = "^1.2.0"
+types-requests = "^2.28.11.17"
 
 [tool.black]
 target-version = ["py37"]
 
 [tool.isort]
 profile = "black"
 line_length = 88
@@ -96,13 +96,13 @@
 [tool.mypy]
 python_version = "3.7"
 files = ["censys"]
 namespace_packages = true
 explicit_package_bases = true
 
 [[tool.mypy.overrides]]
-module = ["parameterized", "importlib_metadata"]
+module = ["parameterized", "importlib_metadata", "rich"]
 ignore_missing_imports = true
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `censys-2.1.9/PKG-INFO` & `censys-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: censys
-Version: 2.1.9
+Version: 2.2.0
 Summary: An easy-to-use and lightweight API wrapper for Censys APIs (censys.io).
 License: Apache-2.0
 Keywords: censys,api,search,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -37,36 +36,36 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: backoff (>=2.0.1,<3.0.0)
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: requests (>=2.26.0)
+Requires-Dist: importlib-metadata ; python_version < "3.8"
+Requires-Dist: requests (>=2.29.0)
 Requires-Dist: rich (>=10.16.2)
 Project-URL: Censys Homepage, https://censys.io/
 Project-URL: Censys Search, https://search.censys.io/
 Project-URL: Changelog, https://github.com/censys/censys-python/releases
 Project-URL: Discussions, https://github.com/censys/censys-python/discussions
 Project-URL: Documentation, https://censys-python.rtfd.io
 Project-URL: Source, https://github.com/censys/censys-python
 Project-URL: Tracker, https://github.com/censys/censys-python/issues
 Description-Content-Type: text/markdown
 
 # Censys Python Library
 
 [![PyPI](https://img.shields.io/pypi/v/censys?color=orange&logo=pypi&logoColor=orange)](https://pypi.org/project/censys/)
-[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue?logo=python)](https://www.python.org/downloads/)
+[![Python Version](https://img.shields.io/badge/python-3.7.2%2B-blue?logo=python)](https://www.python.org/downloads/)
 [![Read the Docs (version)](https://img.shields.io/readthedocs/censys-python/latest?logo=read%20the%20docs)](https://censys-python.readthedocs.io/en/stable/?badge=stable)
 [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-brightgreen?logo=github)](https://github.com/censys/censys-python/discussions)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-organge.svg?logo=git&logoColor=organge)](http://makeapullrequest.com)
 [![License](https://img.shields.io/github/license/censys/censys-python?logo=apache)](https://github.com/censys/censys-python/blob/main/LICENSE)
 
-An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7+ is currently supported.
+An easy-to-use and lightweight API wrapper for Censys APIs ([censys.io](https://censys.io/)). Python 3.7.2+ is currently supported.
 
 > **Notice:** The Censys Search v1 endpoints are deprecated as of Nov. 30, 2021. Please begin using v2 endpoints to query hosts and certificates and check out our [support center](https://support.censys.io/hc/en-us/sections/360013076551-Censys-Search-2-0) for resources.
 
 ## Features
 
 - [Search Censys data](https://censys-python.readthedocs.io/en/stable/usage-v2.html)
 - [Bulk Certificate lookups](https://censys-python.readthedocs.io/en/stable/usage-v1.html#bulk)
```

