# Comparing `tmp/terraform-local-0.7.tar.gz` & `tmp/terraform-local-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraform-local-0.7.tar", last modified: Tue Mar 28 12:01:41 2023, max compression
+gzip compressed data, was "terraform-local-0.8.tar", last modified: Thu Apr 27 08:56:37 2023, max compression
```

## Comparing `terraform-local-0.7.tar` & `terraform-local-0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-03-28 12:01:41.778275 terraform-local-0.7/
--rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-15 00:02:30.000000 terraform-local-0.7/LICENSE
--rw-r--r--   0 whummer    (501) staff       (20)     3002 2023-03-28 12:01:41.778353 terraform-local-0.7/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)     2286 2023-03-28 12:01:08.000000 terraform-local-0.7/README.md
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-03-28 12:01:41.776486 terraform-local-0.7/bin/
--rwxr-xr-x   0 whummer    (501) staff       (20)     7354 2023-03-28 11:59:17.000000 terraform-local-0.7/bin/tflocal
--rwxr-xr-x   0 whummer    (501) staff       (20)       37 2022-06-15 00:02:30.000000 terraform-local-0.7/bin/tflocal.bat
--rw-r--r--   0 whummer    (501) staff       (20)      884 2023-03-28 12:01:41.778684 terraform-local-0.7/setup.cfg
--rwxr-xr-x   0 whummer    (501) staff       (20)       61 2022-06-15 00:02:31.000000 terraform-local-0.7/setup.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-03-28 12:01:41.777785 terraform-local-0.7/terraform_local.egg-info/
--rw-r--r--   0 whummer    (501) staff       (20)     3002 2023-03-28 12:01:41.000000 terraform-local-0.7/terraform_local.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)      352 2023-03-28 12:01:41.000000 terraform-local-0.7/terraform_local.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2023-03-28 12:01:41.000000 terraform-local-0.7/terraform_local.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2022-08-23 10:49:00.000000 terraform-local-0.7/terraform_local.egg-info/not-zip-safe
--rw-r--r--   0 whummer    (501) staff       (20)       63 2023-03-28 12:01:41.000000 terraform-local-0.7/terraform_local.egg-info/requires.txt
--rw-r--r--   0 whummer    (501) staff       (20)        6 2023-03-28 12:01:41.000000 terraform-local-0.7/terraform_local.egg-info/top_level.txt
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-03-28 12:01:41.778184 terraform-local-0.7/tests/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2022-08-27 23:32:12.000000 terraform-local-0.7/tests/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)      228 2022-08-27 23:01:35.000000 terraform-local-0.7/tests/conftest.py
--rw-r--r--   0 whummer    (501) staff       (20)     2850 2023-03-28 11:59:17.000000 terraform-local-0.7/tests/test_apply.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.656624 terraform-local-0.8/
+-rw-r--r--   0 whummer    (501) staff       (20)    11357 2022-06-15 00:02:30.000000 terraform-local-0.8/LICENSE
+-rw-r--r--   0 whummer    (501) staff       (20)     3056 2023-04-27 08:56:37.656686 terraform-local-0.8/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)     2340 2023-04-27 08:56:05.000000 terraform-local-0.8/README.md
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.655051 terraform-local-0.8/bin/
+-rwxr-xr-x   0 whummer    (501) staff       (20)     7328 2023-04-27 08:56:05.000000 terraform-local-0.8/bin/tflocal
+-rwxr-xr-x   0 whummer    (501) staff       (20)       37 2022-06-15 00:02:30.000000 terraform-local-0.8/bin/tflocal.bat
+-rw-r--r--   0 whummer    (501) staff       (20)      884 2023-04-27 08:56:37.657021 terraform-local-0.8/setup.cfg
+-rwxr-xr-x   0 whummer    (501) staff       (20)       61 2022-06-15 00:02:31.000000 terraform-local-0.8/setup.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.655975 terraform-local-0.8/terraform_local.egg-info/
+-rw-r--r--   0 whummer    (501) staff       (20)     3056 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)      352 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/SOURCES.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/dependency_links.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2022-08-23 10:49:00.000000 terraform-local-0.8/terraform_local.egg-info/not-zip-safe
+-rw-r--r--   0 whummer    (501) staff       (20)       63 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/requires.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        6 2023-04-27 08:56:37.000000 terraform-local-0.8/terraform_local.egg-info/top_level.txt
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2023-04-27 08:56:37.656400 terraform-local-0.8/tests/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2022-08-27 23:32:12.000000 terraform-local-0.8/tests/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)      228 2022-08-27 23:01:35.000000 terraform-local-0.8/tests/conftest.py
+-rw-r--r--   0 whummer    (501) staff       (20)     2850 2023-03-28 11:59:17.000000 terraform-local-0.8/tests/test_apply.py
```

### Comparing `terraform-local-0.7/LICENSE` & `terraform-local-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `terraform-local-0.7/PKG-INFO` & `terraform-local-0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-local
-Version: 0.7
+Version: 0.8
 Summary: Thin wrapper script to run Terraform against LocalStack
 Home-page: https://github.com/localstack/terraform-local
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -52,14 +52,15 @@
 ## Usage
 
 The `tflocal` command has the same usage as the `terraform` command. For detailed usage,
 please refer to the man pages of `terraform --help`.
 
 ## Change Log
 
+* v0.8: Configure the endpoint for opensearch service
 * v0.7: Add initial support for provider aliases
 * v0.6: Fix selection of default region
 * v0.5: Make AWS region configurable, add `region` to provider config
 * v0.4: Fix using use_s3_path_style for S3_HOSTNAME=localhost; exclude `meteringmarketplace` service endpoint
 * v0.3: Fix support for -chdir=... to create providers file in target directory
 * v0.2: Add ability to specify custom endpoints; pass INT signals to subprocess
 * v0.1: Initial release
```

### Comparing `terraform-local-0.7/README.md` & `terraform-local-0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 ## Usage
 
 The `tflocal` command has the same usage as the `terraform` command. For detailed usage,
 please refer to the man pages of `terraform --help`.
 
 ## Change Log
 
+* v0.8: Configure the endpoint for opensearch service
 * v0.7: Add initial support for provider aliases
 * v0.6: Fix selection of default region
 * v0.5: Make AWS region configurable, add `region` to provider config
 * v0.4: Fix using use_s3_path_style for S3_HOSTNAME=localhost; exclude `meteringmarketplace` service endpoint
 * v0.3: Fix support for -chdir=... to create providers file in target directory
 * v0.2: Add ability to specify custom endpoints; pass INT signals to subprocess
 * v0.1: Initial release
```

### Comparing `terraform-local-0.7/bin/tflocal` & `terraform-local-0.8/bin/tflocal`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     service_replaces = {
         "apigatewaymanagementapi": "",
         "ce": "costexplorer",
         "edge": "",
         "iotdata": "",
         "iotjobsdata": "",
         "logs": "cloudwatchlogs",
-        "opensearch": "",
         "timestream": ""
     }
     # service names to be excluded (not yet available in TF)
     service_excludes = ["meteringmarketplace"]
 
     # create list of service names
     services = list(config.get_service_ports())
```

### Comparing `terraform-local-0.7/setup.cfg` & `terraform-local-0.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = terraform-local
-version = 0.7
+version = 0.8
 url = https://github.com/localstack/terraform-local
 author = LocalStack Team
 author_email = info@localstack.cloud
 description = Thin wrapper script to run Terraform against LocalStack
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
```

### Comparing `terraform-local-0.7/terraform_local.egg-info/PKG-INFO` & `terraform-local-0.8/terraform_local.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-local
-Version: 0.7
+Version: 0.8
 Summary: Thin wrapper script to run Terraform against LocalStack
 Home-page: https://github.com/localstack/terraform-local
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -52,14 +52,15 @@
 ## Usage
 
 The `tflocal` command has the same usage as the `terraform` command. For detailed usage,
 please refer to the man pages of `terraform --help`.
 
 ## Change Log
 
+* v0.8: Configure the endpoint for opensearch service
 * v0.7: Add initial support for provider aliases
 * v0.6: Fix selection of default region
 * v0.5: Make AWS region configurable, add `region` to provider config
 * v0.4: Fix using use_s3_path_style for S3_HOSTNAME=localhost; exclude `meteringmarketplace` service endpoint
 * v0.3: Fix support for -chdir=... to create providers file in target directory
 * v0.2: Add ability to specify custom endpoints; pass INT signals to subprocess
 * v0.1: Initial release
```

### Comparing `terraform-local-0.7/tests/test_apply.py` & `terraform-local-0.8/tests/test_apply.py`

 * *Files identical despite different names*

