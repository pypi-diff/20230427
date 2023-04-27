# Comparing `tmp/manifester-0.0.8.tar.gz` & `tmp/manifester-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifester-0.0.8.tar", last modified: Mon Sep 12 20:22:21 2022, max compression
+gzip compressed data, was "manifester-0.0.9.tar", last modified: Tue Oct 18 18:50:46 2022, max compression
```

## Comparing `manifester-0.0.8.tar` & `manifester-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:22:21.425030 manifester-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-12 20:22:12.000000 manifester-0.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:22:21.425030 manifester-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:22:21.425030 manifester-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-09-12 20:22:12.000000 manifester-0.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-12 20:22:12.000000 manifester-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-09-12 20:22:12.000000 manifester-0.0.8/.github/workflows/update_manifester_image.yml
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-12 20:22:12.000000 manifester-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-09-12 20:22:12.000000 manifester-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-12 20:22:12.000000 manifester-0.0.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-12 20:22:12.000000 manifester-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-09-12 20:22:21.429030 manifester-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-09-12 20:22:12.000000 manifester-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:22:21.425030 manifester-0.0.8/logs/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-12 20:22:12.000000 manifester-0.0.8/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:22:21.425030 manifester-0.0.8/manifester/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    15973 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester/manifester.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 20:22:21.425030 manifester-0.0.8/manifester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-09-12 20:22:21.000000 manifester-0.0.8/manifester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-12 20:22:21.000000 manifester-0.0.8/manifester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 20:22:21.000000 manifester-0.0.8/manifester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-12 20:22:21.000000 manifester-0.0.8/manifester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 20:22:20.000000 manifester-0.0.8/manifester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-12 20:22:21.000000 manifester-0.0.8/manifester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-12 20:22:21.000000 manifester-0.0.8/manifester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-09-12 20:22:12.000000 manifester-0.0.8/manifester_settings.yaml.example
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-09-12 20:22:21.429030 manifester-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-12 20:22:12.000000 manifester-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.781584 manifester-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-18 18:50:30.000000 manifester-0.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.777584 manifester-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.777584 manifester-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-18 18:50:30.000000 manifester-0.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-18 18:50:30.000000 manifester-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-10-18 18:50:30.000000 manifester-0.0.9/.github/workflows/update_manifester_image.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-10-18 18:50:30.000000 manifester-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-18 18:50:30.000000 manifester-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-18 18:50:30.000000 manifester-0.0.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-18 18:50:30.000000 manifester-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-10-18 18:50:46.781584 manifester-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-10-18 18:50:30.000000 manifester-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.777584 manifester-0.0.9/logs/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-18 18:50:30.000000 manifester-0.0.9/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.781584 manifester-0.0.9/manifester/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/manifester.py
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.781584 manifester-0.0.9/manifester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 18:50:45.000000 manifester-0.0.9/manifester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-10-18 18:50:46.781584 manifester-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-18 18:50:30.000000 manifester-0.0.9/setup.py
```

### Comparing `manifester-0.0.8/.github/workflows/codeql-analysis.yml` & `manifester-0.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/.github/workflows/python-publish.yml` & `manifester-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/.github/workflows/update_manifester_image.yml` & `manifester-0.0.9/.github/workflows/update_manifester_image.yml`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/.gitignore` & `manifester-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/.pre-commit-config.yaml` & `manifester-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/LICENSE` & `manifester-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/PKG-INFO` & `manifester-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifester
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manifester dynamically generates subscription manifests using the Red Hat Subscription Managament API.
 Home-page: https://github.com/SatelliteQE/manifester
 Author: Danny Synk
 Author-email: dsynk@redhat.com
 License: Apache
 Description: # Manifester
```

### Comparing `manifester-0.0.8/README.md` & `manifester-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/manifester/commands.py` & `manifester-0.0.9/manifester/commands.py`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/manifester/helpers.py` & `manifester-0.0.9/manifester/helpers.py`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/manifester/logger.py` & `manifester-0.0.9/manifester/logger.py`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/manifester/manifester.py` & `manifester-0.0.9/manifester/manifester.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,24 @@
             "invalid version" in self.allocation['error'].values()):
             raise ValueError(
                                 f"{self.sat_version} is not a valid version number."
                                 "Versions must be in the form of \"sat-X.Y\". Current"
                                 f"valid versions are {self.valid_sat_versions}."
                             )
         self.allocation_uuid = self.allocation["body"]["uuid"]
+        if self.simple_content_access == "disabled":
+            simple_retry(
+                requests.put,
+                cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}"],
+                cmd_kwargs={
+                    "headers": {"Authorization": f"Bearer {self.access_token}"},
+                    "proxies": self.manifest_data.get("proxies", settings.proxies),
+                    "json": {"simpleContentAccess": "disabled"},
+                },
+            )
         logger.info(
             f"Subscription allocation created with name {self.allocation_name} "
             f"and UUID {self.allocation_uuid}"
         )
         return self.allocation_uuid
 
     def delete_subscription_allocation(self):
```

### Comparing `manifester-0.0.8/manifester/settings.py` & `manifester-0.0.9/manifester/settings.py`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/manifester.egg-info/PKG-INFO` & `manifester-0.0.9/manifester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifester
-Version: 0.0.8
+Version: 0.0.9
 Summary: Manifester dynamically generates subscription manifests using the Red Hat Subscription Managament API.
 Home-page: https://github.com/SatelliteQE/manifester
 Author: Danny Synk
 Author-email: dsynk@redhat.com
 License: Apache
 Description: # Manifester
```

### Comparing `manifester-0.0.8/manifester.egg-info/SOURCES.txt` & `manifester-0.0.9/manifester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/manifester_settings.yaml.example` & `manifester-0.0.9/manifester_settings.yaml.example`

 * *Files identical despite different names*

### Comparing `manifester-0.0.8/setup.cfg` & `manifester-0.0.9/setup.cfg`

 * *Files identical despite different names*

