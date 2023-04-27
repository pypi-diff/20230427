# Comparing `tmp/giscemultitools-0.3.4.tar.gz` & `tmp/giscemultitools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giscemultitools-0.3.4.tar", last modified: Mon Apr  3 11:39:39 2023, max compression
+gzip compressed data, was "giscemultitools-1.0.0.tar", last modified: Thu Apr 27 07:45:28 2023, max compression
```

## Comparing `giscemultitools-0.3.4.tar` & `giscemultitools-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.140196 giscemultitools-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-03 11:39:39.140196 giscemultitools-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.136196 giscemultitools-0.3.4/giscemultitools/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.136196 giscemultitools-0.3.4/giscemultitools/githubutils/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/githubutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/githubutils/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.136196 giscemultitools-0.3.4/giscemultitools/githubutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/githubutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/githubutils/scripts/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/githubutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.136196 giscemultitools-0.3.4/giscemultitools/slackutils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/slackutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.140196 giscemultitools-0.3.4/giscemultitools/slackutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/slackutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/slackutils/scripts/slack_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/giscemultitools/slackutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:39:39.136196 giscemultitools-0.3.4/giscemultitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-03 11:39:39.000000 giscemultitools-0.3.4/giscemultitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-03 11:39:39.000000 giscemultitools-0.3.4/giscemultitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:39:39.000000 giscemultitools-0.3.4/giscemultitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 11:39:39.000000 giscemultitools-0.3.4/giscemultitools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 11:39:39.000000 giscemultitools-0.3.4/giscemultitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-03 11:39:39.000000 giscemultitools-0.3.4/giscemultitools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:39:39.140196 giscemultitools-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-03 11:39:36.000000 giscemultitools-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.474411 giscemultitools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 07:45:28.474411 giscemultitools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/githubutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/githubutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/scripts/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/githubutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/slackutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools/slackutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/scripts/slack_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/giscemultitools/slackutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:45:28.470411 giscemultitools-1.0.0/giscemultitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 07:45:28.000000 giscemultitools-1.0.0/giscemultitools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:45:28.474411 giscemultitools-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 07:45:24.000000 giscemultitools-1.0.0/setup.py
```

### Comparing `giscemultitools-0.3.4/giscemultitools/githubutils/scripts/github_cli.py` & `giscemultitools-1.0.0/giscemultitools/githubutils/scripts/github_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import click
-from pprint import pprint
 from json import dumps
 
 
 @click.group()
 def github_cli():
     pass
 
@@ -37,14 +36,39 @@
 @click.option("--value", help="Text value", required=True, type=click.STRING)
 def update_projectv2_card_from_id(owner, repository, project_id, item_id, field_id, value):
     from giscemultitools.githubutils.utils import GithubUtils
     res = GithubUtils.update_projectv2_item_field_value(owner, repository, project_id, item_id, field_id, value)
     print(dumps(res))
 
 
+@click.command('project-changelog')
+@click.option('--owner', help='GitHub owner name', default='gisce', show_default=True)
+@click.option('--repository', help='GitHub repository name', default='erp', show_default=True)
+@click.option("--project-name", help="Project ID", required=True, type=click.STRING)
+@click.option('--date-since', help='Change log date from ex. 2022-12-27', default=None, show_default=True, type=click.STRING)
+def project_changelog(owner, repository, project_name, date_since):
+    from giscemultitools.githubutils.utils import GithubUtils
+    res = GithubUtils.project_changelog(owner, repository, project_name, date_since=date_since)
+    changelog = GithubUtils.format_changelog(res, 'markdown')
+    print(changelog)
+
+
+@click.command('projects-by-name')
+@click.option('--owner', help='GitHub owner name', default='gisce', show_default=True)
+@click.option('--repository', help='GitHub repository name', default='erp', show_default=True)
+@click.option("--project-pattern", help="Project name pattern", required=True, type=click.STRING)
+@click.option("--only-one", help="To get only one result", default=False, type=click.BOOL, is_flag=True)
+def project_by_name(owner, repository, project_pattern, only_one):
+    from giscemultitools.githubutils.objects import GHAPIRequester
+    res = GHAPIRequester(owner, repository).get_project_info_from_project_name(project_pattern, only_one=only_one)
+    print(res)
+
+
 github_cli.add_command(get_commits_sha_from_merge_commit)
 github_cli.add_command(update_projectv2_card_from_id)
 github_cli.add_command(get_pullrequest_info)
+github_cli.add_command(project_changelog)
+github_cli.add_command(project_by_name)
 
 
 if __name__ == "__main__":
     github_cli()
```

### Comparing `giscemultitools-0.3.4/giscemultitools/slackutils/scripts/slack_cli.py` & `giscemultitools-1.0.0/giscemultitools/slackutils/scripts/slack_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-0.3.4/giscemultitools/slackutils/utils.py` & `giscemultitools-1.0.0/giscemultitools/slackutils/utils.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-0.3.4/giscemultitools.egg-info/SOURCES.txt` & `giscemultitools-1.0.0/giscemultitools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giscemultitools-0.3.4/setup.py` & `giscemultitools-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='giscemultitools',
     description='Llibreria d\'utilitats',
     author='GISCE',
     author_email='devel@gisce.net',
     url='http://www.gisce.net',
-    version='0.3.4',
+    version='1.0.0',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['giscemultitools'],
     install_requires=[
         "requests",
         "click"
     ],
```

