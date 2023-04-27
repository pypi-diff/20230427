# Comparing `tmp/tap_krow-0.7.0.tar.gz` & `tmp/tap_krow-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_krow-0.7.0.tar", max compression
+gzip compressed data, was "tap_krow-0.8.0.tar", max compression
```

## Comparing `tap_krow-0.7.0.tar` & `tap_krow-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1045 2023-03-22 16:51:48.399084 tap_krow-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/__init__.py
--rw-r--r--   0        0        0      399 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/auth.py
--rw-r--r--   0        0        0     9336 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/client.py
--rw-r--r--   0        0        0     2719 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/normalize.py
--rw-r--r--   0        0        0    12491 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/streams.py
--rw-r--r--   0        0        0     1257 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tap.py
--rw-r--r--   0        0        0       31 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/__init__.py
--rw-r--r--   0        0        0    24080 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/applicants/applicants_default.json
--rw-r--r--   0        0        0      549 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json
--rw-r--r--   0        0        0     4922 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/locations/locations_default.json
--rw-r--r--   0        0        0    60100 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/organizations/orgs_default.json
--rw-r--r--   0        0        0      575 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json
--rw-r--r--   0        0        0     7860 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json
--rw-r--r--   0        0        0     4411 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/positions/positions_default.json
--rw-r--r--   0        0        0     4311 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/api_responses/regions/regions_default.json
--rw-r--r--   0        0        0      959 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_applicants_stream.py
--rw-r--r--   0        0        0     2677 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_client.py
--rw-r--r--   0        0        0      681 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_core.py
--rw-r--r--   0        0        0     1375 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_locations_stream.py
--rw-r--r--   0        0        0     1723 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_normalize.py
--rw-r--r--   0        0        0     1523 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_organizations_stream.py
--rw-r--r--   0        0        0     1678 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_paginator.py
--rw-r--r--   0        0        0     1261 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_positions_stream.py
--rw-r--r--   0        0        0     1360 2023-03-22 16:51:47.454971 tap_krow-0.7.0/tap_krow/tests/test_regions_stream.py
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 tap_krow-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1045 2023-04-27 00:02:26.710002 tap_krow-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/auth.py
+-rw-r--r--   0        0        0     9385 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/client.py
+-rw-r--r--   0        0        0     2719 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/normalize.py
+-rw-r--r--   0        0        0    12491 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/streams.py
+-rw-r--r--   0        0        0     1257 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tap.py
+-rw-r--r--   0        0        0       31 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/__init__.py
+-rw-r--r--   0        0        0    24080 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/applicants/applicants_default.json
+-rw-r--r--   0        0        0     1509 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_no_relationships_property.json
+-rw-r--r--   0        0        0      549 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json
+-rw-r--r--   0        0        0     4922 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/locations/locations_default.json
+-rw-r--r--   0        0        0    60100 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_default.json
+-rw-r--r--   0        0        0      575 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json
+-rw-r--r--   0        0        0     7860 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json
+-rw-r--r--   0        0        0     4411 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/positions/positions_default.json
+-rw-r--r--   0        0        0     4311 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/regions/regions_default.json
+-rw-r--r--   0        0        0      959 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_applicants_stream.py
+-rw-r--r--   0        0        0     3186 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_client.py
+-rw-r--r--   0        0        0      681 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_core.py
+-rw-r--r--   0        0        0     1375 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_locations_stream.py
+-rw-r--r--   0        0        0     1723 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_normalize.py
+-rw-r--r--   0        0        0     1523 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_organizations_stream.py
+-rw-r--r--   0        0        0     1678 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_paginator.py
+-rw-r--r--   0        0        0     1261 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_positions_stream.py
+-rw-r--r--   0        0        0     1360 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_regions_stream.py
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 tap_krow-0.8.0/PKG-INFO
```

### Comparing `tap_krow-0.7.0/pyproject.toml` & `tap_krow-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-krow"
-version = "0.7.0"
+version = "0.8.0"
 description = "`tap-krow` is a Singer tap for the KROW API, built with the Meltano SDK for Singer Taps."
 authors = ["Datateer"]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.12"
 requests = "^2.25.1"
```

### Comparing `tap_krow-0.7.0/tap_krow/client.py` & `tap_krow-0.8.0/tap_krow/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,17 @@
         stop_point = self.get_starting_timestamp(None)
         properties_defined_in_schema = self.schema["properties"].keys()
 
         for record in extract_jsonpath(self.records_jsonpath, input=response.json()):
             d = {
                 "id": record["id"],
                 **record["attributes"],
-                **record["relationships"],
             }
+            if 'relationships' in record:
+                d.update(record["relationships"])
             d = make_fields_meltano_select_compatible(d)
 
             # remove extraneous keys that only muddle the field names in the output
             d = remove_unnecessary_keys(d, ["data"])
 
             d = flatten_dict(d)
```

### Comparing `tap_krow-0.7.0/tap_krow/normalize.py` & `tap_krow-0.8.0/tap_krow/normalize.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/streams.py` & `tap_krow-0.8.0/tap_krow/streams.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tap.py` & `tap_krow-0.8.0/tap_krow/tap.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/applicants/applicants_default.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/applicants/applicants_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/locations/locations_default.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/locations/locations_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/organizations/orgs_default.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/positions/positions_default.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/positions/positions_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/api_responses/regions/regions_default.json` & `tap_krow-0.8.0/tap_krow/tests/api_responses/regions/regions_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_applicants_stream.py` & `tap_krow-0.8.0/tap_krow/tests/test_applicants_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_client.py` & `tap_krow-0.8.0/tap_krow/tests/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test general stream capabilities"""
 
 from datetime import datetime
 import pytest
 import pytz
 from urllib.parse import urlparse
 
-from tap_krow.streams import OrganizationsStream
+from tap_krow.streams import CampaignStream, OrganizationsStream
 
 
 @pytest.fixture(scope="module")
 def responses(api_responses):
     """Returns an instance of a stream, which"""
     return api_responses["organizations"]
 
@@ -63,7 +63,14 @@
     stream.get_starting_timestamp = lambda x: datetime(2020, 1, 1, tzinfo=pytz.utc)  # simulate that the last run was some days ago
     records = list(stream.parse_response(responses["orgs_records_before_and_after_2020-01-01.json"]))
     ids = [r["id"] for r in records]
     assert ids == ["record_updated_at_jan_3", "record_updated_at_jan_2"]
 
 
 # endregion
+
+def test_handles_when_entities_do_not_have_a_relationships_property(api_responses, stream_factory):
+    stream = stream_factory(CampaignStream)
+    # test with a file that contains campaign entities without a "relationship" property
+    res = stream.parse_response(api_responses["campaigns"]["campaigns_no_relationships_property.json"])
+    # the simple fact that no exception was thrown indicates that this test succeeded
+    assert next(res)['id'] == '9b2f9b64-ddb5-477b-ac24-4cf015df8c2d'
```

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_core.py` & `tap_krow-0.8.0/tap_krow/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_locations_stream.py` & `tap_krow-0.8.0/tap_krow/tests/test_locations_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_normalize.py` & `tap_krow-0.8.0/tap_krow/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_organizations_stream.py` & `tap_krow-0.8.0/tap_krow/tests/test_organizations_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_paginator.py` & `tap_krow-0.8.0/tap_krow/tests/test_paginator.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_positions_stream.py` & `tap_krow-0.8.0/tap_krow/tests/test_positions_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/tap_krow/tests/test_regions_stream.py` & `tap_krow-0.8.0/tap_krow/tests/test_regions_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.7.0/PKG-INFO` & `tap_krow-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-krow
-Version: 0.7.0
+Version: 0.8.0
 Summary: `tap-krow` is a Singer tap for the KROW API, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Author: Datateer
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

