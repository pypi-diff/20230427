# Comparing `tmp/nci_cidc_cli-0.10.2.tar.gz` & `tmp/nci_cidc_cli-0.10.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-sl6dtw1p/nci_cidc_cli-0.10.2.tar", last modified: Thu Apr 20 18:43:09 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-shnc8uzy/nci_cidc_cli-0.10.2rc0.tar", last modified: Thu Apr 27 20:26:32 2023, max compression
```

## Comparing `nci_cidc_cli-0.10.2.tar` & `nci_cidc_cli-0.10.2rc0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/consent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/cli/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/dbedit/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/dbedit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/dbedit/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/dbedit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/dbedit/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/cli/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:09.000000 nci_cidc_cli-0.10.2/tests/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/dbedit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/dbedit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/dbedit/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57247 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/dbedit/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 18:43:00.000000 nci_cidc_cli-0.10.2/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/consent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57247 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/util.py
```

### Comparing `nci_cidc_cli-0.10.2/LICENSE` & `nci_cidc_cli-0.10.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/PKG-INFO` & `nci_cidc_cli-0.10.2rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_cli
-Version: 0.10.2
+Version: 0.10.2rc0
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.2/README.md` & `nci_cidc_cli-0.10.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/api.py` & `nci_cidc_cli-0.10.2rc0/cli/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,20 @@
 def retry_with_reauth(api_request):
     """
     For a function `api_request` that returns a `Response` object, if that response
     has status code 403, prompt the user to enter a fresh ID token from the portal,
     and retry the request.
     """
 
-    TOKEN_URL = f'https://{"staging" if get_env() != "prod" else ""}portal.cimac-network.org/assays/cli-instructions'
+    urls = {
+        "prod": "https://portal.cimac-network.org/assays/cli-instructions",
+        "staging": "https://stagingportal.cimac-network.org/assays/cli-instructions",
+        "dev-int": "https://cidc-dev.nci.nih.gov/assays/cli-instructions",
+    }
+    TOKEN_URL = urls[get_env()]
 
     @wraps(api_request)
     def wrapped(*args, **kwargs):
         retry = True
         while retry:
             res = api_request(*args, **kwargs)
             # If the error isn't auth-related, break out of the retry loop.
```

### Comparing `nci_cidc_cli-0.10.2/cli/auth.py` & `nci_cidc_cli-0.10.2rc0/cli/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/cache.py` & `nci_cidc_cli-0.10.2rc0/cli/cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/cli.py` & `nci_cidc_cli-0.10.2rc0/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 def config_():
     """Manage CLI configuration."""
 
 
 #### $ cidc config set-env ####
 @click.command()
 @click.argument(
-    "environment", required=True, type=click.Choice(["prod", "staging", "dev"])
+    "environment",
+    required=True,
+    type=click.Choice(["prod", "staging", "dev-int", "dev"]),
 )
 def set_env(environment):
     """Set the CLI environment."""
     config.set_env(environment)
     click.echo(f"Updated CLI environment to {environment}")
```

### Comparing `nci_cidc_cli-0.10.2/cli/config.py` & `nci_cidc_cli-0.10.2rc0/cli/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,11 +69,13 @@
 
 # Environment-specific config
 _current_env = get_env()
 if _current_env == "prod":
     API_V2_URL = "https://api.cimac-network.org"
 elif _current_env == "staging":
     API_V2_URL = "https://staging-api.cimac-network.org"
+elif _current_env == "dev-int":
+    API_V2_URL = "https://nih-nci-cimac-cidc-dpline-dev.uk.r.appspot.com"
 elif _current_env == "dev":
     API_V2_URL = "http://localhost:8000"
 else:
     raise ValueError(f"Unsupported environment: {_current_env}")
```

### Comparing `nci_cidc_cli-0.10.2/cli/consent.py` & `nci_cidc_cli-0.10.2rc0/cli/consent.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/dbedit/cli.py` & `nci_cidc_cli-0.10.2rc0/cli/dbedit/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/dbedit/core.py` & `nci_cidc_cli-0.10.2rc0/cli/dbedit/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,41 +24,48 @@
     uses ENV as set by $ cidc config set-env
     defaults to staging unless `prod` is specified ie no `dev` mode
 
     If not already loaded, will ask for your database username
     Asks for database password every time as to not store it
     """
     ENV: str = get_env()
-    if ENV not in ["prod", "staging"]:
-        print("unknown ENV, applying to staging:", ENV)
-        ENV: str = "staging"
+    # TODO: support dev environment running database locally
+    if ENV not in ["prod", "staging", "dev-int"]:
+        print("unknown ENV, applying to dev-int:", ENV)
+        ENV: str = "dev-int"
 
     username: Optional[str] = get_username()
     if not username:
         username = input("Username: ")
         set_username(username)
 
     password = getpass.getpass()
-    connection_name = (
-        "cidc-dfci:us-east1:cidc-postgresql-prod"
-        if ENV == "prod"
-        else "cidc-dfci-staging:us-central1:cidc-postgresql-staging"
-    )
+    connections = {
+        "prod": "cidc-dfci:us-east1:cidc-postgresql-prod",
+        "staging": "cidc-dfci-staging:us-central1:cidc-postgresql-staging",
+        "dev-int": "nih-nci-cimac-cidc-dpline-dev:us-east4:cidc-postgresql-cidc-dev2",
+    }
+    connection_name = connections[ENV]
 
     # initialize Connector object
     connector = Connector()
 
     # function to return the database connection
     def getconn():
+        databases = {
+            "prod": "cidc-prod",
+            "staging": "cidc-staging",
+            "dev-int": "cidc-cidc-dev2",
+        }
         conn = connector.connect(
             connection_name,
             "pg8000",
             user=username,
             password=password,
-            db="cidc-" + ("prod" if ENV == "prod" else "staging"),
+            db=databases[ENV],
         )
         return conn
 
     Base = automap_base()
     engine = sqlalchemy.create_engine("postgresql+pg8000://", creator=getconn)
 
     global Session
```

### Comparing `nci_cidc_cli-0.10.2/cli/dbedit/list.py` & `nci_cidc_cli-0.10.2rc0/cli/dbedit/list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/dbedit/remove.py` & `nci_cidc_cli-0.10.2rc0/cli/dbedit/remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/gcloud.py` & `nci_cidc_cli-0.10.2rc0/cli/gcloud.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/cli/upload.py` & `nci_cidc_cli-0.10.2rc0/cli/upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/PKG-INFO` & `nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-cli
-Version: 0.10.2
+Version: 0.10.2rc0
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.2/nci_cidc_cli.egg-info/SOURCES.txt` & `nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/setup.py` & `nci_cidc_cli-0.10.2rc0/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/dbedit/constants.py` & `nci_cidc_cli-0.10.2rc0/tests/dbedit/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/dbedit/test_core.py` & `nci_cidc_cli-0.10.2rc0/tests/dbedit/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,35 +100,35 @@
     assert list_mod.Session is not None
     assert list_mod.TrialMetadata is not None
     assert list_mod.UploadJobs is not None
     assert list_mod.Users is not None
 
     mocks.reset_mocks()
     list_mod.reset_mock()
-    # check that it switches to staging if no ENV
+    # check that it switches to dev-int if no ENV
     monkeypatch.setattr(core, "get_env", lambda: None)
     core.connect(list_mod)
     mocks.Connector_instance.connect.assert_called_once_with(
-        "cidc-dfci-staging:us-central1:cidc-postgresql-staging",
+        "nih-nci-cimac-cidc-dpline-dev:us-east4:cidc-postgresql-cidc-dev2",
         "pg8000",
         user=TEST_USER,
         password=TEST_PASSWORD,
-        db="cidc-staging",
+        db="cidc-cidc-dev2",
     )
     mocks.reset_mocks()
     list_mod.reset_mock()
-    # check that it switches to staging if weird ENV
+    # check that it switches to dev-int if weird ENV
     monkeypatch.setattr(core, "get_env", lambda: "foo")
     core.connect(list_mod)
     mocks.Connector_instance.connect.assert_called_once_with(
-        "cidc-dfci-staging:us-central1:cidc-postgresql-staging",
+        "nih-nci-cimac-cidc-dpline-dev:us-east4:cidc-postgresql-cidc-dev2",
         "pg8000",
         user=TEST_USER,
         password=TEST_PASSWORD,
-        db="cidc-staging",
+        db="cidc-cidc-dev2",
     )
 
 
 def test_get_clinical_downloadable_files(monkeypatch):
     monkeypatch.setattr(core, "get_env", lambda: "dev")
     DownloadableFiles = MagicMock()
     monkeypatch.setattr(core, "DownloadableFiles", DownloadableFiles)
```

### Comparing `nci_cidc_cli-0.10.2/tests/dbedit/test_list.py` & `nci_cidc_cli-0.10.2rc0/tests/dbedit/test_list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/dbedit/test_remove.py` & `nci_cidc_cli-0.10.2rc0/tests/dbedit/test_remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/test_api.py` & `nci_cidc_cli-0.10.2rc0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/test_auth.py` & `nci_cidc_cli-0.10.2rc0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/test_cache.py` & `nci_cidc_cli-0.10.2rc0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/test_cli.py` & `nci_cidc_cli-0.10.2rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/test_upload.py` & `nci_cidc_cli-0.10.2rc0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2/tests/util.py` & `nci_cidc_cli-0.10.2rc0/tests/util.py`

 * *Files identical despite different names*

