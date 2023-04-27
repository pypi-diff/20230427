# Comparing `tmp/asaas-sdk-3.1.0.tar.gz` & `tmp/asaas-sdk-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaas-sdk-3.1.0.tar", last modified: Thu Apr 27 02:24:53 2023, max compression
+gzip compressed data, was "asaas-sdk-3.1.1.tar", last modified: Thu Apr 27 03:41:59 2023, max compression
```

## Comparing `asaas-sdk-3.1.0.tar` & `asaas-sdk-3.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-3.1.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/asaas/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12817 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/customers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1649 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/payments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-27 02:23:13.000000 asaas-sdk-3.1.0/asaas/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/asaas_sdk.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-27 02:24:53.000000 asaas-sdk-3.1.0/asaas_sdk.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-27 02:24:20.000000 asaas-sdk-3.1.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-27 02:24:53.816546 asaas-sdk-3.1.0/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 03:41:59.199721 asaas-sdk-3.1.1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-18 02:04:03.000000 asaas-sdk-3.1.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 03:41:59.196388 asaas-sdk-3.1.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1745 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 03:41:59.196388 asaas-sdk-3.1.1/asaas/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12817 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1574 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/customers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1728 2023-04-27 03:41:14.000000 asaas-sdk-3.1.1/asaas/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9408 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/payments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      141 2023-04-27 02:23:13.000000 asaas-sdk-3.1.1/asaas/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-27 03:41:59.196388 asaas-sdk-3.1.1/asaas_sdk.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2376 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       55 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-27 03:41:59.000000 asaas-sdk-3.1.1/asaas_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2023-04-27 03:41:27.000000 asaas-sdk-3.1.1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-27 03:41:59.199721 asaas-sdk-3.1.1/setup.cfg
```

### Comparing `asaas-sdk-3.1.0/LICENSE` & `asaas-sdk-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.0/PKG-INFO` & `asaas-sdk-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaas-sdk
-Version: 3.1.0
+Version: 3.1.1
 Summary:  Biblioteca não oficial de comunicação com a API de pagamento do ASAAS
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/asaas-sdk
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/asaas-sdk/issues
 Keywords: asaas,sdk,payment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asaas-sdk-3.1.0/README.md` & `asaas-sdk-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.0/asaas/__init__.py` & `asaas-sdk-3.1.1/asaas/__init__.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.0/asaas/customers.py` & `asaas-sdk-3.1.1/asaas/customers.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.0/asaas/exceptions.py` & `asaas-sdk-3.1.1/asaas/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,14 +29,17 @@
             
             case 'invalid_dueDate':
                 raise InvalidDueDate(description)
 
             case 'invalid_name':
                 raise InvalidName(description)
             
+            case _:
+                raise AsaasError(description)
+            
     elif response.status_code == 404:
         raise NotFound(response.url)
     
     else:
         try:
             response.raise_for_status()
```

### Comparing `asaas-sdk-3.1.0/asaas/payments.py` & `asaas-sdk-3.1.1/asaas/payments.py`

 * *Files identical despite different names*

### Comparing `asaas-sdk-3.1.0/asaas_sdk.egg-info/PKG-INFO` & `asaas-sdk-3.1.1/asaas_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaas-sdk
-Version: 3.1.0
+Version: 3.1.1
 Summary:  Biblioteca não oficial de comunicação com a API de pagamento do ASAAS
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/asaas-sdk
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/asaas-sdk/issues
 Keywords: asaas,sdk,payment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asaas-sdk-3.1.0/pyproject.toml` & `asaas-sdk-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asaas-sdk"
-version = "3.1.0"
+version = "3.1.1"
 authors = [
   { name="Gabriel Niziolek", email="ganiziolek@gmail.com" },
 ]
 description = " Biblioteca não oficial de comunicação com a API de pagamento do ASAAS"
 keywords = ["asaas", "sdk", "payment"]
 readme = "README.md"
 requires-python = ">=3.10"
```

