# Comparing `tmp/giscemultitools-1.0.1.tar.gz` & `tmp/giscemultitools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giscemultitools-1.0.1.tar", last modified: Thu Apr 27 08:35:22 2023, max compression
+gzip compressed data, was "giscemultitools-1.0.2.tar", last modified: Thu Apr 27 09:36:05 2023, max compression
```

## Comparing `giscemultitools-1.0.1.tar` & `giscemultitools-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.838274 giscemultitools-1.0.1/giscemultitools/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/githubutils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/githubutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/scripts/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/githubutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/slackutils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools/slackutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/scripts/slack_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/giscemultitools/slackutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/giscemultitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 08:35:22.000000 giscemultitools-1.0.1/giscemultitools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:35:22.842274 giscemultitools-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 08:35:19.000000 giscemultitools-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.691651 giscemultitools-1.0.2/giscemultitools/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.691651 giscemultitools-1.0.2/giscemultitools/githubutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/giscemultitools/githubutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/scripts/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/githubutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/giscemultitools/slackutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/giscemultitools/slackutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/scripts/slack_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/giscemultitools/slackutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:36:05.691651 giscemultitools-1.0.2/giscemultitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:36:05.000000 giscemultitools-1.0.2/giscemultitools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:36:05.695651 giscemultitools-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 09:36:03.000000 giscemultitools-1.0.2/setup.py
```

### Comparing `giscemultitools-1.0.1/giscemultitools/githubutils/objects.py` & `giscemultitools-1.0.2/giscemultitools/githubutils/objects.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.1/giscemultitools/githubutils/scripts/github_cli.py` & `giscemultitools-1.0.2/giscemultitools/githubutils/scripts/github_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.1/giscemultitools/githubutils/utils.py` & `giscemultitools-1.0.2/giscemultitools/githubutils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,17 @@
         from .objects import GHAPIRequester
         from datetime import datetime
         if date_since is not None:
             date_since = datetime.strptime(date_since, '%Y-%m-%d')
         requester = GHAPIRequester(owner, repository)
         included_prs = requester.get_pulls_from_project(project_name, pr_states=('merged',), project_status=('Done',))
 
+        if not included_prs:
+            return {}
+
         changelog_data = {
             _category: {
                 _sub_category: {
                     _label: [] for _label in top_labels + ('Otras',)
                 }
                 for _sub_category in sub_categories + ('Otras',)
             } for _category in categories
@@ -139,14 +142,16 @@
                                 if not tag_classified:
                                     changelog_data[_category][_sub_category]['Otras'].append(_pr)
                         if not sub_classified:
                             changelog_data[_category]['Otras']['Otras'].append(_pr)
                 if not classified:
                     not_classified_prs.append(_pr)
 
+        # TODO show not classified
+
         # clean void sections
         for _k in list(changelog_data.keys()):
             for _sk in list(changelog_data[_k].keys()):
                 for _skl in list(changelog_data[_k][_sk].keys()):
                     if not changelog_data[_k][_sk][_skl]:
                         del changelog_data[_k][_sk][_skl]
                 if not changelog_data[_k][_sk]:
@@ -162,14 +167,17 @@
         @param changelog_data: s
         @param project_name:
         @param format: html, markdown
         @return:
         """
         from datetime import datetime
         changelog = ""
+        if not changelog_data:
+            return changelog
+
         if format == 'html':
             pass
         elif format == 'markdown':
             changelog = "# Changelog {project_name} {date_today}\n".format(
                 project_name=project_name, date_today=datetime.today().strftime('%Y-%m-%d')
             )
             for _k in changelog_data.keys():
```

### Comparing `giscemultitools-1.0.1/giscemultitools/slackutils/scripts/slack_cli.py` & `giscemultitools-1.0.2/giscemultitools/slackutils/scripts/slack_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.1/giscemultitools/slackutils/utils.py` & `giscemultitools-1.0.2/giscemultitools/slackutils/utils.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.1/giscemultitools.egg-info/SOURCES.txt` & `giscemultitools-1.0.2/giscemultitools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.0.1/setup.py` & `giscemultitools-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='giscemultitools',
     description='Llibreria d\'utilitats',
     author='GISCE',
     author_email='devel@gisce.net',
     url='http://www.gisce.net',
-    version='1.0.1',
+    version='1.0.2',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['giscemultitools'],
     install_requires=[
         "requests",
         "click"
     ],
```

