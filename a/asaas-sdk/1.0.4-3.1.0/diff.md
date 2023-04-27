# Comparing `tmp/asaas-sdk-1.0.4.tar.gz` & `tmp/asaas-sdk-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaas-sdk-1.0.4.tar", last modified: Wed Apr 26 06:02:13 2023, max compression
+gzip compressed data, was "asaas-sdk-3.1.0.tar", last modified: Thu Apr 27 02:24:53 2023, max compression
```

## Comparing `asaas-sdk-1.0.4.tar` & `asaas-sdk-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 06:02:13.335963 asaas-sdk-1.0.4/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-1.0.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-26 06:02:13.332630 asaas-sdk-1.0.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-20 02:28:32.000000 asaas-sdk-1.0.4/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 06:02:13.332630 asaas-sdk-1.0.4/asaas/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13104 2023-04-26 06:01:35.000000 asaas-sdk-1.0.4/asaas/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-26 05:13:01.000000 asaas-sdk-1.0.4/asaas/customers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      107 2023-04-19 02:53:26.000000 asaas-sdk-1.0.4/asaas/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-26 05:29:32.000000 asaas-sdk-1.0.4/asaas/payments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-19 23:28:03.000000 asaas-sdk-1.0.4/asaas/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-26 06:02:13.332630 asaas-sdk-1.0.4/asaas_sdk.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-26 06:02:13.000000 asaas-sdk-1.0.4/asaas_sdk.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-26 06:02:01.000000 asaas-sdk-1.0.4/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-26 06:02:13.335963 asaas-sdk-1.0.4/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-3.1.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/asaas/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12817 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/customers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1649 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/payments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/asaas_sdk.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-27 02:24:20.000000 asaas-sdk-3.1.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/setup.cfg
```

### Comparing `asaas-sdk-1.0.4/LICENSE` & `asaas-sdk-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.4/PKG-INFO` & `asaas-sdk-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaas-sdk
-Version: 1.0.4
+Version: 3.1.0
 Summary:  Biblioteca não oficial de comunicação com a API de pagamento do ASAAS
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/asaas-sdk
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/asaas-sdk/issues
 Keywords: asaas,sdk,payment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asaas-sdk-1.0.4/README.md` & `asaas-sdk-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.4/asaas/__init__.py` & `asaas-sdk-3.1.0/asaas/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import date
 
 from asaas.customers import Customer
 
 from asaas import payments
 from asaas.payments import Payment
 
-from asaas.exceptions import ErroAsaas
+from asaas.exceptions import raise_for_error
 
 class Asaas():
     def __init__(self, access_token, production = False):
 
         self.access_token = access_token
 
         if production:
@@ -37,35 +37,27 @@
 
         response = self.session.get(
             url     = urljoin(self.url, endpoint),
             headers = self.default_headers,
             params  = params
         )
 
-        try:
-            response.raise_for_status()
-        except HTTPError as e:
-            if 'errors' in response.json():
-                raise ErroAsaas(response.json())
+        raise_for_error(response)
 
         return response.json()
     
-    def post(self, endpoint: str, json: Optional[dict] = None) -> dict:
+    def post(self, endpoint: str, json: dict) -> dict:
 
         response = self.session.post(
             url     = urljoin(self.url, endpoint),
             headers = self.default_headers,
             json    = json
         )
 
-        try:
-            response.raise_for_status()
-        except HTTPError as e:
-            if 'errors' in response.json():
-                raise ErroAsaas(response.json())
+        raise_for_error(response)        
 
         return response.json()
 
 class Customers():
     
     def __init__(self, asaas: Asaas) -> None:
         
@@ -347,27 +339,26 @@
 
     load_dotenv()
 
     acess_token = os.getenv('acess_token')
 
     asaas = Asaas(acess_token, production = False)
 
-    roberto = asaas.customers.get('cus_000005267821')
-
-    exit()
+    roberto = asaas.customers.get('cus_00000526a7821')
 
     pagamento = asaas.payments.new(
         customer = roberto,
         billingType = payments.BillingType.CREDIT_CARD,
         value = 100,
         dueDate = date.today(),
         creditCard = payments.CreditCard(
             holderName = 'marcelo h almeida',
-            number = '5162306219378829',
-            expiryYear = '2024', expiryMonth = '05',
+            number = '5184019740373151',
+            expiryYear = '2024', 
+            expiryMonth = '05',
             ccv = '318'
         ).json(),
         creditCardHolderInfo = payments.CreditCardHolderInfo(
             name = 'Marcelo Henrique Almeida',
             email = 'marcelo.almeida@gmail.com',
             cpfCnpj = '24971563792',
             postalCode = '89223-005',
```

### Comparing `asaas-sdk-1.0.4/asaas/customers.py` & `asaas-sdk-3.1.0/asaas/customers.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.4/asaas/payments.py` & `asaas-sdk-3.1.0/asaas/payments.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-1.0.4/asaas_sdk.egg-info/PKG-INFO` & `asaas-sdk-3.1.0/asaas_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaas-sdk
-Version: 1.0.4
+Version: 3.1.0
 Summary:  Biblioteca não oficial de comunicação com a API de pagamento do ASAAS
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/asaas-sdk
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/asaas-sdk/issues
 Keywords: asaas,sdk,payment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asaas-sdk-1.0.4/pyproject.toml` & `asaas-sdk-3.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asaas-sdk"
-version = "1.0.4"
+version = "3.1.0"
 authors = [
   { name="Gabriel Niziolek", email="ganiziolek@gmail.com" },
 ]
 description = " Biblioteca não oficial de comunicação com a API de pagamento do ASAAS"
 keywords = ["asaas", "sdk", "payment"]
 readme = "README.md"
 requires-python = ">=3.10"
```

