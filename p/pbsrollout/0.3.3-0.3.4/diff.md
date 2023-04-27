# Comparing `tmp/pbsrollout-0.3.3.tar.gz` & `tmp/pbsrollout-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.3.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.4.tar", max compression
```

## Comparing `pbsrollout-0.3.3.tar` & `pbsrollout-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.3/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.3/pbsrollout/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.3/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-26 23:46:43.633234 pbsrollout-0.3.3/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.3/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.3/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.3/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.3/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.3/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.3/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      151 2023-04-27 00:11:18.343944 pbsrollout-0.3.3/pbsrollout/internal/test_utils.py
--rw-r--r--   0        0        0      897 2023-04-27 00:00:07.330017 pbsrollout-0.3.3/pbsrollout/internal/test_utils_gh.py
--rw-r--r--   0        0        0     1155 2023-04-27 00:11:35.911708 pbsrollout-0.3.3/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     2113 2023-04-26 23:47:48.220667 pbsrollout-0.3.3/pbsrollout/internal/utils_gh.py
--rw-r--r--   0        0        0     4717 2023-04-27 00:11:53.981674 pbsrollout-0.3.3/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.3/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.3/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.3/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     6867 2023-04-26 23:59:13.659375 pbsrollout-0.3.3/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      522 2023-04-27 00:12:37.144093 pbsrollout-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.4/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.4/pbsrollout/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:14:13.401261 pbsrollout-0.3.4/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1226 2023-04-27 00:14:13.401590 pbsrollout-0.3.4/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2023-04-27 00:14:13.401821 pbsrollout-0.3.4/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3733 2023-04-27 00:14:13.402052 pbsrollout-0.3.4/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0     9181 2023-04-27 00:14:13.402305 pbsrollout-0.3.4/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2023-04-27 00:14:13.402559 pbsrollout-0.3.4/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1217 2023-04-27 00:14:13.402806 pbsrollout-0.3.4/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      444 2023-04-27 00:14:13.403016 pbsrollout-0.3.4/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      151 2023-04-27 00:14:13.403246 pbsrollout-0.3.4/pbsrollout/internal/test_utils.py
+-rw-r--r--   0        0        0     1076 2023-04-27 21:20:15.861757 pbsrollout-0.3.4/pbsrollout/internal/test_utils_gh.py
+-rw-r--r--   0        0        0     1155 2023-04-27 00:14:13.403703 pbsrollout-0.3.4/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     2966 2023-04-27 21:28:28.932187 pbsrollout-0.3.4/pbsrollout/internal/utils_gh.py
+-rw-r--r--   0        0        0     5123 2023-04-27 21:38:27.099717 pbsrollout-0.3.4/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:14:13.404614 pbsrollout-0.3.4/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-27 00:14:13.404945 pbsrollout-0.3.4/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:14:13.405041 pbsrollout-0.3.4/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     7259 2023-04-27 21:29:29.119174 pbsrollout-0.3.4/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      522 2023-04-27 21:38:05.695021 pbsrollout-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.4/PKG-INFO
```

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.4/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.4/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.4/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.4/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.4/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/test_utils_gh.py` & `pbsrollout-0.3.4/pbsrollout/internal/test_utils_gh.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 class Test(TestCase):
     def test_does_gh_cli_exist(self):
         ret = does_gh_cli_exist()
         assert ret
 
     def test_get_pr_titles_and_author_from_commit_hash(self):
+        ret = get_pr_titles_and_author_from_commit_hash(['6d797938e', '0a60da612'])
+        for r in ret:
+            print(f'{r[0].ljust(18)} - {r[1]} - {r[2]}')
+        return
+
         ret = get_pr_titles_and_author_from_commit_hash('f285a46c4')
         for r in ret:
             print(f'{r[0]} - {r[1]}')
         return
         #
         # ret = get_pr_titles_and_author_from_commit_hash(['93b9fbd94', '378ca4130'])
         # for r in ret:
```

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/utils.py` & `pbsrollout-0.3.4/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/internal/utils_gh.py` & `pbsrollout-0.3.4/pbsrollout/internal/utils_gh.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,47 +12,71 @@
     try:
         ret = subprocess.run(["gh", "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=10)
         return ret.stdout is not None and 'github.com' in ret.stdout
     except Exception:
         return False
 
 
+gh_handle_to_name = {
+    'vchao-ias': 'Vern Chao',
+    'mflynn-ias': 'Melissa Flynn',
+    'eli-ias': 'Elson Li',
+    'barimoto-ias': 'Brent Arimoto',
+    'gli-ias': 'Gordon Li',
+
+}
+
 # support filtering by one or multiple hashs
 # return a list of (author, pr title, hash)
 # only return open PR! Add `-s all` to return all PR
 def get_pr_titles_and_author_from_commit_hash(hash: Union[str, List[str]]) -> List[Tuple[str, str, str]]:
-    def get_name(e):
+    def get_name(e) -> str:
         name = e['name']
         return name if name != '' else e['login']
 
+    def get_name_from_authors(from_commit, from_pr) -> str:
+        try:
+            from_commit = from_commit[0]
+            name = from_commit['name']
+            name_from_commit: str =  name if name != '' else from_commit['login']
+            name_from_pr = get_name(from_pr)
+            name =  name_from_commit if name_from_commit[0].isupper() else name_from_pr
+
+            if name in gh_handle_to_name:
+                return gh_handle_to_name[name]
+            return name
+        except:
+            return '?'
+
     if isinstance(hash, str):
         cmd = f"gh pr list -S {hash} --repo publica-project/platform --json author,title"
     else:
         cmd = 'gh pr list --repo=publica-project/platform --json=author,commits,title --search="sort:updated-desc" --limit=20'
 
-    ret = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=5, shell=True)
+    ret = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=10, shell=True)
     ret.stderr = clean_stderr(ret.stderr)
     if ret.returncode != 0 or ret.stderr != "":
         print_error_body(f"ERROR:\n\ncmd:\n{cmd}\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
         return []
 
     ret_json = json.loads(ret.stdout)
     if len(ret_json) == 0:
         return []
     if isinstance(hash, str):
         return [(get_name(ret_json[0]['author']), ret_json[0]['title'], hash)]
     else:
+        # Get name from commit! + add
         out = []
         # filter to find commit hash
         for e in ret_json:
             commits = e['commits']
             hash_found = False
-            for c in commits:
+            for c in commits[::-1]:  # sorted by date reverse -> we want to stop at the most recent one!
                 if hash_found:
                     break
                 commit_hash: str = c['oid']
                 for h in hash:
                     if commit_hash.startswith(h):
-                        out.append((get_name(e['author']), e['title'], h))
+                        out.append((get_name_from_authors(c['authors'], e['author']), e['title'], h))
                         hash_found = True
                         break
         return out
```

### Comparing `pbsrollout-0.3.3/pbsrollout/main.py` & `pbsrollout-0.3.4/pbsrollout/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,25 @@
                                          raise_error_on_interrupt=True)
             menu_entry_index = terminal_menu.show()
             if menu_entry_index == 0:
                 console.print(f"Please run: [grey66]python3 -m pip install --upgrade pbsrollout\n")
                 exit(0)
 
 
+def print_changelog(console: Console):
+    txt = """[bold gold1]What's new?[/bold gold1]
+[bold misty_rose1]Big features (v/0.3)[/bold misty_rose1]:
+- Support for [italic]staging[/italic]! You can now release/sync/migrate staging envs!
+
+[bold thistle1]Other[/bold thistle1]:
+- staging tags now includ github PR description + author
+"""
+    console.print(txt)
+
+
 def print_welcome(console: Console):
     """
     Print the welcome message.
     Message format:
 
                                           Better Rollout (v0.2.8)
     """
@@ -97,14 +108,15 @@
     # First we are going to init the Console (responsible for the display of all text elements)
     # compared to a "print", this object allow us to style text output.
     # see: https://github.com/Textualize/rich to be amazed
     console = Console()
 
     # We display the welcome message
     print_welcome(console)
+    print_changelog(console)
 
     # We parse some cli arguments.
     # The only one we accept for now is "help". Let's extend this in the future
     if 'help' in sys.argv:
         print_help(console)
     print("\n\n")
 
@@ -112,15 +124,16 @@
     try:
         check_latest_version(console)
         choose_action(console)
 
     # Here we process any possible exception. We use a different print depending on them.
     except Exception as e:
         notify("Error during script!", "PBS Rollout", sound=True)
-        if (isinstance(e, ApiException) and e.reason == 'Unauthorized') or (isinstance(e, ClientError) and 'ExpiredTokenException' in str(e)):
+        if (isinstance(e, ApiException) and e.reason == 'Unauthorized') or (
+                isinstance(e, ClientError) and 'ExpiredTokenException' in str(e)):
             console.print("[bold red]\nerror: please run `zaws_ctv_engineer` to login")
             return 1
         elif isinstance(e, RuntimeError):
             console.print(f"[bold red]\nError: {e}")
         elif isinstance(e, TimeoutExpired):
             console.print(f"[bold red]\nerror: {e}")
         else:
```

### Comparing `pbsrollout-0.3.3/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.4/pbsrollout/pbs_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.3/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.4/pbsrollout/stg_release/main_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,33 +61,42 @@
         images = [x[17:] for x in images]
 
         # enrich tags with github data
 
         # let's only display tags with open PR!
         github_infos = []
         if gh_cli_exist:
+            status.update("[bold green]Fetching github description for those tags...")
             github_infos = get_pr_titles_and_author_from_commit_hash(images)
+            biggest_name_len = 0
+            for g in github_infos:
+                biggest_name_len = max(biggest_name_len, len(g[0]))
 
             enriched_data = []
             for g in github_infos:
                 for idx, tag in enumerate(images):
                     if g[2] == tag:
-                        enriched_data.append(f'{tag} {g[0]} = {g[1]}')
+                        enriched_data.append(f'{tag}  {g[0].ljust(biggest_name_len + 4)} {g[1]}')
             if len(enriched_data) > 0:
                 images = enriched_data
 
     # choose image
+    images.append("manual input")
     terminal_menu = TerminalMenu(images, title="Select tag:",
                                  raise_error_on_interrupt=True)
     menu_entry_index = terminal_menu.show()
     tag = images[menu_entry_index]
-    for f in full_img:
-        if f.endswith(tag[:len('cd1ef6b73')]):
-            tag = f
-            break
+
+    if tag == 'manual input':
+        tag = str(input('enter your image tag: '))
+    else:
+        for f in full_img:
+            if f.endswith(tag[:len('cd1ef6b73')]):
+                tag = f
+                break
 
     # put it in the file
     dir_path = go_path + '/src/github.com/publica-project/prebid-kube-manifests/namespace/stg/'
     for stg in stg_idx:
         console.print(f"Updating tag to [bold blue_violet]{tag}[/bold blue_violet] in file:")
         for pod in ['pbs', 'logger', 'console-api']:
             tag_file_path = dir_path + f"z{stg}-{pod}.tag"
```

### Comparing `pbsrollout-0.3.3/pyproject.toml` & `pbsrollout-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.3/PKG-INFO` & `pbsrollout-0.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

