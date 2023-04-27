# Comparing `tmp/mlflow-watsonml-0.4.0.tar.gz` & `tmp/mlflow-watsonml-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-watsonml-0.4.0.tar", last modified: Wed Apr 12 17:46:18 2023, max compression
+gzip compressed data, was "mlflow-watsonml-0.5.0.tar", last modified: Thu Apr 27 17:35:42 2023, max compression
```

## Comparing `mlflow-watsonml-0.4.0.tar` & `mlflow-watsonml-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:18.651291 mlflow-watsonml-0.4.0/mlflow_watsonml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/wml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:35:42.182649 mlflow-watsonml-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-27 17:35:42.182649 mlflow-watsonml-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:35:42.178649 mlflow-watsonml-0.5.0/mlflow_watsonml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/mlflow_watsonml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/mlflow_watsonml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/mlflow_watsonml/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/mlflow_watsonml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/mlflow_watsonml/wml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:35:42.182649 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-27 17:35:42.000000 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 17:35:42.000000 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:35:42.000000 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 17:35:42.000000 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 17:35:42.000000 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 17:35:42.000000 mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:35:42.182649 mlflow-watsonml-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 17:35:30.000000 mlflow-watsonml-0.5.0/setup.py
```

### Comparing `mlflow-watsonml-0.4.0/PKG-INFO` & `mlflow-watsonml-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.4.0
+Version: 0.5.0
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.4.0/README.md` & `mlflow-watsonml-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.4.0/mlflow_watsonml/utils.py` & `mlflow-watsonml-0.5.0/mlflow_watsonml/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,7 +235,20 @@
         Software Spec, by default "runtime-22.2-py3.10"
     """
     pkg_specs = client.software_specifications.get_details(
         client.software_specifications.get_id_by_name(software_spec)
     )["entity"]["software_specification"]["software_configuration"]["included_packages"]
 
     print(tabulate(pkg_specs, headers="keys"))
+
+
+def list_endpoints(client: APIClient) -> List[Dict]:
+    endpoints = client.spaces.get_details(get_all=True)["resources"]
+    return endpoints
+
+
+def get_endpoint(client: APIClient, endpoint: str):
+    deployment_space_id = get_space_id_from_space_name(
+        client=client, space_name=endpoint
+    )
+    endpoint_details = client.spaces.get_details(space_id=deployment_space_id)
+    return endpoint_details
```

### Comparing `mlflow-watsonml-0.4.0/mlflow_watsonml/wml.py` & `mlflow-watsonml-0.5.0/mlflow_watsonml/wml.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,7 +143,23 @@
 
     except Exception as e:
         raise MlflowException(e)
 
 
 def update_model(client: APIClient):
     raise NotImplementedError()
+
+
+def set_deployment_space(client: APIClient, deployment_space_name: str) -> APIClient:
+    try:
+        space_uid = get_space_id_from_space_name(
+            client=client,
+            space_name=deployment_space_name,
+        )
+        client.set.default_space(space_uid=space_uid)
+
+    except Exception as e:
+        raise MlflowException(
+            f"Failed to set deployment space {deployment_space_name}", f"{e}"
+        )
+
+    return client
```

### Comparing `mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/PKG-INFO` & `mlflow-watsonml-0.5.0/mlflow_watsonml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.4.0
+Version: 0.5.0
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.4.0/setup.py` & `mlflow-watsonml-0.5.0/setup.py`

 * *Files identical despite different names*

