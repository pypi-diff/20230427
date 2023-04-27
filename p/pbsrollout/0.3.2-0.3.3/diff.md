# Comparing `tmp/pbsrollout-0.3.2.tar.gz` & `tmp/pbsrollout-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.2.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.3.tar", max compression
```

## Comparing `pbsrollout-0.3.2.tar` & `pbsrollout-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.2/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.2/pbsrollout/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.2/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1231 2023-04-13 22:21:13.072224 pbsrollout-0.3.2/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.2/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.2/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.2/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.2/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.2/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.2/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.3.2/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     4667 2023-04-17 22:04:49.560368 pbsrollout-0.3.2/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.2/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.2/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.2/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     5927 2023-04-25 16:48:05.489162 pbsrollout-0.3.2/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      522 2023-04-25 16:49:47.310209 pbsrollout-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.3/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.3/pbsrollout/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.3/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1226 2023-04-26 23:46:43.633234 pbsrollout-0.3.3/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.3/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.3/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.3/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.3/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.3/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.3/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      151 2023-04-27 00:11:18.343944 pbsrollout-0.3.3/pbsrollout/internal/test_utils.py
+-rw-r--r--   0        0        0      897 2023-04-27 00:00:07.330017 pbsrollout-0.3.3/pbsrollout/internal/test_utils_gh.py
+-rw-r--r--   0        0        0     1155 2023-04-27 00:11:35.911708 pbsrollout-0.3.3/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     2113 2023-04-26 23:47:48.220667 pbsrollout-0.3.3/pbsrollout/internal/utils_gh.py
+-rw-r--r--   0        0        0     4717 2023-04-27 00:11:53.981674 pbsrollout-0.3.3/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.3/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.3/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.3/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     6867 2023-04-26 23:59:13.659375 pbsrollout-0.3.3/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      522 2023-04-27 00:12:37.144093 pbsrollout-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.3/PKG-INFO
```

### Comparing `pbsrollout-0.3.2/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.3/pbsrollout/internal/aws_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 
 def get_ecr_images(repository: str) -> List[str]:
     # see: https://stackoverflow.com/questions/70533690/boto3-how-to-get-newest-docker-image-from-ecr
 
     # query to sort by newest
     # jmespath_expression = 'Images[?CreationDate>`2022-04-01`]'
-    jmespath_expression = "reverse(sort_by(imageDetails,&to_string(imagePushedAt)))[:10].imageTags[0]"
+    jmespath_expression = "reverse(sort_by(imageDetails,&to_string(imagePushedAt)))[:40].imageTags[0]"
     # jmespath_expression = "reverse(sort_by(imageDetails,&to_string(imagePushedAt)))[:15].imageTags[0]"
 
     client = get_ecr_client()
     paginator = client.get_paginator('describe_images')
     # We need big page size because the result will be sent per page.
     # So if page size is 100, and we return the last 15 items [:15], then we will have 15 items per batch of 100 results!
     iterator = paginator.paginate(repositoryName=repository, registryId='689975898194', PaginationConfig={'PageSize': 1000})
     filter_iterator = iterator.search(jmespath_expression)
-    return sorted(list(filter_iterator), reverse=True)[:10]
+    return sorted(list(filter_iterator), reverse=True)
```

### Comparing `pbsrollout-0.3.2/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.3/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.2/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.3/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.2/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.3/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.2/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.3/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.2/pbsrollout/internal/utils.py` & `pbsrollout-0.3.3/pbsrollout/internal/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,7 +39,16 @@
         import requests
 
         package = 'pbsrollout'
         response = requests.get(f'https://pypi.org/pypi/{package}/json')
         return response.json()['info']['version']
     except:
         return ""
+
+
+def is_dev() -> bool:
+    from os import getenv
+    if getenv('DEV', '').lower() == 'true':
+        return True
+    import pathlib
+    ret = pathlib.Path(__file__).parent.resolve()
+    return 'pbsrollout/pbsrollout' in str(ret)
```

### Comparing `pbsrollout-0.3.2/pbsrollout/main.py` & `pbsrollout-0.3.3/pbsrollout/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import os
 import sys
 from subprocess import TimeoutExpired
 
 from botocore.exceptions import ClientError
 from kubernetes.client import ApiException
 from rich.console import Console
 from rich.markdown import Markdown
 from simple_term_menu import TerminalMenu
 
-from pbsrollout.internal.utils import notify, get_latest_version
+from pbsrollout.internal.utils import notify, get_latest_version, is_dev
 
 VERSION = ""
 try:
     import importlib.metadata
 
     VERSION = importlib.metadata.version("pbsrollout")
 except:
@@ -31,14 +32,16 @@
     """
 
     md = Markdown(mk)
     console.print(md)
 
 
 def check_latest_version(console: Console):
+    if is_dev():
+        return
     latest_version = get_latest_version()
     if latest_version != "":
         if latest_version != VERSION:
             terminal_menu = TerminalMenu(["[y] yes", "[n] It's okay I want to keep an outdated version"],
                                          title=f"You pbsrollout version is outdated!\n- Current version: {VERSION}\n- Latest version: {latest_version}\nDo you want to update?",
                                          raise_error_on_interrupt=True)
             menu_entry_index = terminal_menu.show()
```

### Comparing `pbsrollout-0.3.2/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.3/pbsrollout/pbs_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.2/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.3/pbsrollout/stg_release/main_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import subprocess
+from copy import copy
 from typing import Tuple, Callable, List, Any
 
 from rich.console import Console
 from shellpython.helpers import Dir
 from simple_term_menu import TerminalMenu
 
 from pbsrollout.internal.aws_utils import get_ecr_images
 from pbsrollout.internal.utils import clean_stderr, print_error_body
+from pbsrollout.internal.utils_gh import get_pr_titles_and_author_from_commit_hash, does_gh_cli_exist
 
 NB_STAGINGS = 20
 
-
 def get_and_enforce_go_path(console: Console) -> str:
     # Let's enforce having a gopath
     if 'GOPATH' not in os.environ or os.environ['GOPATH'] == '':
         console.print('GOPATH should be set in your environ! Contact a publica engineer for help')
         raise RuntimeError('GOPATH should be set in your environ! Contact a publica engineer for help')
     return os.environ['GOPATH']
 
@@ -45,22 +46,48 @@
 
     return True
 
 
 def release_staging(console: Console, stg_idx: List[str], go_path: str):
     # step 1: choose and write tags for .tag files
     # load tags
+
+    gh_cli_exist = does_gh_cli_exist()
+    if not gh_cli_exist:
+        console.print('[bold gold1]you should install the gh cli to add more informations about the tags!\n[italic]brew install gh[/italic][/bold gold1]')
+
     with console.status("[bold green]Fetching tags for 'pbs'...") as status:
-        images = get_ecr_images('pbs')[:20]
+        images = get_ecr_images('pbs')
+        full_img = copy(images)
+        images = [x[17:] for x in images]
+
+        # enrich tags with github data
+
+        # let's only display tags with open PR!
+        github_infos = []
+        if gh_cli_exist:
+            github_infos = get_pr_titles_and_author_from_commit_hash(images)
+
+            enriched_data = []
+            for g in github_infos:
+                for idx, tag in enumerate(images):
+                    if g[2] == tag:
+                        enriched_data.append(f'{tag} {g[0]} = {g[1]}')
+            if len(enriched_data) > 0:
+                images = enriched_data
 
     # choose image
-    terminal_menu = TerminalMenu([o[17:] + " - " + o[:16] for o in images], title="Select tag:",
+    terminal_menu = TerminalMenu(images, title="Select tag:",
                                  raise_error_on_interrupt=True)
     menu_entry_index = terminal_menu.show()
     tag = images[menu_entry_index]
+    for f in full_img:
+        if f.endswith(tag[:len('cd1ef6b73')]):
+            tag = f
+            break
 
     # put it in the file
     dir_path = go_path + '/src/github.com/publica-project/prebid-kube-manifests/namespace/stg/'
     for stg in stg_idx:
         console.print(f"Updating tag to [bold blue_violet]{tag}[/bold blue_violet] in file:")
         for pod in ['pbs', 'logger', 'console-api']:
             tag_file_path = dir_path + f"z{stg}-{pod}.tag"
@@ -82,29 +109,29 @@
 def migrate_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
         dir_path = go_path + '/src/github.com/publica-project/prebid-kube-manifests/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tMigrating staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/migrate-staging-db {stg.lstrip('0')}"
-            ret = subprocess.run(cmd.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=90)
+            ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=200)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
                 print_error_body(f"ERROR:\n\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
                 return False
 
 
 def sync_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
         dir_path = go_path + '/src/github.com/publica-project/prebid-kube-manifests/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tSyncing staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/sync-staging-db {stg.lstrip('0')}"
-            ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=90)
+            ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=200)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
                 print_error_body(f"ERROR:\n\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
                 return False
 
 
 def choose_another_staging_idx(console: Console, stg_idx: List[str], go_path: str) -> List[str]:
@@ -126,14 +153,13 @@
     stg_idx = choose_staging_idx(console)
     while True:
         terminal_menu = TerminalMenu([o[0] for o in actions],
                                      title=f"What do you want to do for staging: {' '.join(stg_idx)}?",
                                      raise_error_on_interrupt=True)
         menu_entry_index = terminal_menu.show()
 
-        if actions[menu_entry_index][0] == '' \
-                                           '':
+        if actions[menu_entry_index][0] == 'exit':
             return
 
         ret = actions[menu_entry_index][1](console, stg_idx, go_path)
         if actions[menu_entry_index][0] == 'choose another staging idx':
             stg_idx = ret
```

### Comparing `pbsrollout-0.3.2/pyproject.toml` & `pbsrollout-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.2/PKG-INFO` & `pbsrollout-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

