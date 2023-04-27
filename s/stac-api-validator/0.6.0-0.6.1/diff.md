# Comparing `tmp/stac_api_validator-0.6.0.tar.gz` & `tmp/stac_api_validator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_api_validator-0.6.0.tar", max compression
+gzip compressed data, was "stac_api_validator-0.6.1.tar", max compression
```

## Comparing `stac_api_validator-0.6.0.tar` & `stac_api_validator-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11342 2023-04-23 14:33:55.142043 stac_api_validator-0.6.0/LICENSE
--rw-r--r--   0        0        0     9879 2023-04-23 14:33:55.142043 stac_api_validator-0.6.0/README.md
--rw-r--r--   0        0        0     2450 2023-04-23 14:34:14.914210 stac_api_validator-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/__init__.py
--rw-r--r--   0        0        0     6329 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/__main__.py
--rw-r--r--   0        0        0     9583 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/filters.py
--rw-r--r--   0        0        0     1303 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/geometries.py
--rw-r--r--   0        0        0        0 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/py.typed
--rw-r--r--   0        0        0   130124 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/validations.py
--rw-r--r--   0        0        0    11163 1970-01-01 00:00:00.000000 stac_api_validator-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/LICENSE
+-rw-r--r--   0        0        0     9879 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/README.md
+-rw-r--r--   0        0        0     2450 2023-04-27 16:00:29.129889 stac_api_validator-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/__init__.py
+-rw-r--r--   0        0        0     6329 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/__main__.py
+-rw-r--r--   0        0        0     9583 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/filters.py
+-rw-r--r--   0        0        0     1303 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/geometries.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/py.typed
+-rw-r--r--   0        0        0   130272 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/validations.py
+-rw-r--r--   0        0        0    11163 1970-01-01 00:00:00.000000 stac_api_validator-0.6.1/PKG-INFO
```

### Comparing `stac_api_validator-0.6.0/LICENSE` & `stac_api_validator-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.0/README.md` & `stac_api_validator-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.0/pyproject.toml` & `stac_api_validator-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stac-api-validator"
-version = "0.6.0"
+version = "0.6.1"
 description = "STAC API Validator"
 authors = ["Phil Varner <phil@philvarner.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/stac-utils/stac-api-validator"
 repository = "https://github.com/stac-utils/stac-api-validator"
 documentation = "https://stac-api-validator.readthedocs.io"
```

### Comparing `stac_api_validator-0.6.0/src/stac_api_validator/__main__.py` & `stac_api_validator-0.6.1/src/stac_api_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.0/src/stac_api_validator/filters.py` & `stac_api_validator-0.6.1/src/stac_api_validator/filters.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.0/src/stac_api_validator/geometries.py` & `stac_api_validator-0.6.1/src/stac_api_validator/geometries.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.0/src/stac_api_validator/validations.py` & `stac_api_validator-0.6.1/src/stac_api_validator/validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 from .filters import cql2_text_s_intersects
 from .filters import cql2_text_string_comparisons
 from .filters import cql2_text_timestamp_comparisons
 
 
 logger = logging.getLogger(__name__)
 
-LATEST_STAC_API_VERSION = "https://api.stacspec.org/v1.0.0-rc.2"
+LATEST_STAC_API_FOUNDATION_VERSION = "https://api.stacspec.org/v1.0.0/"
 
 
 class Method(Enum):
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     PATCH = "PATCH"
@@ -436,24 +436,27 @@
         errors += ("CORE-3", "/ : 'links' field must be defined and non-empty.")
 
     conforms_to = body.get("conformsTo", [])
     if not conforms_to:
         errors += (
             "CORE-2",
             "[Core] : Landing Page (/) 'conformsTo' field must be defined and non-empty."
-            "This field is required as of 1.0.0.",
+            "This field is required as of STAC 1.0.0",
         )
     else:
         if any(
             x
             for x in conforms_to
-            if x.startswith("https://api.stacspec.org/v1.0.0")
-            and not x.startswith(LATEST_STAC_API_VERSION)
+            if re.match(
+                r"https://api\.stacspec\.org/v1\.0\.0.*/(core|item-search|ogcapi-features|collections)",
+                x,
+            )
+            and not x.startswith(LATEST_STAC_API_FOUNDATION_VERSION)
         ):
-            warnings += "STAC API Specification v1.0.0-rc.2 is the latest version, but API advertises an older version or older versions."
+            warnings += f"STAC API Specification {LATEST_STAC_API_FOUNDATION_VERSION} is the latest version, but API advertises an older version or older versions."
 
     if not supports(conforms_to, cc_core_regex):
         errors += ("CORE-4", "/: STAC API - Core not contained in 'conformsTo'")
 
     if "browseable" in conformance_classes and not any(
         cc_browseable_regex.fullmatch(x) for x in conforms_to
     ):
```

### Comparing `stac_api_validator-0.6.0/PKG-INFO` & `stac_api_validator-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-api-validator
-Version: 0.6.0
+Version: 0.6.1
 Summary: STAC API Validator
 Home-page: https://github.com/stac-utils/stac-api-validator
 License: Apache-2.0
 Author: Phil Varner
 Author-email: phil@philvarner.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

