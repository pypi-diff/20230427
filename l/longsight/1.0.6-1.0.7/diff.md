# Comparing `tmp/longsight-1.0.6.tar.gz` & `tmp/longsight-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longsight-1.0.6.tar", last modified: Tue Apr 25 14:37:26 2023, max compression
+gzip compressed data, was "longsight-1.0.7.tar", last modified: Thu Apr 27 09:05:51 2023, max compression
```

## Comparing `longsight-1.0.6.tar` & `longsight-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.6/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-25 14:37:26.475587 longsight-1.0.6/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6051 2023-04-24 10:53:59.000000 longsight-1.0.6/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-04-25 14:37:12.000000 longsight-1.0.6/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-04-25 14:37:26.475587 longsight-1.0.6/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/src/longsight/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.6/src/longsight/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12538 2023-04-25 14:36:24.000000 longsight-1.0.6/src/longsight/instrumentation.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/src/longsight.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     6998 2023-03-31 15:41:47.000000 longsight-1.0.6/tests/test_instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.7/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-27 09:05:51.772607 longsight-1.0.7/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6051 2023-04-24 10:53:59.000000 longsight-1.0.7/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-04-27 08:54:33.000000 longsight-1.0.7/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-04-27 09:05:51.772607 longsight-1.0.7/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/src/longsight/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.7/src/longsight/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    13846 2023-04-27 08:50:15.000000 longsight-1.0.7/src/longsight/instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/src/longsight.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8180 2023-04-27 08:50:44.000000 longsight-1.0.7/tests/test_instrumentation.py
```

### Comparing `longsight-1.0.6/LICENSE.md` & `longsight-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.6/PKG-INFO` & `longsight-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.6
+Version: 1.0.7
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `longsight-1.0.6/README.md` & `longsight-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.6/pyproject.toml` & `longsight-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "longsight"
-version = "1.0.6"
+version = "1.0.7"
 description = "This library implements a range of common logging functions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `longsight-1.0.6/setup.cfg` & `longsight-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = longsight
-version = 1.0.6
+version = 1.0.7
 description = This library implements a range of common logging functions.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `longsight-1.0.6/src/longsight/instrumentation.py` & `longsight-1.0.7/src/longsight/instrumentation.py`

 * *Files 11% similar despite different names*

```diff
@@ -287,14 +287,50 @@
         }
 
         if dimensions:
             MetricData["Dimensions"] = dimensions
 
         self._metrics.append(MetricData)
 
+    def add_counter(
+        self,
+        metric_name: str,
+        status_code: int = None,
+        member_id: str = None,
+        additional_dimensions: list[dict] = None,
+        date_time: datetime = None,
+    ):
+        """
+        Add a counter to the list of metrics to send to CloudWatch.
+        :param metric_name: the name of the metric
+        :param status_code: the status code of the request
+        :param member_id: the member id of the request
+        :param additional_dimensions: additional dimensions to add. A list of dictionaries in the form {"Name": "DimensionName", "Value": "DimensionValue"}.
+        :param date_time: the date time of the metric point if you wish to override
+        :return: None
+        """
+        if additional_dimensions is None:
+            additional_dimensions = []
+
+        dimensions = additional_dimensions
+
+        if status_code:
+            dimensions.append({"Name": "StatusCode", "Value": str(status_code)})
+
+        if member_id:
+            dimensions.append({"Name": "MemberId", "Value": str(member_id)})
+
+        self.add_metric_point(
+            metric_name=metric_name,
+            dimensions=dimensions,
+            time_stamp=date_time if date_time else datetime.utcnow(),
+            metric_value=1,
+            unit="Count",
+        )
+
     def __init__(
         self,
         aws_connector: aws_utils.AWSConnector = None,
         namespace: str = "LabsAPI",
         fastapi_app=None,
         request: Request = None,
         cloudwatch_push: bool = False,
```

### Comparing `longsight-1.0.6/src/longsight.egg-info/PKG-INFO` & `longsight-1.0.7/src/longsight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.6
+Version: 1.0.7
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `longsight-1.0.6/tests/test_instrumentation.py` & `longsight-1.0.7/tests/test_instrumentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import sys
 import unittest
+from datetime import datetime
 from unittest.mock import MagicMock, patch
 
 import watchtower
 from fastapi import FastAPI, Request
-from moto import mock_logs
+from moto import mock_logs, mock_cloudwatch
 from starlette.datastructures import MutableHeaders
 from starlette.responses import Response
 from starlette.testclient import TestClient
 from starlette.types import Receive, Scope, Send
 
 sys.path.append("../../")
 sys.path.append("../src")
@@ -103,14 +104,50 @@
         with TestClient(app) as client:
             response = client.get("/dummy_route")
             self.assertEqual(response.status_code, 200)
             self.assertEqual(response.json(), {"success": True})
 
 
 @mock_logs
+@mock_cloudwatch
+class TestAddCounter(unittest.TestCase):
+    def test_add_counter(self):
+        with Instrumentation(request=MagicMock()) as instance:
+            instance.add_metric_point = MagicMock()
+
+            metric_name = "TestMetric"
+            status_code = 200
+            member_id = "12345"
+            additional_dimensions = [{"Name": "Extra", "Value": "Test"}]
+            date_time = datetime.utcnow()
+
+            instance.add_counter(
+                metric_name,
+                status_code,
+                member_id,
+                additional_dimensions,
+                date_time,
+            )
+
+            expected_dimensions = [
+                {"Name": "Extra", "Value": "Test"},
+                {"Name": "StatusCode", "Value": str(status_code)},
+                {"Name": "MemberId", "Value": str(member_id)},
+            ]
+
+            instance.add_metric_point.assert_called_once_with(
+                metric_name=metric_name,
+                dimensions=expected_dimensions,
+                time_stamp=date_time,
+                metric_value=1,
+                unit="Count",
+            )
+
+
+@mock_logs
 class TestInstrumentWithAWSDecorator(unittest.TestCase):
     def test_instrument_with_aws(self):
         @app.get("/test_aws")
         @instrument(bucket="test_bucket", create_aws=True)
         async def test_route(request: Request, instrumentation=None):
             self.assertIsNotNone(instrumentation)
             self.assertIsNotNone(instrumentation.aws_connector)
```

