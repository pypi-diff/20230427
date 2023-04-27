# Comparing `tmp/giscemultitools-1.0.0.tar.gz` & `tmp/giscemultitools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giscemultitools-1.0.0.tar", last modified: Thu Apr 27 07:45:28 2023, max compression
+gzip compressed data, was "giscemultitools-1.0.1.tar", last modified: Thu Apr 27 08:35:22 2023, max compression
```

## Comparing `giscemultitools-1.0.0.tar` & `giscemultitools-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.474411 giscemultitools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 07:45:28.474411 giscemultitools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/githubutils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/githubutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/scripts/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/slackutils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/slackutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/scripts/slack_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:45:28.474411 giscemultitools-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.838274 giscemultitools-1.0.1/giscemultitools/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/githubutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/githubutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/scripts/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/slackutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/slackutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/scripts/slack_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/setup.py
```

### Comparing `giscemultitools-1.0.0/giscemultitools/githubutils/objects.py` & `giscemultitools-1.0.1/giscemultitools/githubutils/objects.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.0/giscemultitools/githubutils/scripts/github_cli.py` & `giscemultitools-1.0.1/giscemultitools/githubutils/scripts/github_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 @click.option('--owner', help='GitHub owner name', default='gisce', show_default=True)
 @click.option('--repository', help='GitHub repository name', default='erp', show_default=True)
 @click.option("--project-pattern", help="Project name pattern", required=True, type=click.STRING)
 @click.option("--only-one", help="To get only one result", default=False, type=click.BOOL, is_flag=True)
 def project_by_name(owner, repository, project_pattern, only_one):
     from giscemultitools.githubutils.objects import GHAPIRequester
     res = GHAPIRequester(owner, repository).get_project_info_from_project_name(project_pattern, only_one=only_one)
-    print(res)
+    print(dumps(res))
 
 
 github_cli.add_command(get_commits_sha_from_merge_commit)
 github_cli.add_command(update_projectv2_card_from_id)
 github_cli.add_command(get_pullrequest_info)
 github_cli.add_command(project_changelog)
 github_cli.add_command(project_by_name)
```

### Comparing `giscemultitools-1.0.0/giscemultitools/githubutils/utils.py` & `giscemultitools-1.0.1/giscemultitools/githubutils/utils.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.0/giscemultitools/slackutils/scripts/slack_cli.py` & `giscemultitools-1.0.1/giscemultitools/slackutils/scripts/slack_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.0/giscemultitools/slackutils/utils.py` & `giscemultitools-1.0.1/giscemultitools/slackutils/utils.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.0/giscemultitools.egg-info/SOURCES.txt` & `giscemultitools-1.0.1/giscemultitools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.0/setup.py` & `giscemultitools-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='giscemultitools',
     description='Llibreria d\'utilitats',
     author='GISCE',
     author_email='devel@gisce.net',
     url='http://www.gisce.net',
-    version='1.0.0',
+    version='1.0.1',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['giscemultitools'],
     install_requires=[
         "requests",
         "click"
     ],
```

