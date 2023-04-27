# Comparing `tmp/arcane-mct-1.2.1.tar.gz` & `tmp/arcane_mct-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-mct-1.2.1.tar", max compression
+gzip compressed data, was "arcane_mct-1.2.2.tar", max compression
```

## Comparing `arcane-mct-1.2.1.tar` & `arcane_mct-1.2.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       13 2022-06-13 09:40:43.132830 arcane-mct-1.2.1/README.md
--rw-r--r--   0        0        0     4432 2022-06-13 09:40:43.132830 arcane-mct-1.2.1/arcane/mct.py
--rw-r--r--   0        0        0      461 2022-06-13 09:40:43.132830 arcane-mct-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      709 2022-06-13 09:40:57.499940 arcane-mct-1.2.1/setup.py
--rw-r--r--   0        0        0      694 2022-06-13 09:40:57.500193 arcane-mct-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-04-27 12:42:50.777430 arcane_mct-1.2.2/README.md
+-rw-r--r--   0        0        0     4468 2023-04-27 12:42:50.777430 arcane_mct-1.2.2/arcane/mct.py
+-rw-r--r--   0        0        0      461 2023-04-27 12:42:50.777430 arcane_mct-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 arcane_mct-1.2.2/PKG-INFO
```

### Comparing `arcane-mct-1.2.1/arcane/mct.py` & `arcane_mct-1.2.2/arcane/mct.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class MerchantCenterServiceDownException(Exception):
     """Raised when we cannot access to MCC service """
     pass
 
 
 def get_exception_message(merchant_id: int, access_token: Optional[str] = None) -> str:
     if access_token:
-        return F"We cannot access your Merchant Center account with the id: {merchant_id}. Are you sure you have access and entered correct ID?"
+        return F"It seems that you do not have direct access to the account with: {merchant_id}. You, as as well as our email, need to have direct access to the account to link it"
     else:
         return F"We cannot access your Merchant Center account with the id: {merchant_id} from the Arcane account. Are you sure you granted access and gave the correct ID?"
 
 
 def get_mct_service(
     adscale_key: Optional[str] = None,
     access_token: Optional[str] = None,
```

### Comparing `arcane-mct-1.2.1/PKG-INFO` & `arcane_mct-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: arcane-mct
-Version: 1.2.1
+Version: 1.2.2
 Summary: Package description
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arcane-core (>=1.6.0,<2.0.0)
 Requires-Dist: backoff (>=1.10.0,<2.0.0)
 Requires-Dist: google-api-python-client (>=1.7.8)
 Requires-Dist: google-auth-httplib2 (==0.1.0)
 Description-Content-Type: text/markdown
 
 # Arcane mct
```

