# Comparing `tmp/qctrl_client-5.0.0.tar.gz` & `tmp/qctrl_client-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-5.0.0.tar", max compression
+gzip compressed data, was "qctrl_client-6.0.0.tar", max compression
```

## Comparing `qctrl_client-5.0.0.tar` & `qctrl_client-6.0.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0    36653 2023-03-30 05:19:17.221607 qctrl_client-5.0.0/LICENSE
--rw-r--r--   0        0        0      214 2023-03-30 05:19:17.221607 qctrl_client-5.0.0/README.md
--rw-r--r--   0        0        0     2597 2023-03-30 05:19:33.033419 qctrl_client-5.0.0/pyproject.toml
--rw-r--r--   0        0        0      747 2023-03-30 05:19:33.041419 qctrl_client-5.0.0/qctrlclient/__init__.py
--rw-r--r--   0        0        0      686 2023-03-30 05:19:33.041419 qctrl_client-5.0.0/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     1831 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     5885 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      972 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     4308 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     7742 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/client.py
--rw-r--r--   0        0        0      773 2023-03-30 05:19:33.045419 qctrl_client-5.0.0/qctrlclient/core/__init__.py
--rw-r--r--   0        0        0     2999 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/core/functions.py
--rw-r--r--   0        0        0      667 2023-03-30 05:19:33.041419 qctrl_client-5.0.0/qctrlclient/core/router/__init__.py
--rw-r--r--   0        0        0     7351 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/core/router/api.py
--rw-r--r--   0        0        0     1189 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/core/router/base.py
--rw-r--r--   0        0        0     1197 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/core/router/local.py
--rw-r--r--   0        0        0     1673 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/core/settings.py
--rw-r--r--   0        0        0      970 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/core/utils.py
--rw-r--r--   0        0        0     1329 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/defaults.py
--rw-r--r--   0        0        0     2172 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1357 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/globals.py
--rw-r--r--   0        0        0     1424 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2023-03-30 05:19:33.045419 qctrl_client-5.0.0/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4625 2023-03-30 05:19:17.225607 qctrl_client-5.0.0/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 qctrl_client-5.0.0/setup.py
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 qctrl_client-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/README.md
+-rw-r--r--   0        0        0     2614 2023-04-27 05:39:36.128281 qctrl_client-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-04-27 05:39:36.140282 qctrl_client-6.0.0/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      686 2023-04-27 05:39:36.136282 qctrl_client-6.0.0/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     1831 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     5885 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      972 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     4308 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1801 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     7742 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/client.py
+-rw-r--r--   0        0        0      809 2023-04-27 05:39:36.144282 qctrl_client-6.0.0/qctrlclient/core/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/constants.py
+-rw-r--r--   0        0        0     2999 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/functions.py
+-rw-r--r--   0        0        0     1180 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/products.py
+-rw-r--r--   0        0        0      638 2023-04-27 05:39:36.148282 qctrl_client-6.0.0/qctrlclient/core/router/__init__.py
+-rw-r--r--   0        0        0    12204 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/router/api.py
+-rw-r--r--   0        0        0     1189 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/router/base.py
+-rw-r--r--   0        0        0     1197 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/router/local.py
+-rw-r--r--   0        0        0     2677 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/settings.py
+-rw-r--r--   0        0        0     1154 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/utils.py
+-rw-r--r--   0        0        0     1329 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/defaults.py
+-rw-r--r--   0        0        0     2172 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1357 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/globals.py
+-rw-r--r--   0        0        0     1424 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2023-04-27 05:39:36.140282 qctrl_client-6.0.0/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4625 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 qctrl_client-6.0.0/setup.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-6.0.0/PKG-INFO
```

### Comparing `qctrl_client-5.0.0/LICENSE` & `qctrl_client-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/pyproject.toml` & `qctrl_client-6.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "5.0.0"
+version = "6.0.0"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -73,14 +73,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 gql = "^3.4.0"
 qctrl-commons = "^18.0.0"
 requests-oauthlib = "^1.3.1"
 PyJWT = "^2.4.0"
 tenacity = "^8.1.0"
+click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
 pylint = "^2.14.4"
```

### Comparing `qctrl_client-5.0.0/qctrlclient/__init__.py` & `qctrl_client-6.0.0/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/__init__.py` & `qctrl_client-6.0.0/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/base.py` & `qctrl_client-6.0.0/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/cli.py` & `qctrl_client-6.0.0/qctrlclient/auth/cli.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/helpers.py` & `qctrl_client-6.0.0/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/keycloak.py` & `qctrl_client-6.0.0/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/oidc.py` & `qctrl_client-6.0.0/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/password.py` & `qctrl_client-6.0.0/qctrlclient/auth/password.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/redirect_listener.py` & `qctrl_client-6.0.0/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/auth/service_account.py` & `qctrl_client-6.0.0/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/client.py` & `qctrl_client-6.0.0/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/core/__init__.py` & `qctrl_client-6.0.0/qctrlclient/transports/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,8 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-from .functions import (
-    core_workflow,
-    print_warnings,
-    run_core_workflow,
-)
-from .router import (
-    ApiRouter,
-    BaseRouter,
-    LocalRouter,
-    RemoteRegistry,
-)
-from .settings import CoreClientSettings
+from .requests_transport import RequestsTransport
```

### Comparing `qctrl_client-5.0.0/qctrlclient/core/functions.py` & `qctrl_client-6.0.0/qctrlclient/core/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/core/router/__init__.py` & `qctrl_client-6.0.0/qctrlclient/core/router/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,13 +7,10 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-from .api import (
-    ApiRouter,
-    RemoteRegistry,
-)
+from .api import ApiRouter
 from .base import BaseRouter
 from .local import LocalRouter
```

### Comparing `qctrl_client-5.0.0/qctrlclient/core/router/base.py` & `qctrl_client-6.0.0/qctrlclient/core/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/core/router/local.py` & `qctrl_client-6.0.0/qctrlclient/core/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/core/settings.py` & `qctrl_client-6.0.0/qctrlclient/core/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,52 +8,82 @@
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 from dataclasses import dataclass
+from functools import cached_property
 from typing import (
     Callable,
+    Optional,
     Union,
 )
 
-from .router import BaseRouter
+from .products import Product
+from .router.base import BaseRouter
 
 
 @dataclass
 class CoreClientSettings:
     """Settings class for core clients.
 
     Parameters
     ----------
     router : Union[BaseRouter, Callable]
         The router to be used in the core client. Can be either
         an instance of `BaseRouter` or a callable which accepts
         no arguments and returns an instance of `BaseRouter`.
+    product: Optional[Product]
+        Information about the product that the client provides
+        access to. Required for any remote execution of workflows
+        (e.g. `ApiRouter`).
+    organization : Optional[str]
+        The organization that a core workflow should run as.
+        Required for any remove execution of workflows (e.g.
+        `ApiRouter`).
     """
 
     router: Union[BaseRouter, Callable]
+    product: Optional[Product] = None
+    organization: Optional[str] = None
 
     def update(self, **kwargs):
         """Updates settings fields."""
 
         for attr, value in kwargs.items():
             if not hasattr(self, attr):
                 raise AttributeError(f"Invalid field: {attr}")
 
             setattr(self, attr, value)
 
-    def get_router(self) -> BaseRouter:
-        """Returns the configured router to be used by the client."""
-        result = self.router
+        # clear any cached router as config changes could
+        # alter it
+        self._clear_cached_router()
+
+    def _clear_cached_router(self):
+        """Clears the cached router."""
+        try:
+            delattr(self, "_router")
+        except AttributeError:
+            pass
+
+    @cached_property
+    def _router(self) -> BaseRouter:
+        """Prepares the router to be used by the core client."""
 
-        if isinstance(result, BaseRouter):
+        router = self.router
+
+        if isinstance(router, BaseRouter):
             pass
 
-        elif callable(result):
-            result = result()
+        elif callable(router):
+            router = router()
+
+        if not isinstance(router, BaseRouter):
+            raise ValueError(f"Invalid router: {router}")
 
-        else:
-            raise ValueError(f"Invalid router: {result}")
+        return router
 
-        return result
+    def get_router(self) -> BaseRouter:
+        """Returns the configured router to be used by the client."""
+        return self._router
```

### Comparing `qctrl_client-5.0.0/qctrlclient/core/utils.py` & `qctrl_client-6.0.0/qctrlclient/core/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
+import sys
 from typing import Optional
 
+import click
 import pkg_resources
 
 
 def get_installed_version(package: str) -> Optional[str]:
     """Get the installed version of the package. If
     the version cannot be found (e.g. package not installed)
     then None is returned.
@@ -24,7 +26,13 @@
     try:
         version = pkg_resources.get_distribution(package).version
 
     except pkg_resources.ResolutionError:
         version = None
 
     return version
+
+
+def show_error_message(error_message: str):
+    """Displays the error message and stops execution."""
+    click.echo(error_message, err=True)
+    sys.exit(1)
```

### Comparing `qctrl_client-5.0.0/qctrlclient/defaults.py` & `qctrl_client-6.0.0/qctrlclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/exceptions.py` & `qctrl_client-6.0.0/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/globals.py` & `qctrl_client-6.0.0/qctrlclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/pytest_plugin.py` & `qctrl_client-6.0.0/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/qctrlclient/transports/requests_transport.py` & `qctrl_client-6.0.0/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-5.0.0/setup.py` & `qctrl_client-6.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,23 @@
  'qctrlclient.transports']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=2.4.0,<3.0.0',
+ 'click>=8.1.3,<9.0.0',
  'gql>=3.4.0,<4.0.0',
  'qctrl-commons>=18.0.0,<19.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'qctrl-client',
-    'version': '5.0.0',
+    'version': '6.0.0',
     'description': 'Q-CTRL Client',
     'long_description': "# Q-CTRL Python Client\n\nThe Q-CTRL Python Client package provides a Python client to access Q-CTRL's GraphQL API. It is used as a base for Q-CTRL's client-side product packages and for inter-service communication.\n",
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
```

### Comparing `qctrl_client-5.0.0/PKG-INFO` & `qctrl_client-6.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 5.0.0
+Version: 6.0.0
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -29,14 +29,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
```

