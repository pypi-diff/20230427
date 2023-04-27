# Comparing `tmp/pubtools-ami-2.1.0.tar.gz` & `tmp/pubtools-ami-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubtools-ami-2.1.0.tar", last modified: Tue Mar 14 09:17:24 2023, max compression
+gzip compressed data, was "pubtools-ami-2.2.0.tar", last modified: Thu Apr 27 08:56:24 2023, max compression
```

## Comparing `pubtools-ami-2.1.0.tar` & `pubtools-ami-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:24.941476 pubtools-ami-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-14 09:17:24.941476 pubtools-ami-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:24.937476 pubtools-ami-2.1.0/pubtools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:24.937476 pubtools-ami-2.1.0/pubtools/_ami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/rhsm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:24.941476 pubtools-ami-2.1.0/pubtools/_ami/services/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/services/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/services/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/services/rhsm_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:24.941476 pubtools-ami-2.1.0/pubtools/_ami/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/pubtools/_ami/tasks/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 09:17:24.941476 pubtools-ami-2.1.0/pubtools_ami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-14 09:17:24.000000 pubtools-ami-2.1.0/pubtools_ami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-14 09:17:24.000000 pubtools-ami-2.1.0/pubtools_ami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 09:17:24.000000 pubtools-ami-2.1.0/pubtools_ami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-14 09:17:24.000000 pubtools-ami-2.1.0/pubtools_ami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-14 09:17:24.000000 pubtools-ami-2.1.0/pubtools_ami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-14 09:17:24.000000 pubtools-ami-2.1.0/pubtools_ami.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 09:17:24.941476 pubtools-ami-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-14 09:17:12.000000 pubtools-ami-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:24.886651 pubtools-ami-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 08:56:24.886651 pubtools-ami-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:24.882651 pubtools-ami-2.2.0/pubtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:24.882651 pubtools-ami-2.2.0/pubtools/_ami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/rhsm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:24.886651 pubtools-ami-2.2.0/pubtools/_ami/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/services/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/services/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/services/rhsm_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:24.886651 pubtools-ami-2.2.0/pubtools/_ami/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/tasks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/pubtools/_ami/tasks/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:56:24.886651 pubtools-ami-2.2.0/pubtools_ami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 08:56:24.000000 pubtools-ami-2.2.0/pubtools_ami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-27 08:56:24.000000 pubtools-ami-2.2.0/pubtools_ami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:56:24.000000 pubtools-ami-2.2.0/pubtools_ami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 08:56:24.000000 pubtools-ami-2.2.0/pubtools_ami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 08:56:24.000000 pubtools-ami-2.2.0/pubtools_ami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 08:56:24.000000 pubtools-ami-2.2.0/pubtools_ami.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:56:24.886651 pubtools-ami-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-27 08:56:07.000000 pubtools-ami-2.2.0/setup.py
```

### Comparing `pubtools-ami-2.1.0/CHANGELOG.md` & `pubtools-ami-2.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 - n/a
 
+## [2.2.0] - 2023-04-27
+
+### Added
+
+- Introduced new command `pubtools-ami-delete`
+
 ## [2.1.0] - 2023-03-14
 
 ### Added
 
 - Support for `public_image` flag on AMI push item.
 
 ### Fixed
@@ -67,13 +73,14 @@
 
 - Added missing dependencies `attrs` and `six`
 
 ## 0.1.0 - 2021-11-17
 
 - Initial release to PyPI
 
-[Unreleased]: https://github.com/release-engineering/pubtools-ami/compare/v2.1.0...HEAD
+[Unreleased]: https://github.com/release-engineering/pubtools-ami/compare/v2.2.0...HEAD
+[2.2.0]: https://github.com/release-engineering/pubtools-ami/compare/v2.1.0...v2.2.0
 [2.1.0]: https://github.com/release-engineering/pubtools-ami/compare/v2.0.0...v2.1.0
 [2.0.0]: https://github.com/release-engineering/pubtools-ami/compare/v1.2.1...v2.0.0
 [1.2.1]: https://github.com/release-engineering/pubtools-ami/compare/v1.2.0...v1.2.1
 [1.2.0]: https://github.com/release-engineering/pubtools-ami/compare/v1.1.0...v1.2.0
 [1.1.0]: https://github.com/release-engineering/pubtools-ami/compare/v1.0.0...v1.1.0
```

### Comparing `pubtools-ami-2.1.0/LICENSE` & `pubtools-ami-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/PKG-INFO` & `pubtools-ami-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-ami
-Version: 2.1.0
+Version: 2.2.0
 Summary: Publishing tools for Amazon machine Images(AMI)
 Home-page: https://github.com/release-engineering/pubtools-ami
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-ami/
 Project-URL: Changelog, https://github.com/release-engineering/pubtools-ami/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pubtools-ami-2.1.0/README.md` & `pubtools-ami-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/arguments.py` & `pubtools-ami-2.2.0/pubtools/_ami/arguments.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/rhsm.py` & `pubtools-ami-2.2.0/pubtools/_ami/rhsm.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,27 +96,34 @@
 
         out = self._executor.submit(self._send, prepped_req)
         out = f_map(out, error_fn=self._on_failure)
 
         return out
 
     def update_image(
-        self, image_id, image_name, arch, product_name, version=None, variant=None
+        self,
+        image_id,
+        image_name,
+        arch,
+        product_name,
+        version=None,
+        variant=None,
+        status="VISIBLE",
     ):
         url = urljoin(self._url, "/v1/internal/cloud_access_providers/amazon/amis")
 
         now = datetime.utcnow().replace(microsecond=0).isoformat()
         rhsm_image = {
             "amiID": image_id,
             "arch": arch.lower(),
             "product": product_name,
             "version": version or "none",
             "variant": variant or "none",
             "description": "Released %s on %s" % (image_name, now),
-            "status": "VISIBLE",
+            "status": status,
         }
         req = requests.Request("PUT", url, json=rhsm_image)
         prepped_req = self._session.prepare_request(req)
 
         out = self._executor.submit(self._send, prepped_req)
         out = f_map(out, error_fn=self._on_failure)
 
@@ -148,7 +155,32 @@
         req = requests.Request("POST", url, json=rhsm_image)
         prepped_req = self._session.prepare_request(req)
 
         out = self._executor.submit(self._send, prepped_req)
         out = f_map(out, error_fn=self._on_failure)
 
         return out
+
+    def list_image_ids(self):
+        url = urljoin(self._url, "/v1/internal/cloud_access_providers/amazon/amis")
+        image_ids = set()
+
+        def handle_page(offset=0):
+            params = {"limit": 1000, "offset": offset}
+            req = requests.Request("GET", url, params=params)
+            prepped_req = self._session.prepare_request(req)
+
+            resp_f = self._executor.submit(self._send, prepped_req)
+            resp_f = f_map(
+                resp_f, fn=self._check_http_response, error_fn=self._on_failure
+            )
+            resp = resp_f.result().json()
+            items_count = resp["pagination"]["count"]
+            if items_count:
+                offset += items_count
+                for item in resp.get("body") or []:
+                    image_ids.add(item["amiID"])
+                return handle_page(offset)
+
+        LOG.debug("Listing all images from rhsm, %s", url)
+        handle_page()
+        return image_ids
```

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/services/aws.py` & `pubtools-ami-2.2.0/pubtools/_ami/services/aws.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/services/base.py` & `pubtools-ami-2.2.0/pubtools/_ami/services/base.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/services/collector.py` & `pubtools-ami-2.2.0/pubtools/_ami/services/collector.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/services/rhsm_.py` & `pubtools-ami-2.2.0/pubtools/_ami/services/rhsm_.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/step.py` & `pubtools-ami-2.2.0/pubtools/_ami/step.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/task.py` & `pubtools-ami-2.2.0/pubtools/_ami/task.py`

 * *Files identical despite different names*

### Comparing `pubtools-ami-2.1.0/pubtools/_ami/tasks/push.py` & `pubtools-ami-2.2.0/pubtools/_ami/tasks/push.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,24 @@
 import logging
-import sys
 import os
 import time
-import datetime
 import json
 import attr
 
 from requests import HTTPError
 from more_executors import Executors
 from cloudimg.aws import AWSPublishingMetadata
-from pushsource import Source, AmiPushItem
-from pubtools._ami.task import AmiTask
-from pubtools._ami.arguments import SplitAndExtend
 from ..services import RHSMClientService, AWSPublishService, CollectorService
+from .base import AmiBase
+from .exceptions import AWSPublishError
 
 LOG = logging.getLogger("pubtools.ami")
 
 
-class MissingProductError(Exception):
-    """Exception class for products missing in the metadata service"""
-
-
-class AWSPublishError(Exception):
-    """Exception class for AWS publish errors"""
-
-
-class AmiPush(AmiTask, RHSMClientService, AWSPublishService, CollectorService):
+class AmiPush(AmiBase, RHSMClientService, AWSPublishService, CollectorService):
     """Pushes one or more Amazon Machine Images to AWS from the specified sources.
 
     This command gets the AMIs from the provided sources, checks for the image product in
     the metadata service e.g. RHSM and then uploads to AWS using the image metadata from
     the source. The image metadata is then updated to the metadata service post upload if
     the images were shipped to the users.
     """
@@ -37,93 +26,14 @@
     _REQUEST_THREADS = int(os.environ.get("AMI_PUSH_REQUEST_THREADS", "5"))
 
     def __init__(self, *args, **kwargs):
         self._ami_push_items = None
         self._rhsm_products = None
         super(AmiPush, self).__init__(*args, **kwargs)
 
-    @property
-    def ami_push_items(self):
-        if not self._ami_push_items:
-            self._ami_push_items = self._get_push_items()
-        return self._ami_push_items or None
-
-    def fail(self, *args, **kwargs):
-        LOG.error(*args, **kwargs)
-        sys.exit(30)
-
-    def _get_push_items(self):
-        ami_push_items = []
-
-        for source_loc in self.args.source:
-            with Source.get(source_loc) as source:
-                for push_item in source:
-                    if not isinstance(push_item, AmiPushItem):
-                        LOG.warning(
-                            "Push Item %s at %s is not an AmiPushItem. "
-                            "Dropping it from the queue",
-                            push_item.name,
-                            push_item.src,
-                        )
-                        continue
-                    ami_push_items.append(push_item)
-        return ami_push_items
-
-    @property
-    def rhsm_products(self):
-        """List of products/image groups for all the service providers"""
-        if self._rhsm_products is None:
-            response = self.rhsm_client.rhsm_products().result()
-            self._rhsm_products = response.json()["body"]
-            prod_names = [
-                "%s(%s)" % (p["name"], p["providerShortName"])
-                for p in self._rhsm_products
-            ]
-            LOG.debug(
-                "%s Products(AWS provider) in rhsm: %s",
-                len(prod_names),
-                ", ".join(sorted(prod_names)),
-            )
-        return self._rhsm_products
-
-    def to_rhsm_product(self, product, image_type):
-        """Product info from rhsm for the specified product in metadata"""
-        # The rhsm prodcut should always be the product (short) plus
-        # "_HOURLY" for hourly type images.
-        image_type = image_type.upper()
-        aws_provider_name = self.args.aws_provider_name
-        if image_type == "HOURLY":
-            product = product + "_" + image_type
-
-        LOG.debug(
-            "Searching for product %s for provider %s in rhsm",
-            product,
-            aws_provider_name,
-        )
-        for rhsm_product in self.rhsm_products:
-            if (
-                rhsm_product["name"] == product
-                and rhsm_product["providerShortName"] == aws_provider_name
-            ):
-                return rhsm_product
-
-        raise MissingProductError("Product not in rhsm: %s" % product)
-
-    def in_rhsm(self, product, image_type):
-        """Checks whether the product is present in rhsm for the provider.
-        Returns True if the product is found in rhsm_products else False.
-        """
-        try:
-            self.to_rhsm_product(product, image_type)
-        except MissingProductError as er:
-            LOG.error(er)
-            return False
-
-        return True
-
     def items_in_metadata_service(self):
         """Checks for all the push_items whether they are in
         rhsm or not.
         Returns false if any of item is missing else true.
         """
         verified = True
         for item in self.ami_push_items:
@@ -133,49 +43,14 @@
                     item.name,
                     item.src,
                 )
                 attr.evolve(item, state="INVALIDFILE")
                 verified = False
         return verified
 
-    def name_from_metadata(self, push_item):
-        """
-        Constructs an image name from the metadata.
-        """
-        parts = []
-        release = push_item.release
-
-        if release.base_product is not None:
-            parts.append(release.base_product)
-            if release.base_version is not None:
-                parts.append(release.base_version)
-
-        parts.append(release.product)
-
-        # Some attributes should be separated by underscores
-        underscore_parts = []
-
-        if release.version is not None:
-            underscore_parts.append(release.version)
-
-        underscore_parts.append(push_item.virtualization.upper())
-
-        if release.type is not None:
-            underscore_parts.append(release.type.upper())
-
-        parts.append("_".join(underscore_parts))
-
-        parts.append(release.date.strftime("%Y%m%d"))
-        parts.append(release.arch)
-        parts.append(str(release.respin))
-        parts.append(push_item.billing_codes.name)
-        parts.append(push_item.volume.upper())
-
-        return "-".join(parts)
-
     # pylint:disable=too-many-locals
     def upload(self, push_item):
         """
         Uploads and imports a disk image to AWS. If ship is not True, the image
         will only be available to internal accounts. Returns a tuple of the
         image id as provided by Amazon and its name.
 
@@ -268,15 +143,15 @@
                 try:
                     aws.publish(publish_meta)
                 except Exception as exc:  # pylint:disable=broad-except
                     raise AWSPublishError(exc) from exc
 
         LOG.info("Successfully uploaded %s [%s] [%s]", name, region, image.id)
 
-        return image.id, name
+        return image.id
 
     def update_rhsm_metadata(self, image, push_item):
         """Update rhsm with the uploaded image info. First it creates the region of
         the image assuming it returns OK if the region is present. Then tries to update
         the existing image info. If the image info is not preset, it creates one.
         """
         LOG.info(
@@ -327,39 +202,28 @@
                     image.id,
                     response.status_code,
                 )
                 LOG.error(response.text)
                 response.raise_for_status()
         LOG.info("Successfully registered image %s with rhsm", image.id)
 
-    def region_data(self):
-        """Aggregate push_items for each item and region
-        for various destinations
-        """
-        region_data = {}
-        for item in self.ami_push_items:
-            for _ in item.dest:
-                region = item.region
-                region_data.setdefault((item, region), []).append({"push_item": item})
-        return region_data.values()
-
     def _push_to_region(self, region_data):
         # sends the push_items for each region to be uploaded in
         # a single thread
         retry_wait = self.args.retry_wait or 30
         max_retries = self.args.max_retries or 4
 
         for dest_data in region_data:
             push_item = dest_data["push_item"]
-            image_id = image_name = None
+            image_id = None
             retries = max_retries
 
             while True:
                 try:
-                    image_id, image_name = self.upload(push_item)
+                    image_id = self.upload(push_item)
                     state = "PUSHED"
                 except (HTTPError, AWSPublishError) as exc:
                     LOG.warning(str(exc))
                     if retries > 0:
                         retries -= 1
                         LOG.info("Retrying upload")
                         time.sleep(retry_wait)
@@ -370,55 +234,23 @@
                     state = "NOTPUSHED"
                 # break statement is not covered in py38
                 # https://github.com/nedbat/coveragepy/issues/772
                 break  # pragma: no cover
             dest_data["push_item"] = attr.evolve(push_item, state=state)
             dest_data["state"] = state
             dest_data["image_id"] = image_id
-            dest_data["image_name"] = image_name
+            dest_data["image_name"] = self.name_from_metadata(push_item)
         return region_data
 
-    def collect_push_result(self, results):
-        """Collects the push results and sends its json to the collector"""
-
-        def convert(obj):
-            if isinstance(obj, (datetime.datetime, datetime.date)):
-                return obj.strftime("%Y%m%d")
-
-        mod_result = []
-        for result in results:
-            res_dict = attr.asdict(result["push_item"])
-            # dict can't be modified during iteration.
-            # so iterate over list of keys.
-            for key in list(res_dict):
-                if res_dict[key] is None:
-                    del res_dict[key]
-            res_dict["ami"] = result["image_id"]
-            res_dict["name"] = result["image_name"]
-            mod_result.append(res_dict)
-
-        metadata = json.dumps(mod_result, default=convert, indent=2, sort_keys=True)
-        return self.collector.attach_file("images.json", metadata).result()
-
     def add_args(self):
         super(AmiPush, self).add_args()
 
         group = self.parser.add_argument_group("AMI Push options")
 
         group.add_argument(
-            "source",
-            nargs="+",
-            help="source location of the staged AMIs with the source type. "
-            "e.g. staged:/path/to/stage/ami or "
-            "errata:https://errata.example.com?errata=RHBA-2020:1234",
-            action=SplitAndExtend,
-            split_on=",",
-        )
-
-        group.add_argument(
             "--ship", help="publish the AMIs in public domain", action="store_true"
         )
 
         group.add_argument(
             "--container-prefix",
             help="prefix to storage container for upload",
             default="redhat-cloudimg",
@@ -437,34 +269,14 @@
         group.add_argument(
             "--allow-public-images",
             help="images are released for general use",
             action="store_true",
         )
 
         group.add_argument(
-            "--aws-provider-name",
-            help="AWS provider e.g. AWS, ACN (AWS China), AGOV (AWS US Gov)",
-            default="AWS",
-        )
-
-        group.add_argument(
-            "--retry-wait",
-            help="duration to wait in sec before retrying upload",
-            type=int,
-            default=30,
-        )
-
-        group.add_argument(
-            "--max-retries",
-            help="number of retries on failure to upload",
-            type=int,
-            default=4,
-        )
-
-        group.add_argument(
             "--snapshot-account-ids",
             help="JSON string mapping region to a list of account ids to give "
             "snapshot creation permissions to if a new snapshot is created "
             "as part of the image push.",
             type=json.loads,
             default={},
         )
```

### Comparing `pubtools-ami-2.1.0/pubtools_ami.egg-info/PKG-INFO` & `pubtools-ami-2.2.0/pubtools_ami.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-ami
-Version: 2.1.0
+Version: 2.2.0
 Summary: Publishing tools for Amazon machine Images(AMI)
 Home-page: https://github.com/release-engineering/pubtools-ami
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-ami/
 Project-URL: Changelog, https://github.com/release-engineering/pubtools-ami/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pubtools-ami-2.1.0/pubtools_ami.egg-info/SOURCES.txt` & `pubtools-ami-2.2.0/pubtools_ami.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 pubtools/_ami/task.py
 pubtools/_ami/services/__init__.py
 pubtools/_ami/services/aws.py
 pubtools/_ami/services/base.py
 pubtools/_ami/services/collector.py
 pubtools/_ami/services/rhsm_.py
 pubtools/_ami/tasks/__init__.py
+pubtools/_ami/tasks/base.py
+pubtools/_ami/tasks/delete.py
+pubtools/_ami/tasks/exceptions.py
 pubtools/_ami/tasks/push.py
 pubtools_ami.egg-info/PKG-INFO
 pubtools_ami.egg-info/SOURCES.txt
 pubtools_ami.egg-info/dependency_links.txt
 pubtools_ami.egg-info/entry_points.txt
 pubtools_ami.egg-info/requires.txt
 pubtools_ami.egg-info/top_level.txt
```

### Comparing `pubtools-ami-2.1.0/setup.py` & `pubtools-ami-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_requirements():
     with open("requirements.in") as f:
         return f.read().splitlines()
 
 
 setup(
     name="pubtools-ami",
-    version="2.1.0",
+    version="2.2.0",
     packages=find_packages(exclude=["tests"]),
     url="https://github.com/release-engineering/pubtools-ami",
     license="GNU General Public License",
     description=get_description(),
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     classifiers=[
@@ -36,14 +36,15 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=get_requirements(),
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "pubtools-ami-push = pubtools._ami.tasks.push:entry_point",
+            "pubtools-ami-delete = pubtools._ami.tasks.delete:entry_point",
         ]
     },
     project_urls={
         "Documentation": "https://release-engineering.github.io/pubtools-ami/",
         "Changelog": "https://github.com/release-engineering/pubtools-ami/blob/master/CHANGELOG.md",
     },
 )
```

