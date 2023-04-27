# Comparing `tmp/raga-cli-0.1.3.tar.gz` & `tmp/raga-cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.1.3.tar", last modified: Wed Apr 26 13:57:32 2023, max compression
+gzip compressed data, was "raga-cli-0.1.4.tar", last modified: Thu Apr 27 08:00:22 2023, max compression
```

## Comparing `raga-cli-0.1.3.tar` & `raga-cli-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.920738 raga-cli-0.1.3/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.3/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.3/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-26 13:57:32.920167 raga-cli-0.1.3/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.3/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-26 13:57:18.000000 raga-cli-0.1.3/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.913833 raga-cli-0.1.3/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-26 13:57:32.000000 raga-cli-0.1.3/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.914587 raga-cli-0.1.3/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.915845 raga-cli-0.1.3/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.3/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.3/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.3/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9804 2023-04-26 13:39:58.000000 raga-cli-0.1.3/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.917109 raga-cli-0.1.3/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.3/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.1.3/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     8399 2023-04-26 13:52:50.000000 raga-cli-0.1.3/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.917831 raga-cli-0.1.3/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5345 2023-04-26 13:51:01.000000 raga-cli-0.1.3/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.918094 raga-cli-0.1.3/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-26 13:57:32.919285 raga-cli-0.1.3/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6463 2023-04-26 13:39:34.000000 raga-cli-0.1.3/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.3/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-26 13:57:32.920833 raga-cli-0.1.3/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.3/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.925590 raga-cli-0.1.4/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.4/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.4/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-27 08:00:22.925237 raga-cli-0.1.4/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.4/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-04-27 07:59:56.000000 raga-cli-0.1.4/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.920156 raga-cli-0.1.4/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-27 08:00:22.000000 raga-cli-0.1.4/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.920757 raga-cli-0.1.4/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.921891 raga-cli-0.1.4/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.4/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.4/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.1.4/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    10165 2023-04-27 07:55:00.000000 raga-cli-0.1.4/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.922870 raga-cli-0.1.4/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.4/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-27 06:41:59.000000 raga-cli-0.1.4/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9205 2023-04-27 07:51:17.000000 raga-cli-0.1.4/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.923662 raga-cli-0.1.4/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5457 2023-04-27 07:35:31.000000 raga-cli-0.1.4/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.4/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.923914 raga-cli-0.1.4/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-27 08:00:22.924866 raga-cli-0.1.4/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6463 2023-04-26 13:39:34.000000 raga-cli-0.1.4/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.4/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-27 08:00:22.925658 raga-cli-0.1.4/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.4/setup.py
```

### Comparing `raga-cli-0.1.3/.gitignore` & `raga-cli-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/LICENSE` & `raga-cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/PKG-INFO` & `raga-cli-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.3/pyproject.toml` & `raga-cli-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.1.3/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.4/raga_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.3/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.4/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.4/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/cli/__init__.py` & `raga-cli-0.1.4/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/cli/parser.py` & `raga-cli-0.1.4/rc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/cli/utils.py` & `raga-cli-0.1.4/rc/cli/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,17 +76,21 @@
 def server_repo_commit_status(ids):
     elastic_processes = []
     for id in ids:
         elastic_processes.append(get_commit_repo(id)['check_elastic_process'])
     logger.debug("ELASTIC PROCESS {}".format(elastic_processes))
     return all(elastic_processes)
 
-def current_commit_hash():
-    result = subprocess.run('git rev-parse HEAD', capture_output=True, shell=True)    
+def current_commit_hash(cwd=None):
+    if cwd:
+        result = subprocess.run('git rev-parse HEAD', capture_output=True, shell=True, cwd=cwd)
+    else:
+        result = subprocess.run('git rev-parse HEAD', capture_output=True, shell=True)
     stdout = str(result.stdout, 'UTF-8')
+    logger.debug(f"COMMIT HASH: {stdout.strip()}")
     return stdout.strip()
 
 def current_branch():
     result = subprocess.run('git rev-parse --abbrev-ref HEAD', capture_output=True, shell=True)    
     stdout = str(result.stdout, 'UTF-8')
     return stdout.strip()
 
@@ -106,16 +110,16 @@
     if not commit_version and not repo_version:
         return True
 
     if commit_version == repo_version:
         return True
     else:
         logger.debug("Local repo version is not stable")
-        print("ERROR: Unable to upload from older version. Please use `rc get` to get the latest version and try again.")
-        sys.exit(50)
+        print("Unable to upload from older version. Please use `rc get` to get the latest version and try again.")
+        return False
 
 def get_min_cpu():
     process = 2
     cpu = cpu_count()
     if cpu>4:
         process = int(cpu/4)
     return process        
@@ -271,8 +275,14 @@
                 except ExceptionToCheck as e:
                     print(f"Got exception '{e}', retrying in {mdelay} seconds...")
                     time.sleep(mdelay)
                     mtries -= 1
                     mdelay *= backoff
             return f(*args, **kwargs)
         return f_retry
-    return deco_retry
+    return deco_retry
+
+
+def folder_exists(folder_name):
+    current_dir = os.getcwd()
+    folder_path = os.path.join(current_dir, folder_name)
+    return os.path.exists(folder_path) and os.path.isdir(folder_path)
```

### Comparing `raga-cli-0.1.3/rc/commands/get.py` & `raga-cli-0.1.4/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/commands/list.py` & `raga-cli-0.1.4/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/commands/put.py` & `raga-cli-0.1.4/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/commands/repo.py` & `raga-cli-0.1.4/rc/commands/repo.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os
 from datetime import timedelta
 import sys 
 from timeit import default_timer as timer
 import os, pwd
 
 from rc.cli.command import CmdBase
-from rc.cli.utils import run_command_on_subprocess, repo_name_valid, get_git_url
-from rc.utils.request import get_config_value_by_key, create_repository, create_repo_lock, get_repository
+from rc.cli.utils import current_commit_hash, folder_exists, run_command_on_subprocess, repo_name_valid, get_git_url
+from rc.utils.request import get_config_value_by_key, create_repository, create_repo_lock, get_repository, insert_repo_commit
 from rc.cli import RctlValidReqError, log_setup
 
 logger = logging.getLogger(__name__)
    
  
 
 """
@@ -61,19 +61,23 @@
             run_command_on_subprocess("git commit -m '{0}' -a".format("Model repo init"), repo_name)  
             run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
             run_command_on_subprocess("git push --set-upstream origin {0}".format(self.GIT_BRANCH), repo_name)    
 
     
     def create_repo(self, args):
         if self.check_git_init():
-            print("The cloning process inside the repository is not possible.")
-            sys.exit(50)
-        print("Repo creating...")   
+            print("The repo creating process inside the repository is not possible.")
+            sys.exit(50) 
         logger.debug(f"START CREATE REPO COMMAND")
-        repository_name = args.name       
+        repository_name = args.name    
+
+        if folder_exists(repository_name):
+            print("The repo creating process could not be completed because the directory already exists. Please rename repo and try again.")
+            sys.exit(50)
+        print("Repo creating...")  
         repository_tag = args.tag  
         if repository_tag not in self.TAGS:
             logger.error("'{0}' tag is not available. Please select from {1}".format(repository_tag, self.TAGS))
             sys.exit(50)                      
         self.run_repo_create_subprocesses(repository_name, repository_tag)
 
         git_repo = get_git_url(repository_name)
@@ -91,16 +95,24 @@
             req_body = json.dumps({
                 "repo_name":repository_name,
                 "tag":repository_tag,
                 "created_by":self.created_by,
                 "git_repo":git_repo.replace('\n', ''),
             })
             logger.debug(req_body)
-
+        commit_hash = current_commit_hash(repository_name)
+        request_payload = {
+                "commit_message" : "Initial commit",
+                "repo" : repository_name,
+                "commit_id":commit_hash,
+                "version":1,
+                "branch":"master"
+            }  
         create_repository(req_body)
+        insert_repo_commit(json.dumps(request_payload))
         create_repo_lock(json.dumps({"repo_name":repository_name, "user_name":self.created_by, "locked":False}))
 
         print("Repository has been created. `cd {}`".format(repository_name))    
         logger.debug(f"END CREATE REPO COMMAND")
     
     def check_git_init(self):
         current_dir = os.getcwd()
@@ -108,18 +120,23 @@
             if os.path.exists(os.path.join(current_dir, '.git')):
                 return True  # .git folder exists, so project has been initialized
             current_dir = os.path.dirname(current_dir)
         return False
 
     def clone_repo(self, args):
         if self.check_git_init():
-            print("The cloning process inside the repository is not possible.")
+            print("The repo cloning process inside the repository is not possible.")
             sys.exit(50)
         start = timer()
-        repository_name = args.name     
+        repository_name = args.name  
+
+        if folder_exists(repository_name):
+            print("The repo cloning process could not be completed because the directory already exists.")
+            sys.exit(50)
+
         print('Cloning...')
         run_command_on_subprocess("git clone git@github.com:{0}/{1}.git".format(self.GIT_ORG, repository_name), None, True)    
         tag = get_repository(repository_name)
         if tag == "dataset":
             run_command_on_subprocess("dvc pull", repository_name, True) 
         print("Repository cloned successfully")
         end = timer()
```

### Comparing `raga-cli-0.1.3/rc/exceptions.py` & `raga-cli-0.1.4/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/prompt.py` & `raga-cli-0.1.4/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/repo/get.py` & `raga-cli-0.1.4/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/repo/put.py` & `raga-cli-0.1.4/rc/repo/put.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 def dir_upload(paths):
     start = timer()
     run_command_on_subprocess("dvc push {0}".format(' '.join(paths)))
     logger.debug('DVC PUSH TIME {0}'.format(timedelta(seconds=timer()-start)))   
 
 @retry(Exception, tries=4, delay=3, backoff=2)
 def dataset_upload(paths,message,repo,current_version):
-    is_current_version_stable()   
+    if not is_current_version_stable():
+        return False   
     print("Files uploading...")   
     paths = back_slash_trim(paths)
 
     for path in paths:
         dir_add(path)
     dir_upload(paths)
     for path in paths:     
@@ -56,20 +57,18 @@
             time.sleep(pool_time)
     return True
 
 def model_upload(message, repo, model_version):
     update_repo_lock(repo, json.dumps({"locked":True}))
     print("Model files uploading...")
     commit_hash = current_commit_hash()
-    commit_hash = current_commit_hash()
     if get_commit_version(commit_hash):
         print("The latest commit is unchanged.")
         sys.exit(50)
     branchName = current_branch()
-    branchName = current_branch()
     request_payload = {
                 "commit_message" : message,
                 "repo" : repo,
                 "commit_id":commit_hash,
                 "version":model_version,
                 "branch":branchName
             }  
@@ -124,14 +123,18 @@
         http_thread = threading.Thread(target=make_repo_lock, args=(stop_event,))
         http_thread.start() 
         try:
             if dataset_upload(paths,message,repo, current_version):
                 # Set the stop event
                 stop_event.set()
                 update_repo_lock(repo, json.dumps({"locked":False}))
+            else:
+                # Set the stop event
+                stop_event.set()
+                update_repo_lock(repo, json.dumps({"locked":False}))
         except Exception as e:
             # Set the stop event
             stop_event.set()
             update_repo_lock(repo, json.dumps({"locked":False}))
             print("Something went wrong.")
             logger.exception(e)
             sys.exit()
```

### Comparing `raga-cli-0.1.3/rc/utils/__init__.py` & `raga-cli-0.1.4/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/utils/request.py` & `raga-cli-0.1.4/rc/utils/request.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.3/rc/utils/sshKeyGen.py` & `raga-cli-0.1.4/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

