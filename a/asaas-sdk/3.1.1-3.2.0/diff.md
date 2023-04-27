# Comparing `tmp/asaas-sdk-3.1.1.tar.gz` & `tmp/asaas-sdk-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaas-sdk-3.1.1.tar", last modified: Thu Apr 27 03:41:59 2023, max compression
+gzip compressed data, was "asaas-sdk-3.2.0.tar", last modified: Thu Apr 27 04:27:35 2023, max compression
```

## Comparing `asaas-sdk-3.1.1.tar` & `asaas-sdk-3.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 03:41:59.199721 asaas-sdk-3.1.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-3.1.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 03:41:59.196388 asaas-sdk-3.1.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 03:41:59.196388 asaas-sdk-3.1.1/asaas/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12817 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/customers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1728 2023-04-27 03:41:14.000000 asaas-sdk-3.1.1/asaas/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/payments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 03:41:59.196388 asaas-sdk-3.1.1/asaas_sdk.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-27 03:41:27.000000 asaas-sdk-3.1.1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-27 03:41:59.199721 asaas-sdk-3.1.1/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 04:27:35.029724 asaas-sdk-3.2.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-3.2.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3321 2023-04-27 04:27:35.029724 asaas-sdk-3.2.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2690 2023-04-27 04:26:04.000000 asaas-sdk-3.2.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 04:27:35.026391 asaas-sdk-3.2.0/asaas/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13084 2023-04-27 04:17:27.000000 asaas-sdk-3.2.0/asaas/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-27 02:23:13.000000 asaas-sdk-3.2.0/asaas/customers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1728 2023-04-27 03:41:14.000000 asaas-sdk-3.2.0/asaas/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-27 02:23:13.000000 asaas-sdk-3.2.0/asaas/payments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-04-27 04:26:18.000000 asaas-sdk-3.2.0/asaas/pix.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-27 02:23:13.000000 asaas-sdk-3.2.0/asaas/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 04:27:35.029724 asaas-sdk-3.2.0/asaas_sdk.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3321 2023-04-27 04:27:35.000000 asaas-sdk-3.2.0/asaas_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      299 2023-04-27 04:27:35.000000 asaas-sdk-3.2.0/asaas_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-27 04:27:35.000000 asaas-sdk-3.2.0/asaas_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-27 04:27:35.000000 asaas-sdk-3.2.0/asaas_sdk.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-27 04:27:35.000000 asaas-sdk-3.2.0/asaas_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-27 04:26:31.000000 asaas-sdk-3.2.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-27 04:27:35.029724 asaas-sdk-3.2.0/setup.cfg
```

### Comparing `asaas-sdk-3.1.1/LICENSE` & `asaas-sdk-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.1/asaas/__init__.py` & `asaas-sdk-3.2.0/asaas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from typing import List
 from requests import Session
 from requests.exceptions import HTTPError
 from urllib.parse import urljoin
 from typing import Optional
 from datetime import date
 
-from asaas.customers import Customer
 
 from asaas import payments
 from asaas.payments import Payment
+from asaas.customers import Customer
+from asaas.pix import Pix
 
 from asaas.exceptions import raise_for_error
 
 class Asaas():
     def __init__(self, access_token, production = False):
 
         self.access_token = access_token
@@ -153,21 +154,29 @@
     
     def __init__(self, asaas: Asaas) -> None:
         
         self.endpoint = 'api/v3/payments'
 
         self.asaas = asaas
 
-    def get(self, id: str) -> dict:
+    def get(self, id: str) -> Payment:
         customer = self.asaas.get(
             endpoint = self.endpoint + '/' + id
         )
 
         return Payment(**customer)
 
+    def get_pix_qr(self, id) -> Pix:
+
+        pix = self.asaas.get(
+            endpoint = f'{self.endpoint}/{id}/pixQrCode'  
+        )
+
+        return Pix(**pix)
+
     def new(self,
             customer: Customer,
             billingType: payments.BillingType,
             dueDate: date,
             value: Optional[float] = None,
             totalValue: Optional[float] = None, 
             description: Optional[str] = None,
@@ -339,14 +348,18 @@
 
     load_dotenv()
 
     acess_token = os.getenv('acess_token')
 
     asaas = Asaas(acess_token, production = False)
 
+    pix = asaas.payments.get_pix_qr('pay_6318443155441227')
+
+    exit()
+
     roberto = asaas.customers.get('cus_00000526a7821')
 
     pagamento = asaas.payments.new(
         customer = roberto,
         billingType = payments.BillingType.CREDIT_CARD,
         value = 100,
         dueDate = date.today(),
```

### Comparing `asaas-sdk-3.1.1/asaas/customers.py` & `asaas-sdk-3.2.0/asaas/customers.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.1/asaas/exceptions.py` & `asaas-sdk-3.2.0/asaas/exceptions.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.1/asaas/payments.py` & `asaas-sdk-3.2.0/asaas/payments.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.1/pyproject.toml` & `asaas-sdk-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asaas-sdk"
-version = "3.1.1"
+version = "3.2.0"
 authors = [
   { name="Gabriel Niziolek", email="ganiziolek@gmail.com" },
 ]
 description = " Biblioteca não oficial de comunicação com a API de pagamento do ASAAS"
 keywords = ["asaas", "sdk", "payment"]
 readme = "README.md"
 requires-python = ">=3.10"
```

