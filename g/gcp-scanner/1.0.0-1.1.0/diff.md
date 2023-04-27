# Comparing `tmp/gcp_scanner-1.0.0.tar.gz` & `tmp/gcp-scanner-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "gcp-scanner-1.1.0.tar", last modified: Thu Apr 27 20:11:41 2023, max compression
```

## Comparing `gcp_scanner-1.0.0.tar` & `gcp-scanner-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/requirements.txt
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/scanner.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/misc/gcp_scanner_logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/__main__.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/arguments.py
--rw-r--r--   0        0        0    34885 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/crawl.py
--rw-r--r--   0        0        0    14448 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/credsdb.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/models.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/src/gcp_scanner/scanner.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/LICENSE
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/README.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 gcp_scanner-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:11:41.495799 gcp-scanner-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-27 20:11:41.495799 gcp-scanner-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:11:41.495799 gcp-scanner-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:11:41.491799 gcp-scanner-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:11:41.495799 gcp-scanner-1.1.0/src/gcp_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34809 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/credsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-04-27 20:11:23.000000 gcp-scanner-1.1.0/src/gcp_scanner/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:11:41.495799 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-27 20:11:41.000000 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-27 20:11:41.000000 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:11:41.000000 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 20:11:41.000000 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 20:11:41.000000 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 20:11:41.000000 gcp-scanner-1.1.0/src/gcp_scanner.egg-info/top_level.txt
```

### Comparing `gcp_scanner-1.0.0/src/gcp_scanner/__main__.py` & `gcp-scanner-1.1.0/src/gcp_scanner/__main__.py`

 * *Files identical despite different names*

### Comparing `gcp_scanner-1.0.0/src/gcp_scanner/arguments.py` & `gcp-scanner-1.1.0/src/gcp_scanner/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,21 @@
   required_named.add_argument(
       '-o',
       '--output-dir',
       required=True,
       dest='output',
       default='scan_db',
       help='Path to output directory')
-
+  parser.add_argument(
+      '-ls',
+      '--light-scan',
+      default=False,
+      dest='light_scan',
+      action='store_true',
+      help='Return only the most important GCP resource fields in the output.')
   parser.add_argument(
       '-k',
       '--sa-key-path',
       default=None,
       dest='key_path',
       help='Path to directory with SA keys in json format')
   parser.add_argument(
@@ -117,16 +123,19 @@
       default=None,
       dest='log_file',
       help='Save logs to the path specified rather than displaying in\
  console')
 
   args: argparse.Namespace = parser.parse_args()
 
-  if not args.key_path and not args.gcloud_profile_path \
-    and not args.use_metadata and not args.access_token_files\
-    and not args.refresh_token_files:
+  if not any(
+          [args.key_path,
+           args.gcloud_profile_path,
+           args.use_metadata,
+           args.access_token_files,
+           args.refresh_token_files]):
     logging.error(
         'Please select at least one option to begin scan\
  -k/--sa-key-path,-g/--gcloud-profile-path, -m, -rt, -at'
     )
 
   return args
```

### Comparing `gcp_scanner-1.0.0/src/gcp_scanner/crawl.py` & `gcp-scanner-1.1.0/src/gcp_scanner/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,15 @@
       response = request.execute()
     except googleapiclient.errors.HttpError:
       logging.info("Failed to list buckets in the %s", project_name)
       logging.info(sys.exc_info())
       break
 
     for bucket in response.get("items", []):
-      buckets_dict[bucket["name"]] = (bucket, None)
+      buckets_dict[bucket["name"]] = bucket
       if dump_fd is not None:
         ret_fields = "nextPageToken,items(name,size,contentType,timeCreated)"
 
         req = service.objects().list(bucket=bucket["name"], fields=ret_fields)
 
         while req:
           try:
@@ -465,15 +465,16 @@
   logging.info("Retrieving list of GKE images")
   project_name = project_name.replace(":", "/")
   regions = ["", "us.", "eu.", "asia."]
   for region in regions:
     gcr_url = f"https://{region}gcr.io/v2/{project_name}/tags/list"
     try:
       res = requests.get(
-          gcr_url, auth=HTTPBasicAuth("oauth2accesstoken", access_token))
+          gcr_url, auth=HTTPBasicAuth("oauth2accesstoken", access_token),
+          timeout=120)
       if not res.ok:
         logging.info("Failed to retrieve gcr images list. Status code: %d",
                      res.status_code)
         continue
       images[region.replace(".", "")] = res.json()
     except Exception:
       logging.info("Failed to retrieve gke images for project %s", project_name)
@@ -893,15 +894,15 @@
 
   if response.get("bindings", None) is not None:
     return response["bindings"]
   else:
     return None
 
 
-def get_associated_service_accounts(
+def get_sas_for_impersonation(
     iam_policy: List[Dict[str, Any]]) -> List[str]:
   """Extract a list of unique SAs from IAM policy associated with project.
 
   Args:
     iam_policy: An IAM policy provided by get_iam_policy function.
 
   Returns:
@@ -909,24 +910,19 @@
   """
 
   if not iam_policy:
     return []
 
   list_of_sas = list()
   for entry in iam_policy:
-    for member in entry["members"]:
-      if "deleted:" in member:
-        continue
-      account_name = None
-      for element in member.split(":"):
-        if "@" in element:
-          account_name = element
-          break
-      if account_name and account_name not in list_of_sas:
-        list_of_sas.append(account_name)
+    for sa_name in entry.get("members", []):
+      if sa_name.startswith("serviceAccount") and "@" in sa_name:
+        account_name = sa_name.split(":")[1]
+        if account_name not in list_of_sas:
+          list_of_sas.append(account_name)
 
   return list_of_sas
 
 
 def get_service_accounts(project_name: str,
                          credentials: Credentials) -> List[Tuple[str, str]]:
   """Retrieve a list of service accounts managed in the project.
@@ -979,15 +975,15 @@
   serviceusage = discovery.build("serviceusage", "v1", credentials=credentials)
 
   request = serviceusage.services().list(
       parent="projects/" + project_id, pageSize=200, filter="state:ENABLED")
   try:
     while request is not None:
       response = request.execute()
-      list_of_services.append(response.get("services", None))
+      list_of_services.extend(response.get("services", []))
 
       request = serviceusage.services().list_next(
           previous_request=request, previous_response=response)
   except Exception:
     logging.info("Failed to retrieve services for project %s", project_id)
     logging.info(sys.exc_info())
 
@@ -1012,15 +1008,15 @@
   request = service.projects().repos().list(
     name="projects/" + project_id,
     pageSize=500
   )
   try:
     while request is not None:
       response = request.execute()
-      list_of_repos.append(response.get("repos", None))
+      list_of_repos.extend(response.get("repos", None))
 
       request = service.projects().repos().list_next(
         previous_request=request,
         previous_response=response
       )
   except Exception:
     logging.info("Failed to retrieve source repos for project %s", project_id)
@@ -1045,15 +1041,15 @@
   request = service.policies().list(
     project=project_id,
     maxResults=500
   )
   try:
     while request is not None:
       response = request.execute()
-      list_of_policies.append(response.get("policies", None))
+      list_of_policies.extend(response.get("policies", None))
 
       request = service.policies().list_next(
         previous_request=request,
         previous_response=response
       )
   except Exception:
     logging.info("Failed to retrieve DNS policies for project %s", project_id)
```

### Comparing `gcp_scanner-1.0.0/src/gcp_scanner/credsdb.py` & `gcp-scanner-1.1.0/src/gcp_scanner/credsdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,29 +91,29 @@
 service-accounts/default/token"
   scope_url = "http://metadata.google.internal/computeMetadata/v1/instance/\
 service-accounts/default/scopes"
   email_url = "http://metadata.google.internal/computeMetadata/v1/instance/\
 service-accounts/default/email"
   headers = {"Metadata-Flavor": "Google"}
   try:
-    res = requests.get(token_url, headers=headers)
+    res = requests.get(token_url, headers=headers, timeout=120)
     if not res.ok:
       logging.error("Failed to retrieve instance token. Status code %d",
                     res.status_code)
       return None, None
     token = res.json()["access_token"]
 
-    res = requests.get(scope_url, headers=headers)
+    res = requests.get(scope_url, headers=headers, timeout=120)
     if not res.ok:
       logging.error("Failed to retrieve instance scopes. Status code %d",
                     res.status_code)
       return None, None
     instance_scopes = res.content.decode("utf-8")
 
-    res = requests.get(email_url, headers=headers)
+    res = requests.get(email_url, headers=headers, timeout=120)
     if not res.ok:
       logging.error("Failed to retrieve instance email. Status code %d",
                     res.status_code)
       return None, None
     email = res.content.decode("utf-8")
 
   except Exception:
```

### Comparing `gcp_scanner-1.0.0/src/gcp_scanner/models.py` & `gcp-scanner-1.1.0/src/gcp_scanner/models.py`

 * *Files identical despite different names*

### Comparing `gcp_scanner-1.0.0/src/gcp_scanner/scanner.py` & `gcp-scanner-1.1.0/src/gcp_scanner/scanner.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,46 +17,101 @@
 
 """
 
 import json
 import logging
 import os
 import sys
+from pathlib import Path
+from datetime import datetime
 from typing import List, Tuple, Dict, Optional,Union
 
 from . import crawl
 from . import credsdb
 from . import arguments
 from google.cloud import container_v1
 from google.cloud import iam_credentials
 from google.cloud.iam_credentials_v1.services.iam_credentials.client import IAMCredentialsClient
 from googleapiclient import discovery
 from httplib2 import Credentials
 from .models import SpiderContext
 
+# We define the schema statically to make it easier for the user and avoid extra
+# config files.
+light_version_scan_schema = {
+  'compute_instances': ['name', 'zone', 'machineType', 'networkInterfaces',
+                        'status'],
+  'compute_images': ['name', 'status', 'diskSizeGb', 'sourceDisk'],
+  'machine_images': ['name', 'description', 'status', 'sourceInstance',
+                     'totalStorageBytes', 'savedDisks'],
+  'compute_disks': ['name', 'sizeGb', 'zone', 'status', 'sourceImage', 'users'],
+  'compute_snapshots': ['name', 'status', 'sourceDisk', 'downloadBytes'],
+  'managed_zones': ['name', 'dnsName', 'description', 'nameServers'],
+  'sql_instances': ['name', 'region', 'ipAddresses', 'databaseVersion'
+                    'state'],
+  'cloud_functions': ['name', 'eventTrigger', 'status', 'entryPoint',
+                      'serviceAccountEmail'],
+  'kms': ['name', 'primary', 'purpose', 'createTime'],
+  'services': ['name'],
+}
+
 def is_set(config: Optional[dict], config_setting: str) -> Union[dict,bool]:
   if config is None:
     return True
   obj = config.get(config_setting, {})
   return obj.get('fetch', False)
 
+def save_results(res_data: Dict, res_path: str, is_light: bool):
+  """The function to save scan results on disk in json format.
+
+  Args:
+    res_data: scan results as a dictionary of entries
+    res_path: full path to save data in file
+    is_light: save only the most interesting results
+  """
+
+  if is_light is True:
+    # returning the light version of the scan based on predefined schema
+    for gcp_resource, schema in light_version_scan_schema.items():
+      projects = res_data.get('projects', {})
+      for project_name, project_data in projects.items():
+        scan_results = project_data.get(gcp_resource, {})
+        light_results = list()
+        for scan_result in scan_results:
+          light_results.append({key: scan_result.get(key) for key in schema})
+
+        project_data.update({gcp_resource: light_results})
+        projects.update({project_name: project_data})
+      res_data.update({'projects': projects})
+
+  # Write out results to json DB
+  sa_results_data = json.dumps(res_data, indent=2, sort_keys=False)
+
+  with open(res_path, 'a', encoding='utf-8') as outfile:
+    outfile.write(sa_results_data)
+
+
 def crawl_loop(initial_sa_tuples: List[Tuple[str, Credentials, List[str]]],
                out_dir: str,
                scan_config: Dict,
+               light_scan: bool,
                target_project: Optional[str] = None,
                force_projects: Optional[str] = None):
   """The main loop function to crawl GCP resources.
 
   Args:
     initial_sa_tuples: [(sa_name, sa_object, chain_so_far)]
     out_dir: directory to save results
     target_project: project name to scan
     force_projects: a list of projects to force scan
   """
 
+  # Generate current timestamp to append to the filename
+  scan_time_suffix = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+
   context = SpiderContext(initial_sa_tuples)
   # Main loop
   processed_sas = set()
   while not context.service_account_queue.empty():
     # Get a new candidate service account / token
     sa_name, credentials, chain_so_far = context.service_account_queue.get()
     if sa_name in processed_sas:
@@ -94,17 +149,28 @@
       project_id = project['projectId']
       project_number = project['projectNumber']
       print(f'Inspecting project {project_id}')
       project_result = sa_results['projects'][project_id]
 
       project_result['project_info'] = project
 
+      # Fail with error if the output file already exists
+      output_file_name = f'{project_id}-{scan_time_suffix}.json'
+      output_path = Path(out_dir, output_file_name)
+
+      try:
+        with open(output_path, 'x', encoding='utf-8'):
+          pass
+
+      except FileExistsError:
+        logging.error('Try removing the %s file and restart the scanner.',
+                      output_file_name)
+
       if is_set(scan_config, 'iam_policy'):
         # Get IAM policy
-        iam_client = iam_client_for_credentials(credentials)
         iam_policy = crawl.get_iam_policy(project_id, credentials)
         project_result['iam_policy'] = iam_policy
 
       if is_set(scan_config, 'service_accounts'):
         # Get service accounts
         project_service_accounts = crawl.get_service_accounts(
             project_number, credentials)
@@ -209,17 +275,17 @@
             project_id, credentials)
 
       # Get Spanner Instances
       if is_set(scan_config, 'spanner_instances'):
         project_result['spanner_instances'] = crawl.get_spanner_instances(
             project_id, credentials)
 
-      # Get CloudStore Instances
-      if is_set(scan_config, 'cloudstore_instances'):
-        project_result['cloudstore_instances'] = crawl.get_filestore_instances(
+      # Get FileStore Instances
+      if is_set(scan_config, 'filestore_instances'):
+        project_result['filestore_instances'] = crawl.get_filestore_instances(
             project_id, credentials)
 
       # Get list of KMS keys
       if is_set(scan_config, 'kms'):
         project_result['kms'] = crawl.get_kms_keys(project_id, credentials)
 
       # Get information about Endpoints
@@ -235,53 +301,45 @@
       # Get list of cloud source repositories enabled in the project
       if is_set(scan_config, 'sourcerepos'):
         project_result['sourcerepos'] = crawl.list_sourcerepo(
           project_id,
           credentials
         )
 
-      # trying to impersonate SAs within project
       if scan_config is not None:
         impers = scan_config.get('service_accounts', None)
       else:
-        impers = {'impersonate': True}
+        impers = {'impersonate': False} # do not impersonate by default
+
+      # trying to impersonate SAs within project
       if impers is not None and impers.get('impersonate', False) is True:
+        iam_client = iam_client_for_credentials(credentials)
         if is_set(scan_config, 'iam_policy') is False:
           iam_policy = crawl.get_iam_policy(project_id, credentials)
 
-        project_service_accounts = crawl.get_associated_service_accounts(
-            iam_policy)
-
+        project_service_accounts = crawl.get_sas_for_impersonation(iam_policy)
         for candidate_service_account in project_service_accounts:
-          logging.info('Trying %s', candidate_service_account)
-          if not candidate_service_account.startswith('serviceAccount'):
-            continue
           try:
+            logging.info('Trying %s', candidate_service_account)
             creds_impersonated = credsdb.impersonate_sa(
                 iam_client, candidate_service_account)
             context.service_account_queue.put(
                 (candidate_service_account, creds_impersonated, updated_chain))
             project_result['service_account_edges'].append(
                 candidate_service_account)
             logging.info('Successfully impersonated %s using %s',
                          candidate_service_account, sa_name)
           except Exception:
             logging.error('Failed to get token for %s',
                                                       candidate_service_account)
             logging.error(sys.exc_info()[1])
 
-      # Write out results to json DB
       logging.info('Saving results for %s into the file', project_id)
 
-      sa_results_data = json.dumps(sa_results, indent=2, sort_keys=False)
-
-      with open(out_dir + '/%s.json' % project_id, 'a',
-                encoding='utf-8') as outfile:
-        outfile.write(sa_results_data)
-
+      save_results(sa_results, output_path, light_scan)
       # Clean memory to avoid leak for large amount projects.
       sa_results.clear()
 
 
 def iam_client_for_credentials(
     credentials: Credentials) -> IAMCredentialsClient:
   return iam_credentials.IAMCredentialsClient(credentials=credentials)
@@ -380,11 +438,10 @@
         sa_tuples.append((token_file_name, credentials, []))
 
   scan_config = None
   if args.config_path is not None:
     with open(args.config_path, 'r', encoding='utf-8') as f:
       scan_config = json.load(f)
 
-
-  crawl_loop(sa_tuples, args.output, scan_config, args.target_project,
-             force_projects_list)
+  crawl_loop(sa_tuples, args.output, scan_config, args.light_scan,
+             args.target_project, force_projects_list)
   return 0
```

### Comparing `gcp_scanner-1.0.0/LICENSE` & `gcp-scanner-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp_scanner-1.0.0/README.md` & `gcp-scanner-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ![pytests](https://github.com/google/gcp_scanner/actions/workflows/python-app.yml/badge.svg)
+[![GCP scanner version](https://img.shields.io/github/v/release/google/gcp_scanner?label=version&color=blue)](https://github.com/google/gcp_scanner/releases/latest)
 
 ### Disclaimer
 
 This project is not an official Google project. It is not supported by
 Google and Google specifically disclaims all warranties as to its quality,
 merchantability, or fitness for a particular purpose.
```

### Comparing `gcp_scanner-1.0.0/pyproject.toml` & `gcp-scanner-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=42", "wheel", "setuptools-git-versioning"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools-git-versioning]
+enabled = true
 
 [project]
 name = "gcp-scanner"
 description = "GCP resource scanner that can help determine what level of access certain credentials possess on GCP"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["gcp", "scan", "access", "security-tool", "python"]
@@ -16,15 +19,15 @@
     "pyu2f==0.1.5",
     "google-api-python-client==2.80.0",
     "google-cloud-container==2.17.4",
     "google-cloud-iam==2.11.2",
     "httplib2==0.21.0",
     "requests==2.28.2",
 ]
-version = "1.0.0"
+dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/google/gcp_scanner"
 
 [project.scripts]
 gcp-scanner = "gcp_scanner.scanner:main"
```

### Comparing `gcp_scanner-1.0.0/PKG-INFO` & `gcp-scanner-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: gcp-scanner
-Version: 1.0.0
+Version: 1.1.0
 Summary: GCP resource scanner that can help determine what level of access certain credentials possess on GCP
-Project-URL: Homepage, https://github.com/google/gcp_scanner
 License: Apache License
-License-File: LICENSE
-Keywords: access,gcp,python,scan,security-tool
+Project-URL: Homepage, https://github.com/google/gcp_scanner
+Keywords: gcp,scan,access,security-tool,python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: google-api-python-client==2.80.0
-Requires-Dist: google-cloud-container==2.17.4
-Requires-Dist: google-cloud-iam==2.11.2
-Requires-Dist: httplib2==0.21.0
-Requires-Dist: pyu2f==0.1.5
-Requires-Dist: requests==2.28.2
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![pytests](https://github.com/google/gcp_scanner/actions/workflows/python-app.yml/badge.svg)
+[![GCP scanner version](https://img.shields.io/github/v/release/google/gcp_scanner?label=version&color=blue)](https://github.com/google/gcp_scanner/releases/latest)
 
 ### Disclaimer
 
 This project is not an official Google project. It is not supported by
 Google and Google specifically disclaims all warranties as to its quality,
 merchantability, or fitness for a particular purpose.
```

